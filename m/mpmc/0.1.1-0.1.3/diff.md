# Comparing `tmp/mpmc-0.1.1.tar.gz` & `tmp/mpmc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpmc-0.1.1.tar", max compression
+gzip compressed data, was "mpmc-0.1.3.tar", max compression
```

## Comparing `mpmc-0.1.1.tar` & `mpmc-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-06-10 21:32:49.808401 mpmc-0.1.1/LICENSE
--rw-r--r--   0        0        0       61 2023-06-11 17:33:30.633475 mpmc-0.1.1/README.md
--rw-r--r--   0        0        0      265 2023-06-11 10:37:13.805974 mpmc-0.1.1/mpmc/__init__.py
--rw-r--r--   0        0        0     1150 2023-06-11 17:28:54.361822 mpmc-0.1.1/mpmc/broadcast.py
--rw-r--r--   0        0        0      409 2023-06-11 17:45:23.373033 mpmc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 mpmc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-10 21:32:49.808401 mpmc-0.1.3/LICENSE
+-rw-r--r--   0        0        0       61 2023-06-11 17:33:30.633475 mpmc-0.1.3/README.md
+-rw-r--r--   0        0        0      265 2023-06-11 10:37:13.805974 mpmc-0.1.3/mpmc/__init__.py
+-rw-r--r--   0        0        0     1150 2023-06-11 17:28:54.361822 mpmc-0.1.3/mpmc/broadcast.py
+-rw-r--r--   0        0        0      414 2023-06-11 17:46:02.692244 mpmc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 mpmc-0.1.3/PKG-INFO
```

### Comparing `mpmc-0.1.1/LICENSE` & `mpmc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpmc-0.1.1/mpmc/broadcast.py` & `mpmc-0.1.3/mpmc/broadcast.py`

 * *Files identical despite different names*

### Comparing `mpmc-0.1.1/PKG-INFO` & `mpmc-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mpmc
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Author: fdv1
 Author-email: francois@pytek.io
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

