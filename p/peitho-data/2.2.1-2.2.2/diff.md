# Comparing `tmp/peitho_data-2.2.1.tar.gz` & `tmp/peitho_data-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.2.1.tar", last modified: Sun Jun 11 02:55:46 2023, max compression
+gzip compressed data, was "peitho_data-2.2.2.tar", last modified: Sun Jun 11 06:15:12 2023, max compression
```

## Comparing `peitho_data-2.2.1.tar` & `peitho_data-2.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.760044 peitho_data-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 02:53:48.000000 peitho_data-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 02:53:48.000000 peitho_data-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-11 02:55:46.760044 peitho_data-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-11 02:53:48.000000 peitho_data-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.752044 peitho_data-2.2.1/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/datafication/epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/graph/knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/graph/visualization/file_based_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/machine_learning/concept_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/tests/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/datafication/test_epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data/tests/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/graph/test_knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.760044 peitho_data-2.2.1/peitho_data/tests/graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/graph/visualization/test_file_based_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.760044 peitho_data-2.2.1/peitho_data/tests/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/machine_learning/test_concept_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/test_trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/tests/test_word_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-11 02:53:48.000000 peitho_data-2.2.1/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:55:46.756044 peitho_data-2.2.1/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:54:09.000000 peitho_data-2.2.1/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 02:55:46.000000 peitho_data-2.2.1/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-11 02:55:46.760044 peitho_data-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-11 02:53:48.000000 peitho_data-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.826266 peitho_data-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 06:12:38.000000 peitho_data-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 06:12:38.000000 peitho_data-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-11 06:15:12.826266 peitho_data-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-11 06:12:38.000000 peitho_data-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/datafication/epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/graph/knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/graph/visualization/file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/machine_learning/concept_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/tests/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/datafication/test_epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.826266 peitho_data-2.2.2/peitho_data/tests/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/graph/test_knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.826266 peitho_data-2.2.2/peitho_data/tests/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/graph/visualization/test_file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.826266 peitho_data-2.2.2/peitho_data/tests/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/machine_learning/test_concept_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/test_trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/test_word_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 06:13:08.000000 peitho_data-2.2.2/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-11 06:15:12.826266 peitho_data-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-11 06:12:38.000000 peitho_data-2.2.2/setup.py
```

### Comparing `peitho_data-2.2.1/LICENSE` & `peitho_data-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/README.md` & `peitho_data-2.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 </a>
 
 <br>
 <br>
 
 [![PyPI](https://img.shields.io/pypi/v/peitho-data?logo=pypi&logoColor=white&style=for-the-badge)](https://pypi.org/project/peitho-data/)
 [![Read the Docs (version)](https://img.shields.io/readthedocs/peitho-data/latest?logo=Read%20the%20Docs&logoColor=white&style=for-the-badge)](https://peitho-data.readthedocs.io/en/latest/)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/QubitPi/peitho-data/release.yml?logo=github&style=for-the-badge)](https://github.com/QubitPi/peitho-data/actions/workflows/release.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/QubitPi/peitho-data/ci-cd.yml?logo=github&style=for-the-badge)](https://github.com/QubitPi/peitho-data/actions/workflows/ci-cd.yml)
 
 [![Discord](https://img.shields.io/discord/1005754525942030366?logo=discord&logoColor=white&style=for-the-badge)](https://discord.com/widget?id=1005754525942030366&theme=dark)
-[![Project Management](https://img.shields.io/badge/Project%20Management-0052CC?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/b/ersqV9rd)
 [![License Badge](https://img.shields.io/badge/Apache%202.0-F25910.svg?style=for-the-badge&logo=Apache&logoColor=white)](https://www.apache.org/licenses/LICENSE-2.0)
-![GitHub last commit (branch)](https://img.shields.io/github/last-commit/QubitPi/peitho-data/master?logo=github&style=for-the-badge)
+![GitHub last commit (master)](https://img.shields.io/github/last-commit/QubitPi/peitho-data/master?logo=github&style=for-the-badge)
 
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=bugs)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
@@ -63,11 +62,10 @@
 -------
 
 The use and distribution terms for [Peitho Data](https://qubitpi.github.io/peitho-data/) are covered by the
 [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
 
 <div align="center">
     <a href="https://opensource.org/licenses">
-        <img align="center" width="50%" alt="License Illustration" src="https://user-images.githubusercontent.com/16126939/186319317-601c8d28-84dd-4e24-ab56-881ddd7933b5.png">
+        <img align="center" width="50%" alt="License Illustration" src="https://github.com/QubitPi/QubitPi/blob/master/img/apache-2.png?raw=true">
     </a>
 </div>
-
```

#### html2text {}

```diff
@@ -2,26 +2,24 @@
                     never-ending_focus_on_data_in_general
 
                 [![PyPI](https://img.shields.io/pypi/v/peitho-
 data?logo=pypi&logoColor=white&style=for-the-badge)](https://pypi.org/project/
  peitho-data/) [![Read the Docs (version)](https://img.shields.io/readthedocs/
 peitho-data/latest?logo=Read%20the%20Docs&logoColor=white&style=for-the-badge)]
   (https://peitho-data.readthedocs.io/en/latest/) [![GitHub Workflow Status]
-  (https://img.shields.io/github/actions/workflow/status/QubitPi/peitho-data/
-   release.yml?logo=github&style=for-the-badge)](https://github.com/QubitPi/
-peitho-data/actions/workflows/release.yml) [![Discord](https://img.shields.io/
-discord/1005754525942030366?logo=discord&logoColor=white&style=for-the-badge)]
-   (https://discord.com/widget?id=1005754525942030366&theme=dark) [![Project
-Management](https://img.shields.io/badge/Project%20Management-0052CC?style=for-
-   the-badge&logo=trello&logoColor=white)](https://trello.com/b/ersqV9rd) [!
-[License Badge](https://img.shields.io/badge/Apache%202.0-F25910.svg?style=for-
-   the-badge&logo=Apache&logoColor=white)](https://www.apache.org/licenses/
-LICENSE-2.0) ![GitHub last commit (branch)](https://img.shields.io/github/last-
-  commit/QubitPi/peitho-data/master?logo=github&style=for-the-badge) [![Bugs]
-   (https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-
+(https://img.shields.io/github/actions/workflow/status/QubitPi/peitho-data/ci-
+  cd.yml?logo=github&style=for-the-badge)](https://github.com/QubitPi/peitho-
+ data/actions/workflows/ci-cd.yml) [![Discord](https://img.shields.io/discord/
+1005754525942030366?logo=discord&logoColor=white&style=for-the-badge)](https://
+discord.com/widget?id=1005754525942030366&theme=dark) [![License Badge](https:/
+         /img.shields.io/badge/Apache%202.0-F25910.svg?style=for-the-
+ badge&logo=Apache&logoColor=white)](https://www.apache.org/licenses/LICENSE-
+2.0) ![GitHub last commit (master)](https://img.shields.io/github/last-commit/
+ QubitPi/peitho-data/master?logo=github&style=for-the-badge) [![Bugs](https://
+       sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-
  data&metric=bugs)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-
       data) [![Vulnerabilities](https://sonarcloud.io/api/project_badges/
      measure?project=QubitPi_peitho-data&metric=vulnerabilities)](https://
 sonarcloud.io/summary/new_code?id=QubitPi_peitho-data) [![Duplicated Lines (%)]
    (https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-
      data&metric=duplicated_lines_density)](https://sonarcloud.io/summary/
 new_code?id=QubitPi_peitho-data) [![Reliability Rating](https://sonarcloud.io/
```

### Comparing `peitho_data-2.2.1/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.2.2/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/datafication/epub.py` & `peitho_data-2.2.2/peitho_data/datafication/epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/graph/knowledge_graph_spec.py` & `peitho_data-2.2.2/peitho_data/graph/knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/graph/visualization/file_based_visualization.py` & `peitho_data-2.2.2/peitho_data/graph/visualization/file_based_visualization.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/machine_learning/concept_learning.py` & `peitho_data-2.2.2/peitho_data/machine_learning/concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/tests/graph/test_knowledge_graph_spec.py` & `peitho_data-2.2.2/peitho_data/tests/graph/test_knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/tests/machine_learning/test_concept_learning.py` & `peitho_data-2.2.2/peitho_data/tests/machine_learning/test_concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/tests/test_trello_api.py` & `peitho_data-2.2.2/peitho_data/tests/test_trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/tests/test_word_cloud.py` & `peitho_data-2.2.2/peitho_data/tests/test_word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/trello_api.py` & `peitho_data-2.2.2/peitho_data/trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data/word_cloud.py` & `peitho_data-2.2.2/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/peitho_data.egg-info/SOURCES.txt` & `peitho_data-2.2.2/peitho_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.1/setup.py` & `peitho_data-2.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="peitho_data",
-    version="2.2.1",
+    version="2.2.2",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

