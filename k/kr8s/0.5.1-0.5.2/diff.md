# Comparing `tmp/kr8s-0.5.1.tar.gz` & `tmp/kr8s-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.5.1.tar", max compression
+gzip compressed data, was "kr8s-0.5.2.tar", max compression
```

## Comparing `kr8s-0.5.1.tar` & `kr8s-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1549 2023-06-11 20:40:51.473449 kr8s-0.5.1/LICENSE
--rw-r--r--   0        0        0     2308 2023-06-11 20:40:51.473449 kr8s-0.5.1/README.md
--rw-r--r--   0        0        0      551 2023-06-11 20:41:14.753836 kr8s-0.5.1/kr8s/__init__.py
--rw-r--r--   0        0        0    10470 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_api.py
--rw-r--r--   0        0        0     5250 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_asyncio.py
--rw-r--r--   0        0        0     5854 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_auth.py
--rw-r--r--   0        0        0     1553 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_exceptions.py
--rw-r--r--   0        0        0    28114 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_objects.py
--rw-r--r--   0        0        0     7764 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/_testutils.py
--rw-r--r--   0        0        0       30 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0      992 2023-06-11 20:40:51.493450 kr8s-0.5.1/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0      685 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0       50 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5575 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/conftest.py
--rw-r--r--   0        0        0     5893 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/objects.py
--rw-r--r--   0        0        0      157 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/portforward.py
--rw-r--r--   0        0        0       61 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/resources/serviceaccount.yaml
--rwxr-xr-x   0        0        0      614 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     4385 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3144 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      639 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0    14477 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-06-11 20:40:51.497450 kr8s-0.5.1/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2576 2023-06-11 20:41:14.753836 kr8s-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 kr8s-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-06-11 20:49:47.175779 kr8s-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2308 2023-06-11 20:49:47.175779 kr8s-0.5.2/README.md
+-rw-r--r--   0        0        0      551 2023-06-11 20:50:18.911588 kr8s-0.5.2/kr8s/__init__.py
+-rw-r--r--   0        0        0    10470 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_api.py
+-rw-r--r--   0        0        0     5250 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_asyncio.py
+-rw-r--r--   0        0        0     5854 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_auth.py
+-rw-r--r--   0        0        0     1553 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_exceptions.py
+-rw-r--r--   0        0        0    28114 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_objects.py
+-rw-r--r--   0        0        0     7764 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_testutils.py
+-rw-r--r--   0        0        0       30 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0      992 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0      685 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0       50 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5575 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/conftest.py
+-rw-r--r--   0        0        0     5893 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/objects.py
+-rw-r--r--   0        0        0      157 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/portforward.py
+-rw-r--r--   0        0        0       61 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/resources/serviceaccount.yaml
+-rwxr-xr-x   0        0        0      614 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     4385 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3144 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      639 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0    14477 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2576 2023-06-11 20:50:18.911588 kr8s-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 kr8s-0.5.2/PKG-INFO
```

### Comparing `kr8s-0.5.1/LICENSE` & `kr8s-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/README.md` & `kr8s-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/__init__.py` & `kr8s-0.5.2/kr8s/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ._api import ALL  # noqa
 from ._api import Api as _AsyncApi
 from ._asyncio import run_sync as _run_sync
 from ._asyncio import sync as _sync  # noqa
 from ._exceptions import NotFoundError  # noqa
 from .asyncio import api as _api  # noqa
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.5.1/kr8s/_api.py` & `kr8s-0.5.2/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/_asyncio.py` & `kr8s-0.5.2/kr8s/_asyncio.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/_auth.py` & `kr8s-0.5.2/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/_data_utils.py` & `kr8s-0.5.2/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/_objects.py` & `kr8s-0.5.2/kr8s/_objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/_portforward.py` & `kr8s-0.5.2/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/_testutils.py` & `kr8s-0.5.2/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/asyncio/_api.py` & `kr8s-0.5.2/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/asyncio/objects.py` & `kr8s-0.5.2/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/conftest.py` & `kr8s-0.5.2/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/objects.py` & `kr8s-0.5.2/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/tests/scripts/envexec.py` & `kr8s-0.5.2/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/tests/test_api.py` & `kr8s-0.5.2/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/tests/test_auth.py` & `kr8s-0.5.2/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/tests/test_data_utils.py` & `kr8s-0.5.2/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/tests/test_objects.py` & `kr8s-0.5.2/kr8s/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/kr8s/tests/test_testutils.py` & `kr8s-0.5.2/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.1/pyproject.toml` & `kr8s-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.5.1"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.5.2"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `kr8s-0.5.1/PKG-INFO` & `kr8s-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

