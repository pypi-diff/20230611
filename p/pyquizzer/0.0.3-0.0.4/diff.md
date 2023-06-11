# Comparing `tmp/pyquizzer-0.0.3.tar.gz` & `tmp/pyquizzer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquizzer-0.0.3.tar", max compression
+gzip compressed data, was "pyquizzer-0.0.4.tar", max compression
```

## Comparing `pyquizzer-0.0.3.tar` & `pyquizzer-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0       11 2023-06-04 06:57:15.811368 pyquizzer-0.0.3/README.md
--rwxr-xr-x   0        0        0       35 2023-06-11 09:12:23.455506 pyquizzer-0.0.3/changelog.md
--rw-r--r--   0        0        0      883 2023-06-11 09:31:10.581154 pyquizzer-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-04 06:53:20.851812 pyquizzer-0.0.3/pyquizzer.py
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 pyquizzer-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0       11 2023-06-04 06:57:15.811368 pyquizzer-0.0.4/README.md
+-rwxr-xr-x   0        0        0       35 2023-06-11 09:12:23.455506 pyquizzer-0.0.4/changelog.md
+-rw-r--r--   0        0        0      894 2023-06-11 09:43:41.831118 pyquizzer-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-04 06:53:20.851812 pyquizzer-0.0.4/pyquizzer.py
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 pyquizzer-0.0.4/PKG-INFO
```

### Comparing `pyquizzer-0.0.3/pyproject.toml` & `pyquizzer-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "pyquizzer"
-version = "0.0.3"
+version = "0.0.4"
 description = "placeholder"
 authors = ["BjornFJohansson <bjornjobb@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/BjornFJohansson/pyquizzer"
 repository = "https://github.com/BjornFJohansson/pyquizzer"
-documentation = "https://readthedocs.org/"
+documentation = "https://readthedocs.org/1"
 include = ["changelog.md"]
 [tool.poetry.dependencies]
 python = "^3.11"
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -19,11 +19,11 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1"
 pytest-cov = "^4.0"
 
 [tool.poetry.urls]
 changelog = "https://github.com/BjornFJohansson/pyquizzer/blob/main/changelog.md"
-documentation = "https://readthedocs.org/"
+documentation = "https://readthedocs.org/2"
 bugtracker = "https://github.com/BjornFJohansson/pyquizzer/issues"
 coverage = "https://about.codecov.io/"
-youtube = "https://youtube.com"
+youtube = "https://youtu.be/C0DPdy98e4c"
```

### Comparing `pyquizzer-0.0.3/PKG-INFO` & `pyquizzer-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pyquizzer
-Version: 0.0.3
+Version: 0.0.4
 Summary: placeholder
 Home-page: https://github.com/BjornFJohansson/pyquizzer
 Author: BjornFJohansson
 Author-email: bjornjobb@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Documentation, https://readthedocs.org/
+Project-URL: Documentation, https://readthedocs.org/1
 Project-URL: Repository, https://github.com/BjornFJohansson/pyquizzer
 Project-URL: bugtracker, https://github.com/BjornFJohansson/pyquizzer/issues
 Project-URL: changelog, https://github.com/BjornFJohansson/pyquizzer/blob/main/changelog.md
 Project-URL: coverage, https://about.codecov.io/
-Project-URL: documentation, https://readthedocs.org/
-Project-URL: youtube, https://youtube.com
+Project-URL: documentation, https://readthedocs.org/2
+Project-URL: youtube, https://youtu.be/C0DPdy98e4c
 Description-Content-Type: text/markdown
 
 placeholder
```

