# Comparing `tmp/tryangle-0.2.2.tar.gz` & `tmp/tryangle-0.2.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryangle-0.2.2.tar", last modified: Sun Jun 11 18:00:51 2023, max compression
+gzip compressed data, was "tryangle-0.2.2.dev0.tar", last modified: Sun Jun 11 17:56:33 2023, max compression
```

## Comparing `tryangle-0.2.2.tar` & `tryangle-0.2.2.dev0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.497604 tryangle-0.2.2/
--rw-r--r--   0 cb        (1000) cb        (1000)    16724 2023-06-10 18:49:01.000000 tryangle-0.2.2/LICENSE
--rw-r--r--   0 cb        (1000) cb        (1000)      336 2023-06-10 18:49:01.000000 tryangle-0.2.2/MANIFEST.in
--rw-r--r--   0 cb        (1000) cb        (1000)     3143 2023-06-11 18:00:51.497604 tryangle-0.2.2/PKG-INFO
--rw-r--r--   0 cb        (1000) cb        (1000)     2385 2023-06-10 19:52:36.000000 tryangle-0.2.2/README.md
--rw-r--r--   0 cb        (1000) cb        (1000)      986 2023-06-11 18:00:30.000000 tryangle-0.2.2/pyproject.toml
--rw-r--r--   0 cb        (1000) cb        (1000)     1355 2023-06-11 17:32:19.000000 tryangle-0.2.2/requirements.txt
--rw-r--r--   0 cb        (1000) cb        (1000)       38 2023-06-11 18:00:51.497604 tryangle-0.2.2/setup.cfg
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.487604 tryangle-0.2.2/src/
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.487604 tryangle-0.2.2/src/tryangle/
--rw-r--r--   0 cb        (1000) cb        (1000)      325 2023-06-11 18:00:32.000000 tryangle-0.2.2/src/tryangle/__init__.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.487604 tryangle-0.2.2/src/tryangle/core/
--rw-r--r--   0 cb        (1000) cb        (1000)      581 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/core/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     2146 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/core/base.py
--rw-r--r--   0 cb        (1000) cb        (1000)     5435 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/core/methods.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.497604 tryangle-0.2.2/src/tryangle/ensemble/
--rw-r--r--   0 cb        (1000) cb        (1000)      596 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/ensemble/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)    16047 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/ensemble/base.py
--rw-r--r--   0 cb        (1000) cb        (1000)      810 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/ensemble/losses.py
--rw-r--r--   0 cb        (1000) cb        (1000)     8055 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/ensemble/optimizers.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.497604 tryangle-0.2.2/src/tryangle/metrics/
--rw-r--r--   0 cb        (1000) cb        (1000)      536 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/metrics/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     1362 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/metrics/base.py
--rw-r--r--   0 cb        (1000) cb        (1000)     2946 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/metrics/score.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.497604 tryangle-0.2.2/src/tryangle/model_selection/
--rw-r--r--   0 cb        (1000) cb        (1000)      391 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/model_selection/__init__.py
--rw-r--r--   0 cb        (1000) cb        (1000)     1543 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/model_selection/split.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.497604 tryangle-0.2.2/src/tryangle/utils/
--rw-r--r--   0 cb        (1000) cb        (1000)      272 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/utils/__init__.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.497604 tryangle-0.2.2/src/tryangle/utils/data/
--rw-r--r--   0 cb        (1000) cb        (1000)     8161 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/utils/data/cas_test.csv
--rw-r--r--   0 cb        (1000) cb        (1000)     9943 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/utils/data/cas_train.csv
--rw-r--r--   0 cb        (1000) cb        (1000)     8177 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/utils/data/sme_test.csv
--rw-r--r--   0 cb        (1000) cb        (1000)    10159 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/utils/data/sme_train.csv
--rw-r--r--   0 cb        (1000) cb        (1000)     8082 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/utils/data/swiss_test.csv
--rw-r--r--   0 cb        (1000) cb        (1000)     4602 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/utils/data/swiss_train.csv
--rw-r--r--   0 cb        (1000) cb        (1000)     2521 2023-06-10 18:49:01.000000 tryangle-0.2.2/src/tryangle/utils/datasets.py
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.487604 tryangle-0.2.2/src/tryangle.egg-info/
--rw-r--r--   0 cb        (1000) cb        (1000)     3143 2023-06-11 18:00:51.000000 tryangle-0.2.2/src/tryangle.egg-info/PKG-INFO
--rw-r--r--   0 cb        (1000) cb        (1000)     1052 2023-06-11 18:00:51.000000 tryangle-0.2.2/src/tryangle.egg-info/SOURCES.txt
--rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-06-11 18:00:51.000000 tryangle-0.2.2/src/tryangle.egg-info/dependency_links.txt
--rw-r--r--   0 cb        (1000) cb        (1000)       89 2023-06-11 18:00:51.000000 tryangle-0.2.2/src/tryangle.egg-info/requires.txt
--rw-r--r--   0 cb        (1000) cb        (1000)        9 2023-06-11 18:00:51.000000 tryangle-0.2.2/src/tryangle.egg-info/top_level.txt
-drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 18:00:51.497604 tryangle-0.2.2/tests/
--rw-r--r--   0 cb        (1000) cb        (1000)     1610 2023-06-10 18:49:01.000000 tryangle-0.2.2/tests/test_datasets.py
--rw-r--r--   0 cb        (1000) cb        (1000)     2714 2023-06-10 18:49:01.000000 tryangle-0.2.2/tests/test_ensemble.py
--rw-r--r--   0 cb        (1000) cb        (1000)     1853 2023-06-10 18:49:01.000000 tryangle-0.2.2/tests/test_methods.py
--rw-r--r--   0 cb        (1000) cb        (1000)      876 2023-06-10 18:49:01.000000 tryangle-0.2.2/tests/test_score.py
--rw-r--r--   0 cb        (1000) cb        (1000)     1444 2023-06-10 18:49:01.000000 tryangle-0.2.2/tests/test_split.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/
+-rw-r--r--   0 cb        (1000) cb        (1000)    16724 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/LICENSE
+-rw-r--r--   0 cb        (1000) cb        (1000)      336 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/MANIFEST.in
+-rw-r--r--   0 cb        (1000) cb        (1000)     3148 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/PKG-INFO
+-rw-r--r--   0 cb        (1000) cb        (1000)     2385 2023-06-10 19:52:36.000000 tryangle-0.2.2.dev0/README.md
+-rw-r--r--   0 cb        (1000) cb        (1000)      991 2023-06-11 17:56:21.000000 tryangle-0.2.2.dev0/pyproject.toml
+-rw-r--r--   0 cb        (1000) cb        (1000)     1355 2023-06-11 17:32:19.000000 tryangle-0.2.2.dev0/requirements.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)       38 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/setup.cfg
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.037664 tryangle-0.2.2.dev0/src/
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.037664 tryangle-0.2.2.dev0/src/tryangle/
+-rw-r--r--   0 cb        (1000) cb        (1000)      330 2023-06-11 17:56:26.000000 tryangle-0.2.2.dev0/src/tryangle/__init__.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/core/
+-rw-r--r--   0 cb        (1000) cb        (1000)      581 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/core/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     2146 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/core/base.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     5435 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/core/methods.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/ensemble/
+-rw-r--r--   0 cb        (1000) cb        (1000)      596 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/ensemble/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)    16047 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/ensemble/base.py
+-rw-r--r--   0 cb        (1000) cb        (1000)      810 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/ensemble/losses.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     8055 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/ensemble/optimizers.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/metrics/
+-rw-r--r--   0 cb        (1000) cb        (1000)      536 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/metrics/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1362 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/metrics/base.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     2946 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/metrics/score.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/model_selection/
+-rw-r--r--   0 cb        (1000) cb        (1000)      391 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/model_selection/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1543 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/model_selection/split.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/utils/
+-rw-r--r--   0 cb        (1000) cb        (1000)      272 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/__init__.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/utils/data/
+-rw-r--r--   0 cb        (1000) cb        (1000)     8161 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/cas_test.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     9943 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/cas_train.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     8177 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/sme_test.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)    10159 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/sme_train.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     8082 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/swiss_test.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     4602 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/swiss_train.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     2521 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/datasets.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle.egg-info/
+-rw-r--r--   0 cb        (1000) cb        (1000)     3148 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/PKG-INFO
+-rw-r--r--   0 cb        (1000) cb        (1000)     1052 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/SOURCES.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/dependency_links.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)       89 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/requires.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        9 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/top_level.txt
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/tests/
+-rw-r--r--   0 cb        (1000) cb        (1000)     1610 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_datasets.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     2714 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_ensemble.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1853 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_methods.py
+-rw-r--r--   0 cb        (1000) cb        (1000)      876 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_score.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1444 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_split.py
```

### Comparing `tryangle-0.2.2/LICENSE` & `tryangle-0.2.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/PKG-INFO` & `tryangle-0.2.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryangle
-Version: 0.2.2
+Version: 0.2.2.dev0
 Summary: Tryangle Package - Scientific P&C Loss Reserving
 Maintainer-email: Caesar Balona <caesar.balona@gmail.com>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/casact/tryangle
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `tryangle-0.2.2/README.md` & `tryangle-0.2.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/pyproject.toml` & `tryangle-0.2.2.dev0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tryangle"
-version = "0.2.2"
+version = "0.2.2.dev0"
 description = "Tryangle Package - Scientific P&C Loss Reserving"
 readme = "README.md"
 maintainers = [{ name = "Caesar Balona", email = "caesar.balona@gmail.com" }]
 classifiers = [
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
```

### Comparing `tryangle-0.2.2/requirements.txt` & `tryangle-0.2.2.dev0/requirements.txt`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/core/__init__.py` & `tryangle-0.2.2.dev0/src/tryangle/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/core/base.py` & `tryangle-0.2.2.dev0/src/tryangle/core/base.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/core/methods.py` & `tryangle-0.2.2.dev0/src/tryangle/core/methods.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/ensemble/__init__.py` & `tryangle-0.2.2.dev0/src/tryangle/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/ensemble/base.py` & `tryangle-0.2.2.dev0/src/tryangle/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/ensemble/losses.py` & `tryangle-0.2.2.dev0/src/tryangle/ensemble/losses.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/ensemble/optimizers.py` & `tryangle-0.2.2.dev0/src/tryangle/ensemble/optimizers.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/metrics/__init__.py` & `tryangle-0.2.2.dev0/src/tryangle/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/metrics/base.py` & `tryangle-0.2.2.dev0/src/tryangle/metrics/base.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/metrics/score.py` & `tryangle-0.2.2.dev0/src/tryangle/metrics/score.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/model_selection/split.py` & `tryangle-0.2.2.dev0/src/tryangle/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/utils/data/cas_test.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/cas_test.csv`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/utils/data/cas_train.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/cas_train.csv`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/utils/data/sme_test.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/sme_test.csv`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/utils/data/sme_train.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/sme_train.csv`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/utils/data/swiss_test.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/swiss_test.csv`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/utils/data/swiss_train.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/swiss_train.csv`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle/utils/datasets.py` & `tryangle-0.2.2.dev0/src/tryangle/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/src/tryangle.egg-info/PKG-INFO` & `tryangle-0.2.2.dev0/src/tryangle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryangle
-Version: 0.2.2
+Version: 0.2.2.dev0
 Summary: Tryangle Package - Scientific P&C Loss Reserving
 Maintainer-email: Caesar Balona <caesar.balona@gmail.com>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/casact/tryangle
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `tryangle-0.2.2/src/tryangle.egg-info/SOURCES.txt` & `tryangle-0.2.2.dev0/src/tryangle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/tests/test_datasets.py` & `tryangle-0.2.2.dev0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/tests/test_ensemble.py` & `tryangle-0.2.2.dev0/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/tests/test_methods.py` & `tryangle-0.2.2.dev0/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/tests/test_score.py` & `tryangle-0.2.2.dev0/tests/test_score.py`

 * *Files identical despite different names*

### Comparing `tryangle-0.2.2/tests/test_split.py` & `tryangle-0.2.2.dev0/tests/test_split.py`

 * *Files identical despite different names*

