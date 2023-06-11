# Comparing `tmp/gaohn-common-utils-0.0.36.tar.gz` & `tmp/gaohn-common-utils-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.36.tar", last modified: Sun Jun 11 08:09:10 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.37.tar", last modified: Sun Jun 11 09:32:36 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.36.tar` & `gaohn-common-utils-0.0.37.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.919264 gaohn-common-utils-0.0.36/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.919264 gaohn-common-utils-0.0.36/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 08:09:10.000000 gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-11 08:08:43.000000 gaohn-common-utils-0.0.36/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 08:09:10.923264 gaohn-common-utils-0.0.36/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.301037 gaohn-common-utils-0.0.37/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.301037 gaohn-common-utils-0.0.37/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.36/LICENSE` & `gaohn-common-utils-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/PKG-INFO` & `gaohn-common-utils-0.0.37/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.36
+Version: 0.0.37
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.36/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.37/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.37/common_utils/core/artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     format="%(asctime)s [%(levelname)s]: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     handlers=[RichHandler()],
 )
 
 logger = logging.getLogger("rich")
 
+
 def get_git_commit_hash(working_dir: Optional[str] = None) -> str:
     """
     Get the current Git commit hash.
 
     If Git is not installed or the working directory is not a Git repository,
     the function returns "N/A".
```

### Comparing `gaohn-common-utils-0.0.36/common_utils/core/common.py` & `gaohn-common-utils-0.0.37/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.37/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.37/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/common_utils/core/logger.py` & `gaohn-common-utils-0.0.37/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.37/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.36
+Version: 0.0.37
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.36/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.36/pyproject.toml` & `gaohn-common-utils-0.0.37/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.36"
+version = "0.0.37"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -31,15 +31,23 @@
     "pydantic==1.10.8",
     "google-cloud-bigquery==3.10.0",
     "google-cloud-storage==2.8.0",
     "python-dotenv==1.0.0",
 ]
 
 [project.optional-dependencies]
-dev = ["black==23.3.0", "pylint==2.17.4", "pytest==6.2.5", "mypy==1.3.0", "isort==5.12.0"]
+dev = [
+    "black==23.3.0",
+    "pylint==2.17.4",
+    "pytest==6.2.5",
+    "mypy==1.3.0",
+    "isort==5.12.0",
+    "bandit==1.7.5",
+    "toml==0.10.2",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/gao-hongnan/common-utils"
 "Bug Tracker" = "https://github.com/gao-hongnan/common-utils/issues"
 
 [tool.black]
 line-length = 88
@@ -116,7 +124,30 @@
         "access-member-before-definition",
         "attribute-defined-outside-init",
         "duplicate-code",
         "logging-fstring-interpolation",
         "no-member",
         "missing-module-docstring",
     ]
+
+# https://bandit.readthedocs.io/en/latest/config.html
+[tool.bandit]
+exclude_dirs = [
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".tox",
+    "venv_*",
+    "venv",
+    ".venv",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+]
+
+# https://mypy.readthedocs.io/en/stable/config_file.html
+[tool.mypy]
+ignore_missing_imports = true
+disallow_untyped_defs = true
+disable_error_code = ['override', 'attr-defined']
```

