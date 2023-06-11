# Comparing `tmp/deva-1.1.6.tar.gz` & `tmp/deva-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deva-1.1.6.tar", last modified: Mon Mar  6 14:14:30 2023, max compression
+gzip compressed data, was "deva-1.1.7.tar", last modified: Sun Jun 11 13:18:24 2023, max compression
```

## Comparing `deva-1.1.6.tar` & `deva-1.1.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.410391 deva-1.1.6/
--rw-r--r--   0 spark      (502) staff       (20)      109 2020-11-18 14:48:20.000000 deva-1.1.6/MANIFEST.in
--rw-r--r--   0 spark      (502) staff       (20)     5618 2023-03-06 14:14:30.409008 deva-1.1.6/PKG-INFO
--rw-r--r--   0 spark      (502) staff       (20)     5373 2022-12-30 19:45:37.000000 deva-1.1.6/README.rst
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.333544 deva-1.1.6/deva/
--rw-r--r--   0 spark      (502) staff       (20)      545 2023-03-06 14:13:30.000000 deva-1.1.6/deva/__init__.py
--rw-r--r--   0 spark      (502) staff       (20)     1261 2022-12-29 22:30:26.000000 deva-1.1.6/deva/bus.py
--rw-r--r--   0 spark      (502) staff       (20)    20881 2020-11-25 15:40:24.000000 deva-1.1.6/deva/compute.py
--rw-r--r--   0 spark      (502) staff       (20)    34102 2023-03-06 08:14:28.000000 deva-1.1.6/deva/core.py
--rw-r--r--   0 spark      (502) staff       (20)     5293 2020-08-31 16:42:35.000000 deva-1.1.6/deva/dask.py
--rw-r--r--   0 spark      (502) staff       (20)     7995 2023-01-19 09:58:36.000000 deva-1.1.6/deva/endpoints.py
--rw-r--r--   0 spark      (502) staff       (20)     2464 2020-12-27 12:45:41.000000 deva-1.1.6/deva/future.py
--rw-r--r--   0 spark      (502) staff       (20)     7412 2020-03-01 12:24:50.000000 deva-1.1.6/deva/graph.py
--rw-r--r--   0 spark      (502) staff       (20)     4526 2020-12-31 18:03:58.000000 deva-1.1.6/deva/lambdas.py
--rw-r--r--   0 spark      (502) staff       (20)     7727 2023-01-27 04:17:29.000000 deva-1.1.6/deva/monitor.py
--rw-r--r--   0 spark      (502) staff       (20)     2896 2023-01-20 18:19:59.000000 deva-1.1.6/deva/namespace.py
--rw-r--r--   0 spark      (502) staff       (20)    21454 2023-01-27 04:10:23.000000 deva-1.1.6/deva/page.py
--rw-r--r--   0 spark      (502) staff       (20)    22260 2023-03-06 14:12:44.000000 deva-1.1.6/deva/pipe.py
--rw-r--r--   0 spark      (502) staff       (20)     1760 2022-01-08 14:58:21.000000 deva-1.1.6/deva/river.py
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.351641 deva-1.1.6/deva/sample/
--rw-r--r--   0 spark      (502) staff       (20)     8196 2020-03-19 16:07:17.000000 deva-1.1.6/deva/sample/.DS_Store
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.355312 deva-1.1.6/deva/sample/bus/
--rw-r--r--   0 spark      (502) staff       (20)      130 2020-03-14 10:10:54.000000 deva-1.1.6/deva/sample/bus/bus_in.py
--rw-r--r--   0 spark      (502) staff       (20)      199 2020-04-02 04:53:57.000000 deva-1.1.6/deva/sample/bus/bus_out.py
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.359355 deva-1.1.6/deva/sample/crawler/
--rw-r--r--   0 spark      (502) staff       (20)     6148 2020-03-19 16:05:00.000000 deva-1.1.6/deva/sample/crawler/.DS_Store
--rw-r--r--   0 spark      (502) staff       (20)      287 2020-03-17 03:48:26.000000 deva-1.1.6/deva/sample/crawler/asynchttp.py
--rw-r--r--   0 spark      (502) staff       (20)     1100 2020-03-18 10:45:44.000000 deva-1.1.6/deva/sample/matmul.py
--rw-r--r--   0 spark      (502) staff       (20)      539 2020-12-27 12:43:34.000000 deva-1.1.6/deva/sample/my_future.py
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.364924 deva-1.1.6/deva/sample/search/
--rw-r--r--   0 spark      (502) staff       (20)     6148 2020-04-20 04:25:11.000000 deva-1.1.6/deva/sample/search/.DS_Store
--rw-r--r--   0 spark      (502) staff       (20)     1191 2020-04-20 04:32:54.000000 deva-1.1.6/deva/sample/search/search_sql.py
--rw-r--r--   0 spark      (502) staff       (20)      765 2020-04-20 04:26:31.000000 deva-1.1.6/deva/sample/search/search_stream.py
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.366692 deva-1.1.6/deva/sample/webview/
--rw-r--r--   0 spark      (502) staff       (20)      695 2020-11-13 18:26:16.000000 deva-1.1.6/deva/sample/webview/stream_page.py
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.373724 deva-1.1.6/deva/sample/when/
--rw-r--r--   0 spark      (502) staff       (20)     1555 2020-03-14 10:08:21.000000 deva-1.1.6/deva/sample/when/scheduler.py
--rw-r--r--   0 spark      (502) staff       (20)      707 2020-03-14 10:31:52.000000 deva-1.1.6/deva/sample/when/timer.py
--rw-r--r--   0 spark      (502) staff       (20)      444 2020-11-29 11:36:11.000000 deva-1.1.6/deva/sample/when/worker.py
--rw-r--r--   0 spark      (502) staff       (20)     3684 2021-06-13 17:15:18.000000 deva-1.1.6/deva/search.py
--rw-r--r--   0 spark      (502) staff       (20)    26908 2023-03-06 14:10:32.000000 deva-1.1.6/deva/sources.py
--rw-r--r--   0 spark      (502) staff       (20)      933 2020-11-29 06:29:06.000000 deva-1.1.6/deva/state.py
--rw-r--r--   0 spark      (502) staff       (20)     5929 2023-02-08 20:49:07.000000 deva-1.1.6/deva/store.py
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.385665 deva-1.1.6/deva/templates/
--rw-r--r--   0 spark      (502) staff       (20)     3011 2022-12-30 22:00:17.000000 deva-1.1.6/deva/templates/monitor.html
--rw-r--r--   0 spark      (502) staff       (20)     1270 2021-07-07 10:25:38.000000 deva-1.1.6/deva/templates/stream.html
--rw-r--r--   0 spark      (502) staff       (20)     1382 2020-11-13 18:40:42.000000 deva-1.1.6/deva/templates/streams.html
--rw-r--r--   0 spark      (502) staff       (20)     4618 2022-12-30 19:31:41.000000 deva-1.1.6/deva/templates/xterm.css
--rw-r--r--   0 spark      (502) staff       (20)   275838 2022-12-30 19:31:41.000000 deva-1.1.6/deva/templates/xterm.js
--rw-r--r--   0 spark      (502) staff       (20)     2664 2023-01-02 11:49:35.000000 deva-1.1.6/deva/topic.py
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.395996 deva-1.1.6/deva/utils/
--rw-r--r--   0 spark      (502) staff       (20)        0 2020-04-09 08:17:47.000000 deva-1.1.6/deva/utils/__init__.py
--rw-r--r--   0 spark      (502) staff       (20)     6131 2019-12-29 10:29:14.000000 deva-1.1.6/deva/utils/simhash.py
--rw-r--r--   0 spark      (502) staff       (20)    21367 2020-11-11 17:12:06.000000 deva-1.1.6/deva/utils/sqlitedict.py
--rw-r--r--   0 spark      (502) staff       (20)     6910 2020-03-13 08:06:52.000000 deva-1.1.6/deva/utils/whooshalchemy.py
--rw-r--r--   0 spark      (502) staff       (20)     5643 2023-02-26 08:43:17.000000 deva-1.1.6/deva/when.py
-drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-03-06 14:14:30.346537 deva-1.1.6/deva.egg-info/
--rw-r--r--   0 spark      (502) staff       (20)     5618 2023-03-06 14:14:29.000000 deva-1.1.6/deva.egg-info/PKG-INFO
--rw-r--r--   0 spark      (502) staff       (20)     1122 2023-03-06 14:14:30.000000 deva-1.1.6/deva.egg-info/SOURCES.txt
--rw-r--r--   0 spark      (502) staff       (20)        1 2023-03-06 14:14:29.000000 deva-1.1.6/deva.egg-info/dependency_links.txt
--rw-r--r--   0 spark      (502) staff       (20)        1 2020-11-14 15:34:05.000000 deva-1.1.6/deva.egg-info/not-zip-safe
--rw-r--r--   0 spark      (502) staff       (20)      233 2023-03-06 14:14:29.000000 deva-1.1.6/deva.egg-info/requires.txt
--rw-r--r--   0 spark      (502) staff       (20)        5 2023-03-06 14:14:29.000000 deva-1.1.6/deva.egg-info/top_level.txt
--rw-r--r--   0 spark      (502) staff       (20)       38 2023-03-06 14:14:30.410666 deva-1.1.6/setup.cfg
--rw-r--r--   0 spark      (502) staff       (20)      614 2023-03-06 14:13:46.000000 deva-1.1.6/setup.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.954566 deva-1.1.7/
+-rw-r--r--   0 spark      (502) staff       (20)      109 2020-11-18 14:48:20.000000 deva-1.1.7/MANIFEST.in
+-rw-r--r--   0 spark      (502) staff       (20)     5618 2023-06-11 13:18:24.953820 deva-1.1.7/PKG-INFO
+-rw-r--r--   0 spark      (502) staff       (20)     5373 2022-12-30 19:45:37.000000 deva-1.1.7/README.rst
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.913279 deva-1.1.7/deva/
+-rw-r--r--   0 spark      (502) staff       (20)      545 2023-06-11 13:17:11.000000 deva-1.1.7/deva/__init__.py
+-rw-r--r--   0 spark      (502) staff       (20)     1261 2022-12-29 22:30:26.000000 deva-1.1.7/deva/bus.py
+-rw-r--r--   0 spark      (502) staff       (20)    20881 2020-11-25 15:40:24.000000 deva-1.1.7/deva/compute.py
+-rw-r--r--   0 spark      (502) staff       (20)    34102 2023-03-06 08:14:28.000000 deva-1.1.7/deva/core.py
+-rw-r--r--   0 spark      (502) staff       (20)     5293 2020-08-31 16:42:35.000000 deva-1.1.7/deva/dask.py
+-rw-r--r--   0 spark      (502) staff       (20)     7995 2023-01-19 09:58:36.000000 deva-1.1.7/deva/endpoints.py
+-rw-r--r--   0 spark      (502) staff       (20)     2464 2020-12-27 12:45:41.000000 deva-1.1.7/deva/future.py
+-rw-r--r--   0 spark      (502) staff       (20)     7412 2020-03-01 12:24:50.000000 deva-1.1.7/deva/graph.py
+-rw-r--r--   0 spark      (502) staff       (20)     4526 2020-12-31 18:03:58.000000 deva-1.1.7/deva/lambdas.py
+-rw-r--r--   0 spark      (502) staff       (20)     7727 2023-01-27 04:17:29.000000 deva-1.1.7/deva/monitor.py
+-rw-r--r--   0 spark      (502) staff       (20)     2906 2023-04-25 18:40:43.000000 deva-1.1.7/deva/namespace.py
+-rw-r--r--   0 spark      (502) staff       (20)    21454 2023-01-27 04:10:23.000000 deva-1.1.7/deva/page.py
+-rw-r--r--   0 spark      (502) staff       (20)    22288 2023-04-12 11:59:28.000000 deva-1.1.7/deva/pipe.py
+-rw-r--r--   0 spark      (502) staff       (20)     1760 2022-01-08 14:58:21.000000 deva-1.1.7/deva/river.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.923146 deva-1.1.7/deva/sample/
+-rw-r--r--   0 spark      (502) staff       (20)     8196 2020-03-19 16:07:17.000000 deva-1.1.7/deva/sample/.DS_Store
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.925632 deva-1.1.7/deva/sample/bus/
+-rw-r--r--   0 spark      (502) staff       (20)      130 2020-03-14 10:10:54.000000 deva-1.1.7/deva/sample/bus/bus_in.py
+-rw-r--r--   0 spark      (502) staff       (20)      199 2020-04-02 04:53:57.000000 deva-1.1.7/deva/sample/bus/bus_out.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.928047 deva-1.1.7/deva/sample/crawler/
+-rw-r--r--   0 spark      (502) staff       (20)     6148 2020-03-19 16:05:00.000000 deva-1.1.7/deva/sample/crawler/.DS_Store
+-rw-r--r--   0 spark      (502) staff       (20)      287 2020-03-17 03:48:26.000000 deva-1.1.7/deva/sample/crawler/asynchttp.py
+-rw-r--r--   0 spark      (502) staff       (20)     1100 2020-03-18 10:45:44.000000 deva-1.1.7/deva/sample/matmul.py
+-rw-r--r--   0 spark      (502) staff       (20)      539 2020-12-27 12:43:34.000000 deva-1.1.7/deva/sample/my_future.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.932624 deva-1.1.7/deva/sample/search/
+-rw-r--r--   0 spark      (502) staff       (20)     6148 2020-04-20 04:25:11.000000 deva-1.1.7/deva/sample/search/.DS_Store
+-rw-r--r--   0 spark      (502) staff       (20)     1191 2020-04-20 04:32:54.000000 deva-1.1.7/deva/sample/search/search_sql.py
+-rw-r--r--   0 spark      (502) staff       (20)      765 2020-04-20 04:26:31.000000 deva-1.1.7/deva/sample/search/search_stream.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.933852 deva-1.1.7/deva/sample/webview/
+-rw-r--r--   0 spark      (502) staff       (20)      695 2020-11-13 18:26:16.000000 deva-1.1.7/deva/sample/webview/stream_page.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.937716 deva-1.1.7/deva/sample/when/
+-rw-r--r--   0 spark      (502) staff       (20)     1555 2020-03-14 10:08:21.000000 deva-1.1.7/deva/sample/when/scheduler.py
+-rw-r--r--   0 spark      (502) staff       (20)      707 2020-03-14 10:31:52.000000 deva-1.1.7/deva/sample/when/timer.py
+-rw-r--r--   0 spark      (502) staff       (20)      444 2020-11-29 11:36:11.000000 deva-1.1.7/deva/sample/when/worker.py
+-rw-r--r--   0 spark      (502) staff       (20)     3684 2023-06-11 13:17:00.000000 deva-1.1.7/deva/search.py
+-rw-r--r--   0 spark      (502) staff       (20)    27067 2023-03-14 08:03:47.000000 deva-1.1.7/deva/sources.py
+-rw-r--r--   0 spark      (502) staff       (20)      933 2020-11-29 06:29:06.000000 deva-1.1.7/deva/state.py
+-rw-r--r--   0 spark      (502) staff       (20)     5929 2023-02-08 20:49:07.000000 deva-1.1.7/deva/store.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.943956 deva-1.1.7/deva/templates/
+-rw-r--r--   0 spark      (502) staff       (20)     3011 2022-12-30 22:00:17.000000 deva-1.1.7/deva/templates/monitor.html
+-rw-r--r--   0 spark      (502) staff       (20)     1270 2021-07-07 10:25:38.000000 deva-1.1.7/deva/templates/stream.html
+-rw-r--r--   0 spark      (502) staff       (20)     1382 2020-11-13 18:40:42.000000 deva-1.1.7/deva/templates/streams.html
+-rw-r--r--   0 spark      (502) staff       (20)     4618 2022-12-30 19:31:41.000000 deva-1.1.7/deva/templates/xterm.css
+-rw-r--r--   0 spark      (502) staff       (20)   275838 2022-12-30 19:31:41.000000 deva-1.1.7/deva/templates/xterm.js
+-rw-r--r--   0 spark      (502) staff       (20)     2664 2023-01-02 11:49:35.000000 deva-1.1.7/deva/topic.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.952445 deva-1.1.7/deva/utils/
+-rw-r--r--   0 spark      (502) staff       (20)        0 2020-04-09 08:17:47.000000 deva-1.1.7/deva/utils/__init__.py
+-rw-r--r--   0 spark      (502) staff       (20)     6131 2019-12-29 10:29:14.000000 deva-1.1.7/deva/utils/simhash.py
+-rw-r--r--   0 spark      (502) staff       (20)    21367 2020-11-11 17:12:06.000000 deva-1.1.7/deva/utils/sqlitedict.py
+-rw-r--r--   0 spark      (502) staff       (20)     6910 2020-03-13 08:06:52.000000 deva-1.1.7/deva/utils/whooshalchemy.py
+-rw-r--r--   0 spark      (502) staff       (20)     5643 2023-02-26 08:43:17.000000 deva-1.1.7/deva/when.py
+drwxr-xr-x   0 spark      (502) staff       (20)        0 2023-06-11 13:18:24.920063 deva-1.1.7/deva.egg-info/
+-rw-r--r--   0 spark      (502) staff       (20)     5618 2023-06-11 13:18:24.000000 deva-1.1.7/deva.egg-info/PKG-INFO
+-rw-r--r--   0 spark      (502) staff       (20)     1122 2023-06-11 13:18:24.000000 deva-1.1.7/deva.egg-info/SOURCES.txt
+-rw-r--r--   0 spark      (502) staff       (20)        1 2023-06-11 13:18:24.000000 deva-1.1.7/deva.egg-info/dependency_links.txt
+-rw-r--r--   0 spark      (502) staff       (20)        1 2020-11-14 15:34:05.000000 deva-1.1.7/deva.egg-info/not-zip-safe
+-rw-r--r--   0 spark      (502) staff       (20)      233 2023-06-11 13:18:24.000000 deva-1.1.7/deva.egg-info/requires.txt
+-rw-r--r--   0 spark      (502) staff       (20)        5 2023-06-11 13:18:24.000000 deva-1.1.7/deva.egg-info/top_level.txt
+-rw-r--r--   0 spark      (502) staff       (20)       38 2023-06-11 13:18:24.954834 deva-1.1.7/setup.cfg
+-rw-r--r--   0 spark      (502) staff       (20)      614 2023-06-11 13:17:28.000000 deva-1.1.7/setup.py
```

### Comparing `deva-1.1.6/PKG-INFO` & `deva-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deva
-Version: 1.1.6
+Version: 1.1.7
 Summary: data eval in future
 Home-page: https://github.com/sostc/deva
 Author: spark
 Author-email: zjw0358@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0.html
 Requires-Python: >=3.5
```

### Comparing `deva-1.1.6/README.rst` & `deva-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/__init__.py` & `deva-1.1.7/deva/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 try:
     # import panel as pn
     from .dask import DaskStream, scatter
 
 except ImportError:
     pass
 
-__version__ = '1.1.6'
+__version__ = '1.1.7'
```

### Comparing `deva-1.1.6/deva/bus.py` & `deva-1.1.7/deva/bus.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/compute.py` & `deva-1.1.7/deva/compute.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/core.py` & `deva-1.1.7/deva/core.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/dask.py` & `deva-1.1.7/deva/dask.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/endpoints.py` & `deva-1.1.7/deva/endpoints.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/future.py` & `deva-1.1.7/deva/future.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/graph.py` & `deva-1.1.7/deva/graph.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/lambdas.py` & `deva-1.1.7/deva/lambdas.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/monitor.py` & `deva-1.1.7/deva/monitor.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/namespace.py` & `deva-1.1.7/deva/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         assert NX('b').data ==10
 
 
     """
     return namespace.create(typ='data', name=name)
 
 
-def NW(name='', host='127.0.0.1', port=9999, start=True):
+def NW(name='', host='127.0.0.1', port=9999, start=True, **kwargs):
     """创建命名web服务器.
 
     返回的对象，data属性存储了数据，用在你们函数内部以及函数管道上快速存储单个数据
 
     Example usage::
 
          pass
```

### Comparing `deva-1.1.6/deva/page.py` & `deva-1.1.7/deva/page.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/pipe.py` & `deva-1.1.7/deva/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,14 +659,15 @@
         {'a':1}>>post_to(url)
         {'a':1}>>post_to(url,asynchronous=False)
 
     """
     headers.update({'tag': quote(tag)})
 
     def _encode(body):
+        import pandas as pd
         if isinstance(body, pd.DataFrame):
             body = body.to_json()
         else:
             body = dill.dumps(body)
         return body
 
     @gen.coroutine
```

### Comparing `deva-1.1.6/deva/river.py` & `deva-1.1.7/deva/river.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/.DS_Store` & `deva-1.1.7/deva/sample/.DS_Store`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/crawler/.DS_Store` & `deva-1.1.7/deva/sample/crawler/.DS_Store`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/matmul.py` & `deva-1.1.7/deva/sample/matmul.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/my_future.py` & `deva-1.1.7/deva/sample/my_future.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/search/.DS_Store` & `deva-1.1.7/deva/sample/search/.DS_Store`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/search/search_sql.py` & `deva-1.1.7/deva/sample/search/search_sql.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/search/search_stream.py` & `deva-1.1.7/deva/sample/search/search_stream.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/webview/stream_page.py` & `deva-1.1.7/deva/sample/webview/stream_page.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/when/scheduler.py` & `deva-1.1.7/deva/sample/when/scheduler.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sample/when/timer.py` & `deva-1.1.7/deva/sample/when/timer.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/search.py` & `deva-1.1.7/deva/search.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/sources.py` & `deva-1.1.7/deva/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -791,15 +791,15 @@
                 finally:
                     return body
 
             def _encode(self, body):
                 if isinstance(body, pd.DataFrame):
                     return body.sample(20).to_html()
                 else:
-                    return json.dumps(body)
+                    return json.dumps(body, ensure_ascii=False)
 
             @gen.coroutine
             def post(self):
                 body = dill.loads(self.request.body)
                 body = [self._loads(i) for i in body]
                 if not isinstance(body, list):
                     body = [body]
@@ -818,15 +818,18 @@
 
             @gen.coroutine
             def get(self):
                 topic = unquote(self.request.path)
                 if topic == '/':
                     data = self.source.recent()
                 else:
-                    data = NS(topic.split('/')[1]).recent()
+                    stream = NS(topic.split('/')[1])
+                    if not stream.is_cache:
+                        stream.start_cache(10, 64*64*24*7)
+                    data = stream.recent()
                 if 'deva' in self.request.headers['User-Agent']:
                     self.write(dill.dumps(data))
                 else:
                     for i in data:
                         self.write(self._encode(i)+'</br>')
 
         self.application = Application([
```

### Comparing `deva-1.1.6/deva/state.py` & `deva-1.1.7/deva/state.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/store.py` & `deva-1.1.7/deva/store.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/templates/monitor.html` & `deva-1.1.7/deva/templates/monitor.html`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/templates/stream.html` & `deva-1.1.7/deva/templates/stream.html`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/templates/streams.html` & `deva-1.1.7/deva/templates/streams.html`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/templates/xterm.css` & `deva-1.1.7/deva/templates/xterm.css`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/templates/xterm.js` & `deva-1.1.7/deva/templates/xterm.js`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/topic.py` & `deva-1.1.7/deva/topic.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/utils/simhash.py` & `deva-1.1.7/deva/utils/simhash.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/utils/sqlitedict.py` & `deva-1.1.7/deva/utils/sqlitedict.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/utils/whooshalchemy.py` & `deva-1.1.7/deva/utils/whooshalchemy.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva/when.py` & `deva-1.1.7/deva/when.py`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/deva.egg-info/PKG-INFO` & `deva-1.1.7/deva.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deva
-Version: 1.1.6
+Version: 1.1.7
 Summary: data eval in future
 Home-page: https://github.com/sostc/deva
 Author: spark
 Author-email: zjw0358@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0.html
 Requires-Python: >=3.5
```

### Comparing `deva-1.1.6/deva.egg-info/SOURCES.txt` & `deva-1.1.7/deva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deva-1.1.6/setup.py` & `deva-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os.path import exists
 
 setup(
     name='deva',
-    version='1.1.6',
+    version='1.1.7',
     include_package_data=True,
     packages=find_packages(),
     python_requires='>=3.5',
     author='spark',
     author_email='zjw0358@gmail.com',
     url='https://github.com/sostc/deva',
     license='http://www.apache.org/licenses/LICENSE-2.0.html',
```

