# Comparing `tmp/gaohn-common-utils-0.0.35.tar.gz` & `tmp/gaohn-common-utils-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.35.tar", last modified: Sat Jun 10 09:13:31 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.36.tar", last modified: Sun Jun 11 08:09:10 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.35.tar` & `gaohn-common-utils-0.0.36.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.297543 gaohn-common-utils-0.0.35/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.297543 gaohn-common-utils-0.0.35/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.919264 gaohn-common-utils-0.0.36/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.919264 gaohn-common-utils-0.0.36/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.35/LICENSE` & `gaohn-common-utils-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/PKG-INFO` & `gaohn-common-utils-0.0.36/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.35
+Version: 0.0.36
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.35/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.36/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.36/common_utils/core/artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     format="%(asctime)s [%(levelname)s]: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     handlers=[RichHandler()],
 )
 
 logger = logging.getLogger("rich")
 
-
 def get_git_commit_hash(working_dir: Optional[str] = None) -> str:
     """
     Get the current Git commit hash.
 
     If Git is not installed or the working directory is not a Git repository,
     the function returns "N/A".
```

### Comparing `gaohn-common-utils-0.0.35/common_utils/core/common.py` & `gaohn-common-utils-0.0.36/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.36/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.36/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/common_utils/core/logger.py` & `gaohn-common-utils-0.0.36/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.36/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.35
+Version: 0.0.36
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.35/pyproject.toml` & `gaohn-common-utils-0.0.36/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.35"
+version = "0.0.36"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -40,14 +40,17 @@
 [project.urls]
 "Homepage" = "https://github.com/gao-hongnan/common-utils"
 "Bug Tracker" = "https://github.com/gao-hongnan/common-utils/issues"
 
 [tool.black]
 line-length = 88
 target-version = ['py37', 'py38', 'py39']
+verbose = false
+diff = false
+color = false
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs                      # exclude a few common directories in the
   | \.git                       # root of the project
   | \.hg
   | \.mypy_cache
@@ -62,14 +65,15 @@
   | dist
 )/
 '''
 
 [tool.isort]
 profile = "black"
 line_length = 88
+verbose = false
 skip = [
     ".eggs",
     ".git",
     ".hg",
     ".mypy_cache",
     ".tox",
     "venv_*",
@@ -110,8 +114,9 @@
     [tool.pylint.'MESSAGES CONTROL']
     disable = [
         "access-member-before-definition",
         "attribute-defined-outside-init",
         "duplicate-code",
         "logging-fstring-interpolation",
         "no-member",
+        "missing-module-docstring",
     ]
```

