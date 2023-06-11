# Comparing `tmp/xia_gpt_openai-0.0.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_gpt_openai-0.0.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 110803 bytes, number of entries: 7
--rw-r--r--  2.0 unx       95 b- defN 23-May-16 07:11 xia_gpt_openai/__init__.py
--rw-r--r--  2.0 unx   261632 b- defN 23-Jun-07 18:38 xia_gpt_openai/gpt.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      150 b- defN 23-Jun-07 18:38 xia_gpt_openai-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      673 b- defN 23-Jun-07 18:38 xia_gpt_openai-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-07 18:38 xia_gpt_openai-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-07 18:38 xia_gpt_openai-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      600 b- defN 23-Jun-07 18:38 xia_gpt_openai-0.0.1.dist-info/RECORD
-7 files, 263264 bytes uncompressed, 109727 bytes compressed:  58.3%
+Zip file size: 110771 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-11 05:36 xia_gpt_openai/__init__.py
+-rw-r--r--  2.0 unx   261632 b- defN 23-Jun-11 05:39 xia_gpt_openai/gpt.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      150 b- defN 23-Jun-11 05:39 xia_gpt_openai-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      673 b- defN 23-Jun-11 05:39 xia_gpt_openai-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-11 05:39 xia_gpt_openai-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-11 05:39 xia_gpt_openai-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      600 b- defN 23-Jun-11 05:39 xia_gpt_openai-0.0.2.dist-info/RECORD
+7 files, 263264 bytes uncompressed, 109695 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_gpt_openai/__init__.py
 Comment: 
 
 Filename: xia_gpt_openai/gpt.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_gpt_openai-0.0.1.dist-info/LICENSE.txt
+Filename: xia_gpt_openai-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.0.1.dist-info/METADATA
+Filename: xia_gpt_openai-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_gpt_openai-0.0.1.dist-info/WHEEL
+Filename: xia_gpt_openai-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_gpt_openai-0.0.1.dist-info/top_level.txt
+Filename: xia_gpt_openai-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.0.1.dist-info/RECORD
+Filename: xia_gpt_openai-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_gpt_openai/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_gpt_openai.gpt import OpenaiGpt
 
 __all__ = [
     "OpenaiGpt"
 ]
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## Comparing `xia_gpt_openai-0.0.1.dist-info/METADATA` & `xia_gpt_openai-0.0.2.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-gpt-openai
-Version: 0.0.1
+Version: 0.0.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-gpt-openai/0.0.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-gpt-openai/0.0.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

