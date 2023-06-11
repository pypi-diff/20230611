# Comparing `tmp/moosez-2.0.4.tar.gz` & `tmp/moosez-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.0.4.tar", last modified: Wed Jun  7 17:49:43 2023, max compression
+gzip compressed data, was "moosez-2.0.5.tar", last modified: Sun Jun 11 14:51:14 2023, max compression
```

## Comparing `moosez-2.0.4.tar` & `moosez-2.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-07 17:49:43.199844 moosez-2.0.4/
--rw-r--r--   0 lalithsimac   (501) staff       (20)    11357 2023-06-06 13:31:59.000000 moosez-2.0.4/LICENSE
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1427 2023-06-07 17:49:43.199448 moosez-2.0.4/PKG-INFO
--rw-r--r--   0 lalithsimac   (501) staff       (20)    19071 2023-06-06 13:31:59.000000 moosez-2.0.4/README.md
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-07 17:49:43.196355 moosez-2.0.4/moosez/
--rw-r--r--   0 lalithsimac   (501) staff       (20)      227 2023-06-06 13:31:59.000000 moosez-2.0.4/moosez/__init__.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1362 2023-06-06 13:31:59.000000 moosez-2.0.4/moosez/constants.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     5434 2023-06-07 12:38:35.000000 moosez-2.0.4/moosez/display.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3662 2023-06-06 13:31:59.000000 moosez-2.0.4/moosez/download.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4119 2023-06-06 13:31:59.000000 moosez-2.0.4/moosez/file_utilities.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4002 2023-06-06 13:31:59.000000 moosez-2.0.4/moosez/image_conversion.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3416 2023-06-06 15:07:22.000000 moosez-2.0.4/moosez/image_processing.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     4163 2023-06-06 13:31:59.000000 moosez-2.0.4/moosez/input_validation.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     7426 2023-06-07 17:48:59.000000 moosez-2.0.4/moosez/moosez.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     6064 2023-06-07 17:45:47.000000 moosez-2.0.4/moosez/predict.py
--rw-r--r--   0 lalithsimac   (501) staff       (20)     3792 2023-06-07 17:45:47.000000 moosez-2.0.4/moosez/resources.py
-drwxr-xr-x   0 lalithsimac   (501) staff       (20)        0 2023-06-07 17:49:43.198767 moosez-2.0.4/moosez.egg-info/
--rw-r--r--   0 lalithsimac   (501) staff       (20)     1427 2023-06-07 17:49:43.000000 moosez-2.0.4/moosez.egg-info/PKG-INFO
--rw-r--r--   0 lalithsimac   (501) staff       (20)      445 2023-06-07 17:49:43.000000 moosez-2.0.4/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)        1 2023-06-07 17:49:43.000000 moosez-2.0.4/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)       47 2023-06-07 17:49:43.000000 moosez-2.0.4/moosez.egg-info/entry_points.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)      234 2023-06-07 17:49:43.000000 moosez-2.0.4/moosez.egg-info/requires.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)        7 2023-06-07 17:49:43.000000 moosez-2.0.4/moosez.egg-info/top_level.txt
--rw-r--r--   0 lalithsimac   (501) staff       (20)       38 2023-06-07 17:49:43.199993 moosez-2.0.4/setup.cfg
--rw-r--r--   0 lalithsimac   (501) staff       (20)     2207 2023-06-07 17:49:24.000000 moosez-2.0.4/setup.py
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-06-11 14:51:14.375541 moosez-2.0.5/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)    11357 2023-06-11 14:35:55.000000 moosez-2.0.5/LICENSE
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1427 2023-06-11 14:51:14.375541 moosez-2.0.5/PKG-INFO
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)    19071 2023-06-11 14:35:55.000000 moosez-2.0.5/README.md
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-06-11 14:51:14.375541 moosez-2.0.5/moosez/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      227 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/__init__.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1362 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/constants.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     5434 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/display.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     3662 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/download.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4119 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/file_utilities.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4002 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/image_conversion.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     3416 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/image_processing.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4163 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/input_validation.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     7426 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/moosez.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     6064 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/predict.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     3854 2023-06-11 14:35:55.000000 moosez-2.0.5/moosez/resources.py
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-06-11 14:51:14.375541 moosez-2.0.5/moosez.egg-info/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1427 2023-06-11 14:51:14.000000 moosez-2.0.5/moosez.egg-info/PKG-INFO
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      445 2023-06-11 14:51:14.000000 moosez-2.0.5/moosez.egg-info/SOURCES.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)        1 2023-06-11 14:51:14.000000 moosez-2.0.5/moosez.egg-info/dependency_links.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)       47 2023-06-11 14:51:14.000000 moosez-2.0.5/moosez.egg-info/entry_points.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      234 2023-06-11 14:51:14.000000 moosez-2.0.5/moosez.egg-info/requires.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)        7 2023-06-11 14:51:14.000000 moosez-2.0.5/moosez.egg-info/top_level.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)       38 2023-06-11 14:51:14.375541 moosez-2.0.5/setup.cfg
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     2207 2023-06-11 14:38:13.000000 moosez-2.0.5/setup.py
```

### Comparing `moosez-2.0.4/LICENSE` & `moosez-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/PKG-INFO` & `moosez-2.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.4
+Version: 2.0.5
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Platform: UNKNOWN
```

### Comparing `moosez-2.0.4/README.md` & `moosez-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/constants.py` & `moosez-2.0.5/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/display.py` & `moosez-2.0.5/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/download.py` & `moosez-2.0.5/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/file_utilities.py` & `moosez-2.0.5/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/image_conversion.py` & `moosez-2.0.5/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/image_processing.py` & `moosez-2.0.5/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/input_validation.py` & `moosez-2.0.5/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/moosez.py` & `moosez-2.0.5/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.4/moosez/predict.py` & `moosez-2.0.5/moosez/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     elif model_name == "clin_ct_ribs":
         return 202
     elif model_name == "clin_ct_vertebrae":
         return 203
     elif model_name == "clin_ct_muscles":
         return 204
     elif model_name == "clin_ct_lungs":
-        return 205
+        return 124
     elif model_name == "clin_ct_fat":
         return 206
     elif model_name == "clin_ct_vessels":
         return 207
     elif model_name == "clin_ct_organs":
         return 123
     elif model_name == "clin_pt_fdg_tumor":
```

### Comparing `moosez-2.0.4/moosez/resources.py` & `moosez-2.0.5/moosez/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     },
     "clin_ct_muscles": {
         "url": "https://example.com/muscles_model.zip",
         "filename": "clin_ct_muscles_model.zip",
         "directory": "clin_ct_muscles_model",
     },
     "clin_ct_lungs": {
-        "url": "https://example.com/ribs_model.zip",
-        "filename": "clin_ct_lungs_model.zip",
-        "directory": "clin_ct_lungs_model",
+        "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/HMS_3dlungs_10062023.zip",
+        "filename": "Dataset124_HMS_3dlungs.zip",
+        "directory": "Dataset124_HMS_3dlungs",
     },
     "clin_ct_fat": {
         "url": "https://example.com/fat_model.zip",
         "filename": "clin_ct_fat_model.zip",
         "directory": "clin_ct_fat_model",
     },
     "clin_ct_vessels": {
```

### Comparing `moosez-2.0.4/moosez.egg-info/PKG-INFO` & `moosez-2.0.5/moosez.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.4
+Version: 2.0.5
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Platform: UNKNOWN
```

### Comparing `moosez-2.0.4/setup.py` & `moosez-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.0.4',
+    version='2.0.5',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

