# Comparing `tmp/paretoset-1.2.1.tar.gz` & `tmp/paretoset-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paretoset-1.2.1.tar", last modified: Sun Jun 11 07:16:36 2023, max compression
+gzip compressed data, was "paretoset-1.2.2.tar", last modified: Sun Jun 11 07:27:29 2023, max compression
```

## Comparing `paretoset-1.2.1.tar` & `paretoset-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:16:36.721978 paretoset-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-11 07:15:43.000000 paretoset-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-11 07:16:36.721978 paretoset-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-11 07:15:43.000000 paretoset-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:16:36.721978 paretoset-1.2.1/paretoset/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/algorithms_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/algorithms_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/user_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-11 07:15:43.000000 paretoset-1.2.1/paretoset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:16:36.721978 paretoset-1.2.1/paretoset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 07:16:36.000000 paretoset-1.2.1/paretoset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 07:16:36.725978 paretoset-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-11 07:15:43.000000 paretoset-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:27:29.207572 paretoset-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-11 07:26:35.000000 paretoset-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-11 07:27:29.207572 paretoset-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-11 07:26:35.000000 paretoset-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:27:29.207572 paretoset-1.2.2/paretoset/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/algorithms_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/algorithms_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/user_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-11 07:26:35.000000 paretoset-1.2.2/paretoset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 07:27:29.207572 paretoset-1.2.2/paretoset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 07:27:29.000000 paretoset-1.2.2/paretoset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 07:27:29.207572 paretoset-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-11 07:26:35.000000 paretoset-1.2.2/setup.py
```

### Comparing `paretoset-1.2.1/LICENSE` & `paretoset-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.1/PKG-INFO` & `paretoset-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: paretoset
-Version: 1.2.1
+Version: 1.2.2
 Summary: Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
 Home-page: https://github.com/tommyod/paretoset
 Author: tommyod
 Author-email: tommy.odland@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # paretoset ![Build Status](https://github.com/tommyod/paretoset/workflows/Python%20CI/badge.svg?branch=master) [![](https://badge.fury.io/py/paretoset.svg)](https://pypi.org/project/paretoset/) [![](https://pepy.tech/badge/paretoset)](https://pepy.tech/project/paretoset) [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
```

### Comparing `paretoset-1.2.1/README.md` & `paretoset-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.1/paretoset/__init__.py` & `paretoset-1.2.2/paretoset/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
 """
 
 # We use semantic versioning
 # See: https://semver.org/
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __author__ = "tommyod"
 
 import sys
 from paretoset.user_interface import paretoset, paretorank
 from paretoset.algorithms_numpy import crowding_distance
```

### Comparing `paretoset-1.2.1/paretoset/algorithms_numba.py` & `paretoset-1.2.2/paretoset/algorithms_numba.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.1/paretoset/algorithms_numpy.py` & `paretoset-1.2.2/paretoset/algorithms_numpy.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.1/paretoset/user_interface.py` & `paretoset-1.2.2/paretoset/user_interface.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.1/paretoset/utils.py` & `paretoset-1.2.2/paretoset/utils.py`

 * *Files identical despite different names*

### Comparing `paretoset-1.2.1/paretoset.egg-info/PKG-INFO` & `paretoset-1.2.2/paretoset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: paretoset
-Version: 1.2.1
+Version: 1.2.2
 Summary: Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
 Home-page: https://github.com/tommyod/paretoset
 Author: tommyod
 Author-email: tommy.odland@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # paretoset ![Build Status](https://github.com/tommyod/paretoset/workflows/Python%20CI/badge.svg?branch=master) [![](https://badge.fury.io/py/paretoset.svg)](https://pypi.org/project/paretoset/) [![](https://pepy.tech/badge/paretoset)](https://pepy.tech/project/paretoset) [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 Compute the Pareto (non-dominated) set, i.e., skyline operator/query.
```

### Comparing `paretoset-1.2.1/setup.py` & `paretoset-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         # Pick your license as you wish (should match "license" above)
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         # Specify the Python versions you support HERE. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     # You can just specify the packages manually HERE if your project is
     # simple. Or you can use find_packages().
     packages=find_packages(".", exclude=["contrib", "docs", "tests"]),
     package_dir={"paretoset": "paretoset"},
     # Alternatively, if you want to distribute just a my_module.py, uncomment
     # this:
```

