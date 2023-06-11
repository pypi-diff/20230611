# Comparing `tmp/Flask_Limit-1.0.3.tar.gz` & `tmp/Flask_Limit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask_Limit-1.0.3.tar", last modified: Fri Dec 30 01:51:34 2022, max compression
+gzip compressed data, was "Flask_Limit-1.0.4.tar", last modified: Sun Jun 11 00:26:08 2023, max compression
```

## Comparing `Flask_Limit-1.0.3.tar` & `Flask_Limit-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2022-12-30 01:51:34.448428 Flask_Limit-1.0.3/
--rw-r--r--   0 tabot      (501) staff       (20)       35 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/AUTHORS
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2022-12-30 01:51:34.447240 Flask_Limit-1.0.3/Flask_Limit.egg-info/
--rw-r--r--   0 tabot      (501) staff       (20)     3376 2022-12-30 01:51:34.000000 Flask_Limit-1.0.3/Flask_Limit.egg-info/PKG-INFO
--rw-r--r--   0 tabot      (501) staff       (20)      362 2022-12-30 01:51:34.000000 Flask_Limit-1.0.3/Flask_Limit.egg-info/SOURCES.txt
--rw-r--r--   0 tabot      (501) staff       (20)        1 2022-12-30 01:51:34.000000 Flask_Limit-1.0.3/Flask_Limit.egg-info/dependency_links.txt
--rw-r--r--   0 tabot      (501) staff       (20)        1 2022-12-30 01:51:34.000000 Flask_Limit-1.0.3/Flask_Limit.egg-info/not-zip-safe
--rw-r--r--   0 tabot      (501) staff       (20)        6 2022-12-30 01:51:34.000000 Flask_Limit-1.0.3/Flask_Limit.egg-info/requires.txt
--rw-r--r--   0 tabot      (501) staff       (20)       12 2022-12-30 01:51:34.000000 Flask_Limit-1.0.3/Flask_Limit.egg-info/top_level.txt
--rw-r--r--   0 tabot      (501) staff       (20)     1068 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/LICENSE
--rw-r--r--   0 tabot      (501) staff       (20)       80 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/MANIFEST.in
--rw-r--r--   0 tabot      (501) staff       (20)     3376 2022-12-30 01:51:34.448310 Flask_Limit-1.0.3/PKG-INFO
--rw-r--r--   0 tabot      (501) staff       (20)     2573 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/README.md
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2022-12-30 01:51:34.447360 Flask_Limit-1.0.3/docs/
--rw-r--r--   0 tabot      (501) staff       (20)     3017 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/docs/index.rst
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2022-12-30 01:51:34.447740 Flask_Limit-1.0.3/flask_limit/
--rw-r--r--   0 tabot      (501) staff       (20)       59 2022-12-30 01:50:27.000000 Flask_Limit-1.0.3/flask_limit/__init__.py
--rwxr-xr-x   0 tabot      (501) staff       (20)     3974 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/flask_limit/rate_limit.py
--rw-r--r--   0 tabot      (501) staff       (20)       38 2022-12-30 01:51:34.448461 Flask_Limit-1.0.3/setup.cfg
--rwxr-xr-x   0 tabot      (501) staff       (20)     1383 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/setup.py
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2022-12-30 01:51:34.448015 Flask_Limit-1.0.3/tests/
--rw-r--r--   0 tabot      (501) staff       (20)        0 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/tests/__init__.py
--rw-r--r--   0 tabot      (501) staff       (20)     1906 2022-12-30 01:49:43.000000 Flask_Limit-1.0.3/tests/test_rate_limit.py
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:26:08.159918 Flask_Limit-1.0.4/
+-rw-r--r--   0 tabot      (501) staff       (20)       35 2022-12-30 01:49:43.000000 Flask_Limit-1.0.4/AUTHORS
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:26:08.158601 Flask_Limit-1.0.4/Flask_Limit.egg-info/
+-rw-r--r--   0 tabot      (501) staff       (20)     3376 2023-06-11 00:26:08.000000 Flask_Limit-1.0.4/Flask_Limit.egg-info/PKG-INFO
+-rw-r--r--   0 tabot      (501) staff       (20)      362 2023-06-11 00:26:08.000000 Flask_Limit-1.0.4/Flask_Limit.egg-info/SOURCES.txt
+-rw-r--r--   0 tabot      (501) staff       (20)        1 2023-06-11 00:26:08.000000 Flask_Limit-1.0.4/Flask_Limit.egg-info/dependency_links.txt
+-rw-r--r--   0 tabot      (501) staff       (20)        1 2022-12-30 01:51:34.000000 Flask_Limit-1.0.4/Flask_Limit.egg-info/not-zip-safe
+-rw-r--r--   0 tabot      (501) staff       (20)        6 2023-06-11 00:26:08.000000 Flask_Limit-1.0.4/Flask_Limit.egg-info/requires.txt
+-rw-r--r--   0 tabot      (501) staff       (20)       12 2023-06-11 00:26:08.000000 Flask_Limit-1.0.4/Flask_Limit.egg-info/top_level.txt
+-rw-r--r--   0 tabot      (501) staff       (20)     1068 2022-12-30 01:49:43.000000 Flask_Limit-1.0.4/LICENSE
+-rw-r--r--   0 tabot      (501) staff       (20)       80 2022-12-30 01:49:43.000000 Flask_Limit-1.0.4/MANIFEST.in
+-rw-r--r--   0 tabot      (501) staff       (20)     3376 2023-06-11 00:26:08.159793 Flask_Limit-1.0.4/PKG-INFO
+-rw-r--r--   0 tabot      (501) staff       (20)     2573 2022-12-30 01:49:43.000000 Flask_Limit-1.0.4/README.md
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:26:08.158724 Flask_Limit-1.0.4/docs/
+-rw-r--r--   0 tabot      (501) staff       (20)     3017 2022-12-30 01:49:43.000000 Flask_Limit-1.0.4/docs/index.rst
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:26:08.159084 Flask_Limit-1.0.4/flask_limit/
+-rw-r--r--   0 tabot      (501) staff       (20)       59 2023-06-11 00:24:05.000000 Flask_Limit-1.0.4/flask_limit/__init__.py
+-rwxr-xr-x   0 tabot      (501) staff       (20)     3976 2023-06-11 00:12:40.000000 Flask_Limit-1.0.4/flask_limit/rate_limit.py
+-rw-r--r--   0 tabot      (501) staff       (20)       38 2023-06-11 00:26:08.159952 Flask_Limit-1.0.4/setup.cfg
+-rwxr-xr-x   0 tabot      (501) staff       (20)     1383 2022-12-30 01:49:43.000000 Flask_Limit-1.0.4/setup.py
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:26:08.159464 Flask_Limit-1.0.4/tests/
+-rw-r--r--   0 tabot      (501) staff       (20)        0 2022-12-30 01:49:43.000000 Flask_Limit-1.0.4/tests/__init__.py
+-rw-r--r--   0 tabot      (501) staff       (20)     1906 2022-12-30 01:49:43.000000 Flask_Limit-1.0.4/tests/test_rate_limit.py
```

### Comparing `Flask_Limit-1.0.3/Flask_Limit.egg-info/PKG-INFO` & `Flask_Limit-1.0.4/Flask_Limit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Limit
-Version: 1.0.3
+Version: 1.0.4
 Summary: An extension that provides rate limiting for Flask routes.
 Home-page: https://github.com/tabotkevin/flask_limit
 Author: Tabot Kevin
 Author-email: tabot.kevin@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flask_Limit-1.0.3/LICENSE` & `Flask_Limit-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask_Limit-1.0.3/PKG-INFO` & `Flask_Limit-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask_Limit
-Version: 1.0.3
+Version: 1.0.4
 Summary: An extension that provides rate limiting for Flask routes.
 Home-page: https://github.com/tabotkevin/flask_limit
 Author: Tabot Kevin
 Author-email: tabot.kevin@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flask_Limit-1.0.3/README.md` & `Flask_Limit-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Flask_Limit-1.0.3/docs/index.rst` & `Flask_Limit-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask_Limit-1.0.3/flask_limit/rate_limit.py` & `Flask_Limit-1.0.4/flask_limit/rate_limit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-import functools
+from functools import wraps
 from time import time
 from flask import current_app, request, g, jsonify
 
 logger = logging.getLogger()
 
 _limiter = None
 
@@ -68,15 +68,15 @@
         answered with a status code 429 Too Many Requests for the remaining of
         that period."""
         if f is None:
             return functools.partial(self.rate_limit, limit=limit, period=period)
         limit = limit if limit else current_app.config['RATELIMITE_LIMIT']
         period = period if period else current_app.config['RATELIMIT_PERIOD']
 
-        functools.wraps(f)
+        @wraps(f)
         def wrapped(*args, **kwargs):
             # initialize the rate limiter the first time here
             global _limiter
             if _limiter is None:
                 _limiter = MemRateLimit()
 
             # generate a unique key to represent the decorated function and
```

### Comparing `Flask_Limit-1.0.3/setup.py` & `Flask_Limit-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `Flask_Limit-1.0.3/tests/test_rate_limit.py` & `Flask_Limit-1.0.4/tests/test_rate_limit.py`

 * *Files identical despite different names*

