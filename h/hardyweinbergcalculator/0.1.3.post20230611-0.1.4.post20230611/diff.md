# Comparing `tmp/hardyweinbergcalculator-0.1.3.post20230611.tar.gz` & `tmp/hardyweinbergcalculator-0.1.4.post20230611.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardyweinbergcalculator-0.1.3.post20230611.tar", last modified: Sun Jun 11 15:58:51 2023, max compression
+gzip compressed data, was "hardyweinbergcalculator-0.1.4.post20230611.tar", last modified: Sun Jun 11 16:27:25 2023, max compression
```

## Comparing `hardyweinbergcalculator-0.1.3.post20230611.tar` & `hardyweinbergcalculator-0.1.4.post20230611.tar`

### file list

```diff
@@ -1,41 +1,38 @@
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.771016 hardyweinbergcalculator-0.1.3.post20230611/
--rw-r--r--   0 delliusalexander   (501) staff       (20)    35148 2023-06-10 04:05:55.000000 hardyweinbergcalculator-0.1.3.post20230611/LICENSE
--rw-r--r--   0 delliusalexander   (501) staff       (20)     3156 2023-06-11 15:58:51.771314 hardyweinbergcalculator-0.1.3.post20230611/PKG-INFO
--rw-r--r--   0 delliusalexander   (501) staff       (20)     2057 2023-06-11 04:31:17.000000 hardyweinbergcalculator-0.1.3.post20230611/README.md
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.753855 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/
--rw-r--r--   0 delliusalexander   (501) staff       (20)      416 2023-06-11 15:53:35.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)      526 2023-06-09 22:58:48.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/config.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.761516 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/genetics/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-10 17:11:37.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/genetics/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1243 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/genetics/allele.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     2778 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/genetics/gene.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.762898 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/hardy_weinberg/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-10 17:11:37.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/hardy_weinberg/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1816 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/hardy_weinberg/hardy_weinberg.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     9017 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/hardy_weinberg/hardy_weinberg_stats.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     4481 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/main.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.763451 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:23:34.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/__init__.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.764715 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/generators/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:35:33.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/generators/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)      372 2023-06-10 19:56:40.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/generators/char_generator.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     3235 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/generators/population_generator.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.765655 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/parsers/
--rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:39:13.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/parsers/__init__.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     2793 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/parsers/args_parser.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.759535 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/
--rw-r--r--   0 delliusalexander   (501) staff       (20)     3156 2023-06-11 15:58:51.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/PKG-INFO
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1205 2023-06-11 15:58:51.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/SOURCES.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)        1 2023-06-11 15:58:51.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/dependency_links.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)       53 2023-06-11 15:58:51.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/entry_points.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)        1 2023-06-11 15:58:51.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/not-zip-safe
--rw-r--r--   0 delliusalexander   (501) staff       (20)       30 2023-06-11 15:58:51.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/requires.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)       24 2023-06-11 15:58:51.000000 hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/top_level.txt
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1872 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/pyproject.toml
--rw-r--r--   0 delliusalexander   (501) staff       (20)      692 2023-06-11 15:58:51.772534 hardyweinbergcalculator-0.1.3.post20230611/setup.cfg
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1789 2023-06-11 15:58:20.000000 hardyweinbergcalculator-0.1.3.post20230611/setup.py
-drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 15:58:51.769890 hardyweinbergcalculator-0.1.3.post20230611/tests/
--rw-r--r--   0 delliusalexander   (501) staff       (20)      677 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/tests/test_asyncio.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)      383 2023-06-11 06:13:57.000000 hardyweinbergcalculator-0.1.3.post20230611/tests/test_hardy_dist.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1001 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/tests/test_hardy_weinberg.py
--rw-r--r--   0 delliusalexander   (501) staff       (20)     1114 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.3.post20230611/tests/test_threading.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.875123 hardyweinbergcalculator-0.1.4.post20230611/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)    35148 2023-06-10 04:05:55.000000 hardyweinbergcalculator-0.1.4.post20230611/LICENSE
+-rw-r--r--   0 delliusalexander   (501) staff       (20)    43642 2023-06-11 16:27:25.875758 hardyweinbergcalculator-0.1.4.post20230611/PKG-INFO
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     2057 2023-06-11 04:31:17.000000 hardyweinbergcalculator-0.1.4.post20230611/README.md
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.853995 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.859306 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/genetics/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-10 17:11:37.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/genetics/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1243 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/genetics/allele.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     2778 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/genetics/gene.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.861528 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardy_weinberg/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-10 17:11:37.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardy_weinberg/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1816 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardy_weinberg/hardy_weinberg.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     9017 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardy_weinberg/hardy_weinberg_stats.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.867469 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)    43642 2023-06-11 16:27:25.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/PKG-INFO
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1271 2023-06-11 16:27:25.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        1 2023-06-11 16:27:25.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)       77 2023-06-11 16:27:25.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/entry_points.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        1 2023-06-11 16:27:25.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/not-zip-safe
+-rw-r--r--   0 delliusalexander   (501) staff       (20)       30 2023-06-11 16:27:25.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/requires.txt
+-rw-r--r--   0 delliusalexander   (501) staff       (20)       30 2023-06-11 16:27:25.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/top_level.txt
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.868209 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:23:34.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/__init__.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.870147 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/generators/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:35:33.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/generators/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      372 2023-06-10 19:56:40.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/generators/char_generator.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     3235 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/generators/population_generator.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.871483 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/parsers/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)        0 2023-06-09 21:39:13.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/parsers/__init__.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     2793 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/parsers/args_parser.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     2337 2023-06-11 16:27:15.000000 hardyweinbergcalculator-0.1.4.post20230611/pyproject.toml
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      716 2023-06-11 16:27:25.877071 hardyweinbergcalculator-0.1.4.post20230611/setup.cfg
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1849 2023-06-11 16:21:46.000000 hardyweinbergcalculator-0.1.4.post20230611/setup.py
+drwxr-xr-x   0 delliusalexander   (501) staff       (20)        0 2023-06-11 16:27:25.874457 hardyweinbergcalculator-0.1.4.post20230611/tests/
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      677 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/tests/test_asyncio.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)      383 2023-06-11 06:13:57.000000 hardyweinbergcalculator-0.1.4.post20230611/tests/test_hardy_dist.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1001 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/tests/test_hardy_weinberg.py
+-rw-r--r--   0 delliusalexander   (501) staff       (20)     1114 2023-06-11 08:22:58.000000 hardyweinbergcalculator-0.1.4.post20230611/tests/test_threading.py
```

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/LICENSE` & `hardyweinbergcalculator-0.1.4.post20230611/LICENSE`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/PKG-INFO` & `hardyweinbergcalculator-0.1.4.post20230611/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: hardyweinbergcalculator
-Version: 0.1.3.post20230611
-Summary: Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the allele frequencies of a population in Hardy-Weinberg equilibrium.
-Author: Dellius Alexander
-Author-email: info@hyfisolutions.com
-Maintainer: info@hyfisolutions.com
-Maintainer-email: info@hyfisolutions.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Hardy Weinberg Equilibrium
 
 
 Hardy-Weinberg Equilibrium Calculator. Calculates the expected 
 genotype frequencies based on the allele frequencies of a 
 population in Hardy-Weinberg equilibrium.
```

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/genetics/allele.py` & `hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/genetics/allele.py`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/genetics/gene.py` & `hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/genetics/gene.py`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/hardy_weinberg/hardy_weinberg.py` & `hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardy_weinberg/hardy_weinberg.py`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/hardy_weinberg/hardy_weinberg_stats.py` & `hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardy_weinberg/hardy_weinberg_stats.py`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/generators/population_generator.py` & `hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/generators/population_generator.py`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator/utils/parsers/args_parser.py` & `hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/utils/parsers/args_parser.py`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/hardyweinbergcalculator.egg-info/SOURCES.txt` & `hardyweinbergcalculator-0.1.4.post20230611/hardyweinbergcalculator/hardyweinbergcalculator.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-hardyweinbergcalculator/__init__.py
-hardyweinbergcalculator/config.py
-hardyweinbergcalculator/main.py
-hardyweinbergcalculator.egg-info/PKG-INFO
-hardyweinbergcalculator.egg-info/SOURCES.txt
-hardyweinbergcalculator.egg-info/dependency_links.txt
-hardyweinbergcalculator.egg-info/entry_points.txt
-hardyweinbergcalculator.egg-info/not-zip-safe
-hardyweinbergcalculator.egg-info/requires.txt
-hardyweinbergcalculator.egg-info/top_level.txt
 hardyweinbergcalculator/genetics/__init__.py
 hardyweinbergcalculator/genetics/allele.py
 hardyweinbergcalculator/genetics/gene.py
 hardyweinbergcalculator/hardy_weinberg/__init__.py
 hardyweinbergcalculator/hardy_weinberg/hardy_weinberg.py
 hardyweinbergcalculator/hardy_weinberg/hardy_weinberg_stats.py
+hardyweinbergcalculator/hardyweinbergcalculator.egg-info/PKG-INFO
+hardyweinbergcalculator/hardyweinbergcalculator.egg-info/SOURCES.txt
+hardyweinbergcalculator/hardyweinbergcalculator.egg-info/dependency_links.txt
+hardyweinbergcalculator/hardyweinbergcalculator.egg-info/entry_points.txt
+hardyweinbergcalculator/hardyweinbergcalculator.egg-info/not-zip-safe
+hardyweinbergcalculator/hardyweinbergcalculator.egg-info/requires.txt
+hardyweinbergcalculator/hardyweinbergcalculator.egg-info/top_level.txt
 hardyweinbergcalculator/utils/__init__.py
 hardyweinbergcalculator/utils/generators/__init__.py
 hardyweinbergcalculator/utils/generators/char_generator.py
 hardyweinbergcalculator/utils/generators/population_generator.py
 hardyweinbergcalculator/utils/parsers/__init__.py
 hardyweinbergcalculator/utils/parsers/args_parser.py
 tests/test_asyncio.py
```

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/pyproject.toml` & `hardyweinbergcalculator-0.1.4.post20230611/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
-#
-#[project]
-#name = "hardyweinbergcalculator"
-#version = "0.1.2"
-#description = 'Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the allele frequencies of a population in Hardy-Weinberg equilibrium.'
-#readme = {file = "README.md", content-type = "text/markdown"}
-#requires-python = ">=3.7"
-#keywords = ["FastAPI", "Hardy Weinberg", "Python"]
-#authors = [
-#  { name="Dellius Alexander",  email="info@hyfisolutions.com" },
-#]
-#
-#maintainers = [
-#    { name="Dellius Alexander", email="info@hyfisolutions.com"}
-#]
-#
-#classifiers = [
-#    "Programming Language :: Python :: 3",
-#    "License :: OSI Approved :: MIT License",
-#    "Operating System :: OS Independent",
-#    "Development Status :: 3 - Alpha",
-#    "Intended Audience :: Developers",
-#    "Topic :: Software Development :: Libraries :: Python Modules",
-#    "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
-#    "Topic :: Internet :: WWW/HTTP :: WSGI :: Server",
-#    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
-#]
-
-#dependencies = [
-#    "sympy",
-#    "numpy",
-#    "matplotlib",
-#    "pandas",
-#]
+
+[project]
+name = "hardyweinbergcalculator"
+version = "0.1.4"
+description = 'Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the allele frequencies of a population in Hardy-Weinberg equilibrium.'
+readme = {file = "README.md", content-type = "text/markdown"}
+requires-python = ">=3.7"
+license = {file = "LICENSE", content-type = "text/plain"}
+keywords = ["FastAPI", "Hardy Weinberg", "Python"]
+authors = [
+  { name="Dellius Alexander",  email="info@hyfisolutions.com" },
+]
+
+maintainers = [
+    { name="Dellius Alexander", email="info@hyfisolutions.com"}
+]
+
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+    "Topic :: Internet :: WWW/HTTP :: WSGI :: Server",
+    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+]
+
+dependencies = [
+    "sympy",
+    "numpy",
+    "matplotlib",
+    "pandas",
+]
+
+[project.scripts]
+hardyweinbergcalculator = "hardyweinbergcalculator.main:app"
+
 
 #[project.urls]
 ## https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 #"Homepage" = "https://github.com/dellius-alexander/FastAPI-GraphQL-MongoDB-Demo.git"
 #"Bug_Tracker" = "https://github.com/dellius-alexander/FastAPI-GraphQL-MongoDB-Demo.git/issues"
 
 [requires]
@@ -58,10 +63,12 @@
 minversion = "6.0"
 addopts = "--verbose --color=yes --trace"
 testpaths = [
     "tests",
     "tests/integration",
 ]
 
-#[project.license]
-#file = "LICENSE"
-
+[tool.setuptools.packages.find]
+where = ["hardyweinbergcalculator"]  # list of folders that contain the packages (["."] by default)
+include = ["*"]  # package names should match these glob patterns (["*"] by default)
+#exclude = ["my_package.tests*"]  # exclude packages matching these glob patterns (empty by default)
+namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
```

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/setup.cfg` & `hardyweinbergcalculator-0.1.4.post20230611/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hardyweinbergcalculator
-version = 0.1.3
+version = 0.1.4
 auther = Dellius Alexander
 auther_email = info@hyfisolutions.com
 description = 
 	A package to calculate Hardy-Weinberg Equilibrium. Hardy-Weinberg Equilibrium Calculator.
 	Calculates the expected genotype frequencies based on the allele frequencies of a population
 	in Hardy-Weinberg equilibrium.
 long_description = file: README.md
@@ -24,9 +24,9 @@
 	sympy
 	numpy
 	matplotlib
 	pandas
 
 [options.entry_points]
 console_scripts = 
-	hwe = hardyweinbergcalculator.main
+	hardyweinbergcalculator = hardyweinbergcalculator.main:app
```

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/setup.py` & `hardyweinbergcalculator-0.1.4.post20230611/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Hardy-Weinberg Equilibrium Calculator. Calculates the expected genotype frequencies based on the ' \
               'allele frequencies of a population in Hardy-Weinberg equilibrium.'
 LONG_DESCRIPTION = None
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
@@ -34,15 +34,19 @@
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    entry_points={"console_scripts": ["hwe = hardyweinbergcalculator.main"]},
+    entry_points={
+        "console_scripts": [
+            "hardyweinbergcalculator = hardyweinbergcalculator.main:app"
+        ]
+    },
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         "sympy",
         "numpy",
         "matplotlib",
         "pandas",
```

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/tests/test_asyncio.py` & `hardyweinbergcalculator-0.1.4.post20230611/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/tests/test_hardy_weinberg.py` & `hardyweinbergcalculator-0.1.4.post20230611/tests/test_hardy_weinberg.py`

 * *Files identical despite different names*

### Comparing `hardyweinbergcalculator-0.1.3.post20230611/tests/test_threading.py` & `hardyweinbergcalculator-0.1.4.post20230611/tests/test_threading.py`

 * *Files identical despite different names*

