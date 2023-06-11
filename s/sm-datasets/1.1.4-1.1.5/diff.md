# Comparing `tmp/sm_datasets-1.1.4.tar.gz` & `tmp/sm_datasets-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sm_datasets-1.1.4.tar", max compression
+gzip compressed data, was "sm_datasets-1.1.5.tar", max compression
```

## Comparing `sm_datasets-1.1.4.tar` & `sm_datasets-1.1.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       43 2023-03-29 04:49:00.699436 sm_datasets-1.1.4/README.md
--rw-r--r--   0        0        0      443 2023-03-29 04:49:00.847437 sm_datasets-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       66 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/__init__.py
--rw-r--r--   0        0        0     6589 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/datasets.py
--rw-r--r--   0        0        0     1072 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/helper.py
--rw-r--r--   0        0        0        0 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/migrations/__init__.py
--rw-r--r--   0        0        0     8418 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/migrations/biotables.py
--rw-r--r--   0        0        0    11547 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/migrations/semtab2020.py
--rw-r--r--   0        0        0     1043 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/migrations/semtab2020_r4sampled.py
--rw-r--r--   0        0        0     1151 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/models.py
--rw-r--r--   0        0        0     4013 2023-03-29 04:49:01.587440 sm_datasets-1.1.4/sm_datasets/verrsion_compare.ipynb
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 sm_datasets-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-06-11 05:30:12.681349 sm_datasets-1.1.5/README.md
+-rw-r--r--   0        0        0      427 2023-06-11 05:30:12.809350 sm_datasets-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/__init__.py
+-rw-r--r--   0        0        0     6687 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/datasets.py
+-rw-r--r--   0        0        0     1072 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/helper.py
+-rw-r--r--   0        0        0        0 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/migrations/__init__.py
+-rw-r--r--   0        0        0     8418 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/migrations/biotables.py
+-rw-r--r--   0        0        0    11547 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/migrations/semtab2020.py
+-rw-r--r--   0        0        0     1043 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/migrations/semtab2020_r4sampled.py
+-rw-r--r--   0        0        0    11324 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/migrations/semtab2022.py
+-rw-r--r--   0        0        0     1151 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/models.py
+-rw-r--r--   0        0        0     4013 2023-06-11 05:30:13.457354 sm_datasets-1.1.5/sm_datasets/verrsion_compare.ipynb
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 sm_datasets-1.1.5/PKG-INFO
```

### Comparing `sm_datasets-1.1.4/sm_datasets/datasets.py` & `sm_datasets-1.1.5/sm_datasets/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
                                 url=row["url"],
                                 entities=[EntityId(row["entity"], WIKIDATA)],
                             )
                             links.append(link)
                         table.links[ri, ci] = links
         return examples
 
+    def semtab2022_r1(self):
+        return Dataset(ROOT_DIR / "semtab2022_hardtable_r1").load()
+
     def semtab2020r4(self):
         return Dataset(ROOT_DIR / "semtab2020_round4").load()
 
     def semtab2020r4_sampled50(self):
         return Dataset(ROOT_DIR / "semtab2020_r4sampled").load()
 
     def semtab2020r4_sampled512(self):
```

### Comparing `sm_datasets-1.1.4/sm_datasets/helper.py` & `sm_datasets-1.1.5/sm_datasets/helper.py`

 * *Files identical despite different names*

### Comparing `sm_datasets-1.1.4/sm_datasets/migrations/biotables.py` & `sm_datasets-1.1.5/sm_datasets/migrations/biotables.py`

 * *Files identical despite different names*

### Comparing `sm_datasets-1.1.4/sm_datasets/migrations/semtab2020.py` & `sm_datasets-1.1.5/sm_datasets/migrations/semtab2020.py`

 * *Files identical despite different names*

### Comparing `sm_datasets-1.1.4/sm_datasets/migrations/semtab2020_r4sampled.py` & `sm_datasets-1.1.5/sm_datasets/migrations/semtab2020_r4sampled.py`

 * *Files identical despite different names*

### Comparing `sm_datasets-1.1.4/sm_datasets/models.py` & `sm_datasets-1.1.5/sm_datasets/models.py`

 * *Files identical despite different names*

### Comparing `sm_datasets-1.1.4/sm_datasets/verrsion_compare.ipynb` & `sm_datasets-1.1.5/sm_datasets/verrsion_compare.ipynb`

 * *Files identical despite different names*

### Comparing `sm_datasets-1.1.4/PKG-INFO` & `sm_datasets-1.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: sm-datasets
-Version: 1.1.4
+Version: 1.1.5
 Summary: Datasets for benchmarking Semantic Modeling problem
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kgdata (>=3.4.2,<4.0.0)
+Requires-Dist: kgdata (>=3.7.0,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
 Requires-Dist: rdflib (>=6.1.1,<7.0.0)
-Requires-Dist: rsoup (>=2.5.1,<3.0.0)
-Requires-Dist: sem-desc (>=4.4.2,<5.0.0)
+Requires-Dist: sem-desc (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 Datasets for the semantic modeling problem
```

