# Comparing `tmp/signway_sdk-0.1.2.tar.gz` & `tmp/signway_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signway_sdk-0.1.2.tar", max compression
+gzip compressed data, was "signway_sdk-0.1.3.tar", max compression
```

## Comparing `signway_sdk-0.1.2.tar` & `signway_sdk-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/LICENSE
--rw-r--r--   0        0        0      428 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/README.md
--rw-r--r--   0        0        0      404 2023-06-10 17:26:22.987849 signway_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/signway_sdk/__init__.py
--rw-r--r--   0        0        0     1471 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/signway_sdk/sign_url.py
--rw-r--r--   0        0        0     3292 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/signway_sdk/signing_functions.py
--rw-r--r--   0        0        0      839 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/signway_sdk/test_sing_url.py
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 signway_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-11 09:41:53.885535 signway_sdk-0.1.3/LICENSE
+-rw-r--r--   0        0        0      428 2023-06-11 09:41:53.885535 signway_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0      447 2023-06-11 09:42:04.885578 signway_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-11 09:41:53.885535 signway_sdk-0.1.3/signway_sdk/__init__.py
+-rw-r--r--   0        0        0     1471 2023-06-11 09:41:53.885535 signway_sdk-0.1.3/signway_sdk/sign_url.py
+-rw-r--r--   0        0        0     3292 2023-06-11 09:41:53.885535 signway_sdk-0.1.3/signway_sdk/signing_functions.py
+-rw-r--r--   0        0        0     2803 2023-06-11 09:41:53.885535 signway_sdk-0.1.3/signway_sdk/test_signed_url.py
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 signway_sdk-0.1.3/PKG-INFO
```

### Comparing `signway_sdk-0.1.2/LICENSE` & `signway_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `signway_sdk-0.1.2/signway_sdk/sign_url.py` & `signway_sdk-0.1.3/signway_sdk/sign_url.py`

 * *Files identical despite different names*

### Comparing `signway_sdk-0.1.2/signway_sdk/signing_functions.py` & `signway_sdk-0.1.3/signway_sdk/signing_functions.py`

 * *Files identical despite different names*

### Comparing `signway_sdk-0.1.2/PKG-INFO` & `signway_sdk-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: signway-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create signed URLs for Signway
 Author: gabotechs
 Author-email: gb.mt.me@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Signway Python SDK
 
 Generate signed urls for [Signway](https://github.com/gabotechs/signway), so that they can be
 used in client-side code.
```

