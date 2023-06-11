# Comparing `tmp/findmyorder-1.4.0.tar.gz` & `tmp/findmyorder-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.4.0.tar", max compression
+gzip compressed data, was "findmyorder-1.4.1.tar", max compression
```

## Comparing `findmyorder-1.4.0.tar` & `findmyorder-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-10 08:36:39.679722 findmyorder-1.4.0/LICENSE
--rw-r--r--   0        0        0     1995 2023-06-10 08:36:39.679722 findmyorder-1.4.0/README.md
--rw-r--r--   0        0        0      113 2023-06-10 08:36:55.536697 findmyorder-1.4.0/findmyorder/__init__.py
--rw-r--r--   0        0        0      629 2023-06-10 08:36:39.679722 findmyorder-1.4.0/findmyorder/config.py
--rw-r--r--   0        0        0      686 2023-06-10 08:36:39.679722 findmyorder-1.4.0/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5703 2023-06-10 08:36:39.679722 findmyorder-1.4.0/findmyorder/main.py
--rw-r--r--   0        0        0     1745 2023-06-10 08:36:55.532697 findmyorder-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-10 12:45:06.491847 findmyorder-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1995 2023-06-10 12:45:06.491847 findmyorder-1.4.1/README.md
+-rw-r--r--   0        0        0      113 2023-06-10 12:45:20.764070 findmyorder-1.4.1/findmyorder/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-10 12:45:06.491847 findmyorder-1.4.1/findmyorder/config.py
+-rw-r--r--   0        0        0     2238 2023-06-10 12:45:06.491847 findmyorder-1.4.1/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5555 2023-06-10 12:45:06.491847 findmyorder-1.4.1/findmyorder/main.py
+-rw-r--r--   0        0        0     1745 2023-06-10 12:45:20.764070 findmyorder-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.4.1/PKG-INFO
```

### Comparing `findmyorder-1.4.0/LICENSE` & `findmyorder-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.0/README.md` & `findmyorder-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.0/findmyorder/config.py` & `findmyorder-1.4.1/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.4.0/findmyorder/main.py` & `findmyorder-1.4.1/findmyorder/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
  FindMyOrder Main
 """
 import logging
 from datetime import datetime
 
-from emoji import is_emoji
+import emoji
 from pyparsing import (
     Combine, Optional, Word, alphas,
     nums, one_of, pyparsing_common, Suppress)
 
 from .config import settings
 
 
@@ -21,28 +21,24 @@
         self.logger = logging.getLogger(name="FMO")
 
     async def search(
         self,
         my_string: str,
     ) -> bool:
         """Search an order."""
-        try:
-            if my_string:
-                string_check = my_string.split()[0].lower()
-                if string_check in settings.action_identifier.lower():
-                    return True
-            return False
-        except Exception as e:
-            return e
+        if my_string:
+            string_check = my_string.split()[0].lower()
+            if string_check in settings.action_identifier.lower():
+                return True
+        return False
+
 
     async def contains_emoji(self, input_string: str) -> bool:
         """Check if the input string contains an emoji."""
-        print(input_string)
-        return is_emoji(input_string)
-
+        return any(emoji.is_emoji(character) for character in input_string)
 
     async def identify_order(
             self,
             my_string: str,
             ) -> dict:
         """Identify an order."""
         try:
@@ -98,37 +94,34 @@
             return e
 
     async def get_order(
         self,
         msg: str,
     ):
         """get an order."""
-        try:
-            logging.debug("get_order %s", msg)
 
-            if await self.search(msg):
-                order = await self.identify_order(msg)
-                if isinstance(order, dict):
-                    order["timestamp"] = datetime.utcnow().strftime(
-                        "%Y-%m-%dT%H:%M:%SZ")
-                if settings.instrument_mapping:
-                    self.replace_symbol(order)
-                return order
-            return None
+        if await self.search(msg):
+            order = await self.identify_order(msg)
+            if isinstance(order, dict):
+                order["timestamp"] = datetime.utcnow().strftime(
+                    "%Y-%m-%dT%H:%M:%SZ")
+            print(settings.instrument_mapping)
+            if settings.instrument_mapping:
+                await self.replace_instrument(order)
+            return order
+        return None
 
-        except Exception as e:
-            return e
+    async def replace_instrument(self, order):
+        instrument = order["instrument"]
+        for item in settings.mapping:
+            if item["id"] == instrument:
+                order["instrument"] = item["alt"]
+                break
+        return order
 
-    async def replace_symbol(
-        self, 
-        order: dict,):
-        symbol = order["instrument"]
-        if symbol in settings.mapping:
-            order["instrument"] = settings.mapping[symbol]
-            return order
 # Grammar
 # class TradingGrammar:
 #     def __init__(self):
 #         self.action = self._action()
 #         self.instrument = self._instrument()
 #         self.exchange = self._exchange()
```

### Comparing `findmyorder-1.4.0/pyproject.toml` & `findmyorder-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.4.0"
+version = "1.4.1"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
```

### Comparing `findmyorder-1.4.0/PKG-INFO` & `findmyorder-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.4.0
+Version: 1.4.1
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

