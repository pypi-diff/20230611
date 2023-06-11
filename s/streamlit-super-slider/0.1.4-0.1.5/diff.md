# Comparing `tmp/streamlit-super-slider-0.1.4.tar.gz` & `tmp/streamlit-super-slider-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-super-slider-0.1.4.tar", last modified: Thu Jun  8 11:59:56 2023, max compression
+gzip compressed data, was "streamlit-super-slider-0.1.5.tar", last modified: Sun Jun 11 06:25:48 2023, max compression
```

## Comparing `streamlit-super-slider-0.1.4.tar` & `streamlit-super-slider-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:59:56.576767 streamlit-super-slider-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-08 11:59:56.576767 streamlit-super-slider-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:59:56.576767 streamlit-super-slider-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:59:56.572767 streamlit-super-slider-0.1.4/streamlit_super_slider/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/streamlit_super_slider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/streamlit_super_slider/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:59:56.576767 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:25:48.810590 streamlit-super-slider-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-11 06:24:15.000000 streamlit-super-slider-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-11 06:25:48.810590 streamlit-super-slider-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-11 06:24:15.000000 streamlit-super-slider-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 06:25:48.810590 streamlit-super-slider-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-11 06:24:15.000000 streamlit-super-slider-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:25:48.810590 streamlit-super-slider-0.1.5/streamlit_super_slider/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-11 06:24:15.000000 streamlit-super-slider-0.1.5/streamlit_super_slider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-11 06:24:15.000000 streamlit-super-slider-0.1.5/streamlit_super_slider/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:25:48.810590 streamlit-super-slider-0.1.5/streamlit_super_slider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-11 06:25:48.000000 streamlit-super-slider-0.1.5/streamlit_super_slider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-11 06:25:48.000000 streamlit-super-slider-0.1.5/streamlit_super_slider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 06:25:48.000000 streamlit-super-slider-0.1.5/streamlit_super_slider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 06:25:48.000000 streamlit-super-slider-0.1.5/streamlit_super_slider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 06:25:48.000000 streamlit-super-slider-0.1.5/streamlit_super_slider.egg-info/top_level.txt
```

### Comparing `streamlit-super-slider-0.1.4/PKG-INFO` & `streamlit-super-slider-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-super-slider
-Version: 0.1.4
+Version: 0.1.5
 Summary: A slider with a lot more features in it than the built in one.
 Home-page: https://github.com/fgdvir/streamlit-super-slider
 Author: Dvir Itzkovits
 Author-email: dvir.itzko@gmail.com
 Keywords: Python,Streamlit,React,JavaScript
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `streamlit-super-slider-0.1.4/README.md` & `streamlit-super-slider-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-super-slider-0.1.4/setup.py` & `streamlit-super-slider-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='streamlit-super-slider',
-    version='0.1.4',
+    version='0.1.5',
     author='Dvir Itzkovits',
     author_email='dvir.itzko@gmail.com',
     description='A slider with a lot more features in it than the built in one.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/fgdvir/streamlit-super-slider',
     # packages=['streamlit-super-slider'],
```

### Comparing `streamlit-super-slider-0.1.4/streamlit_super_slider/__init__.py` & `streamlit-super-slider-0.1.5/streamlit_super_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/PKG-INFO` & `streamlit-super-slider-0.1.5/streamlit_super_slider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-super-slider
-Version: 0.1.4
+Version: 0.1.5
 Summary: A slider with a lot more features in it than the built in one.
 Home-page: https://github.com/fgdvir/streamlit-super-slider
 Author: Dvir Itzkovits
 Author-email: dvir.itzko@gmail.com
 Keywords: Python,Streamlit,React,JavaScript
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

