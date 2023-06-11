# Comparing `tmp/taskiq_aiogram-0.1.0.tar.gz` & `tmp/taskiq_aiogram-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aiogram-0.1.0.tar", max compression
+gzip compressed data, was "taskiq_aiogram-0.2.0.tar", max compression
```

## Comparing `taskiq_aiogram-0.1.0.tar` & `taskiq_aiogram-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-13 23:52:29.041664 taskiq_aiogram-0.1.0/LICENSE
--rw-r--r--   0        0        0     3187 2023-05-13 23:52:29.041664 taskiq_aiogram-0.1.0/README.md
--rw-r--r--   0        0        0     1550 2023-05-13 23:52:29.041664 taskiq_aiogram-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      150 2023-05-13 23:52:29.041664 taskiq_aiogram-0.1.0/taskiq_aiogram/__init__.py
--rw-r--r--   0        0        0     3011 2023-05-13 23:52:29.041664 taskiq_aiogram-0.1.0/taskiq_aiogram/initializer.py
--rw-r--r--   0        0        0        0 2023-05-13 23:52:29.041664 taskiq_aiogram-0.1.0/taskiq_aiogram/py.typed
--rw-r--r--   0        0        0     4495 1970-01-01 00:00:00.000000 taskiq_aiogram-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-11 13:32:07.460091 taskiq_aiogram-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3181 2023-06-11 13:32:07.460091 taskiq_aiogram-0.2.0/README.md
+-rw-r--r--   0        0        0     1547 2023-06-11 13:32:07.464091 taskiq_aiogram-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-11 13:32:07.464091 taskiq_aiogram-0.2.0/taskiq_aiogram/__init__.py
+-rw-r--r--   0        0        0     3011 2023-06-11 13:32:07.464091 taskiq_aiogram-0.2.0/taskiq_aiogram/initializer.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:32:07.464091 taskiq_aiogram-0.2.0/taskiq_aiogram/py.typed
+-rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 taskiq_aiogram-0.2.0/PKG-INFO
```

### Comparing `taskiq_aiogram-0.1.0/LICENSE` & `taskiq_aiogram-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aiogram-0.1.0/README.md` & `taskiq_aiogram-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Taskiq + Aiogram
 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/taskiqtaskiq-aiogram?style=for-the-badge)](https://pypi.org/project/taskiq-aiogram/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/taskiq-aiogram?style=for-the-badge)](https://pypi.org/project/taskiq-aiogram/)
 [![PyPI](https://img.shields.io/pypi/v/taskiq-aiogram?style=for-the-badge)](https://pypi.org/project/taskiq-aiogram/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/taskiq-aiogram?style=for-the-badge)](https://pypistats.org/packages/taskiq-aiogram)
 
 This repo adds integration between your aiogram application and taskiq.
 
 It runs all startup and shutdown events of your application and adds 3 dependencies,
 that you can use in your tasks.
```

### Comparing `taskiq_aiogram-0.1.0/pyproject.toml` & `taskiq_aiogram-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 [tool.poetry]
 name = "taskiq-aiogram"
 description = "Taskiq integration with Aiogram"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.0"
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
 keywords = ["taskiq", "tasks", "distributed", "async"]
 packages = [{ include = "taskiq_aiogram" }]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskiq = "^0"
 aiogram = "^2"
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^4.0.1"
+flake8 = "^6"
 isort = "^5.10.1"
 mypy = "^1"
 pre-commit = "^2.20.0"
 yesqa = "^1.3.0"
 autoflake = "^1.4"
-wemake-python-styleguide = "^0.16.1"
+wemake-python-styleguide = "^0.18"
 types-mock = "^4.0.15"
 black = "^23.1.0"
 
 [tool.mypy]
 strict = true
 ignore_missing_imports = true
 allow_subclassing_any = true
```

### Comparing `taskiq_aiogram-0.1.0/taskiq_aiogram/initializer.py` & `taskiq_aiogram-0.2.0/taskiq_aiogram/initializer.py`

 * *Files identical despite different names*

### Comparing `taskiq_aiogram-0.1.0/PKG-INFO` & `taskiq_aiogram-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 Metadata-Version: 2.1
 Name: taskiq-aiogram
-Version: 0.1.0
+Version: 0.2.0
 Summary: Taskiq integration with Aiogram
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
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
 Requires-Dist: aiogram (>=2,<3)
 Requires-Dist: taskiq (>=0,<1)
 Description-Content-Type: text/markdown
 
 # Taskiq + Aiogram
 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/taskiqtaskiq-aiogram?style=for-the-badge)](https://pypi.org/project/taskiq-aiogram/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/taskiq-aiogram?style=for-the-badge)](https://pypi.org/project/taskiq-aiogram/)
 [![PyPI](https://img.shields.io/pypi/v/taskiq-aiogram?style=for-the-badge)](https://pypi.org/project/taskiq-aiogram/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/taskiq-aiogram?style=for-the-badge)](https://pypistats.org/packages/taskiq-aiogram)
 
 This repo adds integration between your aiogram application and taskiq.
 
 It runs all startup and shutdown events of your application and adds 3 dependencies,
 that you can use in your tasks.
```

