# Comparing `tmp/consumer_base-0.0.2.tar.gz` & `tmp/consumer_base-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consumer_base-0.0.2.tar", last modified: Sun Jun 11 04:56:09 2023, max compression
+gzip compressed data, was "consumer_base-0.1.1.tar", last modified: Sun Jun 11 04:58:09 2023, max compression
```

## Comparing `consumer_base-0.0.2.tar` & `consumer_base-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 brunofioreze  (1000) brunofioreze  (1000)        0 2023-06-11 04:56:09.731890 consumer_base-0.0.2/
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)     1083 2023-06-11 04:36:20.000000 consumer_base-0.0.2/LICENCE
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      390 2023-06-11 04:56:09.731890 consumer_base-0.0.2/PKG-INFO
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)       89 2023-06-11 03:05:25.000000 consumer_base-0.0.2/README.md
-drwxrwxr-x   0 brunofioreze  (1000) brunofioreze  (1000)        0 2023-06-11 04:56:09.731890 consumer_base-0.0.2/consumer_base/
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)        0 2023-06-11 03:05:25.000000 consumer_base-0.0.2/consumer_base/__init__.py
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)     1430 2023-06-11 03:05:25.000000 consumer_base-0.0.2/consumer_base/__main__.py
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)    16445 2023-06-11 03:05:25.000000 consumer_base-0.0.2/consumer_base/base.py
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      264 2023-06-11 03:05:25.000000 consumer_base-0.0.2/consumer_base/config.py
-drwxrwxr-x   0 brunofioreze  (1000) brunofioreze  (1000)        0 2023-06-11 04:56:09.731890 consumer_base-0.0.2/consumer_base.egg-info/
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      390 2023-06-11 04:56:09.000000 consumer_base-0.0.2/consumer_base.egg-info/PKG-INFO
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      323 2023-06-11 04:56:09.000000 consumer_base-0.0.2/consumer_base.egg-info/SOURCES.txt
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)        1 2023-06-11 04:56:09.000000 consumer_base-0.0.2/consumer_base.egg-info/dependency_links.txt
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)       21 2023-06-11 04:56:09.000000 consumer_base-0.0.2/consumer_base.egg-info/requires.txt
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)       14 2023-06-11 04:56:09.000000 consumer_base-0.0.2/consumer_base.egg-info/top_level.txt
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      402 2023-06-11 04:53:15.000000 consumer_base-0.0.2/pyproject.toml
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)       38 2023-06-11 04:56:09.731890 consumer_base-0.0.2/setup.cfg
--rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      476 2023-06-11 04:56:03.000000 consumer_base-0.0.2/setup.py
+drwxrwxr-x   0 brunofioreze  (1000) brunofioreze  (1000)        0 2023-06-11 04:58:09.891674 consumer_base-0.1.1/
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)     1083 2023-06-11 04:36:20.000000 consumer_base-0.1.1/LICENCE
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      390 2023-06-11 04:58:09.891674 consumer_base-0.1.1/PKG-INFO
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)       89 2023-06-11 03:05:25.000000 consumer_base-0.1.1/README.md
+drwxrwxr-x   0 brunofioreze  (1000) brunofioreze  (1000)        0 2023-06-11 04:58:09.891674 consumer_base-0.1.1/consumer_base/
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)        0 2023-06-11 03:05:25.000000 consumer_base-0.1.1/consumer_base/__init__.py
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)     1430 2023-06-11 03:05:25.000000 consumer_base-0.1.1/consumer_base/__main__.py
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)    16445 2023-06-11 03:05:25.000000 consumer_base-0.1.1/consumer_base/base.py
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      264 2023-06-11 03:05:25.000000 consumer_base-0.1.1/consumer_base/config.py
+drwxrwxr-x   0 brunofioreze  (1000) brunofioreze  (1000)        0 2023-06-11 04:58:09.891674 consumer_base-0.1.1/consumer_base.egg-info/
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      390 2023-06-11 04:58:09.000000 consumer_base-0.1.1/consumer_base.egg-info/PKG-INFO
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      323 2023-06-11 04:58:09.000000 consumer_base-0.1.1/consumer_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)        1 2023-06-11 04:58:09.000000 consumer_base-0.1.1/consumer_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)       21 2023-06-11 04:58:09.000000 consumer_base-0.1.1/consumer_base.egg-info/requires.txt
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)       14 2023-06-11 04:58:09.000000 consumer_base-0.1.1/consumer_base.egg-info/top_level.txt
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      402 2023-06-11 04:57:19.000000 consumer_base-0.1.1/pyproject.toml
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)       38 2023-06-11 04:58:09.891674 consumer_base-0.1.1/setup.cfg
+-rw-rw-r--   0 brunofioreze  (1000) brunofioreze  (1000)      477 2023-06-11 04:57:57.000000 consumer_base-0.1.1/setup.py
```

### Comparing `consumer_base-0.0.2/LICENCE` & `consumer_base-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `consumer_base-0.0.2/consumer_base/__main__.py` & `consumer_base-0.1.1/consumer_base/__main__.py`

 * *Files identical despite different names*

### Comparing `consumer_base-0.0.2/consumer_base/base.py` & `consumer_base-0.1.1/consumer_base/base.py`

 * *Files identical despite different names*

