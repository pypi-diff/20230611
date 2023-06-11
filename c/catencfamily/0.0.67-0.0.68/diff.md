# Comparing `tmp/catencfamily-0.0.67.tar.gz` & `tmp/catencfamily-0.0.68.tar.gz`

## Comparing `catencfamily-0.0.67.tar` & `catencfamily-0.0.68.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.67/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.67/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    29710 2020-02-02 00:00:00.000000 catencfamily-0.0.67/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.67/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.67/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.67/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.67/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.68/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.68/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    30649 2020-02-02 00:00:00.000000 catencfamily-0.0.68/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.68/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.68/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.68/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.68/PKG-INFO
```

### Comparing `catencfamily-0.0.67/src/catencfamily/encoders.py` & `catencfamily-0.0.68/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.67/src/catencfamily/utils.py` & `catencfamily-0.0.68/src/catencfamily/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -826,98 +826,128 @@
     # Transform d to pandas Series:
     d = pd.Series(d).sort_values(ascending = False)
     if (normalize):
         d = d/sum(d)
     return d
        
        
-def plotBipartiteGraph(filename, pathToFolder):
+def plotBipartiteGraph(filename, pathToFolder,connected = False):
     """
     Plots a bipartitie graph.  
     
     Parameters
     ----------
     filename : Filename
     pathToFolder : Folder where file resides
-
+    connected: Boolean; Show only connected nodes
+               Default is False
     Returns
     -------
     None.
 
     """
     filepath = pathToFolder / filename
     G = nx.read_gml(filepath) 
-    #gcc = max(nx.connected_components(G), key=lambda x: len(x))
-    # subgraph of connected nodes:
-    # H = G.subgraph(gcc)
+    if connected:
+      gcc = max(nx.connected_components(G), key=lambda x: len(x))
+      # subgraph of connected nodes:
+      H = G.subgraph(gcc)
+      GH = H
+    else:
+      GH = G  
     color_dict = {0:'b',1:'r'}
-    color_list = [color_dict[i[1]] for i in G.nodes.data('bipartite')]
+    color_list = [color_dict[i[1]] for i in GH.nodes.data('bipartite')]
     color_list
-    pos = nx.spring_layout(G, k = None, scale = 4, iterations = 1000)
+    pos = nx.spring_layout(GH, k = None, scale = 4, iterations = 1000)
     plt.figure(figsize= (10,5));
     ax = plt.gca();
-    nx.draw(G, 
+    nx.draw(GH, 
             pos= pos,
             node_size=30,
             with_labels =  False,
             font_size = 10,
             node_color = color_list,
             ax =ax,
             width = 0.1  # edge width
             );
 
 
-
-def plotUnipartiteGraph(filename, pathToFolder):
+def plotUnipartiteGraph(filename, pathToFolder, connected=False):
     """
     Plots a unipartite graph
     Parameters
     ----------
     filename : graph file.
     pathToFolder : Path to folder of graph file.
     Returns
     -------
     None.
 
     """
     filepath = pathToFolder / filename
     G = nx.read_gml(filepath) 
-    #gcc = max(nx.connected_components(G), key=lambda x: len(x))
-    # subgraph of connected nodes:
-    #H = G.subgraph(gcc)
-    pos = nx.spring_layout(G, k = None)
+    if connected:
+        gcc = max(nx.connected_components(G), key=lambda x: len(x))
+        # subgraph of connected nodes:
+        H = G.subgraph(gcc)
+        GH = H
+    else:
+        GH = G
+    pos = nx.spring_layout(GH, k = None)
     plt.figure(figsize= (10,5));
     ax = plt.gca();
-    nx.draw(G, 
+    nx.draw(GH, 
             pos= pos,
             node_size=30,
             with_labels =  False,
             font_size = 10,
             ax =ax,
             width = 0.1  # edge width
             );
     
     
 # Community visualization
 # Kaggle: https://www.kaggle.com/code/rahulgoel1106/commmunity-detection-using-igraph-and-networkx
-def communityVisualization(G, withLabels = False, font_size = 8):
-    colors = ["orange", "yellow", "white"]
+def communityVisualization(filename, pathToFolder,withLabels = False, font_size = 8, edgewidth = 0.1, colorList =  ["orange", "yellow", "white"]):
+    """
+    Desc
+    ----
+    Displays communities created by modularity class.
+
+    Parameters
+    ----------
+    filename : str, Graph file
+    pathToFolder : str, Path to folder having graph files
+    withLabels : boolean, Should labels be displayed? The default is False.
+    font_size : int, Label font size. The default is 8.
+    edgewidth: float, Edge line width
+    colorList: List of colors for difft communitied. 
+               Default is: ["orange", "yellow", "white"]
+
+    Returns
+    -------
+    None.
+
+    """
+    filepath = pathToFolder / filename
+    G = nx.read_gml(filepath) 
+    colors = colorList
     pos = nx.spring_layout(G)
     lst_b = nx.community.greedy_modularity_communities(G)
     color_map_b = {}
     keys = G.nodes()
     values = "black"
     for i in keys:
             color_map_b[i] = values
     counter = 0
     for x in lst_b:
       for n in x:
         color_map_b[n] = colors[counter]
       counter = counter + 1
-    nx.draw_networkx_edges(G, pos, width = 0.1);
+    nx.draw_networkx_edges(G, pos, width = edgewidth);
     nx.draw_networkx_nodes(G, pos, node_color=dict(color_map_b).values());
     if withLabels:
       nx.draw_networkx_labels(G, pos, font_size = font_size, font_weight = 'bold')
     plt.axis("off");
     plt.show();    
     
 ################### That's all folks #######################
```

### Comparing `catencfamily-0.0.67/LICENSE` & `catencfamily-0.0.68/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.67/README.md` & `catencfamily-0.0.68/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.67/pyproject.toml` & `catencfamily-0.0.68/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.67"
+version = "0.0.68"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.67/PKG-INFO` & `catencfamily-0.0.68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.67
+Version: 0.0.68
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

