# Comparing `tmp/confidenceinterval-1.0.2.tar.gz` & `tmp/confidenceinterval-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confidenceinterval-1.0.2.tar", last modified: Sun Jun 11 04:10:25 2023, max compression
+gzip compressed data, was "confidenceinterval-1.0.3.tar", last modified: Sun Jun 11 08:34:43 2023, max compression
```

## Comparing `confidenceinterval-1.0.2.tar` & `confidenceinterval-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 04:10:25.291815 confidenceinterval-1.0.2/
--rw-r--r--   0 gildenbj   (501) staff       (20)     1072 2023-03-11 16:10:01.000000 confidenceinterval-1.0.2/LICENSE
--rw-r--r--   0 gildenbj   (501) staff       (20)       48 2023-04-19 15:52:18.000000 confidenceinterval-1.0.2/MANIFEST.in
--rw-r--r--   0 gildenbj   (501) staff       (20)     8165 2023-06-11 04:10:25.292009 confidenceinterval-1.0.2/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)     7626 2023-06-11 04:08:57.000000 confidenceinterval-1.0.2/README.md
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 04:10:25.288900 confidenceinterval-1.0.2/confidenceinterval/
--rw-r--r--   0 gildenbj   (501) staff       (20)      365 2023-06-10 10:27:57.000000 confidenceinterval-1.0.2/confidenceinterval/__init__.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1666 2023-06-10 11:51:15.000000 confidenceinterval-1.0.2/confidenceinterval/auc.py
--rw-r--r--   0 gildenbj   (501) staff       (20)    17608 2023-06-11 03:54:43.000000 confidenceinterval-1.0.2/confidenceinterval/binary_metrics.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     1444 2023-06-10 15:18:25.000000 confidenceinterval-1.0.2/confidenceinterval/bootstrap.py
--rw-r--r--   0 gildenbj   (501) staff       (20)     7130 2023-03-11 16:36:30.000000 confidenceinterval-1.0.2/confidenceinterval/delong.py
--rw-r--r--   0 gildenbj   (501) staff       (20)    25708 2023-06-10 18:41:22.000000 confidenceinterval-1.0.2/confidenceinterval/takahashi_methods.py
--rw-r--r--   0 gildenbj   (501) staff       (20)      895 2023-03-11 15:07:46.000000 confidenceinterval-1.0.2/confidenceinterval/utils.py
-drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 04:10:25.291332 confidenceinterval-1.0.2/confidenceinterval.egg-info/
--rw-r--r--   0 gildenbj   (501) staff       (20)     8165 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/PKG-INFO
--rw-r--r--   0 gildenbj   (501) staff       (20)      497 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/SOURCES.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/dependency_links.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       55 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/requires.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       19 2023-06-11 04:10:25.000000 confidenceinterval-1.0.2/confidenceinterval.egg-info/top_level.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)       54 2023-06-10 15:04:55.000000 confidenceinterval-1.0.2/requirements.txt
--rw-r--r--   0 gildenbj   (501) staff       (20)      613 2023-06-11 04:10:25.292822 confidenceinterval-1.0.2/setup.cfg
--rw-r--r--   0 gildenbj   (501) staff       (20)      870 2023-06-11 04:10:20.000000 confidenceinterval-1.0.2/setup.py
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 08:34:43.958030 confidenceinterval-1.0.3/
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1072 2023-03-11 16:10:01.000000 confidenceinterval-1.0.3/LICENSE
+-rw-r--r--   0 gildenbj   (501) staff       (20)       48 2023-04-19 15:52:18.000000 confidenceinterval-1.0.3/MANIFEST.in
+-rw-r--r--   0 gildenbj   (501) staff       (20)     8165 2023-06-11 08:34:43.958216 confidenceinterval-1.0.3/PKG-INFO
+-rw-r--r--   0 gildenbj   (501) staff       (20)     7626 2023-06-11 04:08:57.000000 confidenceinterval-1.0.3/README.md
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 08:34:43.955500 confidenceinterval-1.0.3/confidenceinterval/
+-rw-r--r--   0 gildenbj   (501) staff       (20)      365 2023-06-10 10:27:57.000000 confidenceinterval-1.0.3/confidenceinterval/__init__.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1666 2023-06-10 11:51:15.000000 confidenceinterval-1.0.3/confidenceinterval/auc.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)    17608 2023-06-11 08:32:15.000000 confidenceinterval-1.0.3/confidenceinterval/binary_metrics.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     1422 2023-06-11 08:33:05.000000 confidenceinterval-1.0.3/confidenceinterval/bootstrap.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)     7130 2023-03-11 16:36:30.000000 confidenceinterval-1.0.3/confidenceinterval/delong.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)    25708 2023-06-11 08:34:03.000000 confidenceinterval-1.0.3/confidenceinterval/takahashi_methods.py
+-rw-r--r--   0 gildenbj   (501) staff       (20)      895 2023-03-11 15:07:46.000000 confidenceinterval-1.0.3/confidenceinterval/utils.py
+drwxr-xr-x   0 gildenbj   (501) staff       (20)        0 2023-06-11 08:34:43.957631 confidenceinterval-1.0.3/confidenceinterval.egg-info/
+-rw-r--r--   0 gildenbj   (501) staff       (20)     8165 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/PKG-INFO
+-rw-r--r--   0 gildenbj   (501) staff       (20)      497 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/SOURCES.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)        1 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/dependency_links.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       55 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/requires.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       19 2023-06-11 08:34:43.000000 confidenceinterval-1.0.3/confidenceinterval.egg-info/top_level.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)       54 2023-06-11 08:34:14.000000 confidenceinterval-1.0.3/requirements.txt
+-rw-r--r--   0 gildenbj   (501) staff       (20)      613 2023-06-11 08:34:43.958819 confidenceinterval-1.0.3/setup.cfg
+-rw-r--r--   0 gildenbj   (501) staff       (20)      870 2023-06-11 08:30:40.000000 confidenceinterval-1.0.3/setup.py
```

### Comparing `confidenceinterval-1.0.2/LICENSE` & `confidenceinterval-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.2/PKG-INFO` & `confidenceinterval-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidenceinterval
-Version: 1.0.2
+Version: 1.0.3
 Summary: Confidence Intervals in python
 Home-page: https://github.com/jacobgil/confidenceinterval
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/confidenceinterval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `confidenceinterval-1.0.2/README.md` & `confidenceinterval-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.2/confidenceinterval/auc.py` & `confidenceinterval-1.0.3/confidenceinterval/auc.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.2/confidenceinterval/binary_metrics.py` & `confidenceinterval-1.0.3/confidenceinterval/binary_metrics.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.2/confidenceinterval/bootstrap.py` & `confidenceinterval-1.0.3/confidenceinterval/bootstrap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from scipy.stats import bootstrap
 import numpy as np
-from typing import List, Callable, Optional, Tuple, TypedDict
+from typing import List, Callable, Optional, Tuple
 
 bootstrap_methods = [
     'bootstrap_bca',
     'bootstrap_percentile',
     'bootstrap_basic']
 
 
-class BootstrapParams(TypedDict):
+class BootstrapParams:
     n_resamples: int
     random_state: Optional[np.random.RandomState]
 
 
 def bootstrap_ci(y_true: List[int],
                  y_pred: List[int],
                  metric: Callable,
```

### Comparing `confidenceinterval-1.0.2/confidenceinterval/delong.py` & `confidenceinterval-1.0.3/confidenceinterval/delong.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.2/confidenceinterval/takahashi_methods.py` & `confidenceinterval-1.0.3/confidenceinterval/takahashi_methods.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.2/confidenceinterval/utils.py` & `confidenceinterval-1.0.3/confidenceinterval/utils.py`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.2/confidenceinterval.egg-info/PKG-INFO` & `confidenceinterval-1.0.3/confidenceinterval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidenceinterval
-Version: 1.0.2
+Version: 1.0.3
 Summary: Confidence Intervals in python
 Home-page: https://github.com/jacobgil/confidenceinterval
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/confidenceinterval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `confidenceinterval-1.0.2/setup.cfg` & `confidenceinterval-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `confidenceinterval-1.0.2/setup.py` & `confidenceinterval-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name='confidenceinterval',
-    version='1.0.2',
+    version='1.0.3',
     author='Jacob Gildenblat',
     author_email='jacob.gildenblat@gmail.com',
     description='Confidence Intervals in python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jacobgil/confidenceinterval',
     project_urls={
```

