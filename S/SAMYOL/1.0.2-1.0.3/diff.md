# Comparing `tmp/samyol-1.0.2.tar.gz` & `tmp/SAMYOL-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samyol-1.0.2.tar", last modified: Sun Jun 11 20:40:44 2023, max compression
+gzip compressed data, was "SAMYOL-1.0.3.tar", last modified: Sun Jun 11 20:54:00 2023, max compression
```

## Comparing `samyol-1.0.2.tar` & `SAMYOL-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:40:44.418584 samyol-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 20:40:33.000000 samyol-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-11 20:40:44.418584 samyol-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-11 20:40:33.000000 samyol-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:40:44.418584 samyol-1.0.2/samyol/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/prediction_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/sam_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/yolo_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/yolo_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-11 20:40:33.000000 samyol-1.0.2/samyol/yolo_preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:40:44.418584 samyol-1.0.2/samyol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 20:40:44.000000 samyol-1.0.2/samyol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:40:44.418584 samyol-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-11 20:40:33.000000 samyol-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:54:00.829930 SAMYOL-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-11 20:54:00.829930 SAMYOL-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:54:00.825929 SAMYOL-1.0.3/SAMYOL/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/SAMYOL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/SAMYOL/prediction_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/SAMYOL/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/SAMYOL/sam_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/SAMYOL/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/SAMYOL/yolo_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/SAMYOL/yolo_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/SAMYOL/yolo_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:54:00.829930 SAMYOL-1.0.3/SAMYOL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-11 20:54:00.000000 SAMYOL-1.0.3/SAMYOL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-11 20:54:00.000000 SAMYOL-1.0.3/SAMYOL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:54:00.000000 SAMYOL-1.0.3/SAMYOL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 20:54:00.000000 SAMYOL-1.0.3/SAMYOL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 20:54:00.000000 SAMYOL-1.0.3/SAMYOL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:54:00.829930 SAMYOL-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-11 20:53:44.000000 SAMYOL-1.0.3/setup.py
```

### Comparing `samyol-1.0.2/LICENSE` & `SAMYOL-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `samyol-1.0.2/PKG-INFO` & `SAMYOL-1.0.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: samyol
-Version: 1.0.2
-Summary: Combines YOLO models and SAM
-Home-page: https://github.com/Jawher-Ben-Abdallah/SAMYOL
-Author: Jawher Ben Abdallah - Rim Sleimi
-Author-email: jawher.b.abdallah@gmail.com
-License: Apache License 2.0
-Keywords: YOLOv6,YOLOv7,YOLOv8,YOLO-NAS SAM,Object_Detection,Segmentation
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 =======
 SAMYOL
 =======
 .. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
    :target: https://opensource.org/licenses/Apache-2.0
    :alt: License: Apache 2.0
```

### Comparing `samyol-1.0.2/README.rst` & `SAMYOL-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: SAMYOL
+Version: 1.0.3
+Summary: Combines YOLO models and SAM
+Home-page: https://github.com/Jawher-Ben-Abdallah/SAMYOL
+Author: Jawher Ben Abdallah - Rim Sleimi
+Author-email: jawher.b.abdallah@gmail.com
+License: Apache License 2.0
+Keywords: YOLOv6,YOLOv7,YOLOv8,YOLO-NAS SAM,Object_Detection,Segmentation
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 =======
 SAMYOL
 =======
 .. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
    :target: https://opensource.org/licenses/Apache-2.0
    :alt: License: Apache 2.0
```

### Comparing `samyol-1.0.2/samyol/prediction_results.py` & `SAMYOL-1.0.3/SAMYOL/prediction_results.py`

 * *Files identical despite different names*

### Comparing `samyol-1.0.2/samyol/predictor.py` & `SAMYOL-1.0.3/SAMYOL/predictor.py`

 * *Files identical despite different names*

### Comparing `samyol-1.0.2/samyol/sam_inference.py` & `SAMYOL-1.0.3/SAMYOL/sam_inference.py`

 * *Files identical despite different names*

### Comparing `samyol-1.0.2/samyol/utils.py` & `SAMYOL-1.0.3/SAMYOL/utils.py`

 * *Files identical despite different names*

### Comparing `samyol-1.0.2/samyol/yolo_inference.py` & `SAMYOL-1.0.3/SAMYOL/yolo_inference.py`

 * *Files identical despite different names*

### Comparing `samyol-1.0.2/samyol/yolo_postprocessing.py` & `SAMYOL-1.0.3/SAMYOL/yolo_postprocessing.py`

 * *Files identical despite different names*

### Comparing `samyol-1.0.2/samyol/yolo_preprocessing.py` & `SAMYOL-1.0.3/SAMYOL/yolo_preprocessing.py`

 * *Files identical despite different names*

### Comparing `samyol-1.0.2/samyol.egg-info/PKG-INFO` & `SAMYOL-1.0.3/SAMYOL.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: samyol
-Version: 1.0.2
+Name: SAMYOL
+Version: 1.0.3
 Summary: Combines YOLO models and SAM
 Home-page: https://github.com/Jawher-Ben-Abdallah/SAMYOL
 Author: Jawher Ben Abdallah - Rim Sleimi
 Author-email: jawher.b.abdallah@gmail.com
 License: Apache License 2.0
 Keywords: YOLOv6,YOLOv7,YOLOv8,YOLO-NAS SAM,Object_Detection,Segmentation
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `samyol-1.0.2/setup.py` & `SAMYOL-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-  name="samyol",
-  version="1.0.2",
+  name="SAMYOL",
+  version="1.0.3",
   description="Combines YOLO models and SAM",
   packages=find_packages(),
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Jawher-Ben-Abdallah/SAMYOL",
   author="Jawher Ben Abdallah - Rim Sleimi",
   author_email="jawher.b.abdallah@gmail.com",
@@ -30,8 +30,8 @@
         "torchvision>=0.8.1",
         "tqdm>=4.64.0", 
         "onnxruntime"
     ],
     
     extras_require={"dev" : "twine>=4.0.2"},
     python_requires=">=3.10",
-)
+)
```

