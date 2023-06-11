# Comparing `tmp/plasmid_design-0.0.2.tar.gz` & `tmp/plasmid_design-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plasmid_design-0.0.2.tar", last modified: Sun Jun 11 21:00:49 2023, max compression
+gzip compressed data, was "plasmid_design-0.0.3.tar", last modified: Sun Jun 11 21:29:14 2023, max compression
```

## Comparing `plasmid_design-0.0.2.tar` & `plasmid_design-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:00:49.226019 plasmid_design-0.0.2/
--rw-r--r--   0 davidfeldman   (501) staff       (20)     1056 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/LICENSE.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3629 2023-06-11 21:00:49.225894 plasmid_design-0.0.2/PKG-INFO
--rw-r--r--   0 davidfeldman   (501) staff       (20)     1861 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/README.md
--rw-r--r--   0 davidfeldman   (501) staff       (20)      878 2023-06-11 20:59:02.000000 plasmid_design-0.0.2/pyproject.toml
--rw-r--r--   0 davidfeldman   (501) staff       (20)       38 2023-06-11 21:00:49.226054 plasmid_design-0.0.2/setup.cfg
-drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:00:49.223291 plasmid_design-0.0.2/src/
-drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:00:49.224965 plasmid_design-0.0.2/src/plasmid_design/
--rw-r--r--   0 davidfeldman   (501) staff       (20)        0 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/__init__.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)      844 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/constants.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3333 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/drive.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)     4285 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/idt_api.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)    15356 2023-06-11 20:56:39.000000 plasmid_design-0.0.2/src/plasmid_design/plasmid_design.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3057 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/sequence.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)     2664 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/utils.py
-drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:00:49.225750 plasmid_design-0.0.2/src/plasmid_design.egg-info/
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3629 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/PKG-INFO
--rw-r--r--   0 davidfeldman   (501) staff       (20)      507 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/SOURCES.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)        1 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/dependency_links.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)       70 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/entry_points.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)       69 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/requires.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)       15 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/top_level.txt
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:29:14.581647 plasmid_design-0.0.3/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     1056 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/LICENSE.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3629 2023-06-11 21:29:14.581510 plasmid_design-0.0.3/PKG-INFO
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     1861 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/README.md
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      878 2023-06-11 21:28:59.000000 plasmid_design-0.0.3/pyproject.toml
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       38 2023-06-11 21:29:14.581692 plasmid_design-0.0.3/setup.cfg
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:29:14.578857 plasmid_design-0.0.3/src/
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:29:14.580234 plasmid_design-0.0.3/src/plasmid_design/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)        0 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/__init__.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      844 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/constants.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3333 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/drive.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     4285 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/idt_api.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)    15311 2023-06-11 21:25:25.000000 plasmid_design-0.0.3/src/plasmid_design/plasmid_design.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3057 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/sequence.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3076 2023-06-11 21:11:24.000000 plasmid_design-0.0.3/src/plasmid_design/utils.py
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:29:14.581290 plasmid_design-0.0.3/src/plasmid_design.egg-info/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3629 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/PKG-INFO
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      507 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/SOURCES.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)        1 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/dependency_links.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       70 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/entry_points.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       69 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/requires.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       15 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/top_level.txt
```

### Comparing `plasmid_design-0.0.2/LICENSE.txt` & `plasmid_design-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.2/PKG-INFO` & `plasmid_design-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmid_design
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automated plasmid design from speadsheet specification
 Author: David Feldman
 License: Copyright (c) 2022 David Feldman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `plasmid_design-0.0.2/README.md` & `plasmid_design-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.2/pyproject.toml` & `plasmid_design-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "plasmid_design"
-version = "0.0.2"
+version = "0.0.3"
 description = "Automated plasmid design from speadsheet specification"
 authors = [
   { name="David Feldman" },
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `plasmid_design-0.0.2/src/plasmid_design/constants.py` & `plasmid_design-0.0.3/src/plasmid_design/constants.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.2/src/plasmid_design/drive.py` & `plasmid_design-0.0.3/src/plasmid_design/drive.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.2/src/plasmid_design/idt_api.py` & `plasmid_design-0.0.3/src/plasmid_design/idt_api.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.2/src/plasmid_design/plasmid_design.py` & `plasmid_design-0.0.3/src/plasmid_design/plasmid_design.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Templated DNA and vector map generation.
 
 TODO: check that kozak (GCCACC) is always followed by ATG
 """
 from .drive import Drive
-from .utils import load_yaml_table, assert_unique, ProgressParallel
+from .utils import load_yaml_table, assert_unique, format_string_any_field
 from .sequence import read_fasta, write_fasta, translate_dna, reverse_translate_random
 from .sequence import reverse_complement as rc
 from .idt_api import score_dna_idt_parallel
 
 import fire, yaml
 import numpy as np
 import pandas as pd
@@ -24,15 +24,14 @@
 # patch biopython before importing dnachisel
 import Bio.PDB.Polypeptide
 Bio.PDB.Polypeptide.aa1 = str(Bio.PDB.Polypeptide.aa1)
 Bio.PDB.Polypeptide.aa3 = list(Bio.PDB.Polypeptide.aa3)
 
 import dnachisel as dc
 
-
 config_file = 'config.yaml'
 parts_table = 'parts.csv'
 binder_table = 'binders.csv'
 target_table = 'targets.csv'
 feature_table = 'features.csv'
 template_table = 'templates.csv'
 sites_to_avoid = 'reverse_translations/sites_to_avoid.csv'
@@ -281,20 +280,18 @@
     return problem
 
 
 def create_genbank(name, template, parts, topology='circular'):
     """Each field in the `template` string must have an entry in the `parts` dictionary.
     """    
     parts = dict(parts)
-    dna = template.format(**parts)
+    dna = format_string_any_field(template, parts)
     keys = template.replace('{', '').split('}')[:-1]
     features = {x: parts[x] for x in keys}
 
-    dna = ''.join(features.values())
-    
     i = 0
     arr = []
     for key in keys:
         n = len(parts[key])
         location = FeatureLocation(start=i, end=i+n, strand=1)
         arr += [SeqFeature(location, type='from_template',
                            qualifiers=dict(label=key))]
@@ -436,15 +433,14 @@
     commands = [
         'run',
         '0_setup',
         '1_rt',
         '2_design',
         '3_check',
         'split_order',
-        'estimate_cost',
         'validate_template_table',
         ]
 
     # if the command name is different from the function name
     named = {
         '0_setup': setup_block,
         '1_rt': reverse_translate_block,
```

### Comparing `plasmid_design-0.0.2/src/plasmid_design/sequence.py` & `plasmid_design-0.0.3/src/plasmid_design/sequence.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.2/src/plasmid_design/utils.py` & `plasmid_design-0.0.3/src/plasmid_design/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from tqdm.auto import tqdm
 import joblib
 import pandas as pd
 import yaml
+from string import Formatter
 
 
 def assert_unique(df, *cols):
     """Each argument can be a single column or a list of columns.
     """
     a = df.shape[0]
     for col in cols:
@@ -76,7 +77,19 @@
     if drop_duplicates is not None:
         df = df.drop_duplicates(drop_duplicates)
         if verbose:
             print(f'  {len(df):,} after dropping duplicates on {drop_duplicates}')
     if rename is not None:
         df = df.rename(columns=rename)
     return df
+
+
+def format_string_any_field(fmt, fields):
+    """Fill in a python format string with invalid field names 
+    (i.e., containing any character).
+    """
+    s = ''
+    for prefix, stuffing, _, _ in Formatter().parse(fmt):
+        prefix = '' if prefix is None else prefix
+        stuffing = '' if stuffing is None else fields[stuffing]
+        s += (prefix + stuffing)
+    return s
```

### Comparing `plasmid_design-0.0.2/src/plasmid_design.egg-info/PKG-INFO` & `plasmid_design-0.0.3/src/plasmid_design.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmid-design
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automated plasmid design from speadsheet specification
 Author: David Feldman
 License: Copyright (c) 2022 David Feldman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

