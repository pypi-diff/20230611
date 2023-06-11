# Comparing `tmp/taskiq_dependencies-1.2.4.tar.gz` & `tmp/taskiq_dependencies-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_dependencies-1.2.4.tar", max compression
+gzip compressed data, was "taskiq_dependencies-1.3.0.tar", max compression
```

## Comparing `taskiq_dependencies-1.2.4.tar` & `taskiq_dependencies-1.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6368 2023-05-21 21:34:19.764530 taskiq_dependencies-1.2.4/README.md
--rw-r--r--   0        0        0     1621 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/pyproject.toml
--rw-r--r--   0        0        0      386 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/__init__.py
--rw-r--r--   0        0        0    11773 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/ctx.py
--rw-r--r--   0        0        0     3273 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/dependency.py
--rw-r--r--   0        0        0     9626 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/graph.py
--rw-r--r--   0        0        0        0 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/py.typed
--rw-r--r--   0        0        0      573 2023-05-21 21:34:19.768530 taskiq_dependencies-1.2.4/taskiq_dependencies/utils.py
--rw-r--r--   0        0        0     7251 1970-01-01 00:00:00.000000 taskiq_dependencies-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6368 2023-06-11 13:36:41.851076 taskiq_dependencies-1.3.0/README.md
+-rw-r--r--   0        0        0     1618 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      386 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/__init__.py
+-rw-r--r--   0        0        0    11773 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/ctx.py
+-rw-r--r--   0        0        0     3273 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/dependency.py
+-rw-r--r--   0        0        0     9626 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/graph.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/py.typed
+-rw-r--r--   0        0        0      573 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/utils.py
+-rw-r--r--   0        0        0     7205 1970-01-01 00:00:00.000000 taskiq_dependencies-1.3.0/PKG-INFO
```

### Comparing `taskiq_dependencies-1.2.4/README.md` & `taskiq_dependencies-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.4/pyproject.toml` & `taskiq_dependencies-1.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "taskiq-dependencies"
-version = "1.2.4"
+version = "1.3.0"
 description = "FastAPI like dependency injection implementation"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 packages = [{include = "taskiq_dependencies"}]
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
 ]
 keywords = ["taskiq", "dependencies", "injection", "async", "DI"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 graphlib-backport = { version = "^1.0.3", python="<3.9" }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = { version = "^22.6.0", allow-prereleases = true }
-flake8 = "~4.0.1"
+flake8 = "~6"
 isort = "~5.10.1"
 mypy = "~0.971"
 pre-commit = "~2.20.0"
 yesqa = "~1.3.0"
 autoflake = "~1.4"
-wemake-python-styleguide = "~0.16.1"
+wemake-python-styleguide = "~0.18"
 coverage = "~6.4.2"
 pytest-cov = "~3.0.0"
 anyio = "~3.6.1"
 pytest-xdist = { version = "~2.5.0", extras = ["psutil"] }
 
 
 [tool.mypy]
```

### Comparing `taskiq_dependencies-1.2.4/taskiq_dependencies/ctx.py` & `taskiq_dependencies-1.3.0/taskiq_dependencies/ctx.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.4/taskiq_dependencies/dependency.py` & `taskiq_dependencies-1.3.0/taskiq_dependencies/dependency.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.4/taskiq_dependencies/graph.py` & `taskiq_dependencies-1.3.0/taskiq_dependencies/graph.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.4/taskiq_dependencies/utils.py` & `taskiq_dependencies-1.3.0/taskiq_dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.4/PKG-INFO` & `taskiq_dependencies-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: taskiq-dependencies
-Version: 1.2.4
+Version: 1.3.0
 Summary: FastAPI like dependency injection implementation
 Keywords: taskiq,dependencies,injection,async,DI
 Author: Pavel Kirilin
 Author-email: win10@list.ru
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Typing :: Typed
 Requires-Dist: graphlib-backport (>=1.0.3,<2.0.0) ; python_version < "3.9"
 Description-Content-Type: text/markdown
 
 # Taskiq dependencies
 
 This project is used to add FastAPI-like dependency injection to projects.
```

