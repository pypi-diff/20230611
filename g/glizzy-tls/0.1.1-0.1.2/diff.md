# Comparing `tmp/glizzy_tls-0.1.1.tar.gz` & `tmp/glizzy_tls-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glizzy_tls-0.1.1.tar", last modified: Sun Jun 11 21:10:06 2023, max compression
+gzip compressed data, was "glizzy_tls-0.1.2.tar", last modified: Sun Jun 11 21:20:11 2023, max compression
```

## Comparing `glizzy_tls-0.1.1.tar` & `glizzy_tls-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:10:06.579687 glizzy_tls-0.1.1/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-06-11 19:12:41.000000 glizzy_tls-0.1.1/LICENSE
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       56 2023-06-11 20:50:35.000000 glizzy_tls-0.1.1/MANIFEST.in
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6093 2023-06-11 21:10:06.579486 glizzy_tls-0.1.1/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5325 2023-06-11 21:09:21.000000 glizzy_tls-0.1.1/README.md
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:10:06.574740 glizzy_tls-0.1.1/glizzy_tls/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      200 2023-06-11 18:58:24.000000 glizzy_tls-0.1.1/glizzy_tls/__init__.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:10:06.579130 glizzy_tls-0.1.1/glizzy_tls/dependencies/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       27 2023-06-11 20:56:23.000000 glizzy_tls-0.1.1/glizzy_tls/dependencies/__init__.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1580 2023-06-11 20:54:44.000000 glizzy_tls-0.1.1/glizzy_tls/dependencies/build_go.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      531 2023-06-11 18:28:11.000000 glizzy_tls-0.1.1/glizzy_tls/dependencies/go.mod
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2175 2023-06-11 18:28:11.000000 glizzy_tls-0.1.1/glizzy_tls/dependencies/go.sum
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5104 2023-06-11 18:19:01.000000 glizzy_tls-0.1.1/glizzy_tls/dependencies/tls_client.go
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      264 2023-06-11 18:22:27.000000 glizzy_tls-0.1.1/glizzy_tls/exceptions.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1644 2023-06-11 18:36:50.000000 glizzy_tls-0.1.1/glizzy_tls/models.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1149 2023-06-11 18:58:24.000000 glizzy_tls-0.1.1/glizzy_tls/request.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     4970 2023-06-11 20:56:28.000000 glizzy_tls-0.1.1/glizzy_tls/session.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:10:06.577175 glizzy_tls-0.1.1/glizzy_tls.egg-info/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6093 2023-06-11 21:10:06.000000 glizzy_tls-0.1.1/glizzy_tls.egg-info/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      459 2023-06-11 21:10:06.000000 glizzy_tls-0.1.1/glizzy_tls.egg-info/SOURCES.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 21:10:06.000000 glizzy_tls-0.1.1/glizzy_tls.egg-info/dependency_links.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2023-06-11 21:10:06.000000 glizzy_tls-0.1.1/glizzy_tls.egg-info/top_level.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 21:10:06.579747 glizzy_tls-0.1.1/setup.cfg
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1330 2023-06-11 21:09:46.000000 glizzy_tls-0.1.1/setup.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:20:11.692297 glizzy_tls-0.1.2/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-06-11 19:12:41.000000 glizzy_tls-0.1.2/LICENSE
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       56 2023-06-11 20:50:35.000000 glizzy_tls-0.1.2/MANIFEST.in
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6093 2023-06-11 21:20:11.692071 glizzy_tls-0.1.2/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5325 2023-06-11 21:09:21.000000 glizzy_tls-0.1.2/README.md
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:20:11.688526 glizzy_tls-0.1.2/glizzy_tls/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      200 2023-06-11 18:58:24.000000 glizzy_tls-0.1.2/glizzy_tls/__init__.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:20:11.691652 glizzy_tls-0.1.2/glizzy_tls/dependencies/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       27 2023-06-11 20:56:23.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/__init__.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1580 2023-06-11 20:54:44.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/build_go.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      531 2023-06-11 18:28:11.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/go.mod
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2175 2023-06-11 18:28:11.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/go.sum
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5104 2023-06-11 18:19:01.000000 glizzy_tls-0.1.2/glizzy_tls/dependencies/tls_client.go
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      264 2023-06-11 18:22:27.000000 glizzy_tls-0.1.2/glizzy_tls/exceptions.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1644 2023-06-11 18:36:50.000000 glizzy_tls-0.1.2/glizzy_tls/models.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1149 2023-06-11 18:58:24.000000 glizzy_tls-0.1.2/glizzy_tls/request.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     4970 2023-06-11 21:19:01.000000 glizzy_tls-0.1.2/glizzy_tls/session.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:20:11.689513 glizzy_tls-0.1.2/glizzy_tls.egg-info/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6093 2023-06-11 21:20:11.000000 glizzy_tls-0.1.2/glizzy_tls.egg-info/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      459 2023-06-11 21:20:11.000000 glizzy_tls-0.1.2/glizzy_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 21:20:11.000000 glizzy_tls-0.1.2/glizzy_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2023-06-11 21:20:11.000000 glizzy_tls-0.1.2/glizzy_tls.egg-info/top_level.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 21:20:11.692360 glizzy_tls-0.1.2/setup.cfg
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1330 2023-06-11 21:19:15.000000 glizzy_tls-0.1.2/setup.py
```

### Comparing `glizzy_tls-0.1.1/LICENSE` & `glizzy_tls-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.1/PKG-INFO` & `glizzy_tls-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glizzy_tls
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.
 Home-page: https://github.com/glizzykingdreko/glizzy_tls
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `glizzy_tls-0.1.1/README.md` & `glizzy_tls-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.1/glizzy_tls/dependencies/build_go.py` & `glizzy_tls-0.1.2/glizzy_tls/dependencies/build_go.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.1/glizzy_tls/dependencies/go.mod` & `glizzy_tls-0.1.2/glizzy_tls/dependencies/go.mod`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.1/glizzy_tls/dependencies/go.sum` & `glizzy_tls-0.1.2/glizzy_tls/dependencies/go.sum`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.1/glizzy_tls/dependencies/tls_client.go` & `glizzy_tls-0.1.2/glizzy_tls/dependencies/tls_client.go`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.1/glizzy_tls/models.py` & `glizzy_tls-0.1.2/glizzy_tls/models.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.1/glizzy_tls/request.py` & `glizzy_tls-0.1.2/glizzy_tls/request.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.1/glizzy_tls/session.py` & `glizzy_tls-0.1.2/glizzy_tls/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,32 +36,32 @@
         Args:
             client_hello (str, optional): The client hello to use for this session. Defaults to "Chrome_112".
         """
         self.client_hello = client_hello.capitalize().encode('utf-8')
         self.cookies = []
     
 
-    def request(self, method, url, headers: dict=None, body=None, cookies: list=None, proxy: str=None, follow_redirects: int=1, timeout_seconds: int=30, details: bool=False) -> Union[Response, RequestDetails]:
+    def request(self, method, url, headers: dict=None, data=None, cookies: list=None, proxy: str=None, follow_redirects: int=1, timeout_seconds: int=30, details: bool=False) -> Union[Response, RequestDetails]:
         """
         Send a TLS request using this session.
 
         Args:
             method (str): The HTTP method to use for this request.
             url (str): The URL to send the request to.
             headers (dict, optional): The headers to send with this request. Defaults to None.
-            body (dict, optional): The body to send with this request. Defaults to None.
+            data (dict, optional): The body to send with this request. Defaults to None.
             cookies (list, optional): The cookies to send with this request. Defaults to None.
             proxy (str, optional): The proxy to use for this request. Defaults to None.
             follow_redirects (int, optional): Whether or not to follow redirects. Defaults to 1.
             timeout_seconds (int, optional): The number of seconds to wait for a response before timing out. Defaults to 30.
             details (bool, optional): Whether or not to return the request details. Defaults to False.
         """
         # Convert the parameters to JSON strings
         headers_json = dumps(headers).encode('utf-8') if headers else "".encode('utf-8')
-        body_json = dumps(body).encode('utf-8') if body else "".encode('utf-8')
+        body_json = dumps(data).encode('utf-8') if data else "".encode('utf-8')
 
         # If no cookies were provided for this request, use the session cookies
         if not cookies:
             cookies = self.cookies
 
         # Process cookies
         cookies_list = []
```

### Comparing `glizzy_tls-0.1.1/glizzy_tls.egg-info/PKG-INFO` & `glizzy_tls-0.1.2/glizzy_tls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glizzy-tls
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.
 Home-page: https://github.com/glizzykingdreko/glizzy_tls
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `glizzy_tls-0.1.1/setup.py` & `glizzy_tls-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='glizzy_tls',
-    version='0.1.1',
+    version='0.1.2',
     description='A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/glizzykingdreko/glizzy_tls',
     author='glizzykingdreko',
     author_email='glizzykingdreko@protonmail.com',
     license='MIT',
```

