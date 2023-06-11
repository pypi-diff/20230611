# Comparing `tmp/hardy_weinberg_equilibrium-0.1.1.post20230611.tar.gz` & `tmp/hardy_weinberg_equilibrium-0.1.2.post20230611.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardy_weinberg_equilibrium-0.1.1.post20230611.tar", last modified: Sun Jun 11 04:22:28 2023, max compression
+gzip compressed data, was "hardy_weinberg_equilibrium-0.1.2.post20230611.tar", last modified: Sun Jun 11 04:35:17 2023, max compression
```

## Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611.tar` & `hardy_weinberg_equilibrium-0.1.2.post20230611.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.429068 hardy_weinberg_equilibrium-0.1.1.post20230611/
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.427603 hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/
--rw-r--r--   0 delliusalexander   (501) staff       (20)    42061 2023-06-11 04:22:28.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/PKG-INFO
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1483 2023-06-11 04:22:28.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/SOURCES.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)        1 2023-06-11 04:22:28.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/dependency_links.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)       34 2023-06-11 04:22:28.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/entry_points.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)        1 2023-06-10 04:00:15.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/not-zip-safe
--rw-r--r--   0 delliusalexander   (501) staff       (20)      126 2023-06-11 04:22:28.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/requires.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)       10 2023-06-11 04:22:28.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/top_level.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)    35148 2023-06-10 04:05:55.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/LICENSE
--rw-r--r--   0 delliusalexander   (501) staff       (20)    42061 2023-06-11 04:22:28.429493 hardy_weinberg_equilibrium-0.1.1.post20230611/PKG-INFO
--rw-r--r--   0 delliusalexander   (501) staff       (20)      196 2023-06-10 04:18:24.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/README.md
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1949 2023-06-10 05:34:58.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/pyproject.toml
--rw-r--r--   0 delliusalexander   (501) staff       (20)       74 2023-06-11 04:22:28.430097 hardy_weinberg_equilibrium-0.1.1.post20230611/setup.cfg
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1888 2023-06-10 05:13:10.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/setup.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.414765 hardy_weinberg_equilibrium-0.1.1.post20230611/src/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-05 21:19:33.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)      526 2023-06-09 22:58:48.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/config.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.416541 hardy_weinberg_equilibrium-0.1.1.post20230611/src/genetics/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-10 17:11:37.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/genetics/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1223 2023-06-10 17:06:10.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/genetics/allele.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     2746 2023-06-10 19:57:44.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/genetics/gene.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.418245 hardy_weinberg_equilibrium-0.1.1.post20230611/src/hardy_weinberg/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-10 17:11:37.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/hardy_weinberg/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1736 2023-06-10 19:59:59.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/hardy_weinberg/hardy_weinberg.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     8996 2023-06-11 03:03:11.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/hardy_weinberg/hardy_weinberg_stats.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     4343 2023-06-11 03:28:06.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/main.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.419168 hardy_weinberg_equilibrium-0.1.1.post20230611/src/routers/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:15:08.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/routers/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     7559 2023-06-10 17:06:10.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/routers/root.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.419596 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:23:34.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/__init__.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.420905 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/generators/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:35:33.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/generators/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)      372 2023-06-10 19:56:40.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/generators/char_generator.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     3155 2023-06-11 03:14:33.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/generators/population_generator.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.421812 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/parsers/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:39:13.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/parsers/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     2773 2023-06-11 03:50:06.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/parsers/args_parser.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:22:28.424567 hardy_weinberg_equilibrium-0.1.1.post20230611/tests/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:01:33.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/tests/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)      637 2023-06-11 02:54:11.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/tests/test_asyncio.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)      350 2023-06-10 17:11:37.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/tests/test_hardy_dist.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)      940 2023-06-11 03:06:03.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/tests/test_hardy_weinberg.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1034 2023-06-11 03:25:22.000000 hardy_weinberg_equilibrium-0.1.1.post20230611/tests/test_threading.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.864538 hardy_weinberg_equilibrium-0.1.2.post20230611/
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.862939 hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)    43922 2023-06-11 04:35:17.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/PKG-INFO
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1483 2023-06-11 04:35:17.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/SOURCES.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        1 2023-06-11 04:35:17.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/dependency_links.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)       34 2023-06-11 04:35:17.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/entry_points.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        1 2023-06-10 04:00:15.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/not-zip-safe
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      126 2023-06-11 04:35:17.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/requires.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)       10 2023-06-11 04:35:17.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/top_level.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)    35148 2023-06-10 04:05:55.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/LICENSE
+-rw-r--r--   0 delliusalexander   (501) staff       (20)    43922 2023-06-11 04:35:17.865065 hardy_weinberg_equilibrium-0.1.2.post20230611/PKG-INFO
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     2057 2023-06-11 04:31:17.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/README.md
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1949 2023-06-11 04:35:05.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/pyproject.toml
+-rw-r--r--   0 delliusalexander   (501) staff       (20)       74 2023-06-11 04:35:17.865815 hardy_weinberg_equilibrium-0.1.2.post20230611/setup.cfg
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1888 2023-06-11 04:35:05.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/setup.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.851151 hardy_weinberg_equilibrium-0.1.2.post20230611/src/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-05 21:19:33.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      526 2023-06-09 22:58:48.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/config.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.852299 hardy_weinberg_equilibrium-0.1.2.post20230611/src/genetics/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-10 17:11:37.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/genetics/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1223 2023-06-10 17:06:10.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/genetics/allele.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     2746 2023-06-10 19:57:44.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/genetics/gene.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.853581 hardy_weinberg_equilibrium-0.1.2.post20230611/src/hardy_weinberg/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-10 17:11:37.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/hardy_weinberg/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1736 2023-06-10 19:59:59.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/hardy_weinberg/hardy_weinberg.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     8996 2023-06-11 03:03:11.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/hardy_weinberg/hardy_weinberg_stats.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     4343 2023-06-11 03:28:06.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/main.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.854548 hardy_weinberg_equilibrium-0.1.2.post20230611/src/routers/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:15:08.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/routers/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     7559 2023-06-10 17:06:10.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/routers/root.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.855014 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:23:34.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/__init__.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.856290 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/generators/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:35:33.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/generators/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      372 2023-06-10 19:56:40.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/generators/char_generator.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     3155 2023-06-11 03:14:33.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/generators/population_generator.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.857068 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/parsers/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:39:13.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/parsers/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     2773 2023-06-11 03:50:06.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/parsers/args_parser.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 04:35:17.859296 hardy_weinberg_equilibrium-0.1.2.post20230611/tests/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:01:33.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/tests/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      637 2023-06-11 02:54:11.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/tests/test_asyncio.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      350 2023-06-10 17:11:37.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/tests/test_hardy_dist.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      940 2023-06-11 03:06:03.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/tests/test_hardy_weinberg.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1034 2023-06-11 03:25:22.000000 hardy_weinberg_equilibrium-0.1.2.post20230611/tests/test_threading.py
```

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/PKG-INFO` & `hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardy-weinberg-equilibrium
-Version: 0.1.1.post20230611
+Version: 0.1.2.post20230611
 Summary: Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the allele frequencies of a population in Hardy-Weinberg equilibrium.
 Home-page: https://github.com/dellius-alexander/FastAPI-GraphQL-MongoDB-Demo.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <info@hyfisolutions.com>
 Maintainer: info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <info@hyfisolutions.com>
 License:                     GNU GENERAL PUBLIC LICENSE
@@ -699,7 +699,38 @@
 
 # Hardy Weinberg Equilibrium
 
 
 Hardy-Weinberg Equilibrium Calculator. Calculates the expected 
 genotype frequencies based on the allele frequencies of a 
 population in Hardy-Weinberg equilibrium.
+
+## Usage
+
+```text
+usage: 
+    main.py [-h] [--version] [--verbose] [--debug] [--samples SAMPLES] [--p P] [--q Q] [--tpop TPOP] [--ppop PPOP] [--qpop QPOP] [--pq2pop PQ2POP] [--genes GENES [GENES ...]]
+
+Alternate module usage: 
+    python3 -m src.main [-h] [--version] [--verbose] [--debug] [--samples SAMPLES] [--p P] [--q Q] [--tpop TPOP] [--ppop PPOP] [--qpop QPOP] [--pq2pop PQ2POP] [--genes GENES [GENES ...]]
+
+
+Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the allele frequencies of a population in Hardy-Weinberg equilibrium. Alternate module usage: python3 -m src.main --ppop 10 --qpop 10
+--pq2pop 200 --verbose See: https://en.wikipedia.org/wiki/Hardy%E2%80%93Weinberg_principle
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --verbose             Enable verbose logging. (default: False)
+  --debug               Enable debug logging. (default: False)
+  --samples SAMPLES     Number of samples to generate, if using random data generator. (default: None)
+  --p P                 Frequency of dominant allele. (default: None)
+  --q Q                 Frequency of recessive allele. (default: None)
+  --tpop TPOP           Total population. (default: None)
+  --ppop PPOP           Original population of dominant allele. (default: None)
+  --qpop QPOP           Original population of recessive allele. (default: None)
+  --pq2pop PQ2POP       Original population of heterozygous allele. (default: None)
+  --genes GENES [GENES ...]
+                        List of JSON[Genes] to calculate. Note: This is list of json objects representing of Gene class. (default: <lambda>)
+
+Example: python3 -m main.py --ppop 10 --qpop 10 --pq2pop 200 --verbose | Example: python3 -m [package].[module] --samples 1000 --verbose
+```
```

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/Hardy_Weinberg_Equilibrium.egg-info/SOURCES.txt` & `hardy_weinberg_equilibrium-0.1.2.post20230611/Hardy_Weinberg_Equilibrium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/LICENSE` & `hardy_weinberg_equilibrium-0.1.2.post20230611/LICENSE`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/PKG-INFO` & `hardy_weinberg_equilibrium-0.1.2.post20230611/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardy_weinberg_equilibrium
-Version: 0.1.1.post20230611
+Version: 0.1.2.post20230611
 Summary: Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the allele frequencies of a population in Hardy-Weinberg equilibrium.
 Home-page: https://github.com/dellius-alexander/FastAPI-GraphQL-MongoDB-Demo.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <info@hyfisolutions.com>
 Maintainer: info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <info@hyfisolutions.com>
 License:                     GNU GENERAL PUBLIC LICENSE
@@ -699,7 +699,38 @@
 
 # Hardy Weinberg Equilibrium
 
 
 Hardy-Weinberg Equilibrium Calculator. Calculates the expected 
 genotype frequencies based on the allele frequencies of a 
 population in Hardy-Weinberg equilibrium.
+
+## Usage
+
+```text
+usage: 
+    main.py [-h] [--version] [--verbose] [--debug] [--samples SAMPLES] [--p P] [--q Q] [--tpop TPOP] [--ppop PPOP] [--qpop QPOP] [--pq2pop PQ2POP] [--genes GENES [GENES ...]]
+
+Alternate module usage: 
+    python3 -m src.main [-h] [--version] [--verbose] [--debug] [--samples SAMPLES] [--p P] [--q Q] [--tpop TPOP] [--ppop PPOP] [--qpop QPOP] [--pq2pop PQ2POP] [--genes GENES [GENES ...]]
+
+
+Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the allele frequencies of a population in Hardy-Weinberg equilibrium. Alternate module usage: python3 -m src.main --ppop 10 --qpop 10
+--pq2pop 200 --verbose See: https://en.wikipedia.org/wiki/Hardy%E2%80%93Weinberg_principle
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --verbose             Enable verbose logging. (default: False)
+  --debug               Enable debug logging. (default: False)
+  --samples SAMPLES     Number of samples to generate, if using random data generator. (default: None)
+  --p P                 Frequency of dominant allele. (default: None)
+  --q Q                 Frequency of recessive allele. (default: None)
+  --tpop TPOP           Total population. (default: None)
+  --ppop PPOP           Original population of dominant allele. (default: None)
+  --qpop QPOP           Original population of recessive allele. (default: None)
+  --pq2pop PQ2POP       Original population of heterozygous allele. (default: None)
+  --genes GENES [GENES ...]
+                        List of JSON[Genes] to calculate. Note: This is list of json objects representing of Gene class. (default: <lambda>)
+
+Example: python3 -m main.py --ppop 10 --qpop 10 --pq2pop 200 --verbose | Example: python3 -m [package].[module] --samples 1000 --verbose
+```
```

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/pyproject.toml` & `hardy_weinberg_equilibrium-0.1.2.post20230611/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hardy_weinberg_equilibrium"
-version = "0.1.1"
+version = "0.1.2"
 description = 'Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the allele frequencies of a population in Hardy-Weinberg equilibrium.'
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
 scripts = { main_cli = "main" }
 keywords = ["FastAPI", "Hardy Weinberg", "Python"]
 authors = [
   { name="Dellius Alexander",  email="info@hyfisolutions.com" },
```

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/setup.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     # print(long_description)
 
 setup(
     name="hardy_weinberg_equilibrium",
-    version="0.1.0",
+    version="0.1.2",
     author="Dellius Alexander",
     author_email="info@hyfisolutions.com",
     maintainer="info@hyfisolutions.com",
     maintainer_email="info@hyfisolutions.com",
     description='Hardy-Weinberg Equilibrium Calculator. '
                 'Calculates the expected genotype frequencies '
                 'based on the allele frequencies of a population '
```

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/config.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/config.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/genetics/allele.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/genetics/allele.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/genetics/gene.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/genetics/gene.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/hardy_weinberg/hardy_weinberg.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/hardy_weinberg/hardy_weinberg.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/hardy_weinberg/hardy_weinberg_stats.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/hardy_weinberg/hardy_weinberg_stats.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/main.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/main.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/routers/root.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/routers/root.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/generators/population_generator.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/generators/population_generator.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/src/utils/parsers/args_parser.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/src/utils/parsers/args_parser.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/tests/test_asyncio.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/tests/test_hardy_weinberg.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/tests/test_hardy_weinberg.py`

 * *Files identical despite different names*

### Comparing `hardy_weinberg_equilibrium-0.1.1.post20230611/tests/test_threading.py` & `hardy_weinberg_equilibrium-0.1.2.post20230611/tests/test_threading.py`

 * *Files identical despite different names*

