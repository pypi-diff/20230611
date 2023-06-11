# Comparing `tmp/pronounspageviewer-1.0.0-py3-none-any.whl.zip` & `tmp/pronounspageviewer-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4192 bytes, number of entries: 8
+Zip file size: 4204 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     1944 b- defN 23-Jun-11 13:51 pronounspageviewer/__init__.py
 -rw-rw-rw-  2.0 fat      892 b- defN 23-Jun-11 13:51 pronounspageviewer/__main__.py
--rw-rw-rw-  2.0 fat     1714 b- defN 23-Jun-11 14:44 pronounspageviewer-1.0.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      772 b- defN 23-Jun-11 14:44 pronounspageviewer-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-11 14:44 pronounspageviewer-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       65 b- defN 23-Jun-11 14:44 pronounspageviewer-1.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-11 14:44 pronounspageviewer-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      723 b- defN 23-Jun-11 14:44 pronounspageviewer-1.0.0.dist-info/RECORD
-8 files, 6221 bytes uncompressed, 2904 bytes compressed:  53.3%
+-rw-rw-rw-  2.0 fat     1714 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      831 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       72 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      723 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/RECORD
+8 files, 6287 bytes uncompressed, 2916 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: pronounspageviewer/__init__.py
 Comment: 
 
 Filename: pronounspageviewer/__main__.py
 Comment: 
 
-Filename: pronounspageviewer-1.0.0.dist-info/LICENSE.txt
+Filename: pronounspageviewer-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pronounspageviewer-1.0.0.dist-info/METADATA
+Filename: pronounspageviewer-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pronounspageviewer-1.0.0.dist-info/WHEEL
+Filename: pronounspageviewer-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pronounspageviewer-1.0.0.dist-info/entry_points.txt
+Filename: pronounspageviewer-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pronounspageviewer-1.0.0.dist-info/top_level.txt
+Filename: pronounspageviewer-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pronounspageviewer-1.0.0.dist-info/RECORD
+Filename: pronounspageviewer-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pronounspageviewer-1.0.0.dist-info/LICENSE.txt` & `pronounspageviewer-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pronounspageviewer-1.0.0.dist-info/METADATA` & `pronounspageviewer-1.0.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: pronounspageviewer
-Version: 1.0.0
+Version: 1.0.1
 Summary: View a Pronouns.page from its JSON file
 Author: Joe Greaves
 Project-URL: Homepage, https://github.com/Grvs44/Pronouns.page-Viewer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Pronouns.page Viewer
+## Install
+```cmd
+pip install pronounspageviewer
+```
+
 ## Run
 1. Pass the file name with the `-f` argument:
     ```cmd
     pronounspageviewer -f pronouns.json
     ```
 2. Pipe the file into `pronounspageviewer` (or `python -m pronounspageviewer`).  
 An example with Git:
```

