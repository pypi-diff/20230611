# Comparing `tmp/templateMF-0.1.tar.gz` & `tmp/templateMF-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templateMF-0.1.tar", last modified: Fri Jun  9 00:42:45 2023, max compression
+gzip compressed data, was "templateMF-0.2.tar", last modified: Sun Jun 11 17:45:37 2023, max compression
```

## Comparing `templateMF-0.1.tar` & `templateMF-0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2023-06-09 00:20:06.809841 templateMF-0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-06-09 00:30:37.369841 templateMF-0.1/README.md
--rw-r--r--   0        0        0      453 2023-06-09 00:23:27.609841 templateMF-0.1/pyproject.toml
--rw-r--r--   0        0        0     7972 2023-06-09 00:28:54.209841 templateMF-0.1/template.py
--rw-r--r--   0        0        0     7972 2023-06-09 00:31:26.499841 templateMF-0.1/templateMF/__init__.py
--rw-r--r--   0        0        0      816 2023-06-09 00:20:59.909841 templateMF-0.1/templateMF/exemplo.txt
--rw-r--r--   0        0        0        0 2023-06-09 00:31:41.599841 templateMF-0.1/templateMF/templateMF.md
--rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 templateMF-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 00:20:06.809841 templateMF-0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-09 00:30:37.369841 templateMF-0.2/README.md
+-rw-r--r--   0        0        0      448 2023-06-10 17:02:44.611563 templateMF-0.2/pyproject.toml
+-rw-r--r--   0        0        0     7972 2023-06-09 00:28:54.209841 templateMF-0.2/template.py
+-rw-r--r--   0        0        0     7972 2023-06-10 17:02:52.161563 templateMF-0.2/templateMF/__init__.py
+-rw-r--r--   0        0        0      816 2023-06-09 00:20:59.909841 templateMF-0.2/templateMF/exemplo.txt
+-rw-r--r--   0        0        0        0 2023-06-09 00:31:41.599841 templateMF-0.2/templateMF/templateMF.md
+-rw-r--r--   0        0        0      257 1970-01-01 00:00:00.000000 templateMF-0.2/PKG-INFO
```

### Comparing `templateMF-0.1/LICENSE` & `templateMF-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `templateMF-0.1/template.py` & `templateMF-0.2/template.py`

 * *Files identical despite different names*

### Comparing `templateMF-0.1/templateMF/__init__.py` & `templateMF-0.2/templateMF/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """An amazing flit templates package!"""
-__version__ = "0.1"
+__version__ = "0.2"
 
 import argparse
 import re
 import os
 
 input_file = ''
 project=''
```

### Comparing `templateMF-0.1/templateMF/exemplo.txt` & `templateMF-0.2/templateMF/exemplo.txt`

 * *Files identical despite different names*

