# Comparing `tmp/talkytrend-1.1.2.tar.gz` & `tmp/talkytrend-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.1.2.tar", max compression
+gzip compressed data, was "talkytrend-1.1.3.tar", max compression
```

## Comparing `talkytrend-1.1.2.tar` & `talkytrend-1.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-11 09:53:37.286756 talkytrend-1.1.2/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-11 09:53:37.286756 talkytrend-1.1.2/README.md
--rw-r--r--   0        0        0     1669 2023-06-11 09:53:58.934991 talkytrend-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-11 09:53:58.934991 talkytrend-1.1.2/talkytrend/__init__.py
--rw-r--r--   0        0        0      630 2023-06-11 09:53:37.286756 talkytrend-1.1.2/talkytrend/config.py
--rw-r--r--   0        0        0      765 2023-06-11 09:53:37.286756 talkytrend-1.1.2/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     3508 2023-06-11 09:53:37.286756 talkytrend-1.1.2/talkytrend/main.py
--rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 talkytrend-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-11 11:10:59.545361 talkytrend-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-11 11:10:59.545361 talkytrend-1.1.3/README.md
+-rw-r--r--   0        0        0     1669 2023-06-11 11:11:16.141323 talkytrend-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-11 11:11:16.141323 talkytrend-1.1.3/talkytrend/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-11 11:10:59.545361 talkytrend-1.1.3/talkytrend/config.py
+-rw-r--r--   0        0        0      765 2023-06-11 11:10:59.545361 talkytrend-1.1.3/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     3675 2023-06-11 11:10:59.545361 talkytrend-1.1.3/talkytrend/main.py
+-rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 talkytrend-1.1.3/PKG-INFO
```

### Comparing `talkytrend-1.1.2/LICENSE` & `talkytrend-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.2/README.md` & `talkytrend-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.2/pyproject.toml` & `talkytrend-1.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.1.2"
+version = "1.1.3"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.1.2/talkytrend/config.py` & `talkytrend-1.1.3/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.2/talkytrend/default_settings.toml` & `talkytrend-1.1.3/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.2/talkytrend/main.py` & `talkytrend-1.1.3/talkytrend/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 from tradingview_ta import TA_Handler, Interval
 
 from talkytrend import __version__
 from .config import settings
 
 class TalkyTrend:
     def __init__(self):
-        self.economic_calendar = settings.economic_calendar
-        self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else None
         self.enabled = settings.talkytrend_status
         self.assets = settings.assets
         self.asset_signals = {"15m": None, "1h": None, "4h": None}
+        self.economic_calendar = settings.economic_calendar
+        self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else None
+        self.live_tv = settings.live_tv_url
 
     async def fetch_analysis(
         self,
         asset_id,
         exchange,
         screener,
         interval):
@@ -86,15 +87,18 @@
 
     async def scanner(self):
         while True:
             tasks = [self.check_signal()]
             tasks.append(self.fetch_key_events())
             tasks.append(self.fetch_key_news())
             results = await asyncio.gather(*tasks)
+            if results[0] is not None:
+                print("Key signal:", results[0])
+                yield results[0]
             if results[1] is not None:
                 print("Key event:", results[1])
+                yield results[1]
             if results[2] is not None:
                 print("Key news:", results[2]["title"])
+                yield results[2]
             await asyncio.sleep(settings.scanner_frequency)
 
-    async def live_tv(self):
-        return settings.live_tv_url
```

### Comparing `talkytrend-1.1.2/PKG-INFO` & `talkytrend-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.1.2
+Version: 1.1.3
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

