# Comparing `tmp/itables-1.5.2.tar.gz` & `tmp/itables-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/itables-1.5.2.tar", last modified: Sun Mar 26 18:42:45 2023, max compression
+gzip compressed data, was "dist/itables-1.5.3.tar", last modified: Sun Jun 11 13:29:07 2023, max compression
```

## Comparing `itables-1.5.2.tar` & `itables-1.5.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 18:42:45.000000 itables-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (122)     6978 2023-03-26 18:42:45.000000 itables-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5028 2023-03-26 18:42:42.000000 itables-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 18:42:45.000000 itables-1.5.2/itables/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-03-26 18:42:42.000000 itables-1.5.2/itables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-03-26 18:42:42.000000 itables-1.5.2/itables/datatables_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-03-26 18:42:42.000000 itables-1.5.2/itables/downsample.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 18:42:45.000000 itables-1.5.2/itables/external/
--rw-r--r--   0 runner    (1001) docker     (122)    18399 2023-03-26 18:42:44.000000 itables-1.5.2/itables/external/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   450575 2023-03-26 18:42:45.000000 itables-1.5.2/itables/external/jquery.dataTables.mjs
--rw-r--r--   0 runner    (1001) docker     (122)    89501 2023-03-26 18:42:44.000000 itables-1.5.2/itables/external/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 18:42:45.000000 itables-1.5.2/itables/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 18:42:45.000000 itables-1.5.2/itables/html/column_filters/
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-03-26 18:42:42.000000 itables-1.5.2/itables/html/column_filters/initComplete.js
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-03-26 18:42:42.000000 itables-1.5.2/itables/html/column_filters/pre_dt_code.js
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-03-26 18:42:42.000000 itables-1.5.2/itables/html/datatables_template.html
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-03-26 18:42:42.000000 itables-1.5.2/itables/html/datatables_template_connected.html
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-03-26 18:42:42.000000 itables-1.5.2/itables/html/initialize_offline_datatable.html
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-03-26 18:42:42.000000 itables-1.5.2/itables/html/itables.css
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-03-26 18:42:42.000000 itables-1.5.2/itables/interactive.py
--rw-r--r--   0 runner    (1001) docker     (122)    14803 2023-03-26 18:42:42.000000 itables-1.5.2/itables/javascript.py
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-03-26 18:42:42.000000 itables-1.5.2/itables/options.py
--rw-r--r--   0 runner    (1001) docker     (122)    11770 2023-03-26 18:42:42.000000 itables-1.5.2/itables/sample_dfs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 18:42:45.000000 itables-1.5.2/itables/samples/
--rw-r--r--   0 runner    (1001) docker     (122)    31715 2023-03-26 18:42:42.000000 itables-1.5.2/itables/samples/countries.csv
--rw-r--r--   0 runner    (1001) docker     (122)   420013 2023-03-26 18:42:42.000000 itables-1.5.2/itables/samples/indicators.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6390 2023-03-26 18:42:42.000000 itables-1.5.2/itables/samples/population.csv
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-03-26 18:42:42.000000 itables-1.5.2/itables/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-03-26 18:42:42.000000 itables-1.5.2/itables/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 18:42:45.000000 itables-1.5.2/itables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6978 2023-03-26 18:42:45.000000 itables-1.5.2/itables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-26 18:42:45.000000 itables-1.5.2/itables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-26 18:42:45.000000 itables-1.5.2/itables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-03-26 18:42:45.000000 itables-1.5.2/itables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-26 18:42:45.000000 itables-1.5.2/itables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-26 18:42:42.000000 itables-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-03-26 18:42:45.000000 itables-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-03-26 18:42:42.000000 itables-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 13:29:07.000000 itables-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     6978 2023-06-11 13:29:07.000000 itables-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5028 2023-06-11 13:29:03.000000 itables-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 13:29:07.000000 itables-1.5.3/itables/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-11 13:29:03.000000 itables-1.5.3/itables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-06-11 13:29:03.000000 itables-1.5.3/itables/datatables_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-06-11 13:29:03.000000 itables-1.5.3/itables/downsample.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 13:29:07.000000 itables-1.5.3/itables/external/
+-rw-r--r--   0 runner    (1001) docker     (122)    18399 2023-06-11 13:29:06.000000 itables-1.5.3/itables/external/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)   450575 2023-06-11 13:29:06.000000 itables-1.5.3/itables/external/jquery.dataTables.mjs
+-rw-r--r--   0 runner    (1001) docker     (122)    89501 2023-06-11 13:29:06.000000 itables-1.5.3/itables/external/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 13:29:07.000000 itables-1.5.3/itables/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 13:29:07.000000 itables-1.5.3/itables/html/column_filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-11 13:29:03.000000 itables-1.5.3/itables/html/column_filters/initComplete.js
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-06-11 13:29:03.000000 itables-1.5.3/itables/html/column_filters/pre_dt_code.js
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-06-11 13:29:03.000000 itables-1.5.3/itables/html/datatables_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-11 13:29:03.000000 itables-1.5.3/itables/html/datatables_template_connected.html
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-06-11 13:29:03.000000 itables-1.5.3/itables/html/initialize_offline_datatable.html
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-11 13:29:03.000000 itables-1.5.3/itables/html/itables.css
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-06-11 13:29:03.000000 itables-1.5.3/itables/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15057 2023-06-11 13:29:03.000000 itables-1.5.3/itables/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-11 13:29:03.000000 itables-1.5.3/itables/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12105 2023-06-11 13:29:03.000000 itables-1.5.3/itables/sample_dfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 13:29:07.000000 itables-1.5.3/itables/samples/
+-rw-r--r--   0 runner    (1001) docker     (122)    31715 2023-06-11 13:29:03.000000 itables-1.5.3/itables/samples/countries.csv
+-rw-r--r--   0 runner    (1001) docker     (122)   420013 2023-06-11 13:29:03.000000 itables-1.5.3/itables/samples/indicators.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6390 2023-06-11 13:29:03.000000 itables-1.5.3/itables/samples/population.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-06-11 13:29:03.000000 itables-1.5.3/itables/shiny.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-11 13:29:03.000000 itables-1.5.3/itables/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-11 13:29:03.000000 itables-1.5.3/itables/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 13:29:07.000000 itables-1.5.3/itables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6978 2023-06-11 13:29:07.000000 itables-1.5.3/itables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-11 13:29:07.000000 itables-1.5.3/itables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-11 13:29:07.000000 itables-1.5.3/itables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-11 13:29:07.000000 itables-1.5.3/itables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-11 13:29:07.000000 itables-1.5.3/itables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-11 13:29:03.000000 itables-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-11 13:29:07.000000 itables-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-06-11 13:29:03.000000 itables-1.5.3/setup.py
```

### Comparing `itables-1.5.2/PKG-INFO` & `itables-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itables
-Version: 1.5.2
+Version: 1.5.3
 Summary: Interactive Tables in Jupyter
 Home-page: https://github.com/mwouts/itables
 Author: Marc Wouts
 Author-email: marc.wouts@gmail.com
 License: MIT
 Description: # Interactive Tables
```

### Comparing `itables-1.5.2/README.md` & `itables-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/datatables_format.py` & `itables-1.5.3/itables/datatables_format.py`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/downsample.py` & `itables-1.5.3/itables/downsample.py`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/external/jquery.dataTables.min.css` & `itables-1.5.3/itables/external/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/external/jquery.dataTables.mjs` & `itables-1.5.3/itables/external/jquery.dataTables.mjs`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/external/jquery.min.js` & `itables-1.5.3/itables/external/jquery.min.js`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/html/datatables_template.html` & `itables-1.5.3/itables/html/datatables_template.html`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/html/datatables_template_connected.html` & `itables-1.5.3/itables/html/datatables_template_connected.html`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/html/initialize_offline_datatable.html` & `itables-1.5.3/itables/html/initialize_offline_datatable.html`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/javascript.py` & `itables-1.5.3/itables/javascript.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,20 +122,18 @@
     # Generate table head using pandas.to_html(), see issue 63
     pattern = re.compile(r".*<thead>(.*)</thead>", flags=re.MULTILINE | re.DOTALL)
     try:
         html_header = df.head(0).to_html()
     except AttributeError:
         # Polars DataFrames
         html_header = pd.DataFrame(data=[], columns=df.columns).to_html()
-        # Don't remove the index header for empty dfs
-        if not len(df.columns):
-            show_index = True
     match = pattern.match(html_header)
     thead = match.groups()[0]
-    if not show_index:
+    # Don't remove the index header for empty dfs
+    if not show_index and len(df.columns):
         thead = thead.replace("<th></th>", "", 1)
 
     if column_filters:
         # We use this header in the column filters, so we need to remove any column multiindex first"""
         thead_flat = ""
         if show_index:
             for index in df.index.names:
@@ -234,15 +232,17 @@
     pass
 
 
 def _datatables_repr_(df=None, tableId=None, **kwargs):
     return to_html_datatable(df, tableId, connected=_CONNECTED, **kwargs)
 
 
-def to_html_datatable(df=None, caption=None, tableId=None, connected=True, **kwargs):
+def to_html_datatable(
+    df=None, caption=None, tableId=None, connected=True, import_jquery=True, **kwargs
+):
     """Return the HTML representation of the given dataframe as an interactive datatable"""
     # Default options
     for option in dir(opt):
         if (
             option not in kwargs
             and not option.startswith("__")
             and option not in ["read_package_file"]
@@ -320,14 +320,22 @@
 
     # Load the HTML template
     if connected:
         output = read_package_file("html/datatables_template_connected.html")
     else:
         output = read_package_file("html/datatables_template.html")
 
+    if not import_jquery:
+        assert (
+            connected
+        ), "In the offline mode, jQuery is imported through init_notebook_mode"
+        output = replace_value(
+            output, "    import 'https://code.jquery.com/jquery-3.6.0.min.js';\n", ""
+        )
+
     tableId = tableId or str(uuid.uuid4())
     if isinstance(classes, list):
         classes = " ".join(classes)
 
     if not showIndex:
         try:
             df = df.set_index(pd.RangeIndex(len(df.index)))
```

### Comparing `itables-1.5.2/itables/options.py` & `itables-1.5.3/itables/options.py`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/sample_dfs.py` & `itables-1.5.3/itables/sample_dfs.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,15 +100,21 @@
     return df
 
 
 def get_dict_of_test_dfs(N=100, M=100, polars=False):
     NM_values = np.reshape(np.linspace(start=0.0, stop=1.0, num=N * M), (N, M))
 
     test_dfs = {
-        "empty": pd.DataFrame(),
+        "empty": pd.DataFrame(dtype=float),
+        "no_rows": pd.DataFrame(dtype=float, columns=["a"]),
+        "no_columns": pd.DataFrame(dtype=float, index=["a"]),
+        "no_rows_one_column": pd.DataFrame([1.0], index=["a"], columns=["a"]).iloc[:0],
+        "no_columns_one_row": pd.DataFrame([1.0], index=["a"], columns=["a"]).iloc[
+            :, :0
+        ],
         "bool": pd.DataFrame(
             [[True, True, False, False], [True, False, True, False]],
             columns=list("abcd"),
         ),
         "nullable_boolean": pd.DataFrame(
             [
                 [True, True, False, None],
```

### Comparing `itables-1.5.2/itables/samples/countries.csv` & `itables-1.5.3/itables/samples/countries.csv`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/samples/indicators.csv` & `itables-1.5.3/itables/samples/indicators.csv`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables/samples/population.csv` & `itables-1.5.3/itables/samples/population.csv`

 * *Files identical despite different names*

### Comparing `itables-1.5.2/itables.egg-info/PKG-INFO` & `itables-1.5.3/itables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itables
-Version: 1.5.2
+Version: 1.5.3
 Summary: Interactive Tables in Jupyter
 Home-page: https://github.com/mwouts/itables
 Author: Marc Wouts
 Author-email: marc.wouts@gmail.com
 License: MIT
 Description: # Interactive Tables
```

### Comparing `itables-1.5.2/itables.egg-info/SOURCES.txt` & `itables-1.5.3/itables.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 itables/__init__.py
 itables/datatables_format.py
 itables/downsample.py
 itables/interactive.py
 itables/javascript.py
 itables/options.py
 itables/sample_dfs.py
+itables/shiny.py
 itables/utils.py
 itables/version.py
 itables.egg-info/PKG-INFO
 itables.egg-info/SOURCES.txt
 itables.egg-info/dependency_links.txt
 itables.egg-info/requires.txt
 itables.egg-info/top_level.txt
```

### Comparing `itables-1.5.2/setup.py` & `itables-1.5.3/setup.py`

 * *Files identical despite different names*

