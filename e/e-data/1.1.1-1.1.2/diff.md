# Comparing `tmp/e-data-1.1.1.tar.gz` & `tmp/e-data-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-data-1.1.1.tar", last modified: Sun Jun 11 10:08:53 2023, max compression
+gzip compressed data, was "e-data-1.1.2.tar", last modified: Sun Jun 11 10:11:30 2023, max compression
```

## Comparing `e-data-1.1.1.tar` & `e-data-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:08:53.118277 e-data-1.1.1/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)      193 2023-06-11 10:01:58.000000 e-data-1.1.1/MANIFEST.in
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6568 2023-06-11 10:08:53.118277 e-data-1.1.1/PKG-INFO
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     4860 2023-06-11 10:01:58.000000 e-data-1.1.1/README.md
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:08:53.110277 e-data-1.1.1/e_data.egg-info/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6568 2023-06-11 10:08:52.000000 e-data-1.1.1/e_data.egg-info/PKG-INFO
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)      499 2023-06-11 10:08:53.000000 e-data-1.1.1/e_data.egg-info/SOURCES.txt
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        1 2023-06-11 10:08:52.000000 e-data-1.1.1/e_data.egg-info/dependency_links.txt
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)      119 2023-06-11 10:08:52.000000 e-data-1.1.1/e_data.egg-info/requires.txt
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        6 2023-06-11 10:08:52.000000 e-data-1.1.1/e_data.egg-info/top_level.txt
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:08:53.110277 e-data-1.1.1/edata/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/__init__.py
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:08:53.114277 e-data-1.1.1/edata/connectors/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/connectors/__init__.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)    15200 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/connectors/datadis.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     1990 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/connectors/redata.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     3828 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/definitions.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)    22473 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/helpers.py
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:08:53.118277 e-data-1.1.1/edata/processors/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/processors/__init__.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)      624 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/processors/base.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6224 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/processors/billing.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     2330 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/processors/consumption.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     1334 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/processors/maximeter.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     5155 2023-06-11 10:01:58.000000 e-data-1.1.1/edata/processors/utils.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)       54 2023-06-11 10:08:53.122277 e-data-1.1.1/setup.cfg
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     4260 2023-06-11 10:07:20.000000 e-data-1.1.1/setup.py
+drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.496630 e-data-1.1.2/
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)      193 2023-06-11 10:01:58.000000 e-data-1.1.2/MANIFEST.in
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6568 2023-06-11 10:11:30.496630 e-data-1.1.2/PKG-INFO
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     4860 2023-06-11 10:01:58.000000 e-data-1.1.2/README.md
+drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.484630 e-data-1.1.2/e_data.egg-info/
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6568 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/PKG-INFO
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)      499 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)        1 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)      119 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/requires.txt
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)        6 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/top_level.txt
+drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.488630 e-data-1.1.2/edata/
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/__init__.py
+drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.488630 e-data-1.1.2/edata/connectors/
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/connectors/__init__.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)    15204 2023-06-11 10:10:24.000000 e-data-1.1.2/edata/connectors/datadis.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     1990 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/connectors/redata.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     3828 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/definitions.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)    22473 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/helpers.py
+drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.492630 e-data-1.1.2/edata/processors/
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/__init__.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)      624 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/base.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6224 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/billing.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     2330 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/consumption.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     1334 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/maximeter.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     5155 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/utils.py
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)       54 2023-06-11 10:11:30.496630 e-data-1.1.2/setup.cfg
+-rw-r--r--   0 vmayor    (1000) vmayor    (1000)     4260 2023-06-11 10:10:34.000000 e-data-1.1.2/setup.py
```

### Comparing `e-data-1.1.1/PKG-INFO` & `e-data-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-data
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python library for managing spanish energy data from various web providers
 Home-page: https://github.com/uvejota/python-edata
 Author: VMG
 Author-email: vmayorg@outlook.es
 License: GPLv3
 Description: 
         [![Downloads](https://pepy.tech/badge/e-data)](https://pepy.tech/project/e-data)
```

### Comparing `e-data-1.1.1/README.md` & `e-data-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/e_data.egg-info/PKG-INFO` & `e-data-1.1.2/e_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-data
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python library for managing spanish energy data from various web providers
 Home-page: https://github.com/uvejota/python-edata
 Author: VMG
 Author-email: vmayorg@outlook.es
 License: GPLv3
 Description: 
         [![Downloads](https://pepy.tech/badge/e-data)](https://pepy.tech/project/e-data)
```

### Comparing `e-data-1.1.1/edata/connectors/datadis.py` & `e-data-1.1.2/edata/connectors/datadis.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "date",
     "consumptionKWh",
     "obtainMethod",
 ]
 URL_GET_MAX_POWER = "https://datadis.es/api-private/api/get-max-power"
 GET_MAX_POWER_MANDATORY_FIELDS = ["time", "date", "maxPower"]
 
-TIMEOUT = 60
+TIMEOUT = 3 * 60
 
 MAX_CONSUMPTIONS_MONTHS = 1
 
 QUERY_LIMIT = timedelta(hours=24)
 
 RECENT_QUERIES_FILE = "/tmp/edata_recent_queries.json"
```

### Comparing `e-data-1.1.1/edata/connectors/redata.py` & `e-data-1.1.2/edata/connectors/redata.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/edata/definitions.py` & `e-data-1.1.2/edata/definitions.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/edata/helpers.py` & `e-data-1.1.2/edata/helpers.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/edata/processors/base.py` & `e-data-1.1.2/edata/processors/base.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/edata/processors/billing.py` & `e-data-1.1.2/edata/processors/billing.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/edata/processors/consumption.py` & `e-data-1.1.2/edata/processors/consumption.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/edata/processors/maximeter.py` & `e-data-1.1.2/edata/processors/maximeter.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/edata/processors/utils.py` & `e-data-1.1.2/edata/processors/utils.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.1/setup.py` & `e-data-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = (
     "Python library for managing spanish energy data from various web providers"
 )
 URL = "https://github.com/uvejota/python-edata"
 EMAIL = "vmayorg@outlook.es"
 AUTHOR = "VMG"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "dateparser>=1.1.2",
     "freezegun>=1.2.1",
     "holidays>=0.14.2",
     "pandas<2.0.0",
```

