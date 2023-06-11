# Comparing `tmp/bantam-2.3.4.tar.gz` & `tmp/bantam-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.3.4.tar", last modified: Sun Jun 11 03:32:32 2023, max compression
+gzip compressed data, was "bantam-2.3.5.tar", last modified: Sun Jun 11 03:59:44 2023, max compression
```

## Comparing `bantam-2.3.4.tar` & `bantam-2.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-11 03:32:32.431252 bantam-2.3.4/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.3.4/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       55 2023-06-11 01:27:30.000000 bantam-2.3.4/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-11 03:32:32.431252 bantam-2.3.4/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-11 03:23:54.000000 bantam-2.3.4/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4613 2023-06-11 03:31:41.000000 bantam-2.3.4/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    10548 2023-06-10 22:52:38.000000 bantam-2.3.4/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.3.4/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.3.4/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20981 2023-06-10 22:33:04.000000 bantam-2.3.4/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.3.4/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.3.4/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    49446 2023-06-11 03:23:34.000000 bantam-2.3.4/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.3.4/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.3.4/src/bantam/js_async.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.3.4/src/bantam/pythonclient.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       55 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4785 2023-06-10 04:24:24.000000 bantam-2.3.4/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4634 2023-06-10 04:24:36.000000 bantam-2.3.4/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.3.4/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.3.4/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.3.4/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.3.4/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.3.4/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.3.4/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-11 03:59:44.679059 bantam-2.3.5/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.3.5/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.3.5/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-11 03:59:44.679059 bantam-2.3.5/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-11 03:59:41.000000 bantam-2.3.5/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4613 2023-06-11 03:31:41.000000 bantam-2.3.5/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10548 2023-06-10 22:52:38.000000 bantam-2.3.5/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.3.5/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.3.5/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20981 2023-06-10 22:33:04.000000 bantam-2.3.5/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.3.5/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.3.5/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    49446 2023-06-11 03:23:34.000000 bantam-2.3.5/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.3.5/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.3.5/src/bantam/js_async.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.3.5/src/bantam/pythonclient.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-11 03:59:44.000000 bantam-2.3.5/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:59:44.679059 bantam-2.3.5/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4785 2023-06-10 04:24:24.000000 bantam-2.3.5/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4634 2023-06-10 04:24:36.000000 bantam-2.3.5/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.3.5/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.3.5/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.3.5/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.3.5/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.3.5/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.3.5/test/test_js_async.py
```

### Comparing `bantam-2.3.4/PKG-INFO` & `bantam-2.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.3.4
+Version: 2.3.5
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.3.4
+Download-URL: https://github.com/bantam/dist/2.3.5
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.3.4/setup.py` & `bantam-2.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.3.4"
+VERSION = "2.3.5"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.3.4/src/bantam/__init__.py` & `bantam-2.3.5/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/api.py` & `bantam-2.3.5/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/autogen/main.py` & `bantam-2.3.5/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/client.py` & `bantam-2.3.5/src/bantam/client.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/conversions.py` & `bantam-2.3.5/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/decorators.py` & `bantam-2.3.5/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/http.py` & `bantam-2.3.5/src/bantam/http.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/js.py` & `bantam-2.3.5/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/js_async.py` & `bantam-2.3.5/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam/pythonclient.py` & `bantam-2.3.5/src/bantam/pythonclient.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/src/bantam.egg-info/PKG-INFO` & `bantam-2.3.5/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.3.4
+Version: 2.3.5
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.3.4
+Download-URL: https://github.com/bantam/dist/2.3.5
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.3.4/src/bantam.egg-info/SOURCES.txt` & `bantam-2.3.5/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/test/test_client_get.py` & `bantam-2.3.5/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/test/test_client_post.py` & `bantam-2.3.5/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/test/test_client_post_inherited_apis.py` & `bantam-2.3.5/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/test/test_conversions.py` & `bantam-2.3.5/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/test/test_decorators.py` & `bantam-2.3.5/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/test/test_js.py` & `bantam-2.3.5/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.3.4/test/test_js_async.py` & `bantam-2.3.5/test/test_js_async.py`

 * *Files identical despite different names*

