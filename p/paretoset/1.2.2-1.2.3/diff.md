# Comparing `tmp/paretoset-1.2.2.tar.gz` & `tmp/paretoset-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paretoset-1.2.2.tar", last modified: Sun Jun 11 07:27:29 2023, max compression
+gzip compressed data, was "paretoset-1.2.3.tar", last modified: Sun Jun 11 08:50:22 2023, max compression
```

## Comparing `paretoset-1.2.2.tar` & `paretoset-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:27:29.207572 paretoset-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-11 07:26:35.000000 paretoset-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-11 07:27:29.207572 paretoset-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-11 07:26:35.000000 paretoset-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:27:29.207572 paretoset-1.2.2/paretoset/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/algorithms_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/algorithms_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/user_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:27:29.207572 paretoset-1.2.2/paretoset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 07:27:29.207572 paretoset-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-11 07:26:35.000000 paretoset-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:50:22.676870 paretoset-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-11 08:49:18.000000 paretoset-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-11 08:50:22.676870 paretoset-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-11 08:49:18.000000 paretoset-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:50:22.676870 paretoset-1.2.3/paretoset/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-11 08:49:18.000000 paretoset-1.2.3/paretoset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 08:49:18.000000 paretoset-1.2.3/paretoset/algorithms_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-11 08:49:18.000000 paretoset-1.2.3/paretoset/algorithms_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-11 08:49:18.000000 paretoset-1.2.3/paretoset/user_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-11 08:49:18.000000 paretoset-1.2.3/paretoset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:50:22.676870 paretoset-1.2.3/paretoset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-11 08:50:22.000000 paretoset-1.2.3/paretoset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-11 08:50:22.000000 paretoset-1.2.3/paretoset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 08:50:22.000000 paretoset-1.2.3/paretoset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 08:50:22.000000 paretoset-1.2.3/paretoset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 08:50:22.000000 paretoset-1.2.3/paretoset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 08:50:22.676870 paretoset-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-11 08:49:18.000000 paretoset-1.2.3/setup.py
```

### Comparing `paretoset-1.2.2/LICENSE` & `paretoset-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.2/PKG-INFO` & `paretoset-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paretoset
-Version: 1.2.2
+Version: 1.2.3
 Summary: Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
 Home-page: https://github.com/tommyod/paretoset
 Author: tommyod
 Author-email: tommy.odland@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `paretoset-1.2.2/README.md` & `paretoset-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.2/paretoset/__init__.py` & `paretoset-1.2.3/paretoset/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
 """
 
 # We use semantic versioning
 # See: https://semver.org/
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __author__ = "tommyod"
 
 import sys
 from paretoset.user_interface import paretoset, paretorank
 from paretoset.algorithms_numpy import crowding_distance
```

### Comparing `paretoset-1.2.2/paretoset/algorithms_numba.py` & `paretoset-1.2.3/paretoset/algorithms_numba.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.2/paretoset/algorithms_numpy.py` & `paretoset-1.2.3/paretoset/algorithms_numpy.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.2/paretoset/user_interface.py` & `paretoset-1.2.3/paretoset/user_interface.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.2/paretoset/utils.py` & `paretoset-1.2.3/paretoset/utils.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.2/paretoset.egg-info/PKG-INFO` & `paretoset-1.2.3/paretoset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paretoset
-Version: 1.2.2
+Version: 1.2.3
 Summary: Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
 Home-page: https://github.com/tommyod/paretoset
 Author: tommyod
 Author-email: tommy.odland@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `paretoset-1.2.2/setup.py` & `paretoset-1.2.3/setup.py`

 * *Files identical despite different names*

