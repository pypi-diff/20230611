# Comparing `tmp/funcStats-0.0.4.tar.gz` & `tmp/funcStats-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcStats-0.0.4.tar", last modified: Sat Jun 10 02:40:01 2023, max compression
+gzip compressed data, was "funcStats-0.0.6.tar", last modified: Sun Jun 11 03:24:31 2023, max compression
```

## Comparing `funcStats-0.0.4.tar` & `funcStats-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 02:40:01.835934 funcStats-0.0.4/
--rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.4/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     1797 2023-06-10 02:40:01.835464 funcStats-0.0.4/PKG-INFO
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 02:40:01.830453 funcStats-0.0.4/funcStats/
--rw-r--r--   0 tom        (501) staff       (20)      758 2023-06-10 02:26:48.000000 funcStats-0.0.4/funcStats/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 02:40:01.834337 funcStats-0.0.4/funcStats.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     1797 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      202 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-10 02:40:01.836035 funcStats-0.0.4/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     1018 2023-06-10 02:39:53.000000 funcStats-0.0.4/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 03:24:31.463666 funcStats-0.0.6/
+-rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.6/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 03:24:31.463286 funcStats-0.0.6/PKG-INFO
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 03:24:31.460184 funcStats-0.0.6/funcStats/
+-rw-r--r--   0 tom        (501) staff       (20)     4134 2023-06-11 03:21:08.000000 funcStats-0.0.6/funcStats/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-11 02:10:01.000000 funcStats-0.0.6/funcStats/log.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-06-10 22:08:15.000000 funcStats-0.0.6/funcStats/modes.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 03:24:31.462686 funcStats-0.0.6/funcStats.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 03:24:31.000000 funcStats-0.0.6/funcStats.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      238 2023-06-11 03:24:31.000000 funcStats-0.0.6/funcStats.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-11 03:24:31.000000 funcStats-0.0.6/funcStats.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       17 2023-06-11 03:24:31.000000 funcStats-0.0.6/funcStats.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-11 03:24:31.000000 funcStats-0.0.6/funcStats.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-11 03:24:31.463832 funcStats-0.0.6/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     1029 2023-06-11 03:24:11.000000 funcStats-0.0.6/setup.py
```

### Comparing `funcStats-0.0.4/LICENSE` & `funcStats-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.4/setup.py` & `funcStats-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os.path
 
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.4'
+VERSION = '0.0.6'
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
-    install_requires=['datetime'],
+    install_requires=['datetime', 'inspect'],
     keywords=['python', 'functions', 'cronometer', 'crono', 'meter', 'evaluate functions'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

