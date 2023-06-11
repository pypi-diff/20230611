# Comparing `tmp/BLEST-Py-0.0.1.tar.gz` & `tmp/BLEST-Py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLEST-Py-0.0.1.tar", last modified: Sun Jun 11 21:53:10 2023, max compression
+gzip compressed data, was "BLEST-Py-0.0.2.tar", last modified: Sun Jun 11 21:56:44 2023, max compression
```

## Comparing `BLEST-Py-0.0.1.tar` & `BLEST-Py-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-11 21:53:10.607888 BLEST-Py-0.0.1/
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-11 21:53:10.606120 BLEST-Py-0.0.1/BLEST_Py.egg-info/
--rw-r--r--   0 admin      (501) wheel        (0)     3112 2023-06-11 21:53:10.000000 BLEST-Py-0.0.1/BLEST_Py.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)      503 2023-06-11 21:53:10.000000 BLEST-Py-0.0.1/BLEST_Py.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-11 21:53:10.000000 BLEST-Py-0.0.1/BLEST_Py.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) wheel        (0)        8 2023-06-11 21:53:10.000000 BLEST-Py-0.0.1/BLEST_Py.egg-info/requires.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-11 21:53:10.000000 BLEST-Py-0.0.1/BLEST_Py.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-Py-0.0.1/LICENSE
--rw-r--r--   0 admin      (501) wheel        (0)     3112 2023-06-11 21:53:10.607563 BLEST-Py-0.0.1/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)     2498 2023-06-11 21:49:11.000000 BLEST-Py-0.0.1/README.md
--rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-11 21:53:10.607990 BLEST-Py-0.0.1/setup.cfg
--rw-r--r--   0 admin      (501) wheel        (0)      880 2023-06-11 21:53:05.000000 BLEST-Py-0.0.1/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-11 21:56:44.623376 BLEST-Py-0.0.2/
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-11 21:56:44.621541 BLEST-Py-0.0.2/BLEST_Py.egg-info/
+-rw-r--r--   0 admin      (501) wheel        (0)     3115 2023-06-11 21:56:44.000000 BLEST-Py-0.0.2/BLEST_Py.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)      503 2023-06-11 21:56:44.000000 BLEST-Py-0.0.2/BLEST_Py.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-11 21:56:44.000000 BLEST-Py-0.0.2/BLEST_Py.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        8 2023-06-11 21:56:44.000000 BLEST-Py-0.0.2/BLEST_Py.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-11 21:56:44.000000 BLEST-Py-0.0.2/BLEST_Py.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-Py-0.0.2/LICENSE
+-rw-r--r--   0 admin      (501) wheel        (0)     3115 2023-06-11 21:56:44.623029 BLEST-Py-0.0.2/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)     2501 2023-06-11 21:56:18.000000 BLEST-Py-0.0.2/README.md
+-rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-11 21:56:44.623474 BLEST-Py-0.0.2/setup.cfg
+-rw-r--r--   0 admin      (501) wheel        (0)      880 2023-06-11 21:56:39.000000 BLEST-Py-0.0.2/setup.py
```

### Comparing `BLEST-Py-0.0.1/BLEST_Py.egg-info/PKG-INFO` & `BLEST-Py-0.0.2/BLEST_Py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BLEST-Py
-Version: 0.0.1
+Version: 0.0.2
 Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
 License: UNKNOWN
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 - Fully Encrypted - Improve data privacy
 
 ## Installation
 
 Install BLEST-Py from PyPI.
 
 ```bash
-pip install blest
+pip install blest_py
 ```
 
 ## Usage
 
 ### Server-side
 
 Use the `create_request_handler` function to create a request handler suitable for use in a Python application. The following example uses Flask, but you can find examples with other frameworks [here](/examples).
```

### Comparing `BLEST-Py-0.0.1/LICENSE` & `BLEST-Py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BLEST-Py-0.0.1/PKG-INFO` & `BLEST-Py-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BLEST-Py
-Version: 0.0.1
+Version: 0.0.2
 Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
 License: UNKNOWN
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 - Fully Encrypted - Improve data privacy
 
 ## Installation
 
 Install BLEST-Py from PyPI.
 
 ```bash
-pip install blest
+pip install blest_py
 ```
 
 ## Usage
 
 ### Server-side
 
 Use the `create_request_handler` function to create a request handler suitable for use in a Python application. The following example uses Flask, but you can find examples with other frameworks [here](/examples).
```

### Comparing `BLEST-Py-0.0.1/README.md` & `BLEST-Py-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - Fully Encrypted - Improve data privacy
 
 ## Installation
 
 Install BLEST-Py from PyPI.
 
 ```bash
-pip install blest
+pip install blest_py
 ```
 
 ## Usage
 
 ### Server-side
 
 Use the `create_request_handler` function to create a request handler suitable for use in a Python application. The following example uses Flask, but you can find examples with other frameworks [here](/examples).
```

### Comparing `BLEST-Py-0.0.1/setup.py` & `BLEST-Py-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="BLEST-Py",
-    version="0.0.1",
+    version="0.0.2",
     author="JHunt",
     author_email="blest@jhunt.dev",
     description="The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/jhuntdev/blest-py",
     packages=find_packages(),
```

