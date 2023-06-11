# Comparing `tmp/contact_magic-0.3.4.tar.gz` & `tmp/contact_magic-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.3.4.tar", max compression
+gzip compressed data, was "contact_magic-0.3.5.tar", max compression
```

## Comparing `contact_magic-0.3.4.tar` & `contact_magic-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.4/README.md
--rw-r--r--   0        0        0      273 2023-06-11 11:14:26.606174 contact_magic-0.3.4/contact_magic/__init__.py
--rw-r--r--   0        0        0      977 2023-06-11 21:09:57.091034 contact_magic-0.3.4/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.4/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5201 2023-06-11 11:20:08.656242 contact_magic-0.3.4/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-11 11:09:58.728061 contact_magic-0.3.4/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.4/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2177 2023-06-11 12:02:22.673968 contact_magic-0.3.4/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.3.4/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.4/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.4/contact_magic/logger.py
--rw-r--r--   0        0        0    12228 2023-06-11 21:09:23.092781 contact_magic-0.3.4/contact_magic/models.py
--rw-r--r--   0        0        0     3047 2023-06-11 21:07:35.643112 contact_magic-0.3.4/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.4/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.4/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.4/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.4/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.4/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.4/contact_magic/utils.py
--rw-r--r--   0        0        0     1710 2023-06-11 21:09:30.620570 contact_magic-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.5/README.md
+-rw-r--r--   0        0        0      273 2023-06-11 11:14:26.606174 contact_magic-0.3.5/contact_magic/__init__.py
+-rw-r--r--   0        0        0      977 2023-06-11 21:25:16.933482 contact_magic-0.3.5/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.5/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5201 2023-06-11 11:20:08.656242 contact_magic-0.3.5/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-11 11:09:58.728061 contact_magic-0.3.5/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.5/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2177 2023-06-11 12:02:22.673968 contact_magic-0.3.5/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.3.5/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.5/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.5/contact_magic/logger.py
+-rw-r--r--   0        0        0    12240 2023-06-11 21:23:32.498600 contact_magic-0.3.5/contact_magic/models.py
+-rw-r--r--   0        0        0     3047 2023-06-11 21:07:35.643112 contact_magic-0.3.5/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.5/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.5/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.5/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.5/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.5/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.5/contact_magic/utils.py
+-rw-r--r--   0        0        0     1710 2023-06-11 21:25:05.397402 contact_magic-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.5/PKG-INFO
```

### Comparing `contact_magic-0.3.4/README.md` & `contact_magic-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/asyncio.py` & `contact_magic-0.3.5/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/conf/settings.py` & `contact_magic-0.3.5/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/helpers.py` & `contact_magic-0.3.5/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/integrations/copyfactory.py` & `contact_magic-0.3.5/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.3.5/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/integrations/sheets.py` & `contact_magic-0.3.5/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/models.py` & `contact_magic-0.3.5/contact_magic/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
         if not self.field_processors:
             return row, True
 
         from contact_magic.preprocessors import processors
 
         for key, processor in self.field_processors.items():
-            if item := find_item(row.data, key):
+            if item := find_item(row.data, key) is not None:
                 if validation_model := processors.get(
                     processor.get("type", None), None
                 ):
                     value, is_value_valid = validation_model(
                         processor=processor, value=item, scraper=self
                     ).process()
                     if is_value_valid is False:
```

### Comparing `contact_magic-0.3.4/contact_magic/preprocessors.py` & `contact_magic-0.3.5/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/scripts/agency.py` & `contact_magic-0.3.5/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/scripts/run_workflows.py` & `contact_magic-0.3.5/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.3.5/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/contact_magic/utils.py` & `contact_magic-0.3.5/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.4/pyproject.toml` & `contact_magic-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.3.4"
+version = "0.3.5"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.3.4/PKG-INFO` & `contact_magic-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.3.4
+Version: 0.3.5
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

