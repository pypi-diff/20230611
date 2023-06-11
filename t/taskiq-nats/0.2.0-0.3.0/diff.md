# Comparing `tmp/taskiq_nats-0.2.0.tar.gz` & `tmp/taskiq_nats-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_nats-0.2.0.tar", max compression
+gzip compressed data, was "taskiq_nats-0.3.0.tar", max compression
```

## Comparing `taskiq_nats-0.2.0.tar` & `taskiq_nats-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1293 2023-04-09 23:53:49.566584 taskiq_nats-0.2.0/README.md
--rw-r--r--   0        0        0     1453 2023-04-09 23:53:49.566584 taskiq_nats-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      171 2023-04-09 23:53:49.566584 taskiq_nats-0.2.0/taskiq_nats/__init__.py
--rw-r--r--   0        0        0     2261 2023-04-09 23:53:49.566584 taskiq_nats-0.2.0/taskiq_nats/broker.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 taskiq_nats-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1292 2023-06-11 13:15:38.501666 taskiq_nats-0.3.0/README.md
+-rw-r--r--   0        0        0     1452 2023-06-11 13:15:38.501666 taskiq_nats-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-06-11 13:15:38.501666 taskiq_nats-0.3.0/taskiq_nats/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-11 13:15:38.501666 taskiq_nats-0.3.0/taskiq_nats/broker.py
+-rw-r--r--   0        0        0     2117 1970-01-01 00:00:00.000000 taskiq_nats-0.3.0/PKG-INFO
```

### Comparing `taskiq_nats-0.2.0/README.md` & `taskiq_nats-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Taskiq-nats is a plugin for taskiq that adds NATS broker.
 
 ## Installation
 
 To use this project you must have installed core taskiq library:
 
 ```bash
-pip install taskiq taskiq-redis
+pip install taskiq taskiq-nats
 ```
 
 ## Usage
 
 Here's a minimal setup example with a broker and one task.
 
 ```python
```

### Comparing `taskiq_nats-0.2.0/pyproject.toml` & `taskiq_nats-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 [tool.poetry]
 name = "taskiq-nats"
-version = "0.2.0"
+version = "0.3.0"
 description = "NATS integration for taskiq"
 authors = ["taskiq-team <taskiq@norely.com>"]
 readme = "README.md"
 packages = [{ include = "taskiq_nats" }]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 homepage = "https://github.com/taskiq-python/taskiq-nats"
 repository = "https://github.com/taskiq-python/taskiq-nats"
 keywords = ["taskiq", "tasks", "distributed", "async", "nats", "result_backend"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 nats-py = "^2.2.0"
 taskiq = "^0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pre-commit = "^2.20.0"
 mypy = "^1.1.1"
-flake8 = "^4.0.0"
-wemake-python-styleguide = "^0.17.0"
+flake8 = "^6"
 autoflake = "^1.4"
 yesqa = "^1.4.0"
 pytest = "^7.2.2"
 pytest-xdist = "^3.2.1"
 anyio = "^3.6.2"
 pytest-cov = "^4.0.0"
+wemake-python-styleguide = "^0.18.0"
 
 
 [tool.mypy]
 strict = true
 ignore_missing_imports = true
 allow_subclassing_any = true
 allow_untyped_calls = true
```

### Comparing `taskiq_nats-0.2.0/taskiq_nats/broker.py` & `taskiq_nats-0.3.0/taskiq_nats/broker.py`

 * *Files identical despite different names*

### Comparing `taskiq_nats-0.2.0/PKG-INFO` & `taskiq_nats-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 Metadata-Version: 2.1
 Name: taskiq-nats
-Version: 0.2.0
+Version: 0.3.0
 Summary: NATS integration for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-nats
 Keywords: taskiq,tasks,distributed,async,nats,result_backend
 Author: taskiq-team
 Author-email: taskiq@norely.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: nats-py (>=2.2.0,<3.0.0)
 Requires-Dist: taskiq (>=0,<1)
 Project-URL: Repository, https://github.com/taskiq-python/taskiq-nats
 Description-Content-Type: text/markdown
 
 # Taskiq NATS
 
 Taskiq-nats is a plugin for taskiq that adds NATS broker.
 
 ## Installation
 
 To use this project you must have installed core taskiq library:
 
 ```bash
-pip install taskiq taskiq-redis
+pip install taskiq taskiq-nats
 ```
 
 ## Usage
 
 Here's a minimal setup example with a broker and one task.
 
 ```python
```

