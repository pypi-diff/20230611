# Comparing `tmp/pydantic_resolve-0.5.0.tar.gz` & `tmp/pydantic_resolve-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-0.5.0.tar", max compression
+gzip compressed data, was "pydantic_resolve-0.5.1.tar", max compression
```

## Comparing `pydantic_resolve-0.5.0.tar` & `pydantic_resolve-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-0.5.0/LICENSE
--rw-r--r--   0        0        0      444 2023-06-01 01:21:59.065240 pydantic_resolve-0.5.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-0.5.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     1865 2023-05-31 15:35:04.725665 pydantic_resolve-0.5.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-0.5.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     3623 2023-06-01 01:23:39.577926 pydantic_resolve-0.5.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0      148 2023-06-01 01:22:31.561515 pydantic_resolve-0.5.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      942 2023-06-06 14:52:07.189931 pydantic_resolve-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    11861 2023-06-06 15:45:04.470133 pydantic_resolve-0.5.0/README.md
--rw-r--r--   0        0        0    12456 1970-01-01 00:00:00.000000 pydantic_resolve-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-0.5.1/LICENSE
+-rw-r--r--   0        0        0      444 2023-06-01 01:21:59.065240 pydantic_resolve-0.5.1/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-0.5.1/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2040 2023-06-10 09:29:05.251120 pydantic_resolve-0.5.1/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-0.5.1/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     4099 2023-06-10 23:46:22.533588 pydantic_resolve-0.5.1/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     1042 2023-06-10 23:19:01.094684 pydantic_resolve-0.5.1/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      942 2023-06-10 23:53:36.016152 pydantic_resolve-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    12058 2023-06-10 06:56:37.703556 pydantic_resolve-0.5.1/README.md
+-rw-r--r--   0        0        0    12651 1970-01-01 00:00:00.000000 pydantic_resolve-0.5.1/PKG-INFO
```

### Comparing `pydantic_resolve-0.5.0/LICENSE` & `pydantic_resolve-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.5.0/pydantic_resolve/core.py` & `pydantic_resolve-0.5.1/pydantic_resolve/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 from typing import TypeVar
 from .exceptions import ResolverTargetAttrNotFound, DataloaderDependCantBeResolved
 from .constant import PREFIX
 
 T = TypeVar("T")
 
 def is_acceptable_type(target):
+    """
+    Check whether target is Pydantic object or Dataclass object
+
+    :param target: object
+    :type target: BaseModel or Dataclass 
+    :rtype: bool
+
+    """
     return isinstance(target, BaseModel) or is_dataclass(target)
 
 def iter_over_object_resolvers(target):
     """get method starts with resolve_"""
     for k in dir(target):
         if k.startswith(PREFIX) and ismethod(target.__getattribute__(k)):
             yield k
```

### Comparing `pydantic_resolve-0.5.0/pydantic_resolve/resolver.py` & `pydantic_resolve-0.5.1/pydantic_resolve/resolver.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,50 +20,57 @@
         self, dependency: Optional[Callable[..., Any]] = None
     ):
         self.dependency = dependency
 
 T = TypeVar("T")
 
 class Resolver:
+    """
+    Entrypoint of a resolve action
+    """
     def __init__(self, loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None, ensure_type=False):
         self.ctx = contextvars.ContextVar('pydantic_resolve_internal_context', default={})
         self.loader_filters_ctx = contextvars.ContextVar('pydantic_resolve_internal_filter', default=loader_filters or {})
         self.ensure_type = ensure_type
     
     def exec_method(self, method):
         signature = inspect.signature(method)
         params = {}
 
+        # manage the creation of loader instances
         for k, v in signature.parameters.items():
             if isinstance(v.default, Depends):
-                cache_key = str(v.default.dependency.__name__)
-                cache = self.ctx.get()
+                # module.kls to avoid same kls name from different module
+                cache_key = f'{v.default.dependency.__module__}.{v.default.dependency.__name__}'
+                cache_provider = self.ctx.get()
 
-                hit = cache.get(cache_key, None)
+                hit = cache_provider.get(cache_key, None)
                 if hit:
                     loader = hit
                 else:
-                    loader_filters = self.loader_filters_ctx.get()
-                    loader_filter = loader_filters.get(v.default.dependency, {})
-
+                    # create loader instance and pick config from 'loader_filters' param
                     loader = v.default.dependency()
+                    filter_config_provider = self.loader_filters_ctx.get()
+                    filter_config = filter_config_provider.get(v.default.dependency, {})
 
-                    # validate dependency's class field existed in filter and set value 
+                    # class ExampleLoader(DataLoader):
+                    #     filtar_x: bool  <--------------- set this
+                    #
+                    #     async def batch_load_fn(self, keys):
+                    #         ....
                     for field in get_class_field_annotations(v.default.dependency):
                         try:
-                            value = loader_filter[field]
+                            value = filter_config[field]
+                            setattr(loader, field, value)
                         except KeyError:
-                            raise LoaderFieldNotProvidedError(f'{v.default.dependency.__name__}.{field} not found in Resolver()')
-                        setattr(loader, field, value)
-
-                    cache[cache_key] = loader
-                    self.ctx.set(cache)
+                            raise LoaderFieldNotProvidedError(f'{cache_key}.{field} not found in Resolver()')
 
+                    cache_provider[cache_key] = loader
+                    self.ctx.set(cache_provider)
                 params[k] = loader
-                
         return method(**params)
 
     async def resolve_obj(self, target, field):
         item = target.__getattribute__(field)
         target_attr_name = str(field).replace(PREFIX, '')
         val = self.exec_method(item)
```

### Comparing `pydantic_resolve-0.5.0/pyproject.toml` & `pydantic_resolve-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "0.5.0"
+version = "0.5.1"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-0.5.0/README.md` & `pydantic_resolve-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Pydantic-resolve
 
 [![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
+[![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
 
-- If you are a fan of GraphQL and want to quickly build **nested data structures** without any invasion, give it a try.
-- If you want to work with aiodataloader conveniently and effortlessly, give it a try.
+
+- If you are a fan of GraphQL and want to quickly build **nested data structures** without any invasion, try it.
+- If you want to work with aiodataloader conveniently and effortlessly, try it.
 - Using pydantic-resolve with FastAPI (response_model & generating client), will greatly improve your development efficiency.
 
 ```python
 import asyncio
 from random import random
 from pydantic import BaseModel
 from pydantic_resolve import resolve
```

### Comparing `pydantic_resolve-0.5.0/PKG-INFO` & `pydantic_resolve-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 0.5.0
+Version: 0.5.1
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
@@ -23,17 +23,19 @@
 
 # Pydantic-resolve
 
 [![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
+[![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
 
-- If you are a fan of GraphQL and want to quickly build **nested data structures** without any invasion, give it a try.
-- If you want to work with aiodataloader conveniently and effortlessly, give it a try.
+
+- If you are a fan of GraphQL and want to quickly build **nested data structures** without any invasion, try it.
+- If you want to work with aiodataloader conveniently and effortlessly, try it.
 - Using pydantic-resolve with FastAPI (response_model & generating client), will greatly improve your development efficiency.
 
 ```python
 import asyncio
 from random import random
 from pydantic import BaseModel
 from pydantic_resolve import resolve
```

