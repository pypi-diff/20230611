# Comparing `tmp/ttun-2.0.0.tar.gz` & `tmp/ttun-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttun-2.0.0.tar", last modified: Sun Jun 11 11:35:05 2023, max compression
+gzip compressed data, was "ttun-2.0.1.tar", last modified: Sun Jun 11 12:01:22 2023, max compression
```

## Comparing `ttun-2.0.0.tar` & `ttun-2.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.063001 ttun-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-11 11:34:22.000000 ttun-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-11 11:34:22.000000 ttun-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-11 11:35:05.063001 ttun-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-11 11:34:22.000000 ttun-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-11 11:34:22.000000 ttun-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-11 11:35:05.063001 ttun-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.059002 ttun-2.0.0/ttun/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/inspect_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.059002 ttun-2.0.0/ttun/staticfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.063001 ttun-2.0.0/ttun/staticfiles/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   352540 2023-06-11 11:34:56.000000 ttun-2.0.0/ttun/staticfiles/assets/index.120f66e1.js
--rw-r--r--   0 runner    (1001) docker     (123)   324123 2023-06-11 11:34:56.000000 ttun-2.0.0/ttun/staticfiles/assets/index.cc7cded7.css
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 11:34:56.000000 ttun-2.0.0/ttun/staticfiles/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.059002 ttun-2.0.0/ttun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:01:22.059974 ttun-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-11 12:00:38.000000 ttun-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-11 12:00:38.000000 ttun-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-11 12:01:22.059974 ttun-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-11 12:00:38.000000 ttun-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-11 12:00:38.000000 ttun-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-11 12:01:22.063974 ttun-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:01:22.055974 ttun-2.0.1/ttun/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-11 12:00:38.000000 ttun-2.0.1/ttun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-11 12:00:38.000000 ttun-2.0.1/ttun/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-11 12:00:38.000000 ttun-2.0.1/ttun/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-11 12:00:38.000000 ttun-2.0.1/ttun/inspect_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-11 12:00:38.000000 ttun-2.0.1/ttun/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-11 12:00:38.000000 ttun-2.0.1/ttun/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:01:22.055974 ttun-2.0.1/ttun/staticfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:01:22.059974 ttun-2.0.1/ttun/staticfiles/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   352540 2023-06-11 12:01:12.000000 ttun-2.0.1/ttun/staticfiles/assets/index.120f66e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   324123 2023-06-11 12:01:12.000000 ttun-2.0.1/ttun/staticfiles/assets/index.cc7cded7.css
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 12:01:12.000000 ttun-2.0.1/ttun/staticfiles/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-11 12:00:38.000000 ttun-2.0.1/ttun/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:01:22.055974 ttun-2.0.1/ttun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-11 12:01:22.000000 ttun-2.0.1/ttun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-11 12:01:22.000000 ttun-2.0.1/ttun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:01:22.000000 ttun-2.0.1/ttun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-11 12:01:22.000000 ttun-2.0.1/ttun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-11 12:01:22.000000 ttun-2.0.1/ttun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 12:01:22.000000 ttun-2.0.1/ttun.egg-info/top_level.txt
```

### Comparing `ttun-2.0.0/LICENSE` & `ttun-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/PKG-INFO` & `ttun-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttun
-Version: 2.0.0
+Version: 2.0.1
 Summary: Expose a local port via your selfhosted TTUN Server
 Author: Tom van der Lee
 License: BSD-3-Clause
 License-File: LICENSE
 
 ===========
 TTUN Client
```

### Comparing `ttun-2.0.0/README.rst` & `ttun-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun/__main__.py` & `ttun-2.0.1/ttun/__main__.py`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun/client.py` & `ttun-2.0.1/ttun/client.py`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun/inspect_server.py` & `ttun-2.0.1/ttun/inspect_server.py`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun/pubsub.py` & `ttun-2.0.1/ttun/pubsub.py`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun/settings.py` & `ttun-2.0.1/ttun/settings.py`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun/staticfiles/assets/index.120f66e1.js` & `ttun-2.0.1/ttun/staticfiles/assets/index.120f66e1.js`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun/staticfiles/assets/index.cc7cded7.css` & `ttun-2.0.1/ttun/staticfiles/assets/index.cc7cded7.css`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun/types.py` & `ttun-2.0.1/ttun/types.py`

 * *Files identical despite different names*

### Comparing `ttun-2.0.0/ttun.egg-info/PKG-INFO` & `ttun-2.0.1/ttun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttun
-Version: 2.0.0
+Version: 2.0.1
 Summary: Expose a local port via your selfhosted TTUN Server
 Author: Tom van der Lee
 License: BSD-3-Clause
 License-File: LICENSE
 
 ===========
 TTUN Client
```

