# Comparing `tmp/longalpha_utils-0.55.tar.gz` & `tmp/longalpha_utils-0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.55.tar", last modified: Wed Jun  7 01:54:42 2023, max compression
+gzip compressed data, was "longalpha_utils-0.56.tar", last modified: Sun Jun 11 02:16:02 2023, max compression
```

## Comparing `longalpha_utils-0.55.tar` & `longalpha_utils-0.56.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:54:42.054169 longalpha_utils-0.55/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 01:54:42.054169 longalpha_utils-0.55/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:54:42.054169 longalpha_utils-0.55/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-07 01:54:31.000000 longalpha_utils-0.55/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:54:42.054169 longalpha_utils-0.55/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 01:54:42.000000 longalpha_utils-0.55/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 01:54:42.054169 longalpha_utils-0.55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-07 01:54:31.000000 longalpha_utils-0.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:16:02.300947 longalpha_utils-0.56/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 02:16:02.300947 longalpha_utils-0.56/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:16:02.300947 longalpha_utils-0.56/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-11 02:15:46.000000 longalpha_utils-0.56/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:16:02.300947 longalpha_utils-0.56/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 02:16:02.000000 longalpha_utils-0.56/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 02:16:02.300947 longalpha_utils-0.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 02:15:46.000000 longalpha_utils-0.56/setup.py
```

### Comparing `longalpha_utils-0.55/longalpha_utils/messenger.py` & `longalpha_utils-0.56/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.55/longalpha_utils/transfers.py` & `longalpha_utils-0.56/longalpha_utils/transfers.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from sqlalchemy import create_engine
 from sqlalchemy import text
 from minio.error import S3Error
 from datetime import date, timedelta
 from pyspark.sql.utils import AnalysisException
 from longalpha_utils.utils import multi_union_by_name, get_s3_path
 from tqdm import tqdm
+import minio
 
 
 def init_spark(
     spark_executor_memory: str = "30g",
     spark_driver_memory: str = "90g",
     s3_endpoint: Optional[str] = None,
     s3_access_key: Optional[str] = None,
@@ -56,15 +57,15 @@
         .set("spark.sql.execution.arrow.pyspark.enabled", "true")
         .set(
             "spark.jars.packages", ",".join(jars)
         )  # if you set park.jars.packages more than once, only the last one will be used.
         .set("spark.hadoop.fs.s3a.impl", "org.apache.hadoop.fs.s3a.S3AFileSystem")
         .set("spark.hadoop.fs.s3a.path.style.access", "true")
     )
-    builder =SparkSession.builder.config(conf=spark_conf)
+    builder = SparkSession.builder.config(conf=spark_conf)
     # set other configs
     if additional_configs is not None:
         for k, v in additional_configs.items():
             builder.config(k, v)
     # get spark
     spark = builder.getOrCreate()
 
@@ -117,15 +118,15 @@
             object_name: object name in the minio bucket
 
         Returns:
 
         """
         self.minio_client.fput_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
-    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str, index=False, to_pickle=False) -> None:
+    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str,  to_pickle: bool, index=False,) -> None:
         """
         put a pandas frame to parquet in s3
 
         Args:
             dataframe: a pandas dataframe
             bucket_name: Minio bucket_name
             object_name: object name in the minio bucket
@@ -149,15 +150,15 @@
     def fget(self, file_path: str, bucket_name: str, object_name: str):
         self.minio_client.fget_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
     def get(
         self,
         bucket_name: str,
         object_name: str,
-        from_pickle: bool = False,
+        from_pickle: bool,
     ) -> pd.DataFrame:
         """
         get a parquet from s3 and read it into pandas dataframe
         Args:
             bucket_name: Minio bucket_name
             object_name: path + file_name
             from_pickle: whether to read the file from pickle
@@ -201,172 +202,282 @@
         latest_time = max([key for key in time_obj.keys() if key is not None])
         latest_obj = time_obj[latest_time]
         return self.get(bucket_name=bucket_name, object_name=latest_obj.object_name)
 
     def list(self, bucket_name: str) -> List[str]:
         return [i.object_name for i in self.minio_client.list_objects(bucket_name, recursive=True)]
 
-    def delete_objects(self, bucket_name:str, prefix:str) -> None:
+    def delete_objects(self, bucket_name: str, prefix: str) -> None:
         """
         delete all objects in a bucket with a given prefix
         Args:
             bucket_name: Minio bucket_name
             prefix: prefix of the objects to be deleted
 
         Returns:
 
         """
-        objects = self.minio_client.list_objects(
-            bucket_name, prefix,
-            recursive=True
-        )
+        objects = self.minio_client.list_objects(bucket_name, prefix, recursive=True)
 
         for obj in objects:
             self.minio_client.remove_object(bucket_name, obj.object_name)
 
+#
+# def get_s3_data_spark(
+#     spark: SparkSession,
+#     start_date: date,
+#     end_date: date,
+#     bucket: str,
+#     prefix: str,
+#     show_missing_dates: bool = False,
+#     progress_bar: bool = True,
+# ) -> Union[DataFrame, None]:
+#     """
+#     Get data from s3 for a given date range
+#     Args:
+#         spark: spark session
+#         start_date: start date to get options data for
+#         end_date: end date to get options data for
+#         bucket: s3 bucket name
+#         prefix: prefix in the s3 bucket
+#         show_missing_dates: whether to print out missing dates
+#         progress_bar: whether to show a progress bar
+#
+#     Returns: a spark dataframe if data exists, None otherwise
+#
+#     """
+#     dates = []
+#     while start_date <= end_date:
+#         dates.append(start_date)
+#         start_date += timedelta(days=1)
+#     if progress_bar:
+#         dates = tqdm(dates)
+#
+#     options = []
+#     for day in dates:
+#         file_s3_path = get_s3_path(bucket, prefix, day)
+#         try:
+#             option = spark.read.parquet(file_s3_path)
+#             options.append(option)
+#         except AnalysisException:
+#             if show_missing_dates:
+#                 print(f"Options data for {start_date} does not exist.")
+#             else:
+#                 pass
+#     if len(options) == 0:
+#         return None
+#     return multi_union_by_name(options)
+#
+
+#
+# def spark_read_psql(
+#     spark: SparkSession, psql_url: str, psql_db: str, psql_table: str, psql_usr: str, psql_pwd: str
+# ) -> DataFrame:
+#     """
+#     use spark to read psql
+#     Args:
+#         spark: spark instance. Must be created with support for psql.
+#         psql_url: url of psql
+#         psql_db: database name
+#         psql_table: table name
+#         psql_usr: username of psql
+#         psql_pwd: password of psql
+#
+#     Returns: a pyspark dataframe
+#
+#     """
+#     return (
+#         spark.read.format("jdbc")
+#         .option("url", f"jdbc:postgresql://{psql_url}/{psql_db}")
+#         .option("dbtable", psql_table)
+#         .option("user", psql_usr)
+#         .option("password", psql_pwd)
+#         .option("driver", "org.postgresql.Driver")
+#         .load()
+#     )
+#
+#
+# def df_to_psql(
+#     df: pd.DataFrame,
+#     table_name: str,
+#     index=False,
+#     dtype: Optional[Dict[str, Any]] = None,
+#     if_exists: str = "append",
+#     engine: Optional[Engine] = None,
+#     user_name: Optional[str] = None,
+#     password: Optional[str] = None,
+#     host_with_port: Optional[str] = None,
+#     db_name: Optional[str] = None,
+#     **kwargs: Any,
+# ) -> None:
+#     """
+#     write a pandas dataframe to psql
+#     Args:
+#         df: pandas dataframe
+#         table_name: table name to write to psql
+#         index: whether to write index to psql
+#         dtype: data type of column. If a dictionary is used, the keys should be the column names and the values
+#         should be the SQLAlchemy types or strings for the sqlite3 legacy mode
+#         if_exists: {‘fail’, ‘replace’, ‘append’}, default ‘append’. How to behave if the table already exists.
+#         engine: sqlalchemy engine. If not None, then we will use this engine to write to psql.
+#         user_name: username of psql
+#         password: password of psql
+#         host_with_port: host_with_port of psql
+#         db_name: database name of psql to write to
+#         kwargs: additional keyword argument passed to DataFrame.to_sql
+#
+#     Returns: None
+#
+#     """
+#     if engine is not None and user_name is not None:
+#         raise ValueError("engine and user_name cannot be both not None")
+#     if engine is None and user_name is None:
+#         raise ValueError("engine and user_name cannot be both None")
+#     if engine is None:
+#         engine = create_engine(f"postgresql://{user_name}:{password}@{host_with_port}/{db_name}")
+#     df.to_sql(table_name, con=engine, index=index, if_exists=if_exists, dtype=dtype, **kwargs)
+#
+#
+# def df_from_psql(
+#     sql: str,
+#     engine: Optional[Engine] = None,
+#     user_name: Optional[str] = None,
+#     password: Optional[str] = None,
+#     host_with_port: Optional[str] = None,
+#     db_name: Optional[str] = None,
+#     **kwargs: Any,
+# ) -> pd.DataFrame:
+#     """
+#     read a pandas dataframe from psql
+#     Args:
+#         sql: sql query
+#         engine: sqlalchemy engine. If not None, then we will use this engine to write to psql.
+#         user_name:  username of psql
+#         password: password of psql
+#         host_with_port: host_with_port of psql
+#         db_name: database name of psql to write to
+#         **kwargs: additional keyword argument passed to pd.read_sql
+#
+#     Returns:
+#
+#     """
+#     if engine is not None and user_name is not None:
+#         raise ValueError("engine and user_name cannot be both not None")
+#     if engine is None and user_name is None:
+#         raise ValueError("engine and user_name cannot be both None")
+#     if engine is None:
+#         engine = create_engine(f"postgresql://{user_name}:{password}@{host_with_port}/{db_name}")
+#     query = text(sql)
+#     return pd.read_sql(sql=query, con=engine.connect(), **kwargs)
 
 
-def get_s3_data_spark(
-    spark: SparkSession,
-    start_date: date,
-    end_date: date,
-    bucket: str,
-    prefix: str,
-    show_missing_dates: bool = False,
-    progress_bar: bool = True,
-) -> Union[DataFrame, None]:
-    """
-    Get data from s3 for a given date range
-    Args:
-        spark: spark session
-        start_date: start date to get options data for
-        end_date: end date to get options data for
-        bucket: s3 bucket name
-        prefix: prefix in the s3 bucket
-        show_missing_dates: whether to print out missing dates
-        progress_bar: whether to show a progress bar
+class S3DataReader:
+    def __init__(self, start_date, end_date, s3_bucket: str, s3_prefix: str, show_missing_date: bool =True) -> None:
+        """
+        read pyspark data (in folder of snappy file) and pandas data (in pickle file) from s3
+        Args:
+            start_date: start date to get options data for
+            end_date: end date to get options data for
+            s3_bucket: s3 bucket name
+            s3_prefix: prefix in the s3 bucket
+            show_missing_date: whether to print out missing dates
+        """
+        self.s3_bucket = s3_bucket
+        self.s3_prefix = s3_prefix
+        self.start_date = start_date
+        self.end_date = end_date
+        self.show_missing_date = show_missing_date
+
+    @staticmethod
+    def _get_data_rage(start_date: date, end_date: date) -> List[date]:
+        dates = []
+        while start_date <= end_date:
+            dates.append(start_date)
+            start_date += timedelta(days=1)
+        return dates
+
+    @staticmethod
+    def get_spark_data_one_day(
+        spark: SparkSession, s3_bucket: str, s3_prefix: str, day: date, show_missing_date: bool = True
+    ) -> Union[DataFrame, None]:
+        """
+        get pyspark data for one day
+        Args:
+            spark:  spark session
+            s3_bucket:  s3 bucket name
+            s3_prefix:  s3 prefix, excluding data path such as /year/month/day
+            day:  date to get data for
+            show_missing_date:  whether to print out missing dates
 
-    Returns: a spark dataframe if data exists, None otherwise
+        Returns: pyspark dataframe for the day or None if the data does not exist
 
-    """
-    dates = []
-    while start_date <= end_date:
-        dates.append(start_date)
-        start_date += timedelta(days=1)
-    if progress_bar:
-        dates = tqdm(dates)
-
-    options = []
-    for day in dates:
-        file_s3_path = get_s3_path(bucket, prefix, day)
+        """
         try:
-            option = spark.read.parquet(file_s3_path)
-            options.append(option)
+            return spark.read.parquet(get_s3_path(s3_bucket, s3_prefix, day))
         except AnalysisException:
-            if show_missing_dates:
-                print(f"Options data for {start_date} does not exist.")
+            if show_missing_date:
+                print(f"Options data for {day} does not exist.")
             else:
                 pass
-    if len(options) == 0:
-        return None
-    return multi_union_by_name(options)
 
+    @staticmethod
+    def get_pandas_data_one_day(
+        mw: MinioWrapper, s3_bucket, s3_prefix, day: date, show_missing_date: bool = True
+    ) -> Union[DataFrame, None]:
+        try:
+            object_name = os.path.join(s3_prefix, f"{day}.pkl")
+            return mw.get(bucket_name=s3_bucket, object_name=object_name, from_pickle=True)
+        except minio.error.S3Error:
+            if show_missing_date:
+                print(f"Options data for {day} does not exist.")
+            else:
+                pass
 
-def spark_read_psql(
-    spark: SparkSession, psql_url: str, psql_db: str, psql_table: str, psql_usr: str, psql_pwd: str
-) -> DataFrame:
-    """
-    use spark to read psql
-    Args:
-        spark: spark instance. Must be created with support for psql.
-        psql_url: url of psql
-        psql_db: database name
-        psql_table: table name
-        psql_usr: username of psql
-        psql_pwd: password of psql
+    def get_spark_data(self, spark: SparkSession) -> Union[DataFrame, None]:
+        """
+        Get data from s3 for a given date range from self.start_date to self.end_date
+        Args:
+            spark: spark session
 
-    Returns: a pyspark dataframe
+        Returns: a spark dataframe if data exists, None otherwise
 
-    """
-    return (
-        spark.read.format("jdbc")
-        .option("url", f"jdbc:postgresql://{psql_url}/{psql_db}")
-        .option("dbtable", psql_table)
-        .option("user", psql_usr)
-        .option("password", psql_pwd)
-        .option("driver", "org.postgresql.Driver")
-        .load()
-    )
+        """
 
+        dfs = []
+        for day in tqdm(self._get_data_rage(self.start_date, self.end_date)):
+            df = self.get_spark_data_one_day(
+                spark=spark,
+                s3_bucket=self.s3_bucket,
+                s3_prefix=self.s3_prefix,
+                day=day,
+                show_missing_date=self.show_missing_date,
+            )
+            dfs.append(df)
+        if len(dfs) == 0:
+            return None
+        return multi_union_by_name(dfs)
 
-def df_to_psql(
-    df: pd.DataFrame,
-    table_name: str,
-    index=False,
-    dtype: Optional[Dict[str, Any]] = None,
-    if_exists: str = "append",
-    engine: Optional[Engine] = None,
-    user_name: Optional[str] = None,
-    password: Optional[str] = None,
-    host_with_port: Optional[str] = None,
-    db_name: Optional[str] = None,
-    **kwargs: Any,
-) -> None:
-    """
-    write a pandas dataframe to psql
-    Args:
-        df: pandas dataframe
-        table_name: table name to write to psql
-        index: whether to write index to psql
-        dtype: data type of column. If a dictionary is used, the keys should be the column names and the values
-        should be the SQLAlchemy types or strings for the sqlite3 legacy mode
-        if_exists: {‘fail’, ‘replace’, ‘append’}, default ‘append’. How to behave if the table already exists.
-        engine: sqlalchemy engine. If not None, then we will use this engine to write to psql.
-        user_name: username of psql
-        password: password of psql
-        host_with_port: host_with_port of psql
-        db_name: database name of psql to write to
-        kwargs: additional keyword argument passed to DataFrame.to_sql
+    def get_pandas_data(self, mw: MinioWrapper) -> Union[pd.DataFrame, None]:
+        """
+        Get padnas data in pickle files from s3 for a given date range
+        Args:
+            mw: minio wrapper
 
-    Returns: None
+        Returns: a pandas dataframe if data exists, None otherwise
 
-    """
-    if engine is not None and user_name is not None:
-        raise ValueError("engine and user_name cannot be both not None")
-    if engine is None and user_name is None:
-        raise ValueError("engine and user_name cannot be both None")
-    if engine is None:
-        engine = create_engine(f"postgresql://{user_name}:{password}@{host_with_port}/{db_name}")
-    df.to_sql(table_name, con=engine, index=index, if_exists=if_exists, dtype=dtype, **kwargs)
-
-
-def df_from_psql(
-    sql: str,
-    engine: Optional[Engine] = None,
-    user_name: Optional[str] = None,
-    password: Optional[str] = None,
-    host_with_port: Optional[str] = None,
-    db_name: Optional[str] = None,
-    **kwargs: Any,
-) -> pd.DataFrame:
-    """
-    read a pandas dataframe from psql
-    Args:
-        sql: sql query
-        engine: sqlalchemy engine. If not None, then we will use this engine to write to psql.
-        user_name:  username of psql
-        password: password of psql
-        host_with_port: host_with_port of psql
-        db_name: database name of psql to write to
-        **kwargs: additional keyword argument passed to pd.read_sql
+        """
 
-    Returns:
+        dfs = []
+        for day in tqdm(self._get_data_rage(self.start_date, self.end_date)):
+            df = self.get_pandas_data_one_day(
+                mw=mw,
+                s3_bucket=self.s3_bucket,
+                s3_prefix=self.s3_prefix,
+                day=day,
+                show_missing_date=self.show_missing_date,
+            )
+            dfs.append(df)
+
+        if len(dfs) == 0:
+            return None
+        return pd.concat(dfs, axis=0, join="outer", ignore_index=True)
 
-    """
-    if engine is not None and user_name is not None:
-        raise ValueError("engine and user_name cannot be both not None")
-    if engine is None and user_name is None:
-        raise ValueError("engine and user_name cannot be both None")
-    if engine is None:
-        engine = create_engine(f"postgresql://{user_name}:{password}@{host_with_port}/{db_name}")
-    query = text(sql)
-    return pd.read_sql(sql=query, con=engine.connect(), **kwargs)
```

### Comparing `longalpha_utils-0.55/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.56/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.55/longalpha_utils/utils.py` & `longalpha_utils-0.56/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.55/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.56/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.55/setup.py` & `longalpha_utils-0.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.55",
+    version="0.56",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

