# Comparing `tmp/pymangaplus-1.1.1.tar.gz` & `tmp/pymangaplus-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymangaplus-1.1.1.tar", last modified: Fri Jun  9 12:37:06 2023, max compression
+gzip compressed data, was "pymangaplus-1.1.2.tar", last modified: Sun Jun 11 13:01:13 2023, max compression
```

## Comparing `pymangaplus-1.1.1.tar` & `pymangaplus-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:37:06.454589 pymangaplus-1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-06-09 12:34:31.000000 pymangaplus-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3453 2023-06-09 12:37:06.454589 pymangaplus-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2023-06-09 12:36:54.000000 pymangaplus-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 12:37:06.430654 pymangaplus-1.1.1/pymangaplus/
--rw-rw-rw-   0        0        0       82 2023-06-09 12:34:58.000000 pymangaplus-1.1.1/pymangaplus/__init__.py
--rw-rw-rw-   0        0        0   101493 2023-06-09 12:34:31.000000 pymangaplus-1.1.1/pymangaplus/api_protocol_pb2.py
--rw-rw-rw-   0        0        0     6381 2023-06-09 12:34:31.000000 pymangaplus-1.1.1/pymangaplus/client.py
--rw-rw-rw-   0        0        0      356 2023-06-09 12:34:31.000000 pymangaplus-1.1.1/pymangaplus/constants.py
--rw-rw-rw-   0        0        0      529 2023-06-09 12:34:31.000000 pymangaplus-1.1.1/pymangaplus/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:37:06.454589 pymangaplus-1.1.1/pymangaplus.egg-info/
--rw-rw-rw-   0        0        0     3453 2023-06-09 12:37:06.000000 pymangaplus-1.1.1/pymangaplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-06-09 12:37:06.000000 pymangaplus-1.1.1/pymangaplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:37:06.000000 pymangaplus-1.1.1/pymangaplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-09 12:37:06.000000 pymangaplus-1.1.1/pymangaplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 12:37:06.000000 pymangaplus-1.1.1/pymangaplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 12:37:06.454589 pymangaplus-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-06-09 12:34:58.000000 pymangaplus-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:01:13.894760 pymangaplus-1.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-11 11:44:56.000000 pymangaplus-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3447 2023-06-11 13:01:13.894760 pymangaplus-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2537 2023-06-11 13:01:02.000000 pymangaplus-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 13:01:13.870335 pymangaplus-1.1.2/pymangaplus/
+-rw-rw-rw-   0        0        0       79 2023-06-11 12:58:18.000000 pymangaplus-1.1.2/pymangaplus/__init__.py
+-rw-rw-rw-   0        0        0   101493 2023-06-11 11:44:56.000000 pymangaplus-1.1.2/pymangaplus/api_protocol_pb2.py
+-rw-rw-rw-   0        0        0     6379 2023-06-11 12:57:34.000000 pymangaplus-1.1.2/pymangaplus/client.py
+-rw-rw-rw-   0        0        0      356 2023-06-11 11:44:56.000000 pymangaplus-1.1.2/pymangaplus/constants.py
+-rw-rw-rw-   0        0        0      529 2023-06-11 11:44:56.000000 pymangaplus-1.1.2/pymangaplus/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:01:13.894760 pymangaplus-1.1.2/pymangaplus.egg-info/
+-rw-rw-rw-   0        0        0     3447 2023-06-11 13:01:13.000000 pymangaplus-1.1.2/pymangaplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-06-11 13:01:13.000000 pymangaplus-1.1.2/pymangaplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 13:01:13.000000 pymangaplus-1.1.2/pymangaplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-11 13:01:13.000000 pymangaplus-1.1.2/pymangaplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-11 13:01:13.000000 pymangaplus-1.1.2/pymangaplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 13:01:13.894760 pymangaplus-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-06-11 12:58:18.000000 pymangaplus-1.1.2/setup.py
```

### Comparing `pymangaplus-1.1.1/LICENSE` & `pymangaplus-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymangaplus-1.1.1/PKG-INFO` & `pymangaplus-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymangaplus
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python client for the MangaPlus API.
 Home-page: https://github.com/hyugogirubato/pymangaplus
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: client,manga,ebooks,manga-plus
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,23 +55,23 @@
 ## Usage
 
 Here's an example of how to use the PyMangaPlus library:
 
 ```python
 import secrets
 
-from pymangaplus.client import MangaPlus
+from pymangaplus.client import Client
 from pymangaplus.constants import Quality
 
 if __name__ == "__main__":
     title_id = 100191  # OSHI NO KO
     chapter_id = 1014090  # Chapter 86: ASSISTANT DIRECTOR
     android_id = secrets.token_bytes(8).hex()
 
-    client = MangaPlus()
+    client = Client()
 
     # Register new device
     client.register(android_id)
 
     # Home titles
     content = client.home()
     print(content)
```

### Comparing `pymangaplus-1.1.1/README.md` & `pymangaplus-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 ## Usage
 
 Here's an example of how to use the PyMangaPlus library:
 
 ```python
 import secrets
 
-from pymangaplus.client import MangaPlus
+from pymangaplus.client import Client
 from pymangaplus.constants import Quality
 
 if __name__ == "__main__":
     title_id = 100191  # OSHI NO KO
     chapter_id = 1014090  # Chapter 86: ASSISTANT DIRECTOR
     android_id = secrets.token_bytes(8).hex()
 
-    client = MangaPlus()
+    client = Client()
 
     # Register new device
     client.register(android_id)
 
     # Home titles
     content = client.home()
     print(content)
```

### Comparing `pymangaplus-1.1.1/pymangaplus/api_protocol_pb2.py` & `pymangaplus-1.1.2/pymangaplus/api_protocol_pb2.py`

 * *Files identical despite different names*

### Comparing `pymangaplus-1.1.1/pymangaplus/client.py` & `pymangaplus-1.1.2/pymangaplus/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import hashlib
 import requests
 
 from pymangaplus.constants import Language, Mode, Quality
 from pymangaplus.utils import proto2dict
 
 
-class MangaPlus:
+class Client:
 
     def __init__(self, language: Language = Language.ENGLISH):
         self.language = language.value
         self.secret = None
         self.api = "https://jumpg-api.tokyo-cdn.com/api"
 
     def _request(self, **kwargs) -> dict:
         headers = {
             "accept": "*/*",
             "user-agent": "okhttp/4.9.0"
         }
-        headers.update(kwargs.get("update") or {})
+        headers.update(kwargs.get("headers") or {})
 
         params = kwargs.get("params") or {}
         params["os"] = "android"
         params["os_ver"] = 29
         params["app_ver"] = 47
         if self._secret:
             params["secret"] = self._secret
```

### Comparing `pymangaplus-1.1.1/pymangaplus/utils.py` & `pymangaplus-1.1.2/pymangaplus/utils.py`

 * *Files identical despite different names*

### Comparing `pymangaplus-1.1.1/pymangaplus.egg-info/PKG-INFO` & `pymangaplus-1.1.2/pymangaplus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymangaplus
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python client for the MangaPlus API.
 Home-page: https://github.com/hyugogirubato/pymangaplus
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: client,manga,ebooks,manga-plus
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,23 +55,23 @@
 ## Usage
 
 Here's an example of how to use the PyMangaPlus library:
 
 ```python
 import secrets
 
-from pymangaplus.client import MangaPlus
+from pymangaplus.client import Client
 from pymangaplus.constants import Quality
 
 if __name__ == "__main__":
     title_id = 100191  # OSHI NO KO
     chapter_id = 1014090  # Chapter 86: ASSISTANT DIRECTOR
     android_id = secrets.token_bytes(8).hex()
 
-    client = MangaPlus()
+    client = Client()
 
     # Register new device
     client.register(android_id)
 
     # Home titles
     content = client.home()
     print(content)
```

### Comparing `pymangaplus-1.1.1/setup.py` & `pymangaplus-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pymangaplus",
-    version="1.1.1",
+    version="1.1.2",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python client for the MangaPlus API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pymangaplus",
     packages=find_packages(),
```

