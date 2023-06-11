# Comparing `tmp/Spanve-0.1.1.tar.gz` & `tmp/Spanve-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Spanve-0.1.1.tar", last modified: Thu Feb 16 09:20:53 2023, max compression
+gzip compressed data, was "Spanve-0.1.2.tar", last modified: Sun Jun 11 06:50:40 2023, max compression
```

## Comparing `Spanve-0.1.1.tar` & `Spanve-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 09:20:53.819455 Spanve-0.1.1/
--rw-rw-rw-   0        0        0    11558 2022-11-08 02:57:36.000000 Spanve-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      282 2023-02-16 09:20:53.818455 Spanve-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-16 09:20:53.807453 Spanve-0.1.1/Spanve/
--rw-rw-rw-   0        0        0     2784 2022-11-07 13:06:42.000000 Spanve-0.1.1/Spanve/Spanve_cli.py
--rw-rw-rw-   0        0        0    24825 2023-02-16 09:19:19.000000 Spanve-0.1.1/Spanve/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 09:20:53.816455 Spanve-0.1.1/Spanve.egg-info/
--rw-rw-rw-   0        0        0      282 2023-02-16 09:20:52.000000 Spanve-0.1.1/Spanve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-02-16 09:20:53.000000 Spanve-0.1.1/Spanve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 09:20:52.000000 Spanve-0.1.1/Spanve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-02-16 09:20:52.000000 Spanve-0.1.1/Spanve.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       84 2023-02-16 09:20:52.000000 Spanve-0.1.1/Spanve.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-16 09:20:52.000000 Spanve-0.1.1/Spanve.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-16 09:20:53.820454 Spanve-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-02-16 09:20:15.000000 Spanve-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 06:50:40.587045 Spanve-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2022-11-08 02:57:36.000000 Spanve-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      282 2023-06-11 06:50:40.587045 Spanve-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 06:50:40.580038 Spanve-0.1.2/Spanve/
+-rw-rw-rw-   0        0        0     2784 2022-11-07 13:06:42.000000 Spanve-0.1.2/Spanve/Spanve_cli.py
+-rw-rw-rw-   0        0        0    25793 2023-04-26 07:09:55.000000 Spanve-0.1.2/Spanve/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 06:50:40.586045 Spanve-0.1.2/Spanve.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 06:50:40.587045 Spanve-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-04-21 01:54:04.000000 Spanve-0.1.2/setup.py
```

### Comparing `Spanve-0.1.1/LICENSE` & `Spanve-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Spanve-0.1.1/Spanve/Spanve_cli.py` & `Spanve-0.1.2/Spanve/Spanve_cli.py`

 * *Files identical despite different names*

### Comparing `Spanve-0.1.1/Spanve/__init__.py` & `Spanve-0.1.2/Spanve/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
         adata = anndata.copy()
 
     sc.pp.normalize_total(
         adata,
         exclude_highly_expressed=exclude_highly_expressed,
         )
     sc.pp.log1p(adata)
-    adata.X = ((adata.X / (eps+np.median(adata.X,axis=0))) * np.median(anndata.X,axis=0)).astype(int)
+    expr_median = eps+np.median(adata.X,axis=0)
+    adata.X = ((adata.X / expr_median) * expr_median).astype(int)
 
     return adata
 
 def elbow(X: np.ndarray) -> int:
     max_idx = np.argmax(X)
 
     X = X[max_idx:]  # truncate data from max (not origin) to endpoint.
@@ -224,32 +225,54 @@
         assert self.hypoth_type in ["nodist","possion"], f"hypoth_type should be 'nodist' or 'possion', now get {self.hypoth_type}"
         assert self.X.shape[0] == self.L.shape[0], f"expression data is not consistent with spatial data, now get {self.X.shape[0]} != {self.L.shape[0]}"
 
         if self.adata.X.dtype not in [np.int64, np.int32, np.int16, np.int8, np.int0]:
             warnings.warn("""
             WARNNING: X must be an int matrix; 
             ----------------------------------------
-            Will automatically convert to int. Inputs can be Raw Counts or use `adata_preprocess_int` to get a normalized data with int dtype. """
+            Will NOT automatically convert to int. Inputs can be Raw Counts or use `adata_preprocess_int` to get a normalized data with int dtype. """
             )
 
-    def spatial_coexp(self,search_space):
+    def spatial_coexp(self,search_space,groupby=None,verbose=False):
+        
         def spatial_coexp_single(x,y):
             sample_corr = (x - x.mean()) * (y - y.mean()) / (x.std() * y.std()+1e-7)
             return sample_corr.astype(int)
+        
+        def spatial_coexp_group(adata):
+            newdf = pd.DataFrame(
+                spatial_coexp_single(adata[:,list(var1)].X.toarray(),adata[:,list(var2)].X.toarray()),
+                index = adata.obs_names,
+                columns = [f"{i}~{j}" for i,j in search_space]
+            )
 
+            newad = sc.AnnData(newdf,obsm={'spatial':adata.obsm['spatial']},dtype=int)
+            return newad
+        
         adata = self.adata.copy()
-
-        newdf = pd.DataFrame(
-            index=adata.obs_names,
-            columns=[f"{x}~{y}" for x,y in search_space]
-        )
-        for var1,var2 in search_space:
-            newdf[f"{var1}~{var2}"] = spatial_coexp_single(adata.obs_vector(var1),adata.obs_vector(var2))
+        var1,var2 = zip(*search_space)
+        
+        if groupby is not None:
+            assert groupby in adata.obs.columns, "groupby should be obs columns and should be categories." 
+            groups = adata.obs_vector(groupby)
+            n_groups = np.unique(groups).size
+            newads = []
+            
+            bar = tqdm(total=n_groups,disable=not verbose, desc = f'There are {n_groups} groups. Will cal coexp strength separately.') 
+            for g in np.unique(groups):
+                adata_ = adata[groups==g,:]
+                newad_ = spatial_coexp_group(adata_)
+                newads.append(newad_)
+                bar.update(1)
+            newad = sc.concat(newads)
+            bar.close()
+        else:
+            newad = spatial_coexp_group(adata)
         
-        newad = sc.AnnData(newdf,obsm={'spatial':adata.obsm['spatial']},dtype=int)
+        sc.pp.filter_genes(newad,min_counts=1)
         self.adata = newad
         self.X = newad.X
 
     def possion_hypoth(self, X, verbose=False):
         overall_max = X.max(axis=0)
         n_features = X.shape[1]
         lams = np.std(X, axis=0) ** 2
```

### Comparing `Spanve-0.1.1/setup.py` & `Spanve-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Spanve',
-    version='0.1.1',
+    version='0.1.2',
     description='Spatial Neighbourhood Variably Expressed (Spanve) is a method for detecting spatially expressed genes in spatial transcriptomics data.',
     url='https://github.com/gx-Cai/Spanve',
     author='gx.Cai',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
-        'numpy<=1.21',
+        'numpy',
         'scanpy',
         'scipy>=1.8',
         'joblib',
         'scikit-learn',
         'statsmodels',
         'tqdm',
         'click'
```

