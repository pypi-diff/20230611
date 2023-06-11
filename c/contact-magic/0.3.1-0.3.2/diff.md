# Comparing `tmp/contact_magic-0.3.1.tar.gz` & `tmp/contact_magic-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.3.1.tar", max compression
+gzip compressed data, was "contact_magic-0.3.2.tar", max compression
```

## Comparing `contact_magic-0.3.1.tar` & `contact_magic-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.1/README.md
--rw-r--r--   0        0        0      210 2023-06-11 10:15:21.249868 contact_magic-0.3.1/contact_magic/__init__.py
--rw-r--r--   0        0        0      926 2023-06-10 13:28:29.820843 contact_magic-0.3.1/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.1/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     4996 2023-06-11 10:23:59.826220 contact_magic-0.3.1/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-10 00:10:37.387140 contact_magic-0.3.1/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.1/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2151 2023-06-10 00:10:37.388687 contact_magic-0.3.1/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1471 2023-06-10 14:15:09.990381 contact_magic-0.3.1/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.1/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.1/contact_magic/logger.py
--rw-r--r--   0        0        0    11917 2023-06-10 22:11:15.895054 contact_magic-0.3.1/contact_magic/models.py
--rw-r--r--   0        0        0     2991 2023-06-10 22:11:15.757144 contact_magic-0.3.1/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.1/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.1/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.1/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4083 2023-06-10 00:10:37.399377 contact_magic-0.3.1/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.1/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.1/contact_magic/utils.py
--rw-r--r--   0        0        0     1710 2023-06-11 10:23:34.527712 contact_magic-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.2/README.md
+-rw-r--r--   0        0        0      273 2023-06-11 11:14:26.606174 contact_magic-0.3.2/contact_magic/__init__.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:28:29.820843 contact_magic-0.3.2/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.2/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5201 2023-06-11 11:20:08.656242 contact_magic-0.3.2/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-11 11:09:58.728061 contact_magic-0.3.2/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.2/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2151 2023-06-10 00:10:37.388687 contact_magic-0.3.2/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1471 2023-06-10 14:15:09.990381 contact_magic-0.3.2/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.2/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.2/contact_magic/logger.py
+-rw-r--r--   0        0        0    12203 2023-06-11 11:19:53.677151 contact_magic-0.3.2/contact_magic/models.py
+-rw-r--r--   0        0        0     2991 2023-06-10 22:11:15.757144 contact_magic-0.3.2/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.2/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.2/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.2/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.2/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.2/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.2/contact_magic/utils.py
+-rw-r--r--   0        0        0     1710 2023-06-11 11:10:38.580950 contact_magic-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.2/PKG-INFO
```

### Comparing `contact_magic-0.3.1/README.md` & `contact_magic-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/asyncio.py` & `contact_magic-0.3.2/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/conf/settings.py` & `contact_magic-0.3.2/contact_magic/conf/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,19 @@
         default={},
     )
     COPYFACTORY_MAPPING: dict = Field(
         description="Mapping where the keys are field names "
         "in your data and the values are what you want to swap it with.",
         default={},
     )
+    SCRAPER_OPTIONS: dict = Field(
+        description="Mapping where the keys are the scraper names "
+        "and the values are a dict of additional scraper options to pass.",
+        default={},
+    )
 
     @validator("TIMEZONE")
     def validate_timezone(cls, value):
         timezones = pytz.all_timezones_set
         if value not in timezones:
             value = "America/New_York"
         return value
```

### Comparing `contact_magic-0.3.1/contact_magic/helpers.py` & `contact_magic-0.3.2/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/integrations/copyfactory.py` & `contact_magic-0.3.2/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.3.2/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/integrations/sheets.py` & `contact_magic-0.3.2/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/models.py` & `contact_magic-0.3.2/contact_magic/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,22 @@
             return row, row.data[content_col_name] is not None
         row = await self.run_sales_scraper(row, col_prefix=content_col_name)
         row, success = await self.run_copyfactory(
             row, content_col_name, source_col_name
         )
         return row, success
 
+    def __init__(self, **data: Any):
+        if data.get("scraper_name", None):
+            if default_options := SETTINGS.SCRAPER_OPTIONS.get(
+                data.get("scraper_name"), None
+            ):
+                data = data | default_options
+        super().__init__(**data)
+
 
 class DataPoint(BaseModel):
     """
     A reference to a datapoint to create for a given contact
     targeting a column and a list of allowed scrapers.
     """
```

### Comparing `contact_magic-0.3.1/contact_magic/preprocessors.py` & `contact_magic-0.3.2/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/scripts/agency.py` & `contact_magic-0.3.2/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/scripts/run_workflows.py` & `contact_magic-0.3.2/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.3.2/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/contact_magic/utils.py` & `contact_magic-0.3.2/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.1/pyproject.toml` & `contact_magic-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.3.1"
+version = "0.3.2"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.3.1/PKG-INFO` & `contact_magic-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.3.1
+Version: 0.3.2
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

