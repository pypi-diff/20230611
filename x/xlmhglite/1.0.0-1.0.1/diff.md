# Comparing `tmp/xlmhglite-1.0.0.tar.gz` & `tmp/xlmhglite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlmhglite-1.0.0.tar", last modified: Sun Jun 11 09:56:24 2023, max compression
+gzip compressed data, was "xlmhglite-1.0.1.tar", last modified: Sun Jun 11 10:04:39 2023, max compression
```

## Comparing `xlmhglite-1.0.0.tar` & `xlmhglite-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 09:56:24.957225 xlmhglite-1.0.0/
--rw-rw-rw-   0        0        0     1489 2022-10-18 12:34:21.000000 xlmhglite-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     6221 2023-06-11 09:56:24.957225 xlmhglite-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5137 2023-06-10 14:05:10.000000 xlmhglite-1.0.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-11 09:56:24.957225 xlmhglite-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4089 2023-06-11 07:55:16.000000 xlmhglite-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 09:56:24.933222 xlmhglite-1.0.0/xlmhglite/
--rw-rw-rw-   0        0        0      262 2023-06-11 07:51:28.000000 xlmhglite-1.0.0/xlmhglite/__init__.py
--rw-rw-rw-   0        0        0    11935 2023-06-10 12:47:41.000000 xlmhglite-1.0.0/xlmhglite/mhg.py
--rw-rw-rw-   0        0        0  1002952 2023-06-11 09:47:51.000000 xlmhglite-1.0.0/xlmhglite/mhg_cython.c
--rw-rw-rw-   0        0        0    12577 2023-06-11 09:47:10.000000 xlmhglite-1.0.0/xlmhglite/mhg_cython.pyx
--rw-rw-rw-   0        0        0     5633 2023-02-09 21:45:34.000000 xlmhglite-1.0.0/xlmhglite/result.py
--rw-rw-rw-   0        0        0    15086 2023-06-10 12:11:48.000000 xlmhglite-1.0.0/xlmhglite/test.py
--rw-rw-rw-   0        0        0    11984 2023-06-11 07:49:03.000000 xlmhglite-1.0.0/xlmhglite/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-11 09:56:24.949243 xlmhglite-1.0.0/xlmhglite.egg-info/
--rw-rw-rw-   0        0        0     6221 2023-06-11 09:56:24.000000 xlmhglite-1.0.0/xlmhglite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-06-11 09:56:24.000000 xlmhglite-1.0.0/xlmhglite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 09:56:24.000000 xlmhglite-1.0.0/xlmhglite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-11 09:56:24.000000 xlmhglite-1.0.0/xlmhglite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-11 09:56:24.000000 xlmhglite-1.0.0/xlmhglite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.725869 xlmhglite-1.0.1/
+-rw-rw-rw-   0        0        0      177 2023-06-11 10:03:43.000000 xlmhglite-1.0.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1489 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      250 2023-06-11 10:01:19.000000 xlmhglite-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6308 2023-06-11 10:04:39.725869 xlmhglite-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5137 2023-06-10 14:05:10.000000 xlmhglite-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.641775 xlmhglite-1.0.1/docs/
+-rw-rw-rw-   0        0        0     7840 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.542423 xlmhglite-1.0.1/docs/build/
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.562420 xlmhglite-1.0.1/docs/build/_images/
+-rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/build/_images/test_figure.png
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.590492 xlmhglite-1.0.1/docs/build/_static/
+-rw-rw-rw-   0        0        0      286 2023-05-14 14:35:23.000000 xlmhglite-1.0.1/docs/build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 xlmhglite-1.0.1/docs/build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 xlmhglite-1.0.1/docs/build/_static/plus.png
+-rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/build/_static/test_figure.png
+-rwxrwxrwx   0        0        0     7741 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.661603 xlmhglite-1.0.1/docs/source/
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.618437 xlmhglite-1.0.1/docs/source/_static/
+-rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/source/_static/test_figure.png
+-rw-rw-rw-   0        0        0     1916 2023-06-10 13:02:12.000000 xlmhglite-1.0.1/docs/source/api.rst
+-rw-rw-rw-   0        0        0     4673 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/source/background.rst
+-rw-rw-rw-   0        0        0      363 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/source/citing.rst
+-rw-rw-rw-   0        0        0     5326 2023-06-10 14:14:36.000000 xlmhglite-1.0.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0     2807 2023-06-10 13:01:06.000000 xlmhglite-1.0.1/docs/source/examples.rst
+-rw-rw-rw-   0        0        0       30 2023-05-15 20:30:53.000000 xlmhglite-1.0.1/docs/source/history.rst
+-rw-rw-rw-   0        0        0      312 2023-06-10 13:37:09.000000 xlmhglite-1.0.1/docs/source/index.rst
+-rw-rw-rw-   0        0        0     3052 2023-06-10 13:01:06.000000 xlmhglite-1.0.1/docs/source/install.rst
+-rw-rw-rw-   0        0        0     1960 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/source/license.rst
+-rw-rw-rw-   0        0        0       30 2019-07-11 11:49:50.000000 xlmhglite-1.0.1/docs/source/readme.rst
+-rw-rw-rw-   0        0        0       33 2023-06-10 14:10:04.000000 xlmhglite-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0      380 2023-06-10 13:11:55.000000 xlmhglite-1.0.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0      148 2023-02-09 08:44:48.000000 xlmhglite-1.0.1/requirements_extra.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 10:04:39.725869 xlmhglite-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     4089 2023-06-11 10:03:09.000000 xlmhglite-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.546420 xlmhglite-1.0.1/tests/
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.685604 xlmhglite-1.0.1/tests/01_algorithms/
+-rw-rw-rw-   0        0        0     3536 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_bound.py
+-rw-rw-rw-   0        0        0     3302 2023-06-10 11:23:08.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_escore.py
+-rw-rw-rw-   0        0        0     1594 2023-02-09 22:51:29.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_pval.py
+-rw-rw-rw-   0        0        0     5932 2023-06-10 12:32:34.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_python.py
+-rw-rw-rw-   0        0        0     2979 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_stat.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.697618 xlmhglite-1.0.1/tests/02_api/
+-rw-rw-rw-   0        0        0      931 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/tests/02_api/conftest.py
+-rw-rw-rw-   0        0        0     4293 2023-02-09 22:59:34.000000 xlmhglite-1.0.1/tests/02_api/test_advanced_api.py
+-rw-rw-rw-   0        0        0     1216 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/tests/02_api/test_result.py
+-rw-rw-rw-   0        0        0     1469 2023-02-09 23:00:14.000000 xlmhglite-1.0.1/tests/02_api/test_simple_api.py
+-rw-rw-rw-   0        0        0     1543 2023-06-11 07:41:42.000000 xlmhglite-1.0.1/tests/02_api/test_visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.715254 xlmhglite-1.0.1/xlmhglite/
+-rw-rw-rw-   0        0        0      262 2023-06-11 10:03:09.000000 xlmhglite-1.0.1/xlmhglite/__init__.py
+-rw-rw-rw-   0        0        0    11935 2023-06-10 12:47:41.000000 xlmhglite-1.0.1/xlmhglite/mhg.py
+-rw-rw-rw-   0        0        0  1002952 2023-06-11 09:47:51.000000 xlmhglite-1.0.1/xlmhglite/mhg_cython.c
+-rw-rw-rw-   0        0        0    12577 2023-06-11 09:47:10.000000 xlmhglite-1.0.1/xlmhglite/mhg_cython.pyx
+-rw-rw-rw-   0        0        0     5633 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/xlmhglite/result.py
+-rw-rw-rw-   0        0        0    15086 2023-06-10 12:11:48.000000 xlmhglite-1.0.1/xlmhglite/test.py
+-rw-rw-rw-   0        0        0    11984 2023-06-11 07:49:03.000000 xlmhglite-1.0.1/xlmhglite/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.721897 xlmhglite-1.0.1/xlmhglite.egg-info/
+-rw-rw-rw-   0        0        0     6308 2023-06-11 10:04:37.000000 xlmhglite-1.0.1/xlmhglite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1689 2023-06-11 10:04:39.000000 xlmhglite-1.0.1/xlmhglite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 10:04:37.000000 xlmhglite-1.0.1/xlmhglite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-11 10:04:37.000000 xlmhglite-1.0.1/xlmhglite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-11 10:04:37.000000 xlmhglite-1.0.1/xlmhglite.egg-info/top_level.txt
```

### Comparing `xlmhglite-1.0.0/LICENSE` & `xlmhglite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.0/PKG-INFO` & `xlmhglite-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlmhglite
-Version: 1.0.0
+Version: 1.0.1
 Summary: XL-mHG lite: A light implementation of the Semiparametric Enrichment Test
 Home-page: https://github.com/GuyTeichman/xlmhglite
 Author: Guy Teichman
 Author-email: guyteichman@gmail.com
 License: GPLv3
 Keywords: statistics,nonparametric,semiparametric,enrichment test,ranked lists
 Classifier: Development Status :: 5 - Production/Stable
@@ -158,10 +158,14 @@
     :target: https://github.com/GuyTeichman/xlmhglite/actions/workflows/tests.yml
     :alt: Build status
 
 =======
 History
 =======
 
+1.0.1 (2023-06-11)
+------------------
+Minor patch addressing installation issues.
+
 1.0.0 (2023-06-10)
 ------------------
 First stable release.
```

### Comparing `xlmhglite-1.0.0/README.rst` & `xlmhglite-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.0/setup.py` & `xlmhglite-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     return extra_deps
 
 
 here = path.abspath(path.dirname(__file__))
 root = 'xlmhglite'
 description = 'XL-mHG lite: A light implementation of the Semiparametric Enrichment Test'
-version = '1.0.0'
+version = '1.0.1'
 
 with open('README.rst', encoding='utf8') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `xlmhglite-1.0.0/xlmhglite/mhg.py` & `xlmhglite-1.0.1/xlmhglite/mhg.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.0/xlmhglite/mhg_cython.c` & `xlmhglite-1.0.1/xlmhglite/mhg_cython.c`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.0/xlmhglite/mhg_cython.pyx` & `xlmhglite-1.0.1/xlmhglite/mhg_cython.pyx`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.0/xlmhglite/result.py` & `xlmhglite-1.0.1/xlmhglite/result.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.0/xlmhglite/test.py` & `xlmhglite-1.0.1/xlmhglite/test.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.0/xlmhglite/visualize.py` & `xlmhglite-1.0.1/xlmhglite/visualize.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.0/xlmhglite.egg-info/PKG-INFO` & `xlmhglite-1.0.1/xlmhglite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlmhglite
-Version: 1.0.0
+Version: 1.0.1
 Summary: XL-mHG lite: A light implementation of the Semiparametric Enrichment Test
 Home-page: https://github.com/GuyTeichman/xlmhglite
 Author: Guy Teichman
 Author-email: guyteichman@gmail.com
 License: GPLv3
 Keywords: statistics,nonparametric,semiparametric,enrichment test,ranked lists
 Classifier: Development Status :: 5 - Production/Stable
@@ -158,10 +158,14 @@
     :target: https://github.com/GuyTeichman/xlmhglite/actions/workflows/tests.yml
     :alt: Build status
 
 =======
 History
 =======
 
+1.0.1 (2023-06-11)
+------------------
+Minor patch addressing installation issues.
+
 1.0.0 (2023-06-10)
 ------------------
 First stable release.
```

