# Comparing `tmp/pydantic_resolve-0.5.1.tar.gz` & `tmp/pydantic_resolve-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-0.5.1.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.0.0.tar", max compression
```

## Comparing `pydantic_resolve-0.5.1.tar` & `pydantic_resolve-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-0.5.1/LICENSE
--rw-r--r--   0        0        0      444 2023-06-01 01:21:59.065240 pydantic_resolve-0.5.1/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-0.5.1/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2040 2023-06-10 09:29:05.251120 pydantic_resolve-0.5.1/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-0.5.1/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     4099 2023-06-10 23:46:22.533588 pydantic_resolve-0.5.1/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     1042 2023-06-10 23:19:01.094684 pydantic_resolve-0.5.1/pydantic_resolve/util.py
--rw-r--r--   0        0        0      942 2023-06-10 23:53:36.016152 pydantic_resolve-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    12058 2023-06-10 06:56:37.703556 pydantic_resolve-0.5.1/README.md
--rw-r--r--   0        0        0    12651 1970-01-01 00:00:00.000000 pydantic_resolve-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.0.0/LICENSE
+-rw-r--r--   0        0        0      527 2023-06-11 08:17:15.013163 pydantic_resolve-1.0.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-1.0.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2040 2023-06-10 09:29:05.251120 pydantic_resolve-1.0.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.0.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     4522 2023-06-11 08:14:37.971337 pydantic_resolve-1.0.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     1042 2023-06-10 23:19:01.094684 pydantic_resolve-1.0.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-06-11 08:22:10.679448 pydantic_resolve-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12153 2023-06-11 08:33:24.276635 pydantic_resolve-1.0.0/README.md
+-rw-r--r--   0        0        0    12694 1970-01-01 00:00:00.000000 pydantic_resolve-1.0.0/PKG-INFO
```

### Comparing `pydantic_resolve-0.5.1/LICENSE` & `pydantic_resolve-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.5.1/pydantic_resolve/core.py` & `pydantic_resolve-1.0.0/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.5.1/pydantic_resolve/resolver.py` & `pydantic_resolve-1.0.0/pydantic_resolve/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from inspect import iscoroutine
 from typing import TypeVar, Dict
 from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError, MissingAnnotationError
 from typing import Any, Callable, Optional
 from pydantic_resolve import core
 from .constant import PREFIX
 from .util import get_class_field_annotations
+from inspect import isclass
+from aiodataloader import DataLoader
 
 
 def LoaderDepend(  # noqa: N802
     dependency: Optional[Callable[..., Any]] = None 
 ) -> Any:
     return Depends(dependency=dependency)
 
@@ -43,30 +45,37 @@
                 cache_key = f'{v.default.dependency.__module__}.{v.default.dependency.__name__}'
                 cache_provider = self.ctx.get()
 
                 hit = cache_provider.get(cache_key, None)
                 if hit:
                     loader = hit
                 else:
-                    # create loader instance and pick config from 'loader_filters' param
-                    loader = v.default.dependency()
-                    filter_config_provider = self.loader_filters_ctx.get()
-                    filter_config = filter_config_provider.get(v.default.dependency, {})
-
-                    # class ExampleLoader(DataLoader):
-                    #     filtar_x: bool  <--------------- set this
-                    #
-                    #     async def batch_load_fn(self, keys):
-                    #         ....
-                    for field in get_class_field_annotations(v.default.dependency):
-                        try:
-                            value = filter_config[field]
-                            setattr(loader, field, value)
-                        except KeyError:
-                            raise LoaderFieldNotProvidedError(f'{cache_key}.{field} not found in Resolver()')
+                    # create loader instance 
+                    if isclass(v.default.dependency):
+                        loader = v.default.dependency()
+
+                        # and pick config from 'loader_filters' param, only for DataClass
+                        filter_config_provider = self.loader_filters_ctx.get()
+                        filter_config = filter_config_provider.get(v.default.dependency, {})
+
+                        # class ExampleLoader(DataLoader):
+                        #     filtar_x: bool  <--------------- set this
+                        #
+                        #     async def batch_load_fn(self, keys):
+                        #         ....
+                        for field in get_class_field_annotations(v.default.dependency):
+                            try:
+                                value = filter_config[field]
+                                setattr(loader, field, value)
+                            except KeyError:
+                                raise LoaderFieldNotProvidedError(f'{cache_key}.{field} not found in Resolver()')
+
+                    # build loader from batch_load_fn, filters config is impossible
+                    else:
+                        loader = DataLoader(batch_load_fn=v.default.dependency)
 
                     cache_provider[cache_key] = loader
                     self.ctx.set(cache_provider)
                 params[k] = loader
         return method(**params)
 
     async def resolve_obj(self, target, field):
```

### Comparing `pydantic_resolve-0.5.1/pydantic_resolve/util.py` & `pydantic_resolve-1.0.0/pydantic_resolve/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-0.5.1/pyproject.toml` & `pydantic_resolve-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "0.5.1"
+version = "1.0.0"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = "^1.10.4"
-
-# optional
-aiodataloader = { version = "^0.4.0", optional = true } 
-
-[tool.poetry.extras]
-dataloader = ['aiodataloader']
+aiodataloader = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.4.6"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.1"
-aiodataloader = "^0.4.0"
 aiosqlite = "^0.18.0"
 sqlalchemy = {extras = ["asyncio"], version = "^2.0.7"}
 pytest-asyncio = "^0.21.0"
 fastapi = "^0.96.0"
 uvicorn = "^0.22.0"
 
 [build-system]
```

### Comparing `pydantic_resolve-0.5.1/README.md` & `pydantic_resolve-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 [![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 [![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
 
+> v1.0.0 released
 
 - If you are a fan of GraphQL and want to quickly build **nested data structures** without any invasion, try it.
 - If you want to work with aiodataloader conveniently and effortlessly, try it.
 - Using pydantic-resolve with FastAPI (response_model & generating client), will greatly improve your development efficiency.
 
 ```python
 import asyncio
@@ -65,15 +66,15 @@
 - [Comparsion with common solutions](./doc/compare-en.md)
 
 ## Install
 
 ```shell
 pip install pydantic-resolve
 
-pip install "pydantic-resolve[dataloader]"  # install with aiodataloader
+pip install "pydantic-resolve[dataloader]"  # install with aiodataloader, from v1.0, aiodataloader is a default dependency, [dataloader] is removed.
 ```
 
 - use `resolve` for simple scenario,
 - use `Resolver` and `LoaderDepend` for complicated nested batch query.
 
 ```python
 from pydantic_resolve import (
```

### Comparing `pydantic_resolve-0.5.1/PKG-INFO` & `pydantic_resolve-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 0.5.1
+Version: 1.0.0
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: dataloader
-Requires-Dist: aiodataloader (>=0.4.0,<0.5.0) ; extra == "dataloader"
+Requires-Dist: aiodataloader (>=0.4.0,<0.5.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Project-URL: Repository, https://github.com/allmonday/pydantic_resolve
 Description-Content-Type: text/markdown
 
 # Pydantic-resolve
 
 [![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 [![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
 
+> v1.0.0 released
 
 - If you are a fan of GraphQL and want to quickly build **nested data structures** without any invasion, try it.
 - If you want to work with aiodataloader conveniently and effortlessly, try it.
 - Using pydantic-resolve with FastAPI (response_model & generating client), will greatly improve your development efficiency.
 
 ```python
 import asyncio
@@ -88,15 +88,15 @@
 - [Comparsion with common solutions](./doc/compare-en.md)
 
 ## Install
 
 ```shell
 pip install pydantic-resolve
 
-pip install "pydantic-resolve[dataloader]"  # install with aiodataloader
+pip install "pydantic-resolve[dataloader]"  # install with aiodataloader, from v1.0, aiodataloader is a default dependency, [dataloader] is removed.
 ```
 
 - use `resolve` for simple scenario,
 - use `Resolver` and `LoaderDepend` for complicated nested batch query.
 
 ```python
 from pydantic_resolve import (
```

