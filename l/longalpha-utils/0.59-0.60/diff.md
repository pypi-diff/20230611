# Comparing `tmp/longalpha_utils-0.59.tar.gz` & `tmp/longalpha_utils-0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.59.tar", last modified: Sun Jun 11 05:24:51 2023, max compression
+gzip compressed data, was "longalpha_utils-0.60.tar", last modified: Sun Jun 11 15:49:53 2023, max compression
```

## Comparing `longalpha_utils-0.59.tar` & `longalpha_utils-0.60.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:24:51.078390 longalpha_utils-0.59/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 05:24:51.078390 longalpha_utils-0.59/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:24:51.078390 longalpha_utils-0.59/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-11 05:24:41.000000 longalpha_utils-0.59/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:24:51.078390 longalpha_utils-0.59/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 05:24:51.000000 longalpha_utils-0.59/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 05:24:51.078390 longalpha_utils-0.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 05:24:41.000000 longalpha_utils-0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:49:53.130668 longalpha_utils-0.60/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 15:49:53.130668 longalpha_utils-0.60/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:49:53.126668 longalpha_utils-0.60/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 15:49:43.000000 longalpha_utils-0.60/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 15:49:43.000000 longalpha_utils-0.60/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 15:49:43.000000 longalpha_utils-0.60/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-11 15:49:43.000000 longalpha_utils-0.60/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 15:49:43.000000 longalpha_utils-0.60/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-11 15:49:43.000000 longalpha_utils-0.60/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:49:53.126668 longalpha_utils-0.60/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 15:49:53.000000 longalpha_utils-0.60/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 15:49:53.000000 longalpha_utils-0.60/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:49:53.000000 longalpha_utils-0.60/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 15:49:53.000000 longalpha_utils-0.60/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 15:49:53.000000 longalpha_utils-0.60/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 15:49:53.130668 longalpha_utils-0.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 15:49:43.000000 longalpha_utils-0.60/setup.py
```

### Comparing `longalpha_utils-0.59/longalpha_utils/messenger.py` & `longalpha_utils-0.60/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.59/longalpha_utils/transfers.py` & `longalpha_utils-0.60/longalpha_utils/transfers.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.59/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.60/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.59/longalpha_utils/utils.py` & `longalpha_utils-0.60/longalpha_utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 from typing import List, Optional
-from datetime import date
+from datetime import date, timedelta
 import os
 import pandas as pd
 from pyspark.sql import DataFrame
 
 
 def max_pandas_display(pd: pd, max_row: int = 100) -> None:
     """
@@ -57,7 +57,14 @@
     Returns: s3 path
 
     """
     if day:
         return f"s3a://" + os.path.join(bucket, prefix, day.strftime("%Y"), day.strftime("%m"), day.strftime("%d"))
     else:
         return f"s3a://" + os.path.join(bucket, prefix)
+
+def get_date_range(star_date: date, end_date: date) -> List[date]:
+    dates = []
+    while star_date <= end_date:
+        dates.append(star_date)
+        star_date += timedelta(days=1)
+    return dates
```

### Comparing `longalpha_utils-0.59/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.60/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.59/setup.py` & `longalpha_utils-0.60/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.59",
+    version="0.60",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

