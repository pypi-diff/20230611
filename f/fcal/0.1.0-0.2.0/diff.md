# Comparing `tmp/fcal-0.1.0.tar.gz` & `tmp/fcal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcal-0.1.0.tar", max compression
+gzip compressed data, was "fcal-0.2.0.tar", max compression
```

## Comparing `fcal-0.1.0.tar` & `fcal-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       43 2023-06-11 15:23:38.446405 fcal-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-11 15:22:00.251495 fcal-0.1.0/fcal/__init__.py
--rw-r--r--   0        0        0     1169 2023-06-11 14:49:04.675259 fcal-0.1.0/fcal/main.py
--rw-r--r--   0        0        0      356 2023-06-11 15:23:51.776574 fcal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 fcal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-06-11 15:23:38.446405 fcal-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 15:22:00.251495 fcal-0.2.0/fcal/__init__.py
+-rw-r--r--   0        0        0     1169 2023-06-11 14:49:04.675259 fcal-0.2.0/fcal/main.py
+-rw-r--r--   0        0        0      355 2023-06-11 15:34:30.422316 fcal-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 fcal-0.2.0/PKG-INFO
```

### Comparing `fcal-0.1.0/fcal/main.py` & `fcal-0.2.0/fcal/main.py`

 * *Files identical despite different names*

### Comparing `fcal-0.1.0/PKG-INFO` & `fcal-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcal
-Version: 0.1.0
+Version: 0.2.0
 Summary: display days before/after today
 License: MIT
 Author: suman chapai
 Author-email: sumanchapai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

