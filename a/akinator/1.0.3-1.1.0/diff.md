# Comparing `tmp/akinator-1.0.3.tar.gz` & `tmp/akinator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akinator-1.0.3.tar", last modified: Sat Sep 17 16:00:18 2022, max compression
+gzip compressed data, was "akinator-1.1.0.tar", last modified: Sun Jun 11 11:27:28 2023, max compression
```

## Comparing `akinator-1.0.3.tar` & `akinator-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 16:00:18.271532 akinator-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-09-17 16:00:05.000000 akinator-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-17 16:00:05.000000 akinator-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-09-17 16:00:18.271532 akinator-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-09-17 16:00:05.000000 akinator-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 16:00:18.271532 akinator-1.0.3/akinator/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-09-17 16:00:05.000000 akinator-1.0.3/akinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11100 2022-09-17 16:00:05.000000 akinator-1.0.3/akinator/akinator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 16:00:18.271532 akinator-1.0.3/akinator/async_aki/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-17 16:00:05.000000 akinator-1.0.3/akinator/async_aki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12332 2022-09-17 16:00:05.000000 akinator-1.0.3/akinator/async_aki/async_akinator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2510 2022-09-17 16:00:05.000000 akinator-1.0.3/akinator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5559 2022-09-17 16:00:05.000000 akinator-1.0.3/akinator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 16:00:18.271532 akinator-1.0.3/akinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-09-17 16:00:18.000000 akinator-1.0.3/akinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-17 16:00:18.000000 akinator-1.0.3/akinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-17 16:00:18.000000 akinator-1.0.3/akinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-17 16:00:18.000000 akinator-1.0.3/akinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-17 16:00:18.000000 akinator-1.0.3/akinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-17 16:00:05.000000 akinator-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-17 16:00:18.271532 akinator-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-09-17 16:00:05.000000 akinator-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:27:28.653851 akinator-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-11 11:27:16.000000 akinator-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 11:27:16.000000 akinator-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-11 11:27:28.653851 akinator-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-11 11:27:16.000000 akinator-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:27:28.653851 akinator-1.1.0/akinator/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/akinator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:27:28.653851 akinator-1.1.0/akinator/async_aki/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/async_aki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/async_aki/async_akinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-11 11:27:16.000000 akinator-1.1.0/akinator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:27:28.653851 akinator-1.1.0/akinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 11:27:28.000000 akinator-1.1.0/akinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-11 11:27:16.000000 akinator-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 11:27:28.653851 akinator-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-11 11:27:16.000000 akinator-1.1.0/setup.py
```

### Comparing `akinator-1.0.3/LICENSE` & `akinator-1.1.0/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
-Copyright (c) 2022 Omkaar
+Copyright (c) 2019 NinjaSnail1080
+Copyright (c) 2022-present Omkaar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `akinator-1.0.3/PKG-INFO` & `akinator-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akinator
-Version: 1.0.3
+Version: 1.1.0
 Summary: An API wrapper for Akinator.
 Home-page: https://github.com/Infiniticity/akinator.py
 Author: Omkaar
 Author-email: omkaar.nerurkar@gmail.com
 License: MIT License
 Project-URL: Documentation, https://akinator.readthedocs.io
 Project-URL: Source, https://github.com/Infiniticity/akinator.py
```

### Comparing `akinator-1.0.3/README.rst` & `akinator-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `akinator-1.0.3/akinator/akinator.py` & `akinator-1.1.0/akinator/akinator.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
         return json.loads(",".join(response.split("(")[1::])[:-1])
 
     def _get_session_info(self):
         """Get uid and frontaddr from akinator.com/game"""
 
         info_regex = re.compile("var uid_ext_session = '(.*)'\\;\\n.*var frontaddr = '(.*)'\\;")
-        r = requests.get("https://en.akinator.com/game")
+        r = requests.get("https://en.akinator.com/game", verify=False)
 
         match = info_regex.search(r.text)
         self.uid, self.frontaddr = match.groups()[0], match.groups()[1]
 
     def _auto_get_region(self, lang, theme):
         """Automatically get the uri and server from akinator.com for the specified language and theme"""
```

### Comparing `akinator-1.0.3/akinator/async_aki/async_akinator.py` & `akinator-1.1.0/akinator/async_aki/async_akinator.py`

 * *Files identical despite different names*

### Comparing `akinator-1.0.3/akinator/exceptions.py` & `akinator-1.1.0/akinator/exceptions.py`

 * *Files identical despite different names*

### Comparing `akinator-1.0.3/akinator/utils.py` & `akinator-1.1.0/akinator/utils.py`

 * *Files identical despite different names*

### Comparing `akinator-1.0.3/akinator.egg-info/PKG-INFO` & `akinator-1.1.0/akinator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akinator
-Version: 1.0.3
+Version: 1.1.0
 Summary: An API wrapper for Akinator.
 Home-page: https://github.com/Infiniticity/akinator.py
 Author: Omkaar
 Author-email: omkaar.nerurkar@gmail.com
 License: MIT License
 Project-URL: Documentation, https://akinator.readthedocs.io
 Project-URL: Source, https://github.com/Infiniticity/akinator.py
```

### Comparing `akinator-1.0.3/pyproject.toml` & `akinator-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "akinator"
-version = "1.0.3"
+version = "1.1.0"
 description = "An API wrapper for Akinator."
 authors = ["Infiniticity <omkaar.nerurkar@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/Infiniticity/akinator.py/"
 documentation = "https://akinator.readthedocs.io/"
 keywords = ["python", "akinator"]
```

### Comparing `akinator-1.0.3/setup.py` & `akinator-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "async": ["aiohttp"],
     "fast_async": ["aiohttp", "cchardet", "aiodns"]
 }
 READ_ME = open(os.path.join(DIRECTORY, "README.rst")).read()
 
 setup(
     name = "akinator",
-    version = "1.0.3",
+    version = "1.1.0",
     author = "Omkaar",
     author_email = "omkaar.nerurkar@gmail.com",
     packages = ["akinator", "akinator.async_aki"],
     package_data = {
         "akinator": ["VERSION.txt"]
     },
     url = "https://github.com/Infiniticity/akinator.py",
```

