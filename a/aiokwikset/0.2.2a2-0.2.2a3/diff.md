# Comparing `tmp/aiokwikset-0.2.2a2.tar.gz` & `tmp/aiokwikset-0.2.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokwikset-0.2.2a2.tar", last modified: Sun Jun 11 01:21:45 2023, max compression
+gzip compressed data, was "aiokwikset-0.2.2a3.tar", last modified: Sun Jun 11 19:53:13 2023, max compression
```

## Comparing `aiokwikset-0.2.2a2.tar` & `aiokwikset-0.2.2a3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:21:45.481462 aiokwikset-0.2.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-11 01:21:45.481462 aiokwikset-0.2.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:21:45.477462 aiokwikset-0.2.2a2/aiokwikset/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/aws_kwikset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:21:45.477462 aiokwikset-0.2.2a2/aiokwikset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 01:21:45.481462 aiokwikset-0.2.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:53:13.109844 aiokwikset-0.2.2a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-11 19:53:13.109844 aiokwikset-0.2.2a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:53:13.105843 aiokwikset-0.2.2a3/aiokwikset/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/aws_kwikset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/aiokwikset/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:53:13.109844 aiokwikset-0.2.2a3/aiokwikset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-11 19:53:13.000000 aiokwikset-0.2.2a3/aiokwikset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-11 19:53:13.000000 aiokwikset-0.2.2a3/aiokwikset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:53:13.000000 aiokwikset-0.2.2a3/aiokwikset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 19:53:13.000000 aiokwikset-0.2.2a3/aiokwikset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 19:53:13.000000 aiokwikset-0.2.2a3/aiokwikset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:53:12.000000 aiokwikset-0.2.2a3/aiokwikset.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:53:13.109844 aiokwikset-0.2.2a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-11 19:53:00.000000 aiokwikset-0.2.2a3/setup.py
```

### Comparing `aiokwikset-0.2.2a2/LICENSE` & `aiokwikset-0.2.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a2/PKG-INFO` & `aiokwikset-0.2.2a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokwikset
-Version: 0.2.2a2
+Version: 0.2.2a3
 Summary: Python interface for Kwikset Smart Locks
 Home-page: https://github.com/explosivo22/aiokwikset
 Author: Brad Barbour
 Author-email: barbourbj@gmail.com
 License: Apache Software License
 Keywords: kwikset,home automation,kwikset halo,kwikset smart lock
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiokwikset-0.2.2a2/README.md` & `aiokwikset-0.2.2a3/README.md`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a2/aiokwikset/api.py` & `aiokwikset-0.2.2a3/aiokwikset/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import aioboto3
 import botocore.exceptions
 import attr
 import datetime
+import traceback
 
 from typing import Optional
 from envs import env
 from jose import jwt, JWTError
 from urllib.parse import urlparse
 
 from aiohttp import ClientSession, ClientTimeout
@@ -173,14 +174,15 @@
         dec_access_token = jwt.get_unverified_claims(self.id_token)
 
         if now > datetime.datetime.fromtimestamp(dec_access_token['exp']):
             expired = True
             LOGGER.debug("Access token has expired.")
             if renew:
                 LOGGER.debug("Attempting to renew access token.")
+                LOGGER.debug(traceback.print_stack())
                 await self.renew_access_token()
         else:
             expired = False
             LOGGER.debug("Access token not expired")
         return expired
 
     async def renew_access_token(self):
```

### Comparing `aiokwikset-0.2.2a2/aiokwikset/aws_kwikset.py` & `aiokwikset-0.2.2a3/aiokwikset/aws_kwikset.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a2/aiokwikset/client.py` & `aiokwikset-0.2.2a3/aiokwikset/client.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a2/aiokwikset/const.py` & `aiokwikset-0.2.2a3/aiokwikset/const.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a2/aiokwikset/device.py` & `aiokwikset-0.2.2a3/aiokwikset/device.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a2/aiokwikset/user.py` & `aiokwikset-0.2.2a3/aiokwikset/user.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a2/aiokwikset.egg-info/PKG-INFO` & `aiokwikset-0.2.2a3/aiokwikset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokwikset
-Version: 0.2.2a2
+Version: 0.2.2a3
 Summary: Python interface for Kwikset Smart Locks
 Home-page: https://github.com/explosivo22/aiokwikset
 Author: Brad Barbour
 Author-email: barbourbj@gmail.com
 License: Apache Software License
 Keywords: kwikset,home automation,kwikset halo,kwikset smart lock
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiokwikset-0.2.2a2/setup.py` & `aiokwikset-0.2.2a3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name="aiokwikset",
-    version="0.2.2a2",
+    version="0.2.2a3",
     description="Python interface for Kwikset Smart Locks",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/explosivo22/aiokwikset",
     author="Brad Barbour",
     author_email="barbourbj@gmail.com",
     license='Apache Software License',
```

