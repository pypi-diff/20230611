# Comparing `tmp/aiohttp_deps-0.1.4.tar.gz` & `tmp/aiohttp_deps-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_deps-0.1.4.tar", max compression
+gzip compressed data, was "aiohttp_deps-0.2.0.tar", max compression
```

## Comparing `aiohttp_deps-0.1.4.tar` & `aiohttp_deps-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-05-04 00:28:39.646442 aiohttp_deps-0.1.4/LICENSE
--rw-r--r--   0        0        0     7669 2023-05-04 00:28:39.646442 aiohttp_deps-0.1.4/README.md
--rw-r--r--   0        0        0      497 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/__init__.py
--rw-r--r--   0        0        0     3202 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/initializer.py
--rw-r--r--   0        0        0        0 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/py.typed
--rw-r--r--   0        0        0     1250 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/router.py
--rw-r--r--   0        0        0      898 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/router.pyi
--rw-r--r--   0        0        0     9364 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/swagger.py
--rw-r--r--   0        0        0     9138 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/utils.py
--rw-r--r--   0        0        0     1317 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/view.py
--rw-r--r--   0        0        0     1766 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9076 1970-01-01 00:00:00.000000 aiohttp_deps-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7669 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/README.md
+-rw-r--r--   0        0        0      497 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/__init__.py
+-rw-r--r--   0        0        0     3202 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/initializer.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/py.typed
+-rw-r--r--   0        0        0     1250 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/router.py
+-rw-r--r--   0        0        0      898 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/router.pyi
+-rw-r--r--   0        0        0     9363 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/swagger.py
+-rw-r--r--   0        0        0     9138 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/utils.py
+-rw-r--r--   0        0        0     1317 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/aiohttp_deps/view.py
+-rw-r--r--   0        0        0     1763 2023-06-11 13:29:52.959211 aiohttp_deps-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8781 1970-01-01 00:00:00.000000 aiohttp_deps-0.2.0/PKG-INFO
```

### Comparing `aiohttp_deps-0.1.4/LICENSE` & `aiohttp_deps-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.4/README.md` & `aiohttp_deps-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.4/aiohttp_deps/initializer.py` & `aiohttp_deps-0.2.0/aiohttp_deps/initializer.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.4/aiohttp_deps/router.py` & `aiohttp_deps-0.2.0/aiohttp_deps/router.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.4/aiohttp_deps/router.pyi` & `aiohttp_deps-0.2.0/aiohttp_deps/router.pyi`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.4/aiohttp_deps/swagger.py` & `aiohttp_deps-0.2.0/aiohttp_deps/swagger.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,11 +273,10 @@
 
     :param additional_schema: dict with updates.
     :return: same function with new attributes.
     """
 
     def decorator(func: Any) -> Any:
         func.__extra_openapi__ = additional_schema
-
         return func
 
     return decorator
```

### Comparing `aiohttp_deps-0.1.4/aiohttp_deps/utils.py` & `aiohttp_deps-0.2.0/aiohttp_deps/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.4/aiohttp_deps/view.py` & `aiohttp_deps-0.2.0/aiohttp_deps/view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.4/pyproject.toml` & `aiohttp_deps-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 [tool.poetry]
 name = "aiohttp-deps"
 description = "Dependency injection for AioHTTP"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.4"
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
 keywords = ["aiohttp", "taskiq-dependencies"]
 homepage = "https://github.com/taskiq-python/aiohttp-deps"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 aiohttp = "^3"
 taskiq-dependencies = "^1"
 pydantic = "^1"
 
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

### Comparing `aiohttp_deps-0.1.4/PKG-INFO` & `aiohttp_deps-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 Metadata-Version: 2.1
 Name: aiohttp-deps
-Version: 0.1.4
+Version: 0.2.0
 Summary: Dependency injection for AioHTTP
 Home-page: https://github.com/taskiq-python/aiohttp-deps
 License: LICENSE
 Keywords: aiohttp,taskiq-dependencies
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
 Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: taskiq-dependencies (>=1,<2)
 Description-Content-Type: text/markdown
```

