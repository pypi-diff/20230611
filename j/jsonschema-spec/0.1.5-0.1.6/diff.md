# Comparing `tmp/jsonschema_spec-0.1.5.tar.gz` & `tmp/jsonschema_spec-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_spec-0.1.5.tar", max compression
+gzip compressed data, was "jsonschema_spec-0.1.6.tar", max compression
```

## Comparing `jsonschema_spec-0.1.5.tar` & `jsonschema_spec-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/LICENSE
--rw-r--r--   0        0        0     3123 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/README.rst
--rw-r--r--   0        0        0      301 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/__init__.py
--rw-r--r--   0        0        0     1362 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/accessors.py
--rw-r--r--   0        0        0      761 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/__init__.py
--rw-r--r--   0        0        0     1557 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/file.py
--rw-r--r--   0        0        0      395 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/protocols.py
--rw-r--r--   0        0        0      747 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/requests.py
--rw-r--r--   0        0        0      587 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/urllib.py
--rw-r--r--   0        0        0      361 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/utils.py
--rw-r--r--   0        0        0     1392 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/loaders.py
--rw-r--r--   0        0        0     1559 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/paths.py
--rw-r--r--   0        0        0        0 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/py.typed
--rw-r--r--   0        0        0     1082 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/readers.py
--rw-r--r--   0        0        0      247 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/utils.py
--rw-r--r--   0        0        0     2001 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4359 1970-01-01 00:00:00.000000 jsonschema_spec-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3123 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/README.rst
+-rw-r--r--   0        0        0      301 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/__init__.py
+-rw-r--r--   0        0        0     1362 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/accessors.py
+-rw-r--r--   0        0        0      761 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/__init__.py
+-rw-r--r--   0        0        0     1557 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/file.py
+-rw-r--r--   0        0        0      395 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/protocols.py
+-rw-r--r--   0        0        0      747 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/requests.py
+-rw-r--r--   0        0        0      587 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/urllib.py
+-rw-r--r--   0        0        0      361 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/utils.py
+-rw-r--r--   0        0        0     1392 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/loaders.py
+-rw-r--r--   0        0        0     1559 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/paths.py
+-rw-r--r--   0        0        0        0 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/py.typed
+-rw-r--r--   0        0        0     1082 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/readers.py
+-rw-r--r--   0        0        0      247 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/utils.py
+-rw-r--r--   0        0        0     2030 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4384 1970-01-01 00:00:00.000000 jsonschema_spec-0.1.6/PKG-INFO
```

### Comparing `jsonschema_spec-0.1.5/LICENSE` & `jsonschema_spec-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/README.rst` & `jsonschema_spec-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/jsonschema_spec/accessors.py` & `jsonschema_spec-0.1.6/jsonschema_spec/accessors.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/jsonschema_spec/handlers/__init__.py` & `jsonschema_spec-0.1.6/jsonschema_spec/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/jsonschema_spec/handlers/file.py` & `jsonschema_spec-0.1.6/jsonschema_spec/handlers/file.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/jsonschema_spec/handlers/requests.py` & `jsonschema_spec-0.1.6/jsonschema_spec/handlers/requests.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/jsonschema_spec/handlers/urllib.py` & `jsonschema_spec-0.1.6/jsonschema_spec/handlers/urllib.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/jsonschema_spec/loaders.py` & `jsonschema_spec-0.1.6/jsonschema_spec/loaders.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/jsonschema_spec/paths.py` & `jsonschema_spec-0.1.6/jsonschema_spec/paths.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/jsonschema_spec/readers.py` & `jsonschema_spec-0.1.6/jsonschema_spec/readers.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.5/pyproject.toml` & `jsonschema_spec-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [[tool.mypy.overrides]]
 module = "jsonschema.validators"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "jsonschema-spec"
-version = "0.1.5"
+version = "0.1.6"
 description = "JSONSchema Spec with object-oriented paths"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/p1c2u/jsonschema-spec"
 keywords = ["jsonschema", "swagger", "spec"]
 classifiers = [
@@ -41,15 +41,15 @@
 ]
 
 [tool.poetry.dependencies]
 jsonschema = ">=4.0.0,<4.18.0"
 pathable = "^0.4.1"
 python = "^3.7.0"
 PyYAML = ">=5.1"
-typing-extensions = "<4.6.0" # See https://github.com/p1c2u/jsonschema-spec/issues/14
+typing-extensions = {version = "<4.6.0", python = "<3.8"} # See https://github.com/p1c2u/jsonschema-spec/issues/14
 requests = {version = "^2.31.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
 pytest = "^7.3.1"
 pytest-flake8 = "=1.1.0"
 pytest-cov = "^4.1.0"
```

### Comparing `jsonschema_spec-0.1.5/PKG-INFO` & `jsonschema_spec-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-spec
-Version: 0.1.5
+Version: 0.1.6
 Summary: JSONSchema Spec with object-oriented paths
 Home-page: https://github.com/p1c2u/jsonschema-spec
 License: Apache-2.0
 Keywords: jsonschema,swagger,spec
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=5.1)
 Requires-Dist: jsonschema (>=4.0.0,<4.18.0)
 Requires-Dist: pathable (>=0.4.1,<0.5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: typing-extensions (<4.6.0)
+Requires-Dist: typing-extensions (<4.6.0) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/p1c2u/jsonschema-spec
 Description-Content-Type: text/x-rst
 
 ***************
 JSONSchema Spec
 ***************
```

