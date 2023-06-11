# Comparing `tmp/phantom-types-2.0.1.tar.gz` & `tmp/phantom-types-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phantom-types-2.0.1.tar", last modified: Sun May 28 15:54:34 2023, max compression
+gzip compressed data, was "phantom-types-2.1.0.tar", last modified: Sun Jun 11 19:42:27 2023, max compression
```

## Comparing `phantom-types-2.0.1.tar` & `phantom-types-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:34.562997 phantom-types-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-28 15:54:20.000000 phantom-types-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-28 15:54:20.000000 phantom-types-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-28 15:54:34.562997 phantom-types-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-28 15:54:20.000000 phantom-types-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-28 15:54:20.000000 phantom-types-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-28 15:54:34.562997 phantom-types-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 15:54:20.000000 phantom-types-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:34.554998 phantom-types-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:34.558997 phantom-types-2.0.1/src/phantom/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/_hypothesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:34.558997 phantom-types-2.0.1/src/phantom/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/_utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:34.558997 phantom-types-2.0.1/src/phantom/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/ext/phonenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/iso3166.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/negated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:34.558997 phantom-types-2.0.1/src/phantom/predicates/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/predicates/re.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-28 15:54:20.000000 phantom-types-2.0.1/src/phantom/sized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:54:34.562997 phantom-types-2.0.1/src/phantom_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-28 15:54:34.000000 phantom-types-2.0.1/src/phantom_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-28 15:54:34.000000 phantom-types-2.0.1/src/phantom_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:54:34.000000 phantom-types-2.0.1/src/phantom_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-28 15:54:34.000000 phantom-types-2.0.1/src/phantom_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 15:54:34.000000 phantom-types-2.0.1/src/phantom_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-11 19:42:06.000000 phantom-types-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-11 19:42:06.000000 phantom-types-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-11 19:42:27.411161 phantom-types-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-11 19:42:06.000000 phantom-types-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-11 19:42:06.000000 phantom-types-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-11 19:42:27.411161 phantom-types-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:42:06.000000 phantom-types-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.407161 phantom-types-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_hypothesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/ext/phonenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/iso3166.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/negated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom/predicates/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/sized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/top_level.txt
```

### Comparing `phantom-types-2.0.1/LICENSE` & `phantom-types-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/PKG-INFO` & `phantom-types-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phantom-types
-Version: 2.0.1
+Version: 2.1.0
 Summary: Phantom types for Python
 Home-page: https://github.com/antonagestam/phantom-types/
 Author: Anton Agestam
 Author-email: git@antonagestam.se
 License: BSD 3-Clause License
 Project-URL: Source Repository, https://github.com/antonagestam/phantom-types/
 Project-URL: Documentation, https://phantom-types.readthedocs.io/en/stable/
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: phonenumbers
 Provides-Extra: pydantic
 Provides-Extra: dateutil
 Provides-Extra: hypothesis
@@ -113,14 +114,27 @@
 
 But this will yield a static type checking error.
 
 ```python
 greet("bird")
 ```
 
+To be clear, the reason the first example passes is not because the type checker somehow
+magically knows about our predicate, but because we provided the type checker with proof
+through the `assert`. All the type checker cares about is that runtime cannot continue
+executing past the assertion, unless the variable is a `Name`. If we move the calls
+around like in the example below, the type checker would give an error for the `greet()`
+call.
+
+```python
+joe = "Joe"
+greet(joe)
+assert isinstance(joe, Name)
+```
+
 ### Runtime type checking
 
 By combining phantom types with a runtime type-checker like [beartype] or [typeguard],
 we can achieve the same level of security as you'd gain from using [contracts][dbc].
 
 ```python
 import datetime
```

### Comparing `phantom-types-2.0.1/README.md` & `phantom-types-2.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -83,14 +83,27 @@
 
 But this will yield a static type checking error.
 
 ```python
 greet("bird")
 ```
 
+To be clear, the reason the first example passes is not because the type checker somehow
+magically knows about our predicate, but because we provided the type checker with proof
+through the `assert`. All the type checker cares about is that runtime cannot continue
+executing past the assertion, unless the variable is a `Name`. If we move the calls
+around like in the example below, the type checker would give an error for the `greet()`
+call.
+
+```python
+joe = "Joe"
+greet(joe)
+assert isinstance(joe, Name)
+```
+
 ### Runtime type checking
 
 By combining phantom types with a runtime type-checker like [beartype] or [typeguard],
 we can achieve the same level of security as you'd gain from using [contracts][dbc].
 
 ```python
 import datetime
```

### Comparing `phantom-types-2.0.1/pyproject.toml` & `phantom-types-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/setup.cfg` & `phantom-types-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Development Status :: 5 - Production/Stable
 author = Anton Agestam
 author_email = git@antonagestam.se
 url = https://github.com/antonagestam/phantom-types/
 project_urls = 
 	Source Repository = https://github.com/antonagestam/phantom-types/
 	Documentation = https://phantom-types.readthedocs.io/en/stable/
@@ -27,15 +28,15 @@
 [options]
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	typeguard>=2.10,<3
+	typeguard>=4
 	typing_extensions>=4.3.0
 	numerary>=0.4.3
 
 [options.packages.find]
 where = src
 
 [options.package_data]
```

### Comparing `phantom-types-2.0.1/src/phantom/__init__.py` & `phantom-types-2.1.0/src/phantom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ._base import Phantom
 from ._base import PhantomBase
 from ._base import PhantomMeta
 from .bounds import get_bound_parser
 from .errors import BoundError
 from .predicates import Predicate
 
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 __all__ = (
     "BoundError",
     "Phantom",
     "PhantomBase",
     "PhantomMeta",
     "get_bound_parser",
     "Predicate",
```

### Comparing `phantom-types-2.0.1/src/phantom/_base.py` & `phantom-types-2.1.0/src/phantom/_base.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/_hypothesis.py` & `phantom-types-2.1.0/src/phantom/_hypothesis.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/_utils/misc.py` & `phantom-types-2.1.0/src/phantom/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/_utils/types.py` & `phantom-types-2.1.0/src/phantom/_utils/types.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/boolean.py` & `phantom-types-2.1.0/src/phantom/boolean.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/bounds.py` & `phantom-types-2.1.0/src/phantom/bounds.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/datetime.py` & `phantom-types-2.1.0/src/phantom/datetime.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/ext/phonenumbers.py` & `phantom-types-2.1.0/src/phantom/ext/phonenumbers.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/fn.py` & `phantom-types-2.1.0/src/phantom/fn.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/interval.py` & `phantom-types-2.1.0/src/phantom/interval.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/iso3166.py` & `phantom-types-2.1.0/src/phantom/iso3166.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/negated.py` & `phantom-types-2.1.0/src/phantom/negated.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/predicates/_utils.py` & `phantom-types-2.1.0/src/phantom/predicates/_utils.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/predicates/boolean.py` & `phantom-types-2.1.0/src/phantom/predicates/boolean.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/predicates/collection.py` & `phantom-types-2.1.0/src/phantom/predicates/collection.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/predicates/generic.py` & `phantom-types-2.1.0/src/phantom/predicates/generic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import types
 from typing import Tuple
 from typing import Union
 
 import typeguard
-from typing_extensions import get_args
-
-from phantom._utils.misc import is_union_type
+from typeguard import CollectionCheckStrategy
+from typeguard import ForwardRefPolicy
 
 from . import Predicate
 from ._utils import bind_name
 
 
 def equal(a: object) -> Predicate[object]:
     """Create a new predicate that succeeds when its argument is equal to ``a``."""
@@ -40,26 +38,22 @@
     def check(a: object) -> bool:
         return isinstance(a, t)
 
     return check
 
 
 def of_complex_type(t: type) -> Predicate[object]:
-    # Hack to support PEP 604 before it's implemented in typeguard, tracking issue for
-    # that feature is here: https://github.com/agronholm/typeguard/issues/222
-    # Rewrite types.UnionType objects generated by PEP 604 unions as types.GenericAlias,
-    # as if it was generated by a Union[].
-    t = (
-        types.GenericAlias(Union, get_args(t))  # type: ignore
-        if is_union_type(t)
-        else t
-    )
-
     @bind_name(of_complex_type, t)
     def check(a: object) -> bool:
         try:
-            typeguard.check_type("a", a, t, globals={}, locals={})
-        except TypeError:
+            typeguard.check_type(
+                value=a,
+                expected_type=t,
+                typecheck_fail_callback=None,
+                forward_ref_policy=ForwardRefPolicy.ERROR,
+                collection_check_strategy=CollectionCheckStrategy.ALL_ITEMS,
+            )
+        except typeguard.TypeCheckError:
             return False
         return True
 
     return check
```

### Comparing `phantom-types-2.0.1/src/phantom/predicates/interval.py` & `phantom-types-2.1.0/src/phantom/predicates/interval.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/predicates/numeric.py` & `phantom-types-2.1.0/src/phantom/predicates/numeric.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/predicates/re.py` & `phantom-types-2.1.0/src/phantom/predicates/re.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/re.py` & `phantom-types-2.1.0/src/phantom/re.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/schema.py` & `phantom-types-2.1.0/src/phantom/schema.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom/sized.py` & `phantom-types-2.1.0/src/phantom/sized.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.0.1/src/phantom_types.egg-info/PKG-INFO` & `phantom-types-2.1.0/src/phantom_types.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phantom-types
-Version: 2.0.1
+Version: 2.1.0
 Summary: Phantom types for Python
 Home-page: https://github.com/antonagestam/phantom-types/
 Author: Anton Agestam
 Author-email: git@antonagestam.se
 License: BSD 3-Clause License
 Project-URL: Source Repository, https://github.com/antonagestam/phantom-types/
 Project-URL: Documentation, https://phantom-types.readthedocs.io/en/stable/
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: phonenumbers
 Provides-Extra: pydantic
 Provides-Extra: dateutil
 Provides-Extra: hypothesis
@@ -113,14 +114,27 @@
 
 But this will yield a static type checking error.
 
 ```python
 greet("bird")
 ```
 
+To be clear, the reason the first example passes is not because the type checker somehow
+magically knows about our predicate, but because we provided the type checker with proof
+through the `assert`. All the type checker cares about is that runtime cannot continue
+executing past the assertion, unless the variable is a `Name`. If we move the calls
+around like in the example below, the type checker would give an error for the `greet()`
+call.
+
+```python
+joe = "Joe"
+greet(joe)
+assert isinstance(joe, Name)
+```
+
 ### Runtime type checking
 
 By combining phantom types with a runtime type-checker like [beartype] or [typeguard],
 we can achieve the same level of security as you'd gain from using [contracts][dbc].
 
 ```python
 import datetime
```

### Comparing `phantom-types-2.0.1/src/phantom_types.egg-info/SOURCES.txt` & `phantom-types-2.1.0/src/phantom_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

