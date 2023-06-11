# Comparing `tmp/funcStats-0.0.8.tar.gz` & `tmp/funcStats-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcStats-0.0.8.tar", last modified: Sun Jun 11 05:19:47 2023, max compression
+gzip compressed data, was "funcStats-0.0.9.tar", last modified: Sun Jun 11 05:50:28 2023, max compression
```

## Comparing `funcStats-0.0.8.tar` & `funcStats-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:19:47.340089 funcStats-0.0.8/
--rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.8/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:19:47.339566 funcStats-0.0.8/PKG-INFO
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:19:47.335386 funcStats-0.0.8/funcStats/
--rw-r--r--   0 tom        (501) staff       (20)     4047 2023-06-11 05:14:38.000000 funcStats-0.0.8/funcStats/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-11 02:10:01.000000 funcStats-0.0.8/funcStats/log.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:19:47.338818 funcStats-0.0.8/funcStats.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      219 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-11 05:19:47.000000 funcStats-0.0.8/funcStats.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-11 05:19:47.340236 funcStats-0.0.8/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     1018 2023-06-11 05:18:02.000000 funcStats-0.0.8/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:50:28.543279 funcStats-0.0.9/
+-rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.9/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:50:28.542869 funcStats-0.0.9/PKG-INFO
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:50:28.538689 funcStats-0.0.9/funcStats/
+-rw-r--r--   0 tom        (501) staff       (20)     4196 2023-06-11 05:47:21.000000 funcStats-0.0.9/funcStats/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-11 02:10:01.000000 funcStats-0.0.9/funcStats/log.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:50:28.542286 funcStats-0.0.9/funcStats.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      219 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-11 05:50:28.543396 funcStats-0.0.9/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     1018 2023-06-11 05:49:53.000000 funcStats-0.0.9/setup.py
```

### Comparing `funcStats-0.0.8/LICENSE` & `funcStats-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.8/PKG-INFO` & `funcStats-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.0.8
+Version: 0.0.9
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.0.8/funcStats/__init__.py` & `funcStats-0.0.9/funcStats/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,18 @@
 
                 self.logStream.skipLine()
                 self.logStream.add(f'Meter Execution Count: {self.count}')
                 self.logStream.add(f"Meter Execution Starts at: {startTime}")
                 self.logStream.add(f"Meter Execution Args: {argPack}")
 
                 try:
-                    executionResult = str(self.func(*argPack))
+                    if not isinstance(argPack, str):
+                        executionResult = str(self.func(*argPack))
+                    else:
+                        executionResult = str(self.func(argPack))
                 except Exception as e:
                     executionResult = e
 
                 self.logStream.add(f"Meter Execution Returns: {str(executionResult)}...")
 
                 endTime = datetime.now()
```

### Comparing `funcStats-0.0.8/funcStats/log.py` & `funcStats-0.0.9/funcStats/log.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.8/funcStats.egg-info/PKG-INFO` & `funcStats-0.0.9/funcStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.0.8
+Version: 0.0.9
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.0.8/setup.py` & `funcStats-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path
 
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'A module that helps to evaluate functions when some tests are needed'
 LONG_DESCRIPTION = str(open('/Volumes/Projetos/Git/funcStats/README.MD', 'r').read())
 
 setup(
     name="funcStats",
     version=VERSION,
     author="Elemental (Tom Neto)",
```

