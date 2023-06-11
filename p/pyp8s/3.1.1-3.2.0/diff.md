# Comparing `tmp/pyp8s-3.1.1-py3-none-any.whl.zip` & `tmp/pyp8s-3.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19046 bytes, number of entries: 10
--rw-r--r--  2.0 unx      298 b- defN 23-May-11 01:50 pyp8s/__init__.py
--rw-r--r--  2.0 unx      250 b- defN 23-May-11 01:50 pyp8s/_version.py
--rw-r--r--  2.0 unx    11426 b- defN 23-May-11 01:50 pyp8s/metrics.py
--rw-r--r--  2.0 unx      226 b- defN 23-May-11 01:50 tests/__init__.py
--rw-r--r--  2.0 unx     1300 b- defN 23-May-11 01:50 tests/test_import.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2462 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      747 b- defN 23-May-11 01:50 pyp8s-3.1.1.dist-info/RECORD
-10 files, 51962 bytes uncompressed, 17792 bytes compressed:  65.8%
+Zip file size: 19299 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      298 b- defN 23-Jun-11 02:56 pyp8s/__init__.py
+-rw-r--r--  2.0 unx      250 b- defN 23-Jun-11 02:56 pyp8s/_version.py
+-rw-r--r--  2.0 unx    11751 b- defN 23-Jun-11 02:56 pyp8s/metrics.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Jun-11 02:56 tests/__init__.py
+-rw-r--r--  2.0 unx     1300 b- defN 23-Jun-11 02:56 tests/test_import.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2937 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      747 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/RECORD
+10 files, 52762 bytes uncompressed, 18045 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_import.py
 Comment: 
 
-Filename: pyp8s-3.1.1.dist-info/LICENSE
+Filename: pyp8s-3.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyp8s-3.1.1.dist-info/METADATA
+Filename: pyp8s-3.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pyp8s-3.1.1.dist-info/WHEEL
+Filename: pyp8s-3.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyp8s-3.1.1.dist-info/top_level.txt
+Filename: pyp8s-3.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyp8s-3.1.1.dist-info/RECORD
+Filename: pyp8s-3.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyp8s/_version.py

```diff
@@ -1,8 +1,8 @@
 #!/usr/bin/env python3
 # pylint: disable=line-too-long, missing-function-docstring, logging-fstring-interpolation
 # pylint: disable=too-many-locals, broad-except, too-many-arguments, raise-missing-from
 """
     pyp8s module
 """
 
-__version__ = "3.1.1"
+__version__ = "3.2.0"
```

## pyp8s/metrics.py

```diff
@@ -192,14 +192,35 @@
         try:
             self.server.shutdown()
         except Exception as e:
             logging.error(f"Couldn't shutdown the metrics server: {e}")
             raise e
 
     @staticmethod
+    def render():
+        self = MetricsHandler()
+        result = []
+        for metric_name, metric_item in self.get_metrics().items():
+
+            help_header = f"""# HELP {metric_name} {metric_item.get_help()}\n"""
+            result.append(help_header)
+
+            type_header = f"""# TYPE {metric_name} {metric_item.get_type()}\n"""
+            result.append(type_header)
+
+            for _, labelset in metric_item.get_labelsets().items():
+                metric_value = labelset['value']
+                metric_labels_formatted_joined = ",".join(labelset['labels_formatted'])
+
+                metric_line = f"""{metric_name}{{{metric_labels_formatted_joined}}} {metric_value}\n"""
+                result.append(metric_line)
+
+        return "".join(result)
+
+    @staticmethod
     def get_metrics():
         self = MetricsHandler()
         return self.metrics
 
     @staticmethod
     def get_metric(metric_name):
         self = MetricsHandler()
@@ -255,21 +276,24 @@
 
         self = MetricsHandler()
 
         metric = self.__get_metric_obj(metric_name=metric_name)
         metric.set(value=value, **kwargs)
 
     @staticmethod
-    def init(metric_name, metric_type, description=None):
+    def init(metric_name, metric_type, description=None, init_value=None):
         self = MetricsHandler()
 
         metric = self.__get_metric_obj(metric_name=metric_name)
         metric.set_help(description)
         metric.set_type(metric_type)
 
+        if init_value is not None:
+            metric.set(value=init_value)
+
 
 class ReqHandlerMetrics(BaseHTTPRequestHandler):
 
     MetricsHandler.init("http_get_requests", "counter", "Number GET requests accepted")
     MetricsHandler.init("http_get_metrics", "counter", "Number times the metrics endpoint was called")
 
     def do_GET(self):
@@ -281,30 +305,15 @@
         if self.path == "/":
             MetricsHandler.inc("http_get_index", 1)
             header = """<html><head><title>pyp8s Exporter</title></head><body><p><a href="/metrics">Metrics</a></p></body></html>\n"""
             self.wfile.write(bytes(header, "utf-8"))
 
         elif self.path == "/metrics":
             MetricsHandler.inc("http_get_metrics", 1)
-
-            for metric_name, metric_item in MetricsHandler.get_metrics().items():
-
-                help_header = f"""# HELP {metric_name} {metric_item.get_help()}\n"""
-                self.wfile.write(bytes(help_header, "utf-8"))
-
-                type_header = f"""# TYPE {metric_name} {metric_item.get_type()}\n"""
-                self.wfile.write(bytes(type_header, "utf-8"))
-
-                for _, labelset in metric_item.get_labelsets().items():
-                    metric_value = labelset['value']
-                    metric_labels_formatted_joined = ",".join(labelset['labels_formatted'])
-
-                    metric_line = f"""{metric_name}{{{metric_labels_formatted_joined}}} {metric_value}\n"""
-                    self.wfile.write(bytes(metric_line, "utf-8"))
-
+            self.wfile.write(bytes(MetricsHandler.render(), "utf-8"))
 
         else:
             response = {"error": True, "message": "Bad request, bad"}
             self.wfile.write(json.dumps(response))
 
 
 class ThreadedHTTPServer(ThreadingMixIn, HTTPServer):
@@ -321,14 +330,15 @@
             logging.StreamHandler()
         ]
     )
 
     MetricsHandler.init("calls", "counter", "Number of calls I've received")
     MetricsHandler.init("doorbells", "counter", "Number of doorbells I've answered")
     MetricsHandler.init("yawns", "counter", "Quite self-explanatory")
+    MetricsHandler.init("giggles", "counter", "Not what you thought it was", init_value=10)
 
     MetricsHandler.inc("calls", 1)
     MetricsHandler.inc("calls", 1, who="telemarketers", when="morning")
     MetricsHandler.inc("calls", 1, who="collectors", when="all_day")
     MetricsHandler.inc("calls", 1, who="collectors", when="all_day")
     MetricsHandler.inc("calls", 1, who="collectors", when="all_day")
     MetricsHandler.inc("calls", 1, who="collectors", when="all_day")
@@ -350,12 +360,13 @@
         "if": "fi",
     }
 
     MetricsHandler.set("busy", 200, **small_hack)
     MetricsHandler.set("busy", 4, **{"for": "the", "gods": "sake", "please": "stop"})
 
     logging.info(f"Metrics: {MetricsHandler.get_metrics()}")
+    logging.info(f"Rendered: {MetricsHandler.render()}")
 
     MetricsHandler.serve(listen_address="127.0.0.1", listen_port=9000)
     logging.debug("Waiting before shutdown")
     time.sleep(20)
     MetricsHandler.shutdown()
```

## Comparing `pyp8s-3.1.1.dist-info/LICENSE` & `pyp8s-3.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyp8s-3.1.1.dist-info/METADATA` & `pyp8s-3.2.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp8s
-Version: 3.1.1
+Version: 3.2.0
 Summary: Customisable prometheus exporter for your python application
 Home-page: https://github.com/pyp8s/pyp8s
 Author: Pavel Kim
 Author-email: hello@pavelkim.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -37,14 +37,15 @@
 
     meh.serve(listen_address="0.0.0.0", listen_port=8081)
 
     meh.init("calls", "counter", "Number of calls I've received")
     meh.init("doorbells", "counter", "Number of doorbells I've answered")
     meh.init("yawns", "counter", "Quite self-explanatory")
     meh.init("mood", "gauge", "How do I feel myself from 1 to good enough")
+    meh.init("giggles", "counter", "Measurement of the joke power.", init_value=0)
 
     meh.inc("calls", 1)
 
     meh.inc("doorbells", 100, can="have", extra="labels", since="2.1.0")
     meh.inc("doorbells", 9000, this="will", be="useful")
 
     meh.inc("yawns", 8, satisfying="yes")
@@ -75,16 +76,34 @@
 # HELP yawns Quite self-explanatory
 # TYPE yawns counter
 yawns{satisfying="yes"} 8
 yawns{satisfying="no",loud="yes"} 1
 # HELP mood How do I feel myself from 1 to good enough
 # TYPE mood gauge
 mood{} 6
+# HELP giggles Measurement of the joke power.
+# TYPE giggles counter
+giggles{} -50
 ```
 
+## Usage without starting a server
+
+When you only need this thing to collect and render metrics:
+
+```python
+from pyp8s import MetricsHandler as meh
+
+if __name__ == '__main__':
+    meh.init("calls", "counter", "Number of calls I've received")
+
+    print(meh.render())
+```
+
+`render()` returns a string object.
+
 ## Test environment
 
 ```bash
 python3.10 -m virtualenv --prompt="py3.10 pyp8s" .virtualenv
 source .virtualenv/bin/activate
 ```
```

