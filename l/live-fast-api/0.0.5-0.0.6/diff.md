# Comparing `tmp/live-fast-api-0.0.5.tar.gz` & `tmp/live-fast-api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live-fast-api-0.0.5.tar", last modified: Sun Jun 11 21:12:45 2023, max compression
+gzip compressed data, was "live-fast-api-0.0.6.tar", last modified: Sun Jun 11 21:25:25 2023, max compression
```

## Comparing `live-fast-api-0.0.5.tar` & `live-fast-api-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 21:12:45.296704 live-fast-api-0.0.5/
--rw-rw-rw-   0        0        0      215 2023-06-11 21:12:42.000000 live-fast-api-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2054 2023-06-11 21:12:45.296704 live-fast-api-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.5/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.5/build.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:12:44.577125 live-fast-api-0.0.5/live_api/
--rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.5/live_api/__init__.py
--rw-rw-rw-   0        0        0     7565 2023-06-11 21:12:00.000000 live-fast-api-0.0.5/live_api/base.py
--rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.5/live_api/document.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:12:45.183190 live-fast-api-0.0.5/live_api/endpoints/
--rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.5/live_api/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.5/live_api/endpoints/data.py
--rw-rw-rw-   0        0        0    11004 2023-06-11 21:12:10.000000 live-fast-api-0.0.5/live_api/endpoints/engine.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.5/live_api/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.5/live_api/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:12:45.193191 live-fast-api-0.0.5/live_api/service/
--rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.5/live_api/service/__init__.py
--rw-rw-rw-   0        0        0    18856 2023-06-11 21:11:32.000000 live-fast-api-0.0.5/live_api/service/rest.py
--rw-rw-rw-   0        0        0     2991 2023-04-21 18:19:24.000000 live-fast-api-0.0.5/live_api/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:12:44.551127 live-fast-api-0.0.5/live_api/source/
-drwxrwxrwx   0        0        0        0 2023-06-11 21:12:44.551127 live-fast-api-0.0.5/live_api/source/assets/
-drwxrwxrwx   0        0        0        0 2023-06-11 21:12:45.198190 live-fast-api-0.0.5/live_api/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.5/live_api/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.5/live_api/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-06-11 21:12:45.295704 live-fast-api-0.0.5/live_fast_api.egg-info/
--rw-rw-rw-   0        0        0     2054 2023-06-11 21:12:43.000000 live-fast-api-0.0.5/live_fast_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-06-11 21:12:43.000000 live-fast-api-0.0.5/live_fast_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 21:12:43.000000 live-fast-api-0.0.5/live_fast_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-06-11 21:12:43.000000 live-fast-api-0.0.5/live_fast_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 21:12:43.000000 live-fast-api-0.0.5/live_fast_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-06-11 21:12:42.000000 live-fast-api-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-04-21 18:21:15.000000 live-fast-api-0.0.5/requirements-dev.txt
--rw-rw-rw-   0        0        0       91 2023-04-21 18:18:24.000000 live-fast-api-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 21:12:45.297704 live-fast-api-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1580 2023-06-11 21:12:29.000000 live-fast-api-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:25:25.866204 live-fast-api-0.0.6/
+-rw-rw-rw-   0        0        0      215 2023-06-11 21:25:25.000000 live-fast-api-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2054 2023-06-11 21:25:25.865191 live-fast-api-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.6/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.6/build.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:25:25.843666 live-fast-api-0.0.6/live_api/
+-rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.6/live_api/__init__.py
+-rw-rw-rw-   0        0        0     7565 2023-06-11 21:12:00.000000 live-fast-api-0.0.6/live_api/base.py
+-rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.6/live_api/document.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:25:25.847666 live-fast-api-0.0.6/live_api/endpoints/
+-rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.6/live_api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.6/live_api/endpoints/data.py
+-rw-rw-rw-   0        0        0    11004 2023-06-11 21:12:10.000000 live-fast-api-0.0.6/live_api/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.6/live_api/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.6/live_api/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:25:25.850666 live-fast-api-0.0.6/live_api/service/
+-rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.6/live_api/service/__init__.py
+-rw-rw-rw-   0        0        0    19305 2023-06-11 21:25:12.000000 live-fast-api-0.0.6/live_api/service/rest.py
+-rw-rw-rw-   0        0        0     2991 2023-04-21 18:19:24.000000 live-fast-api-0.0.6/live_api/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:25:25.830661 live-fast-api-0.0.6/live_api/source/
+drwxrwxrwx   0        0        0        0 2023-06-11 21:25:25.830661 live-fast-api-0.0.6/live_api/source/assets/
+drwxrwxrwx   0        0        0        0 2023-06-11 21:25:25.852168 live-fast-api-0.0.6/live_api/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.6/live_api/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.6/live_api/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-06-11 21:25:25.864173 live-fast-api-0.0.6/live_fast_api.egg-info/
+-rw-rw-rw-   0        0        0     2054 2023-06-11 21:25:25.000000 live-fast-api-0.0.6/live_fast_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-06-11 21:25:25.000000 live-fast-api-0.0.6/live_fast_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:25:25.000000 live-fast-api-0.0.6/live_fast_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-06-11 21:25:25.000000 live-fast-api-0.0.6/live_fast_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 21:25:25.000000 live-fast-api-0.0.6/live_fast_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-06-11 21:25:25.000000 live-fast-api-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-04-21 18:21:15.000000 live-fast-api-0.0.6/requirements-dev.txt
+-rw-rw-rw-   0        0        0       91 2023-04-21 18:18:24.000000 live-fast-api-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 21:25:25.866204 live-fast-api-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1580 2023-06-11 21:25:21.000000 live-fast-api-0.0.6/setup.py
```

### Comparing `live-fast-api-0.0.5/PKG-INFO` & `live-fast-api-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.5/README.md` & `live-fast-api-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/build.py` & `live-fast-api-0.0.6/build.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_api/base.py` & `live-fast-api-0.0.6/live_api/base.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_api/endpoints/data.py` & `live-fast-api-0.0.6/live_api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_api/endpoints/engine.py` & `live-fast-api-0.0.6/live_api/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_api/endpoints/exceptions.py` & `live-fast-api-0.0.6/live_api/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_api/endpoints/process.py` & `live-fast-api-0.0.6/live_api/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_api/service/rest.py` & `live-fast-api-0.0.6/live_api/service/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import functools
 from typing import (
     Any, Union, Iterable, Optional, Dict, Callable
 )
 
 from uvicorn import Server, Config as ServiceConfig
 from fastapi import FastAPI, APIRouter
+import fastapi
 
 from live_api.base import terminate_thread, icons
 from live_api.endpoints import (
     EndpointFileResponse, BaseEndpoint,
     GET, EndpointRedirectResponse,
     DocsEndpoint, FAVICON, DOCS, valid_endpoints
 )
@@ -431,23 +432,37 @@
         )
 
         router = APIRouter()
 
         for endpoint in self.endpoints.values():
             endpoint.set_root(self.root)
 
-            router.add_api_route(
-                ("/" + endpoint.root if endpoint.root else '') + endpoint.path,
-                override_signature(
-                    partial(endpoint.__call__, endpoint),
-                    new=endpoint.endpoint
-                ),
-                methods=endpoint.methods, description=endpoint.description,
-                **endpoint.options
+            path = ("/" + endpoint.root if endpoint.root else '') + endpoint.path
+
+            command = override_signature(
+                partial(endpoint.__call__, endpoint),
+                new=endpoint.endpoint
             )
+
+            try:
+                router.add_api_route(
+                    path, command,
+                    methods=endpoint.methods, description=endpoint.description,
+                    **endpoint.options
+                )
+
+            except fastapi.exceptions.FastAPIError:
+                endpoint.options.setdefault('response_model', None)
+
+                router.add_api_route(
+                    path, command,
+                    methods=endpoint.methods, description=endpoint.description,
+                    **endpoint.options
+                )
+            # end try
         # end for
 
         if (self.icon is not None) and os.path.exists(self.icon):
             router.add_api_route(
                 ("/" + self.root if self.root else '') + FAVICON,
                 lambda: EndpointFileResponse(self.icon),
                 methods=[GET], include_in_schema=False
```

### Comparing `live-fast-api-0.0.5/live_api/service/sockets.py` & `live-fast-api-0.0.6/live_api/service/sockets.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_api/source/assets/icon/icon.ico` & `live-fast-api-0.0.6/live_api/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_api/source/assets/icon/icon.png` & `live-fast-api-0.0.6/live_api/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/live_fast_api.egg-info/PKG-INFO` & `live-fast-api-0.0.6/live_fast_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.5/live_fast_api.egg-info/SOURCES.txt` & `live-fast-api-0.0.6/live_fast_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.5/pyproject.toml` & `live-fast-api-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'live-fast-api'
-version = '0.0.5'
+version = '0.0.6'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `live-fast-api-0.0.5/setup.py` & `live-fast-api-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "live_api/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='live-fast-api',
-        version='0.0.5',
+        version='0.0.6',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

