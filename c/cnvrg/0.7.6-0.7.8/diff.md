# Comparing `tmp/cnvrg-0.7.6.tar.gz` & `tmp/cnvrg-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnvrg-0.7.6.tar", last modified: Tue Sep 22 07:38:07 2020, max compression
+gzip compressed data, was "dist/cnvrg-0.7.8.tar", last modified: Fri Oct  2 08:51:46 2020, max compression
```

## Comparing `cnvrg-0.7.6.tar` & `cnvrg-0.7.8.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:07.072523 cnvrg-0.7.6/
--rw-r--r--   0 leah4kosh   (501) staff       (20)      208 2020-09-22 07:38:07.072165 cnvrg-0.7.6/PKG-INFO
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.810795 cnvrg-0.7.6/cnvrg/
--rw-r--r--   0 leah4kosh   (501) staff       (20)      563 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/__init__.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.829468 cnvrg-0.7.6/cnvrg/actions/
--rw-r--r--   0 leah4kosh   (501) staff       (20)       42 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/actions/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2548 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/actions/experiment_actions.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.830298 cnvrg-0.7.6/cnvrg/actions/file_actions/
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/actions/file_actions/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      291 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/actions/global_actions.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2898 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/actions/project_actions.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/actions/status_helpers.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.838809 cnvrg-0.7.6/cnvrg/charts/
--rw-r--r--   0 leah4kosh   (501) staff       (20)     4776 2020-06-12 18:12:30.000000 cnvrg-0.7.6/cnvrg/charts/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2798 2019-12-22 14:21:28.000000 cnvrg-0.7.6/cnvrg/charts/pandas_analyzer.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.896354 cnvrg-0.7.6/cnvrg/helpers/
--rw-r--r--   0 leah4kosh   (501) staff       (20)       62 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3304 2020-09-07 09:28:07.000000 cnvrg-0.7.6/cnvrg/helpers/apis_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      907 2020-06-25 08:11:06.000000 cnvrg-0.7.6/cnvrg/helpers/args_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      842 2020-06-23 11:28:19.000000 cnvrg-0.7.6/cnvrg/helpers/async_runner.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3224 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/helpers/auth_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      834 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/chart_show_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1037 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/cli_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      612 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/clone_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1238 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/cnvrgignore_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2969 2020-06-25 08:19:45.000000 cnvrg-0.7.6/cnvrg/helpers/config_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2256 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/helpers/control_stdout_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      336 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/crypto_helpers.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      232 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/helpers/data_working_dir_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1316 2020-02-23 00:07:47.000000 cnvrg-0.7.6/cnvrg/helpers/env_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      251 2020-03-31 11:36:39.000000 cnvrg-0.7.6/cnvrg/helpers/error_catcher.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2975 2019-08-29 06:44:11.000000 cnvrg-0.7.6/cnvrg/helpers/export_library_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1481 2019-09-23 15:06:07.000000 cnvrg-0.7.6/cnvrg/helpers/files_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      920 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/hash_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      881 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/hyper_search_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      121 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/libs_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1191 2019-12-22 14:21:28.000000 cnvrg-0.7.6/cnvrg/helpers/logger_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1477 2019-09-23 15:06:07.000000 cnvrg-0.7.6/cnvrg/helpers/parallel_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1842 2020-06-12 18:12:30.000000 cnvrg-0.7.6/cnvrg/helpers/param_build_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      275 2019-12-22 14:21:28.000000 cnvrg-0.7.6/cnvrg/helpers/param_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      261 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/random_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1910 2020-06-25 08:11:06.000000 cnvrg-0.7.6/cnvrg/helpers/spawn_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      401 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/status_helpers.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      147 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/string_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      180 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/time_helper.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      267 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/helpers/url_builder_helper.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.897449 cnvrg-0.7.6/cnvrg/libs/
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/libs/__init__.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.898664 cnvrg-0.7.6/cnvrg/libs/limit/
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1189 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/libs/limit/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      319 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/main.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.946576 cnvrg-0.7.6/cnvrg/modules/
--rw-r--r--   0 leah4kosh   (501) staff       (20)       82 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/modules/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      699 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/modules/base_module.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     5433 2019-12-02 07:12:19.000000 cnvrg-0.7.6/cnvrg/modules/cnvrg_files.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3707 2019-12-02 07:12:19.000000 cnvrg-0.7.6/cnvrg/modules/cnvrg_job.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1126 2019-08-29 06:44:11.000000 cnvrg-0.7.6/cnvrg/modules/cnvrg_keras_callback.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      377 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/cnvrg_me.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3805 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/modules/commituploader.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.954360 cnvrg-0.7.6/cnvrg/modules/data_connector/
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1145 2019-08-29 06:44:11.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1435 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/base_connector.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.975147 cnvrg-0.7.6/cnvrg/modules/data_connector/files_connector/
--rw-r--r--   0 leah4kosh   (501) staff       (20)      186 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/files_connector/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     4261 2019-08-29 06:44:11.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/files_connector/base_files_connector.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1359 2019-12-25 12:55:47.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/files_connector/dataset_connector.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3406 2019-08-29 06:44:11.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/files_connector/s3_bucket_connector.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.985022 cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/
--rw-r--r--   0 leah4kosh   (501) staff       (20)      263 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      441 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/base_sql_connector.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      932 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/hive_connector.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3616 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/mysql_connector.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      660 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/snowflake_connector.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.991360 cnvrg-0.7.6/cnvrg/modules/data_connector/stream_connector/
--rw-r--r--   0 leah4kosh   (501) staff       (20)       88 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/stream_connector/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1758 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/stream_connector/base_stream_connector.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      978 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_connector/stream_connector/kafka_connector.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2978 2019-08-12 13:29:30.000000 cnvrg-0.7.6/cnvrg/modules/data_loader.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     6276 2020-05-13 09:15:10.000000 cnvrg-0.7.6/cnvrg/modules/dataset.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     9623 2020-09-22 07:21:49.000000 cnvrg-0.7.6/cnvrg/modules/endpoint.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      560 2020-07-20 08:07:44.000000 cnvrg-0.7.6/cnvrg/modules/errors.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)    19955 2020-08-20 08:56:56.000000 cnvrg-0.7.6/cnvrg/modules/experiment.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2388 2020-08-24 10:25:39.000000 cnvrg-0.7.6/cnvrg/modules/flow.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      830 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/flow_version.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1163 2019-08-29 06:44:11.000000 cnvrg-0.7.6/cnvrg/modules/grid.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     8699 2020-07-21 03:26:37.000000 cnvrg-0.7.6/cnvrg/modules/library.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.993444 cnvrg-0.7.6/cnvrg/modules/mixins/
--rw-r--r--   0 leah4kosh   (501) staff       (20)       61 2019-12-24 22:42:47.000000 cnvrg-0.7.6/cnvrg/modules/mixins/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3491 2020-06-12 18:12:30.000000 cnvrg-0.7.6/cnvrg/modules/mixins/charts_mixin.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:07.010652 cnvrg-0.7.6/cnvrg/modules/moduleHelpers/
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/modules/moduleHelpers/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     7817 2020-08-20 08:56:56.000000 cnvrg-0.7.6/cnvrg/modules/project.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:07.031458 cnvrg-0.7.6/cnvrg/modules/storage/
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1236 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/storage/__init__.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:07.033799 cnvrg-0.7.6/cnvrg/modules/storage/azure/
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2020-06-12 18:12:30.000000 cnvrg-0.7.6/cnvrg/modules/storage/azure/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1485 2020-07-06 09:01:50.000000 cnvrg-0.7.6/cnvrg/modules/storage/azure/storage.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1466 2020-06-25 08:19:45.000000 cnvrg-0.7.6/cnvrg/modules/storage/base_storage.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     8925 2020-08-20 08:56:56.000000 cnvrg-0.7.6/cnvrg/modules/storage/file_uploader.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:07.038908 cnvrg-0.7.6/cnvrg/modules/storage/gcp/
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/storage/gcp/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1264 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/storage/gcp/storage.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:07.042296 cnvrg-0.7.6/cnvrg/modules/storage/minio/
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2020-06-12 18:12:30.000000 cnvrg-0.7.6/cnvrg/modules/storage/minio/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1497 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/storage/minio/storage.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      921 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/storage/progress.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:07.046903 cnvrg-0.7.6/cnvrg/modules/storage/s3/
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2020-06-12 18:12:30.000000 cnvrg-0.7.6/cnvrg/modules/storage/s3/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1638 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/storage/s3/storage.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3637 2020-06-19 18:07:27.000000 cnvrg-0.7.6/cnvrg/modules/storage/storage.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:07.071431 cnvrg-0.7.6/cnvrg/subcommands/
--rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/subcommands/__init__.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     1244 2020-01-06 11:14:36.000000 cnvrg-0.7.6/cnvrg/subcommands/cnvrg.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      136 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/subcommands/experiment.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)     2205 2020-07-05 08:17:15.000000 cnvrg-0.7.6/cnvrg/subcommands/library.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)      656 2019-07-28 13:08:03.000000 cnvrg-0.7.6/cnvrg/subcommands/project.py
--rw-r--r--   0 leah4kosh   (501) staff       (20)       16 2020-09-22 07:28:24.000000 cnvrg-0.7.6/cnvrg/version.py
-drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-09-22 07:38:06.823156 cnvrg-0.7.6/cnvrg.egg-info/
--rw-r--r--   0 leah4kosh   (501) staff       (20)      208 2020-09-22 07:38:06.000000 cnvrg-0.7.6/cnvrg.egg-info/PKG-INFO
--rw-r--r--   0 leah4kosh   (501) staff       (20)     3552 2020-09-22 07:38:06.000000 cnvrg-0.7.6/cnvrg.egg-info/SOURCES.txt
--rw-r--r--   0 leah4kosh   (501) staff       (20)        1 2020-09-22 07:38:06.000000 cnvrg-0.7.6/cnvrg.egg-info/dependency_links.txt
--rw-r--r--   0 leah4kosh   (501) staff       (20)       61 2020-09-22 07:38:06.000000 cnvrg-0.7.6/cnvrg.egg-info/entry_points.txt
--rw-r--r--   0 leah4kosh   (501) staff       (20)      151 2020-09-22 07:38:06.000000 cnvrg-0.7.6/cnvrg.egg-info/requires.txt
--rw-r--r--   0 leah4kosh   (501) staff       (20)        6 2020-09-22 07:38:06.000000 cnvrg-0.7.6/cnvrg.egg-info/top_level.txt
--rw-r--r--   0 leah4kosh   (501) staff       (20)       38 2020-09-22 07:38:07.072664 cnvrg-0.7.6/setup.cfg
--rw-r--r--   0 leah4kosh   (501) staff       (20)      581 2020-07-09 09:42:25.000000 cnvrg-0.7.6/setup.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.839824 cnvrg-0.7.8/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      208 2020-10-02 08:51:46.839487 cnvrg-0.7.8/PKG-INFO
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.715399 cnvrg-0.7.8/cnvrg/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      563 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/__init__.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.728336 cnvrg-0.7.8/cnvrg/actions/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)       42 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/actions/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     2548 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/actions/experiment_actions.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.729206 cnvrg-0.7.8/cnvrg/actions/file_actions/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/actions/file_actions/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      291 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/actions/global_actions.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     2898 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/actions/project_actions.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/actions/status_helpers.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.732493 cnvrg-0.7.8/cnvrg/charts/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     4776 2020-06-12 18:12:30.000000 cnvrg-0.7.8/cnvrg/charts/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     2798 2019-12-22 14:21:28.000000 cnvrg-0.7.8/cnvrg/charts/pandas_analyzer.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.775784 cnvrg-0.7.8/cnvrg/helpers/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)       62 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3443 2020-10-02 08:50:18.000000 cnvrg-0.7.8/cnvrg/helpers/apis_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      907 2020-06-25 08:11:06.000000 cnvrg-0.7.8/cnvrg/helpers/args_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      842 2020-06-23 11:28:19.000000 cnvrg-0.7.8/cnvrg/helpers/async_runner.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3224 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/helpers/auth_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      834 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/chart_show_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1037 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/cli_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      612 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/clone_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1238 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/cnvrgignore_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     2969 2020-06-25 08:19:45.000000 cnvrg-0.7.8/cnvrg/helpers/config_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     2246 2020-10-02 08:50:18.000000 cnvrg-0.7.8/cnvrg/helpers/control_stdout_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      336 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/crypto_helpers.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      232 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/helpers/data_working_dir_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1316 2020-02-23 00:07:47.000000 cnvrg-0.7.8/cnvrg/helpers/env_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      251 2020-03-31 11:36:39.000000 cnvrg-0.7.8/cnvrg/helpers/error_catcher.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     2975 2019-08-29 06:44:11.000000 cnvrg-0.7.8/cnvrg/helpers/export_library_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1481 2019-09-23 15:06:07.000000 cnvrg-0.7.8/cnvrg/helpers/files_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      920 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/hash_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      881 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/hyper_search_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      121 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/libs_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1191 2019-12-22 14:21:28.000000 cnvrg-0.7.8/cnvrg/helpers/logger_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1477 2019-09-23 15:06:07.000000 cnvrg-0.7.8/cnvrg/helpers/parallel_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1842 2020-06-12 18:12:30.000000 cnvrg-0.7.8/cnvrg/helpers/param_build_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      275 2019-12-22 14:21:28.000000 cnvrg-0.7.8/cnvrg/helpers/param_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      261 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/random_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1910 2020-06-25 08:11:06.000000 cnvrg-0.7.8/cnvrg/helpers/spawn_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      401 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/status_helpers.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      147 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/string_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      180 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/time_helper.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      267 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/helpers/url_builder_helper.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.776862 cnvrg-0.7.8/cnvrg/libs/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/libs/__init__.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.778022 cnvrg-0.7.8/cnvrg/libs/limit/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1189 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/libs/limit/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      319 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/main.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.796004 cnvrg-0.7.8/cnvrg/modules/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)       82 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/modules/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      699 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/modules/base_module.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     5433 2019-12-02 07:12:19.000000 cnvrg-0.7.8/cnvrg/modules/cnvrg_files.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3707 2019-12-02 07:12:19.000000 cnvrg-0.7.8/cnvrg/modules/cnvrg_job.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1126 2019-08-29 06:44:11.000000 cnvrg-0.7.8/cnvrg/modules/cnvrg_keras_callback.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      377 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/cnvrg_me.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3805 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/modules/commituploader.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.800803 cnvrg-0.7.8/cnvrg/modules/data_connector/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1145 2019-08-29 06:44:11.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1435 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/base_connector.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.806467 cnvrg-0.7.8/cnvrg/modules/data_connector/files_connector/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      186 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/files_connector/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     4261 2019-08-29 06:44:11.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/files_connector/base_files_connector.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1359 2019-12-25 12:55:47.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/files_connector/dataset_connector.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3406 2019-08-29 06:44:11.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/files_connector/s3_bucket_connector.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.812320 cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      263 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      441 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/base_sql_connector.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      932 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/hive_connector.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3616 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/mysql_connector.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      660 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/snowflake_connector.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.816501 cnvrg-0.7.8/cnvrg/modules/data_connector/stream_connector/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)       88 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/stream_connector/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1758 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/stream_connector/base_stream_connector.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      978 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_connector/stream_connector/kafka_connector.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     2978 2019-08-12 13:29:30.000000 cnvrg-0.7.8/cnvrg/modules/data_loader.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     6276 2020-05-13 09:15:10.000000 cnvrg-0.7.8/cnvrg/modules/dataset.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     9623 2020-09-25 12:11:33.000000 cnvrg-0.7.8/cnvrg/modules/endpoint.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      560 2020-07-20 08:07:44.000000 cnvrg-0.7.8/cnvrg/modules/errors.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)    19955 2020-08-20 08:56:56.000000 cnvrg-0.7.8/cnvrg/modules/experiment.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3605 2020-10-02 08:50:18.000000 cnvrg-0.7.8/cnvrg/modules/flow.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      830 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/flow_version.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1163 2019-08-29 06:44:11.000000 cnvrg-0.7.8/cnvrg/modules/grid.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     8699 2020-07-21 03:26:37.000000 cnvrg-0.7.8/cnvrg/modules/library.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.818606 cnvrg-0.7.8/cnvrg/modules/mixins/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)       61 2019-12-24 22:42:47.000000 cnvrg-0.7.8/cnvrg/modules/mixins/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3491 2020-06-12 18:12:30.000000 cnvrg-0.7.8/cnvrg/modules/mixins/charts_mixin.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.819470 cnvrg-0.7.8/cnvrg/modules/moduleHelpers/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/modules/moduleHelpers/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     7817 2020-08-20 08:56:56.000000 cnvrg-0.7.8/cnvrg/modules/project.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.823756 cnvrg-0.7.8/cnvrg/modules/storage/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1236 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/storage/__init__.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.825422 cnvrg-0.7.8/cnvrg/modules/storage/azure/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2020-06-12 18:12:30.000000 cnvrg-0.7.8/cnvrg/modules/storage/azure/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1485 2020-07-06 09:01:50.000000 cnvrg-0.7.8/cnvrg/modules/storage/azure/storage.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1466 2020-06-25 08:19:45.000000 cnvrg-0.7.8/cnvrg/modules/storage/base_storage.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     8925 2020-08-20 08:56:56.000000 cnvrg-0.7.8/cnvrg/modules/storage/file_uploader.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.826892 cnvrg-0.7.8/cnvrg/modules/storage/gcp/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/storage/gcp/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1264 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/storage/gcp/storage.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.828542 cnvrg-0.7.8/cnvrg/modules/storage/minio/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2020-06-12 18:12:30.000000 cnvrg-0.7.8/cnvrg/modules/storage/minio/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1497 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/storage/minio/storage.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      921 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/storage/progress.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.832765 cnvrg-0.7.8/cnvrg/modules/storage/s3/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2020-06-12 18:12:30.000000 cnvrg-0.7.8/cnvrg/modules/storage/s3/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1638 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/storage/s3/storage.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3637 2020-06-19 18:07:27.000000 cnvrg-0.7.8/cnvrg/modules/storage/storage.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.838987 cnvrg-0.7.8/cnvrg/subcommands/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        0 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/subcommands/__init__.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     1244 2020-01-06 11:14:36.000000 cnvrg-0.7.8/cnvrg/subcommands/cnvrg.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      136 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/subcommands/experiment.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     2205 2020-07-05 08:17:15.000000 cnvrg-0.7.8/cnvrg/subcommands/library.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      656 2019-07-28 13:08:03.000000 cnvrg-0.7.8/cnvrg/subcommands/project.py
+-rw-r--r--   0 leah4kosh   (501) staff       (20)       16 2020-10-02 08:50:29.000000 cnvrg-0.7.8/cnvrg/version.py
+drwxr-xr-x   0 leah4kosh   (501) staff       (20)        0 2020-10-02 08:51:46.722829 cnvrg-0.7.8/cnvrg.egg-info/
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      208 2020-10-02 08:51:46.000000 cnvrg-0.7.8/cnvrg.egg-info/PKG-INFO
+-rw-r--r--   0 leah4kosh   (501) staff       (20)     3552 2020-10-02 08:51:46.000000 cnvrg-0.7.8/cnvrg.egg-info/SOURCES.txt
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        1 2020-10-02 08:51:46.000000 cnvrg-0.7.8/cnvrg.egg-info/dependency_links.txt
+-rw-r--r--   0 leah4kosh   (501) staff       (20)       61 2020-10-02 08:51:46.000000 cnvrg-0.7.8/cnvrg.egg-info/entry_points.txt
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      151 2020-10-02 08:51:46.000000 cnvrg-0.7.8/cnvrg.egg-info/requires.txt
+-rw-r--r--   0 leah4kosh   (501) staff       (20)        6 2020-10-02 08:51:46.000000 cnvrg-0.7.8/cnvrg.egg-info/top_level.txt
+-rw-r--r--   0 leah4kosh   (501) staff       (20)       38 2020-10-02 08:51:46.839937 cnvrg-0.7.8/setup.cfg
+-rw-r--r--   0 leah4kosh   (501) staff       (20)      581 2020-07-09 09:42:25.000000 cnvrg-0.7.8/setup.py
```

### Comparing `cnvrg-0.7.6/cnvrg/__init__.py` & `cnvrg-0.7.8/cnvrg/__init__.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/actions/experiment_actions.py` & `cnvrg-0.7.8/cnvrg/actions/experiment_actions.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/actions/project_actions.py` & `cnvrg-0.7.8/cnvrg/actions/project_actions.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/charts/__init__.py` & `cnvrg-0.7.8/cnvrg/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/charts/pandas_analyzer.py` & `cnvrg-0.7.8/cnvrg/charts/pandas_analyzer.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/apis_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/apis_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from cnvrg.modules.errors import CnvrgError
 import cnvrg.helpers.auth_helper as auth_helper
 import cnvrg.helpers.logger_helper as logger_helper
 from cnvrg.helpers.url_builder_helper import url_join
 import urllib
 import ssl
 from cnvrg.helpers.error_catcher import suppress_exception
+import urllib3
 
 JSON_HEADERS = {
     "Content-Type": "application/json"
 }
 
 def verify_logged_in():
     if not credentials.logged_in:
@@ -28,23 +29,25 @@
         logger_helper.log_error(resp.text)
         logger_helper.log_bad_response(**kwargs)
         return {"status": 400, "error": str(e)}
 
 
 @suppress_exception
 def request(action, url, **kwargs):
+    urllib3.disable_warnings()
     callee = getattr(session, action)
     try:
         resp = callee(url, **kwargs)
         return __parse_resp(resp, url=url, **kwargs)
     except Exception as e:
         return {"status": 400, "error": str(e)}
 
 @suppress_exception
 def get_v2(url):
+    urllib3.disable_warnings()
     verify_logged_in()
     get_url = url_join(credentials.api_url, "v2", url)
     return requests.get(url=get_url, headers={"Auth-Token": credentials.token}, verify=False)
 
 @suppress_exception
 def get(url, data=None):
     verify_logged_in()
@@ -56,21 +59,23 @@
 def post(url, data=None, files=None):
     verify_logged_in()
     get_url = url_join(base_url, url)
     return request('post', get_url, timeout=900, data=json.dumps(data), files=files, verify=False)
 
 @suppress_exception
 def post_v2(url, data):
+    urllib3.disable_warnings()
     verify_logged_in()
     get_url = url_join(credentials.api_url, "v2", url)
     return requests.post(url=get_url, json=data, headers={"Auth-Token": credentials.token}, verify=False)
 
 
 @suppress_exception
 def send_file(url, data=None, files=None):
+    urllib3.disable_warnings()
     verify_logged_in()
     get_url = url_join(base_url, url)
     resp = requests.post(get_url, files=files, data=data, headers={"AUTH-TOKEN": credentials.token}, verify=False)
     return __parse_resp(resp, url=url, data=data)
 
 
 @suppress_exception
```

### Comparing `cnvrg-0.7.6/cnvrg/helpers/args_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/args_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/async_runner.py` & `cnvrg-0.7.8/cnvrg/helpers/async_runner.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/auth_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/auth_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/chart_show_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/chart_show_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/cli_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/cli_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/clone_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/clone_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/cnvrgignore_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/cnvrgignore_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/config_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/config_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/control_stdout_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/control_stdout_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
     ## those threads will monitor the buffer and will call the relevant "prints"
     t = threading.Thread(target=check_buffer_thread, args=(buffer, get_buffer_callbacks(callback, stdio)))
     terr = threading.Thread(target=check_buffer_thread, args=(err_buffer, get_buffer_callbacks(err_callback, errio)))
     t.start()
     terr.start()
     try:
-        callable(*arguments)
-        exit_status = 0
+        exit_status = callable(*arguments)
     except Exception as e:
         exit_status = 1
         err_callback(str(e))
     except KeyboardInterrupt as e:
         exit_status = -100
         err_callback("Keyboard Interrupt")
     time.sleep(0.5)
```

### Comparing `cnvrg-0.7.6/cnvrg/helpers/env_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/env_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/export_library_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/export_library_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/files_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/files_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/hash_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/hash_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/hyper_search_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/hyper_search_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/logger_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/logger_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/parallel_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/parallel_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/param_build_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/param_build_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/helpers/spawn_helper.py` & `cnvrg-0.7.8/cnvrg/helpers/spawn_helper.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/libs/limit/__init__.py` & `cnvrg-0.7.8/cnvrg/libs/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/base_module.py` & `cnvrg-0.7.8/cnvrg/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/cnvrg_files.py` & `cnvrg-0.7.8/cnvrg/modules/cnvrg_files.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/cnvrg_job.py` & `cnvrg-0.7.8/cnvrg/modules/cnvrg_job.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/cnvrg_keras_callback.py` & `cnvrg-0.7.8/cnvrg/modules/cnvrg_keras_callback.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/commituploader.py` & `cnvrg-0.7.8/cnvrg/modules/commituploader.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/__init__.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/base_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/base_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/files_connector/base_files_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/files_connector/base_files_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/files_connector/dataset_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/files_connector/dataset_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/files_connector/s3_bucket_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/files_connector/s3_bucket_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/hive_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/hive_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/mysql_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/sql_connector/snowflake_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/sql_connector/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/stream_connector/base_stream_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/stream_connector/base_stream_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_connector/stream_connector/kafka_connector.py` & `cnvrg-0.7.8/cnvrg/modules/data_connector/stream_connector/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/data_loader.py` & `cnvrg-0.7.8/cnvrg/modules/data_loader.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/dataset.py` & `cnvrg-0.7.8/cnvrg/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/endpoint.py` & `cnvrg-0.7.8/cnvrg/modules/endpoint.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/errors.py` & `cnvrg-0.7.8/cnvrg/modules/errors.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/experiment.py` & `cnvrg-0.7.8/cnvrg/modules/experiment.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/flow.py` & `cnvrg-0.7.8/cnvrg/modules/flow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import yaml
-
+import os
 from cnvrg.modules.project import Project
 from cnvrg.modules.flow_version import FlowVersion
 from cnvrg.helpers.url_builder_helper import url_join
 from cnvrg.modules.errors import CnvrgError
 
 import cnvrg.helpers.param_build_helper as param_build_helper
 import cnvrg.helpers.apis_helper as apis_helper
@@ -31,14 +31,48 @@
         status = resp["status"]
         if status == 200:
             fv_title = resp["flow_version"]["title"]
             return FlowVersion(self, fv_title, project)
         else:
             raise CnvrgError("Could not create flow")
 
+    def __latest_artifacts(self, task=None):
+        resp = apis_helper.get_v2(
+            url_join(
+                self.project.get_base_url(api="v2"),
+                'flows',
+                self.slug,
+                "latest_end_commits?exec_task_title={}".format(task),
+            )
+        )
+
+        if not resp:
+            return None
+
+        return resp.json().get("artifacts")
+
+    def artifacts(self, task=None):
+        artifacts = self.__latest_artifacts(task=task)
+        if not artifacts: return []
+        return artifacts
+
+    def pull_artifacts(self, path=".", task=None):
+        artifacts = self.artifacts(task=task)
+        mapped_files = []
+        for artifact in artifacts:
+            try:
+                fpath = os.path.join(path, artifact.get("fullpath"))
+                os.makedirs(os.path.dirname(fpath), exist_ok=True)
+                artifact_path = apis_helper.download_file(artifact.get("url"), fpath)
+                mapped_files.append({**artifact, **{"path": os.path.abspath(artifact_path)}})
+            except Exception as e:
+                print(e)
+                print("Error while downloading {}".format(artifact.get("name")))
+        return mapped_files
+
     @staticmethod
     def create(file=None, yaml_content=None, project=None):
         if not file and not yaml_content:
             raise errors.CnvrgError("File or yaml is missing")
 
         project = project or Project()
 
@@ -63,7 +97,8 @@
         if status == 200:
             flow_title = resp["flow_version"]["title"]
             print("Flow {} created successfully".format(flow_title))
             flow_slug = resp["flow_version"]["flow_id"]
             return Flow(flow_slug, project)
         else:
             raise CnvrgError("Could not create flow")
+
```

### Comparing `cnvrg-0.7.6/cnvrg/modules/flow_version.py` & `cnvrg-0.7.8/cnvrg/modules/flow_version.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/grid.py` & `cnvrg-0.7.8/cnvrg/modules/grid.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/library.py` & `cnvrg-0.7.8/cnvrg/modules/library.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/mixins/charts_mixin.py` & `cnvrg-0.7.8/cnvrg/modules/mixins/charts_mixin.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/project.py` & `cnvrg-0.7.8/cnvrg/modules/project.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/__init__.py` & `cnvrg-0.7.8/cnvrg/modules/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/azure/storage.py` & `cnvrg-0.7.8/cnvrg/modules/storage/azure/storage.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/base_storage.py` & `cnvrg-0.7.8/cnvrg/modules/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/file_uploader.py` & `cnvrg-0.7.8/cnvrg/modules/storage/file_uploader.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/gcp/storage.py` & `cnvrg-0.7.8/cnvrg/modules/storage/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/minio/storage.py` & `cnvrg-0.7.8/cnvrg/modules/storage/minio/storage.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/progress.py` & `cnvrg-0.7.8/cnvrg/modules/storage/progress.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/s3/storage.py` & `cnvrg-0.7.8/cnvrg/modules/storage/s3/storage.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/modules/storage/storage.py` & `cnvrg-0.7.8/cnvrg/modules/storage/storage.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/subcommands/cnvrg.py` & `cnvrg-0.7.8/cnvrg/subcommands/cnvrg.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/subcommands/library.py` & `cnvrg-0.7.8/cnvrg/subcommands/library.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg/subcommands/project.py` & `cnvrg-0.7.8/cnvrg/subcommands/project.py`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/cnvrg.egg-info/SOURCES.txt` & `cnvrg-0.7.8/cnvrg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnvrg-0.7.6/setup.py` & `cnvrg-0.7.8/setup.py`

 * *Files identical despite different names*

