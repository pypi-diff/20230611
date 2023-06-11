# Comparing `tmp/SAMYOL-1.0.1.tar.gz` & `tmp/samyol-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMYOL-1.0.1.tar", last modified: Sun Jun 11 16:37:56 2023, max compression
+gzip compressed data, was "samyol-1.0.2.tar", last modified: Sun Jun 11 20:40:44 2023, max compression
```

## Comparing `SAMYOL-1.0.1.tar` & `samyol-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:37:56.103617 SAMYOL-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 16:37:45.000000 SAMYOL-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-11 16:37:56.103617 SAMYOL-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-11 16:37:45.000000 SAMYOL-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:37:56.099617 SAMYOL-1.0.1/SAMYOL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-11 16:37:56.000000 SAMYOL-1.0.1/SAMYOL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-11 16:37:56.000000 SAMYOL-1.0.1/SAMYOL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:37:56.000000 SAMYOL-1.0.1/SAMYOL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 16:37:56.000000 SAMYOL-1.0.1/SAMYOL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:37:56.000000 SAMYOL-1.0.1/SAMYOL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 16:37:56.103617 SAMYOL-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-11 16:37:45.000000 SAMYOL-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:40:44.418584 samyol-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 20:40:33.000000 samyol-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-11 20:40:44.418584 samyol-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-11 20:40:33.000000 samyol-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:40:44.418584 samyol-1.0.2/samyol/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/prediction_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/sam_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/yolo_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/yolo_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/yolo_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:40:44.418584 samyol-1.0.2/samyol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:40:44.418584 samyol-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-11 20:40:33.000000 samyol-1.0.2/setup.py
```

### Comparing `SAMYOL-1.0.1/LICENSE` & `samyol-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.1/PKG-INFO` & `samyol-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SAMYOL
-Version: 1.0.1
+Name: samyol
+Version: 1.0.2
 Summary: Combines YOLO models and SAM
 Home-page: https://github.com/Jawher-Ben-Abdallah/SAMYOL
 Author: Jawher Ben Abdallah - Rim Sleimi
 Author-email: jawher.b.abdallah@gmail.com
 License: Apache License 2.0
 Keywords: YOLOv6,YOLOv7,YOLOv8,YOLO-NAS SAM,Object_Detection,Segmentation
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `SAMYOL-1.0.1/README.rst` & `samyol-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.1/SAMYOL.egg-info/PKG-INFO` & `samyol-1.0.2/samyol.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SAMYOL
-Version: 1.0.1
+Name: samyol
+Version: 1.0.2
 Summary: Combines YOLO models and SAM
 Home-page: https://github.com/Jawher-Ben-Abdallah/SAMYOL
 Author: Jawher Ben Abdallah - Rim Sleimi
 Author-email: jawher.b.abdallah@gmail.com
 License: Apache License 2.0
 Keywords: YOLOv6,YOLOv7,YOLOv8,YOLO-NAS SAM,Object_Detection,Segmentation
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `SAMYOL-1.0.1/setup.py` & `samyol-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-  name="SAMYOL",
-  version="1.0.1",
+  name="samyol",
+  version="1.0.2",
   description="Combines YOLO models and SAM",
-  package_dir={"samyol": "."},
-  packages=find_packages(where="samyol"),
+  packages=find_packages(),
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Jawher-Ben-Abdallah/SAMYOL",
   author="Jawher Ben Abdallah - Rim Sleimi",
   author_email="jawher.b.abdallah@gmail.com",
   license='Apache License 2.0',
   classifiers=[
```

