# Comparing `tmp/uwdtool-1.0.3.tar.gz` & `tmp/uwdtool-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwdtool-1.0.3.tar", max compression
+gzip compressed data, was "uwdtool-1.1.0.tar", max compression
```

## Comparing `uwdtool-1.0.3.tar` & `uwdtool-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2678 2023-04-22 04:09:15.499847 uwdtool-1.0.3/README.md
--rw-r--r--   0        0        0      342 2023-04-22 04:08:23.555632 uwdtool-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7459 2023-04-22 04:08:30.747662 uwdtool-1.0.3/uwdtool/UWDTool.py
--rw-r--r--   0        0        0        0 2023-04-22 03:25:18.701618 uwdtool-1.0.3/uwdtool/__init__.py
--rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 uwdtool-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2678 2023-04-22 04:09:15.499847 uwdtool-1.1.0/README.md
+-rw-r--r--   0        0        0      342 2023-06-10 14:50:26.661629 uwdtool-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7497 2023-06-10 14:50:18.941381 uwdtool-1.1.0/uwdtool/UWDTool.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:25:18.701618 uwdtool-1.1.0/uwdtool/__init__.py
+-rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 uwdtool-1.1.0/PKG-INFO
```

### Comparing `uwdtool-1.0.3/README.md` & `uwdtool-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `uwdtool-1.0.3/uwdtool/UWDTool.py` & `uwdtool-1.1.0/uwdtool/UWDTool.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import struct
 import os
 import hashlib
 from glob import glob
 from pathlib import Path
 
 
-UWDT_VERSION = "1.0.3"
+UWDT_VERSION = "1.1.0"
 HELP_STR = f"""UWDTool v{UWDT_VERSION}"""
 
 
 class UWDTException(Exception):
     def __init__(self, msg):
         self.msg = msg
 
@@ -96,17 +96,17 @@
         print(f"Pack files in {self.input_path} to {self.output_path}")
 
         files = [y for x in os.walk(self.input_path) for y in glob(os.path.join(x[0], '*'))]
         targets_ = [x for x in files if os.path.isfile(x)]
         targets = []
         for target in targets_:
             if self.input_path.endswith("/"):
-                targets.append(target[len(self.input_path):])
+                targets.append(target[len(self.input_path):].replace("\\", "/"))
             else:
-                targets.append(target[len(self.input_path)+1:])
+                targets.append(target[len(self.input_path)+1:].replace("\\", "/"))
 
         OUTPUT = open(self.output_path, "wb")
 
         OUTPUT.write(bytes("UnityWebData1.0\0", "utf-8"))
 
         header_length = 0
         for file_name in targets:
```

### Comparing `uwdtool-1.0.3/PKG-INFO` & `uwdtool-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwdtool
-Version: 1.0.3
+Version: 1.1.0
 Summary: The tool to pack and unpack UnityWebData files
 Author: yuria0309
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

