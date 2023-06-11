# Comparing `tmp/matildapeak_scoly_api-1.0.0.tar.gz` & `tmp/matildapeak_scoly_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matildapeak_scoly_api-1.0.0.tar", max compression
+gzip compressed data, was "matildapeak_scoly_api-1.0.1.tar", max compression
```

## Comparing `matildapeak_scoly_api-1.0.0.tar` & `matildapeak_scoly_api-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3768 2023-06-11 20:16:10.582685 matildapeak_scoly_api-1.0.0/README.md
--rw-r--r--   0        0        0     1097 2023-06-11 20:16:25.028545 matildapeak_scoly_api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 20:16:10.604685 matildapeak_scoly_api-1.0.0/scoly_api/__init__.py
--rw-r--r--   0        0        0     4443 2023-06-11 20:16:10.583685 matildapeak_scoly_api-1.0.0/scoly_api/client.py
--rw-r--r--   0        0        0     4275 1970-01-01 00:00:00.000000 matildapeak_scoly_api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3823 2023-06-11 21:44:08.035863 matildapeak_scoly_api-1.0.1/README.md
+-rw-r--r--   0        0        0     1097 2023-06-11 21:44:20.948805 matildapeak_scoly_api-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-11 21:44:08.057863 matildapeak_scoly_api-1.0.1/scoly_api/__init__.py
+-rw-r--r--   0        0        0     4291 2023-06-11 21:44:08.036863 matildapeak_scoly_api-1.0.1/scoly_api/client.py
+-rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 matildapeak_scoly_api-1.0.1/PKG-INFO
```

### Comparing `matildapeak_scoly_api-1.0.0/README.md` & `matildapeak_scoly_api-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,19 @@
     )
 
 And then add sensor events, which will be transmitted to **Scoly** when the
 cache is full: -
 
     client.add_sensor_data(
         sensor="Rimmer",
-        timestamp_utc=datetime.now(),
-        data={"battery": 67, "presence": False, "celsius": 23.4, "lux": 45.6}
+        data={"timestamp": "2023-05-30T00:00:00Z",
+              "battery": 67,
+              "presence": False,
+              "celsius": 23.4,
+              "lux": 45.6}
     )
 
 By default the cache will be flushed when it contains 50 events or if the
 cache contents are older than 6 minutes. You can set your own
 values when you initialise the `ScolyAPI` instance with some extra parameters.
 To set a cache size of 10 and maximum age of 2 minutes initialise the ScolyAPI
 instance like this: -
```

### Comparing `matildapeak_scoly_api-1.0.0/pyproject.toml` & `matildapeak_scoly_api-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matildapeak-scoly-api"
-version = "1.0.0"
+version = "1.0.1"
 description = "The Scoly API Package"
 authors = ["Alan Christie <alan.christie@matildapeak.com>"]
 readme = "README.md"
 packages = [{include = "scoly_api"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `matildapeak_scoly_api-1.0.0/scoly_api/client.py` & `matildapeak_scoly_api-1.0.1/scoly_api/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,30 +57,26 @@
         self._last_transmit_success: Optional[bool] = None
 
     def flush(self) -> None:
         """Flushes cached information like the sensor event cache to scoly."""
         now_utc: datetime = datetime.now(timezone.utc)
         _ = self._transmit_sensor_event_cache(now_utc)
 
-    def add_sensor_data(
-        self, *, sensor: str, timestamp_utc: datetime, data: Dict[str, Any]
-    ) -> None:
+    def add_sensor_data(self, *, sensor: str, data: Dict[str, Any]) -> None:
         """Adds Given a sensor (name) and its data to the cache. If the cache is full
         or the cache period has been met, the cache is transmitted to scoly.
         """
         assert sensor
-        assert timestamp_utc
         assert data
 
         now_utc: datetime = datetime.now(timezone.utc)
 
         if sensor not in self._sensor_event_cache:
             self._sensor_event_cache[sensor] = []
-        sensor_data = {"timestamp": timestamp_utc.isoformat(), "data": data}
-        self._sensor_event_cache[sensor].append(sensor_data)
+        self._sensor_event_cache[sensor].append(data)
         self._sensor_cache_event_count += 1
 
         if (
             self._sensor_cache_event_count >= self._sensor_event_cache_size
             or now_utc - self._sensor_cache_timestamp_utc
             >= self._sensor_event_cache_period
         ):
```

### Comparing `matildapeak_scoly_api-1.0.0/PKG-INFO` & `matildapeak_scoly_api-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matildapeak-scoly-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: The Scoly API Package
 Author: Alan Christie
 Author-email: alan.christie@matildapeak.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -39,16 +39,19 @@
     )
 
 And then add sensor events, which will be transmitted to **Scoly** when the
 cache is full: -
 
     client.add_sensor_data(
         sensor="Rimmer",
-        timestamp_utc=datetime.now(),
-        data={"battery": 67, "presence": False, "celsius": 23.4, "lux": 45.6}
+        data={"timestamp": "2023-05-30T00:00:00Z",
+              "battery": 67,
+              "presence": False,
+              "celsius": 23.4,
+              "lux": 45.6}
     )
 
 By default the cache will be flushed when it contains 50 events or if the
 cache contents are older than 6 minutes. You can set your own
 values when you initialise the `ScolyAPI` instance with some extra parameters.
 To set a cache size of 10 and maximum age of 2 minutes initialise the ScolyAPI
 instance like this: -
```

