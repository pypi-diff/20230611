# Comparing `tmp/scikit-query-0.1.tar.gz` & `tmp/scikit-query-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-query-0.1.tar", last modified: Sun Jun  4 20:21:17 2023, max compression
+gzip compressed data, was "scikit-query-0.1.1.tar", last modified: Sat Jun 10 22:00:25 2023, max compression
```

## Comparing `scikit-query-0.1.tar` & `scikit-query-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:21:17.039232 scikit-query-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-04 20:20:22.000000 scikit-query-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-04 20:21:17.039232 scikit-query-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-04 20:20:22.000000 scikit-query-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:21:17.035232 scikit-query-0.1/scikit_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-04 20:21:16.000000 scikit-query-0.1/scikit_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-04 20:21:16.000000 scikit-query-0.1/scikit_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:21:16.000000 scikit-query-0.1/scikit_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:21:16.000000 scikit-query-0.1/scikit_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-04 20:21:16.000000 scikit-query-0.1/scikit_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 20:21:16.000000 scikit-query-0.1/scikit_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:21:17.039232 scikit-query-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-04 20:20:22.000000 scikit-query-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:21:17.035232 scikit-query-0.1/skquery/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:21:17.035232 scikit-query-0.1/skquery/oracle/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/oracle/MLCLOracle.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/oracle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:21:17.035232 scikit-query-0.1/skquery/pairwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/pairwise/AIPC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/pairwise/FFQS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/pairwise/MinMax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/pairwise/NPUincr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/pairwise/Pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/pairwise/Random.py
--rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/pairwise/SASC.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:21:17.035232 scikit-query-0.1/skquery/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/tests/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:21:17.039232 scikit-query-0.1/skquery/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    21382 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/utils/BaseSVDD.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-04 20:20:22.000000 scikit-query-0.1/skquery/utils/line_intercept.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-10 21:59:40.000000 scikit-query-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-10 22:00:25.608819 scikit-query-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-10 21:59:40.000000 scikit-query-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.604819 scikit-query-0.1.1/scikit_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 22:00:25.000000 scikit-query-0.1.1/scikit_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 22:00:25.608819 scikit-query-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-10 21:59:40.000000 scikit-query-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-10 21:59:41.000000 scikit-query-0.1.1/skquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/oracle/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/oracle/MLCLOracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/oracle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/AIPC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/FFQS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/MinMax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/NPU.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/Pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/RandomMLCL.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/SASC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:00:25.608819 scikit-query-0.1.1/skquery/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/utils/BaseSVDD.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-10 21:59:40.000000 scikit-query-0.1.1/skquery/utils/line_intercept.py
```

### Comparing `scikit-query-0.1/LICENSE` & `scikit-query-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-query-0.1/scikit_query.egg-info/SOURCES.txt` & `scikit-query-0.1.1/scikit_query.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 skquery/exceptions.py
 skquery/strategy.py
 skquery/oracle/MLCLOracle.py
 skquery/oracle/__init__.py
 skquery/pairwise/AIPC.py
 skquery/pairwise/FFQS.py
 skquery/pairwise/MinMax.py
-skquery/pairwise/NPUincr.py
+skquery/pairwise/NPU.py
 skquery/pairwise/Pairwise.py
-skquery/pairwise/Random.py
+skquery/pairwise/RandomMLCL.py
 skquery/pairwise/SASC.py
 skquery/pairwise/__init__.py
 skquery/tests/__init__.py
 skquery/tests/test_query.py
 skquery/utils/BaseSVDD.py
 skquery/utils/__init__.py
 skquery/utils/line_intercept.py
```

### Comparing `scikit-query-0.1/setup.py` & `scikit-query-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-query-0.1/skquery/oracle/MLCLOracle.py` & `scikit-query-0.1.1/skquery/oracle/MLCLOracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..exceptions import MaximumQueriesExceeded
 
 
 class MLCLOracle:
-    def __init__(self, budget=20, truth=None):
+    def __init__(self, budget=10, truth=None):
         self.queries = 0
         self.budget = budget
         self.truth = truth
 
     def query(self, i, j):
         """
         Query the oracle to find out whether i and j should be must-linked
```

### Comparing `scikit-query-0.1/skquery/pairwise/AIPC.py` & `scikit-query-0.1.1/skquery/pairwise/AIPC.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,83 @@
 """
  Active Informative Pairwise Constraint Formulation algorithm from Zhong et al. 2019.
 """
-# Authors : Brice Jacquesson, Matthéo Pailler
+# Authors : Brice Jacquesson, Matthéo Pailler, Aymeric Beauchamp
 
 import pandas as pd
 from sklearn.metrics import pairwise_distances
+from ..exceptions import MaximumQueriesExceeded
 from ..strategy import QueryStrategy
 import numpy as np
 import skfuzzy as fuzz
 
 
 class AIPC(QueryStrategy):
 
-    def __init__(self, nb_centre: int, epsilon: float = 0.05):
+    def __init__(self, epsilon: float = 0.05):
         super().__init__()
-        self.data = None
-        self.epsilon = epsilon * nb_centre
+        self.partition = []
+        self.epsilon = epsilon
         self.centres = None
         self.u = None
         self.d = None
-        self.nb_centre = nb_centre
-        self.budget = 0
 
-    def fit(self, X, partition, oracle):
-        self.budget = oracle.budget
+    def fit(self, X, oracle, **kwargs):
+        X = self._check_dataset_type(X)
 
-        self.data = X
+        if "partition" in kwargs:
+            self.partition = kwargs["partition"]
 
-        self._fuzzy_cmeans()
+        if len(self.partition) > 0:
+            K = len(set(self.partition))
+        elif "n_clusters" in kwargs:
+            K = kwargs["n_clusters"]
+        else:
+            raise ValueError("No cluster number provided")
+        self.epsilon = self.epsilon * K
+        self._fuzzy_cmeans(X, K)
 
         ml, cl = [], []
         constraints = {"ml": ml, "cl": cl}
 
-        nb_queries = 0
-        entropy = self._entropy()  # récupérer les weak samples (voir discord)
+        entropy = self._entropy(X)  # récupérer les weak samples (voir discord)
         weak_samples = []
         for i in range(len(entropy)):  # récupération des weak samples
-            if entropy[i][1] > np.log(self.nb_centre) - self.epsilon:
+            if entropy[i][1] > np.log(K) - self.epsilon:
                 # entropy[1] = entropie
                 weak_samples.append(entropy[i])
         weak_samples.sort(key=lambda x: x[1], reverse=True)  # tri par entropy
 
         strong_samples = self._compute_medoids()  # récupération des strong samples.
 
-        while (nb_queries < self.budget) and (len(weak_samples) > 0):
-            nb_queries += 1
-            xweak = weak_samples.pop()
-            strong_samples.sort(key=lambda x: self._symmetric_relative_entropy(xweak, x))
-            first_strong = strong_samples[0][1]
-            second_strong = strong_samples[1][1]
-            weak = xweak[0]
-
-            must_link = oracle.query(weak, second_strong)
-            if must_link:
-                ml.append((weak, second_strong))
-            else:
-                cl.append((weak, second_strong))
-                ml.append((weak, first_strong))
+        while True:
+            try:
+                xweak = weak_samples.pop()
+                strong_samples.sort(key=lambda x: self._symmetric_relative_entropy(xweak, x, K))
+                first_strong = strong_samples[0][1]
+                second_strong = strong_samples[1][1]
+                weak = xweak[0]
+
+                if oracle.query(weak, second_strong):
+                    ml.append((weak, second_strong))
+                else:
+                    cl.append((weak, second_strong))
+                    ml.append((weak, first_strong))
 
-        return constraints
+            except MaximumQueriesExceeded:
+                break
 
-    """
-    return entropy : list of tuple ([x, y], entropy) where x and y are the coordinate of the point and entropy is the entropy of the point.
-    """
+        return constraints
 
-    def _entropy(self):
+    def _entropy(self, X):
+        """
+        return entropy : list of tuple ([x, y], entropy) where x and y are the coordinate of the point and entropy is the entropy of the point.
+        """
         entropy = []
-        for j in range(len(self.data)):
+        for j in range(X.shape[0]):
             entropyX = 0
             for i in range(len(self.u)):
                 u_ij = self.u[i][j]
                 entropyX += u_ij * np.log(u_ij)
             entropy.append([j, -entropyX])
         return entropy
 
@@ -83,31 +90,24 @@
                 if e < dist_min:
                     dist_min = e
                     minInd = ind
             medoids.append((i, minInd))
 
         return medoids
 
-    def _symmetric_relative_entropy(self, xweak, x):
+    def _symmetric_relative_entropy(self, xweak, x, k):
         # a et b correspondent respectivement à la première et seconde somme de l'équation (12) de l'article.
         a = 0
         b = 0
-        for i in range(self.nb_centre):
+        for i in range(k):
             u_xj = self.u[i][x[1]]  # x[1] correspond à l'indice dans la data
             u_xweak = self.u[i][xweak[0]]  # xweak[0] correspond à l'indice dans la data
             a += u_xj * (np.log((np.divide(u_xj, u_xweak))))
             b += u_xweak * (np.log((np.divide(u_xweak, u_xj))))
 
         return (a + b) / 2
 
-    def _fuzzy_cmeans(self):
-        datatemp = np.empty((2, len(self.data)), float)
-
-        data = self.data
-        for i in range(len(data)):
-            datatemp[0][i] = data[i][0]
-            datatemp[1][i] = data[i][1]
-
-        fcm = fuzz.cmeans(datatemp, self.nb_centre, 2, 0.05, maxiter=1000)
+    def _fuzzy_cmeans(self, X, k):
+        fcm = fuzz.cmeans(X.T, k, 2, 0.05, maxiter=1000)
         self.centres = fcm[0]
         self.u = fcm[1]
         self.d = fcm[3]
```

### Comparing `scikit-query-0.1/skquery/pairwise/MinMax.py` & `scikit-query-0.1.1/skquery/pairwise/MinMax.py`

 * *Files identical despite different names*

### Comparing `scikit-query-0.1/skquery/pairwise/NPUincr.py` & `scikit-query-0.1.1/skquery/pairwise/NPU.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,47 @@
+""" Normalized Point-wise Uncertainty algorithm. Based off the implementation at
+https://github.com/datamole-ai/active-semi-supervised-clustering
+"""
+# Authors : Aymeric Beauchamp
+
 import numpy as np
 from ..exceptions import MaximumQueriesExceeded
 from ..strategy import QueryStrategy
 from sklearn.ensemble import RandomForestClassifier
 
 
-class NPUincr(QueryStrategy):
-    """ Incremental version of NPU. Based off the implementation at
-    https://github.com/datamole-ai/active-semi-supervised-clustering
-    """
+class NPU(QueryStrategy):
 
-    def __init__(self, neighborhoods=None):
+    def __init__(self, neighborhoods=None, clusterer=None):
         super().__init__()
+        self.partition = []
         self.neighborhoods = [] if not neighborhoods or type(neighborhoods) != list else neighborhoods
+        self.clusterer = clusterer
+
+    def fit(self, X, oracle, **kwargs):
+        X = self._check_dataset_type(X)
 
-    def fit(self, X, partition, oracle):
         ml, cl = [], []
         constraints = {"ml": ml, "cl": cl}
-        self.partition = partition
-        n = X.shape[0]
+        if not self.clusterer and "partition" in kwargs:
+            # disregard if a CC algorithm is provided
+            self.partition = kwargs["partition"]
 
-        if not self.neighborhoods:
+        if len(self.neighborhoods) == 0:
             # Initialization
-            x_i = np.random.choice(list(range(n)))
+            x_i = np.random.choice(list(range(X.shape[0])))
             self.neighborhoods.append([x_i])
 
         while True:
             try:
+                if self.clusterer is not None:
+                    # only works with CC algorithms from active-semi-supervised-clustering library
+                    self.clusterer.fit(X.to_numpy(), ml=ml, cl=cl)
+                    self.partition = self.clusterer.labels_
+
                 x_i, p_i = self._most_informative(X)
 
                 sorted_neighborhoods = list(zip(*reversed(sorted(zip(p_i, self.neighborhoods)))))[1]
                 #  print(x_i, self.neighborhoods, p_i, sorted_neighborhoods)
 
                 must_link_found = False
```

### Comparing `scikit-query-0.1/skquery/pairwise/Pairwise.py` & `scikit-query-0.1.1/skquery/pairwise/Pairwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         for iteration in range(precision):
             array = np.copy(algo.fit(dataset.data).labels_)
             generer_matrice(mat=mat, cluster=array)
             list_cluster = np.concatenate((list_cluster, array), axis=0) if list_cluster is not None else np.copy(array)
 
         return mat
 
-    def fit(self, dataset):
-        return self.active_HACC(dataset)
+    def fit(self, X, *args):
+        return self.active_HACC(X)
 
     def paire(self, point_ic, point_jc, clusters):
         # print(f" ({point_ic},{point_jc})")
         paire_de_point: bool = clusters[point_ic] == clusters[point_jc]
         return True if paire_de_point else False
 
     def jcc(self, C1, C2):
```

### Comparing `scikit-query-0.1/skquery/pairwise/Random.py` & `scikit-query-0.1.1/skquery/pairwise/RandomMLCL.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 from ..strategy import QueryStrategy
 
 
-class Random(QueryStrategy):
-    def __init__(self, n_clusters):
+class RandomMLCL(QueryStrategy):
+    def __init__(self):
         super().__init__()
-        self.n_clusters = n_clusters
 
-    def fit(self, X, partition=None, oracle=None):
+    def fit(self, X, oracle, **kwargs):
+        X = self._check_dataset_type(X)
+
         ml, cl = [], []
         constraints = {"ml": ml, "cl": cl}
         candidates = [np.random.choice(range(X.shape[0]), size=2, replace=False).tolist() for _ in range(oracle.budget)]
 
         for i, j in candidates:
-            must_linked = oracle.query(i, j)
-            if must_linked:
+            if oracle.query(i, j):
                 ml.append((i, j))
             else:
                 cl.append((i, j))
 
         return constraints
```

### Comparing `scikit-query-0.1/skquery/pairwise/SASC.py` & `scikit-query-0.1.1/skquery/pairwise/SASC.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
         self.alpha = alpha
         self.svdd_clusters = []
         self.support_vectors = []
         self.label_svdds = []
         self.distance_svdd = []
         self.max = 0
 
-    def fit(self, X, partition, oracle):
-        self.partition = partition
+    def fit(self, X, oracle, **kwargs):
         #self._svdd_clusters(X)
         self._svdd(X)
         self._distance_frontiere(X)
 
         c_t = []
         ml = []
         cl = []
```

### Comparing `scikit-query-0.1/skquery/utils/BaseSVDD.py` & `scikit-query-0.1.1/skquery/utils/BaseSVDD.py`

 * *Files 0% similar despite different names*

```diff
@@ -602,9 +602,9 @@
             ax3.scatter(line.allsegs[0][i][:, 0], line.allsegs[0][i][:, 1], c="orange")
 
         ax3.legend(["Data", "Support vectors"] if self.y_type == "single" else ["Data (+)", "Data (-)", "Support vectors"],
                    ncol=1, loc='upper left', edgecolor='black',
                    markerscale=1.2, fancybox=True)
 
         plt.grid()
-        plt.show()
+        #plt.show()
         return line.allsegs[0]
```

### Comparing `scikit-query-0.1/skquery/utils/line_intercept.py` & `scikit-query-0.1.1/skquery/utils/line_intercept.py`

 * *Files identical despite different names*

