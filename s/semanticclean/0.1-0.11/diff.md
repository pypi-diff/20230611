# Comparing `tmp/semanticclean-0.1.tar.gz` & `tmp/semanticclean-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticclean-0.1.tar", last modified: Sun Jun 11 13:17:48 2023, max compression
+gzip compressed data, was "semanticclean-0.11.tar", last modified: Sun Jun 11 16:42:46 2023, max compression
```

## Comparing `semanticclean-0.1.tar` & `semanticclean-0.11.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 13:17:48.577678 semanticclean-0.1/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      233 2023-06-11 13:17:48.577678 semanticclean-0.1/PKG-INFO
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 13:17:48.577678 semanticclean-0.1/semanticclean/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 13:16:36.000000 semanticclean-0.1/semanticclean/__init__.py
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)     6374 2023-06-11 11:34:16.000000 semanticclean-0.1/semanticclean/label.py
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 13:17:48.577678 semanticclean-0.1/semanticclean.egg-info/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      233 2023-06-11 13:17:48.000000 semanticclean-0.1/semanticclean.egg-info/PKG-INFO
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      241 2023-06-11 13:17:48.000000 semanticclean-0.1/semanticclean.egg-info/SOURCES.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 13:17:48.000000 semanticclean-0.1/semanticclean.egg-info/dependency_links.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 13:17:48.000000 semanticclean-0.1/semanticclean.egg-info/not-zip-safe
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       14 2023-06-11 13:17:48.000000 semanticclean-0.1/semanticclean.egg-info/top_level.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 13:17:48.577678 semanticclean-0.1/setup.cfg
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      301 2023-06-11 13:15:47.000000 semanticclean-0.1/setup.py
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 16:42:46.232499 semanticclean-0.11/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 16:42:46.232499 semanticclean-0.11/PKG-INFO
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 16:42:46.232499 semanticclean-0.11/semanticclean/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 13:16:36.000000 semanticclean-0.11/semanticclean/__init__.py
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)     6768 2023-06-11 16:09:42.000000 semanticclean-0.11/semanticclean/label.py
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 16:42:46.232499 semanticclean-0.11/semanticclean.egg-info/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/PKG-INFO
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      241 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/not-zip-safe
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       14 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/top_level.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 16:42:46.232499 semanticclean-0.11/setup.cfg
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      302 2023-06-11 16:42:39.000000 semanticclean-0.11/setup.py
```

### Comparing `semanticclean-0.1/semanticclean/label.py` & `semanticclean-0.11/semanticclean/label.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
-from typing import List
+from typing import List, Dict
 
 class LabelIssues:
     def __init__(self, labels, pred_probs):
         self.labels = np.array(labels)
         self.pred_probs = pred_probs
         self.epsilon = 1e-6
         self.num_examples = len(labels)
@@ -120,23 +120,30 @@
         if len(args) > 0:
             for arr in args:
                 arr = np.delete(arr, to_remove, axis=axis)
                 new_data.append(arr)
         new_data.append(np.delete(self.labels, to_remove, axis=axis))
         return new_data
         
-    def suggest(self):
+    def suggest(self, frac: float=0.4, n: int=0):
         # provide a new version of data with suggested labels
-        return self.guessed_labels
+        if n > 0:
+            num_to_return = n
+        num_to_return = int(frac * len(self.guessed_labels))
+        return self.guessed_labels[:num_to_return]
     
-    def report(self):
-        df = pd.DataFrame(
-            {'example': self.idx_issues, 'given_label': self.labels[self.idx_issues], \
+    def report(self, include_cols: Dict[str, np.ndarray]={}):
+        data_cols = {'example': self.idx_issues, 'given_label': self.labels[self.idx_issues], \
              'score': self.score_list, 'guessed_label': self.guessed_labels}
-        )
+        
+        if len(include_cols) > 0:
+            include_cols = {'_'+k: v[:len(self)] for k, v in include_cols.items()}
+            data_cols = {**include_cols,**data_cols}
+        
+        df = pd.DataFrame(data_cols)
         return df
     
     def summary(self):
         print('-'*79)
         for i in range(self.num_classes):
             for j in range(self.num_classes):
                 if i==j:
```

