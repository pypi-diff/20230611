# Comparing `tmp/pybart-nlp-3.4.5.tar.gz` & `tmp/pybart-nlp-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybart-nlp-3.4.5.tar", last modified: Sun Jun 11 18:58:54 2023, max compression
+gzip compressed data, was "pybart-nlp-3.4.6.tar", last modified: Sun Jun 11 20:28:30 2023, max compression
```

## Comparing `pybart-nlp-3.4.5.tar` & `pybart-nlp-3.4.6.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:58:54.262149 pybart-nlp-3.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-11 18:58:54.262149 pybart-nlp-3.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:58:54.262149 pybart-nlp-3.4.5/pybart/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/pybart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/pybart/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/pybart/conllu_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/pybart/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    90095 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/pybart/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/pybart/graph_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/pybart/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/pybart/spacy_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:58:54.262149 pybart-nlp-3.4.5/pybart_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-11 18:58:54.000000 pybart-nlp-3.4.5/pybart_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-11 18:58:54.000000 pybart-nlp-3.4.5/pybart_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:58:54.000000 pybart-nlp-3.4.5/pybart_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 18:58:54.000000 pybart-nlp-3.4.5/pybart_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:58:54.262149 pybart-nlp-3.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-11 18:58:45.000000 pybart-nlp-3.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:28:30.647191 pybart-nlp-3.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-11 20:28:30.647191 pybart-nlp-3.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:28:30.647191 pybart-nlp-3.4.6/pybart/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/conllu_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:28:30.647191 pybart-nlp-3.4.6/pybart/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90095 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/graph_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/pybart/spacy_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:28:30.647191 pybart-nlp-3.4.6/pybart_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-11 20:28:30.000000 pybart-nlp-3.4.6/pybart_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-11 20:28:30.000000 pybart-nlp-3.4.6/pybart_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:28:30.000000 pybart-nlp-3.4.6/pybart_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 20:28:30.000000 pybart-nlp-3.4.6/pybart_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:28:30.647191 pybart-nlp-3.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-11 20:28:21.000000 pybart-nlp-3.4.6/setup.py
```

### Comparing `pybart-nlp-3.4.5/LICENSE` & `pybart-nlp-3.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/PKG-INFO` & `pybart-nlp-3.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybart-nlp
-Version: 3.4.5
+Version: 3.4.6
 Summary: python converter from UD-tree to BART-graph representations
 Home-page: https://github.com/allenai/pybart
 Author: Aryeh Tiktinsky
 Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.5 Summary: python converter
+Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.6 Summary: python converter
 from UD-tree to BART-graph representations Home-page: https://github.com/
 allenai/pybart Author: Aryeh Tiktinsky Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown License-File: LICENSE ![CI](https://github.com/allenai/pybart/actions/
 workflows/ci.yml/badge.svg)
```

### Comparing `pybart-nlp-3.4.5/README.md` & `pybart-nlp-3.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/pybart/api.py` & `pybart-nlp-3.4.6/pybart/api.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/pybart/conllu_wrapper.py` & `pybart-nlp-3.4.6/pybart/conllu_wrapper.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/pybart/constraints.py` & `pybart-nlp-3.4.6/pybart/constraints.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/pybart/converter.py` & `pybart-nlp-3.4.6/pybart/converter.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/pybart/graph_token.py` & `pybart-nlp-3.4.6/pybart/graph_token.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/pybart/matcher.py` & `pybart-nlp-3.4.6/pybart/matcher.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/pybart/spacy_wrapper.py` & `pybart-nlp-3.4.6/pybart/spacy_wrapper.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.5/pybart_nlp.egg-info/PKG-INFO` & `pybart-nlp-3.4.6/pybart_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybart-nlp
-Version: 3.4.5
+Version: 3.4.6
 Summary: python converter from UD-tree to BART-graph representations
 Home-page: https://github.com/allenai/pybart
 Author: Aryeh Tiktinsky
 Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.5 Summary: python converter
+Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.6 Summary: python converter
 from UD-tree to BART-graph representations Home-page: https://github.com/
 allenai/pybart Author: Aryeh Tiktinsky Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown License-File: LICENSE ![CI](https://github.com/allenai/pybart/actions/
 workflows/ci.yml/badge.svg)
```

### Comparing `pybart-nlp-3.4.5/setup.py` & `pybart-nlp-3.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybart-nlp",
-    version="3.4.5",
+    version="3.4.6",
     author="Aryeh Tiktinsky",
     author_email="aryehgigi@gmail.com",
     description="python converter from UD-tree to BART-graph representations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allenai/pybart",
     packages=setuptools.find_packages(),
```

