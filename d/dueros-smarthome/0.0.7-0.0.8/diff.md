# Comparing `tmp/dueros_smarthome-0.0.7.tar.gz` & `tmp/dueros_smarthome-0.0.8.tar.gz`

## Comparing `dueros_smarthome-0.0.7.tar` & `dueros_smarthome-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/src/dueros_smarthome/__init__.py
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/src/dueros_smarthome/client.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/src/dueros_smarthome/const.py
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/src/dueros_smarthome/models.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/LICENSE
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/README.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/src/dueros_smarthome/__init__.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/src/dueros_smarthome/client.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/src/dueros_smarthome/const.py
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/src/dueros_smarthome/models.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/LICENSE
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/README.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dueros_smarthome-0.0.8/PKG-INFO
```

### Comparing `dueros_smarthome-0.0.7/.github/workflows/publish-to-pypi.yml` & `dueros_smarthome-0.0.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `dueros_smarthome-0.0.7/src/dueros_smarthome/client.py` & `dueros_smarthome-0.0.8/src/dueros_smarthome/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,34 @@
 
 class ResponseCommon:
     def __init__(self, response: dict):
         self._status = response[const.STATUS]
         self._msg = response[const.MSG]
         self._log_id = response[const.LOGID]
 
+    @property
+    def status(self):
+        return self._status
+
+    @property
+    def msg(self):
+        return self._msg
+
+    @property
+    def log_id(self):
+        return self._log_id
+
 class GetDeviceListResponse(ResponseCommon):
     def __init__(self, response: dict):
         super().__init__(response)
         self._appliances = [models.Appliance(appliance) for appliance in response[const.DATA][const.APPLIANCES]]
+    
+    @property
+    def appliances(self):
+        return self._appliances
 
 class DeviceActionResponse(ResponseCommon):
     def __init__(self, response: dict):
         super().__init__(response)
 
 class Request:
     def __init__(self, namespace: str, name: str, payload: dict, payloadVersion: int = const.DEFAULT_PAYLOAD_VERSION):
@@ -37,17 +53,17 @@
     def __init__(self, appliance_id: str):
         payload = get_device_action_request_payload(appliance_id)
         super().__init__(const.CONTROL_REQUEST_NAMESPACE, const.TURN_ON_REQUEST, payload)
 
 class SetBrightnessPercentageRequest(Request):
     def __init__(self, appliance_id: str, brightness: models.Brightness):
         payload = get_device_action_request_payload(appliance_id)
-        payload[const.BRIGHTNESS] = {const.VALUE: brightness.percentage()}
+        payload[const.BRIGHTNESS] = {const.VALUE: brightness.percentage}
         payload[const.REQUEST_PARAMETERS][const.ATTRIBUTE] = const.BRIGHTNESS
-        payload[const.REQUEST_PARAMETERS][const.ATTRIBUTE_VALUE] = brightness.percentage()
+        payload[const.REQUEST_PARAMETERS][const.ATTRIBUTE_VALUE] = brightness.percentage
         super().__init__(const.CONTROL_REQUEST_NAMESPACE, const.SET_BRIGHTNESS_PERCENTAGE_REQUEST, payload)
 
 class SetColorTemperatureRequest(Request):
     def __init__(self, appliance_id: str, color_temp: models.ColorTemperatureInKelvin):
         payload = get_device_action_request_payload(appliance_id)
         payload[const.COLOR_TEMPERATURE_IN_KELVIN] = color_temp.percentage()
         payload[const.REQUEST_PARAMETERS][const.ATTRIBUTE] = const.COLOR_TEMPERATURE_IN_KELVIN
@@ -57,15 +73,19 @@
 class SmartHomeClient:
     def __init__(self, bduss: str, host: str = const.DEFAULT_HOST, schema: str = const.DEFAULT_SCHEMA) -> None:
         self._host = host
         self._schema = schema
         self._bduss = bduss
         self._cookies = httpx.Cookies()
         self._cookies.set(const.BDUSS_COOKIE_KEY, self._bduss, domain = self._host)
-
+    
+    @property
+    def host(self):
+        return self._host
+    
     def _get_device_list_url(self) -> str:
         return f'{self._schema}{self._host}{const.DEVICE_LIST_QUERY}'
 
     async def get_device_list(self) -> GetDeviceListResponse:
         async with httpx.AsyncClient() as client:
             response = await client.get(self._get_device_list_url(), cookies=self._cookies)
             return GetDeviceListResponse(response.json())
```

### Comparing `dueros_smarthome-0.0.7/src/dueros_smarthome/const.py` & `dueros_smarthome-0.0.8/src/dueros_smarthome/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,11 +55,13 @@
 MODE = "mode"
 ICON_URL = "icon"
 BRIGHTNESS_AND_COLOR_TEMPERATURE = "brightnessAndColorTemperature"
 BRIGHTNESS_AND_COLOR_TEMPERATURE_WITH_ICON = "brightnessAndColorTemperatureWithIcon"
 ICON_URLS = "icons"
 STATUS = "status"
 
+STATUS_OK = 0
+
 TURN_OFF_REQUEST = "TurnOffRequest"
 TURN_ON_REQUEST = "TurnOnRequest"
 SET_BRIGHTNESS_PERCENTAGE_REQUEST = "SetBrightnessPercentageRequest"
 SET_COLOR_TEMPERATURE_REQUEST = "SetColorTemperatureRequest"
```

### Comparing `dueros_smarthome-0.0.7/.gitignore` & `dueros_smarthome-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dueros_smarthome-0.0.7/LICENSE` & `dueros_smarthome-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dueros_smarthome-0.0.7/pyproject.toml` & `dueros_smarthome-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dueros_smarthome"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Shaoyu Zhang", email="zsy056@gmail.com" },
 ]
 description = "Duer OS SmartHome APIs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dueros_smarthome-0.0.7/PKG-INFO` & `dueros_smarthome-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dueros_smarthome
-Version: 0.0.7
+Version: 0.0.8
 Summary: Duer OS SmartHome APIs
 Project-URL: Homepage, https://github.com/zsy056/dueros-smarthome
 Project-URL: Bug Tracker, https://github.com/zsy056/dueros-smarthome/issues
 Author-email: Shaoyu Zhang <zsy056@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

