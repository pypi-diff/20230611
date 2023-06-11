# Comparing `tmp/plasmid_design-0.0.1.tar.gz` & `tmp/plasmid_design-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plasmid_design-0.0.1.tar", last modified: Mon Dec 26 06:01:42 2022, max compression
+gzip compressed data, was "plasmid_design-0.0.2.tar", last modified: Sun Jun 11 21:00:49 2023, max compression
```

## Comparing `plasmid_design-0.0.1.tar` & `plasmid_design-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dfeldman   (501) staff       (20)        0 2022-12-26 06:01:42.581584 plasmid_design-0.0.1/
--rw-r--r--   0 dfeldman   (501) staff       (20)     1056 2022-12-26 04:35:00.000000 plasmid_design-0.0.1/LICENSE.txt
--rw-r--r--   0 dfeldman   (501) staff       (20)     3228 2022-12-26 06:01:42.581231 plasmid_design-0.0.1/PKG-INFO
--rw-r--r--   0 dfeldman   (501) staff       (20)     1460 2022-12-26 05:50:26.000000 plasmid_design-0.0.1/README.md
--rw-r--r--   0 dfeldman   (501) staff       (20)      878 2022-12-26 06:01:00.000000 plasmid_design-0.0.1/pyproject.toml
--rw-r--r--   0 dfeldman   (501) staff       (20)       38 2022-12-26 06:01:42.581660 plasmid_design-0.0.1/setup.cfg
-drwxr-xr-x   0 dfeldman   (501) staff       (20)        0 2022-12-26 06:01:42.575200 plasmid_design-0.0.1/src/
-drwxr-xr-x   0 dfeldman   (501) staff       (20)        0 2022-12-26 06:01:42.578100 plasmid_design-0.0.1/src/plasmid_design/
--rw-r--r--   0 dfeldman   (501) staff       (20)        0 2022-12-26 04:51:26.000000 plasmid_design-0.0.1/src/plasmid_design/__init__.py
--rw-r--r--   0 dfeldman   (501) staff       (20)      844 2022-12-26 05:08:07.000000 plasmid_design-0.0.1/src/plasmid_design/constants.py
--rw-r--r--   0 dfeldman   (501) staff       (20)     3333 2022-12-26 04:28:50.000000 plasmid_design-0.0.1/src/plasmid_design/drive.py
--rw-r--r--   0 dfeldman   (501) staff       (20)     4285 2022-12-26 04:28:50.000000 plasmid_design-0.0.1/src/plasmid_design/idt_api.py
--rw-r--r--   0 dfeldman   (501) staff       (20)    15547 2022-12-26 05:24:36.000000 plasmid_design-0.0.1/src/plasmid_design/plasmid_design.py
--rw-r--r--   0 dfeldman   (501) staff       (20)     3057 2022-12-26 05:13:54.000000 plasmid_design-0.0.1/src/plasmid_design/sequence.py
--rw-r--r--   0 dfeldman   (501) staff       (20)     2664 2022-12-26 05:16:39.000000 plasmid_design-0.0.1/src/plasmid_design/utils.py
-drwxr-xr-x   0 dfeldman   (501) staff       (20)        0 2022-12-26 06:01:42.580835 plasmid_design-0.0.1/src/plasmid_design.egg-info/
--rw-r--r--   0 dfeldman   (501) staff       (20)     3228 2022-12-26 06:01:42.000000 plasmid_design-0.0.1/src/plasmid_design.egg-info/PKG-INFO
--rw-r--r--   0 dfeldman   (501) staff       (20)      507 2022-12-26 06:01:42.000000 plasmid_design-0.0.1/src/plasmid_design.egg-info/SOURCES.txt
--rw-r--r--   0 dfeldman   (501) staff       (20)        1 2022-12-26 06:01:42.000000 plasmid_design-0.0.1/src/plasmid_design.egg-info/dependency_links.txt
--rw-r--r--   0 dfeldman   (501) staff       (20)       70 2022-12-26 06:01:42.000000 plasmid_design-0.0.1/src/plasmid_design.egg-info/entry_points.txt
--rw-r--r--   0 dfeldman   (501) staff       (20)       69 2022-12-26 06:01:42.000000 plasmid_design-0.0.1/src/plasmid_design.egg-info/requires.txt
--rw-r--r--   0 dfeldman   (501) staff       (20)       15 2022-12-26 06:01:42.000000 plasmid_design-0.0.1/src/plasmid_design.egg-info/top_level.txt
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:00:49.226019 plasmid_design-0.0.2/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     1056 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/LICENSE.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3629 2023-06-11 21:00:49.225894 plasmid_design-0.0.2/PKG-INFO
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     1861 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/README.md
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      878 2023-06-11 20:59:02.000000 plasmid_design-0.0.2/pyproject.toml
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       38 2023-06-11 21:00:49.226054 plasmid_design-0.0.2/setup.cfg
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:00:49.223291 plasmid_design-0.0.2/src/
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:00:49.224965 plasmid_design-0.0.2/src/plasmid_design/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)        0 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/__init__.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      844 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/constants.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3333 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/drive.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     4285 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/idt_api.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)    15356 2023-06-11 20:56:39.000000 plasmid_design-0.0.2/src/plasmid_design/plasmid_design.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3057 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/sequence.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     2664 2023-06-11 20:51:05.000000 plasmid_design-0.0.2/src/plasmid_design/utils.py
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:00:49.225750 plasmid_design-0.0.2/src/plasmid_design.egg-info/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3629 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/PKG-INFO
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      507 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/SOURCES.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)        1 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/dependency_links.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       70 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/entry_points.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       69 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/requires.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       15 2023-06-11 21:00:49.000000 plasmid_design-0.0.2/src/plasmid_design.egg-info/top_level.txt
```

### Comparing `plasmid_design-0.0.1/LICENSE.txt` & `plasmid_design-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.1/PKG-INFO` & `plasmid_design-0.0.2/src/plasmid_design.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: plasmid_design
-Version: 0.0.1
+Name: plasmid-design
+Version: 0.0.2
 Summary: Automated plasmid design from speadsheet specification
 Author: David Feldman
 License: Copyright (c) 2022 David Feldman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -61,19 +61,24 @@
   restriction_enzymes: 
     table: drive_key:enzymes
     # selects just these rows
     gate: pT02_BsaI == "x"
     drive_key: 1QWFQUlIJYERJ6zY-THD9uNagD2a_He7RUfcOeF2eEKM
 ```
 
-### Configuration
+The `run` command prints estimated cost and complexity scores. the following files will be generated.
+
+## Configuration
 Tables can be sourced in different ways.
 - local csv
     - `table: /path/to/csv`
 - private google sheets
     - `table: "drive:{spreadsheet name}/{sheet name}"`
 - public google sheets
     - `table: "drive_key:{sheet_name}"`
     - `drive_key: {drive_key}`
 
 For the public option, first enable link access in google sheets, then copy `drive_key` from the URL: `https://docs.google.com/spreadsheets/d/{drive_key}/`.
 
+## Changing the vector backbone
+The DNA sequences upstream and downstream of the designed gene are identified by having "up" or "down" in the part name. To change the vector backbone, define new upstream and downstream DNA parts, then change the template column in the templates sheet accordingly.
+
```

### Comparing `plasmid_design-0.0.1/pyproject.toml` & `plasmid_design-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "plasmid_design"
-version = "0.0.1"
+version = "0.0.2"
 description = "Automated plasmid design from speadsheet specification"
 authors = [
   { name="David Feldman" },
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `plasmid_design-0.0.1/src/plasmid_design/constants.py` & `plasmid_design-0.0.2/src/plasmid_design/constants.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.1/src/plasmid_design/drive.py` & `plasmid_design-0.0.2/src/plasmid_design/drive.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.1/src/plasmid_design/idt_api.py` & `plasmid_design-0.0.2/src/plasmid_design/idt_api.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.1/src/plasmid_design/plasmid_design.py` & `plasmid_design-0.0.2/src/plasmid_design/plasmid_design.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,24 +384,14 @@
     # copies features but not annotations
     new_record = record[:]
     new_record.annotations = record.annotations
     new_record.features += arr
     return new_record
 
 
-def estimate_cost():
-    cost = 0
-    for _, seq in read_fasta(gene_order_fasta):
-        if len(seq) > 3000:
-            cost += 0.19 * len(seq)
-        else:
-            cost += 0.08 * len(seq)
-    return int(cost)
-
-
 def setup_block():
     setup()
     download_tables()
     validate_template_table()
 
 
 def reverse_translate_block(**rt_args):
@@ -415,15 +405,14 @@
     do_reverse_translations(**rt_args)
     print(f'Wrote RT outputs to {rt_output_fasta}')
     print(f'More information in reverse_translations/dna_chisel/')
 
 
 def design_block():
     generate_vectors()
-    print(f'Estimated cost (USD): {estimate_cost()}')
 
 
 def check_complexity_block():
     work = ((rt_output_fasta, rt_idt_scores), (gene_order_fasta, gene_idt_scores))
     for fasta, output_table in work:
         print(f'Retrieving IDT complexity scores for {fasta}')
         check_idt_complexity(fasta, output_table)
@@ -431,15 +420,17 @@
         print(f'Scores saved to {output_table}, worst score is {x}')
     
 
 def run():
     setup_block()
     if pd.read_csv(template_table).shape[0] == 0:
         raise SystemExit('Aborting! No templates.')
-    reverse_translate_block(seed=1)
+    rt_args = {'seed': 1}
+    rt_args.update(load_config().get('rt_args', {}))
+    reverse_translate_block(**rt_args)
     design_block()
     check_complexity_block()
     
 
 def main():
     # order is preserved
     commands = [
```

### Comparing `plasmid_design-0.0.1/src/plasmid_design/sequence.py` & `plasmid_design-0.0.2/src/plasmid_design/sequence.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.1/src/plasmid_design/utils.py` & `plasmid_design-0.0.2/src/plasmid_design/utils.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.1/src/plasmid_design.egg-info/PKG-INFO` & `plasmid_design-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: plasmid-design
-Version: 0.0.1
+Name: plasmid_design
+Version: 0.0.2
 Summary: Automated plasmid design from speadsheet specification
 Author: David Feldman
 License: Copyright (c) 2022 David Feldman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -61,19 +61,24 @@
   restriction_enzymes: 
     table: drive_key:enzymes
     # selects just these rows
     gate: pT02_BsaI == "x"
     drive_key: 1QWFQUlIJYERJ6zY-THD9uNagD2a_He7RUfcOeF2eEKM
 ```
 
-### Configuration
+The `run` command prints estimated cost and complexity scores. the following files will be generated.
+
+## Configuration
 Tables can be sourced in different ways.
 - local csv
     - `table: /path/to/csv`
 - private google sheets
     - `table: "drive:{spreadsheet name}/{sheet name}"`
 - public google sheets
     - `table: "drive_key:{sheet_name}"`
     - `drive_key: {drive_key}`
 
 For the public option, first enable link access in google sheets, then copy `drive_key` from the URL: `https://docs.google.com/spreadsheets/d/{drive_key}/`.
 
+## Changing the vector backbone
+The DNA sequences upstream and downstream of the designed gene are identified by having "up" or "down" in the part name. To change the vector backbone, define new upstream and downstream DNA parts, then change the template column in the templates sheet accordingly.
+
```

