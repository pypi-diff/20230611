# Comparing `tmp/blip-ci-0.0.4.tar.gz` & `tmp/blip-ci-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blip-ci-0.0.4.tar", last modified: Sat Jun 10 16:07:37 2023, max compression
+gzip compressed data, was "blip-ci-0.0.5.tar", last modified: Sun Jun 11 16:45:55 2023, max compression
```

## Comparing `blip-ci-0.0.4.tar` & `blip-ci-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.602746 blip-ci-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-10 16:07:28.000000 blip-ci-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-10 16:07:28.000000 blip-ci-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-10 16:07:37.602746 blip-ci-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-06-10 16:07:28.000000 blip-ci-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.598746 blip-ci-0.0.4/blip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.598746 blip-ci-0.0.4/blip/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/bert_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/caption_coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/med_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/nlvr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/nocaps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/pretrain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/retrieval_coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/retrieval_flickr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/retrieval_msrvtt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/configs/vqa.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.602746 blip-ci-0.0.4/blip/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/coco_karpathy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/flickr30k_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/nlvr_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/nocaps_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/pretrain_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/data/vqa_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.602746 blip-ci-0.0.4/blip/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_itm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_nlvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/blip_vqa.py
--rw-r--r--   0 runner    (1001) docker     (123)    41786 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    36738 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/nlvr_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-10 16:07:28.000000 blip-ci-0.0.4/blip/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:07:37.602746 blip-ci-0.0.4/blip_ci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 16:07:37.000000 blip-ci-0.0.4/blip_ci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 16:07:28.000000 blip-ci-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 16:07:28.000000 blip-ci-0.0.4/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-10 16:07:28.000000 blip-ci-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:07:37.602746 blip-ci-0.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1486 2023-06-10 16:07:28.000000 blip-ci-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:45:55.828553 blip-ci-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-11 16:45:46.000000 blip-ci-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-11 16:45:46.000000 blip-ci-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-11 16:45:55.828553 blip-ci-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-06-11 16:45:46.000000 blip-ci-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:45:55.824553 blip-ci-0.0.5/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:45:55.824553 blip-ci-0.0.5/blip/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/bert_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/caption_coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/nlvr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/nocaps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/pretrain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/retrieval_coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/retrieval_flickr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/retrieval_msrvtt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/configs/vqa.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:45:55.824553 blip-ci-0.0.5/blip/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/coco_karpathy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/flickr30k_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/nlvr_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/nocaps_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/pretrain_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/data/vqa_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:45:55.828553 blip-ci-0.0.5/blip/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/blip_itm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/blip_nlvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/blip_pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/blip_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/blip_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41786 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36738 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/nlvr_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-11 16:45:46.000000 blip-ci-0.0.5/blip/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:45:55.828553 blip-ci-0.0.5/blip_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-11 16:45:55.000000 blip-ci-0.0.5/blip_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-11 16:45:55.000000 blip-ci-0.0.5/blip_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:45:55.000000 blip-ci-0.0.5/blip_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-11 16:45:55.000000 blip-ci-0.0.5/blip_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 16:45:55.000000 blip-ci-0.0.5/blip_ci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-11 16:45:46.000000 blip-ci-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 16:45:46.000000 blip-ci-0.0.5/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-06-11 16:45:46.000000 blip-ci-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 16:45:55.828553 blip-ci-0.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1486 2023-06-11 16:45:46.000000 blip-ci-0.0.5/setup.py
```

### Comparing `blip-ci-0.0.4/LICENSE.txt` & `blip-ci-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/PKG-INFO` & `blip-ci-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blip-ci
-Version: 0.0.4
+Version: 0.0.5
 Summary: BLIP library for use with CLIP Interrogator
 Home-page: https://github.com/pharmapsychotic/BLIP
 Author: salesforce
 Author-email: 
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blip-ci Version: 0.0.4 Summary: BLIP library for
+Metadata-Version: 2.1 Name: blip-ci Version: 0.0.5 Summary: BLIP library for
 use with CLIP Interrogator Home-page: https://github.com/pharmapsychotic/BLIP
 Author: salesforce Author-email: License: BSD-3 Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 2 - Pre-Alpha Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: dev Provides-Extra: all License-File: LICENSE.txt ## BLIP:
 Bootstrapping Language-Image Pre-training for Unified Vision-Language
```

### Comparing `blip-ci-0.0.4/README.md` & `blip-ci-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/configs/caption_coco.yaml` & `blip-ci-0.0.5/blip/configs/caption_coco.yaml`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/configs/retrieval_coco.yaml` & `blip-ci-0.0.5/blip/configs/retrieval_coco.yaml`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/configs/retrieval_flickr.yaml` & `blip-ci-0.0.5/blip/configs/retrieval_flickr.yaml`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/configs/vqa.yaml` & `blip-ci-0.0.5/blip/configs/vqa.yaml`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/__init__.py` & `blip-ci-0.0.5/blip/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/coco_karpathy_dataset.py` & `blip-ci-0.0.5/blip/data/coco_karpathy_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/flickr30k_dataset.py` & `blip-ci-0.0.5/blip/data/flickr30k_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/nlvr_dataset.py` & `blip-ci-0.0.5/blip/data/nlvr_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/nocaps_dataset.py` & `blip-ci-0.0.5/blip/data/nocaps_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/pretrain_dataset.py` & `blip-ci-0.0.5/blip/data/pretrain_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/utils.py` & `blip-ci-0.0.5/blip/data/utils.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/video_dataset.py` & `blip-ci-0.0.5/blip/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/data/vqa_dataset.py` & `blip-ci-0.0.5/blip/data/vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/blip.py` & `blip-ci-0.0.5/blip/models/blip.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/blip_itm.py` & `blip-ci-0.0.5/blip/models/blip_itm.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/blip_nlvr.py` & `blip-ci-0.0.5/blip/models/blip_nlvr.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/blip_pretrain.py` & `blip-ci-0.0.5/blip/models/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/blip_retrieval.py` & `blip-ci-0.0.5/blip/models/blip_retrieval.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/blip_vqa.py` & `blip-ci-0.0.5/blip/models/blip_vqa.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/med.py` & `blip-ci-0.0.5/blip/models/med.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/nlvr_encoder.py` & `blip-ci-0.0.5/blip/models/nlvr_encoder.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip/models/vit.py` & `blip-ci-0.0.5/blip/models/vit.py`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/blip_ci.egg-info/PKG-INFO` & `blip-ci-0.0.5/blip_ci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blip-ci
-Version: 0.0.4
+Version: 0.0.5
 Summary: BLIP library for use with CLIP Interrogator
 Home-page: https://github.com/pharmapsychotic/BLIP
 Author: salesforce
 Author-email: 
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blip-ci Version: 0.0.4 Summary: BLIP library for
+Metadata-Version: 2.1 Name: blip-ci Version: 0.0.5 Summary: BLIP library for
 use with CLIP Interrogator Home-page: https://github.com/pharmapsychotic/BLIP
 Author: salesforce Author-email: License: BSD-3 Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 2 - Pre-Alpha Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: dev Provides-Extra: all License-File: LICENSE.txt ## BLIP:
 Bootstrapping Language-Image Pre-training for Unified Vision-Language
```

### Comparing `blip-ci-0.0.4/blip_ci.egg-info/SOURCES.txt` & `blip-ci-0.0.5/blip_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blip-ci-0.0.4/setup.py` & `blip-ci-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         DEVELOPMENT_MODULES = [line.strip()
                                for line in file if "-e" not in line]
     extras = {"dev": DEVELOPMENT_MODULES}
     extras["all"] = [item for group in extras.values() for item in group]
 
     setup(
         name="blip-ci",
-        version="0.0.4",
+        version="0.0.5",
         license="BSD-3",
         author="salesforce",
         author_email="",
         url="https://github.com/pharmapsychotic/BLIP",
         description="BLIP library for use with CLIP Interrogator",
         long_description=open('README.md', encoding="utf8").read(),
         long_description_content_type="text/markdown",
```

