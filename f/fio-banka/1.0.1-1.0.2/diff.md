# Comparing `tmp/fio_banka-1.0.1.tar.gz` & `tmp/fio_banka-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fio_banka-1.0.1.tar", last modified: Sun Jun 11 17:26:33 2023, max compression
+gzip compressed data, was "fio_banka-1.0.2.tar", last modified: Sun Jun 11 17:44:34 2023, max compression
```

## Comparing `fio_banka-1.0.1.tar` & `fio_banka-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:26:33.072378 fio_banka-1.0.1/
--rw-r--r--   0 petr      (1000) petr      (1000)     1069 2023-06-09 11:17:31.000000 fio_banka-1.0.1/LICENSE
--rw-r--r--   0 petr      (1000) petr      (1000)     5636 2023-06-11 17:26:33.072378 fio_banka-1.0.1/PKG-INFO
--rw-r--r--   0 petr      (1000) petr      (1000)     3632 2023-06-11 14:21:57.000000 fio_banka-1.0.1/README.md
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:26:33.071378 fio_banka-1.0.1/fio_banka.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     5636 2023-06-11 17:26:33.000000 fio_banka-1.0.1/fio_banka.egg-info/PKG-INFO
--rw-r--r--   0 petr      (1000) petr      (1000)      233 2023-06-11 17:26:33.000000 fio_banka-1.0.1/fio_banka.egg-info/SOURCES.txt
--rw-r--r--   0 petr      (1000) petr      (1000)        1 2023-06-11 17:26:33.000000 fio_banka-1.0.1/fio_banka.egg-info/dependency_links.txt
--rw-r--r--   0 petr      (1000) petr      (1000)      125 2023-06-11 17:26:33.000000 fio_banka-1.0.1/fio_banka.egg-info/requires.txt
--rw-r--r--   0 petr      (1000) petr      (1000)       10 2023-06-11 17:26:33.000000 fio_banka-1.0.1/fio_banka.egg-info/top_level.txt
--rw-r--r--   0 petr      (1000) petr      (1000)    11902 2023-06-09 11:30:08.000000 fio_banka-1.0.1/fio_banka.py
--rw-r--r--   0 petr      (1000) petr      (1000)     2153 2023-06-11 17:21:13.000000 fio_banka-1.0.1/pyproject.toml
--rw-r--r--   0 petr      (1000) petr      (1000)       38 2023-06-11 17:26:33.072378 fio_banka-1.0.1/setup.cfg
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:26:33.071378 fio_banka-1.0.1/tests/
--rw-r--r--   0 petr      (1000) petr      (1000)     9507 2023-06-09 11:30:08.000000 fio_banka-1.0.1/tests/test_fio_banka.py
+drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:44:34.596285 fio_banka-1.0.2/
+-rw-r--r--   0 petr      (1000) petr      (1000)     1069 2023-06-09 11:17:31.000000 fio_banka-1.0.2/LICENSE
+-rw-r--r--   0 petr      (1000) petr      (1000)     5588 2023-06-11 17:44:34.595286 fio_banka-1.0.2/PKG-INFO
+-rw-r--r--   0 petr      (1000) petr      (1000)     3584 2023-06-11 17:40:12.000000 fio_banka-1.0.2/README.md
+drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:44:34.595286 fio_banka-1.0.2/fio_banka.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     5588 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/PKG-INFO
+-rw-r--r--   0 petr      (1000) petr      (1000)      233 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/SOURCES.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)        1 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/dependency_links.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)      125 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/requires.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)       10 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/top_level.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)    11902 2023-06-09 11:30:08.000000 fio_banka-1.0.2/fio_banka.py
+-rw-r--r--   0 petr      (1000) petr      (1000)     2153 2023-06-11 17:40:12.000000 fio_banka-1.0.2/pyproject.toml
+-rw-r--r--   0 petr      (1000) petr      (1000)       38 2023-06-11 17:44:34.596285 fio_banka-1.0.2/setup.cfg
+drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:44:34.595286 fio_banka-1.0.2/tests/
+-rw-r--r--   0 petr      (1000) petr      (1000)     9507 2023-06-09 11:30:08.000000 fio_banka-1.0.2/tests/test_fio_banka.py
```

### Comparing `fio_banka-1.0.1/LICENSE` & `fio_banka-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fio_banka-1.0.1/PKG-INFO` & `fio_banka-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio_banka
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thin wrapper for Fio Banka, a.s. API
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Petr Beranek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,15 +55,15 @@
 ### Fio Banka API documentation:
 * [Specification](https://www.fio.cz/docs/cz/API_Bankovnictvi.pdf) (Czech only)
 * [XSD Schema](https://www.fio.cz/xsd/IBSchema.xsd)
 
 ## Installation
 
 ```
-python3 -m pip install git+https://github.com/peberanek/fio-banka.git
+pip install fio-banka
 ```
 
 ## Usage
 
 ```python
 >>> from datetime import date
 >>> from fio_banka import Account, TransactionsFmt
```

### Comparing `fio_banka-1.0.1/README.md` & `fio_banka-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ### Fio Banka API documentation:
 * [Specification](https://www.fio.cz/docs/cz/API_Bankovnictvi.pdf) (Czech only)
 * [XSD Schema](https://www.fio.cz/xsd/IBSchema.xsd)
 
 ## Installation
 
 ```
-python3 -m pip install git+https://github.com/peberanek/fio-banka.git
+pip install fio-banka
 ```
 
 ## Usage
 
 ```python
 >>> from datetime import date
 >>> from fio_banka import Account, TransactionsFmt
```

### Comparing `fio_banka-1.0.1/fio_banka.egg-info/PKG-INFO` & `fio_banka-1.0.2/fio_banka.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-banka
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thin wrapper for Fio Banka, a.s. API
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Petr Beranek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,15 +55,15 @@
 ### Fio Banka API documentation:
 * [Specification](https://www.fio.cz/docs/cz/API_Bankovnictvi.pdf) (Czech only)
 * [XSD Schema](https://www.fio.cz/xsd/IBSchema.xsd)
 
 ## Installation
 
 ```
-python3 -m pip install git+https://github.com/peberanek/fio-banka.git
+pip install fio-banka
 ```
 
 ## Usage
 
 ```python
 >>> from datetime import date
 >>> from fio_banka import Account, TransactionsFmt
```

### Comparing `fio_banka-1.0.1/fio_banka.py` & `fio_banka-1.0.2/fio_banka.py`

 * *Files identical despite different names*

### Comparing `fio_banka-1.0.1/pyproject.toml` & `fio_banka-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fio_banka"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name = "Petr Beranek", email = "petrberanek.mail@gmail.com" },
 ]
 description = "Thin wrapper for Fio Banka, a.s. API"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
```

### Comparing `fio_banka-1.0.1/tests/test_fio_banka.py` & `fio_banka-1.0.2/tests/test_fio_banka.py`

 * *Files identical despite different names*

