# Comparing `tmp/liquer-framework-0.8.0.tar.gz` & `tmp/liquer-framework-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/liquer-framework-0.8.0.tar", last modified: Sun Jan 22 17:38:41 2023, max compression
+gzip compressed data, was "dist/liquer-framework-0.9.0.tar", last modified: Sun Jun 11 17:47:25 2023, max compression
```

## Comparing `liquer-framework-0.8.0.tar` & `liquer-framework-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-01-22 17:38:41.390193 liquer-framework-0.8.0/
--rw-r--r--   0 orest     (1000) orest     (1000)       41 2020-04-26 21:21:24.000000 liquer-framework-0.8.0/MANIFEST.in
--rw-rw-r--   0 orest     (1000) orest     (1000)     7213 2023-01-22 17:38:41.390193 liquer-framework-0.8.0/PKG-INFO
--rw-rw-r--   0 orest     (1000) orest     (1000)     5994 2023-01-22 17:34:02.000000 liquer-framework-0.8.0/README.md
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-01-22 17:38:41.386193 liquer-framework-0.8.0/liquer/
--rw-r--r--   0 orest     (1000) orest     (1000)      185 2023-01-22 17:32:54.000000 liquer-framework-0.8.0/liquer/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      259 2021-10-27 15:33:04.000000 liquer-framework-0.8.0/liquer/blueprint.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    30114 2021-12-15 12:59:32.000000 liquer-framework-0.8.0/liquer/cache.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    32155 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/commands.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3631 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/constants.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    41625 2023-01-21 20:50:42.000000 liquer-framework-0.8.0/liquer/context.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3855 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/dependencies.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-01-22 17:38:41.386193 liquer-framework-0.8.0/liquer/ext/
--rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.8.0/liquer/ext/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     9243 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/ext/basic.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    13175 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/ext/dataframe_batches.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7937 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/ext/lq_datafusion.py
--rw-r--r--   0 orest     (1000) orest     (1000)     4370 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/ext/lq_hxl.py
--rw-r--r--   0 orest     (1000) orest     (1000)     3933 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/ext/lq_keras.py
--rw-r--r--   0 orest     (1000) orest     (1000)     3686 2022-07-07 19:34:25.000000 liquer-framework-0.8.0/liquer/ext/lq_matplotlib.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3447 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/ext/lq_openpyxl.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    16171 2023-01-21 22:45:29.000000 liquer-framework-0.8.0/liquer/ext/lq_pandas.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3432 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/ext/lq_pil.py
--rw-r--r--   0 orest     (1000) orest     (1000)     2304 2021-10-27 15:33:04.000000 liquer-framework-0.8.0/liquer/ext/lq_plotly.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2853 2023-01-21 20:13:08.000000 liquer-framework-0.8.0/liquer/ext/lq_polars.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2244 2023-01-21 17:53:31.000000 liquer-framework-0.8.0/liquer/ext/lq_pptx.py
--rw-r--r--   0 orest     (1000) orest     (1000)      701 2021-10-27 15:33:04.000000 liquer-framework-0.8.0/liquer/ext/lq_pygments.py
--rw-r--r--   0 orest     (1000) orest     (1000)      368 2021-10-27 15:33:04.000000 liquer-framework-0.8.0/liquer/ext/lq_python.py
--rw-r--r--   0 orest     (1000) orest     (1000)     1805 2021-10-27 15:33:04.000000 liquer-framework-0.8.0/liquer/ext/lq_sklearn_regression.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      712 2023-01-21 22:45:23.000000 liquer-framework-0.8.0/liquer/ext/lq_sweetviz.py
--rw-r--r--   0 orest     (1000) orest     (1000)    16409 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/ext/meta.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7325 2023-01-21 22:51:41.000000 liquer-framework-0.8.0/liquer/indexer.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7020 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/metadata.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    30590 2023-01-21 17:53:33.000000 liquer-framework-0.8.0/liquer/parser.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     6273 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/pool.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     1199 2023-01-15 17:53:35.000000 liquer-framework-0.8.0/liquer/query.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    35765 2023-01-21 17:53:34.000000 liquer-framework-0.8.0/liquer/recipes.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     4122 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/remote_store.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     5713 2023-01-08 21:15:57.000000 liquer-framework-0.8.0/liquer/s3_store.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-01-22 17:38:41.386193 liquer-framework-0.8.0/liquer/server/
--rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.8.0/liquer/server/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    14961 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/server/blueprint.py
--rw-r--r--   0 orest     (1000) orest     (1000)    19348 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/server/handlers.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-01-22 17:38:41.386193 liquer-framework-0.8.0/liquer/server/static/
--rw-rw-r--   0 orest     (1000) orest     (1000)    26489 2021-01-31 21:05:09.000000 liquer-framework-0.8.0/liquer/server/static/index.html
--rw-rw-r--   0 orest     (1000) orest     (1000)    18057 2021-12-15 17:45:48.000000 liquer-framework-0.8.0/liquer/server/static/liquer.js
--rw-r--r--   0 orest     (1000) orest     (1000)     6071 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/server/tornado_handlers.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7656 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/state.py
--rw-r--r--   0 orest     (1000) orest     (1000)    17774 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/state_types.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    44447 2023-01-21 22:51:19.000000 liquer-framework-0.8.0/liquer/store.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    11266 2022-07-30 08:12:25.000000 liquer-framework-0.8.0/liquer/template.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      621 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/tools.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      521 2023-01-21 17:53:32.000000 liquer-framework-0.8.0/liquer/util.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2721 2023-01-21 22:45:45.000000 liquer-framework-0.8.0/liquer/web.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-01-22 17:38:41.390193 liquer-framework-0.8.0/liquer_framework.egg-info/
--rw-r--r--   0 orest     (1000) orest     (1000)     7213 2023-01-22 17:38:41.000000 liquer-framework-0.8.0/liquer_framework.egg-info/PKG-INFO
--rw-r--r--   0 orest     (1000) orest     (1000)     1289 2023-01-22 17:38:41.000000 liquer-framework-0.8.0/liquer_framework.egg-info/SOURCES.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        1 2023-01-22 17:38:41.000000 liquer-framework-0.8.0/liquer_framework.egg-info/dependency_links.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        1 2019-12-07 17:16:04.000000 liquer-framework-0.8.0/liquer_framework.egg-info/not-zip-safe
--rw-r--r--   0 orest     (1000) orest     (1000)        6 2023-01-22 17:38:41.000000 liquer-framework-0.8.0/liquer_framework.egg-info/requires.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        7 2023-01-22 17:38:41.000000 liquer-framework-0.8.0/liquer_framework.egg-info/top_level.txt
--rw-rw-r--   0 orest     (1000) orest     (1000)       38 2023-01-22 17:38:41.390193 liquer-framework-0.8.0/setup.cfg
--rw-r--r--   0 orest     (1000) orest     (1000)      702 2023-01-22 17:32:42.000000 liquer-framework-0.8.0/setup.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.458686 liquer-framework-0.9.0/
+-rw-r--r--   0 orest     (1000) orest     (1000)       67 2023-05-18 20:29:33.000000 liquer-framework-0.9.0/MANIFEST.in
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7667 2023-06-11 17:47:25.458686 liquer-framework-0.9.0/PKG-INFO
+-rw-rw-r--   0 orest     (1000) orest     (1000)     6456 2023-06-11 17:29:55.000000 liquer-framework-0.9.0/README.md
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.442685 liquer-framework-0.9.0/liquer/
+-rw-r--r--   0 orest     (1000) orest     (1000)      185 2023-01-22 17:32:54.000000 liquer-framework-0.9.0/liquer/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      259 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/blueprint.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    30437 2023-04-22 13:59:35.000000 liquer-framework-0.9.0/liquer/cache.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    32155 2023-02-04 11:03:51.000000 liquer-framework-0.9.0/liquer/commands.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3631 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/constants.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    41902 2023-05-18 22:09:05.000000 liquer-framework-0.9.0/liquer/context.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3855 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/dependencies.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.450686 liquer-framework-0.9.0/liquer/ext/
+-rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.0/liquer/ext/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     9243 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/basic.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    13175 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/ext/dataframe_batches.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7937 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_datafusion.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     4381 2023-05-10 20:11:49.000000 liquer-framework-0.9.0/liquer/ext/lq_hxl.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     3933 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_keras.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     3686 2022-07-07 19:34:25.000000 liquer-framework-0.9.0/liquer/ext/lq_matplotlib.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3447 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_openpyxl.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    16337 2023-05-10 20:10:02.000000 liquer-framework-0.9.0/liquer/ext/lq_pandas.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3432 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_pil.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     2304 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/ext/lq_plotly.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2853 2023-01-21 20:13:08.000000 liquer-framework-0.9.0/liquer/ext/lq_polars.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2244 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_pptx.py
+-rw-r--r--   0 orest     (1000) orest     (1000)      701 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/ext/lq_pygments.py
+-rw-r--r--   0 orest     (1000) orest     (1000)      368 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/ext/lq_python.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     1805 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/ext/lq_sklearn_regression.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      712 2023-01-21 22:45:23.000000 liquer-framework-0.9.0/liquer/ext/lq_sweetviz.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     4300 2023-05-18 21:10:45.000000 liquer-framework-0.9.0/liquer/ext/lq_whoosh.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    16409 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/ext/meta.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7326 2023-05-16 21:41:40.000000 liquer-framework-0.9.0/liquer/indexer.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7020 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/metadata.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    34618 2023-05-10 20:15:46.000000 liquer-framework-0.9.0/liquer/parser.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     6273 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/pool.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     1199 2023-01-15 17:53:35.000000 liquer-framework-0.9.0/liquer/query.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    35940 2023-05-10 20:16:08.000000 liquer-framework-0.9.0/liquer/recipes.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     4122 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/remote_store.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     5713 2023-01-08 21:15:57.000000 liquer-framework-0.9.0/liquer/s3_store.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.454686 liquer-framework-0.9.0/liquer/server/
+-rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.0/liquer/server/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    14961 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/server/blueprint.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    19882 2023-05-18 22:06:45.000000 liquer-framework-0.9.0/liquer/server/handlers.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.454686 liquer-framework-0.9.0/liquer/server/static/
+-rw-rw-r--   0 orest     (1000) orest     (1000)    26489 2021-01-31 21:05:09.000000 liquer-framework-0.9.0/liquer/server/static/index.html
+-rw-rw-r--   0 orest     (1000) orest     (1000)    18057 2021-12-15 17:45:48.000000 liquer-framework-0.9.0/liquer/server/static/liquer.js
+-rw-r--r--   0 orest     (1000) orest     (1000)     7371 2023-05-18 21:51:28.000000 liquer-framework-0.9.0/liquer/server/tornado_handlers.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7656 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/state.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    17774 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/state_types.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    44447 2023-01-21 22:51:19.000000 liquer-framework-0.9.0/liquer/store.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    11266 2022-07-30 08:12:25.000000 liquer-framework-0.9.0/liquer/template.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      621 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/tools.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      521 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/util.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2721 2023-01-21 22:45:45.000000 liquer-framework-0.9.0/liquer/web.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.458686 liquer-framework-0.9.0/liquer_framework.egg-info/
+-rw-r--r--   0 orest     (1000) orest     (1000)     7667 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/PKG-INFO
+-rw-r--r--   0 orest     (1000) orest     (1000)     1313 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        1 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        1 2019-12-07 17:16:04.000000 liquer-framework-0.9.0/liquer_framework.egg-info/not-zip-safe
+-rw-r--r--   0 orest     (1000) orest     (1000)        6 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/requires.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        7 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/top_level.txt
+-rw-rw-r--   0 orest     (1000) orest     (1000)       38 2023-06-11 17:47:25.458686 liquer-framework-0.9.0/setup.cfg
+-rw-r--r--   0 orest     (1000) orest     (1000)      702 2023-06-11 17:07:10.000000 liquer-framework-0.9.0/setup.py
```

### Comparing `liquer-framework-0.8.0/PKG-INFO` & `liquer-framework-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquer-framework
-Version: 0.8.0
+Version: 0.9.0
 Summary: LiQuer - Query in (URL) link
 Home-page: https://github.com/orest-d/liquer
 Author: Orest Dubay
 Author-email: orest3.dubay@gmail.com
 License: UNKNOWN
 Description: # LiQuer (Link Query) 
         
@@ -38,14 +38,20 @@
         
         ```
         pip install liquer-framework
         ```
         
         # News
         
+        ## Changes in v0.9
+        - Basic search-engine support - [whoosh](https://whoosh.readthedocs.io/en/latest/intro.html) based on indexer. Current implementation is indexing title and description from the metadata and allows to search interactively via a simple web-interface. See *examples/whoosh_example.py*.
+        - Relative path support in recipes (recipe queries can contain '.' and/or '..' as a reference to the current warking directory or parent directory). 
+        - Tornad-based server with restricted access only supporting reading, but not writing and execution. This can be either used directly or as a starting point for developing a customized secure server. See *examples/hello_server_tornado_ro.py*.
+        
+        
         ## Changes in v0.8
         - Early indexer support - customized updating of metadata, future integration into search engines
         - Specialized indexers allow to specify/customize *tools* that can be used for viewing and editing in GUI.
         - Added S3 store
         - Remote store allows to mount a remote LiQuer server as a store
         
         
@@ -91,22 +97,15 @@
         - 2022-01-03 - v0.7.0  - many enhancements - e.g. modular recipes, support for datafusion, pptx, pillow
         - 2022-01-04 - v0.7.1  - root path bugfix, sync store
         - 2022-01-05 - v0.7.2  - several small fixes, e.g. fixing missing log in recipe-created metadata
         - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
         - 2022-01-07 - v0.7.4  - more bugfixes
         - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
         - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
-        - 2022-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
+        - 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
+        - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
         
-        ### New features
-        - API documentation improved on multiple places
-        - EXTERNAL status
-        - Basic support for DataFusion, pptx-python, Pillow images
-        - Tornado driver updated
-        - Extensible recipes; parquet_sql recipe type
-        - Read-only store proxy
-        - v0.7 is accompanied with new GUI [liquer-gui v0.1.0](https://github.com/orest-d/liquer-gui)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `liquer-framework-0.8.0/README.md` & `liquer-framework-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 
 ```
 pip install liquer-framework
 ```
 
 # News
 
+## Changes in v0.9
+- Basic search-engine support - [whoosh](https://whoosh.readthedocs.io/en/latest/intro.html) based on indexer. Current implementation is indexing title and description from the metadata and allows to search interactively via a simple web-interface. See *examples/whoosh_example.py*.
+- Relative path support in recipes (recipe queries can contain '.' and/or '..' as a reference to the current warking directory or parent directory). 
+- Tornad-based server with restricted access only supporting reading, but not writing and execution. This can be either used directly or as a starting point for developing a customized secure server. See *examples/hello_server_tornado_ro.py*.
+
+
 ## Changes in v0.8
 - Early indexer support - customized updating of metadata, future integration into search engines
 - Specialized indexers allow to specify/customize *tools* that can be used for viewing and editing in GUI.
 - Added S3 store
 - Remote store allows to mount a remote LiQuer server as a store
 
 
@@ -83,17 +89,9 @@
 - 2022-01-03 - v0.7.0  - many enhancements - e.g. modular recipes, support for datafusion, pptx, pillow
 - 2022-01-04 - v0.7.1  - root path bugfix, sync store
 - 2022-01-05 - v0.7.2  - several small fixes, e.g. fixing missing log in recipe-created metadata
 - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
 - 2022-01-07 - v0.7.4  - more bugfixes
 - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
 - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
-- 2022-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
-
-### New features
-- API documentation improved on multiple places
-- EXTERNAL status
-- Basic support for DataFusion, pptx-python, Pillow images
-- Tornado driver updated
-- Extensible recipes; parquet_sql recipe type
-- Read-only store proxy
-- v0.7 is accompanied with new GUI [liquer-gui v0.1.0](https://github.com/orest-d/liquer-gui)
+- 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
+- 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh)
```

### Comparing `liquer-framework-0.8.0/liquer/cache.py` & `liquer-framework-0.9.0/liquer/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,14 +346,17 @@
 
     def __repr__(self):
         return f"CacheProxy({repr(self.cache)})"
 
 
 class NoCache(CacheMixin):
     """Trivial cache object which does not cache any state"""
+    @classmethod
+    def from_config(cls, config):
+        return cls()
 
     def clean(self):
         pass
 
     def get(self, key):
         return None
 
@@ -388,14 +391,18 @@
     may lead to filling the memory, therefore this is not ideal
     for long running services.
     """
 
     def __init__(self):
         self.storage = {}
 
+    @classmethod
+    def from_config(cls, config):
+        return cls()
+
     def clean(self):
         self.storage = {}
 
     def get(self, key):
         state = self.storage.get(key)
 
         if state is None:
@@ -457,14 +464,17 @@
 
     def __init__(self, path):
         self.path = path
         try:
             makedirs(path)
         except FileExistsError:
             pass
+    @classmethod
+    def from_config(cls, config):
+        return cls(config["path"])
 
     def clean(self):
         import glob
 
         print(f"Clean {self}")
         for f in glob.glob(os.path.join(self.path, "*")):
             logging.debug(f"Removing cache file {f}")
@@ -616,14 +626,18 @@
     def __init__(self, store, path, flat=False):
         self.storage = store
         self.path = path
         if not self.storage.is_dir(path):
             self.storage.makedir(path)
         self.flat = flat
 
+    @classmethod
+    def from_config(cls, config):
+        return cls(path=config["path"])
+
     def clean(self):
         import glob
 
         print(f"Clean {self}")
         path = "" if self.path in (None, "") else self.path + "/"
         for key in self.storage.keys():
             if not self.storage.is_dir(key) and key.startswith(path):
```

### Comparing `liquer-framework-0.8.0/liquer/commands.py` & `liquer-framework-0.9.0/liquer/commands.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/constants.py` & `liquer-framework-0.9.0/liquer/constants.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/context.py` & `liquer-framework-0.9.0/liquer/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -938,20 +938,25 @@
             self.set_description(description)
 
         if cache is None:
             cache = self.cache()
 
         self.debug(f"Using cache {repr(cache)}")
         self.debug(f"Try cache {query}")
-        state = cache.get(query.encode())
-        if state is not None:
-            self.debug(f"Cache hit {query}")
-            self._store_state(state)
-            state = self.index_state(state)
-            return state
+        if extra_parameters is None or len(extra_parameters)==0:
+            state = cache.get(query.encode())
+            if state is not None:
+                self.debug(f"Cache hit {query}")
+                self._store_state(state)
+                state = self.index_state(state)
+                return state
+        else:
+            state=None
+            print("Extra parameters specified, cache disabled", extra_parameters)
+            self.debug("Extra parameters specified, cache disabled")
         self.enable_store_metadata = (
             True  # Metadata can be only written after trying to read from cache,
         )
         # so that cache does not get overwritten
         self.debug(f"Cache miss {query}")
 
         if query.is_resource_query():
```

### Comparing `liquer-framework-0.8.0/liquer/dependencies.py` & `liquer-framework-0.9.0/liquer/dependencies.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/basic.py` & `liquer-framework-0.9.0/liquer/ext/basic.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/dataframe_batches.py` & `liquer-framework-0.9.0/liquer/ext/dataframe_batches.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_datafusion.py` & `liquer-framework-0.9.0/liquer/ext/lq_datafusion.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_hxl.py` & `liquer-framework-0.9.0/liquer/ext/lq_hxl.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 c: tag.strip() if tag.strip().startswith("#") else "#" + tag.strip()
                 for c, tag in zip(df.columns, tags)
             }
         ],
         columns=df.columns,
     )
     tags.fillna(value="", inplace=True)
-    return tags.append(df, ignore_index=True)
+    return pd.concat([tags,df], ignore_index=True)
 
 
 @command
 def set_tags(df, *column_tag):
     """Set tags in pandas dataframe, tags are specified as a list with alternating column, tag.
     Creates a first row with tags in a dataframe.
     Hash characters are automatically prepended if not present.
@@ -132,8 +132,8 @@
                 else "#" + column_tag[i + 1].strip()
                 for i in range(0, len(column_tag), 2)
             }
         ],
         columns=df.columns,
     )
     tags.fillna(value="", inplace=True)
-    return tags.append(df, ignore_index=True)
+    return pd.concat([tags, df], ignore_index=True)
```

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_keras.py` & `liquer-framework-0.9.0/liquer/ext/lq_keras.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_matplotlib.py` & `liquer-framework-0.9.0/liquer/ext/lq_matplotlib.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_openpyxl.py` & `liquer-framework-0.9.0/liquer/ext/lq_openpyxl.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_pandas.py` & `liquer-framework-0.9.0/liquer/ext/lq_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,30 +161,30 @@
         raise Exception(f"Unsupported file extension: {extension}")
 
 
 @command
 def append_df(df, url, extension=None):
     """Append dataframe from URL"""
     df1 = df_from(url, extension=extension).get()
-    return df.append(df1, ignore_index=True)
+    return pd.concat([df,df1], ignore_index=True)
 
 
 @command
 def eq(state, *column_values):
     """Equals filter
     Accepts one or more column-value pairs. Keep only rows where value in the column equals specified value.
     Example: eq-column1-1
     """
     df = state.get()
     assert state.type_identifier == "dataframe"
     for i in range(0, len(column_values), 2):
         c = column_values[i]
         v = column_values[i + 1]
         state.log_info(f"Equals: {c} == {v}")
-        index = np.array([x == v for x in df[c]], np.bool)
+        index = np.array([x == v for x in df[c]], bool)
         try:
             if int(v) == float(v):
                 index = index | (df[c] == int(v))
             else:
                 index = index | (df[c] == float(v))
         except:
             pass
@@ -203,24 +203,25 @@
     tags = df.iloc[:1, :]
     df = df.iloc[1:, :]
     assert state.type_identifier == "dataframe"
     for i in range(0, len(column_values), 2):
         c = column_values[i]
         v = column_values[i + 1]
         state.log_info(f"Equals: {c} == {v}")
-        index = np.array([x == v for x in df[c]], np.bool)
+        index = np.array([x == v for x in df[c]], bool)
         try:
             if int(v) == float(v):
                 index = index | (df[c] == int(v))
             else:
                 index = index | (df[c] == float(v))
         except:
             pass
         df = df.loc[index, :]
-    df = tags.append(df, ignore_index=True)
+    #df = tags.append(df, ignore_index=True)
+    df = pd.concat([tags, df], ignore_index=True)
     return state.with_data(df)
 
 
 @command
 def qsplit_df(state, *columns):
     """Quick/query split of dataframe by columns
     Creates a dataframe with unique (combinations of) value from supplied columns and queries
@@ -242,15 +243,16 @@
     data = []
     ql = decode(state.query)
     for row in keys:
         pairs = list(zip(columns, row))
         d = dict(pairs)
         query = encode(ql + [["eq"] + [str(x) for p in pairs for x in p]])
         d[query_column] = query
-        sdf = sdf.append(d, ignore_index=True)
+        data.append(d)
+    sdf = pd.concat([sdf, pd.DataFrame(data)], ignore_index=True)
 
     return state.with_data(sdf)
 
 
 @command
 def qtsplit_df(state, *columns):
     """Quick/query split of dataframe by columns (version expecting a first row with tags)
@@ -268,25 +270,25 @@
     else:
         keys = sorted(df.groupby(by=list(columns)).groups.keys())
 
     query_column = state.vars.get("query_column")
     if query_column is None:
         query_column = "query"
 
-    sdf = pd.DataFrame(columns=list(columns) + [query_column])
-    sdf = sdf.append({c: tags[c] for c in columns}, ignore_index=True)
+    sdf = pd.DataFrame([{c: tags[c] for c in columns}],columns=list(columns) + [query_column])
+    #sdf = sdf.append({c: tags[c] for c in columns}, ignore_index=True)
     data = []
     ql = decode(state.query)
     for row in keys:
         pairs = list(zip(columns, row))
         d = dict(pairs)
         query = encode(ql + [["teq"] + [str(x) for p in pairs for x in p]])
         d[query_column] = query
-        sdf = sdf.append(d, ignore_index=True)
-
+        data.append(d)
+    sdf = pd.concat([sdf, pd.DataFrame(data)], ignore_index=True)
     return state.with_data(sdf)
 
 
 @command
 def split_df(state, *columns):
     """Split of dataframe by columns
     Creates a dataframe with unique (combinations of) value from supplied columns and queries
```

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_pil.py` & `liquer-framework-0.9.0/liquer/ext/lq_pil.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_plotly.py` & `liquer-framework-0.9.0/liquer/ext/lq_plotly.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_polars.py` & `liquer-framework-0.9.0/liquer/ext/lq_polars.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_pptx.py` & `liquer-framework-0.9.0/liquer/ext/lq_pptx.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_pygments.py` & `liquer-framework-0.9.0/liquer/ext/lq_pygments.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_sklearn_regression.py` & `liquer-framework-0.9.0/liquer/ext/lq_sklearn_regression.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/lq_sweetviz.py` & `liquer-framework-0.9.0/liquer/ext/lq_sweetviz.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/ext/meta.py` & `liquer-framework-0.9.0/liquer/ext/meta.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/indexer.py` & `liquer-framework-0.9.0/liquer/indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     def register(self, indexer, identifier=None, priority=100):
         """Register an indexer"""
         if identifier is None:
             if isinstance(indexer, Indexer):
                 identifier = indexer.identifier()
             else:
                 identifier = indexer.__name__
-        print("REGISTER", indexer, identifier, priority)
+        #print("REGISTER", indexer, identifier, priority)
         self.indexers[identifier] = indexer
         self.identifiers = [
             (p, r, i)
             for r, (p, i) in enumerate(
                 (p, i) for (p, r, i) in self.identifiers if i != identifier
             )
         ]
```

### Comparing `liquer-framework-0.8.0/liquer/metadata.py` & `liquer-framework-0.9.0/liquer/metadata.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/parser.py` & `liquer-framework-0.9.0/liquer/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,14 +156,18 @@
         self.query = query
 
 
 class ActionParameter(object):
     def __init__(self, position=None):
         self.position = position or Position()
 
+    def clean_position(self):
+        self.position = Position()
+        return self
+
     def __repr__(self):
         return f"{self.__class__.__name__}({repr(self.position)})"
 
     def __str__(self):
         return f"{self.__class__.__name__} at {self.position}"
 
 
@@ -237,14 +241,20 @@
 
 class ActionRequest(object):
     def __init__(self, name: str, parameters=None, position=None):
         self.name = name
         self.parameters = [] if parameters is None else parameters
         self.position = position or Position()
 
+    def clean_position(self):
+        self.position = Position()
+        for p in self.parameters:
+            p.clean_position()
+        return self
+
     @classmethod
     def from_arguments(cls, name: str, *parameters):
         assert type(name) == str
         typedparam = []
         for p in parameters:
             if isinstance(p, ActionParameter):
                 typedparam.append(p)
@@ -306,14 +316,20 @@
     ):
         self.name = name
         self.level = level
         self.parameters = parameters or []
         self.resource = resource
         self.position = position or Position()
 
+    def clean_position(self):
+        self.position = Position()
+        for p in self.parameters:
+            p.clean_position()
+        return self
+
     def is_trivial(self):
         """Terurns true if the header does not contain any data,
         I.e. trivial header has no name, level is 1 and no parameters.
         Trivial header can be both for resource and query, it does not depend on the resource flas.
         """
         return self.name in ("", None) and self.level == 1 and len(self.parameters) == 0
 
@@ -348,14 +364,26 @@
 
     def __init__(self, header=None, query=None, filename=None):
         "header can be SegmentHeader, query is a list of ActionRequest objects"
         self.header = header
         self.query = query or []
         self.filename = filename
 
+    def clean_position(self):
+        if self.header is not None:
+            self.header.clean_position()
+        for a in self.query:
+            a.clean_position()
+        try:
+            self.filename.clean_position()
+        except:
+            pass
+
+        return self
+
     def predecessor(self):
         if self.filename is None:
             if len(self.query):
                 p = TransformQuerySegment(
                     header=self.header, query=self.query[:-1], filename=None
                 )
                 r = TransformQuerySegment(
@@ -457,14 +485,27 @@
     """Query segment representing a resource, i.e. path to a file in a store."""
 
     def __init__(self, header=None, query=None):
         "header can be SegmentHeader, query is a list of ActionRequest objects"
         self.header = header
         self.query = query or []
 
+    def segment_name(self):
+        if self.header is None:
+            return ""
+        else:
+            return self.header.name
+
+    def clean_position(self):
+        if self.header is not None:
+            self.header.clean_position()
+        for a in self.query:
+            a.clean_position()
+        return self
+
     @property
     def position(self):
         if self.header is not None:
             return self.header.position
         else:
             if len(self.query):
                 return self.query[0].position
@@ -483,14 +524,54 @@
         if len(rqs):
             rqs += "/"
         if len(query):
             return f"{rqs}{query}"
         else:
             return rqs
 
+    def _query_to_absolute(self, path, processed, rest):
+        if len(rest) == 0:
+            return processed
+        if rest[0].encode() == ".":
+            if len(processed) == 0:
+                return self._query_to_absolute(path, path[:], rest[1:])
+            else:
+                return self._query_to_absolute(path, processed, rest[1:])
+
+        if rest[0].encode() == "..":
+            if len(processed) == 0:
+                if len(path) == 0:
+                    raise Exception("Can't go up from root")
+                return self._query_to_absolute(path, path[:-1], rest[1:])
+            else:
+                return self._query_to_absolute(path, processed[:-1], rest[1:])
+        return self._query_to_absolute(path, processed + [rest[0]], rest[1:])
+
+    def to_absolute(self, path):
+        """Convert relative path to absolute path.
+        Replace first "." with *path*, and interpret ".." returning the canonical absolute path.
+        Resource segment header stays unchanged.
+        Path argument should point to a directory key in a store - i.e. it should be an absolute path without a header.
+        Path may be a string or a ResourceQuerySegment.
+        """
+        if isinstance(path, str):
+            if len(path) == 0:
+                path = []
+            else:
+                path = list(resource_path.parseString(path, True))
+                for s in path:
+                    s.clean_position()
+        canonical_path = []
+
+        if self.query is None or len(self.query) == 0:
+            return self
+        return ResourceQuerySegment(
+            header=self.header, query=self._query_to_absolute(path, [], self.query)
+        )
+
     def __repr__(self):
         return f"""ResourceQuerySegment(
   header = {indent(repr(self.header))},
   query  = {indent(list_indent(self.query))}
 )"""
 
     def __str__(self):
@@ -501,14 +582,19 @@
     """Query is a sequence of query segment.
     Typically this will be a resource and and/or a transformation applied to a resource."""
 
     def __init__(self, segments: list = None, absolute=False):
         self.segments = segments or []
         self.absolute = absolute
 
+    def clean_position(self):
+        for s in self.segments:
+            s.clean_position()
+        return self
+
     def filename(self):
         "Return filename if present, None otherwise."
         if len(self.segments):
             segment = self.segments[-1]
             if (
                 isinstance(segment, TransformQuerySegment)
                 and segment.filename is not None
@@ -649,14 +735,39 @@
         if self.is_resource_query():
             if not q.startswith("-"):
                 q = "-R/" + q
         if self.absolute:
             q = "/" + q
         return q
 
+    def to_absolute(self, path, resource_segment_name=""):
+        """Convert relative path to absolute path in the selected resource.
+        Replace first "." with *path*, and interpret ".." returning the canonical absolute path.
+        Everything else besides selected resources stays unchanged.
+        Resources are selected by resource_segment_name (default is the unnamed default resource).
+        None resource_segment_name means all resources.
+        Path argument should point to a directory key in a store - i.e. it should be an absolute path without a header.
+        Path may be a string or a ResourceQuerySegment.
+        """
+        segments = []
+        for s in self.segments:
+            if isinstance(s, TransformQuerySegment):
+                segments.append(s)
+            elif isinstance(s, ResourceQuerySegment):
+                if (
+                    resource_segment_name is None
+                    or resource_segment_name == s.segment_name()
+                ):
+                    segments.append(s.to_absolute(path))
+                else:
+                    segments.append(s)
+            else:
+                raise ValueError(f"Unknown segment type {type(s)}")
+        return Query(segments, absolute=self.absolute)
+
     def __repr__(self):
         return f"""Query(
 {indent(list_indent(self.segments))},
   absolute = {self.absolute}
 )"""
 
     def __str__(self):
```

### Comparing `liquer-framework-0.8.0/liquer/pool.py` & `liquer-framework-0.9.0/liquer/pool.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/query.py` & `liquer-framework-0.9.0/liquer/query.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/recipes.py` & `liquer-framework-0.9.0/liquer/recipes.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,19 +131,20 @@
     def is_volatile(self):
         return self.data.get("volatile", False)
 
 
 def resolve_recipe_definition(r, directory, metadata):
     if type(r) == str:
         try:
-            query = parse(r)
+            query = parse(r).to_absolute(directory)
             filename = query.filename()
             return dict(
                 type="query",
-                query=r,
+                query=query.encode(),
+                original_query=r,
                 CWD=directory,
                 filename=filename,
                 provides=[filename],
             )
         except:
             metadata.warning(
                 f"Can't resolve recipe '{r}'", traceback=traceback.format_exc()
@@ -151,24 +152,25 @@
             print(f"Can't resolve recipe '{r}'")
             traceback.print_exc()
             return None
 
     elif isinstance(r, dict):
         if r.get("type") in (None, "query") and "query" in r:
             try:
-                query = parse(r["query"])
+                query = parse(r["query"]).to_absolute(directory)
                 filename = r.get("filename", query.filename())
                 title = r.get("title", filename)
                 description = r.get(
                     "description", f'Generated from query: {r["query"]}'
                 )
                 rkey = join_key(directory, filename)
                 return dict(
                     type="query",
-                    query=r["query"],
+                    query=query.encode(),
+                    original_query=r["query"],
                     title=title,
                     description=description,
                     CWD=directory,
                     filename=filename,
                     provides=[filename],
                 )
             except:
@@ -853,17 +855,20 @@
                                 )
                             d["recipe_name"] = (
                                 self.to_root_key(recipes_key)
                                 + f"/-Ryaml/{directory}/{i}#"
                                 + d.get("filename", "")
                             )
                             d["recipes_key"] = self.to_root_key(recipes_key)
+
+                            
                             d["recipes_directory"] = (
                                 "" if directory == self.LOCAL_RECIPES else directory
                             )
+
                             try:
                                 recipe = recipe_registry().from_dict(d)
                             except:
                                 metadata.warning(
                                     f"Failed parsing recipe {i+1} in {directory}",
                                     traceback=traceback.format_exc(),
                                 )
```

### Comparing `liquer-framework-0.8.0/liquer/remote_store.py` & `liquer-framework-0.9.0/liquer/remote_store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/s3_store.py` & `liquer-framework-0.9.0/liquer/s3_store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/server/blueprint.py` & `liquer-framework-0.9.0/liquer/server/blueprint.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/server/handlers.py` & `liquer-framework-0.9.0/liquer/server/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
         keys = self.request.arguments.keys()
         kwargs.update({key: self.get_argument(key) for key in keys})
         try:
             b, mimetype, filename = response(evaluate(query, extra_parameters=kwargs))
         except:
             traceback.print_exc()
             self.set_status(500)
-            self.finish(f"500 - Failed to create a respone to {query}")
+            self.finish(f"500 - Failed to create a response to {query}")
+            return
 
         header = "Content-Type"
         body = mimetype if mimetype is not None else "application/octet-stream"
         self.set_header(header, body)
 
         self.write(b)
 
@@ -92,18 +93,30 @@
         self.get(query)
 
 
 # /api/cache/get/<path:query>
 class CacheGetDataHandler:
     def get(self, query):
         """Main service for evaluating queries"""
+        try:
+            kwargs = json.loads(self.request.body)
+        except:
+            kwargs = {}
+        keys = self.request.arguments.keys()
+        kwargs.update({key: self.get_argument(key) for key in keys})
+        if len(kwargs):
+            self.set_status(404)
+            self.finish(f"404 - {query} parameters not allowed")
+            return
+
         state = get_cache().get(query)
         if state is None:
             self.set_status(404)
             self.finish(f"404 - {query} not found in cache")
+            return
 
         b, mimetype, filename = response(state)
         header = "Content-Type"
         body = mimetype
         self.set_header(header, body)
 
         self.write(b)
@@ -281,15 +294,15 @@
     def post(self, param):
         self.write(
             json.dumps(command_registry().register_remote_serialized(self.request.body))
         )
 
 
 # /api/store/data/<path:query>
-class StoreDataHandler:
+class GetStoreDataHandler:
     def get(self, query):
         """Get data from store. Equivalent to Store.get_bytes.
         Content type (MIME) is obtained from the metadata.
         """
         store = get_store()
         metadata = store.get_metadata(query)
 
@@ -303,14 +316,16 @@
             )
 
         header = "Content-Type"
         body = mimetype
         self.set_header(header, body)
         self.write(b)
 
+# /api/store/data/<path:query>
+class StoreDataHandler(GetStoreDataHandler):
     def post(self, query):
         """Set data in store. Equivalent to Store.store.
         Unlike store method, which stores both data and metadata in one call,
         the api/store/data POST only stores the data. The metadata needs to be set in a separate POST of api/store/metadata
         either before or after the api/store/data POST.
         """
         store = get_store()
@@ -390,28 +405,29 @@
         header = "Content-Type"
         body = mimetype
         self.set_header(header, body)
         self.write(json.dumps(response))
 
 
 # /api/store/metadata/<path:query>
-class StoreMetadataHandler:
+class GetStoreMetadataHandler:
     def get(self, query):
         """Get data from store. Equivalent to Store.get_bytes.
         Content type (MIME) is obtained from the metadata.
         """
         store = get_store()
         metadata = store.get_metadata(query)
 
         mimetype = "application/json"
         header = "Content-Type"
         body = mimetype
         self.set_header(header, body)
         self.write(json.dumps(metadata))
 
+class StoreMetadataHandler(GetStoreMetadataHandler):
     def post(self, query):
         """Set data from store. Equivalent to Store.store.
         Unlike store method, which stores both data and metadata in one call,
         the api/store/data POST only stores the data. The metadata needs to be set in a separate POST of api/store/metadata
         either before or after the api/store/data POST.
         """
         store = get_store()
```

### Comparing `liquer-framework-0.8.0/liquer/server/static/index.html` & `liquer-framework-0.9.0/liquer/server/static/index.html`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/server/static/liquer.js` & `liquer-framework-0.9.0/liquer/server/static/liquer.js`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/server/tornado_handlers.py` & `liquer-framework-0.9.0/liquer/server/tornado_handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -85,27 +85,33 @@
 
 #'/api/register_command/
 class RegisterCommandHandler(h.RegisterCommandHandler, tornado.web.RequestHandler):
     pass
 
 
 # /api/store/data/<path:query>
-class StoreDataHandler(h.StoreDataHandler, tornado.web.RequestHandler):
+class GetStoreDataHandler(h.GetStoreDataHandler, tornado.web.RequestHandler):
     pass
 
+# /api/store/data/<path:query>
+class StoreDataHandler(h.StoreDataHandler, tornado.web.RequestHandler):
+    pass
 
 # /api/store/upload/<path:query>
 class StoreUploadHandler(h.StoreUploadHandler, tornado.web.RequestHandler):
     pass
 
 
 # /api/store/metadata/<path:query>
-class StoreMetadataHandler(h.StoreMetadataHandler, tornado.web.RequestHandler):
+class GetStoreMetadataHandler(h.GetStoreMetadataHandler, tornado.web.RequestHandler):
     pass
 
+# /api/store/metadata/<path:query>
+class StoreMetadataHandler(h.StoreMetadataHandler, tornado.web.RequestHandler):
+    pass
 
 # /web/<path:query>
 class WebStoreHandler(h.WebStoreHandler, tornado.web.RequestHandler):
     pass
 
 
 # /api/store/remove/<path:query>
@@ -154,15 +160,14 @@
         (r"/liquer/q/(.*)", QueryHandler),
         (r"/liquer/api/cache/get/(.*)", CacheGetDataHandler),
         (r"/liquer/api/cache/meta/(.*)", CacheMetadataHandler),
         (r"/liquer/api/cache/remove/(.*)", CacheRemoveHandler),
         (r"/liquer/api/cache/contains/(.*)", CacheContainsHandler),
         (r"/liquer/api/cache/keys.json", CacheKeysHandler),
         (r"/liquer/api/cache/clean", CacheCleanHandler),
-        (r"/liquer/api/commands.json", CommandsHandler),
         (r"/liquer/api/debug-json/(.*)", GetMetadataHandler),
         (r"/liquer/api/metadata/(.*)", GetMetadataHandler),
         (r"/liquer/api/stored_metadata/(.*)", GetStoredMetadataHandler),
         (r"/liquer/api/build", BuildHandler),
         (r"/liquer/api/register_command", RegisterCommandHandler),
         (r"/liquer/api/store/data/(.*)", StoreDataHandler),
         (r"/liquer/api/store/upload/(.*)", StoreUploadHandler),
@@ -173,14 +178,35 @@
         (r"/liquer/api/store/contains/(.*)", StoreContainsHandler),
         (r"/liquer/api/store/is_dir/(.*)", StoreIsDirHandler),
         (r"/liquer/api/store/keys", StoreKeysHandler),
         (r"/liquer/api/store/listdir/(.*)", StoreListdirHandler),
         (r"/liquer/api/store/makedir/(.*)", StoreMakedirHandler),
     ]
 
+def url_mapping_ro():
+    return [
+        (r"/liquer/api/commands.json", CommandsHandler),
+        (r"/liquer/api/cache/get/(.*)", CacheGetDataHandler),
+        (r"/liquer/api/cache/meta/(.*)", CacheMetadataHandler),
+        #(r"/liquer/api/cache/remove/(.*)", CacheRemoveHandler),
+        (r"/liquer/api/cache/contains/(.*)", CacheContainsHandler),
+        (r"/liquer/api/cache/keys.json", CacheKeysHandler),
+        (r"/liquer/q/(.*)", CacheGetDataHandler),
+        (r"/liquer/api/debug-json/(.*)", GetStoredMetadataHandler),
+        (r"/liquer/api/metadata/(.*)", GetStoredMetadataHandler),
+        (r"/liquer/api/stored_metadata/(.*)", GetStoredMetadataHandler),
+        (r"/liquer/api/store/data/(.*)", GetStoreDataHandler),
+        (r"/liquer/api/store/metadata/(.*)", GetStoreMetadataHandler),
+        (r"/liquer/web/(.*)", WebStoreHandler),
+        (r"/liquer/api/store/contains/(.*)", StoreContainsHandler),
+        (r"/liquer/api/store/is_dir/(.*)", StoreIsDirHandler),
+        (r"/liquer/api/store/keys", StoreKeysHandler),
+        (r"/liquer/api/store/listdir/(.*)", StoreListdirHandler),
+    ]
+
 
 if __name__ == "__main__":
     import liquer.ext.basic
     import liquer.ext.meta
     import liquer.ext.lq_pandas
 
     #    import liquer.ext.lq_hxl
```

### Comparing `liquer-framework-0.8.0/liquer/state.py` & `liquer-framework-0.9.0/liquer/state.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/state_types.py` & `liquer-framework-0.9.0/liquer/state_types.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/store.py` & `liquer-framework-0.9.0/liquer/store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/template.py` & `liquer-framework-0.9.0/liquer/template.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/tools.py` & `liquer-framework-0.9.0/liquer/tools.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/util.py` & `liquer-framework-0.9.0/liquer/util.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer/web.py` & `liquer-framework-0.9.0/liquer/web.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.8.0/liquer_framework.egg-info/PKG-INFO` & `liquer-framework-0.9.0/liquer_framework.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquer-framework
-Version: 0.8.0
+Version: 0.9.0
 Summary: LiQuer - Query in (URL) link
 Home-page: https://github.com/orest-d/liquer
 Author: Orest Dubay
 Author-email: orest3.dubay@gmail.com
 License: UNKNOWN
 Description: # LiQuer (Link Query) 
         
@@ -38,14 +38,20 @@
         
         ```
         pip install liquer-framework
         ```
         
         # News
         
+        ## Changes in v0.9
+        - Basic search-engine support - [whoosh](https://whoosh.readthedocs.io/en/latest/intro.html) based on indexer. Current implementation is indexing title and description from the metadata and allows to search interactively via a simple web-interface. See *examples/whoosh_example.py*.
+        - Relative path support in recipes (recipe queries can contain '.' and/or '..' as a reference to the current warking directory or parent directory). 
+        - Tornad-based server with restricted access only supporting reading, but not writing and execution. This can be either used directly or as a starting point for developing a customized secure server. See *examples/hello_server_tornado_ro.py*.
+        
+        
         ## Changes in v0.8
         - Early indexer support - customized updating of metadata, future integration into search engines
         - Specialized indexers allow to specify/customize *tools* that can be used for viewing and editing in GUI.
         - Added S3 store
         - Remote store allows to mount a remote LiQuer server as a store
         
         
@@ -91,22 +97,15 @@
         - 2022-01-03 - v0.7.0  - many enhancements - e.g. modular recipes, support for datafusion, pptx, pillow
         - 2022-01-04 - v0.7.1  - root path bugfix, sync store
         - 2022-01-05 - v0.7.2  - several small fixes, e.g. fixing missing log in recipe-created metadata
         - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
         - 2022-01-07 - v0.7.4  - more bugfixes
         - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
         - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
-        - 2022-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
+        - 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
+        - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
         
-        ### New features
-        - API documentation improved on multiple places
-        - EXTERNAL status
-        - Basic support for DataFusion, pptx-python, Pillow images
-        - Tornado driver updated
-        - Extensible recipes; parquet_sql recipe type
-        - Read-only store proxy
-        - v0.7 is accompanied with new GUI [liquer-gui v0.1.0](https://github.com/orest-d/liquer-gui)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `liquer-framework-0.8.0/liquer_framework.egg-info/SOURCES.txt` & `liquer-framework-0.9.0/liquer_framework.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 liquer/ext/lq_plotly.py
 liquer/ext/lq_polars.py
 liquer/ext/lq_pptx.py
 liquer/ext/lq_pygments.py
 liquer/ext/lq_python.py
 liquer/ext/lq_sklearn_regression.py
 liquer/ext/lq_sweetviz.py
+liquer/ext/lq_whoosh.py
 liquer/ext/meta.py
 liquer/server/__init__.py
 liquer/server/blueprint.py
 liquer/server/handlers.py
 liquer/server/tornado_handlers.py
 liquer/server/static/index.html
 liquer/server/static/liquer.js
```

### Comparing `liquer-framework-0.8.0/setup.py` & `liquer-framework-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="liquer-framework",
-    version="0.8.0",
+    version="0.9.0",
     author="Orest Dubay",
     author_email="orest3.dubay@gmail.com",
     description="LiQuer - Query in (URL) link",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/orest-d/liquer",
     packages=setuptools.find_packages(),
```

