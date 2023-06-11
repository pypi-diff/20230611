# Comparing `tmp/taskiq_aiohttp-0.1.3.tar.gz` & `tmp/taskiq_aiohttp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aiohttp-0.1.3.tar", max compression
+gzip compressed data, was "taskiq_aiohttp-0.2.0.tar", max compression
```

## Comparing `taskiq_aiohttp-0.1.3.tar` & `taskiq_aiohttp-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-19 00:42:43.563116 taskiq_aiohttp-0.1.3/LICENSE
--rw-r--r--   0        0        0     2780 2023-05-19 00:42:43.563116 taskiq_aiohttp-0.1.3/README.md
--rw-r--r--   0        0        0     1716 2023-05-19 00:42:43.567116 taskiq_aiohttp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      144 2023-05-19 00:42:43.567116 taskiq_aiohttp-0.1.3/taskiq_aiohttp/__init__.py
--rw-r--r--   0        0        0     4469 2023-05-19 00:42:43.567116 taskiq_aiohttp-0.1.3/taskiq_aiohttp/initializer.py
--rw-r--r--   0        0        0        0 2023-05-19 00:42:43.567116 taskiq_aiohttp-0.1.3/taskiq_aiohttp/py.typed
--rw-r--r--   0        0        0     4098 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2780 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/README.md
+-rw-r--r--   0        0        0     1713 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/taskiq_aiohttp/__init__.py
+-rw-r--r--   0        0        0     4469 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/taskiq_aiohttp/initializer.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:34:07.793958 taskiq_aiohttp-0.2.0/taskiq_aiohttp/py.typed
+-rw-r--r--   0        0        0     3803 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.2.0/PKG-INFO
```

### Comparing `taskiq_aiohttp-0.1.3/LICENSE` & `taskiq_aiohttp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.1.3/README.md` & `taskiq_aiohttp-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.1.3/pyproject.toml` & `taskiq_aiohttp-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [tool.poetry]
 name = "taskiq-aiohttp"
 description = "Taskiq integration with AioHTTP framework"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.3"
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
 packages = [{ include = "taskiq_aiohttp" }]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskiq = "^0"
 aiohttp = "^3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
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
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 anyio = "^3.6.1"
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
 black = "^23.1.0"
```

### Comparing `taskiq_aiohttp-0.1.3/taskiq_aiohttp/initializer.py` & `taskiq_aiohttp-0.2.0/taskiq_aiohttp/initializer.py`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.1.3/PKG-INFO` & `taskiq_aiohttp-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 Metadata-Version: 2.1
 Name: taskiq-aiohttp
-Version: 0.1.3
+Version: 0.2.0
 Summary: Taskiq integration with AioHTTP framework
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
 Requires-Dist: aiohttp (>=3,<4)
 Requires-Dist: taskiq (>=0,<1)
 Description-Content-Type: text/markdown
 
 # Taskiq + AioHTTP
```

