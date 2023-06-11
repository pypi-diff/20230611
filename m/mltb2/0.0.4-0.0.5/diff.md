# Comparing `tmp/mltb2-0.0.4.tar.gz` & `tmp/mltb2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltb2-0.0.4.tar", last modified: Sat Jun 10 12:39:25 2023, max compression
+gzip compressed data, was "dist/mltb2-0.0.5.tar", last modified: Sun Jun 11 10:23:10 2023, max compression
```

## Comparing `mltb2-0.0.4.tar` & `mltb2-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:39:25.000000 mltb2-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-10 12:39:14.000000 mltb2-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-10 12:39:14.000000 mltb2-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-10 12:39:25.000000 mltb2-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-10 12:39:14.000000 mltb2-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-10 12:39:14.000000 mltb2-0.0.4/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 12:39:25.000000 mltb2-0.0.4/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-10 12:39:14.000000 mltb2-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-10 12:39:25.000000 mltb2-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-10 12:39:14.000000 mltb2-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:39:25.000000 mltb2-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-10 12:39:14.000000 mltb2-0.0.4/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:23:10.000000 mltb2-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-11 10:23:00.000000 mltb2-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 10:23:00.000000 mltb2-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-11 10:23:10.000000 mltb2-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-11 10:23:00.000000 mltb2-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-11 10:23:00.000000 mltb2-0.0.5/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 10:23:10.000000 mltb2-0.0.5/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-11 10:23:00.000000 mltb2-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-11 10:23:10.000000 mltb2-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-11 10:23:00.000000 mltb2-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:23:10.000000 mltb2-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-11 10:23:00.000000 mltb2-0.0.5/tests/test_transformers.py
```

### Comparing `mltb2-0.0.4/LICENSE` & `mltb2-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/PKG-INFO` & `mltb2-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.4
+Version: 0.0.5
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
```

### Comparing `mltb2-0.0.4/README.md` & `mltb2-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/mltb2/fasttext.py` & `mltb2-0.0.5/mltb2/fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/mltb2/files.py` & `mltb2-0.0.5/mltb2/files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/mltb2/optuna.py` & `mltb2-0.0.5/mltb2/optuna.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     :mod:`Optuna's standard pruners <optuna.pruners>` assume that you only adjust the model once
     per hyperparameter set. Those pruners work on the basis of intermediate results. For example,
     once per epoch. In contrast, this pruner does not work on intermediate results but on the
     results of a cross validation or more precisely the results of the individual folds.
 
     Below is a minimalist example:
 
-    .. code-block:: python
+    .. testcode::
 
         from mltb2.optuna import SignificanceRepeatedTrainingPruner
         import logging
         import numpy as np
         import optuna
         from sklearn.datasets import load_iris
         from sklearn.model_selection import StratifiedKFold
@@ -81,15 +81,15 @@
                 if trial.should_prune():
                     # prune here - we are done with this CV
                     break
 
             return np.mean(validation_result_list)
 
         study = optuna.create_study(
-            storage="sqlite:///optuna.db",
+            # storage="sqlite:///optuna.db",  # we use in-memory storage here
             study_name="iris_cv",
             direction="maximize",
             load_if_exists=True,
             sampler=optuna.samplers.TPESampler(multivariate=True),
             # add pruner to optuna
             pruner=SignificanceRepeatedTrainingPruner(
                 alpha=0.4,
```

### Comparing `mltb2-0.0.4/mltb2/plot.py` & `mltb2-0.0.5/mltb2/plot.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/mltb2/somajo.py` & `mltb2-0.0.5/mltb2/somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/mltb2/somajo_transformers.py` & `mltb2-0.0.5/mltb2/somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/mltb2/transformers.py` & `mltb2-0.0.5/mltb2/transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/mltb2.egg-info/PKG-INFO` & `mltb2-0.0.5/mltb2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.4
+Version: 0.0.5
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
```

### Comparing `mltb2-0.0.4/mltb2.egg-info/SOURCES.txt` & `mltb2-0.0.5/mltb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/mltb2.egg-info/requires.txt` & `mltb2-0.0.5/mltb2.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 numpy
 scipy
 tqdm
 
 [all]
-matplotlib
-mypy
-optuna
-fasttext-wheel
-pydocstyle
 myst_parser
-packaging
-transformers
-scikit-learn
-torch
-black
-pylintfileheader
+sphinx_copybutton
 flake8
-mdformat
+isort
+pylintfileheader
+fasttext-wheel
 pytest
+torch
+scikit-learn
+pylint
 sphinx
+sphinx_rtd_theme
 SoMaJo
-isort
+mypy
+black
+pydocstyle
+optuna
+mdformat
+matplotlib
+transformers
+packaging
 platformdirs
-sphinx_rtd_theme
-pylint
-sphinx_copybutton
 
 [checking]
 black
 flake8
 isort
 mdformat
 pydocstyle
```

### Comparing `mltb2-0.0.4/pyproject.toml` & `mltb2-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/setup.py` & `mltb2-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/tests/test_fasttext.py` & `mltb2-0.0.5/tests/test_fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/tests/test_files.py` & `mltb2-0.0.5/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/tests/test_optuna.py` & `mltb2-0.0.5/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/tests/test_somajo.py` & `mltb2-0.0.5/tests/test_somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/tests/test_somajo_transformers.py` & `mltb2-0.0.5/tests/test_somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.4/tests/test_transformers.py` & `mltb2-0.0.5/tests/test_transformers.py`

 * *Files identical despite different names*

