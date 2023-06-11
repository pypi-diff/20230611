# Comparing `tmp/scikit-gbm-0.0.1.tar.gz` & `tmp/scikit-gbm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-gbm-0.0.1.tar", last modified: Wed Apr 19 19:37:06 2023, max compression
+gzip compressed data, was "scikit-gbm-0.1.0.tar", last modified: Sun Jun 11 19:44:06 2023, max compression
```

## Comparing `scikit-gbm-0.0.1.tar` & `scikit-gbm-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-04-19 19:37:06.520351 scikit-gbm-0.0.1/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1077 2023-04-15 14:39:04.000000 scikit-gbm-0.0.1/LICENSE
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1546 2023-04-19 19:37:06.520351 scikit-gbm-0.0.1/PKG-INFO
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      998 2023-04-19 19:26:31.000000 scikit-gbm-0.0.1/README.md
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      620 2023-04-15 19:26:38.000000 scikit-gbm-0.0.1/pyproject.toml
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-04-19 19:37:06.500352 scikit-gbm-0.0.1/scikit_gbm.egg-info/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1546 2023-04-19 19:37:06.000000 scikit-gbm-0.0.1/scikit_gbm.egg-info/PKG-INFO
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      249 2023-04-19 19:37:06.000000 scikit-gbm-0.0.1/scikit_gbm.egg-info/SOURCES.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        1 2023-04-19 19:37:06.000000 scikit-gbm-0.0.1/scikit_gbm.egg-info/dependency_links.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        6 2023-04-19 19:37:06.000000 scikit-gbm-0.0.1/scikit_gbm.egg-info/top_level.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       38 2023-04-19 19:37:06.520351 scikit-gbm-0.0.1/setup.cfg
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-04-19 19:37:06.500352 scikit-gbm-0.0.1/skgbm/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      112 2023-04-15 14:39:58.000000 scikit-gbm-0.0.1/skgbm/__init__.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2104 2023-04-15 15:54:18.000000 scikit-gbm-0.0.1/skgbm/base.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1851 2023-04-19 19:19:32.000000 scikit-gbm-0.0.1/skgbm/preprocessing.py
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-04-19 19:37:06.504351 scikit-gbm-0.0.1/tests/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2587 2023-04-15 16:16:57.000000 scikit-gbm-0.0.1/tests/test_gbm_wrapper.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-11 19:44:06.880912 scikit-gbm-0.1.0/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1077 2023-04-15 14:39:04.000000 scikit-gbm-0.1.0/LICENSE
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2295 2023-06-11 19:44:06.880912 scikit-gbm-0.1.0/PKG-INFO
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1747 2023-06-10 20:23:41.000000 scikit-gbm-0.1.0/README.md
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      720 2023-06-11 19:42:50.000000 scikit-gbm-0.1.0/pyproject.toml
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       75 2023-06-10 23:00:01.000000 scikit-gbm-0.1.0/requirements.txt
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-11 19:44:06.852914 scikit-gbm-0.1.0/scikit_gbm.egg-info/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2295 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/PKG-INFO
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      387 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        1 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       75 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/requires.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        6 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/top_level.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       38 2023-06-11 19:44:06.880912 scikit-gbm-0.1.0/setup.cfg
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-11 19:44:06.864913 scikit-gbm-0.1.0/skgbm/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       48 2023-06-09 20:23:00.000000 scikit-gbm-0.1.0/skgbm/__init__.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     4073 2023-06-10 20:23:41.000000 scikit-gbm-0.1.0/skgbm/base.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1787 2023-06-09 20:23:00.000000 scikit-gbm-0.1.0/skgbm/preprocessing.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     3664 2023-06-10 19:49:26.000000 scikit-gbm-0.1.0/skgbm/tools.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     5348 2023-06-09 20:23:00.000000 scikit-gbm-0.1.0/skgbm/tree.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     7896 2023-06-10 23:04:56.000000 scikit-gbm-0.1.0/skgbm/trees_extraction.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-11 19:44:06.880912 scikit-gbm-0.1.0/tests/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2587 2023-04-15 16:16:57.000000 scikit-gbm-0.1.0/tests/test_gbm_wrapper.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1574 2023-06-09 20:23:00.000000 scikit-gbm-0.1.0/tests/test_trees_to_dataframe.py
```

### Comparing `scikit-gbm-0.0.1/LICENSE` & `scikit-gbm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.0.1/PKG-INFO` & `scikit-gbm-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: scikit-gbm
-Version: 0.0.1
+Version: 0.1.0
 Summary: scikit-learn compatible tools to work with GBM models
 Author-email: Krzysztof Joachimiak <joachimiak.krzysztof@gmail.com>
 Project-URL: Homepage, https://github.com/krzjoa/scikit-gbm
 Project-URL: Bug Tracker, https://github.com/krzjoa/scikit-gbm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scikit-gbm
+
+[![Documentation Status](https://readthedocs.org/projects/scikit-gbm/badge/?version=latest)](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest)
+
 scikit-learn compatible tools to work with GBM models
 
 ## Installation
 
 ```
 pip install scikit-gbm
 
 # or 
 
 pip install git+https://github.com/krzjoa/scikit-gbm.git
-
 ```
 
 ## Usage
 
 For the moment, the only available class is `GBMFeaturezier`. It's a wrapper around
-scikit-learn GBMs, XGBoost, LightGBM and CatBoost models.
+scikit-learn GBMs, XGBoost, LightGBM and CatBoost models. 
 
 ```python
 
-
 # Classification
 from sklearn.datasets import make_classification
 from sklearn.pipeline import Pipeline
 from sklearn.linear_model import LogisticRegression
 
 from skgbm.preprocessing import GBMFeaturizer
+from lightgbm import LGBMRegressor
 from xgboost import XGBClassifier
 
 X, y = make_classification()
 # train_test_split
 
 pipeline = \
     Pipeline([
@@ -54,10 +56,29 @@
 # Try also:
 # ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
 
 
 # Regression
+X, y = load_breast_cancer(return_X_y=True)
+X_train, X_test, y_train, y_test = train_test_split(X, y)
+
+# Try also:
+# ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
+# ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
+# ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
+
+pipeline = \
+    Pipeline([
+        ('gbm_featurizer', GBMFeaturizer(XGBClassifier())),
+        ('logistic_regression', LogisticRegression())
+    ])
+
+# Training
+pipeline.fit(X_train, y_train)
+
+# Predictions for the test set
+pipeline_pred = pipeline.predict(X_test)
 
 
 ```
```

### Comparing `scikit-gbm-0.0.1/README.md` & `scikit-gbm-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # scikit-gbm
+
+[![Documentation Status](https://readthedocs.org/projects/scikit-gbm/badge/?version=latest)](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest)
+
 scikit-learn compatible tools to work with GBM models
 
 ## Installation
 
 ```
 pip install scikit-gbm
 
 # or 
 
 pip install git+https://github.com/krzjoa/scikit-gbm.git
-
 ```
 
 ## Usage
 
 For the moment, the only available class is `GBMFeaturezier`. It's a wrapper around
-scikit-learn GBMs, XGBoost, LightGBM and CatBoost models.
+scikit-learn GBMs, XGBoost, LightGBM and CatBoost models. 
 
 ```python
 
-
 # Classification
 from sklearn.datasets import make_classification
 from sklearn.pipeline import Pipeline
 from sklearn.linear_model import LogisticRegression
 
 from skgbm.preprocessing import GBMFeaturizer
+from lightgbm import LGBMRegressor
 from xgboost import XGBClassifier
 
 X, y = make_classification()
 # train_test_split
 
 pipeline = \
     Pipeline([
@@ -40,10 +42,29 @@
 # Try also:
 # ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
 
 
 # Regression
+X, y = load_breast_cancer(return_X_y=True)
+X_train, X_test, y_train, y_test = train_test_split(X, y)
+
+# Try also:
+# ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
+# ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
+# ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
+
+pipeline = \
+    Pipeline([
+        ('gbm_featurizer', GBMFeaturizer(XGBClassifier())),
+        ('logistic_regression', LogisticRegression())
+    ])
+
+# Training
+pipeline.fit(X_train, y_train)
+
+# Predictions for the test set
+pipeline_pred = pipeline.predict(X_test)
 
 
 ```
```

### Comparing `scikit-gbm-0.0.1/pyproject.toml` & `scikit-gbm-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [project]
 name = "scikit-gbm"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Krzysztof Joachimiak", email="joachimiak.krzysztof@gmail.com" },
 ]
 description = "scikit-learn compatible tools to work with GBM models"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dynamic = ["dependencies"]
 
 [project.urls]
 "Homepage" = "https://github.com/krzjoa/scikit-gbm"
 "Bug Tracker" = "https://github.com/krzjoa/scikit-gbm/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
```

### Comparing `scikit-gbm-0.0.1/scikit_gbm.egg-info/PKG-INFO` & `scikit-gbm-0.1.0/scikit_gbm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: scikit-gbm
-Version: 0.0.1
+Version: 0.1.0
 Summary: scikit-learn compatible tools to work with GBM models
 Author-email: Krzysztof Joachimiak <joachimiak.krzysztof@gmail.com>
 Project-URL: Homepage, https://github.com/krzjoa/scikit-gbm
 Project-URL: Bug Tracker, https://github.com/krzjoa/scikit-gbm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scikit-gbm
+
+[![Documentation Status](https://readthedocs.org/projects/scikit-gbm/badge/?version=latest)](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest)
+
 scikit-learn compatible tools to work with GBM models
 
 ## Installation
 
 ```
 pip install scikit-gbm
 
 # or 
 
 pip install git+https://github.com/krzjoa/scikit-gbm.git
-
 ```
 
 ## Usage
 
 For the moment, the only available class is `GBMFeaturezier`. It's a wrapper around
-scikit-learn GBMs, XGBoost, LightGBM and CatBoost models.
+scikit-learn GBMs, XGBoost, LightGBM and CatBoost models. 
 
 ```python
 
-
 # Classification
 from sklearn.datasets import make_classification
 from sklearn.pipeline import Pipeline
 from sklearn.linear_model import LogisticRegression
 
 from skgbm.preprocessing import GBMFeaturizer
+from lightgbm import LGBMRegressor
 from xgboost import XGBClassifier
 
 X, y = make_classification()
 # train_test_split
 
 pipeline = \
     Pipeline([
@@ -54,10 +56,29 @@
 # Try also:
 # ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
 
 
 # Regression
+X, y = load_breast_cancer(return_X_y=True)
+X_train, X_test, y_train, y_test = train_test_split(X, y)
+
+# Try also:
+# ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
+# ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
+# ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
+
+pipeline = \
+    Pipeline([
+        ('gbm_featurizer', GBMFeaturizer(XGBClassifier())),
+        ('logistic_regression', LogisticRegression())
+    ])
+
+# Training
+pipeline.fit(X_train, y_train)
+
+# Predictions for the test set
+pipeline_pred = pipeline.predict(X_test)
 
 
 ```
```

### Comparing `scikit-gbm-0.0.1/skgbm/preprocessing.py` & `scikit-gbm-0.1.0/skgbm/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-Created on Sat Apr 15 17:46:28 2023
-
-@author: krzysztof
-"""
 
 import scipy
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import OneHotEncoder
 
 from .base import GBMWrapper
```

### Comparing `scikit-gbm-0.0.1/tests/test_gbm_wrapper.py` & `scikit-gbm-0.1.0/tests/test_gbm_wrapper.py`

 * *Files identical despite different names*

