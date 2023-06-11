# Comparing `tmp/reflect-client-1.1.1.tar.gz` & `tmp/reflect-client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflect-client-1.1.1.tar", last modified: Mon Jun  5 12:22:01 2023, max compression
+gzip compressed data, was "reflect-client-1.1.2.tar", last modified: Sun Jun 11 14:32:24 2023, max compression
```

## Comparing `reflect-client-1.1.1.tar` & `reflect-client-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-05 12:22:01.344523 reflect-client-1.1.1/
--rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-05 12:22:01.343523 reflect-client-1.1.1/PKG-INFO
--rw-r--r--   0 victor    (1000) victor    (1000)     2027 2023-06-03 12:07:24.000000 reflect-client-1.1.1/README.md
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-05 12:22:01.328523 reflect-client-1.1.1/reflect_client/
--rw-r--r--   0 victor    (1000) victor    (1000)     4084 2023-06-05 12:19:31.000000 reflect-client-1.1.1/reflect_client/Client.py
--rw-r--r--   0 victor    (1000) victor    (1000)        0 2023-06-03 12:07:24.000000 reflect-client-1.1.1/reflect_client/__init__.py
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-05 12:22:01.343523 reflect-client-1.1.1/reflect_client.egg-info/
--rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-05 12:22:00.000000 reflect-client-1.1.1/reflect_client.egg-info/PKG-INFO
--rw-r--r--   0 victor    (1000) victor    (1000)      259 2023-06-05 12:22:01.000000 reflect-client-1.1.1/reflect_client.egg-info/SOURCES.txt
--rw-r--r--   0 victor    (1000) victor    (1000)        1 2023-06-05 12:22:00.000000 reflect-client-1.1.1/reflect_client.egg-info/dependency_links.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       20 2023-06-05 12:22:00.000000 reflect-client-1.1.1/reflect_client.egg-info/requires.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       15 2023-06-05 12:22:00.000000 reflect-client-1.1.1/reflect_client.egg-info/top_level.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       38 2023-06-05 12:22:01.344523 reflect-client-1.1.1/setup.cfg
--rw-r--r--   0 victor    (1000) victor    (1000)      529 2023-06-05 12:19:58.000000 reflect-client-1.1.1/setup.py
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-11 14:32:24.388578 reflect-client-1.1.2/
+-rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-11 14:32:24.387578 reflect-client-1.1.2/PKG-INFO
+-rw-r--r--   0 victor    (1000) victor    (1000)     2027 2023-06-03 12:07:24.000000 reflect-client-1.1.2/README.md
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-11 14:32:24.382578 reflect-client-1.1.2/reflect_client/
+-rw-r--r--   0 victor    (1000) victor    (1000)     4082 2023-06-11 14:31:25.000000 reflect-client-1.1.2/reflect_client/Client.py
+-rw-r--r--   0 victor    (1000) victor    (1000)        0 2023-06-03 12:07:24.000000 reflect-client-1.1.2/reflect_client/__init__.py
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-11 14:32:24.385578 reflect-client-1.1.2/reflect_client.egg-info/
+-rw-r--r--   0 victor    (1000) victor    (1000)      350 2023-06-11 14:32:23.000000 reflect-client-1.1.2/reflect_client.egg-info/PKG-INFO
+-rw-r--r--   0 victor    (1000) victor    (1000)      259 2023-06-11 14:32:24.000000 reflect-client-1.1.2/reflect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)        1 2023-06-11 14:32:23.000000 reflect-client-1.1.2/reflect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       20 2023-06-11 14:32:23.000000 reflect-client-1.1.2/reflect_client.egg-info/requires.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       15 2023-06-11 14:32:23.000000 reflect-client-1.1.2/reflect_client.egg-info/top_level.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       38 2023-06-11 14:32:24.388578 reflect-client-1.1.2/setup.cfg
+-rw-r--r--   0 victor    (1000) victor    (1000)      529 2023-06-11 14:32:05.000000 reflect-client-1.1.2/setup.py
```

### Comparing `reflect-client-1.1.1/README.md` & `reflect-client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `reflect-client-1.1.1/reflect_client/Client.py` & `reflect-client-1.1.2/reflect_client/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 
     # Construct list of headers to send with HTTP request
     def http_headers(self) -> list:
         headers = {
             "Content-Type": "application/json"
         }
 
-        # Append Authentication header if API key is provided
+        # Append Authorization header if API key is provided
         if (self._key):
-            headers["Authentication"] = f"Bearer {self._key}"
+            headers["Authorization"] = f"Bearer {self._key}"
 
         return headers
 
     # Make request and return response over HTTP
     def http_call(self, endpoint: str, method: Method, payload: list = None) -> tuple:
         # Remove leading "/" if present, as it's already present in self._endpoint
         endpoint = endpoint if endpoint[-1] != "/" else endpoint[:-1]
```

### Comparing `reflect-client-1.1.1/setup.py` & `reflect-client-1.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "reflect-client",
-    version = "1.1.1",
+    version = "1.1.2",
     description = "Python library for communicating with an API built with Reflect over HTTP or UNIX sockets",
     author = "Victor Westerlund",
     author_email = "victor.vesterlund@gmail.com",
     url = "https://github.com/victorwesterlund/reflect-client-python",
     packages = ["reflect_client"],
     # The requirement.txt file should also be updated when changing this
     install_requires = ["validators", "requests"]
```

