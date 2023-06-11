# Comparing `tmp/kally-0.1.1.tar.gz` & `tmp/kally-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kally-0.1.1.tar", last modified: Fri Jun  9 06:51:47 2023, max compression
+gzip compressed data, was "kally-0.1.2.tar", last modified: Sun Jun 11 00:36:49 2023, max compression
```

## Comparing `kally-0.1.1.tar` & `kally-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:51:47.731364 kally-0.1.1/
--rw-rw-rw-   0        0        0     1101 2023-06-09 06:26:48.000000 kally-0.1.1/LICENSE.txt.txt
--rw-rw-rw-   0        0        0      467 2023-06-09 06:51:47.730366 kally-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 06:51:47.732363 kally-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-06-09 06:51:42.000000 kally-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:51:47.704991 kally-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 06:51:47.728382 kally-0.1.1/src/kally.egg-info/
--rw-rw-rw-   0        0        0      467 2023-06-09 06:51:47.000000 kally-0.1.1/src/kally.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-09 06:51:47.000000 kally-0.1.1/src/kally.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:51:47.000000 kally-0.1.1/src/kally.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-09 06:51:47.000000 kally-0.1.1/src/kally.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:51:47.000000 kally-0.1.1/src/kally.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 00:36:49.732653 kally-0.1.2/
+-rw-rw-rw-   0        0        0     1101 2023-06-11 00:36:38.000000 kally-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1107 2023-06-11 00:36:49.731654 kally-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-06-11 00:36:09.000000 kally-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 00:36:49.733653 kally-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-06-11 00:31:18.000000 kally-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 00:36:49.694702 kally-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 00:36:49.729655 kally-0.1.2/src/kally.egg-info/
+-rw-rw-rw-   0        0        0     1107 2023-06-11 00:36:49.000000 kally-0.1.2/src/kally.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-06-11 00:36:49.000000 kally-0.1.2/src/kally.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 00:36:49.000000 kally-0.1.2/src/kally.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-11 00:36:49.000000 kally-0.1.2/src/kally.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 00:36:49.000000 kally-0.1.2/src/kally.egg-info/top_level.txt
```

### Comparing `kally-0.1.1/LICENSE.txt.txt` & `kally-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kally-0.1.1/setup.py` & `kally-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kally",
-    version="0.1.1",
+    version="0.1.2",
     license='MIT',
     description="This is a clustering algorithm created based on the philosophy of competition for alliances, against the backdrop of the events of struggle for allies between warring countries. Especially the Russian-Ukrainian war.",
     author="Aslan Alwi and Munirah",
     author_email="elangbijak4@email.com",
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     url="https://github.com/elangbijak4/k-ally.1.0/blob/main/k-ally.1.0",
     packages=find_packages('src'),
     package_dir={'': 'src'},
-    #packages=["kally"],
     install_requires=[
           'pandas',
           'numpy'
       ],
 
 )
```

