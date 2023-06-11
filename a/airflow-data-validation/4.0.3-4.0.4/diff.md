# Comparing `tmp/airflow-data-validation-4.0.3.tar.gz` & `tmp/airflow-data-validation-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-data-validation-4.0.3.tar", max compression
+gzip compressed data, was "airflow-data-validation-4.0.4.tar", max compression
```

## Comparing `airflow-data-validation-4.0.3.tar` & `airflow-data-validation-4.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.3/airflow_data_validation/__init__.py
--rw-r--r--   0        0        0     9467 2023-06-11 13:32:57.418396 airflow-data-validation-4.0.3/airflow_data_validation/data_validation.py
--rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.3/airflow_data_validation/setup.py
--rw-r--r--   0        0        0      604 2023-06-11 13:31:39.159595 airflow-data-validation-4.0.3/pyproject.toml
--rw-r--r--   0        0        0      711 2023-06-11 13:34:05.196623 airflow-data-validation-4.0.3/setup.py
--rw-r--r--   0        0        0      695 2023-06-11 13:34:05.196824 airflow-data-validation-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.4/airflow_data_validation/__init__.py
+-rw-r--r--   0        0        0     9467 2023-06-11 13:32:57.418396 airflow-data-validation-4.0.4/airflow_data_validation/data_validation.py
+-rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.4/airflow_data_validation/setup.py
+-rw-r--r--   0        0        0      603 2023-06-11 13:42:15.352955 airflow-data-validation-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-06-11 13:42:24.314680 airflow-data-validation-4.0.4/setup.py
+-rw-r--r--   0        0        0      694 2023-06-11 13:42:24.314934 airflow-data-validation-4.0.4/PKG-INFO
```

### Comparing `airflow-data-validation-4.0.3/airflow_data_validation/data_validation.py` & `airflow-data-validation-4.0.4/airflow_data_validation/data_validation.py`

 * *Files identical despite different names*

### Comparing `airflow-data-validation-4.0.3/pyproject.toml` & `airflow-data-validation-4.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "airflow-data-validation"
-version = "4.0.3"
+version = "4.0.4"
 description = ""
 authors = ["sapir.krespil <sapir.krespil@guesty.com>"]
 readme = "README.md"
 homepage = "https://github.com/guestyorg/airflow_data_validation"
 repository = "https://github.com/guestyorg/airflow_data_validation"
 packages = [{include = "airflow_data_validation"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 google-cloud-bigquery = "^2.4.0"
-requests = "^2.31.0"
+requests = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>=61.1.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
```

### Comparing `airflow-data-validation-4.0.3/setup.py` & `airflow-data-validation-4.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['airflow_data_validation']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['google-cloud-bigquery>=2.4.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
+['google-cloud-bigquery>=2.4.0,<3.0.0', 'requests>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'airflow-data-validation',
-    'version': '4.0.3',
+    'version': '4.0.4',
     'description': '',
     'long_description': '',
     'author': 'sapir.krespil',
     'author_email': 'sapir.krespil@guesty.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/guestyorg/airflow_data_validation',
```

### Comparing `airflow-data-validation-4.0.3/PKG-INFO` & `airflow-data-validation-4.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: airflow-data-validation
-Version: 4.0.3
+Version: 4.0.4
 Summary: 
 Home-page: https://github.com/guestyorg/airflow_data_validation
 Author: sapir.krespil
 Author-email: sapir.krespil@guesty.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: google-cloud-bigquery (>=2.4.0,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/guestyorg/airflow_data_validation
 Description-Content-Type: text/markdown
```

