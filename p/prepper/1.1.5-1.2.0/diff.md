# Comparing `tmp/prepper-1.1.5.tar.gz` & `tmp/prepper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepper-1.1.5.tar", last modified: Fri Jun  9 20:50:37 2023, max compression
+gzip compressed data, was "prepper-1.2.0.tar", last modified: Sun Jun 11 21:48:10 2023, max compression
```

## Comparing `prepper-1.1.5.tar` & `prepper-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-09 20:50:27.000000 prepper-1.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 20:50:27.000000 prepper-1.1.5/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-09 20:50:27.000000 prepper-1.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-09 20:50:27.000000 prepper-1.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-09 20:50:27.000000 prepper-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:50:37.749493 prepper-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 20:50:27.000000 prepper-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/prepper/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/exportable.py
--rw-r--r--   0 runner    (1001) docker     (123)    26985 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/io_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/prepper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/tests/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-09 20:50:27.000000 prepper-1.1.5/prepper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:50:37.749493 prepper-1.1.5/prepper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 20:50:37.000000 prepper-1.1.5/prepper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-09 20:50:27.000000 prepper-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:50:37.749493 prepper-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.456364 prepper-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-11 21:48:00.000000 prepper-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-11 21:48:00.000000 prepper-1.2.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-11 21:48:00.000000 prepper-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-11 21:48:00.000000 prepper-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-11 21:48:00.000000 prepper-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-11 21:48:10.460364 prepper-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-11 21:48:00.000000 prepper-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/prepper/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/exportable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26985 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/io_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/prepper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/tests/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/prepper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-11 21:48:00.000000 prepper-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 21:48:10.460364 prepper-1.2.0/setup.cfg
```

### Comparing `prepper-1.1.5/.github/workflows/python-publish.yml` & `prepper-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/.github/workflows/python-test.yml` & `prepper-1.2.0/.github/workflows/python-test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `prepper-1.1.5/.gitignore` & `prepper-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/.pre-commit-config.yaml` & `prepper-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/LICENSE` & `prepper-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/prepper/caching.py` & `prepper-1.2.0/prepper/caching.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import functools
+from collections.abc import Callable
 from functools import update_wrapper
+from typing import Generic, overload, TYPE_CHECKING, TypeVar, Union
 
 import numpy as np
 from joblib import hash as joblib_hash
 from numpy import ndarray
+from typing_extensions import Concatenate, ParamSpec, Self
+
+if TYPE_CHECKING:
+    from .exportable import ExportableClassMixin
 
 __all__ = [
     "break_key",
     "make_cache_name",
     "cached_property",
     "local_cache",
 ]
 
 KWD_SENTINEL = "__prepper_kwd_sentinel__"
+T = TypeVar("T")  # class using the descriptor
+P = ParamSpec("P")  # parameter specs of the decorated method
+R = TypeVar("R")  # return value of the decorated method
 
 
 class _HashedSeq(list):
     """This class guarantees that hash() will be called no more than once
     per element.  This is important because the lru_cache() will hash
     the key multiple times on a cache miss.
     """
@@ -107,54 +116,85 @@
         result = user_function(instance, *args, **kwds)
         cache[fname][key] = result
         return result
 
     return wrapper
 
 
-class cached_property:
+class cached_property(Generic[T, R]):
     """A property that is only computed once per instance and then replaces
     itself with an ordinary attribute. Deleting the attribute resets the
     property. Implementation adapted from https://github.com/pydanny/cached-property
     """
 
-    def __init__(self, func):
+    func: Callable[[T], R]
+
+    def __init__(self, func: Callable[[T], R]):
         update_wrapper(self, func)
         self.func = func
 
-    def __get__(self, obj, cls):
-        if obj is None:
+    @overload
+    def __get__(self, instance: T, owner: object) -> R:
+        ...
+
+    @overload
+    def __get__(self, instance: None, owner: object) -> Self:
+        ...
+
+    def __get__(
+        self, instance: Union[T, None], owner: object
+    ) -> Union[Self, R]:
+        if instance is None:
             return self
 
         qualname = self.func.__qualname__
-        if qualname in obj.__dict__:
-            return obj.__dict__[qualname]
+        if qualname in instance.__dict__:
+            return instance.__dict__[qualname]
 
-        obj.__dict__[self.func.__qualname__] = self.func(obj)
+        instance.__dict__[self.func.__qualname__] = self.func(instance)
 
-        return obj.__dict__[self.func.__qualname__]
+        return instance.__dict__[self.func.__qualname__]
 
 
-class local_cache:
+class local_cache(Generic[T, P, R]):
     """Caches the result of a function call locally to the instance.
     This is different from functools.cache, which caches the function result to the class, which means that
     the cache is not invalidated even if the instance is deleted.
     The functools implementation is good for i.e. HTTPS lookups,
     but causes memory leaks if the class being cached is very large
     """
 
-    def __init__(self, wrapped_func):
+    user_func: Callable[Concatenate[T, P], R]
+
+    def __init__(self, wrapped_func: Callable[Concatenate[T, P], R]):
         self.user_func = wrapped_func
 
-    def __get__(self, obj, cls):
-        partial_function = functools.update_wrapper(
-            functools.partial(_cache_wrapper(self.user_func), obj),
-            self.user_func,
-        )
-        return partial_function
+    @overload
+    def __get__(
+        self, instance: T, owner: ExportableClassMixin
+    ) -> Callable[P, R]:
+        ...
+
+    @overload
+    def __get__(
+        self, instance: None, owner: ExportableClassMixin
+    ) -> Callable[Concatenate[T, P], R]:
+        ...
+
+    def __get__(
+        self, instance: Union[T, None], owner: ExportableClassMixin
+    ) -> Union[Callable[P, R], Callable[Concatenate[T, P], R]]:
+        if instance is None:
+            return self.user_func
+        else:
+            partial_function = functools.update_wrapper(
+                functools.partial(_cache_wrapper(self.user_func), instance),
+                self.user_func,
+            )
+            return partial_function
 
     def __set__(self, obj, value):
         fname = make_cache_name(self.user_func.__qualname__)
         if fname not in obj.__dict__:
             obj.__dict__[fname] = {}
 
         key, return_value = value
```

### Comparing `prepper-1.1.5/prepper/enums.py` & `prepper-1.2.0/prepper/enums.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/prepper/exportable.py` & `prepper-1.2.0/prepper/exportable.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import shutil
 import tempfile
 import traceback
 import uuid
 import warnings
 from abc import ABCMeta
 from inspect import Parameter, signature
-from typing import Any, Dict, List, Tuple
+from typing import Any, Callable, Dict, List, Tuple, Type
 
 import h5py
 import joblib
 import loguru
 import numpy as np
 
 from prepper import H5StoreException
@@ -35,21 +35,21 @@
 ]
 
 
 def saveable_class(
     api_version: float,
     attributes: List[str] = None,
     functions: List[str] = None,
-):
+) -> Callable[[ExportableClassMixin], ExportableClassMixin]:
     if attributes is None:
         attributes = []
     if functions is None:
         functions = []
 
-    def decorator(cls: ExportableClassMixin):
+    def decorator(cls: ExportableClassMixin) -> ExportableClassMixin:
         if not issubclass(cls, ExportableClassMixin):
             raise ValueError(
                 "Only subclasses of ExportableClassMixin can be decorated with saveable_class"
             )
         attribute_names = []
         function_names = []
```

### Comparing `prepper-1.1.5/prepper/io_handlers.py` & `prepper-1.2.0/prepper/io_handlers.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/prepper/tests/test_IO.py` & `prepper-1.2.0/prepper/tests/test_IO.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/prepper/tests/test_decorators.py` & `prepper-1.2.0/prepper/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/prepper/utils.py` & `prepper-1.2.0/prepper/utils.py`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/prepper.egg-info/SOURCES.txt` & `prepper-1.2.0/prepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prepper-1.1.5/pyproject.toml` & `prepper-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [project]
 name = "prepper"
 authors = [
     {name = "Varchas Gopalaswamy", email = "vgop@lle.rochester.edu"},
 ]
 description = "Allows python objects to be stored and loaded from an HDF5 file in a language-agnostic manner"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "h5py ~= 3.8.0",
     "loguru >= 0.6.0",
     "aenum ~= 3.1.11",
     "numpy ~= 1.23.5",
     "pandas ~= 1.5.1",
     "joblib ~= 1.2.0",
+    "typing_extensions >= 4.6.3",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 CI = ["pytest", "pytest-cov","hypothesis","pylint"]
 
 [build-system]
```

