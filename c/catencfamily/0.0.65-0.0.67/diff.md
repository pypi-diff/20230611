# Comparing `tmp/catencfamily-0.0.65.tar.gz` & `tmp/catencfamily-0.0.67.tar.gz`

## Comparing `catencfamily-0.0.65.tar` & `catencfamily-0.0.67.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.65/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89414 2020-02-02 00:00:00.000000 catencfamily-0.0.65/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    26450 2020-02-02 00:00:00.000000 catencfamily-0.0.65/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.65/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.65/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.65/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.65/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.67/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.67/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    29710 2020-02-02 00:00:00.000000 catencfamily-0.0.67/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.67/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.67/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.67/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.67/PKG-INFO
```

### Comparing `catencfamily-0.0.65/src/catencfamily/encoders.py` & `catencfamily-0.0.67/src/catencfamily/encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -2070,55 +2070,9 @@
                 ax.set_title('Projected graph of ' + colToProject + ' (all nodes) as seen through ' + intermediaryCol) 
                 ax.title.set_size(20)  # title font size
                 ax.title.set_weight('bold')
                 pos = nx.spring_layout(G, k = k)
                 nx.draw_networkx(G,pos = pos, node_size=30, with_labels =  withLabels, font_size=fontSize, node_color = 'r', ax =ax)
         return
     
-                
-       
-
-
-############################
-# https://stackoverflow.com/a/60186800/3282777
-class FeatureTransformer:
-    
-    def __init__(self, categorical_features):
-        self.categorical_features = categorical_features
-        
-    def fit(self, X):
-
-        if not isinstance(X, pd.DataFrame):
-            raise ValueError("Pass a pandas.DataFrame")
-            
-        if not isinstance(self.categorical_features, list):
-            raise ValueError(
-                "Pass categorical_features as a list of column names")
-                    
-        self.encoding = {}
-        for c in self.categorical_features:
-
-            _, int_id = X[c].factorize()
-            self.encoding[c] = dict(zip(list(int_id), range(1,len(int_id)+1)))
-            
-        return self
-
-    def transform(self, X, onehot=True):
-
-        if not isinstance(X, pd.DataFrame):
-            raise ValueError("Pass a pandas.DataFrame")
-
-        if not hasattr(self, 'encoding'):
-            raise AttributeError("FeatureTransformer must be fitted")
-            
-        df = X.drop(self.categorical_features, axis=1)
-        
-        if onehot:  # one-hot encoding
-            for c in sorted(self.categorical_features):            
-                categories = X[c].map(self.encoding[c]).values
-                for val in self.encoding[c].values():
-                    df["{}_{}".format(c,val)] = (categories == val).astype('int16')
-        else:       # label encoding
-            for c in sorted(self.categorical_features):
-                df[c] = X[c].map(self.encoding[c]).fillna(0)
-            
-        return df
+ ###############333##################               
+
```

### Comparing `catencfamily-0.0.65/src/catencfamily/utils.py` & `catencfamily-0.0.67/src/catencfamily/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# 6th June, 2023
+# 11th June, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import kurtosis
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 from sklearn.datasets import make_classification
 from sklearn.feature_selection import  mutual_info_classif
+import networkx as nx
 import pickle
 import pathlib
 import string
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 
@@ -717,14 +718,30 @@
     """
     Desc
     ----
     In the colList, how many columns pertain to
     degree centrality, eigenvector centrality,
     page-rank and clustering coeff. Plot
     by using plotSeries().
+    
+    Example:
+        Here is a table of col-name wise xgboost impt score
+        
+        deg_abc   0.01
+        pr_cde    0.02
+        pr_def    0.015
+        eig_xy    0.11
+        deg_ff    0.001
+        deg_uy    0.01
+        
+    Result (normalized):
+        
+        degree      3/6
+        pagerank    2/6
+        eigenvector 1/6
 
     Parameters
     ----------
     colList : A list of columns
     normalize: Boolean
 
     Returns
@@ -760,14 +777,28 @@
     """
     Desc
     ----
     In the colList, total score of columns
     that pertain to degree centrality, to eigenvector
     centrality, to page-rank and clustering coeff and 
     others. Plot by using plotSeries().
+    
+    Example:
+        Here is a table of col-name wise xgboost impt score
+        
+        deg_abc   0.01
+        pr_cde    0.02
+        pr_def    0.015
+        eig_xy    0.11
+        deg_ff    0.001
+        
+    Result:
+        degree      0.011
+        pagerank    0.035
+        eigenvector 0.11
 
     Parameters
     ----------
     score: Pandas Series giving column wise impt score
     colList : A list of dataframe columns
     normalize: Boolean
 
@@ -794,14 +825,102 @@
     d['leidencomsdensity'] = score[den].sum()
     # Transform d to pandas Series:
     d = pd.Series(d).sort_values(ascending = False)
     if (normalize):
         d = d/sum(d)
     return d
        
-           
+       
+def plotBipartiteGraph(filename, pathToFolder):
+    """
+    Plots a bipartitie graph.  
+    
+    Parameters
+    ----------
+    filename : Filename
+    pathToFolder : Folder where file resides
+
+    Returns
+    -------
+    None.
+
+    """
+    filepath = pathToFolder / filename
+    G = nx.read_gml(filepath) 
+    #gcc = max(nx.connected_components(G), key=lambda x: len(x))
+    # subgraph of connected nodes:
+    # H = G.subgraph(gcc)
+    color_dict = {0:'b',1:'r'}
+    color_list = [color_dict[i[1]] for i in G.nodes.data('bipartite')]
+    color_list
+    pos = nx.spring_layout(G, k = None, scale = 4, iterations = 1000)
+    plt.figure(figsize= (10,5));
+    ax = plt.gca();
+    nx.draw(G, 
+            pos= pos,
+            node_size=30,
+            with_labels =  False,
+            font_size = 10,
+            node_color = color_list,
+            ax =ax,
+            width = 0.1  # edge width
+            );
+
+
+
+def plotUnipartiteGraph(filename, pathToFolder):
+    """
+    Plots a unipartite graph
+    Parameters
+    ----------
+    filename : graph file.
+    pathToFolder : Path to folder of graph file.
+    Returns
+    -------
+    None.
 
+    """
+    filepath = pathToFolder / filename
+    G = nx.read_gml(filepath) 
+    #gcc = max(nx.connected_components(G), key=lambda x: len(x))
+    # subgraph of connected nodes:
+    #H = G.subgraph(gcc)
+    pos = nx.spring_layout(G, k = None)
+    plt.figure(figsize= (10,5));
+    ax = plt.gca();
+    nx.draw(G, 
+            pos= pos,
+            node_size=30,
+            with_labels =  False,
+            font_size = 10,
+            ax =ax,
+            width = 0.1  # edge width
+            );
+    
+    
+# Community visualization
+# Kaggle: https://www.kaggle.com/code/rahulgoel1106/commmunity-detection-using-igraph-and-networkx
+def communityVisualization(G, withLabels = False, font_size = 8):
+    colors = ["orange", "yellow", "white"]
+    pos = nx.spring_layout(G)
+    lst_b = nx.community.greedy_modularity_communities(G)
+    color_map_b = {}
+    keys = G.nodes()
+    values = "black"
+    for i in keys:
+            color_map_b[i] = values
+    counter = 0
+    for x in lst_b:
+      for n in x:
+        color_map_b[n] = colors[counter]
+      counter = counter + 1
+    nx.draw_networkx_edges(G, pos, width = 0.1);
+    nx.draw_networkx_nodes(G, pos, node_color=dict(color_map_b).values());
+    if withLabels:
+      nx.draw_networkx_labels(G, pos, font_size = font_size, font_weight = 'bold')
+    plt.axis("off");
+    plt.show();    
     
-############################ BEGIN ###################
+################### That's all folks #######################
```

### Comparing `catencfamily-0.0.65/LICENSE` & `catencfamily-0.0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.65/README.md` & `catencfamily-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.65/pyproject.toml` & `catencfamily-0.0.67/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.65"
+version = "0.0.67"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.65/PKG-INFO` & `catencfamily-0.0.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.65
+Version: 0.0.67
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

