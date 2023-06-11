# Comparing `tmp/yeastmlp-0.0.2.tar.gz` & `tmp/yeastmlp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yeastmlp-0.0.2.tar", last modified: Sun Jun 11 20:36:44 2023, max compression
+gzip compressed data, was "dist/yeastmlp-0.0.3.tar", last modified: Sun Jun 11 20:40:23 2023, max compression
```

## Comparing `yeastmlp-0.0.2.tar` & `yeastmlp-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-06-11 20:36:44.395215 yeastmlp-0.0.2/
--rw-r--r--   0 bencekover   (501) staff       (20)     1065 2023-06-11 20:27:20.000000 yeastmlp-0.0.2/LICENSE
--rw-r--r--   0 bencekover   (501) staff       (20)      582 2023-06-11 20:36:44.395041 yeastmlp-0.0.2/PKG-INFO
--rw-r--r--   0 bencekover   (501) staff       (20)      865 2023-06-11 20:27:20.000000 yeastmlp-0.0.2/README.md
--rw-r--r--   0 bencekover   (501) staff       (20)       38 2023-06-11 20:36:44.395258 yeastmlp-0.0.2/setup.cfg
--rw-r--r--   0 bencekover   (501) staff       (20)     1015 2023-06-11 20:36:13.000000 yeastmlp-0.0.2/setup.py
-drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-06-11 20:36:44.394180 yeastmlp-0.0.2/yeastmlp/
--rw-r--r--   0 bencekover   (501) staff       (20)        0 2023-06-02 09:17:34.000000 yeastmlp-0.0.2/yeastmlp/__init__.py
--rw-r--r--   0 bencekover   (501) staff       (20)    15569 2023-06-05 09:12:24.000000 yeastmlp-0.0.2/yeastmlp/adhesion.py
--rw-r--r--   0 bencekover   (501) staff       (20)     4764 2023-06-02 13:55:35.000000 yeastmlp-0.0.2/yeastmlp/flocculation.py
-drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-06-11 20:36:44.394880 yeastmlp-0.0.2/yeastmlp.egg-info/
--rw-r--r--   0 bencekover   (501) staff       (20)      582 2023-06-11 20:36:44.000000 yeastmlp-0.0.2/yeastmlp.egg-info/PKG-INFO
--rw-r--r--   0 bencekover   (501) staff       (20)      252 2023-06-11 20:36:44.000000 yeastmlp-0.0.2/yeastmlp.egg-info/SOURCES.txt
--rw-r--r--   0 bencekover   (501) staff       (20)        1 2023-06-11 20:36:44.000000 yeastmlp-0.0.2/yeastmlp.egg-info/dependency_links.txt
--rw-r--r--   0 bencekover   (501) staff       (20)       43 2023-06-11 20:36:44.000000 yeastmlp-0.0.2/yeastmlp.egg-info/requires.txt
--rw-r--r--   0 bencekover   (501) staff       (20)        9 2023-06-11 20:36:44.000000 yeastmlp-0.0.2/yeastmlp.egg-info/top_level.txt
+drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-06-11 20:40:23.730798 yeastmlp-0.0.3/
+-rw-r--r--   0 bencekover   (501) staff       (20)     1065 2023-06-11 20:27:20.000000 yeastmlp-0.0.3/LICENSE
+-rw-r--r--   0 bencekover   (501) staff       (20)      582 2023-06-11 20:40:23.730600 yeastmlp-0.0.3/PKG-INFO
+-rw-r--r--   0 bencekover   (501) staff       (20)      865 2023-06-11 20:27:20.000000 yeastmlp-0.0.3/README.md
+-rw-r--r--   0 bencekover   (501) staff       (20)       38 2023-06-11 20:40:23.730853 yeastmlp-0.0.3/setup.cfg
+-rw-r--r--   0 bencekover   (501) staff       (20)     1015 2023-06-11 20:40:07.000000 yeastmlp-0.0.3/setup.py
+drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-06-11 20:40:23.729684 yeastmlp-0.0.3/yeastmlp/
+-rw-r--r--   0 bencekover   (501) staff       (20)        0 2023-06-02 09:17:34.000000 yeastmlp-0.0.3/yeastmlp/__init__.py
+-rw-r--r--   0 bencekover   (501) staff       (20)    15569 2023-06-05 09:12:24.000000 yeastmlp-0.0.3/yeastmlp/adhesion.py
+-rw-r--r--   0 bencekover   (501) staff       (20)     4764 2023-06-02 13:55:35.000000 yeastmlp-0.0.3/yeastmlp/flocculation.py
+drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-06-11 20:40:23.730428 yeastmlp-0.0.3/yeastmlp.egg-info/
+-rw-r--r--   0 bencekover   (501) staff       (20)      582 2023-06-11 20:40:23.000000 yeastmlp-0.0.3/yeastmlp.egg-info/PKG-INFO
+-rw-r--r--   0 bencekover   (501) staff       (20)      252 2023-06-11 20:40:23.000000 yeastmlp-0.0.3/yeastmlp.egg-info/SOURCES.txt
+-rw-r--r--   0 bencekover   (501) staff       (20)        1 2023-06-11 20:40:23.000000 yeastmlp-0.0.3/yeastmlp.egg-info/dependency_links.txt
+-rw-r--r--   0 bencekover   (501) staff       (20)       43 2023-06-11 20:40:23.000000 yeastmlp-0.0.3/yeastmlp.egg-info/requires.txt
+-rw-r--r--   0 bencekover   (501) staff       (20)        9 2023-06-11 20:40:23.000000 yeastmlp-0.0.3/yeastmlp.egg-info/top_level.txt
```

### Comparing `yeastmlp-0.0.2/LICENSE` & `yeastmlp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yeastmlp-0.0.2/PKG-INFO` & `yeastmlp-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastmlp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for analysis of Multicellular-like phenotype formation in yeast species
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: python,yeast,biology,multicellularity,adhesion,flocculation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yeastmlp-0.0.2/README.md` & `yeastmlp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `yeastmlp-0.0.2/setup.py` & `yeastmlp-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Python package for analysis of Multicellular-like phenotype formation in yeast species'
 LONG_DESCRIPTION = 'Python package for analysis of Multicellular-like phenotype formation in yeast, for more information see https://github.com/BKover99/yeastmlp'
 
 
 setup(
     name="yeastmlp",
     version=VERSION,
```

### Comparing `yeastmlp-0.0.2/yeastmlp/adhesion.py` & `yeastmlp-0.0.3/yeastmlp/adhesion.py`

 * *Files identical despite different names*

### Comparing `yeastmlp-0.0.2/yeastmlp/flocculation.py` & `yeastmlp-0.0.3/yeastmlp/flocculation.py`

 * *Files identical despite different names*

### Comparing `yeastmlp-0.0.2/yeastmlp.egg-info/PKG-INFO` & `yeastmlp-0.0.3/yeastmlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastmlp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for analysis of Multicellular-like phenotype formation in yeast species
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: python,yeast,biology,multicellularity,adhesion,flocculation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

