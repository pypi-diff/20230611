# Comparing `tmp/morel-0.1.1.tar.gz` & `tmp/morel-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-0.1.1.tar", last modified: Sun Jun 11 11:28:03 2023, max compression
+gzip compressed data, was "morel-1.0.0.tar", last modified: Sun Jun 11 13:33:58 2023, max compression
```

## Comparing `morel-0.1.1.tar` & `morel-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,20 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 11:28:03.159790 morel-0.1.1/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-0.1.1/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      710 2023-06-11 11:28:03.159790 morel-0.1.1/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      116 2023-06-11 11:24:38.000000 morel-0.1.1/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      744 2023-06-11 11:27:58.000000 morel-0.1.1/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-11 11:28:03.159790 morel-0.1.1/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 11:28:03.155790 morel-0.1.1/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 11:28:03.157790 morel-0.1.1/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)        0 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      959 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/__main__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1401 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/config.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1699 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/db.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     4489 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      588 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/lipsum.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     2061 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/logger.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 11:28:03.158790 morel-0.1.1/src/morel/processes/
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1646 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/processes/FileObserver.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1596 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/processes/FlagSubmitter.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3785 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/processes/GametickManager.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      125 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/processes/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-11 10:43:51.000000 morel-0.1.1/src/morel/singleton.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 11:28:03.158790 morel-0.1.1/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      710 2023-06-11 11:28:03.000000 morel-0.1.1/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      505 2023-06-11 11:28:03.000000 morel-0.1.1/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-11 11:28:03.000000 morel-0.1.1/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        7 2023-06-11 11:28:03.000000 morel-0.1.1/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-11 11:28:03.000000 morel-0.1.1/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 13:33:58.303155 morel-1.0.0/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.0.0/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-11 13:33:58.302155 morel-1.0.0/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.0.0/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-11 13:33:21.000000 morel-1.0.0/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-11 13:33:58.303155 morel-1.0.0/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 13:33:58.300155 morel-1.0.0/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 13:33:58.301155 morel-1.0.0/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       48 2023-06-11 13:30:07.000000 morel-1.0.0/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     2363 2023-06-11 13:31:43.000000 morel-1.0.0/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      904 2023-06-11 13:31:40.000000 morel-1.0.0/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     2061 2023-06-11 13:20:57.000000 morel-1.0.0/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      687 2023-06-11 12:28:03.000000 morel-1.0.0/src/morel/template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 13:33:58.302155 morel-1.0.0/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      335 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/top_level.txt
```

### Comparing `morel-0.1.1/LICENSE` & `morel-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-0.1.1/PKG-INFO` & `morel-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 0.1.1
+Version: 1.0.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyPI - License](https://img.shields.io/pypi/l/morel)
 
-https://en.wikipedia.org/wiki/Morelia_(snake)?oldformat=true
+https://en.wikipedia.org/wiki/Morelia_(snake)
```

### Comparing `morel-0.1.1/src/morel/logger.py` & `morel-1.0.0/src/morel/logger.py`

 * *Files identical despite different names*

### Comparing `morel-0.1.1/src/morel.egg-info/PKG-INFO` & `morel-1.0.0/src/morel.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 0.1.1
+Version: 1.0.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyPI - License](https://img.shields.io/pypi/l/morel)
 
-https://en.wikipedia.org/wiki/Morelia_(snake)?oldformat=true
+https://en.wikipedia.org/wiki/Morelia_(snake)
```

