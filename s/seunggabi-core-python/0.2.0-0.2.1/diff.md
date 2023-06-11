# Comparing `tmp/seunggabi_core_python-0.2.0.tar.gz` & `tmp/seunggabi_core_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seunggabi_core_python-0.2.0.tar", last modified: Thu May 18 14:05:14 2023, max compression
+gzip compressed data, was "seunggabi_core_python-0.2.1.tar", last modified: Sun Jun 11 16:46:41 2023, max compression
```

## Comparing `seunggabi_core_python-0.2.0.tar` & `seunggabi_core_python-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.066094 seunggabi_core_python-0.2.0/
--rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.2.0/LICENSE
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-18 14:05:14.065955 seunggabi_core_python-0.2.0/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      362 2023-05-18 14:04:41.000000 seunggabi_core_python-0.2.0/README.md
--rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-05-18 14:05:14.066124 seunggabi_core_python-0.2.0/setup.cfg
--rw-r--r--   0 seunggabi   (501) staff       (20)      746 2023-05-15 13:20:26.000000 seunggabi_core_python-0.2.0/setup.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.064212 seunggabi_core_python-0.2.0/seunggabi_core_python/
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-18 14:05:01.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/const.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.065029 seunggabi_core_python-0.2.0/seunggabi_core_python/exception/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/exception/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       95 2023-05-15 12:54:12.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/exception/bad_request.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.065738 seunggabi_core_python-0.2.0/seunggabi_core_python/util/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-17 20:21:40.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/arg_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      781 2023-05-15 15:07:17.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/config_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      149 2023-05-15 15:07:03.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/json_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      193 2023-05-18 13:38:22.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/request_util.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.064698 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-18 14:05:14.000000 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      565 2023-05-18 14:05:14.000000 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/SOURCES.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-05-18 14:05:14.000000 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/dependency_links.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-18 14:05:14.000000 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/top_level.txt
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 16:46:41.238161 seunggabi_core_python-0.2.1/
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.2.1/LICENSE
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-06-11 16:46:41.238056 seunggabi_core_python-0.2.1/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      362 2023-06-11 16:46:36.000000 seunggabi_core_python-0.2.1/README.md
+-rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-06-11 16:46:41.238189 seunggabi_core_python-0.2.1/setup.cfg
+-rw-r--r--   0 seunggabi   (501) staff       (20)      746 2023-05-15 13:20:26.000000 seunggabi_core_python-0.2.1/setup.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 16:46:41.235800 seunggabi_core_python-0.2.1/seunggabi_core_python/
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-06-11 16:46:37.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/const.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 16:46:41.236880 seunggabi_core_python-0.2.1/seunggabi_core_python/exception/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/exception/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       97 2023-06-11 16:43:34.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/exception/bad_request.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       93 2023-06-11 16:43:28.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/exception/not_found.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 16:46:41.237785 seunggabi_core_python-0.2.1/seunggabi_core_python/util/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/util/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-18 14:08:20.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/util/arg_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      894 2023-06-11 16:44:44.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/util/config_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      149 2023-05-15 15:07:03.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/util/json_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      193 2023-05-18 14:08:20.000000 seunggabi_core_python-0.2.1/seunggabi_core_python/util/request_util.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-06-11 16:46:41.236557 seunggabi_core_python-0.2.1/seunggabi_core_python.egg-info/
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-06-11 16:46:41.000000 seunggabi_core_python-0.2.1/seunggabi_core_python.egg-info/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      610 2023-06-11 16:46:41.000000 seunggabi_core_python-0.2.1/seunggabi_core_python.egg-info/SOURCES.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-06-11 16:46:41.000000 seunggabi_core_python-0.2.1/seunggabi_core_python.egg-info/dependency_links.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-06-11 16:46:41.000000 seunggabi_core_python-0.2.1/seunggabi_core_python.egg-info/top_level.txt
```

### Comparing `seunggabi_core_python-0.2.0/LICENSE` & `seunggabi_core_python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.2.0/PKG-INFO` & `seunggabi_core_python-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seunggabi_core_python
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.2.0/setup.py` & `seunggabi_core_python-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.2.0/seunggabi_core_python/util/arg_util.py` & `seunggabi_core_python-0.2.1/seunggabi_core_python/util/arg_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/PKG-INFO` & `seunggabi_core_python-0.2.1/seunggabi_core_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seunggabi-core-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/SOURCES.txt` & `seunggabi_core_python-0.2.1/seunggabi_core_python.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 seunggabi_core_python/const.py
 seunggabi_core_python.egg-info/PKG-INFO
 seunggabi_core_python.egg-info/SOURCES.txt
 seunggabi_core_python.egg-info/dependency_links.txt
 seunggabi_core_python.egg-info/top_level.txt
 seunggabi_core_python/exception/__init__.py
 seunggabi_core_python/exception/bad_request.py
+seunggabi_core_python/exception/not_found.py
 seunggabi_core_python/util/__init__.py
 seunggabi_core_python/util/arg_util.py
 seunggabi_core_python/util/config_util.py
 seunggabi_core_python/util/json_util.py
 seunggabi_core_python/util/request_util.py
```

