# Comparing `tmp/glizzy_tls-0.1.2.tar.gz` & `tmp/glizzy_tls-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glizzy_tls-0.1.2.tar", last modified: Sun Jun 11 21:20:11 2023, max compression
+gzip compressed data, was "glizzy_tls-0.1.3.tar", last modified: Sun Jun 11 21:24:57 2023, max compression
```

## Comparing `glizzy_tls-0.1.2.tar` & `glizzy_tls-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:20:11.692297 glizzy_tls-0.1.2/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-06-11 19:12:41.000000 glizzy_tls-0.1.2/LICENSE
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       56 2023-06-11 20:50:35.000000 glizzy_tls-0.1.2/MANIFEST.in
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6093 2023-06-11 21:20:11.692071 glizzy_tls-0.1.2/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5325 2023-06-11 21:09:21.000000 glizzy_tls-0.1.2/README.md
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:20:11.688526 glizzy_tls-0.1.2/glizzy_tls/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      200 2023-06-11 18:58:24.000000 glizzy_tls-0.1.2/glizzy_tls/__init__.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:20:11.691652 glizzy_tls-0.1.2/glizzy_tls/dependencies/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       27 2023-06-11 20:56:23.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/__init__.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1580 2023-06-11 20:54:44.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/build_go.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      531 2023-06-11 18:28:11.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/go.mod
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2175 2023-06-11 18:28:11.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/go.sum
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5104 2023-06-11 18:19:01.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/tls_client.go
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      264 2023-06-11 18:22:27.000000 glizzy_tls-0.1.2/glizzy_tls/exceptions.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1644 2023-06-11 18:36:50.000000 glizzy_tls-0.1.2/glizzy_tls/models.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1149 2023-06-11 18:58:24.000000 glizzy_tls-0.1.2/glizzy_tls/request.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     4970 2023-06-11 21:19:01.000000 glizzy_tls-0.1.2/glizzy_tls/session.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:20:11.689513 glizzy_tls-0.1.2/glizzy_tls.egg-info/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6093 2023-06-11 21:20:11.000000 glizzy_tls-0.1.2/glizzy_tls.egg-info/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      459 2023-06-11 21:20:11.000000 glizzy_tls-0.1.2/glizzy_tls.egg-info/SOURCES.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 21:20:11.000000 glizzy_tls-0.1.2/glizzy_tls.egg-info/dependency_links.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2023-06-11 21:20:11.000000 glizzy_tls-0.1.2/glizzy_tls.egg-info/top_level.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 21:20:11.692360 glizzy_tls-0.1.2/setup.cfg
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1330 2023-06-11 21:19:15.000000 glizzy_tls-0.1.2/setup.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:24:57.749292 glizzy_tls-0.1.3/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-06-11 19:12:41.000000 glizzy_tls-0.1.3/LICENSE
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       56 2023-06-11 20:50:35.000000 glizzy_tls-0.1.3/MANIFEST.in
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6093 2023-06-11 21:24:57.749093 glizzy_tls-0.1.3/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5325 2023-06-11 21:09:21.000000 glizzy_tls-0.1.3/README.md
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:24:57.746037 glizzy_tls-0.1.3/glizzy_tls/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      200 2023-06-11 18:58:24.000000 glizzy_tls-0.1.3/glizzy_tls/__init__.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:24:57.748710 glizzy_tls-0.1.3/glizzy_tls/dependencies/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       27 2023-06-11 20:56:23.000000 glizzy_tls-0.1.3/glizzy_tls/dependencies/__init__.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1669 2023-06-11 21:23:56.000000 glizzy_tls-0.1.3/glizzy_tls/dependencies/build_go.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      531 2023-06-11 18:28:11.000000 glizzy_tls-0.1.3/glizzy_tls/dependencies/go.mod
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2175 2023-06-11 18:28:11.000000 glizzy_tls-0.1.3/glizzy_tls/dependencies/go.sum
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5104 2023-06-11 18:19:01.000000 glizzy_tls-0.1.3/glizzy_tls/dependencies/tls_client.go
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      264 2023-06-11 18:22:27.000000 glizzy_tls-0.1.3/glizzy_tls/exceptions.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1644 2023-06-11 18:36:50.000000 glizzy_tls-0.1.3/glizzy_tls/models.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1149 2023-06-11 18:58:24.000000 glizzy_tls-0.1.3/glizzy_tls/request.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     4970 2023-06-11 21:19:01.000000 glizzy_tls-0.1.3/glizzy_tls/session.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:24:57.746907 glizzy_tls-0.1.3/glizzy_tls.egg-info/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6093 2023-06-11 21:24:57.000000 glizzy_tls-0.1.3/glizzy_tls.egg-info/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      459 2023-06-11 21:24:57.000000 glizzy_tls-0.1.3/glizzy_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 21:24:57.000000 glizzy_tls-0.1.3/glizzy_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2023-06-11 21:24:57.000000 glizzy_tls-0.1.3/glizzy_tls.egg-info/top_level.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 21:24:57.749347 glizzy_tls-0.1.3/setup.cfg
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1330 2023-06-11 21:24:01.000000 glizzy_tls-0.1.3/setup.py
```

### Comparing `glizzy_tls-0.1.2/LICENSE` & `glizzy_tls-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.2/PKG-INFO` & `glizzy_tls-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glizzy_tls
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.
 Home-page: https://github.com/glizzykingdreko/glizzy_tls
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `glizzy_tls-0.1.2/README.md` & `glizzy_tls-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.2/glizzy_tls/dependencies/go.mod` & `glizzy_tls-0.1.3/glizzy_tls/dependencies/go.mod`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.2/glizzy_tls/dependencies/go.sum` & `glizzy_tls-0.1.3/glizzy_tls/dependencies/go.sum`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.2/glizzy_tls/dependencies/tls_client.go` & `glizzy_tls-0.1.3/glizzy_tls/dependencies/tls_client.go`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.2/glizzy_tls/models.py` & `glizzy_tls-0.1.3/glizzy_tls/models.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.2/glizzy_tls/request.py` & `glizzy_tls-0.1.3/glizzy_tls/request.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.2/glizzy_tls/session.py` & `glizzy_tls-0.1.3/glizzy_tls/session.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.2/glizzy_tls.egg-info/PKG-INFO` & `glizzy_tls-0.1.3/glizzy_tls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glizzy-tls
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.
 Home-page: https://github.com/glizzykingdreko/glizzy_tls
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `glizzy_tls-0.1.2/setup.py` & `glizzy_tls-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='glizzy_tls',
-    version='0.1.2',
+    version='0.1.3',
     description='A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/glizzykingdreko/glizzy_tls',
     author='glizzykingdreko',
     author_email='glizzykingdreko@protonmail.com',
     license='MIT',
```

