# Comparing `tmp/quik-ai-1.0.1.tar.gz` & `tmp/quik-ai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quik-ai-1.0.1.tar", last modified: Sat Jun 10 17:43:42 2023, max compression
+gzip compressed data, was "quik-ai-1.0.2.tar", last modified: Sun Jun 11 11:02:00 2023, max compression
```

## Comparing `quik-ai-1.0.1.tar` & `quik-ai-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 17:43:42.283012 quik-ai-1.0.1/
--rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2262 2023-06-10 17:43:42.284011 quik-ai-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1724 2023-06-10 03:32:27.000000 quik-ai-1.0.1/README.md
--rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      768 2023-06-10 17:43:42.294007 quik-ai-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 17:43:42.216522 quik-ai-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 17:43:42.254092 quik-ai-1.0.1/src/quik_ai/
--rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.0.1/src/quik_ai/__init__.py
--rw-rw-rw-   0        0        0     2158 2023-06-05 20:31:06.000000 quik-ai-1.0.1/src/quik_ai/backend.py
--rw-rw-rw-   0        0        0    11609 2023-06-08 23:02:28.000000 quik-ai-1.0.1/src/quik_ai/engine.py
--rw-rw-rw-   0        0        0     4917 2023-06-07 22:39:50.000000 quik-ai-1.0.1/src/quik_ai/heads.py
--rw-rw-rw-   0        0        0    18541 2023-06-08 20:45:11.000000 quik-ai-1.0.1/src/quik_ai/layers.py
--rw-rw-rw-   0        0        0      940 2023-06-07 22:39:39.000000 quik-ai-1.0.1/src/quik_ai/losses.py
--rw-rw-rw-   0        0        0     1291 2023-06-10 01:46:43.000000 quik-ai-1.0.1/src/quik_ai/metrics.py
--rw-rw-rw-   0        0        0    29903 2023-06-10 15:57:06.000000 quik-ai-1.0.1/src/quik_ai/models.py
--rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.0.1/src/quik_ai/optimizers.py
--rw-rw-rw-   0        0        0     8285 2023-06-10 16:20:00.000000 quik-ai-1.0.1/src/quik_ai/predictors.py
--rw-rw-rw-   0        0        0     9621 2023-06-08 21:13:03.000000 quik-ai-1.0.1/src/quik_ai/tuners.py
--rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.0.1/src/quik_ai/tuning.py
-drwxrwxrwx   0        0        0        0 2023-06-10 17:43:42.282049 quik-ai-1.0.1/src/quik_ai.egg-info/
--rw-rw-rw-   0        0        0     2262 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 11:02:00.979385 quik-ai-1.0.2/
+-rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2262 2023-06-11 11:02:00.980392 quik-ai-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1724 2023-06-10 03:32:27.000000 quik-ai-1.0.2/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      768 2023-06-11 11:02:00.983373 quik-ai-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:02:00.814022 quik-ai-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 11:02:00.949697 quik-ai-1.0.2/src/quik_ai/
+-rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.0.2/src/quik_ai/__init__.py
+-rw-rw-rw-   0        0        0     2437 2023-06-11 01:06:26.000000 quik-ai-1.0.2/src/quik_ai/backend.py
+-rw-rw-rw-   0        0        0    10544 2023-06-11 11:01:12.000000 quik-ai-1.0.2/src/quik_ai/engine.py
+-rw-rw-rw-   0        0        0     4917 2023-06-07 22:39:50.000000 quik-ai-1.0.2/src/quik_ai/heads.py
+-rw-rw-rw-   0        0        0    18541 2023-06-08 20:45:11.000000 quik-ai-1.0.2/src/quik_ai/layers.py
+-rw-rw-rw-   0        0        0      940 2023-06-07 22:39:39.000000 quik-ai-1.0.2/src/quik_ai/losses.py
+-rw-rw-rw-   0        0        0     1291 2023-06-10 01:46:43.000000 quik-ai-1.0.2/src/quik_ai/metrics.py
+-rw-rw-rw-   0        0        0    29903 2023-06-10 15:57:06.000000 quik-ai-1.0.2/src/quik_ai/models.py
+-rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.0.2/src/quik_ai/optimizers.py
+-rw-rw-rw-   0        0        0     8204 2023-06-11 01:25:52.000000 quik-ai-1.0.2/src/quik_ai/predictors.py
+-rw-rw-rw-   0        0        0     9621 2023-06-08 21:13:03.000000 quik-ai-1.0.2/src/quik_ai/tuners.py
+-rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.0.2/src/quik_ai/tuning.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:02:00.978382 quik-ai-1.0.2/src/quik_ai.egg-info/
+-rw-rw-rw-   0        0        0     2262 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/top_level.txt
```

### Comparing `quik-ai-1.0.1/LICENSE` & `quik-ai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/PKG-INFO` & `quik-ai-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.2.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quik-ai-1.0.1/README.md` & `quik-ai-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/setup.cfg` & `quik-ai-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7569 6b2d 6169 0d0a 7665 7273   = quik-ai..vers
-00000020: 696f 6e20 3d20 312e 302e 310d 0a61 7574  ion = 1.0.1..aut
+00000020: 696f 6e20 3d20 312e 302e 320d 0a61 7574  ion = 1.0.2..aut
 00000030: 686f 7220 3d20 416c 656b 7361 6e64 7220  hor = Aleksandr 
 00000040: 546f 757a 6f76 0d0a 6465 7363 7269 7074  Touzov..descript
 00000050: 696f 6e20 3d20 5175 6963 6b20 556e 6966  ion = Quick Unif
 00000060: 7969 6e67 2049 6e66 7261 7374 7275 6374  ying Infrastruct
 00000070: 7572 6520 4b69 7420 666f 7220 4d61 6368  ure Kit for Mach
 00000080: 696e 6520 4c65 6172 6e69 6e67 2061 6e64  ine Learning and
 00000090: 2041 490d 0a6c 6f6e 675f 6465 7363 7269   AI..long_descri
@@ -16,15 +16,15 @@
 000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000100: 2f74 6f75 7a6f 7631 3031 322f 7175 696b  /touzov1012/quik
 00000110: 2d61 690d 0a64 6f77 6e6c 6f61 645f 7572  -ai..download_ur
 00000120: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000130: 7562 2e63 6f6d 2f74 6f75 7a6f 7631 3031  ub.com/touzov101
 00000140: 322f 7175 696b 2d61 692f 6172 6368 6976  2/quik-ai/archiv
 00000150: 652f 7265 6673 2f74 6167 732f 7631 2e30  e/refs/tags/v1.0
-00000160: 2e31 2e74 6172 2e67 7a0d 0a63 6c61 7373  .1.tar.gz..class
+00000160: 2e32 2e74 6172 2e67 7a0d 0a63 6c61 7373  .2.tar.gz..class
 00000170: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
 00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
 000001a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001b0: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
 000001c0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
 000001d0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
```

### Comparing `quik-ai-1.0.1/src/quik_ai/backend.py` & `quik-ai-1.0.2/src/quik_ai/backend.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,14 +60,22 @@
         if data[col].dtype.kind in 'biu':
             new_df[col] = new_df[col].fillna(0).astype(data[col].dtype)
         else:
             new_df[col] = new_df[col].astype(data[col].dtype)
     
     return new_df
 
+def get_k_from_end(data, k, fill=0):
+    rows = len(data)
+    if rows >= k:
+        return data[-k:]
+    else:
+        pad_rows = np.full((k-rows, data.shape[1]), fill) if len(data.shape) > 1 else np.full((k-rows,), fill)
+        return np.concatenate((pad_rows, data), axis=0)
+
 def train_val_test_split(df, p=[0.8,0.1,0.1]):
     
     n0 = int(df.shape[0] * p[0])
     n1 = int(df.shape[0] * (p[0] + p[1]))
     n2 = int(df.shape[0] * (p[0] + p[1] + p[2]))
     
     df_train = df.iloc[0:n0].reset_index(drop=True)
```

### Comparing `quik-ai-1.0.1/src/quik_ai/engine.py` & `quik-ai-1.0.2/src/quik_ai/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,162 +82,135 @@
         if self.max_steps_per_epoch is not None:
             return min(self.max_steps_per_epoch, steps_per_epoch)
         return steps_per_epoch
     
     def get_validation_steps_per_epoch(self, hp):
         return max(self.validation_data.shape[0] // self.get_parameters(hp)['batch_size'], 1)
     
-    def __get_phantom_time_data(self, data, time_window):
-        
-        # we have no time series data
-        if time_window <= 1:
-            return []
-        
-        # we dont have a time group, but want to make sure there is enough data in our time window
-        if self.time_group_column is None:
-            extras = backend.nan_copy_of_size(time_window - 1, data)
-            extras = backend.fillna(extras)
-            return [extras]
-        
-        to_append = []
-        group_counts = data.groupby(self.time_group_column).size().to_dict()
-        for key, value in group_counts.items():
-            # append empty data
-            extras = backend.nan_copy_of_size(time_window - 1, data)
-            extras = backend.fillna(extras)
-            extras[self.time_group_column] = key
-            to_append.append(extras)
-            
-        return to_append
-    
     def __get_partitioned_data(self, data, input_names, response):
         
         # cache the names of the columns
         names_flt = []
         names_str = []
         for name in input_names:
             if self.get_input_dtype(name) == tf.string:
                 names_str.append(name)
             else:
                 names_flt.append(name)
         
-        # get the str and float parts of the new_data
-        Xf = data[names_flt].astype(np.float32).reset_index(drop=True)
-        Xs = data[names_str].astype(str).reset_index(drop=True)
+        # the array may be shuffled, but the index of the true order remains
+        # we need to build a map to the locations of the new ordered elements
+        row_order = data.index.to_numpy()
         
-        # generate Y and W if we have them
-        Y = data[response].reset_index(drop=True) if response is not None else None
-        W = data[self.weights_column].reset_index(drop=True) if self.weights_column is not None else None
+        # create a dictionary from the shuffled list with numbers as keys and their indices as values
+        row_order = {number: index for index, number in enumerate(row_order)}
+
+        # create a new list with the indices of the numbers from 0 to n-1 in the shuffled list
+        row_order = [row_order[i] for i in range(data.shape[0])]
         
-        # remove W if no response
-        W = None if Y is None else W
+        # cache the group order
+        group_order = data.__group_id__.to_numpy() if self.time_group_column is not None else None
         
-        return names_flt, Xf, names_str, Xs, Y, W
-    
-    def __build_data_time_groups(self, data, Xf, Xs, Y, W):
-        # mapping for all data arrays
-        indices = { '__ALL__' : Xf[[]] }
-        Xf_dict = { '__ALL__' : Xf.to_numpy() }
-        Xs_dict = { '__ALL__' : Xs.to_numpy() }
-        Y_dict = { '__ALL__' : Y.to_numpy() if Y is not None else None }
-        W_dict = { '__ALL__' : W.to_numpy() if W is not None else None }
-        
-        # no time groups
-        if self.time_group_column is None:
-            return indices, Xf_dict, Xs_dict, Y_dict, W_dict, None
-        
-        time_group = data[self.time_group_column].reset_index(drop=True)
-        for val in time_group.unique():
-            flags = time_group == val
-            indices[val] = indices['__ALL__'][flags]
-            Xf_dict[val] = Xf_dict['__ALL__'][flags]
-            Xs_dict[val] = Xs_dict['__ALL__'][flags]
-            Y_dict[val] = Y_dict['__ALL__'][flags] if Y_dict['__ALL__'] is not None else None
-            W_dict[val] = W_dict['__ALL__'][flags] if W_dict['__ALL__'] is not None else None
-            
-        return indices, Xf_dict, Xs_dict, Y_dict, W_dict, time_group
+        # get the str and float parts of the new_data
+        x_flt = data[names_flt].astype(np.float32).to_numpy()
+        x_str = data[names_str].astype(str).to_numpy()
+        
+        # generate y and w if we have them
+        y = data[response].to_numpy() if response is not None else None
+        w = data[self.weights_column].to_numpy() if self.weights_column is not None else None
+        
+        # remove w if no response
+        w = None if y is None else w
+        
+        return {
+            'row_order' : row_order,
+            'group_order' : group_order,
+            'names_flt' : names_flt,
+            'names_str' : names_str,
+            'x_flt' : x_flt,
+            'x_str' : x_str,
+            'y' : y,
+            'w' : w,
+        }
     
     def __get_tensorflow_generator(
         self, 
         data, 
         input_names, 
         response, 
         run_forever,
         time_window, 
         batch_size, 
         shuffle, 
         **kwargs
-    ):
+    ):  
+        # presort by index
+        data = data.sort_index()
+        
+        # if we have a time group, first sort by group
+        if self.time_group_column is not None:
+            data = data.reset_index().rename(columns={'index': '__group_id__'})
+            data = data.sort_values(by=[self.time_group_column, '__group_id__'])
+            data['__group_id__'] = data.groupby(self.time_group_column).cumcount()
+        
+        # split the data into different type tensors and get the
+        # order of the rows as well as the element of the row in
+        # each group if we have a time group
+        cache = self.__get_partitioned_data(data, input_names, response)
         
-        # get additional buffer data for our time series
-        to_append = self.__get_phantom_time_data(data, time_window)
-        
-        # add the buffer
-        original_data_count = data.shape[0]
-        if to_append:
-            to_append.append(data)
-            data = pd.concat(to_append, ignore_index=True)
-        
-        # split the data into different types
-        Xf_names, Xf, Xs_names, Xs, Y, W = self.__get_partitioned_data(data, input_names, response)
-        
-        # build numpy tensors which will be read in generator, key by time group
-        indices, Xf_dict, Xs_dict, Y_dict, W_dict, time_group = self.__build_data_time_groups(data, Xf, Xs, Y, W)
-        
-        # generator for getting data from the dataframe
-        ends = np.arange(data.shape[0] - original_data_count, data.shape[0])
+        # get the order of our results
+        row_order = cache['row_order']
         
         # build the generator
         def generator():
             while True:
                 # shuffle if we need to
                 if shuffle:
-                    np.random.shuffle(ends)
+                    np.random.shuffle(row_order)
 
                 # yield loop to iterate over the data
-                for end in ends:
-
-                    # cut off data after end
-                    Xf = Xf_dict['__ALL__'][:end+1]
-                    Xs = Xs_dict['__ALL__'][:end+1]
-                    Y = Y_dict['__ALL__'][:end+1] if Y_dict['__ALL__'] is not None else None
-                    W = W_dict['__ALL__'][:end+1] if W_dict['__ALL__'] is not None else None
-
-                    # filter to sub-array if we have a time group
-                    if self.time_group_column is not None:
-                        group_type = time_group[end]
-                        end_loc = indices[group_type].index.get_loc(end)
-                        Xf = Xf_dict[group_type][:end_loc+1]
-                        Xs = Xs_dict[group_type][:end_loc+1]
-                        Y = Y_dict[group_type][:end_loc+1] if Y is not None else None
-                        W = W_dict[group_type][:end_loc+1] if W is not None else None
+                for end in row_order:
+                    
+                    # filter to sub-array depending on if we have a time group
+                    if self.time_group_column is None:
+                        x_flt = cache['x_flt'][:end+1]
+                        x_str = cache['x_str'][:end+1]
+                        y = cache['y'][:end+1] if cache['y'] is not None else None
+                        w = cache['w'][:end+1] if cache['w'] is not None else None
+                    else:
+                        group_id = cache['group_order'][end]
+                        x_flt = cache['x_flt'][end-group_id:end+1]
+                        x_str = cache['x_str'][end-group_id:end+1]
+                        y = cache['y'][end-group_id:end+1] if cache['y'] is not None else None
+                        w = cache['w'][end-group_id:end+1] if cache['w'] is not None else None
 
-                    # different fetch for time series and flat array
+                    # different fetch for time series and flat array, we may need to pad
+                    # the time series if it there is not enough history
                     if time_window >= 2:
-                        Xf = np.squeeze(np.lib.stride_tricks.sliding_window_view(Xf[-time_window:], (time_window, Xf.shape[1])), axis=(0,1))
-                        Xs = np.squeeze(np.lib.stride_tricks.sliding_window_view(Xs[-time_window:], (time_window, Xs.shape[1])), axis=(0,1))
+                        x_flt = backend.get_k_from_end(x_flt, time_window, fill=0)
+                        x_str = backend.get_k_from_end(x_str, time_window, fill='[UNK]')
                     else:
-                        Xf = Xf[-1]
-                        Xs = Xs[-1]
-
-                    X_keys = []
-                    X_vals = []
-                    if len(Xf_names) > 0:
-                        X_keys += Xf_names
-                        X_vals += np.split(Xf, Xf.shape[-1], axis=-1)
-                    if len(Xs_names) > 0:
-                        X_keys += Xs_names
-                        X_vals += np.split(Xs, Xs.shape[-1], axis=-1)
-                    if Y is None:
-                        yield dict(zip(X_keys, X_vals))
+                        x_flt = x_flt[-1]
+                        x_str = x_str[-1]
+                        
+                    # combine the predictor names
+                    x_keys = [*cache['names_flt'], *cache['names_str']]
+                    
+                    # combine the predictor vectors
+                    x_flt_vals = [] if x_flt.shape[-1] == 0 else np.split(x_flt, x_flt.shape[-1], axis=-1)
+                    x_str_vals = [] if x_str.shape[-1] == 0 else np.split(x_str, x_str.shape[-1], axis=-1)
+                    x_vals = [*x_flt_vals, *x_str_vals]
+                    
+                    if y is None:
+                        yield dict(zip(x_keys, x_vals))
                     else:
-                        if W is None:
-                            yield (dict(zip(X_keys, X_vals)), Y[-1])
+                        if w is None:
+                            yield (dict(zip(x_keys, x_vals)), y[-1])
                         else:
-                            yield (dict(zip(X_keys, X_vals)), Y[-1], W[-1])
+                            yield (dict(zip(x_keys, x_vals)), y[-1], w[-1])
                 
                 # should we terminate the forever loop for a single data pass?
                 if not run_forever:
                     break
         
         # we either have a time series or not, if we have a time series
         # we will use the generator to get data to avoid memory overflow
@@ -253,16 +226,16 @@
             
             input_tensor_specs.append(tf.TensorSpec(shape=shape, dtype=dtype))
         
         # build the signature
         output_signature = dict(zip(input_names, input_tensor_specs))
 
         # append the response and weights
-        if Y is not None:
-            if W is None:
+        if cache['y'] is not None:
+            if cache['w'] is None:
                 output_signature = (output_signature, tf.TensorSpec(shape=(), dtype=tf.float32))
             else:
                 output_signature = (output_signature, tf.TensorSpec(shape=(), dtype=tf.float32), tf.TensorSpec(shape=(), dtype=tf.float32))
         
         # return the built generator
         return tf.data.Dataset.from_generator(
             generator,
```

### Comparing `quik-ai-1.0.1/src/quik_ai/heads.py` & `quik-ai-1.0.2/src/quik_ai/heads.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/src/quik_ai/layers.py` & `quik-ai-1.0.2/src/quik_ai/layers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/src/quik_ai/losses.py` & `quik-ai-1.0.2/src/quik_ai/losses.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/src/quik_ai/metrics.py` & `quik-ai-1.0.2/src/quik_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/src/quik_ai/models.py` & `quik-ai-1.0.2/src/quik_ai/models.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/src/quik_ai/optimizers.py` & `quik-ai-1.0.2/src/quik_ai/optimizers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/src/quik_ai/predictors.py` & `quik-ai-1.0.2/src/quik_ai/predictors.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             'drop' : self._get_hp(None, 'drop', hp)
         })
         return config
     
     def transform(self, inputs, driver, hp):
         return None
 
-class LambdaPredictor(Predictor):
+class Lambda(Predictor):
     def __init__(self, names, lambdas=None, **kwargs):
         super().__init__(names, **kwargs)
         
         if callable(lambdas):
             lambdas = [lambdas]
         
         if not isinstance(lambdas, (list, tuple)):
@@ -68,15 +68,15 @@
                 res.append(lbda(inputs, driver, **config))
         
         if len(res) == 0:
             return None
         
         return tf.concat(res, axis=-1)
     
-class NumericalPredictor(LambdaPredictor):
+class Numerical(Lambda):
     def __init__(self, names, normalize=False, **kwargs):
         super().__init__(names, lambdas=self.body, **kwargs)
         self.normalize = normalize
     
     def get_parameters(self, hp):
         config = super().get_parameters(hp)
         
@@ -96,15 +96,15 @@
                 outputs.append(normal_layer(inputs[name]))
         else:
             for name in self.names:
                 outputs.append(inputs[name])
         
         return tf.concat(outputs, axis=-1)
 
-class PeriodicPredictor(LambdaPredictor):
+class Periodic(Lambda):
     def __init__(self, names, period, **kwargs):
         super().__init__(names, lambdas=self.body, **kwargs)
         self.period = period
     
     def get_parameters(self, hp):
         config = super().get_parameters(hp)
         
@@ -118,15 +118,15 @@
         
         outputs = tf.concat(outputs, axis=-1)
         
         theta = 2 * np.pi * outputs / period
         
         return tf.concat([tf.math.sin(theta), tf.math.cos(theta)], axis=-1)
     
-class TimeMaskedPredictor(LambdaPredictor):
+class TimeMasked(Lambda):
     def __init__(self, names, mask_n=1, **kwargs):
         super().__init__(names, lambdas=self.body, **kwargs)
         self.mask_n = mask_n
     
     def body(self, inputs, driver, **kwargs):
         outputs = [inputs[name] for name in self.names]
         
@@ -136,15 +136,15 @@
             raise ValueError('Time masked predictor must have at least (3) dimensions')
         
         unmasked, masked = tf.split(outputs, [-1, self.mask_n], axis=1)
         masked = masked * 0.0
         
         return tf.concat([unmasked, masked], axis=1)
 
-class CategoricalPredictor(LambdaPredictor):
+class Categorical(Lambda):
     def __init__(
         self, 
         names, 
         dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
         use_one_hot=tuning.HyperBoolean(),
         embed_dim=tuning.HyperInt(min_value=8, max_value=32, step=8),
         embed_l2_regularizer=tuning.HyperFloat(min_value=0.0, max_value=0.2, step=0.1),
```

### Comparing `quik-ai-1.0.1/src/quik_ai/tuners.py` & `quik-ai-1.0.2/src/quik_ai/tuners.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/src/quik_ai/tuning.py` & `quik-ai-1.0.2/src/quik_ai/tuning.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.1/src/quik_ai.egg-info/PKG-INFO` & `quik-ai-1.0.2/src/quik_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.2.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

