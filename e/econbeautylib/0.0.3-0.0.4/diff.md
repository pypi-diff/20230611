# Comparing `tmp/econbeautylib-0.0.3.tar.gz` & `tmp/econbeautylib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/econbeautylib-0.0.3.tar", last modified: Sun Jun 11 21:32:56 2023, max compression
+gzip compressed data, was "dist/econbeautylib-0.0.4.tar", last modified: Sun Jun 11 21:37:06 2023, max compression
```

## Comparing `econbeautylib-0.0.3.tar` & `econbeautylib-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       36 2023-06-11 21:25:49.000000 econbeautylib-0.0.3/MANIFEST.in
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/PKG-INFO
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.3/README.md
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/econbeautylib/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.3/econbeautylib/__init__.py
--rw-r--r--   0 dashka-z (1587325521) 593637566   171119 2023-06-11 21:32:48.000000 econbeautylib-0.0.3/econbeautylib/econstats.py
--rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.3/econbeautylib/tasks_base.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.3/econbeautylib/upload_task_to_base.py
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/econbeautylib.egg-info/
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/econbeautylib.egg-info/PKG-INFO
--rw-r--r--   0 dashka-z (1587325521) 593637566      343 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/econbeautylib.egg-info/SOURCES.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/econbeautylib.egg-info/dependency_links.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.3/econbeautylib.egg-info/not-zip-safe
--rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/econbeautylib.egg-info/top_level.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-11 21:32:56.000000 econbeautylib-0.0.3/setup.cfg
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-11 21:32:53.000000 econbeautylib-0.0.3/setup.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       69 2023-06-11 21:36:53.000000 econbeautylib-0.0.4/MANIFEST.in
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/PKG-INFO
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.4/README.md
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/econbeautylib/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.4/econbeautylib/__init__.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566   171119 2023-06-11 21:32:48.000000 econbeautylib-0.0.4/econbeautylib/econstats.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566    12503 2023-06-11 20:36:33.000000 econbeautylib-0.0.4/econbeautylib/tasks.docx
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.4/econbeautylib/tasks_base.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.4/econbeautylib/upload_task_to_base.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/econbeautylib.egg-info/
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/econbeautylib.egg-info/PKG-INFO
+-rw-r--r--   0 dashka-z (1587325521) 593637566      368 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/econbeautylib.egg-info/SOURCES.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/econbeautylib.egg-info/dependency_links.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.4/econbeautylib.egg-info/not-zip-safe
+-rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/econbeautylib.egg-info/top_level.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-11 21:37:06.000000 econbeautylib-0.0.4/setup.cfg
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-11 21:37:00.000000 econbeautylib-0.0.4/setup.py
```

### Comparing `econbeautylib-0.0.3/README.md` & `econbeautylib-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.3/econbeautylib/econstats.py` & `econbeautylib-0.0.4/econbeautylib/econstats.py`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.3/econbeautylib/tasks_base.txt` & `econbeautylib-0.0.4/econbeautylib/tasks_base.txt`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.3/econbeautylib/upload_task_to_base.py` & `econbeautylib-0.0.4/econbeautylib/upload_task_to_base.py`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.3/setup.py` & `econbeautylib-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author:
 Зайцева Дарья
 """
 
 from setuptools import setup, find_packages
 long_description = '''Library for the 5 semester'''
 setup(name='econbeautylib',
-      version='0.0.3',
+      version='0.0.4',
       url='https://github.com/dashkazaitseva',
       packages=['econbeautylib'],
       license='MIT',
       description='',
       zip_safe=False,
       package_data={'econbeautylib': ['*.txt', '*.docx']},
       include_package_data=True
```

