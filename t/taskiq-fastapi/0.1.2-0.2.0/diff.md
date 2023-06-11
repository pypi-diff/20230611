# Comparing `tmp/taskiq_fastapi-0.1.2.tar.gz` & `tmp/taskiq_fastapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_fastapi-0.1.2.tar", max compression
+gzip compressed data, was "taskiq_fastapi-0.2.0.tar", max compression
```

## Comparing `taskiq_fastapi-0.1.2.tar` & `taskiq_fastapi-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-05-11 21:11:59.963935 taskiq_fastapi-0.1.2/LICENSE
--rw-r--r--   0        0        0     4034 2023-05-11 21:11:59.963935 taskiq_fastapi-0.1.2/README.md
--rw-r--r--   0        0        0     1568 2023-05-11 21:11:59.967935 taskiq_fastapi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-11 21:11:59.967935 taskiq_fastapi-0.1.2/taskiq_fastapi/__init__.py
--rw-r--r--   0        0        0     2646 2023-05-11 21:11:59.967935 taskiq_fastapi-0.1.2/taskiq_fastapi/initializator.py
--rw-r--r--   0        0        0     5344 1970-01-01 00:00:00.000000 taskiq_fastapi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4034 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/README.md
+-rw-r--r--   0        0        0     1565 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/taskiq_fastapi/__init__.py
+-rw-r--r--   0        0        0     2646 2023-06-11 13:20:21.216347 taskiq_fastapi-0.2.0/taskiq_fastapi/initializator.py
+-rw-r--r--   0        0        0     5049 1970-01-01 00:00:00.000000 taskiq_fastapi-0.2.0/PKG-INFO
```

### Comparing `taskiq_fastapi-0.1.2/LICENSE` & `taskiq_fastapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_fastapi-0.1.2/README.md` & `taskiq_fastapi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_fastapi-0.1.2/pyproject.toml` & `taskiq_fastapi-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 [tool.poetry]
 name = "taskiq-fastapi"
 description = "FastAPI integration for taskiq"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.2"
+version = "0.2.0"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: System :: Networking",
     "Development Status :: 3 - Alpha",
 ]
 keywords = ["taskiq", "tasks", "distributed", "async", "fastapi"]
 packages = [{ include = "taskiq_fastapi" }]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskiq = "^0,>=0.3.1"
 fastapi = "*"
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^4.0.1"
+flake8 = "^6"
 isort = "^5.10.1"
 mypy = "^0.971"
 pre-commit = "^2.20.0"
 yesqa = "^1.3.0"
 autoflake = "^1.4"
-wemake-python-styleguide = "^0.16.1"
+wemake-python-styleguide = "^0.18"
 coverage = "^6.4.2"
 black = "^23.1.0"
 
 [tool.mypy]
 strict = true
 ignore_missing_imports = true
 allow_subclassing_any = true
```

### Comparing `taskiq_fastapi-0.1.2/taskiq_fastapi/initializator.py` & `taskiq_fastapi-0.2.0/taskiq_fastapi/initializator.py`

 * *Files identical despite different names*

### Comparing `taskiq_fastapi-0.1.2/PKG-INFO` & `taskiq_fastapi-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 Metadata-Version: 2.1
 Name: taskiq-fastapi
-Version: 0.1.2
+Version: 0.2.0
 Summary: FastAPI integration for taskiq
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async,fastapi
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
 Maintainer-email: taskiq@no-reply.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
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
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Dist: fastapi
 Requires-Dist: taskiq (>=0.3.1,<1)
 Description-Content-Type: text/markdown
 
 # Taskiq + FastAPI
```

