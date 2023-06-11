# Comparing `tmp/redhat_qe_cloud_tools-1.0.5.tar.gz` & `tmp/redhat_qe_cloud_tools-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redhat_qe_cloud_tools-1.0.5.tar", max compression
+gzip compressed data, was "redhat_qe_cloud_tools-1.0.6.tar", max compression
```

## Comparing `redhat_qe_cloud_tools-1.0.5.tar` & `redhat_qe_cloud_tools-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/LICENSE
--rw-r--r--   0        0        0      845 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/__init__.py
--rw-r--r--   0        0        0      787 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/README.md
--rw-r--r--   0        0        0        0 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/__init__.py
--rw-r--r--   0        0        0     1893 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/aws_utils.py
--rw-r--r--   0        0        0     6218 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/delete_s3_velero_bucket.py
--rw-r--r--   0        0        0      455 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/roles/README.md
--rw-r--r--   0        0        0        0 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/roles/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/clouds/aws/roles/roles.py
--rw-r--r--   0        0        0      782 2023-05-28 09:47:44.322196 redhat_qe_cloud_tools-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/LICENSE
+-rw-r--r--   0        0        0      852 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/clouds/__init__.py
+-rw-r--r--   0        0        0      787 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/clouds/aws/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/clouds/aws/__init__.py
+-rw-r--r--   0        0        0     4066 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/aws_utils.py
+-rw-r--r--   0        0        0     4317 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/delete_s3_velero_bucket.py
+-rw-r--r--   0        0        0      455 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/roles/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/roles/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/roles/roles.py
+-rw-r--r--   0        0        0      554 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/session_clients.py
+-rw-r--r--   0        0        0     7789 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/utilities/delete_aws_resources.py
+-rw-r--r--   0        0        0      815 2023-06-11 14:32:12.060322 redhat_qe_cloud_tools-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.6/PKG-INFO
```

### Comparing `redhat_qe_cloud_tools-1.0.5/LICENSE` & `redhat_qe_cloud_tools-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.5/README.md` & `redhat_qe_cloud_tools-1.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Install [poetry](https://github.com/python-poetry/poetry)
 
 ```
 poetry install
 ```
 
 ## Docs
-- [AWS readme](aws/README.md)
+- [AWS Readme](clouds/aws/README.md)
 
 ## Release new version
 ### requirements:
 * Export GitHub token
 ```bash
 export GITHUB_TOKEN=<your_github_token>
 ```
```

### Comparing `redhat_qe_cloud_tools-1.0.5/clouds/aws/README.md` & `redhat_qe_cloud_tools-1.0.6/clouds/aws/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.5/clouds/aws/roles/roles.py` & `redhat_qe_cloud_tools-1.0.6/clouds/aws/roles/roles.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.5/pyproject.toml` & `redhat_qe_cloud_tools-1.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "redhat-qe-cloud-tools"
-version = "1.0.5"
+version = "1.0.6"
 description = "Python utilities to manage cloud services, such as AWS."
 authors = ["Meni Yakove", "Ruth Netser"]
 readme = "README.md"
 repository = "https://github.com/RedHatQE/cloud-tools"
 packages = [{include = "clouds"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 colorlog = "*"
 boto3 = "*"
 click = "*"
 configparser = "*"
 python-simple-logger="*"
+openshift-python-utilities = "*"
 
 [tool.poetry.dev-dependencies]
 ipython = "*"
 ipdb = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `redhat_qe_cloud_tools-1.0.5/PKG-INFO` & `redhat_qe_cloud_tools-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: redhat-qe-cloud-tools
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python utilities to manage cloud services, such as AWS.
 Home-page: https://github.com/RedHatQE/cloud-tools
 Author: Meni Yakove
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3
 Requires-Dist: click
 Requires-Dist: colorlog
 Requires-Dist: configparser
+Requires-Dist: openshift-python-utilities
 Requires-Dist: python-simple-logger
 Project-URL: Repository, https://github.com/RedHatQE/cloud-tools
 Description-Content-Type: text/markdown
 
 # cloud-tools
 Python utilities to manage cloud services, such as AWS.
 
@@ -32,15 +33,15 @@
 Install [poetry](https://github.com/python-poetry/poetry)
 
 ```
 poetry install
 ```
 
 ## Docs
-- [AWS readme](aws/README.md)
+- [AWS Readme](clouds/aws/README.md)
 
 ## Release new version
 ### requirements:
 * Export GitHub token
 ```bash
 export GITHUB_TOKEN=<your_github_token>
 ```
```

