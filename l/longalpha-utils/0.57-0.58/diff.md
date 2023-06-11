# Comparing `tmp/longalpha_utils-0.57.tar.gz` & `tmp/longalpha_utils-0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.57.tar", last modified: Sun Jun 11 03:30:37 2023, max compression
+gzip compressed data, was "longalpha_utils-0.58.tar", last modified: Sun Jun 11 03:59:54 2023, max compression
```

## Comparing `longalpha_utils-0.57.tar` & `longalpha_utils-0.58.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:30:37.522178 longalpha_utils-0.57/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:30:37.522178 longalpha_utils-0.57/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:30:37.518178 longalpha_utils-0.57/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-11 03:30:27.000000 longalpha_utils-0.57/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:30:37.522178 longalpha_utils-0.57/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 03:30:37.000000 longalpha_utils-0.57/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:30:37.522178 longalpha_utils-0.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 03:30:27.000000 longalpha_utils-0.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:54.310248 longalpha_utils-0.58/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:59:54.310248 longalpha_utils-0.58/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:54.310248 longalpha_utils-0.58/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-11 03:59:44.000000 longalpha_utils-0.58/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:54.310248 longalpha_utils-0.58/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 03:59:54.000000 longalpha_utils-0.58/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:59:54.310248 longalpha_utils-0.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 03:59:44.000000 longalpha_utils-0.58/setup.py
```

### Comparing `longalpha_utils-0.57/longalpha_utils/messenger.py` & `longalpha_utils-0.58/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.57/longalpha_utils/transfers.py` & `longalpha_utils-0.58/longalpha_utils/transfers.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,28 +411,28 @@
         Returns: pyspark dataframe for the day or None if the data does not exist
 
         """
         try:
             return spark.read.parquet(get_s3_path(s3_bucket, s3_prefix, day))
         except AnalysisException:
             if show_missing_date:
-                print(f"Options data for {day} does not exist.")
+                print(f"Data for {day} does not exist.")
             else:
                 pass
 
     @staticmethod
     def get_pandas_data_one_day(
         mw: MinioWrapper, s3_bucket, s3_prefix, day: date, show_missing_date: bool = True
     ) -> Union[DataFrame, None]:
         try:
             object_name = os.path.join(s3_prefix, f"{day}.pkl")
             return mw.get(bucket_name=s3_bucket, object_name=object_name, from_pickle=True)
         except minio.error.S3Error:
             if show_missing_date:
-                print(f"Options data for {day} does not exist.")
+                print(f"Data for {day} does not exist.")
             else:
                 pass
 
     def get_spark_data(self, spark: SparkSession) -> Union[DataFrame, None]:
         """
         Get data from s3 for a given date range from self.start_date to self.end_date. Note this only gets data
         from spark saved location (snappy file)
```

### Comparing `longalpha_utils-0.57/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.58/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.57/longalpha_utils/utils.py` & `longalpha_utils-0.58/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.57/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.58/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.57/setup.py` & `longalpha_utils-0.58/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.57",
+    version="0.58",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

