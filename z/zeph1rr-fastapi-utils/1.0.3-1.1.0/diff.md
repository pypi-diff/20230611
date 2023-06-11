# Comparing `tmp/zeph1rr_fastapi_utils-1.0.3.tar.gz` & `tmp/zeph1rr_fastapi_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeph1rr_fastapi_utils-1.0.3.tar", max compression
+gzip compressed data, was "zeph1rr_fastapi_utils-1.1.0.tar", max compression
```

## Comparing `zeph1rr_fastapi_utils-1.0.3.tar` & `zeph1rr_fastapi_utils-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      527 2023-06-11 19:18:40.585663 zeph1rr_fastapi_utils-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 20:54:40.889819 zeph1rr_fastapi_utils-1.0.3/README.md
--rw-r--r--   0        0        0      158 2023-05-28 20:57:48.425054 zeph1rr_fastapi_utils-1.0.3/zeph1rr_fastapi_utils/__init__.py
--rw-r--r--   0        0        0     1870 2023-06-11 19:18:33.764440 zeph1rr_fastapi_utils-1.0.3/zeph1rr_fastapi_utils/logger.py
--rw-r--r--   0        0        0     2234 2023-05-30 22:47:23.232714 zeph1rr_fastapi_utils-1.0.3/zeph1rr_fastapi_utils/utils.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 zeph1rr_fastapi_utils-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      527 2023-06-11 19:23:48.796067 zeph1rr_fastapi_utils-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 20:54:40.889819 zeph1rr_fastapi_utils-1.1.0/README.md
+-rw-r--r--   0        0        0      158 2023-05-28 20:57:48.425054 zeph1rr_fastapi_utils-1.1.0/zeph1rr_fastapi_utils/__init__.py
+-rw-r--r--   0        0        0     1870 2023-06-11 19:18:33.764440 zeph1rr_fastapi_utils-1.1.0/zeph1rr_fastapi_utils/logger.py
+-rw-r--r--   0        0        0     2234 2023-05-30 22:47:23.232714 zeph1rr_fastapi_utils-1.1.0/zeph1rr_fastapi_utils/utils.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 zeph1rr_fastapi_utils-1.1.0/PKG-INFO
```

### Comparing `zeph1rr_fastapi_utils-1.0.3/zeph1rr_fastapi_utils/logger.py` & `zeph1rr_fastapi_utils-1.1.0/zeph1rr_fastapi_utils/logger.py`

 * *Files identical despite different names*

### Comparing `zeph1rr_fastapi_utils-1.0.3/zeph1rr_fastapi_utils/utils.py` & `zeph1rr_fastapi_utils-1.1.0/zeph1rr_fastapi_utils/utils.py`

 * *Files identical despite different names*

### Comparing `zeph1rr_fastapi_utils-1.0.3/PKG-INFO` & `zeph1rr_fastapi_utils-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeph1rr-fastapi-utils
-Version: 1.0.3
+Version: 1.1.0
 Summary: Package for unificate functions in fastapi
 Author: Zeph1rr
 Author-email: grianton535@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
```

