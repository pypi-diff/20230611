# Comparing `tmp/econbeautylib-0.0.1.tar.gz` & `tmp/econbeautylib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/econbeautylib-0.0.1.tar", last modified: Sun Jun 11 21:26:21 2023, max compression
+gzip compressed data, was "dist/econbeautylib-0.0.2.tar", last modified: Sun Jun 11 21:29:58 2023, max compression
```

## Comparing `econbeautylib-0.0.1.tar` & `econbeautylib-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       36 2023-06-11 21:25:49.000000 econbeautylib-0.0.1/MANIFEST.in
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/PKG-INFO
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.1/README.md
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/econbeautylib/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       32 2023-06-11 21:25:49.000000 econbeautylib-0.0.1/econbeautylib/__init__.py
--rw-r--r--   0 dashka-z (1587325521) 593637566   171078 2023-06-11 21:25:53.000000 econbeautylib-0.0.1/econbeautylib/econstats.py
--rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.1/econbeautylib/tasks_base.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.1/econbeautylib/upload_task_to_base.py
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/econbeautylib.egg-info/
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/econbeautylib.egg-info/PKG-INFO
--rw-r--r--   0 dashka-z (1587325521) 593637566      343 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/econbeautylib.egg-info/SOURCES.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/econbeautylib.egg-info/dependency_links.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.1/econbeautylib.egg-info/not-zip-safe
--rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/econbeautylib.egg-info/top_level.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-11 21:26:21.000000 econbeautylib-0.0.1/setup.cfg
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-11 21:25:50.000000 econbeautylib-0.0.1/setup.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       36 2023-06-11 21:25:49.000000 econbeautylib-0.0.2/MANIFEST.in
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/PKG-INFO
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.2/README.md
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/econbeautylib/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.2/econbeautylib/__init__.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566   171078 2023-06-11 21:28:15.000000 econbeautylib-0.0.2/econbeautylib/econstats.py
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.2/econbeautylib/tasks_base.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.2/econbeautylib/upload_task_to_base.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/econbeautylib.egg-info/
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/econbeautylib.egg-info/PKG-INFO
+-rw-r--r--   0 dashka-z (1587325521) 593637566      343 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/econbeautylib.egg-info/SOURCES.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/econbeautylib.egg-info/dependency_links.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.2/econbeautylib.egg-info/not-zip-safe
+-rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/econbeautylib.egg-info/top_level.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-11 21:29:58.000000 econbeautylib-0.0.2/setup.cfg
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-11 21:29:48.000000 econbeautylib-0.0.2/setup.py
```

### Comparing `econbeautylib-0.0.1/README.md` & `econbeautylib-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.1/econbeautylib/econstats.py` & `econbeautylib-0.0.2/econbeautylib/econstats.py`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.1/econbeautylib/tasks_base.txt` & `econbeautylib-0.0.2/econbeautylib/tasks_base.txt`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.1/econbeautylib/upload_task_to_base.py` & `econbeautylib-0.0.2/econbeautylib/upload_task_to_base.py`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.1/setup.py` & `econbeautylib-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author:
 Зайцева Дарья
 """
 
 from setuptools import setup, find_packages
 long_description = '''Library for the 5 semester'''
 setup(name='econbeautylib',
-      version='0.0.1',
+      version='0.0.2',
       url='https://github.com/dashkazaitseva',
       packages=['econbeautylib'],
       license='MIT',
       description='',
       zip_safe=False,
       package_data={'econbeautylib': ['*.txt', '*.docx']},
       include_package_data=True
```

