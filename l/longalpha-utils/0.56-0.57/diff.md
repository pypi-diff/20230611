# Comparing `tmp/longalpha_utils-0.56.tar.gz` & `tmp/longalpha_utils-0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.56.tar", last modified: Sun Jun 11 02:16:02 2023, max compression
+gzip compressed data, was "longalpha_utils-0.57.tar", last modified: Sun Jun 11 03:30:37 2023, max compression
```

## Comparing `longalpha_utils-0.56.tar` & `longalpha_utils-0.57.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:16:02.300947 longalpha_utils-0.56/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 02:16:02.300947 longalpha_utils-0.56/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:16:02.300947 longalpha_utils-0.56/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:16:02.300947 longalpha_utils-0.56/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 02:16:02.300947 longalpha_utils-0.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 02:15:46.000000 longalpha_utils-0.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:30:37.522178 longalpha_utils-0.57/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:30:37.522178 longalpha_utils-0.57/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:30:37.518178 longalpha_utils-0.57/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:30:37.522178 longalpha_utils-0.57/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:30:37.522178 longalpha_utils-0.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 03:30:27.000000 longalpha_utils-0.57/setup.py
```

### Comparing `longalpha_utils-0.56/longalpha_utils/messenger.py` & `longalpha_utils-0.57/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.56/longalpha_utils/transfers.py` & `longalpha_utils-0.57/longalpha_utils/transfers.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,16 @@
             if show_missing_date:
                 print(f"Options data for {day} does not exist.")
             else:
                 pass
 
     def get_spark_data(self, spark: SparkSession) -> Union[DataFrame, None]:
         """
-        Get data from s3 for a given date range from self.start_date to self.end_date
+        Get data from s3 for a given date range from self.start_date to self.end_date. Note this only gets data
+        from spark saved location (snappy file)
         Args:
             spark: spark session
 
         Returns: a spark dataframe if data exists, None otherwise
 
         """
 
@@ -447,15 +448,16 @@
             df = self.get_spark_data_one_day(
                 spark=spark,
                 s3_bucket=self.s3_bucket,
                 s3_prefix=self.s3_prefix,
                 day=day,
                 show_missing_date=self.show_missing_date,
             )
-            dfs.append(df)
+            if df is not None:
+                dfs.append(df)
         if len(dfs) == 0:
             return None
         return multi_union_by_name(dfs)
 
     def get_pandas_data(self, mw: MinioWrapper) -> Union[pd.DataFrame, None]:
         """
         Get padnas data in pickle files from s3 for a given date range
@@ -471,13 +473,14 @@
             df = self.get_pandas_data_one_day(
                 mw=mw,
                 s3_bucket=self.s3_bucket,
                 s3_prefix=self.s3_prefix,
                 day=day,
                 show_missing_date=self.show_missing_date,
             )
-            dfs.append(df)
+            if df is not None:
+                dfs.append(df)
 
         if len(dfs) == 0:
             return None
         return pd.concat(dfs, axis=0, join="outer", ignore_index=True)
```

### Comparing `longalpha_utils-0.56/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.57/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.56/longalpha_utils/utils.py` & `longalpha_utils-0.57/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.56/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.57/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.56/setup.py` & `longalpha_utils-0.57/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.56",
+    version="0.57",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

