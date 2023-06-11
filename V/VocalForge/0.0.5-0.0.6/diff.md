# Comparing `tmp/VocalForge-0.0.5.tar.gz` & `tmp/VocalForge-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VocalForge-0.0.5.tar", last modified: Sun Jun 11 00:11:28 2023, max compression
+gzip compressed data, was "VocalForge-0.0.6.tar", last modified: Sun Jun 11 01:36:04 2023, max compression
```

## Comparing `VocalForge-0.0.5.tar` & `VocalForge-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.977277 VocalForge-0.0.5/
--rw-rw-r--   0 rio       (1000) rio       (1000)     1067 2023-05-21 03:39:13.000000 VocalForge-0.0.5/LICENSE.md
--rw-rw-r--   0 rio       (1000) rio       (1000)     6156 2023-06-11 00:11:28.977277 VocalForge-0.0.5/PKG-INFO
--rw-rw-r--   0 rio       (1000) rio       (1000)     5774 2023-05-21 03:39:13.000000 VocalForge-0.0.5/README.md
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.973277 VocalForge-0.0.5/VocalForge/
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.977277 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/
--rw-rw-r--   0 rio       (1000) rio       (1000)     6156 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/PKG-INFO
--rw-rw-r--   0 rio       (1000) rio       (1000)      848 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/SOURCES.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)        1 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/dependency_links.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)      279 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/requires.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)       11 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/top_level.txt
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.977277 VocalForge-0.0.5/VocalForge/audio/
--rw-rw-r--   0 rio       (1000) rio       (1000)      204 2023-05-31 00:06:05.000000 VocalForge-0.0.5/VocalForge/audio/__init__.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    11150 2023-06-06 03:10:36.000000 VocalForge-0.0.5/VocalForge/audio/audio_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     4439 2023-06-04 02:30:09.000000 VocalForge-0.0.5/VocalForge/audio/export_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     9966 2023-06-04 02:30:19.000000 VocalForge-0.0.5/VocalForge/audio/isolate.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2706 2023-06-10 23:55:14.000000 VocalForge-0.0.5/VocalForge/audio/overlap.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2386 2023-05-31 00:06:30.000000 VocalForge-0.0.5/VocalForge/audio/refine_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     3825 2023-06-10 23:51:14.000000 VocalForge-0.0.5/VocalForge/audio/voice_detection.py
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.977277 VocalForge-0.0.5/VocalForge/text/
--rw-rw-r--   0 rio       (1000) rio       (1000)      250 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/__init__.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     3555 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/create_dataset.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2211 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/ctc.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    26284 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/ctc_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1666 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/normalization_helpers.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     4247 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/normalize_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    10460 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/process_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2442 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/refine_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2277 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/segment.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1759 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/split_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     5407 2023-05-31 04:31:49.000000 VocalForge-0.0.5/VocalForge/text/text_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2330 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/transcribe.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1076 2023-06-11 00:11:24.000000 VocalForge-0.0.5/pyproject.toml
--rw-rw-r--   0 rio       (1000) rio       (1000)       38 2023-06-11 00:11:28.977277 VocalForge-0.0.5/setup.cfg
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1067 2023-05-21 03:39:13.000000 VocalForge-0.0.6/LICENSE.md
+-rw-rw-r--   0 rio       (1000) rio       (1000)     6156 2023-06-11 01:36:04.149953 VocalForge-0.0.6/PKG-INFO
+-rw-rw-r--   0 rio       (1000) rio       (1000)     5774 2023-05-21 03:39:13.000000 VocalForge-0.0.6/README.md
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/VocalForge/
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/VocalForge/audio/
+-rw-rw-r--   0 rio       (1000) rio       (1000)      204 2023-05-31 00:06:05.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/__init__.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    11150 2023-06-06 03:10:36.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/audio_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4439 2023-06-04 02:30:09.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/export_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     9966 2023-06-04 02:30:19.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/isolate.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2706 2023-06-10 23:55:14.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/overlap.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2386 2023-05-31 00:06:30.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/refine_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3825 2023-06-10 23:51:14.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/voice_detection.py
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/VocalForge/text/
+-rw-rw-r--   0 rio       (1000) rio       (1000)      250 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/__init__.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3555 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/create_dataset.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2211 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/ctc.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    26284 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/ctc_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1666 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/normalization_helpers.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4247 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/normalize_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    10460 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/process_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2442 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/refine_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2277 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/segment.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1759 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/split_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     5407 2023-05-31 04:31:49.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/text_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2330 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/transcribe.py
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/
+-rw-rw-r--   0 rio       (1000) rio       (1000)     6156 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/PKG-INFO
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1057 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/SOURCES.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)        1 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/dependency_links.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)      279 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/requires.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)       11 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/top_level.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1078 2023-06-11 01:35:43.000000 VocalForge-0.0.6/pyproject.toml
+-rw-rw-r--   0 rio       (1000) rio       (1000)       38 2023-06-11 01:36:04.149953 VocalForge-0.0.6/setup.cfg
```

### Comparing `VocalForge-0.0.5/LICENSE.md` & `VocalForge-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/PKG-INFO` & `VocalForge-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VocalForge
-Version: 0.0.5
+Version: 0.0.6
 Summary: Your one-stop solution for voice dataset creation
 Author-email: rio@rioharper.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

### Comparing `VocalForge-0.0.5/README.md` & `VocalForge-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/VocalForge.egg-info/PKG-INFO` & `VocalForge-0.0.6/VocalForge/VocalForge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VocalForge
-Version: 0.0.5
+Version: 0.0.6
 Summary: Your one-stop solution for voice dataset creation
 Author-email: rio@rioharper.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: audio
```

### Comparing `VocalForge-0.0.5/VocalForge/audio/audio_utils.py` & `VocalForge-0.0.6/VocalForge/VocalForge/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/audio/export_audio.py` & `VocalForge-0.0.6/VocalForge/VocalForge/audio/export_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/audio/isolate.py` & `VocalForge-0.0.6/VocalForge/VocalForge/audio/isolate.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/audio/overlap.py` & `VocalForge-0.0.6/VocalForge/VocalForge/audio/overlap.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/audio/refine_audio.py` & `VocalForge-0.0.6/VocalForge/VocalForge/audio/refine_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/audio/voice_detection.py` & `VocalForge-0.0.6/VocalForge/VocalForge/audio/voice_detection.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/create_dataset.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/create_dataset.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/ctc.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/ctc.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/ctc_utils.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/ctc_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/normalization_helpers.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/normalization_helpers.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/normalize_text.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/normalize_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/process_text.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/process_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/refine_text.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/refine_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/segment.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/segment.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/split_audio.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/split_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/text_utils.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/text_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/VocalForge/text/transcribe.py` & `VocalForge-0.0.6/VocalForge/VocalForge/text/transcribe.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.5/pyproject.toml` & `VocalForge-0.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "VocalForge"
-version = "0.0.5"
+version = "0.0.6"
 
 authors = [
   {email="rio@rioharper.com" },
 ]
 description = "Your one-stop solution for voice dataset creation"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -37,20 +37,20 @@
 [tool.setuptools]
 package-dir = {"" = "VocalForge"}
 
 [project.optional-dependencies]
 audio = [
         'deepfilternet',
         'pyannote.core',
-        'pyannote.audio'
+        'pyannote.audio',
+        'yt_dlp',
         ]
 
 text = [
         'ctc_segmentation',
         'nemo==4.5.5',
         'nemo_text_processing',
         'nemo_toolkit',
         'num2words==0.5.12',
         'openai_whisper',
         'whisper',
-        'yt_dlp'
 ]
```

