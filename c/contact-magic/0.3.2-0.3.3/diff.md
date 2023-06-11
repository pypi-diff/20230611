# Comparing `tmp/contact_magic-0.3.2.tar.gz` & `tmp/contact_magic-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.3.2.tar", max compression
+gzip compressed data, was "contact_magic-0.3.3.tar", max compression
```

## Comparing `contact_magic-0.3.2.tar` & `contact_magic-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.2/README.md
--rw-r--r--   0        0        0      273 2023-06-11 11:14:26.606174 contact_magic-0.3.2/contact_magic/__init__.py
--rw-r--r--   0        0        0      926 2023-06-10 13:28:29.820843 contact_magic-0.3.2/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.2/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5201 2023-06-11 11:20:08.656242 contact_magic-0.3.2/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-11 11:09:58.728061 contact_magic-0.3.2/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.2/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2151 2023-06-10 00:10:37.388687 contact_magic-0.3.2/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1471 2023-06-10 14:15:09.990381 contact_magic-0.3.2/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.2/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.2/contact_magic/logger.py
--rw-r--r--   0        0        0    12203 2023-06-11 11:19:53.677151 contact_magic-0.3.2/contact_magic/models.py
--rw-r--r--   0        0        0     2991 2023-06-10 22:11:15.757144 contact_magic-0.3.2/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.2/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.2/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.2/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.2/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.2/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.2/contact_magic/utils.py
--rw-r--r--   0        0        0     1710 2023-06-11 11:10:38.580950 contact_magic-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.3/README.md
+-rw-r--r--   0        0        0      273 2023-06-11 11:14:26.606174 contact_magic-0.3.3/contact_magic/__init__.py
+-rw-r--r--   0        0        0      977 2023-06-11 12:02:32.388322 contact_magic-0.3.3/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.3/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5201 2023-06-11 11:20:08.656242 contact_magic-0.3.3/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-11 11:09:58.728061 contact_magic-0.3.3/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.3/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2177 2023-06-11 12:02:22.673968 contact_magic-0.3.3/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.3.3/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.3/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.3/contact_magic/logger.py
+-rw-r--r--   0        0        0    12203 2023-06-11 11:19:53.677151 contact_magic-0.3.3/contact_magic/models.py
+-rw-r--r--   0        0        0     2991 2023-06-10 22:11:15.757144 contact_magic-0.3.3/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.3/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.3/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.3/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.3/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.3/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.3/contact_magic/utils.py
+-rw-r--r--   0        0        0     1710 2023-06-11 12:01:47.241837 contact_magic-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.3/PKG-INFO
```

### Comparing `contact_magic-0.3.2/README.md` & `contact_magic-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/asyncio.py` & `contact_magic-0.3.3/contact_magic/asyncio.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,10 +30,11 @@
             index, op = queue.get_nowait()
         except QueueEmpty:
             break
 
         try:
             response = await op[0](**op[1])
             results[index] = response
-        except Exception:
-            results[index] = None
+        except Exception as e:
+            # log warning
+            results[index] = {"data": {}, "index": 0}
         queue.task_done()
```

### Comparing `contact_magic-0.3.2/contact_magic/conf/settings.py` & `contact_magic-0.3.3/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/helpers.py` & `contact_magic-0.3.3/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/integrations/copyfactory.py` & `contact_magic-0.3.3/contact_magic/integrations/copyfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from contact_magic.utils import find_item
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 
 endpoint = "https://app.copyfactory.io/api/v2/generate/"
 
-headers = {"Accept": "application/json", "Authorization": SETTINGS.COPYFACTORY_API_KEY}
-
 
 def _get_rate_limit_sleep_time(response):
     """Get rate limit window expiration time from response if the response
     status code is 429.
     """
     try:
         data = response.headers
@@ -25,14 +23,18 @@
     except (AttributeError, KeyError, ValueError):
         return 60
 
 
 async def make_copyfactory_request(premise_id: int, variables: dict, max_retries=3):
     if not SETTINGS.COPYFACTORY_API_KEY:
         return None
+    headers = {
+        "Accept": "application/json",
+        "Authorization": SETTINGS.COPYFACTORY_API_KEY,
+    }
     data = {
         "premise_id": premise_id,
         "variables": variables,
     }
     try:
         session = httpx.AsyncClient(timeout=90)
         retries = 0
```

### Comparing `contact_magic-0.3.2/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.3.3/contact_magic/integrations/sales_scrapers.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 from contact_magic.logger import logger
 from contact_magic.utils import fix_website
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 base_url = "https://salesscrapers.dev/api/"
 
-headers = {"Accept": "application/json", "X-API-Key": SETTINGS.SALES_SCRAPERS_API_KEY}
-
 
 async def make_sales_scraper_request(endpoint, data: dict, max_retries=3):
     if not SETTINGS.SALES_SCRAPERS_API_KEY:
         return None
+    headers = {
+        "Accept": "application/json",
+        "X-API-Key": SETTINGS.SALES_SCRAPERS_API_KEY,
+    }
+
     url = f"{base_url}{endpoint}"
     try:
         session = httpx.AsyncClient(timeout=120)
         retries = 0
         while retries < max_retries:
             res = await session.request(
                 method="get", url=url, headers=headers, params=data
```

### Comparing `contact_magic-0.3.2/contact_magic/integrations/sheets.py` & `contact_magic-0.3.3/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/models.py` & `contact_magic-0.3.3/contact_magic/models.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/preprocessors.py` & `contact_magic-0.3.3/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/scripts/agency.py` & `contact_magic-0.3.3/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/scripts/run_workflows.py` & `contact_magic-0.3.3/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.3.3/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/contact_magic/utils.py` & `contact_magic-0.3.3/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.2/pyproject.toml` & `contact_magic-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.3.2"
+version = "0.3.3"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.3.2/PKG-INFO` & `contact_magic-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.3.2
+Version: 0.3.3
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

