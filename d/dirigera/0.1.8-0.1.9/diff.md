# Comparing `tmp/dirigera-0.1.8.tar.gz` & `tmp/dirigera-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-0.1.8.tar", last modified: Thu May 25 18:02:22 2023, max compression
+gzip compressed data, was "dirigera-0.1.9.tar", last modified: Sun Jun 11 13:33:01 2023, max compression
```

## Comparing `dirigera-0.1.8.tar` & `dirigera-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.677058 dirigera-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-25 18:02:10.000000 dirigera-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-25 18:02:22.677058 dirigera-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-25 18:02:10.000000 dirigera-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-25 18:02:10.000000 dirigera-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:02:22.677058 dirigera-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:02:10.000000 dirigera-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.673058 dirigera-0.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.673058 dirigera-0.1.8/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.677058 dirigera-0.1.8/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/outlet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.677058 dirigera-0.1.8/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.673058 dirigera-0.1.8/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.677058 dirigera-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_outlet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:33:01.000330 dirigera-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-11 13:32:51.000000 dirigera-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-11 13:33:01.000330 dirigera-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-11 13:32:51.000000 dirigera-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-11 13:32:51.000000 dirigera-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 13:33:01.000330 dirigera-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 13:32:51.000000 dirigera-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:33:00.996330 dirigera-0.1.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:33:00.996330 dirigera-0.1.9/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:33:00.996330 dirigera-0.1.9/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/devices/outlet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:33:00.996330 dirigera-0.1.9/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-11 13:32:51.000000 dirigera-0.1.9/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:33:00.996330 dirigera-0.1.9/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-11 13:33:00.000000 dirigera-0.1.9/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-11 13:33:00.000000 dirigera-0.1.9/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 13:33:00.000000 dirigera-0.1.9/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-11 13:33:00.000000 dirigera-0.1.9/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-11 13:33:00.000000 dirigera-0.1.9/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-11 13:33:00.000000 dirigera-0.1.9/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:33:01.000330 dirigera-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-11 13:32:51.000000 dirigera-0.1.9/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-11 13:32:51.000000 dirigera-0.1.9/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-11 13:32:51.000000 dirigera-0.1.9/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-06-11 13:32:51.000000 dirigera-0.1.9/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-11 13:32:51.000000 dirigera-0.1.9/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-11 13:32:51.000000 dirigera-0.1.9/tests/test_outlet.py
```

### Comparing `dirigera-0.1.8/LICENSE` & `dirigera-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/PKG-INFO` & `dirigera-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.8
+Version: 0.1.9
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-0.1.8/README.md` & `dirigera-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/pyproject.toml` & `dirigera-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
    "setuptools",
    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "0.1.8"
+version = "0.1.9"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["python", "iot", "smarthome", "hub", "lighting", "ikea", "tradfri", "dirigera"]
 dependencies = [
     "requests >= 2.22.0",
```

### Comparing `dirigera-0.1.8/src/dirigera/devices/blinds.py` & `dirigera-0.1.9/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/src/dirigera/devices/controller.py` & `dirigera-0.1.9/src/dirigera/devices/controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/src/dirigera/devices/device.py` & `dirigera-0.1.9/src/dirigera/devices/device.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/src/dirigera/devices/environment_sensor.py` & `dirigera-0.1.9/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/src/dirigera/devices/light.py` & `dirigera-0.1.9/src/dirigera/devices/light.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,16 @@
         self.is_on = lamp_on
 
     def set_light_level(self, light_level: int) -> None:
         if "lightLevel" not in self.can_receive:
             raise AssertionError(
                 "This lamp does not support the set lightLevel function"
             )
-        if light_level < 0 or light_level > 100:
-            raise AssertionError("light_level must be a value between 0 and 100")
+        if light_level < 1 or light_level > 100:
+            raise AssertionError("light_level must be a value between 1 and 100")
 
         data = [{"attributes": {"lightLevel": light_level}}]
         self.dirigera_client.patch(route=f"/devices/{self.device_id}", data=data)
         self.light_level = light_level
 
     def set_color_temperature(self, color_temp: int) -> None:
         if "colorTemperature" not in self.can_receive:
```

### Comparing `dirigera-0.1.8/src/dirigera/devices/open_close_sensor.py` & `dirigera-0.1.9/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/src/dirigera/devices/outlet.py` & `dirigera-0.1.9/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-0.1.9/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/src/dirigera/hub/auth.py` & `dirigera-0.1.9/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/src/dirigera/hub/hub.py` & `dirigera-0.1.9/src/dirigera/hub/hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,14 +110,24 @@
         """
         Fetches all outlets registered in the Hub
         """
         devices = self.get("/devices")
         outlets = list(filter(lambda x: x["type"] == "outlet", devices))
         return [dict_to_outlet(outlet, self) for outlet in outlets]
 
+    def get_outlet_by_name(self, outlet_name: str) -> Outlet:
+        """
+        Fetches all outlets and returns first result that matches this name
+        """
+        outlets = self.get_outlets()
+        outlets = list(filter(lambda x: x.custom_name == outlet_name, outlets))
+        if len(outlets) == 0:
+            raise AssertionError(f"No outlet found with name {outlet_name}")
+        return outlets[0]
+
     def get_environment_sensors(self) -> List[EnvironmentSensor]:
         """
         Fetches all environment sensors registered in the Hub
         """
         devices = self.get("/devices")
         sensors = list(
             filter(lambda x: x["deviceType"] == "environmentSensor", devices)
```

### Comparing `dirigera-0.1.8/src/dirigera.egg-info/PKG-INFO` & `dirigera-0.1.9/src/dirigera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.8
+Version: 0.1.9
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-0.1.8/src/dirigera.egg-info/SOURCES.txt` & `dirigera-0.1.9/src/dirigera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/tests/test_blinds.py` & `dirigera-0.1.9/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/tests/test_controller.py` & `dirigera-0.1.9/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/tests/test_environment_sensor.py` & `dirigera-0.1.9/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/tests/test_light.py` & `dirigera-0.1.9/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/tests/test_open_close_sensor.py` & `dirigera-0.1.9/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.8/tests/test_outlet.py` & `dirigera-0.1.9/tests/test_outlet.py`

 * *Files identical despite different names*

