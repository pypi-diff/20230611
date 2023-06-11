# Comparing `tmp/quickstart-vdk-0.2.895757559.dev11276.tar.gz` & `tmp/quickstart-vdk-0.2.896146019.dev11277.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.895757559.dev11276.tar", last modified: Sat Jun 10 04:21:35 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.896146019.dev11277.tar", last modified: Sun Jun 11 04:22:26 2023, max compression
```

## Comparing `quickstart-vdk-0.2.895757559.dev11276.tar` & `quickstart-vdk-0.2.896146019.dev11277.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 04:21:35.827620 quickstart-vdk-0.2.895757559.dev11276/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-10 04:21:35.827620 quickstart-vdk-0.2.895757559.dev11276/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-10 04:18:43.000000 quickstart-vdk-0.2.895757559.dev11276/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 04:21:35.827620 quickstart-vdk-0.2.895757559.dev11276/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-10 04:21:35.000000 quickstart-vdk-0.2.895757559.dev11276/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-10 04:21:35.000000 quickstart-vdk-0.2.895757559.dev11276/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 04:21:35.000000 quickstart-vdk-0.2.895757559.dev11276/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-10 04:21:35.000000 quickstart-vdk-0.2.895757559.dev11276/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-10 04:21:35.000000 quickstart-vdk-0.2.895757559.dev11276/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 04:21:35.827620 quickstart-vdk-0.2.895757559.dev11276/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-10 04:21:25.000000 quickstart-vdk-0.2.895757559.dev11276/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 04:21:35.827620 quickstart-vdk-0.2.895757559.dev11276/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-10 04:18:43.000000 quickstart-vdk-0.2.895757559.dev11276/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:22:26.983727 quickstart-vdk-0.2.896146019.dev11277/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-11 04:22:26.983727 quickstart-vdk-0.2.896146019.dev11277/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-11 04:19:45.000000 quickstart-vdk-0.2.896146019.dev11277/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:22:26.983727 quickstart-vdk-0.2.896146019.dev11277/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-11 04:22:26.000000 quickstart-vdk-0.2.896146019.dev11277/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-11 04:22:26.000000 quickstart-vdk-0.2.896146019.dev11277/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 04:22:26.000000 quickstart-vdk-0.2.896146019.dev11277/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-11 04:22:26.000000 quickstart-vdk-0.2.896146019.dev11277/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-11 04:22:26.000000 quickstart-vdk-0.2.896146019.dev11277/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 04:22:26.983727 quickstart-vdk-0.2.896146019.dev11277/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-11 04:22:17.000000 quickstart-vdk-0.2.896146019.dev11277/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:22:26.983727 quickstart-vdk-0.2.896146019.dev11277/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-11 04:19:45.000000 quickstart-vdk-0.2.896146019.dev11277/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.895757559.dev11276/PKG-INFO` & `quickstart-vdk-0.2.896146019.dev11277/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.895757559.dev11276
+Version: 0.2.896146019.dev11277
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.895757559.dev11276/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.896146019.dev11277/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.895757559.dev11276
+Version: 0.2.896146019.dev11277
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.895757559.dev11276/setup.py` & `quickstart-vdk-0.2.896146019.dev11277/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.895757559.dev11276"
+__version__ = "0.2.896146019.dev11277"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

