# Comparing `tmp/mleko-0.4.1.tar.gz` & `tmp/mleko-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.4.1.tar", max compression
+gzip compressed data, was "mleko-0.4.2.tar", max compression
```

## Comparing `mleko-0.4.1.tar` & `mleko-0.4.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1073 2023-06-04 20:58:16.253797 mleko-0.4.1/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-04 20:58:16.253797 mleko-0.4.1/README.md
--rw-r--r--   0        0        0     1323 2023-06-04 20:58:49.939543 mleko-0.4.1/mleko/__init__.py
--rw-r--r--   0        0        0      584 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/__init__.py
--rw-r--r--   0        0        0    11493 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0      805 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     2843 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1233 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0      398 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/format/__init__.py
--rw-r--r--   0        0        0     1933 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/format/vaex_cache_format_mixin.py
--rw-r--r--   0        0        0     5974 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      740 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      491 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1435 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    11536 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     1613 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0     5918 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     5267 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     4983 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5248 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7078 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5501 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      877 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     2211 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    18015 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0     9632 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      679 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     3815 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     5934 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0      644 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1420 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4496 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3595 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      638 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2359 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     2179 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2141 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     2248 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0        0 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/py.typed
--rw-r--r--   0        0        0      765 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3430 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1403 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     2836 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2752 2023-06-04 20:58:49.999546 mleko-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 mleko-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-11 08:22:08.292228 mleko-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-11 08:22:08.292228 mleko-0.4.2/README.md
+-rw-r--r--   0        0        0     1323 2023-06-11 08:22:37.196064 mleko-0.4.2/mleko/__init__.py
+-rw-r--r--   0        0        0      584 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    11493 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0      805 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     2843 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1233 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0      398 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/format/__init__.py
+-rw-r--r--   0        0        0     1933 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/format/vaex_cache_format_mixin.py
+-rw-r--r--   0        0        0     5974 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      740 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1435 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    11572 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     1613 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0     5918 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     5267 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     4983 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5248 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7078 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5578 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      877 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2211 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    18015 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0     9632 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      679 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     3815 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     5934 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0      644 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1420 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4496 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3595 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      638 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2359 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     2179 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2141 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     2248 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0        0 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/py.typed
+-rw-r--r--   0        0        0      765 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3430 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1403 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     2836 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2839 2023-06-11 08:22:37.244064 mleko-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 mleko-0.4.2/PKG-INFO
```

### Comparing `mleko-0.4.1/LICENSE` & `mleko-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/README.md` & `mleko-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/__init__.py` & `mleko-0.4.2/mleko/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
 from __future__ import annotations
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `mleko-0.4.1/mleko/cache/__init__.py` & `mleko-0.4.2/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/cache/cache_mixin.py` & `mleko-0.4.2/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/cache/fingerprinters/__init__.py` & `mleko-0.4.2/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-0.4.2/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-0.4.2/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-0.4.2/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/cache/format/vaex_cache_format_mixin.py` & `mleko-0.4.2/mleko/cache/format/vaex_cache_format_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/cache/lru_cache_mixin.py` & `mleko-0.4.2/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/__init__.py` & `mleko-0.4.2/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/convert/base_converter.py` & `mleko-0.4.2/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-0.4.2/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
                     "%Y-%m-%dT%H:%M:%S",
                     "%Y-%m-%dT%H:%M:%S.%f",
                 ],
             ),
         ).drop(drop_columns)
 
         output_path = output_directory / f"df_chunk_{file_path.stem}.{dataframe_suffix}"
-        df_chunk.export(output_path)
+        df_chunk.export(output_path, chunk_size=100_000, parallel=False)
         df_chunk.close()
 
     def _convert(self, file_paths: list[Path] | list[str]) -> vaex.DataFrame:
         """Converts a list of CSV files to Arrow format using parallel processing.
 
         Chunks of files are processed in parallel and saved in the output directory.
```

### Comparing `mleko-0.4.1/mleko/dataset/feature_select/__init__.py` & `mleko-0.4.2/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-0.4.2/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-0.4.2/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-0.4.2/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-0.4.2/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-0.4.2/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-0.4.2/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,19 +99,23 @@
 
         Returns:
             The DataFrame with the selected features.
         """
         features = self._feature_set(dataframe)
         logger.info(f"Selecting features from the following set ({len(features)}): {features}.")
 
-        scaler = MaxAbsScaler(features=list(features), prefix="")
-        df_scaled = scaler.fit_transform(dataframe)
+        if self._variance_threshold > 0:
+            scaler = MaxAbsScaler(features=list(features), prefix="")
+            df = scaler.fit_transform(dataframe)
+        else:
+            df = dataframe
+
         variance: dict[str, float] = {}
         for feature in tqdm(features, desc="Calculating variance for features"):
-            column = get_column(df_scaled, feature)
+            column = get_column(df, feature)
             variance[feature] = column.var()
 
         dropped_features = {feature for feature in features if variance[feature] <= self._variance_threshold}
         logger.info(
             f"Dropping ({len(dropped_features)}) features with normalized variance <= {self._variance_threshold}: "
             f"{dropped_features}."
         )
```

### Comparing `mleko-0.4.1/mleko/dataset/ingest/__init__.py` & `mleko-0.4.2/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/ingest/base_ingester.py` & `mleko-0.4.2/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-0.4.2/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/ingest/s3_ingester.py` & `mleko-0.4.2/mleko/dataset/ingest/s3_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/split/__init__.py` & `mleko-0.4.2/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/split/base_splitter.py` & `mleko-0.4.2/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/split/expression_splitter.py` & `mleko-0.4.2/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/dataset/split/random_splitter.py` & `mleko-0.4.2/mleko/dataset/split/random_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/__init__.py` & `mleko-0.4.2/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/data_container.py` & `mleko-0.4.2/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/pipeline.py` & `mleko-0.4.2/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/pipeline_step.py` & `mleko-0.4.2/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/steps/__init__.py` & `mleko-0.4.2/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/steps/convert_step.py` & `mleko-0.4.2/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/steps/feature_select_step.py` & `mleko-0.4.2/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/steps/ingest_step.py` & `mleko-0.4.2/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/pipeline/steps/split_step.py` & `mleko-0.4.2/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/utils/__init__.py` & `mleko-0.4.2/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/utils/custom_logger.py` & `mleko-0.4.2/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/utils/decorators.py` & `mleko-0.4.2/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/utils/file_helpers.py` & `mleko-0.4.2/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/utils/tqdm_helpers.py` & `mleko-0.4.2/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/mleko/utils/vaex_helpers.py` & `mleko-0.4.2/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.1/pyproject.toml` & `mleko-0.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.4.1"
+version = "0.4.2"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
@@ -18,15 +18,14 @@
 [tool.poetry.dependencies]
 python = "3.10.* || 3.9.* || 3.8.*"
 boto3 = "^1.26.91"
 botocore = "^1.29.91"
 tqdm = "^4.65.0"
 vaex = "^4.16.0"
 scikit-learn = "^1.2.2"
-pandas = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 boto3-stubs = {extras = ["s3"], version = "^1.26.91"}
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
@@ -113,7 +112,8 @@
 version_source = "tag"
 commit_version_number = true
 tag_commit = true
 upload_to_pypi = false
 upload_to_release = false
 hvcs = "github"
 commit_message = "chore(release): release {version}"
+changelog_sections = "feature,fix,breaking,performance,documentation,refactor,style,test,build,ci,chore"
```

### Comparing `mleko-0.4.1/PKG-INFO` & `mleko-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.4.1
+Version: 0.4.2
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: boto3 (>=1.26.91,<2.0.0)
 Requires-Dist: botocore (>=1.29.91,<2.0.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: vaex (>=4.16.0,<5.0.0)
 Project-URL: Changelog, https://github.com/ErikBavenstrand/mleko/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://mleko.readthedocs.io
 Project-URL: Repository, https://github.com/ErikBavenstrand/mleko
 Description-Content-Type: text/markdown
```

