# Comparing `tmp/bhv-0.5.7.tar.gz` & `tmp/bhv-0.5.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.5.7.tar", last modified: Sun Jun 11 00:58:32 2023, max compression
+gzip compressed data, was "bhv-0.5.7a0.tar", last modified: Sun Jun 11 01:10:46 2023, max compression
```

## Comparing `bhv-0.5.7.tar` & `bhv-0.5.7a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 00:58:32.537017 bhv-0.5.7/
--rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.5.7/LICENSE
--rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-11 00:58:32.536017 bhv-0.5.7/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.5.7/README.md
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 00:58:32.536017 bhv-0.5.7/bhv/
--rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.5.7/bhv/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)    14829 2023-06-06 19:12:06.000000 bhv-0.5.7/bhv/abstract.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 00:58:32.536017 bhv-0.5.7/bhv/cnative/
--rw-r--r--   0 adam      (1000) adam      (1000)     9757 2023-06-11 00:54:32.000000 bhv-0.5.7/bhv/cnative/bindings.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/embedding.py
--rw-r--r--   0 adam      (1000) adam      (1000)     4220 2023-06-06 19:12:06.000000 bhv-0.5.7/bhv/lookup.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1476 2023-06-11 00:46:52.000000 bhv-0.5.7/bhv/native.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11951 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/np.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/poibin.py
--rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/pytorch.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/shared.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/slice.py
--rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/symbolic.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/unification.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3456 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/vanilla.py
--rw-r--r--   0 adam      (1000) adam      (1000)      782 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/visualization.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 00:58:32.536017 bhv-0.5.7/bhv.egg-info/
--rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      399 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       45 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-11 00:58:32.537017 bhv-0.5.7/setup.cfg
--rw-r--r--   0 adam      (1000) adam      (1000)     1565 2023-06-11 00:55:47.000000 bhv-0.5.7/setup.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:10:46.904894 bhv-0.5.7a0/
+-rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.5.7a0/LICENSE
+-rw-r--r--   0 adam      (1000) adam      (1000)     1093 2023-06-11 01:10:46.904894 bhv-0.5.7a0/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.5.7a0/README.md
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:10:46.904894 bhv-0.5.7a0/bhv/
+-rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.5.7a0/bhv/__init__.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    14829 2023-06-06 19:12:06.000000 bhv-0.5.7a0/bhv/abstract.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:10:46.904894 bhv-0.5.7a0/bhv/cnative/
+-rw-r--r--   0 adam      (1000) adam      (1000)     9757 2023-06-11 00:54:32.000000 bhv-0.5.7a0/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/embedding.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     4220 2023-06-06 19:12:06.000000 bhv-0.5.7a0/bhv/lookup.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1476 2023-06-11 00:46:52.000000 bhv-0.5.7a0/bhv/native.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11951 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/np.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/poibin.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/pytorch.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/shared.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/slice.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/symbolic.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/unification.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3456 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/vanilla.py
+-rw-r--r--   0 adam      (1000) adam      (1000)      782 2023-05-25 19:11:00.000000 bhv-0.5.7a0/bhv/visualization.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:10:46.904894 bhv-0.5.7a0/bhv.egg-info/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1093 2023-06-11 01:10:46.000000 bhv-0.5.7a0/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)      399 2023-06-11 01:10:46.000000 bhv-0.5.7a0/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-11 01:10:46.000000 bhv-0.5.7a0/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       45 2023-06-11 01:10:46.000000 bhv-0.5.7a0/bhv.egg-info/requires.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-11 01:10:46.000000 bhv-0.5.7a0/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-11 01:10:46.904894 bhv-0.5.7a0/setup.cfg
+-rw-r--r--   0 adam      (1000) adam      (1000)     1566 2023-06-11 01:10:43.000000 bhv-0.5.7a0/setup.py
```

### Comparing `bhv-0.5.7/LICENSE` & `bhv-0.5.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/PKG-INFO` & `bhv-0.5.7a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.5.7
+Version: 0.5.7a0
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.5.7/README.md` & `bhv-0.5.7a0/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/abstract.py` & `bhv-0.5.7a0/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/cnative/bindings.cpp` & `bhv-0.5.7a0/bhv/cnative/bindings.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/embedding.py` & `bhv-0.5.7a0/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/lookup.py` & `bhv-0.5.7a0/bhv/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/native.py` & `bhv-0.5.7a0/bhv/native.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/np.py` & `bhv-0.5.7a0/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/poibin.py` & `bhv-0.5.7a0/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/pytorch.py` & `bhv-0.5.7a0/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/shared.py` & `bhv-0.5.7a0/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/slice.py` & `bhv-0.5.7a0/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/symbolic.py` & `bhv-0.5.7a0/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/unification.py` & `bhv-0.5.7a0/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/vanilla.py` & `bhv-0.5.7a0/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv/visualization.py` & `bhv-0.5.7a0/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7/bhv.egg-info/PKG-INFO` & `bhv-0.5.7a0/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.5.7
+Version: 0.5.7a0
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.5.7/setup.py` & `bhv-0.5.7a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages, Extension
 
-VERSION = '0.5.7'
+VERSION = '0.5.7a'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 native = Extension("bhv.cnative", sources=['bhv/cnative/bindings.cpp'],
-                   extra_compile_args=['-std=c++20', '-O3', '-march=native'],
+                   extra_compile_args=['-std=c++2a', '-O3', '-march=native'],
                    language='c++')
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
     author_email="contact@adamv.be",
     description=DESCRIPTION,
```

