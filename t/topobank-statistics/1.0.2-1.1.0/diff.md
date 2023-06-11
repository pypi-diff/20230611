# Comparing `tmp/topobank-statistics-1.0.2.tar.gz` & `tmp/topobank-statistics-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topobank-statistics-1.0.2.tar", last modified: Thu Apr  6 18:13:07 2023, max compression
+gzip compressed data, was "topobank-statistics-1.1.0.tar", last modified: Sun Jun 11 21:45:16 2023, max compression
```

## Comparing `topobank-statistics-1.0.2.tar` & `topobank-statistics-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.692922 topobank-statistics-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.684922 topobank-statistics-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.688922 topobank-statistics-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-06 18:13:07.692922 topobank-statistics-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-06 18:13:07.692922 topobank-statistics-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.688922 topobank-statistics-1.0.2/topobank_statistics/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    33382 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.688922 topobank-statistics-1.0.2/topobank_statistics/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.684922 topobank-statistics-1.0.2/topobank_statistics/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.688922 topobank-statistics-1.0.2/topobank_statistics/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/static/images/ce_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.684922 topobank-statistics-1.0.2/topobank_statistics/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.688922 topobank-statistics-1.0.2/topobank_statistics/templates/topobank_statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/templates/topobank_statistics/example.html
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/templates/topobank_statistics/roughnessparameters_card_datatables.html
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/templates/topobank_statistics/roughnessparameters_card_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/templates/topobank_statistics/roughnessparameters_card_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.692922 topobank-statistics-1.0.2/topobank_statistics/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26827 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/tests/test_reentrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/tests/test_results_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-06 18:12:56.000000 topobank-statistics-1.0.2/topobank_statistics/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:13:07.688922 topobank-statistics-1.0.2/topobank_statistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-06 18:13:07.000000 topobank-statistics-1.0.2/topobank_statistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-06 18:13:07.000000 topobank-statistics-1.0.2/topobank_statistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 18:13:07.000000 topobank-statistics-1.0.2/topobank_statistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-06 18:13:07.000000 topobank-statistics-1.0.2/topobank_statistics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-06 18:13:07.000000 topobank-statistics-1.0.2/topobank_statistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 18:13:07.000000 topobank-statistics-1.0.2/topobank_statistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.215458 topobank-statistics-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.207458 topobank-statistics-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-11 21:45:16.215458 topobank-statistics-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 21:45:16.215458 topobank-statistics-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/frontend/RoughnessParametersCard.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/frontend/roughness_parameters_card.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33625 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/static/images/ce_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.215458 topobank-statistics-1.1.0/topobank_statistics/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/test_reentrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/test_results_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/top_level.txt
```

### Comparing `topobank-statistics-1.0.2/.github/workflows/publish.yml` & `topobank-statistics-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/.github/workflows/test.yml` & `topobank-statistics-1.1.0/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -45,18 +45,18 @@
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install
       run: |
         pip install --upgrade pip pip-tools
         pushd /tmp
-        git clone --branch develop https://github.com/ContactEngineering/topobank.git
+        git clone https://github.com/ContactEngineering/topobank.git
         popd
         pip-compile --extra dev pyproject.toml /tmp/topobank/pyproject.toml
         pip install -r requirements.txt
         pushd /tmp/topobank
         USE_DOCKER=no python manage.py collectstatic
         popd
         pip install -e .[dev]
 
     - name: Test
-      run: PYTHONPATH=/tmp/topobank pytest -v
+      run: PYTHONPATH=/tmp/topobank pytest -v
```

### Comparing `topobank-statistics-1.0.2/.gitignore` & `topobank-statistics-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/LICENSE` & `topobank-statistics-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/PKG-INFO` & `topobank-statistics-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topobank-statistics
-Version: 1.0.2
+Version: 1.1.0
 Summary: This is a plugin for "topobank" for statistical analysis of measurements and digital surface twins.
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 License: 
         The MIT License (MIT)
         Copyright (c) 2018-2019, Simulation Group, IMTEK, University of Freiburg, Germany
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `topobank-statistics-1.0.2/README.rst` & `topobank-statistics-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/pyproject.toml` & `topobank-statistics-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/topobank_statistics/apps.py` & `topobank-statistics-1.1.0/topobank_statistics/apps.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/topobank_statistics/downloads.py` & `topobank-statistics-1.1.0/topobank_statistics/downloads.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,65 @@
 """
 Place here all download function and register with @register_download_function
 """
 import io
 
 import pandas as pd
+import pint
 from django.http import HttpResponse
+from django.utils.text import slugify
 
 from topobank.analysis.registry import register_download_function
 from topobank.analysis.downloads import publications_urls, analyses_meta_data_dataframe, analysis_header_for_txt_file
 
-from .functions import ART_ROUGHNESS_PARAMETERS
+from .functions import VIZ_ROUGHNESS_PARAMETERS
 
 
-@register_download_function(ART_ROUGHNESS_PARAMETERS, 'results', 'txt')
+def roughness_parameters_data_frame(analyses):
+    # Unit conversion
+    ureg = pint.UnitRegistry()
+    ureg.default_format = '~P'
+
+    # Collect data
+    data = []
+    for analysis in analyses:
+        result = analysis.result
+        topography = analysis.subject
+
+        row = {
+            'Digital surface twin': topography.surface.name,
+            'Measurement': topography.name,
+            'Creator': topography.creator,
+            'Instrument name': topography.instrument_name,
+            'Instrument type': topography.instrument_type,
+            'Instrument parameters': topography.instrument_parameters
+        }
+        for quantity in result:
+            v = ureg.Quantity(quantity['value'], 'dimensionless' if quantity['unit'] == 1 else quantity['unit'])
+            v_si = v.to_base_units()  # Convert to SI units
+
+            quantity_header = quantity['quantity']
+            if quantity['from']:
+                quantity_header += ', ' +  quantity['from']
+            if quantity['direction']:
+                quantity_header += ', ' +  quantity['direction']
+            if quantity['symbol']:
+                quantity_header = quantity['symbol'].replace(r'&Delta;', 'Δ') + ' [' + quantity_header + ']'
+            quantity_header += f' ({v_si.units})'
+
+            row |= {quantity_header: v_si.magnitude}
+        data += [row]
+
+    # Return data frame
+    df = pd.DataFrame(data)
+
+    return df
+
+
+@register_download_function(VIZ_ROUGHNESS_PARAMETERS, 'results', 'csv')
 def download_roughness_parameters_to_txt(request, analyses):
     """Download roughness parameters from given analyses as CSV file.
 
        Tables with roughness parameters only make sense for analyses
        where subject is a topography (so far). All other analyses
        (e.g. for surfaces) will be ignored here.
 
@@ -55,43 +98,30 @@
                 f.write('# For these analyses, published data was used. Please visit these URLs for details:\n')
                 for pub_url in publication_urls:
                     f.write(f'# - {pub_url}\n')
                 f.write('#\n')
 
         f.write(analysis_header_for_txt_file(analysis))
 
-        result = analysis.result
-        topography = analysis.subject
-        for row in result:
-            data.append([topography.surface.name,
-                         topography.name,
-                         row['quantity'],
-                         row['direction'] if row['direction'] else '',
-                         row['from'] if row['from'] else '',
-                         row['symbol'] if row['symbol'] else '',
-                         row['value'],
-                         row['unit']])
-
     f.write('# Table of roughness parameters\n')
-    df = pd.DataFrame(data, columns=['digital surface twin', 'measurement', 'quantity', 'direction',
-                                     'from', 'symbol', 'value', 'unit'])
-    df.to_csv(f, index=False)
+    df = roughness_parameters_data_frame(analyses)
+    df.to_csv(f, sep=';', index=False)
     f.write('\n')
 
     # Prepare response object.
     response = HttpResponse(f.getvalue(), content_type='application/text')
-    filename = '{}.txt'.format(analysis.function.name.replace(' ', '_'))
+    filename = '{}.csv'.format(analysis.function.name.replace(' ', '_'))
     response['Content-Disposition'] = f'attachment; filename="{filename}"'
 
     # Close file and return response.
     f.close()
     return response
 
 
-@register_download_function(ART_ROUGHNESS_PARAMETERS, 'results', 'xlsx')
+@register_download_function(VIZ_ROUGHNESS_PARAMETERS, 'results', 'xlsx')
 def download_roughness_parameters_to_xlsx(request, analyses):
     """Download roughness parameters from given analyses as XLSX file.
 
        Tables with roughness parameters only make sense for analyses
        where subject is a topography (so far). All other analyses
        (e.g. for surfaces) will be ignored here.
 
@@ -107,33 +137,23 @@
         HTTPResponse
     """
     analyses = [a for a in analyses if a.is_topography_related]
 
     f = io.BytesIO()
     excel = pd.ExcelWriter(f)
 
-    data = []
-    for analysis in analyses:
-        topo = analysis.subject
-        for row in analysis.result:
-            row['digital surface twin'] = topo.surface.name
-            row['measurement'] = topo.name
-            data.append(row)
-
-    roughness_df = pd.DataFrame(data, columns=['digital surface twin', 'measurement', 'quantity', 'direction',
-                                               'from', 'symbol', 'value', 'unit'])
-    roughness_df.replace(r'&Delta;', 'Δ', inplace=True, regex=True)  # we want a real greek delta
+    roughness_df = roughness_parameters_data_frame(analyses)
     roughness_df.to_excel(excel, sheet_name="Roughness parameters", index=False)
     info_df = analyses_meta_data_dataframe(analyses, request)
     info_df.to_excel(excel, sheet_name='INFORMATION', index=False)
     excel.close()
 
     # Prepare response object.
     response = HttpResponse(f.getvalue(),
                             content_type='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
-    filename = '{}.xlsx'.format(analysis.function.name.replace(' ', '_'))
+    filename = f'{slugify(analyses[0].function.name)}.xlsx'
     response['Content-Disposition'] = f'attachment; filename="{filename}"'
 
     # Close file and return response.
     f.close()
     return response
```

### Comparing `topobank-statistics-1.0.2/topobank_statistics/functions.py` & `topobank-statistics-1.1.0/topobank_statistics/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 from SurfaceTopography.Container.Averaging import log_average
 from SurfaceTopography.Container.ScaleDependentStatistics import scale_dependent_statistical_property
 from SurfaceTopography.Container.common import suggest_length_unit
 from SurfaceTopography.Exceptions import CannotPerformAnalysisError, ReentrantDataError
 
 from topobank.analysis.functions import reasonable_bins_argument, wrap_series, \
-    make_alert_entry, ContainerProxy, ART_SERIES
+    make_alert_entry, ContainerProxy, VIZ_SERIES
 from topobank.analysis.registry import register_implementation
 
-
-ART_ROUGHNESS_PARAMETERS = "roughness parameters"
+APP_NAME = "topobank_statistics"
+VIZ_ROUGHNESS_PARAMETERS = "roughness-parameters"
 
 GAUSSIAN_FIT_SERIES_NAME = 'Gaussian fit'
 
 
-@register_implementation(art=ART_SERIES, name="Height distribution")
+@register_implementation("analysis", VIZ_SERIES, "Height distribution")
 def height_distribution(topography, bins=None, wfac=5, progress_recorder=None, storage_prefix=None):
     # Get low level topography from SurfaceTopography model
     topography = topography.topography()
 
     if bins is None:
         bins = reasonable_bins_argument(topography)
 
@@ -148,15 +148,15 @@
                  x=x_gauss,
                  y=y_gauss)
         )
 
     return scalars, series
 
 
-@register_implementation(art=ART_SERIES, name="Slope distribution")
+@register_implementation("analysis", VIZ_SERIES, "Slope distribution")
 def slope_distribution(topography, bins=None, wfac=5, progress_recorder=None, storage_prefix=None):
     """Calculates slope distribution for given topography."""
     # Get low level topography from SurfaceTopography model
     topography = topography.topography()
 
     if bins is None:
         bins = reasonable_bins_argument(topography)
@@ -222,15 +222,15 @@
         xunit='1',
         yunit='1',
         scalars=scalars,
         series=wrap_series(series)
     )
 
 
-@register_implementation(art=ART_SERIES, name="Curvature distribution")
+@register_implementation("analysis", VIZ_SERIES, "Curvature distribution")
 def curvature_distribution(topography, bins=None, wfac=5, progress_recorder=None, storage_prefix=None):
     # Get low level topography from SurfaceTopography model
     topography = topography.topography()
 
     if bins is None:
         bins = reasonable_bins_argument(topography)
 
@@ -290,15 +290,15 @@
         ylabel='Probability density',
         xunit=inverse_unit,
         yunit=unit,
         series=wrap_series(series)
     )
 
 
-@register_implementation(art=ART_SERIES, name="Power spectrum")
+@register_implementation("analysis", VIZ_SERIES, "Power spectrum")
 def power_spectrum(topography, progress_recorder=None, storage_prefix=None, window=None,
                    nb_points_per_decade=10):
     """Calculate Power Spectrum for given topography."""
     # Get low level topography from SurfaceTopography model
     return _analysis_function(topography,
                              'power_spectrum_from_profile',
                              'power_spectrum_from_area',
@@ -313,15 +313,15 @@
                               conv_2d_fac=1 / np.pi,
                               conv_2d_exponent=1,
                               window=window,
                               nb_points_per_decade=nb_points_per_decade,
                               storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_SERIES, name="Power spectrum")
+@register_implementation("analysis", VIZ_SERIES, "Power spectrum")
 def power_spectrum_for_surface(surface, progress_recorder=None, storage_prefix=None, window=None,
                                nb_points_per_decade=10):
     """Calculate Power Spectrum for given topography."""
     # Get low level topography from SurfaceTopography model
 
     return _analysis_function_for_surface(surface,
                                           progress_recorder,
@@ -333,15 +333,15 @@
                                          '{}⁻¹',
                                          '{}³',
                                           window=window,
                                           nb_points_per_decade=nb_points_per_decade,
                                           storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_SERIES, name="Autocorrelation")
+@register_implementation("analysis", VIZ_SERIES, "Autocorrelation")
 def autocorrelation(topography, progress_recorder=None, storage_prefix=None, nb_points_per_decade=10):
     return _analysis_function(topography,
                              'autocorrelation_from_profile',
                              'autocorrelation_from_area',
                              'Height-difference autocorrelation function (ACF)',
                              'Distance',
                              'ACF',
@@ -350,30 +350,30 @@
                              'Radial average',
                              '{}',
                              '{}²',
                               nb_points_per_decade=nb_points_per_decade,
                               storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_SERIES, name="Autocorrelation")
+@register_implementation("analysis", VIZ_SERIES, "Autocorrelation")
 def autocorrelation_for_surface(surface, progress_recorder=None, storage_prefix=None, nb_points_per_decade=10):
     return _analysis_function_for_surface(surface,
                                           progress_recorder,
                                          'autocorrelation_from_profile',
                                          'Height-difference autocorrelation function (ACF)',
                                          'Distance',
                                          'ACF',
                                          'Along x',
                                          '{}',
                                          '{}²',
                                           nb_points_per_decade=nb_points_per_decade,
                                           storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_SERIES, name="Variable bandwidth")
+@register_implementation("analysis", VIZ_SERIES, "Variable bandwidth")
 def variable_bandwidth(topography, progress_recorder=None, storage_prefix=None):
     return _analysis_function(topography,
                              'variable_bandwidth_from_profile',
                              'variable_bandwidth_from_area',
                              'Variable-bandwidth analysis',
                              'Bandwidth',
                              'RMS height',
@@ -381,16 +381,19 @@
                              'Profile decomposition along y',
                              'Areal decomposition',
                              '{}',
                              '{}',
                               storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_SERIES, name="Variable bandwidth")
-def variable_bandwidth_for_surface(surface, progress_recorder=None, storage_prefix=None, nb_points_per_decade=10):
+@register_implementation("analysis", VIZ_SERIES, "Variable bandwidth")
+def variable_bandwidth_for_surface(surface, progress_recorder=None, storage_prefix=None):
+    # Resampling not possible for topographies, but all function for same name must have identical signatures. We hence
+    # simply fix `nb_points_per_decade` here.
+    nb_points_per_decade = 10
     return _analysis_function_for_surface(surface,
                                           progress_recorder,
                                          'variable_bandwidth_from_profile',
                                          'Variable-bandwidth analysis',
                                          'Bandwidth',
                                          'RMS height',
                                          'Profile decomposition along x',
@@ -515,15 +518,15 @@
         yunit=yunit.format(unit),
         xscale='log',
         yscale='log',
         series=wrap_series(series),
         alerts=alerts)
 
 
-@register_implementation(art=ART_SERIES, name="Scale-dependent slope")
+@register_implementation("analysis", VIZ_SERIES, "Scale-dependent slope")
 def scale_dependent_slope(topography, progress_recorder=None, storage_prefix=None, nb_points_per_decade=10):
     return scale_dependent_roughness_parameter(
         topography,
         progress_recorder,
         1,
         'Scale-dependent slope',
         'Slope',
@@ -532,29 +535,29 @@
         lambda x, y: x * x + y * y,
         'Gradient',
         '1',
         nb_points_per_decade=nb_points_per_decade,
         storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_SERIES, name="Scale-dependent slope")
+@register_implementation("analysis", VIZ_SERIES, "Scale-dependent slope")
 def scale_dependent_slope_for_surface(surface, progress_recorder=None, storage_prefix=None, nb_points_per_decade=10):
     return scale_dependent_roughness_parameter_for_surface(
         surface,
         progress_recorder,
         1,
         'Scale-dependent slope',
         'Slope',
         'Slope in x-direction',
         '1',
         nb_points_per_decade=nb_points_per_decade,
         storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_SERIES, name="Scale-dependent curvature")
+@register_implementation("analysis", VIZ_SERIES, "Scale-dependent curvature")
 def scale_dependent_curvature(topography, progress_recorder=None, storage_prefix=None, nb_points_per_decade=10):
     return scale_dependent_roughness_parameter(
         topography,
         progress_recorder,
         2,
         'Scale-dependent curvature',
         'Curvature',
@@ -563,30 +566,30 @@
         lambda x, y: (x + y) ** 2 / 4,
         '1/2 Laplacian',
         '{}⁻¹',
         nb_points_per_decade=nb_points_per_decade,
         storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_SERIES, name="Scale-dependent curvature")
+@register_implementation("analysis", VIZ_SERIES, "Scale-dependent curvature")
 def scale_dependent_curvature_for_surface(surface, progress_recorder=None, storage_prefix=None,
                                           nb_points_per_decade=10):
     return scale_dependent_roughness_parameter_for_surface(
         surface,
         progress_recorder,
         2,
         'Scale-dependent curvature',
         'Curvature',
         'Curvature in x-direction',
         '{}⁻¹',
         nb_points_per_decade=nb_points_per_decade,
         storage_prefix=storage_prefix)
 
 
-@register_implementation(art=ART_ROUGHNESS_PARAMETERS, name="Roughness parameters")
+@register_implementation(APP_NAME, VIZ_ROUGHNESS_PARAMETERS, "Roughness parameters")
 def roughness_parameters(topography, progress_recorder=None, storage_prefix=None):
     """Calculate roughness parameters for given topography.
 
     Parameters
     ----------
     topography: topobank.manager.models.Topography
     progress_recorder: celery_progress.backend.ProgressRecorder or None
```

### Comparing `topobank-statistics-1.0.2/topobank_statistics/static/images/ce_logo.svg` & `topobank-statistics-1.1.0/topobank_statistics/static/images/ce_logo.svg`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/topobank_statistics/tests/test_functions.py` & `topobank-statistics-1.1.0/topobank_statistics/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numpy as np
 import math
+
+import pint
 import pytest
 from dataclasses import dataclass
 from numpy.testing import assert_allclose
 
 from SurfaceTopography import Topography, NonuniformLineScan
 
 from topobank.analysis.models import AnalysisFunction
-from topobank.analysis.functions import IncompatibleTopographyException
 from topobank_statistics.functions import height_distribution, slope_distribution, curvature_distribution, \
     power_spectrum, power_spectrum_for_surface, autocorrelation, autocorrelation_for_surface, variable_bandwidth, \
     variable_bandwidth_for_surface, scale_dependent_slope, scale_dependent_slope_for_surface, roughness_parameters
 
 EXPECTED_KEYS_FOR_DIST_ANALYSIS = sorted(['name', 'scalars', 'xlabel', 'ylabel', 'xunit', 'yunit', 'series'])
 EXPECTED_KEYS_FOR_PLOT_CARD_ANALYSIS = sorted(['alerts', 'name',
                                                'xlabel', 'ylabel', 'xunit', 'yunit',
@@ -444,14 +445,17 @@
 
 def test_roughness_parameters(simple_linear_2d_topography):
     unit = simple_linear_2d_topography.unit
     inverse_unit = '{}⁻¹'.format(unit)
     topography = FakeTopographyModel(simple_linear_2d_topography)
     result = roughness_parameters(topography)
 
+    ureg = pint.UnitRegistry()
+    ureg.default_format = '~P'
+
     expected = [
         {
             'quantity': 'RMS height',
             'direction': 'x',
             'from': 'profile (1D)',
             'symbol': 'Rq',
             'value': 0,
@@ -475,71 +479,71 @@
         },
         {
             'quantity': 'RMS curvature',
             'direction': 'y',
             'from': 'profile (1D)',
             'symbol': '',
             'value': 0,
-            'unit': inverse_unit,
+            'unit': inverse_unit
         },
         {
             'quantity': 'RMS curvature',
             'direction': None,
             'from': 'area (2D)',
             'symbol': '',
             'value': 0,
-            'unit': inverse_unit,
+            'unit': inverse_unit
         },
         {
             'quantity': 'RMS curvature',
             'direction': 'x',
             'from': 'profile (1D)',
             'symbol': '',
             'value': 0,
-            'unit': inverse_unit,
+            'unit': inverse_unit
         },
         {
             'quantity': 'RMS slope',
             'direction': 'x',
             'from': 'profile (1D)',
             'symbol': 'R&Delta;q',
             'value': 0,
-            'unit': 1,
+            'unit': 1
         },
         {
             'quantity': 'RMS slope',
             'direction': 'y',
             'from': 'profile (1D)',
             'symbol': 'R&Delta;q',
             'value': 2,
-            'unit': 1,
+            'unit': 1
         },
         {
             'quantity': 'RMS gradient',
             'direction': None,
             'from': 'area (2D)',
             'symbol': '',
             'value': 2,
-            'unit': 1,
+            'unit': 1
         },
         {
             'quantity': 'Bandwidth: lower bound',
             'direction': None,
             'from': 'area (2D)',
             'symbol': '',
             'value': 1.0,
-            'unit': unit,
+            'unit': unit
         },
         {
             'quantity': 'Bandwidth: upper bound',
             'direction': None,
             'from': 'area (2D)',
             'symbol': '',
             'value': 7.5,
-            'unit': unit,
+            'unit': unit
         },
     ]
 
     # Look whether all fields are included
     assert len(result) == len(expected)
 
     # compare all fields in detail
@@ -667,34 +671,36 @@
     assert_allclose(expected_result['series'][0]['x'], result['series'][0]['x'], rtol=1e-6)
     assert_allclose(expected_result['series'][0]['y'], result['series'][0]['y'], rtol=1e-6)
 
 
 def test_variable_bandwidth_for_surface(simple_surface):
     """Testing variable bandwidth for an artificial surface."""
 
-    result = variable_bandwidth_for_surface(simple_surface, nb_points_per_decade=3)
+    result = variable_bandwidth_for_surface(simple_surface)
 
     expected_result = {
         'name': 'Variable-bandwidth analysis',
         'xlabel': 'Bandwidth',
         'ylabel': 'RMS height',
         'xunit': 'nm',
         'yunit': 'nm',
         'xscale': 'log',
         'yscale': 'log',
         'series': [
             {
                 'name': 'Profile decomposition along x',
                 # This is a pure regression test
-                'x': [3.892199e-01, 7.784397e-01, 1.556879, 3.113759,
-                      6.227518, 1.342703e+01, 2.808543e+01, 6.861511e+01,
-                      1.250000e+02, 2.500000e+02, 7.500000e+02],
+                'x': [3.892199e-01, 7.784397e-01, 1.556879e+00, 3.113759e+00,
+                      6.227518e+00, 1.171622e+01, 2.348236e+01, 4.706498e+01,
+                      5.991179e+01, 9.433142e+01, 1.250000e+02, 2.500000e+02,
+                      5.000000e+02, 1.000000e+03],
                 'y': [9.832030e-03, 3.501679e-02, 1.304232e-01, 4.237846e-01,
-                      6.662862e-01, 6.774048e-01, 6.856179e-01, 3.342818e+02,
-                      7.008752e+02, 7.070114e+02, 7.083317e+02],
+                      6.662862e-01, 6.774048e-01, 6.856179e-01, 6.874945e-01,
+                      6.678760e+02, 6.875201e-01, 7.008752e+02, 7.070114e+02,
+                      7.081023e+02, 7.085611e+02],
             }
         ]
     }
 
     for k in ['name', 'xunit', 'yunit', 'xlabel', 'ylabel', 'xscale', 'yscale']:
         assert expected_result[k] == result[k]
```

### Comparing `topobank-statistics-1.0.2/topobank_statistics/tests/test_reentrant.py` & `topobank-statistics-1.1.0/topobank_statistics/tests/test_reentrant.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/topobank_statistics/tests/test_results_view.py` & `topobank-statistics-1.1.0/topobank_statistics/tests/test_results_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import pytest
 
-from django.shortcuts import reverse
-
 import tempfile
 import numpy as np
 import openpyxl
 
-from topobank.manager.utils import subjects_to_json
+from topobank.manager.utils import subjects_to_base64
 from topobank.manager.tests.utils import two_topos
 from topobank.analysis.models import AnalysisFunction
 from topobank.analysis.tests.utils import TopographyAnalysisFactory, Topography2DFactory, SurfaceFactory
-from topobank.analysis.registry import AnalysisRegistry
-from topobank.organizations.tests.utils import OrganizationFactory
 
-from ..views import RoughnessParametersCardView, NUM_SIGNIFICANT_DIGITS_RMS_VALUES
+from ..functions import APP_NAME, VIZ_ROUGHNESS_PARAMETERS
+from ..views import roughness_parameters_card_view, NUM_SIGNIFICANT_DIGITS_RMS_VALUES
 
 
 @pytest.mark.parametrize('file_format', ['txt', 'xlsx'])
 @pytest.mark.django_db
 def test_roughness_params_download_as_txt(client, two_topos, file_format, handle_usage_statistics, rf):
     # This is only a simple test which checks whether the file can be downloaded
     t1, t2 = two_topos
 
     func = AnalysisFunction.objects.get(name='Roughness parameters')
 
-    import pickle
-    pickled_kwargs = pickle.dumps({})
+    kwargs = {}
 
-    ana1 = TopographyAnalysisFactory.create(subject=t1, function=func, kwargs=pickled_kwargs)
-    ana2 = TopographyAnalysisFactory.create(subject=t1, function=func, kwargs=pickled_kwargs)
+    ana1 = TopographyAnalysisFactory.create(subject=t1, function=func, kwargs=kwargs)
+    ana2 = TopographyAnalysisFactory.create(subject=t1, function=func, kwargs=kwargs)
 
     username = 'testuser'
     password = 'abcd$1234'
 
     assert client.login(username=username, password=password)
 
     # ids_downloadable_analyses = [ana1.id, ana2.id]
@@ -73,25 +69,24 @@
 
         assert len(xlsx.worksheets) == 2
 
         ws = xlsx.get_sheet_by_name("Roughness parameters")
 
         all_values_list = list(np.array(list(ws.values)).flatten())
 
-        assert 'RMS height' in all_values_list
-        assert 'RMS slope' in all_values_list
-        assert 'RMS curvature' in all_values_list
+        assert 'Rq [RMS height, profile (1D), x] (m)' in all_values_list
+        assert 'RMS curvature, profile (1D), y (1/m)' in all_values_list
 
         xlsx.get_sheet_by_name("INFORMATION")
 
 
 @pytest.mark.urls('topobank_statistics.tests.urls')
 @pytest.mark.parametrize('template_flavor', ['list', 'detail'])
 @pytest.mark.django_db
-def test_roughness_params_rounded(rf, mocker, template_flavor, user_with_plugin):
+def test_roughness_params_rounded(api_rf, mocker, template_flavor, user_with_plugin, handle_usage_statistics):
 
     def myfunc(topography, *args, **kwargs):
         """Return some fake values for testing rounding"""
         return [
             {
                 'quantity': 'RMS Height',
                 'direction': None,
@@ -130,41 +125,31 @@
                 'from': 'profile (1D)',
                 'symbol': 'S&Delta;q',
                 'value': np.float32('nan'),
                 'unit': 1,
             }
         ]
 
-    m = mocker.patch('topobank.analysis.registry.AnalysisFunctionImplementation.python_function')
+    m = mocker.patch('topobank.analysis.registry.AnalysisFunctionImplementation.python_function',
+                     new_callable=mocker.PropertyMock)
     m.return_value = myfunc
 
     surf = SurfaceFactory(creator=user_with_plugin)
     topo = Topography2DFactory(size_x=1, size_y=1, surface=surf)
 
     func = AnalysisFunction.objects.get(name='Roughness parameters')
     TopographyAnalysisFactory(subject=topo, function=func)
 
-    request = rf.post(reverse('analysis:card'), data={
-        'function_id': func.id,
-        'card_id': 'card',
-        'template_flavor': template_flavor,
-        'subjects_ids_json': subjects_to_json([topo]),
-    }, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+    request = api_rf.get(f'/plugins/topobank_statistics/card/roughness-parameters/{func.id}',
+                         {'function_id': func.id, 'subjects': subjects_to_base64([topo])})
     request.user = topo.surface.creator
     request.session = {}
 
-    reg = AnalysisRegistry()
-    card_view_class = reg.get_card_view_class(reg.get_analysis_result_type_for_function_name(func.name))
-
-    assert card_view_class == RoughnessParametersCardView
-
-    card_view = card_view_class.as_view()
-    response = card_view(request)
+    response = roughness_parameters_card_view(request)
     assert response.status_code == 200
-    assert response.template_name == [f'topobank_statistics/roughnessparameters_card_{template_flavor}.html']
 
     # we want rounding to 5 digits
     assert NUM_SIGNIFICANT_DIGITS_RMS_VALUES == 5
 
     topo_url = topo.get_absolute_url()
 
     exp_table_data = [
@@ -216,15 +201,15 @@
             'value': None,
             'unit': 1,
             'topography_name': topo.name,
             'topography_url': topo_url
         }
     ]
 
-    assert response.context_data['table_data'] == exp_table_data
+    assert response.data['tableData'] == exp_table_data
 
     #
     # We do not render response here, because this causes problems
     # when resolving static files from topobank package
     #
     # response.render()
     # assert b"1.2346" in response.content
```

### Comparing `topobank-statistics-1.0.2/topobank_statistics/tests/urls.py` & `topobank-statistics-1.1.0/topobank_statistics/tests/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 """
 from django.urls import include, path
 from django.conf import settings
 from django.conf.urls.static import static
 
 from topobank.views import HomeView
 
-urlpatterns = [
-    path("", HomeView.as_view(), name="home"),
-    path(
-        "manager/",
-        include("topobank.manager.urls", namespace="manager"),
-    ),
-    path(
-        "analysis/",
-        include("topobank.analysis.urls", namespace="analysis"),
-    ),
-] + static(
+urlpatterns = [path("", HomeView.as_view(), name="home"),
+               path(
+                   "manager/",
+                   include("topobank.manager.urls", namespace="manager"),
+               ),
+               path(
+                   "users/",
+                   include("topobank.users.urls", namespace="users"),
+               ),
+               path(
+                   "analysis/",
+                   include("topobank.analysis.urls", namespace="analysis"),
+               ),
+               ] + static(
     settings.MEDIA_URL, document_root=settings.MEDIA_ROOT
 )
```

### Comparing `topobank-statistics-1.0.2/topobank_statistics/tests.py` & `topobank-statistics-1.1.0/topobank_statistics/tests.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.0.2/topobank_statistics.egg-info/PKG-INFO` & `topobank-statistics-1.1.0/topobank_statistics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topobank-statistics
-Version: 1.0.2
+Version: 1.1.0
 Summary: This is a plugin for "topobank" for statistical analysis of measurements and digital surface twins.
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 License: 
         The MIT License (MIT)
         Copyright (c) 2018-2019, Simulation Group, IMTEK, University of Freiburg, Germany
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `topobank-statistics-1.0.2/topobank_statistics.egg-info/SOURCES.txt` & `topobank-statistics-1.1.0/topobank_statistics.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,18 +21,16 @@
 topobank_statistics/views.py
 topobank_statistics.egg-info/PKG-INFO
 topobank_statistics.egg-info/SOURCES.txt
 topobank_statistics.egg-info/dependency_links.txt
 topobank_statistics.egg-info/entry_points.txt
 topobank_statistics.egg-info/requires.txt
 topobank_statistics.egg-info/top_level.txt
+topobank_statistics/frontend/RoughnessParametersCard.vue
+topobank_statistics/frontend/roughness_parameters_card.js
 topobank_statistics/migrations/__init__.py
 topobank_statistics/static/images/ce_logo.svg
-topobank_statistics/templates/topobank_statistics/example.html
-topobank_statistics/templates/topobank_statistics/roughnessparameters_card_datatables.html
-topobank_statistics/templates/topobank_statistics/roughnessparameters_card_detail.html
-topobank_statistics/templates/topobank_statistics/roughnessparameters_card_list.html
 topobank_statistics/tests/__init__.py
 topobank_statistics/tests/test_functions.py
 topobank_statistics/tests/test_reentrant.py
 topobank_statistics/tests/test_results_view.py
 topobank_statistics/tests/urls.py
```

