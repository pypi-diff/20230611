# Comparing `tmp/funcStats-0.0.7.tar.gz` & `tmp/funcStats-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcStats-0.0.7.tar", last modified: Sun Jun 11 05:15:00 2023, max compression
+gzip compressed data, was "funcStats-0.0.8.tar", last modified: Sun Jun 11 05:19:47 2023, max compression
```

## Comparing `funcStats-0.0.7.tar` & `funcStats-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:15:00.154183 funcStats-0.0.7/
--rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.7/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:15:00.153702 funcStats-0.0.7/PKG-INFO
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:15:00.149576 funcStats-0.0.7/funcStats/
--rw-r--r--   0 tom        (501) staff       (20)     4047 2023-06-11 05:14:38.000000 funcStats-0.0.7/funcStats/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-11 02:10:01.000000 funcStats-0.0.7/funcStats/log.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:15:00.153008 funcStats-0.0.7/funcStats.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:15:00.000000 funcStats-0.0.7/funcStats.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      219 2023-06-11 05:15:00.000000 funcStats-0.0.7/funcStats.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-11 05:15:00.000000 funcStats-0.0.7/funcStats.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       20 2023-06-11 05:15:00.000000 funcStats-0.0.7/funcStats.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-11 05:15:00.000000 funcStats-0.0.7/funcStats.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-11 05:15:00.154342 funcStats-0.0.7/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     1035 2023-06-11 05:14:38.000000 funcStats-0.0.7/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:19:47.340089 funcStats-0.0.8/
+-rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.8/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:19:47.339566 funcStats-0.0.8/PKG-INFO
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:19:47.335386 funcStats-0.0.8/funcStats/
+-rw-r--r--   0 tom        (501) staff       (20)     4047 2023-06-11 05:14:38.000000 funcStats-0.0.8/funcStats/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-11 02:10:01.000000 funcStats-0.0.8/funcStats/log.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:19:47.338818 funcStats-0.0.8/funcStats.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      219 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-11 05:19:47.340236 funcStats-0.0.8/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     1018 2023-06-11 05:18:02.000000 funcStats-0.0.8/setup.py
```

### Comparing `funcStats-0.0.7/LICENSE` & `funcStats-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.7/PKG-INFO` & `funcStats-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.0.7
+Version: 0.0.8
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.0.7/funcStats/__init__.py` & `funcStats-0.0.8/funcStats/__init__.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.7/funcStats/log.py` & `funcStats-0.0.8/funcStats/log.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.7/funcStats.egg-info/PKG-INFO` & `funcStats-0.0.8/funcStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.0.7
+Version: 0.0.8
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.0.7/setup.py` & `funcStats-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os.path
 
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'A module that helps to evaluate functions when some tests are needed'
 LONG_DESCRIPTION = str(open('/Volumes/Projetos/Git/funcStats/README.MD', 'r').read())
 
 setup(
     name="funcStats",
     version=VERSION,
     author="Elemental (Tom Neto)",
     author_email="<info@elemental.run>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['datetime', 'inspect', 'os'],
+    install_requires=['datetime'],
     keywords=['python', 'functions', 'cronometer', 'crono', 'meter', 'evaluate functions'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

