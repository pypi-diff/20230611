# Comparing `tmp/ayla_iot_unofficial-1.0.0.tar.gz` & `tmp/ayla_iot_unofficial-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayla_iot_unofficial-1.0.0.tar", last modified: Sun Jun 11 02:54:50 2023, max compression
+gzip compressed data, was "ayla_iot_unofficial-1.0.1.tar", last modified: Sun Jun 11 15:58:51 2023, max compression
```

## Comparing `ayla_iot_unofficial-1.0.0.tar` & `ayla_iot_unofficial-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:54:50.723646 ayla_iot_unofficial-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-11 02:54:50.723646 ayla_iot_unofficial-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 02:54:50.723646 ayla_iot_unofficial-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:54:50.719646 ayla_iot_unofficial-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:54:50.723646 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16289 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/ayla_iot_unofficial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    28291 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-11 02:54:39.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:54:50.723646 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-11 02:54:50.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-11 02:54:50.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:54:50.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-11 02:54:50.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-11 02:54:50.000000 ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:58:51.412529 ayla_iot_unofficial-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-11 15:58:51.412529 ayla_iot_unofficial-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 15:58:51.412529 ayla_iot_unofficial-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:58:51.408529 ayla_iot_unofficial-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:58:51.412529 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16287 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/ayla_iot_unofficial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-11 15:58:38.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:58:51.412529 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-11 15:58:51.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-11 15:58:51.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:58:51.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-11 15:58:51.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-11 15:58:51.000000 ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial.egg-info/top_level.txt
```

### Comparing `ayla_iot_unofficial-1.0.0/LICENSE` & `ayla_iot_unofficial-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ayla_iot_unofficial-1.0.0/PKG-INFO` & `ayla_iot_unofficial-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayla_iot_unofficial
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API for Ayla IoT products
 Home-page: https://github.com/rewardone/ayla-iot-unofficial
 Author: Reward One
 Author-email: Reward One <rewardone@gmail.com>
 Project-URL: Homepage, https://github.com/rewardone/ayla-iot-unofficial
 Project-URL: Bug Tracker, https://github.com/rewardone/ayla-iot-unofficial/issues
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,22 @@
 Intended to be generic for multi-device use.
 
 Designed primarily to be a support package for [Home Assistant](https://www.home-assistant.io/) integrations.
 
 This library is heavily based off of [sharkiq](https://github.com/JeffResc/sharkiq) by [@JeffResc](https://github.com/JeffResc).
 
 [PyPi](https://pypi.org/project/ayla-iot-unofficial/)
+
+# Ayla References
+This device is integrated by/with Ayla Networks and (generally) uses their documentation. 
+
+These can be used as starting references:
+* https://developer.aylanetworks.com/apibrowser
+* https://docs.aylanetworks.com/reference/getting_started
+* https://connection.aylanetworks.com/s/article/2080270
  
 ## Installation
 From PyPi
 ```bash
 pip install ayla-iot-unofficial
 ```
```

### Comparing `ayla_iot_unofficial-1.0.0/README.md` & `ayla_iot_unofficial-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 Intended to be generic for multi-device use.
 
 Designed primarily to be a support package for [Home Assistant](https://www.home-assistant.io/) integrations.
 
 This library is heavily based off of [sharkiq](https://github.com/JeffResc/sharkiq) by [@JeffResc](https://github.com/JeffResc).
 
 [PyPi](https://pypi.org/project/ayla-iot-unofficial/)
+
+# Ayla References
+This device is integrated by/with Ayla Networks and (generally) uses their documentation. 
+
+These can be used as starting references:
+* https://developer.aylanetworks.com/apibrowser
+* https://docs.aylanetworks.com/reference/getting_started
+* https://connection.aylanetworks.com/s/article/2080270
  
 ## Installation
 From PyPi
 ```bash
 pip install ayla-iot-unofficial
 ```
```

### Comparing `ayla_iot_unofficial-1.0.0/pyproject.toml` & `ayla_iot_unofficial-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ayla_iot_unofficial"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Reward One", email="rewardone@gmail.com" },
 ]
 description = "Python API for Ayla IoT products"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ayla_iot_unofficial-1.0.0/setup.py` & `ayla_iot_unofficial-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/ayla_iot_unofficial.py` & `ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/ayla_iot_unofficial.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 """
 
 from aiohttp    import ClientSession             # async http
 from requests   import post, request, Response   # http request library
 from datetime   import datetime, timedelta       # datetime operations
 from typing     import Dict, List, Optional      # object types
 
+from .const import (
+    EU_USER_FIELD_BASE,
+    EU_ADS_BASE,
+    EU_RULESSERVICE_BASE,
+    USER_FIELD_BASE,
+    ADS_BASE,
+    RULESSERVICE_BASE
+)
+
 # Custom error handling 
 from .exc import (
     AylaError,
     AylaAuthError,
     AylaAuthExpiringError,
     AylaNotAuthedError,
     AylaReadOnlyPropertyError,
@@ -50,20 +59,20 @@
         self._refresh_token     = None          # type: Optional[str]
         self._auth_expiration   = None          # type: Optional[datetime]
         self._is_authed         = False         # type: bool
         self._app_id            = app_id
         self._app_secret        = app_secret
         self.websession         = websession
         self.europe             = europe
-        self.eu_user_field_url  = "https://user-field-eu.aylanetworks.com"
-        self.eu_ads_url         = "https://ads-eu.aylanetworks.com"
-        self.eu_rulesservice_url= "https://rulesservice-field-eu.aylanetworks.com"
-        self.user_field_url     = "https://user-field.aylanetworks.com"
-        self.ads_url            = "https://ads-field.aylanetworks.com"
-        self.rulesservice_url   = "https://rulesservice-field.aylanetworks.com"
+        self.eu_user_field_url  = EU_USER_FIELD_BASE
+        self.eu_ads_url         = EU_ADS_BASE
+        self.eu_rulesservice_url= EU_RULESSERVICE_BASE
+        self.user_field_url     = USER_FIELD_BASE
+        self.ads_url            = ADS_BASE
+        self.rulesservice_url   = RULESSERVICE_BASE
 
     async def ensure_session(self) -> ClientSession:
         """Ensure that we have an aiohttp ClientSession"""
         if self.websession is None:
             self.websession = ClientSession()
         return self.websession
```

### Comparing `ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/device.py` & `ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,15 +587,15 @@
             Needs testing. Set vacation mode value from 0 (default) to 255 (max).
             Properties and values may vary per manufacturer.
         """
         PropertyName    = "set_vacation_mode"
         PropertyValue   = 255
         self.set_property_value(PropertyName, PropertyValue)
 
-    async def start_vacation_mode(self):
+    async def async_start_vacation_mode(self):
         """
             Needs testing. Set vacation mode value from 0 (default) to 255 (max).
             Properties and values may vary per manufacturer.
         """
         PropertyName    = "set_vacation_mode"
         PropertyValue   = 255
         await self.async_set_property_value(PropertyName, PropertyValue)
@@ -605,15 +605,15 @@
             Needs testing. Set vacation mode value from 255 (max) to 0 (default).
             Properties and values may vary per manufacturer.
         """
         PropertyName    = "set_vacation_mode"
         PropertyValue   = 0
         self.set_property_value(PropertyName, PropertyValue)
 
-    async def stop_vacation_mode(self):
+    async def async_stop_vacation_mode(self):
         """
             Needs testing. Set vacation mode value from 255 (max) to 0 (default).
             Properties and values may vary per manufacturer.
         """
         PropertyName    = "set_vacation_mode"
         PropertyValue   = 0
         await self.async_set_property_value(PropertyName, PropertyValue)
```

### Comparing `ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial/exc.py` & `ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial/exc.py`

 * *Files identical despite different names*

### Comparing `ayla_iot_unofficial-1.0.0/src/ayla_iot_unofficial.egg-info/PKG-INFO` & `ayla_iot_unofficial-1.0.1/src/ayla_iot_unofficial.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayla-iot-unofficial
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API for Ayla IoT products
 Home-page: https://github.com/rewardone/ayla-iot-unofficial
 Author: Reward One
 Author-email: Reward One <rewardone@gmail.com>
 Project-URL: Homepage, https://github.com/rewardone/ayla-iot-unofficial
 Project-URL: Bug Tracker, https://github.com/rewardone/ayla-iot-unofficial/issues
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,22 @@
 Intended to be generic for multi-device use.
 
 Designed primarily to be a support package for [Home Assistant](https://www.home-assistant.io/) integrations.
 
 This library is heavily based off of [sharkiq](https://github.com/JeffResc/sharkiq) by [@JeffResc](https://github.com/JeffResc).
 
 [PyPi](https://pypi.org/project/ayla-iot-unofficial/)
+
+# Ayla References
+This device is integrated by/with Ayla Networks and (generally) uses their documentation. 
+
+These can be used as starting references:
+* https://developer.aylanetworks.com/apibrowser
+* https://docs.aylanetworks.com/reference/getting_started
+* https://connection.aylanetworks.com/s/article/2080270
  
 ## Installation
 From PyPi
 ```bash
 pip install ayla-iot-unofficial
 ```
```

