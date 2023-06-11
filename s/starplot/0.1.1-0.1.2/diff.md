# Comparing `tmp/starplot-0.1.1.tar.gz` & `tmp/starplot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starplot-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starplot-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starplot-0.1.1.tar` & `starplot-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      608 2023-06-11 19:04:16.904060 starplot-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      531 2023-06-11 19:04:16.904060 starplot-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1891 2023-06-11 19:04:16.904060 starplot-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2023-06-11 19:04:16.904060 starplot-0.1.1/LICENSE
--rw-r--r--   0        0        0      731 2023-06-11 19:04:16.904060 starplot-0.1.1/Makefile
--rw-r--r--   0        0        0     1203 2023-06-11 19:04:16.904060 starplot-0.1.1/README.md
--rw-r--r--   0        0        0      648 2023-06-11 19:04:16.904060 starplot-0.1.1/example.py
--rw-r--r--   0        0        0   708681 2023-06-11 19:04:16.912060 starplot-0.1.1/examples/starchart-blue.png
--rw-r--r--   0        0        0   664967 2023-06-11 19:04:16.916061 starplot-0.1.1/examples/starchart-chalk.png
--rw-r--r--   0        0        0   681737 2023-06-11 19:04:16.924060 starplot-0.1.1/examples/starchart-mono.png
--rw-r--r--   0        0        0   600936 2023-06-11 19:04:16.928061 starplot-0.1.1/examples/starchart-red.png
--rw-r--r--   0        0        0      673 2023-06-11 19:04:16.928061 starplot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       84 2023-06-11 19:04:16.928061 starplot-0.1.1/requirements-dev.txt
--rw-r--r--   0        0        0      130 2023-06-11 19:04:16.928061 starplot-0.1.1/requirements.txt
--rw-r--r--   0        0        0       50 2023-06-11 19:04:16.928061 starplot-0.1.1/src/starplot/__init__.py
--rw-r--r--   0        0        0     5743 2023-06-11 19:04:16.928061 starplot-0.1.1/src/starplot/charts.py
--rw-r--r--   0        0        0     4557 2023-06-11 19:04:16.928061 starplot-0.1.1/src/starplot/constellations.py
--rw-r--r--   0        0        0     3678 2023-06-11 19:04:16.928061 starplot-0.1.1/src/starplot/stars.py
--rw-r--r--   0        0        0     2421 2023-06-11 19:04:16.928061 starplot-0.1.1/src/starplot/styles.py
--rw-r--r--   0        0        0      188 2023-06-11 19:04:16.928061 starplot-0.1.1/src/starplot/utils.py
--rw-r--r--   0        0        0        0 2023-06-11 19:04:16.928061 starplot-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      134 2023-06-11 19:04:16.928061 starplot-0.1.1/tests/test_constellations.py
--rw-r--r--   0        0        0     1012 2023-06-11 19:04:16.928061 starplot-0.1.1/tests/test_styles.py
--rw-r--r--   0        0        0      286 2023-06-11 19:04:16.928061 starplot-0.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 starplot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      629 2023-06-11 20:11:35.440452 starplot-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      531 2023-06-11 20:11:35.440452 starplot-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1891 2023-06-11 20:11:35.440452 starplot-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2023-06-11 20:11:35.440452 starplot-0.1.2/LICENSE
+-rw-r--r--   0        0        0      731 2023-06-11 20:11:35.440452 starplot-0.1.2/Makefile
+-rw-r--r--   0        0        0     2286 2023-06-11 20:11:35.440452 starplot-0.1.2/README.md
+-rw-r--r--   0        0        0      648 2023-06-11 20:11:35.440452 starplot-0.1.2/example.py
+-rw-r--r--   0        0        0   708681 2023-06-11 20:11:35.444452 starplot-0.1.2/examples/starchart-blue.png
+-rw-r--r--   0        0        0   664967 2023-06-11 20:11:35.448452 starplot-0.1.2/examples/starchart-chalk.png
+-rw-r--r--   0        0        0   681737 2023-06-11 20:11:35.456452 starplot-0.1.2/examples/starchart-mono.png
+-rw-r--r--   0        0        0   600936 2023-06-11 20:11:35.460452 starplot-0.1.2/examples/starchart-red.png
+-rw-r--r--   0        0        0      910 2023-06-11 20:11:35.460452 starplot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-11 20:11:35.460452 starplot-0.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0       94 2023-06-11 20:11:35.460452 starplot-0.1.2/requirements.txt
+-rw-r--r--   0        0        0       50 2023-06-11 20:11:35.460452 starplot-0.1.2/src/starplot/__init__.py
+-rw-r--r--   0        0        0     5743 2023-06-11 20:11:35.460452 starplot-0.1.2/src/starplot/charts.py
+-rw-r--r--   0        0        0     4557 2023-06-11 20:11:35.460452 starplot-0.1.2/src/starplot/constellations.py
+-rw-r--r--   0        0        0     3678 2023-06-11 20:11:35.460452 starplot-0.1.2/src/starplot/stars.py
+-rw-r--r--   0        0        0     2421 2023-06-11 20:11:35.460452 starplot-0.1.2/src/starplot/styles.py
+-rw-r--r--   0        0        0      188 2023-06-11 20:11:35.460452 starplot-0.1.2/src/starplot/utils.py
+-rw-r--r--   0        0        0        0 2023-06-11 20:11:35.460452 starplot-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-11 20:11:35.460452 starplot-0.1.2/tests/test_constellations.py
+-rw-r--r--   0        0        0     1012 2023-06-11 20:11:35.460452 starplot-0.1.2/tests/test_styles.py
+-rw-r--r--   0        0        0      286 2023-06-11 20:11:35.460452 starplot-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 starplot-0.1.2/PKG-INFO
```

### Comparing `starplot-0.1.1/.github/workflows/test.yml` & `starplot-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/.gitignore` & `starplot-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/LICENSE` & `starplot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/Makefile` & `starplot-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/example.py` & `starplot-0.1.2/example.py`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/examples/starchart-blue.png` & `starplot-0.1.2/examples/starchart-blue.png`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/examples/starchart-chalk.png` & `starplot-0.1.2/examples/starchart-chalk.png`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/examples/starchart-mono.png` & `starplot-0.1.2/examples/starchart-mono.png`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/examples/starchart-red.png` & `starplot-0.1.2/examples/starchart-red.png`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/src/starplot/charts.py` & `starplot-0.1.2/src/starplot/charts.py`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/src/starplot/constellations.py` & `starplot-0.1.2/src/starplot/constellations.py`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/src/starplot/stars.py` & `starplot-0.1.2/src/starplot/stars.py`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/src/starplot/styles.py` & `starplot-0.1.2/src/starplot/styles.py`

 * *Files identical despite different names*

### Comparing `starplot-0.1.1/tests/test_styles.py` & `starplot-0.1.2/tests/test_styles.py`

 * *Files identical despite different names*

