# Comparing `tmp/peitho_data-2.2.0.tar.gz` & `tmp/peitho_data-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.2.0.tar", last modified: Tue May  9 09:51:19 2023, max compression
+gzip compressed data, was "peitho_data-2.2.1.tar", last modified: Sun Jun 11 02:55:46 2023, max compression
```

## Comparing `peitho_data-2.2.0.tar` & `peitho_data-2.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.975470 peitho_data-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 09:51:18.000000 peitho_data-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 09:51:18.000000 peitho_data-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-09 09:51:19.975470 peitho_data-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-09 09:51:18.000000 peitho_data-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/datafication/epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/graph/knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/graph/visualization/file_based_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/machine_learning/concept_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/tests/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/datafication/test_epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/tests/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/graph/test_knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/tests/graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/graph/visualization/test_file_based_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.975470 peitho_data-2.2.0/peitho_data/tests/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/machine_learning/test_concept_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/test_trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/test_word_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 09:51:19.975470 peitho_data-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-09 09:51:18.000000 peitho_data-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.760044 peitho_data-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 02:53:48.000000 peitho_data-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 02:53:48.000000 peitho_data-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-11 02:55:46.760044 peitho_data-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-11 02:53:48.000000 peitho_data-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.752044 peitho_data-2.2.1/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/datafication/epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/graph/knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/graph/visualization/file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/machine_learning/concept_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/tests/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/datafication/test_epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/tests/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/graph/test_knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.760044 peitho_data-2.2.1/peitho_data/tests/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/graph/visualization/test_file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.760044 peitho_data-2.2.1/peitho_data/tests/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/machine_learning/test_concept_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/test_trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/test_word_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:54:09.000000 peitho_data-2.2.1/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-11 02:55:46.760044 peitho_data-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-11 02:53:48.000000 peitho_data-2.2.1/setup.py
```

### Comparing `peitho_data-2.2.0/LICENSE` & `peitho_data-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/README.md` & `peitho_data-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.2.1/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/datafication/epub.py` & `peitho_data-2.2.1/peitho_data/datafication/epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/graph/knowledge_graph_spec.py` & `peitho_data-2.2.1/peitho_data/graph/knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/graph/visualization/file_based_visualization.py` & `peitho_data-2.2.1/peitho_data/graph/visualization/file_based_visualization.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/machine_learning/concept_learning.py` & `peitho_data-2.2.1/peitho_data/machine_learning/concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/tests/graph/test_knowledge_graph_spec.py` & `peitho_data-2.2.1/peitho_data/tests/graph/test_knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/tests/machine_learning/test_concept_learning.py` & `peitho_data-2.2.1/peitho_data/tests/machine_learning/test_concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/tests/test_trello_api.py` & `peitho_data-2.2.1/peitho_data/tests/test_trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/tests/test_word_cloud.py` & `peitho_data-2.2.1/peitho_data/tests/test_word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/trello_api.py` & `peitho_data-2.2.1/peitho_data/trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data/word_cloud.py` & `peitho_data-2.2.1/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/peitho_data.egg-info/SOURCES.txt` & `peitho_data-2.2.1/peitho_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.0/setup.py` & `peitho_data-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="peitho_data",
-    version="2.2.0",
+    version="2.2.1",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

