# Comparing `tmp/xlmhglite-1.0.1.tar.gz` & `tmp/xlmhglite-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlmhglite-1.0.1.tar", last modified: Sun Jun 11 10:04:39 2023, max compression
+gzip compressed data, was "xlmhglite-1.1.0.tar", last modified: Sun Jun 11 15:32:17 2023, max compression
```

## Comparing `xlmhglite-1.0.1.tar` & `xlmhglite-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.725869 xlmhglite-1.0.1/
--rw-rw-rw-   0        0        0      177 2023-06-11 10:03:43.000000 xlmhglite-1.0.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1489 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      250 2023-06-11 10:01:19.000000 xlmhglite-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6308 2023-06-11 10:04:39.725869 xlmhglite-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5137 2023-06-10 14:05:10.000000 xlmhglite-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.641775 xlmhglite-1.0.1/docs/
--rw-rw-rw-   0        0        0     7840 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.542423 xlmhglite-1.0.1/docs/build/
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.562420 xlmhglite-1.0.1/docs/build/_images/
--rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/build/_images/test_figure.png
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.590492 xlmhglite-1.0.1/docs/build/_static/
--rw-rw-rw-   0        0        0      286 2023-05-14 14:35:23.000000 xlmhglite-1.0.1/docs/build/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 xlmhglite-1.0.1/docs/build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 xlmhglite-1.0.1/docs/build/_static/plus.png
--rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/build/_static/test_figure.png
--rwxrwxrwx   0        0        0     7741 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.661603 xlmhglite-1.0.1/docs/source/
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.618437 xlmhglite-1.0.1/docs/source/_static/
--rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/source/_static/test_figure.png
--rw-rw-rw-   0        0        0     1916 2023-06-10 13:02:12.000000 xlmhglite-1.0.1/docs/source/api.rst
--rw-rw-rw-   0        0        0     4673 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/source/background.rst
--rw-rw-rw-   0        0        0      363 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/source/citing.rst
--rw-rw-rw-   0        0        0     5326 2023-06-10 14:14:36.000000 xlmhglite-1.0.1/docs/source/conf.py
--rw-rw-rw-   0        0        0     2807 2023-06-10 13:01:06.000000 xlmhglite-1.0.1/docs/source/examples.rst
--rw-rw-rw-   0        0        0       30 2023-05-15 20:30:53.000000 xlmhglite-1.0.1/docs/source/history.rst
--rw-rw-rw-   0        0        0      312 2023-06-10 13:37:09.000000 xlmhglite-1.0.1/docs/source/index.rst
--rw-rw-rw-   0        0        0     3052 2023-06-10 13:01:06.000000 xlmhglite-1.0.1/docs/source/install.rst
--rw-rw-rw-   0        0        0     1960 2022-10-18 12:34:21.000000 xlmhglite-1.0.1/docs/source/license.rst
--rw-rw-rw-   0        0        0       30 2019-07-11 11:49:50.000000 xlmhglite-1.0.1/docs/source/readme.rst
--rw-rw-rw-   0        0        0       33 2023-06-10 14:10:04.000000 xlmhglite-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0      380 2023-06-10 13:11:55.000000 xlmhglite-1.0.1/requirements_dev.txt
--rw-rw-rw-   0        0        0      148 2023-02-09 08:44:48.000000 xlmhglite-1.0.1/requirements_extra.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 10:04:39.725869 xlmhglite-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4089 2023-06-11 10:03:09.000000 xlmhglite-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.546420 xlmhglite-1.0.1/tests/
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.685604 xlmhglite-1.0.1/tests/01_algorithms/
--rw-rw-rw-   0        0        0     3536 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_bound.py
--rw-rw-rw-   0        0        0     3302 2023-06-10 11:23:08.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_escore.py
--rw-rw-rw-   0        0        0     1594 2023-02-09 22:51:29.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_pval.py
--rw-rw-rw-   0        0        0     5932 2023-06-10 12:32:34.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_python.py
--rw-rw-rw-   0        0        0     2979 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/tests/01_algorithms/test_correct_stat.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.697618 xlmhglite-1.0.1/tests/02_api/
--rw-rw-rw-   0        0        0      931 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/tests/02_api/conftest.py
--rw-rw-rw-   0        0        0     4293 2023-02-09 22:59:34.000000 xlmhglite-1.0.1/tests/02_api/test_advanced_api.py
--rw-rw-rw-   0        0        0     1216 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/tests/02_api/test_result.py
--rw-rw-rw-   0        0        0     1469 2023-02-09 23:00:14.000000 xlmhglite-1.0.1/tests/02_api/test_simple_api.py
--rw-rw-rw-   0        0        0     1543 2023-06-11 07:41:42.000000 xlmhglite-1.0.1/tests/02_api/test_visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.715254 xlmhglite-1.0.1/xlmhglite/
--rw-rw-rw-   0        0        0      262 2023-06-11 10:03:09.000000 xlmhglite-1.0.1/xlmhglite/__init__.py
--rw-rw-rw-   0        0        0    11935 2023-06-10 12:47:41.000000 xlmhglite-1.0.1/xlmhglite/mhg.py
--rw-rw-rw-   0        0        0  1002952 2023-06-11 09:47:51.000000 xlmhglite-1.0.1/xlmhglite/mhg_cython.c
--rw-rw-rw-   0        0        0    12577 2023-06-11 09:47:10.000000 xlmhglite-1.0.1/xlmhglite/mhg_cython.pyx
--rw-rw-rw-   0        0        0     5633 2023-02-09 21:45:34.000000 xlmhglite-1.0.1/xlmhglite/result.py
--rw-rw-rw-   0        0        0    15086 2023-06-10 12:11:48.000000 xlmhglite-1.0.1/xlmhglite/test.py
--rw-rw-rw-   0        0        0    11984 2023-06-11 07:49:03.000000 xlmhglite-1.0.1/xlmhglite/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:04:39.721897 xlmhglite-1.0.1/xlmhglite.egg-info/
--rw-rw-rw-   0        0        0     6308 2023-06-11 10:04:37.000000 xlmhglite-1.0.1/xlmhglite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1689 2023-06-11 10:04:39.000000 xlmhglite-1.0.1/xlmhglite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 10:04:37.000000 xlmhglite-1.0.1/xlmhglite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-11 10:04:37.000000 xlmhglite-1.0.1/xlmhglite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-11 10:04:37.000000 xlmhglite-1.0.1/xlmhglite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.533966 xlmhglite-1.1.0/
+-rw-rw-rw-   0        0        0      918 2023-06-11 15:30:51.000000 xlmhglite-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1489 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      256 2023-06-11 14:39:58.000000 xlmhglite-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7038 2023-06-11 15:32:17.534923 xlmhglite-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5141 2023-06-11 15:31:26.000000 xlmhglite-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.437384 xlmhglite-1.1.0/docs/
+-rw-rw-rw-   0        0        0     7840 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.358816 xlmhglite-1.1.0/docs/build/
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.391810 xlmhglite-1.1.0/docs/build/_images/
+-rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/docs/build/_images/test_figure.png
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.402815 xlmhglite-1.1.0/docs/build/_static/
+-rw-rw-rw-   0        0        0      286 2023-05-14 14:35:23.000000 xlmhglite-1.1.0/docs/build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 xlmhglite-1.1.0/docs/build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 xlmhglite-1.1.0/docs/build/_static/plus.png
+-rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/docs/build/_static/test_figure.png
+-rwxrwxrwx   0        0        0     7741 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.450386 xlmhglite-1.1.0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.429379 xlmhglite-1.1.0/docs/source/_static/
+-rw-rw-rw-   0        0        0    33754 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/docs/source/_static/test_figure.png
+-rw-rw-rw-   0        0        0     1916 2023-06-10 13:02:12.000000 xlmhglite-1.1.0/docs/source/api.rst
+-rw-rw-rw-   0        0        0     4673 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/docs/source/background.rst
+-rw-rw-rw-   0        0        0      363 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/docs/source/citing.rst
+-rw-rw-rw-   0        0        0     5326 2023-06-10 14:14:36.000000 xlmhglite-1.1.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0     2807 2023-06-10 13:01:06.000000 xlmhglite-1.1.0/docs/source/examples.rst
+-rw-rw-rw-   0        0        0       30 2023-05-15 20:30:53.000000 xlmhglite-1.1.0/docs/source/history.rst
+-rw-rw-rw-   0        0        0      312 2023-06-10 13:37:09.000000 xlmhglite-1.1.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0     3052 2023-06-10 13:01:06.000000 xlmhglite-1.1.0/docs/source/install.rst
+-rw-rw-rw-   0        0        0     1960 2022-10-18 12:34:21.000000 xlmhglite-1.1.0/docs/source/license.rst
+-rw-rw-rw-   0        0        0       30 2019-07-11 11:49:50.000000 xlmhglite-1.1.0/docs/source/readme.rst
+-rw-rw-rw-   0        0        0      116 2023-06-11 14:39:58.000000 xlmhglite-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      380 2023-06-10 13:11:55.000000 xlmhglite-1.1.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     1228 2023-06-11 15:32:17.535930 xlmhglite-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      376 2023-06-11 14:46:03.000000 xlmhglite-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.364812 xlmhglite-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.470384 xlmhglite-1.1.0/tests/01_algorithms/
+-rw-rw-rw-   0        0        0     3536 2023-02-09 21:45:34.000000 xlmhglite-1.1.0/tests/01_algorithms/test_correct_bound.py
+-rw-rw-rw-   0        0        0     3302 2023-06-10 11:23:08.000000 xlmhglite-1.1.0/tests/01_algorithms/test_correct_escore.py
+-rw-rw-rw-   0        0        0     1594 2023-02-09 22:51:29.000000 xlmhglite-1.1.0/tests/01_algorithms/test_correct_pval.py
+-rw-rw-rw-   0        0        0     5932 2023-06-10 12:32:34.000000 xlmhglite-1.1.0/tests/01_algorithms/test_correct_python.py
+-rw-rw-rw-   0        0        0     2979 2023-02-09 21:45:34.000000 xlmhglite-1.1.0/tests/01_algorithms/test_correct_stat.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.482389 xlmhglite-1.1.0/tests/02_api/
+-rw-rw-rw-   0        0        0      931 2023-02-09 21:45:34.000000 xlmhglite-1.1.0/tests/02_api/conftest.py
+-rw-rw-rw-   0        0        0     4293 2023-02-09 22:59:34.000000 xlmhglite-1.1.0/tests/02_api/test_advanced_api.py
+-rw-rw-rw-   0        0        0     1216 2023-02-09 21:45:34.000000 xlmhglite-1.1.0/tests/02_api/test_result.py
+-rw-rw-rw-   0        0        0     1469 2023-02-09 23:00:14.000000 xlmhglite-1.1.0/tests/02_api/test_simple_api.py
+-rw-rw-rw-   0        0        0     1543 2023-06-11 07:41:42.000000 xlmhglite-1.1.0/tests/02_api/test_visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.500384 xlmhglite-1.1.0/xlmhglite/
+-rw-rw-rw-   0        0        0      491 2023-06-11 15:19:26.000000 xlmhglite-1.1.0/xlmhglite/__init__.py
+-rw-rw-rw-   0        0        0    11935 2023-06-11 15:16:50.000000 xlmhglite-1.1.0/xlmhglite/mhg.py
+-rw-rw-rw-   0        0        0  1009588 2023-06-11 14:47:49.000000 xlmhglite-1.1.0/xlmhglite/mhg_cython.c
+-rw-rw-rw-   0        0        0    12577 2023-06-11 09:47:10.000000 xlmhglite-1.1.0/xlmhglite/mhg_cython.pyx
+-rw-rw-rw-   0        0        0     5569 2023-06-11 15:03:51.000000 xlmhglite-1.1.0/xlmhglite/result.py
+-rw-rw-rw-   0        0        0    14924 2023-06-11 14:59:51.000000 xlmhglite-1.1.0/xlmhglite/test.py
+-rw-rw-rw-   0        0        0    11984 2023-06-11 07:49:03.000000 xlmhglite-1.1.0/xlmhglite/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:32:17.532968 xlmhglite-1.1.0/xlmhglite.egg-info/
+-rw-rw-rw-   0        0        0     7038 2023-06-11 15:32:15.000000 xlmhglite-1.1.0/xlmhglite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1730 2023-06-11 15:32:17.000000 xlmhglite-1.1.0/xlmhglite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 15:32:15.000000 xlmhglite-1.1.0/xlmhglite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-11 15:32:15.000000 xlmhglite-1.1.0/xlmhglite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-11 15:32:15.000000 xlmhglite-1.1.0/xlmhglite.egg-info/top_level.txt
```

### Comparing `xlmhglite-1.0.1/LICENSE` & `xlmhglite-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/PKG-INFO` & `xlmhglite-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlmhglite
-Version: 1.0.1
+Version: 1.1.0
 Summary: XL-mHG lite: A light implementation of the Semiparametric Enrichment Test
 Home-page: https://github.com/GuyTeichman/xlmhglite
 Author: Guy Teichman
 Author-email: guyteichman@gmail.com
 License: GPLv3
 Keywords: statistics,nonparametric,semiparametric,enrichment test,ranked lists
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,16 +14,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.8
-Provides-Extra: plotly
-Provides-Extra: visualize
+Description-Content-Type: text/x-rst
 Provides-Extra: all
 License-File: LICENSE
 
 XL-mHG Lite
 =============
 
 
@@ -76,18 +75,18 @@
 
 - ``stat``: The XL-mHG test statistic
 - ``cutoff``: The cutoff at which XL-mHG test statistic was attained
 - ``pval``: The XL-mHG p-value
 
 __ user_manual_
 
-Documentation
--------------
+XL-mHG Lite Documentation
+---------------------------
 
-Please refer to the `XL-mHG User Manual`__ (hosted on ReadTheDocs).
+Please refer to the `XL-mHG User Manual`__.
 
 __ user_manual_
 
 Citing XL-mHG
 -------------
 
 If you use the XL-mHG test in your research, please cite `Eden et al. (PLoS
@@ -154,18 +153,33 @@
     :target: https://pypi.python.org/pypi/xlmhglite
     :alt: Python versions supported
 
 ..  |githubactions| image:: https://github.com/guyteichman/xlmhglite/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/GuyTeichman/xlmhglite/actions/workflows/tests.yml
     :alt: Build status
 
-=======
+
 History
 =======
 
+1.1.0 (2023-06-11)
+------------------
+This version improves clarity of warning messages and addresses some additional bugs.
+Moreover, the project has been transitioned to use pyproject.toml and setup.cfg, and old code was cleaned up for better maintainability.
+
+Changed
+********
+* Warning messages regarding failed import of the cython module were made more informative.
+* Transitioned the project to use pyproject.toml and setup.cfg, and cleaned up legacy code from setup.py.
+
+Fixed
+******
+* Fixed bug where calculating enrichment scores using the pure Python implementation would raise an AttributeError.
+* Fixed bug where the pure Python implementation would raise an ImportError if numba is not already installed on the system.
+
 1.0.1 (2023-06-11)
 ------------------
 Minor patch addressing installation issues.
 
 1.0.0 (2023-06-10)
 ------------------
 First stable release.
```

### Comparing `xlmhglite-1.0.1/README.rst` & `xlmhglite-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
 
 - ``stat``: The XL-mHG test statistic
 - ``cutoff``: The cutoff at which XL-mHG test statistic was attained
 - ``pval``: The XL-mHG p-value
 
 __ user_manual_
 
-Documentation
--------------
+XL-mHG Lite Documentation
+---------------------------
 
-Please refer to the `XL-mHG User Manual`__ (hosted on ReadTheDocs).
+Please refer to the `XL-mHG User Manual`__.
 
 __ user_manual_
 
 Citing XL-mHG
 -------------
 
 If you use the XL-mHG test in your research, please cite `Eden et al. (PLoS
@@ -127,8 +127,8 @@
     :alt: Downloads
 .. |versionssupported| image:: https://img.shields.io/pypi/pyversions/xlmhglite.svg
     :target: https://pypi.python.org/pypi/xlmhglite
     :alt: Python versions supported
 
 ..  |githubactions| image:: https://github.com/guyteichman/xlmhglite/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/GuyTeichman/xlmhglite/actions/workflows/tests.yml
-    :alt: Build status
+    :alt: Build status
```

### Comparing `xlmhglite-1.0.1/docs/Makefile` & `xlmhglite-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/build/_images/test_figure.png` & `xlmhglite-1.1.0/docs/build/_images/test_figure.png`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/build/_static/test_figure.png` & `xlmhglite-1.1.0/docs/build/_static/test_figure.png`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/make.bat` & `xlmhglite-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/source/_static/test_figure.png` & `xlmhglite-1.1.0/docs/source/_static/test_figure.png`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/source/api.rst` & `xlmhglite-1.1.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/source/background.rst` & `xlmhglite-1.1.0/docs/source/background.rst`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/source/conf.py` & `xlmhglite-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/source/examples.rst` & `xlmhglite-1.1.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/source/install.rst` & `xlmhglite-1.1.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/docs/source/license.rst` & `xlmhglite-1.1.0/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/01_algorithms/test_correct_bound.py` & `xlmhglite-1.1.0/tests/01_algorithms/test_correct_bound.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/01_algorithms/test_correct_escore.py` & `xlmhglite-1.1.0/tests/01_algorithms/test_correct_escore.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/01_algorithms/test_correct_pval.py` & `xlmhglite-1.1.0/tests/01_algorithms/test_correct_pval.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/01_algorithms/test_correct_python.py` & `xlmhglite-1.1.0/tests/01_algorithms/test_correct_python.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/01_algorithms/test_correct_stat.py` & `xlmhglite-1.1.0/tests/01_algorithms/test_correct_stat.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/02_api/conftest.py` & `xlmhglite-1.1.0/tests/02_api/conftest.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/02_api/test_advanced_api.py` & `xlmhglite-1.1.0/tests/02_api/test_advanced_api.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/02_api/test_result.py` & `xlmhglite-1.1.0/tests/02_api/test_result.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/02_api/test_simple_api.py` & `xlmhglite-1.1.0/tests/02_api/test_simple_api.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/tests/02_api/test_visualize.py` & `xlmhglite-1.1.0/tests/02_api/test_visualize.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/xlmhglite/mhg.py` & `xlmhglite-1.1.0/xlmhglite/mhg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright (c) 2016-2019 Florian Wagner
 #
 # This file is part of XL-mHG.
 
 """XL-mHG Python implementation."""
 
-import numba
 import numpy as np
 
 DEFAULT_TOL = 1e-12
 
 
-@numba.njit()
+def get_default_tol():
+    return float(DEFAULT_TOL)
+
+
 def is_equal(a: float, b: float, tol: float):
     """Ratio test to check if two floating point numbers are equal.
 
     Parameters
     ----------
     a: float
         The first floating point number.
@@ -30,15 +32,14 @@
     """
     if a == b or abs(a - b) <= tol * max(abs(a), abs(b)):
         return True
     else:
         return False
 
 
-@numba.njit()
 def get_hgp(p, k, N, K, n):
     """Calculate the hypergeometric p-value when p = f(k; N,K,n) is already known.
     """
     pval = p
     while k < min(K, n):
         p *= (float((n - k) * (K - k) / float((k + 1) * (N - K - n + k + 1))))
         pval += p
@@ -121,15 +122,15 @@
             if hgp <= stat:
                 stat = hgp
                 cutoff = n
         i += 1
     stat = min(stat, 1.0)  # because we initially set stat to 1.1
     return stat, cutoff
 
-# @numba.njit()
+
 def get_xlmhg_pval1(N: int, K: int, X: int, L: int, stat: float, tol: float = DEFAULT_TOL):
     """Calculate the XL-mHG p-value using "Algorithm 1".
 
     Parameters
     ----------
     N: int
         The length of the list.
```

### Comparing `xlmhglite-1.0.1/xlmhglite/mhg_cython.c` & `xlmhglite-1.1.0/xlmhglite/mhg_cython.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,42 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
+
+/* BEGIN: Cython Metadata
+{
+    "distutils": {
+        "depends": [
+            "C:\\Users\\Guy_Teichman\\AppData\\Local\\Temp\\pip-build-env-zq6cttwt\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "C:\\Users\\Guy_Teichman\\AppData\\Local\\Temp\\pip-build-env-zq6cttwt\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "C:\\Users\\Guy_Teichman\\AppData\\Local\\Temp\\pip-build-env-zq6cttwt\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "C:\\Users\\Guy_Teichman\\AppData\\Local\\Temp\\pip-build-env-zq6cttwt\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "C:\\Users\\Guy_Teichman\\AppData\\Local\\Temp\\pip-build-env-zq6cttwt\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+        ],
+        "include_dirs": [
+            "C:\\Users\\Guy_Teichman\\AppData\\Local\\Temp\\pip-build-env-zq6cttwt\\overlay\\Lib\\site-packages\\numpy\\core\\include"
+        ],
+        "name": "xlmhglite.mhg_cython",
+        "sources": [
+            "xlmhglite/mhg_cython.pyx"
+        ]
+    },
+    "module_name": "xlmhglite.mhg_cython"
+}
+END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,24 +96,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -199,15 +225,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +264,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -548,35 +574,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1092,195 +1118,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":689
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":690
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":691
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":692
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":696
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":697
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":698
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":699
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":703
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":704
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":713
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":714
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":715
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":717
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":718
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":719
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":721
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":722
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":724
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":725
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":726
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1311,42 +1337,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":728
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":729
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":730
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":732
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1833,26 +1859,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1986,22 +2012,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -6680,15 +6714,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_indices, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":734
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6697,29 +6731,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":735
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":734
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6730,15 +6764,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":737
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6747,29 +6781,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":738
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":737
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6780,15 +6814,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":740
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6797,29 +6831,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":741
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":740
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6830,15 +6864,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":743
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6847,29 +6881,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":744
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":743
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6880,15 +6914,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":746
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6897,29 +6931,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":747
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":746
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6930,212 +6964,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":749
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":750
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":751
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":750
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":753
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":749
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":928
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":929
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":930
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":928
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":932
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":933
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":934
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":935
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":934
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":936
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":932
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":940
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7151,15 +7185,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":941
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7167,53 +7201,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":942
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":941
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":943
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":944
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -7221,30 +7255,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":941
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":940
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7259,15 +7293,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":946
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7283,15 +7317,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":947
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7299,53 +7333,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":948
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":947
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":949
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":950
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -7353,30 +7387,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":947
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":946
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7391,15 +7425,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":952
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7415,15 +7449,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":953
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7431,53 +7465,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":954
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":953
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":955
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":956
+      /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -7485,30 +7519,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":953
+    /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":952
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7523,176 +7557,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":966
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":978
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":966
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":981
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":993
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":981
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":996
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":1003
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":996
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":1006
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":1010
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":1006
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":1013
+/* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":1017
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":1013
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8001,15 +8035,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -9979,15 +10013,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -12282,15 +12316,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -12355,15 +12389,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -20558,15 +20592,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -20925,15 +20959,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -21047,15 +21081,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -21311,15 +21345,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -21460,15 +21494,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -21667,26 +21701,26 @@
  * 
  *     cdef long double hgp
  */
   __pyx_tuple_ = PyTuple_Pack(2, __pyx_float_1_0, __pyx_int_0); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":944
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "C:/Users/Guy_Teichman/anaconda3/envs/py38/lib/site-packages/numpy/__init__.pxd":950
+  /* "C:/Users/Guy_Teichman/AppData/Local/Temp/pip-build-env-zq6cttwt/overlay/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -22025,15 +22059,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_0 = PyFloat_FromDouble(0.0); if (unlikely(!__pyx_float_0_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1_0 = PyFloat_FromDouble(1.0); if (unlikely(!__pyx_float_1_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1eneg_12 = PyFloat_FromDouble(1e-12); if (unlikely(!__pyx_float_1eneg_12)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -22152,55 +22186,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -22386,15 +22404,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_xlmhglite__mhg_cython) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -22781,17 +22799,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -23404,28 +23420,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -23938,15 +23954,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -24668,61 +24684,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -24730,15 +24764,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -25982,15 +26016,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -26136,15 +26170,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -26288,15 +26322,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26560,15 +26594,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26756,15 +26790,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `xlmhglite-1.0.1/xlmhglite/mhg_cython.pyx` & `xlmhglite-1.1.0/xlmhglite/mhg_cython.pyx`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/xlmhglite/result.py` & `xlmhglite-1.1.0/xlmhglite/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) 2016-2019 Florian Wagner
 #
 # This file is part of XL-mHG.
 
 """Contains the `mHGResult` class."""
 
-import sys
 import hashlib
 import logging
 
 import numpy as np
 
+from . import cython_warning
+
 try:
     # This is a duct-tape fix for the Google App Engine, on which importing
     # the C extension fails.
     from . import mhg_cython
 except ImportError:
-    print('Warning (xlmhglite): Failed to import "mhg_cython" C extension.',
-          file=sys.stderr)
+    cython_warning()
     from . import mhg as mhg_cython
 
 logger = logging.getLogger(__name__)
 
 
 class mHGResult(object):
     """The result of an XL-mHG test.
```

### Comparing `xlmhglite-1.0.1/xlmhglite/test.py` & `xlmhglite-1.1.0/xlmhglite/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # Copyright (c) 2016-2019 Florian Wagner
 #
 # This file is part of XL-mHG.
 
 """Python API for performing XL-mHG tests."""
 
-import sys
-from math import isnan
 import logging
+from math import isnan
 
 import numpy as np
 
-from . import mhg
+from . import cython_warning
+
 try:
     # This is a duct-tape fix for the Google App Engine, on which importing
     # the C extension fails.
     from . import mhg_cython
 except ImportError:
-    print('Warning (xlmhglite): Failed to import the "mhg_cython" C extension.'
-          'Falling back to the pure Python implementation, which is very '
-          'slow.', file=sys.stderr)
+    cython_warning()
     from . import mhg as mhg_cython
 
 from .result import mHGResult
 
 logger = logging.getLogger(__name__)
 
 
@@ -37,20 +35,20 @@
     max_X1 = max(X, 1)  # there is never a p-value based on zero 1's
 
     if stat == 1.0:
         return 1.0  # by definition
     elif min_KL == 0 or X > min_KL:
         return 0.0
 
-    upper_bound = min((min_KL-max_X1+1)*stat, 1.0)
+    upper_bound = min((min_KL - max_X1 + 1) * stat, 1.0)
     return upper_bound
 
 
 def get_xlmhg_test_result(N, indices, X=None, L=None,
-                          exact_pval='always', # if_necessary, if_significant
+                          exact_pval='always',  # if_necessary, if_significant
                           pval_thresh=None, escore_pval_thresh=None,
                           table=None, use_alg1=False, tol=1e-12):
     """Perform an XL-mHG test.
 
     This function accepts a list in the form of a numpy ``indices`` array
     containing the indices of the non-zero elements (sorted), along with the
     length ``N`` of the list. It returns an `mHGResult` object.
@@ -106,28 +104,28 @@
     Returns
     -------
     `mHGResult`
         The test result.
     """
     # type checks
     assert isinstance(N, (int, np.integer))
-    assert isinstance(indices, np.ndarray) and indices.ndim == 1 and\
-        np.issubdtype(indices.dtype, np.uint16)
+    assert isinstance(indices, np.ndarray) and indices.ndim == 1 and \
+           np.issubdtype(indices.dtype, np.uint16)
     if X is not None:
         assert isinstance(X, (int, np.integer))
     if L is not None:
         assert isinstance(L, (int, np.integer))
     assert isinstance(exact_pval, str)
     if pval_thresh is not None:
         assert isinstance(pval_thresh, float)
     if escore_pval_thresh is not None:
         assert isinstance(escore_pval_thresh, float)
     if table is not None:
         assert isinstance(table, np.ndarray) and table.ndim == 2 and \
-            np.issubdtype(table.dtype, np.longdouble)
+               np.issubdtype(table.dtype, np.longdouble)
     assert isinstance(use_alg1, (bool, np.bool_))
     assert isinstance(tol, float)
 
     # assign default values, if None
     K = indices.size
     if X is None:
         X = 0
@@ -140,41 +138,41 @@
                          '"np.ascontiguousarray()".')
     if N > 65536:
         raise ValueError(
             'Length of list cannot exceed 65536.'
         )
     if not (0 <= X <= N):
         raise ValueError(
-            'Invalid value X=%d; should be >= 0 and <= %d.' %(X, N)
+            'Invalid value X=%d; should be >= 0 and <= %d.' % (X, N)
         )
     if not (0 <= L <= N):
         raise ValueError(
-            'Invalid value L=%d; should be >= 0 and <= %d.' %(L, N)
+            'Invalid value L=%d; should be >= 0 and <= %d.' % (L, N)
         )
     if pval_thresh is not None and not (0.0 <= pval_thresh <= 1.0):
         raise ValueError(
             'Invalid value pval_thresh=%.1e; should be in [0,1).' % pval_thresh
         )
     if escore_pval_thresh is not None and \
             not (0.0 <= escore_pval_thresh <= 1.0):
         raise ValueError(
             'Invalid value escore_pval_thersh=%.1e; should be in [0,1).'
-                % escore_pval_thresh
+            % escore_pval_thresh
         )
     if not (0.0 <= tol < 1.0):
         raise ValueError('Invalid value tol=%.1e; should be in [0,1).' % tol)
 
     ### check if combination of argument values is valid
     if exact_pval not in ['always', 'if_significant', 'if_necessary']:
         raise ValueError('Invalid value exact_pval="%s".'
                          'Must be "always", "if_necessary", '
                          'or "if_significant".')
 
     if exact_pval in ['if_necessary', 'if_significant'] and \
-                    pval_thresh is None:
+            pval_thresh is None:
         raise ValueError('Missing argument: exact_pval=%s requires '
                          'a significance level to be specified (pval_thresh).')
 
     if escore_pval_thresh is not None and pval_thresh is None:
         raise ValueError('Missing argument: Setting escore_pval_thresh '
                          'requires a significance level to be specified'
                          '(pval_thresh).')
@@ -192,20 +190,20 @@
                            escore_pval_thresh=escore_pval_thresh)
         return result
 
     # If an array for the dynamic programming table is supplied, make sure it's
     # large enough. Otherwise, create an empty array.
     W = N - K
     if table is None:
-        table = np.empty((K+1, W+1), dtype = np.longdouble)
-    elif table.shape[0] < K+1 or table.shape[1] < W+1:
+        table = np.empty((K + 1, W + 1), dtype=np.longdouble)
+    elif table.shape[0] < K + 1 or table.shape[1] < W + 1:
         raise ValueError('Supplied array for dynamic programming table not'
                          'large enough. It is: %d x %d, but must be at least '
                          '%d x %d ((K+1) x (W+1)).'
-                         % (table.shape[0], table.shape[1], K+1, W+1))
+                         % (table.shape[0], table.shape[1], K + 1, W + 1))
 
     ### Step 1: Calculate XL-mHG test statistic.
     from xlmhglite import mhg
 
     stat, cutoff = mhg.get_xlmhg_stat(indices, N, K, X, L, tol)
     assert 0.0 <= stat <= 1.0
 
@@ -259,15 +257,15 @@
 
         else:
             # O(1)-bound was inconclusive
             # => calculate O(N)-bound
             ON_upper_bound = mhg_cython.get_xlmhg_ON_bound(N, K, X, L, stat,
                                                            tol)
             if ON_upper_bound <= pval_thresh or \
-                mhg.is_equal(ON_upper_bound, pval_thresh, tol):
+                    mhg.is_equal(ON_upper_bound, pval_thresh, tol):
                 # The upper bound is "<=" the significance threshold.
                 # This means that the test *is* significant.
                 # => Depending on the value of `exact_pval`, we report either
                 #    the upper bound or the exact p-value (see Step 3).
                 pval = ON_upper_bound
                 pval_is_significant = True
 
@@ -292,18 +290,17 @@
         if not use_alg1:
             # use PVAL2 algorithm
             pval = mhg_cython.get_xlmhg_pval2(N, K, X, L, stat, table, tol)
         else:
             # use PVAL1 algorithm
             pval = mhg_cython.get_xlmhg_pval1(N, K, X, L, stat, table, tol)
 
-
     if isnan(pval) or pval <= 0 or \
             (pval > O1_upper_bound and
-                 (not mhg.is_equal(pval, O1_upper_bound, tol))):
+             (not mhg.is_equal(pval, O1_upper_bound, tol))):
         # insufficient floating point precision for calculating p-value,
         # report O(1)-bound instead
         logger.warning('Insufficient floating point precision for calculating '
                        'the exact XL-mHG p-value. Using upper bound instead.')
         pval = O1_upper_bound
 
     # generate result object
@@ -340,18 +337,15 @@
     cutoff: int
         The (first) cutoff at which stat was attained.
         (0 if no cutoff was tested.)
     pval: float
         The XL-mHG p-value (either exact or an upper bound).
     """
     assert isinstance(v, np.ndarray) and v.ndim == 1 \
-        and np.issubdtype(v.dtype, np.integer)
+           and np.issubdtype(v.dtype, np.integer)
     if v.size > 65536:
         raise ValueError('List is too long. The maximum length supported is '
                          ' 65536.')
     indices = np.uint16(np.nonzero(v)[0])
     N = v.size
     result = get_xlmhg_test_result(N, indices, X, L, table=table)
     return result.stat, result.cutoff, result.pval
-
-
-
```

### Comparing `xlmhglite-1.0.1/xlmhglite/visualize.py` & `xlmhglite-1.1.0/xlmhglite/visualize.py`

 * *Files identical despite different names*

### Comparing `xlmhglite-1.0.1/xlmhglite.egg-info/PKG-INFO` & `xlmhglite-1.1.0/xlmhglite.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlmhglite
-Version: 1.0.1
+Version: 1.1.0
 Summary: XL-mHG lite: A light implementation of the Semiparametric Enrichment Test
 Home-page: https://github.com/GuyTeichman/xlmhglite
 Author: Guy Teichman
 Author-email: guyteichman@gmail.com
 License: GPLv3
 Keywords: statistics,nonparametric,semiparametric,enrichment test,ranked lists
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,16 +14,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.8
-Provides-Extra: plotly
-Provides-Extra: visualize
+Description-Content-Type: text/x-rst
 Provides-Extra: all
 License-File: LICENSE
 
 XL-mHG Lite
 =============
 
 
@@ -76,18 +75,18 @@
 
 - ``stat``: The XL-mHG test statistic
 - ``cutoff``: The cutoff at which XL-mHG test statistic was attained
 - ``pval``: The XL-mHG p-value
 
 __ user_manual_
 
-Documentation
--------------
+XL-mHG Lite Documentation
+---------------------------
 
-Please refer to the `XL-mHG User Manual`__ (hosted on ReadTheDocs).
+Please refer to the `XL-mHG User Manual`__.
 
 __ user_manual_
 
 Citing XL-mHG
 -------------
 
 If you use the XL-mHG test in your research, please cite `Eden et al. (PLoS
@@ -154,18 +153,33 @@
     :target: https://pypi.python.org/pypi/xlmhglite
     :alt: Python versions supported
 
 ..  |githubactions| image:: https://github.com/guyteichman/xlmhglite/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/GuyTeichman/xlmhglite/actions/workflows/tests.yml
     :alt: Build status
 
-=======
+
 History
 =======
 
+1.1.0 (2023-06-11)
+------------------
+This version improves clarity of warning messages and addresses some additional bugs.
+Moreover, the project has been transitioned to use pyproject.toml and setup.cfg, and old code was cleaned up for better maintainability.
+
+Changed
+********
+* Warning messages regarding failed import of the cython module were made more informative.
+* Transitioned the project to use pyproject.toml and setup.cfg, and cleaned up legacy code from setup.py.
+
+Fixed
+******
+* Fixed bug where calculating enrichment scores using the pure Python implementation would raise an AttributeError.
+* Fixed bug where the pure Python implementation would raise an ImportError if numba is not already installed on the system.
+
 1.0.1 (2023-06-11)
 ------------------
 Minor patch addressing installation issues.
 
 1.0.0 (2023-06-10)
 ------------------
 First stable release.
```

### Comparing `xlmhglite-1.0.1/xlmhglite.egg-info/SOURCES.txt` & `xlmhglite-1.1.0/xlmhglite.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
+requirements_dev.txt
+setup.cfg
 setup.py
 ./HISTORY.rst
 ./README.rst
-./requirements.txt
 ./requirements_dev.txt
-./requirements_extra.txt
 ./docs/build/_images/test_figure.png
 ./docs/build/_static/file.png
 ./docs/build/_static/minus.png
 ./docs/build/_static/plus.png
 ./docs/build/_static/test_figure.png
 ./docs/source/api.rst
 ./docs/source/background.rst
@@ -18,14 +20,15 @@
 ./docs/source/examples.rst
 ./docs/source/history.rst
 ./docs/source/index.rst
 ./docs/source/install.rst
 ./docs/source/license.rst
 ./docs/source/readme.rst
 ./docs/source/_static/test_figure.png
+./xlmhglite/mhg_cython.pyx
 docs/Makefile
 docs/make.bat
 docs/build/_images/test_figure.png
 docs/build/_static/file.png
 docs/build/_static/minus.png
 docs/build/_static/plus.png
 docs/build/_static/test_figure.png
```

