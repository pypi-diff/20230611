# Comparing `tmp/hapless-0.2.0.tar.gz` & `tmp/hapless-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hapless-0.2.0.tar", max compression
+gzip compressed data, was "hapless-0.2.1.tar", max compression
```

## Comparing `hapless-0.2.0.tar` & `hapless-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     2543 2022-11-05 12:41:27.129292 hapless-0.2.0/README.md
--rw-r--r--   0        0        0        0 2022-04-19 07:56:57.295450 hapless-0.2.0/hapless/__init__.py
--rw-r--r--   0        0        0     4424 2022-11-05 11:49:13.993984 hapless-0.2.0/hapless/cli.py
--rw-r--r--   0        0        0      479 2022-11-07 11:37:01.668111 hapless-0.2.0/hapless/config.py
--rw-r--r--   0        0        0     5895 2022-11-07 11:37:01.668925 hapless-0.2.0/hapless/hap.py
--rw-r--r--   0        0        0    11257 2022-11-16 17:10:25.386768 hapless-0.2.0/hapless/main.py
--rw-r--r--   0        0        0     2093 2022-11-16 19:59:08.115269 hapless-0.2.0/hapless/utils.py
--rw-r--r--   0        0        0     1563 2022-11-17 17:09:52.914512 hapless-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 hapless-0.2.0/setup.py
--rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 hapless-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2476 2023-06-11 12:05:03.143518 hapless-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2022-04-19 07:56:57.295450 hapless-0.2.1/hapless/__init__.py
+-rw-r--r--   0        0        0     4424 2022-11-05 11:49:13.993984 hapless-0.2.1/hapless/cli.py
+-rw-r--r--   0        0        0      479 2022-11-07 11:37:01.668111 hapless-0.2.1/hapless/config.py
+-rw-r--r--   0        0        0     5895 2022-11-07 11:37:01.668925 hapless-0.2.1/hapless/hap.py
+-rw-r--r--   0        0        0    11257 2022-11-16 17:10:25.386768 hapless-0.2.1/hapless/main.py
+-rw-r--r--   0        0        0     2093 2022-11-16 19:59:08.115269 hapless-0.2.1/hapless/utils.py
+-rw-r--r--   0        0        0     1632 2023-06-11 12:12:17.225141 hapless-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 hapless-0.2.1/PKG-INFO
```

### Comparing `hapless-0.2.0/README.md` & `hapless-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ## hapless
 
 ![Checks](https://github.com/bmwant/hapless/actions/workflows/tests.yml/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/hapless)](https://pypi.org/project/hapless/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hapless)
+
+
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![EditorConfig](https://img.shields.io/badge/-EditorConfig-grey?logo=editorconfig)](https://editorconfig.org/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 > **hapless** (*adjective*) - (especially of a person) unfortunate. A developer who accidentally launched long-running process in the foreground.
 
 Simplest way of running and tracking processes in the background.
 
@@ -54,14 +57,10 @@
 
 ### See also
 
 * [Rich](https://rich.readthedocs.io/en/stable/introduction.html) console UI library.
 * [Supervisor](http://supervisord.org/) full-fledged process manager.
 * [podmena](https://github.com/bmwant/podmena) provides nice emoji icons to commit messages.
 
-### Support project, support 🇺🇦 Ukraine!
-
-🐶 `D7DA74qzZUyh9cctCxWovPTEovUSjGzL2S` this is [Dogecoin](https://dogecoin.com/) wallet to support the project.
-
-🇺🇦 All donations will go towards supporting Ukraine in the war.
+### Support 🇺🇦 Ukraine in the war!
 
-✉️ [Contact author](mailto:bmwant@gmail.com) directly in case you want to donate with some different payment option or check what has already been done.
+🇺🇦 Donate to [this foundation](https://prytulafoundation.org/en) in case you want to help. Every donation matter!
```

### Comparing `hapless-0.2.0/hapless/cli.py` & `hapless-0.2.1/hapless/cli.py`

 * *Files identical despite different names*

### Comparing `hapless-0.2.0/hapless/hap.py` & `hapless-0.2.1/hapless/hap.py`

 * *Files identical despite different names*

### Comparing `hapless-0.2.0/hapless/main.py` & `hapless-0.2.1/hapless/main.py`

 * *Files identical despite different names*

### Comparing `hapless-0.2.0/hapless/utils.py` & `hapless-0.2.1/hapless/utils.py`

 * *Files identical despite different names*

### Comparing `hapless-0.2.0/pyproject.toml` & `hapless-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hapless"
-version = "0.2.0"
+version = "0.2.1"
 description = "Run and track processes in background"
 authors = ["Misha Behersky <bmwant@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bmwant/hapless"
 keywords = ["cli", "job", "runner", "background", "process"]
 classifiers = [
@@ -34,26 +34,27 @@
 importlib-metadata = { version = "^4.11.3", python = "<3.8" }
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
 pytest = "^7.1.1"
 isort = "^5.10.1"
 pytest-cov = "^3.0.0"
+ruff = "^0.0.272"
 
 [tool.poetry.group.ci]
 optional = true
 
 [tool.poetry.group.ci.dependencies]
 github3-py = "^3.2.0"
 
 [tool.poetry.scripts]
 hap = 'hapless.cli:cli'
 
 [tool.poetry.urls]
-"Blog post" = "https://bmwlog.pp.ua/"
+"Blog post" = "https://bmwlog.pp.ua/hapless-easily-run-and-manage-background-processes/"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
```

### Comparing `hapless-0.2.0/PKG-INFO` & `hapless-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapless
-Version: 0.2.0
+Version: 0.2.1
 Summary: Run and track processes in background
 Home-page: https://github.com/bmwant/hapless
 License: MIT
 Keywords: cli,job,runner,background,process
 Author: Misha Behersky
 Author-email: bmwant@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -15,39 +15,36 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: System
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: humanize (>=4.0.0,<5.0.0)
-Requires-Dist: importlib-metadata (>=4.11.3,<5.0.0); python_version < "3.8"
+Requires-Dist: importlib-metadata (>=4.11.3,<5.0.0) ; python_version < "3.8"
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: rich (>=12.2.0,<13.0.0)
-Project-URL: Blog post, https://bmwlog.pp.ua/
+Project-URL: Blog post, https://bmwlog.pp.ua/hapless-easily-run-and-manage-background-processes/
 Project-URL: Repository, https://github.com/bmwant/hapless
 Description-Content-Type: text/markdown
 
 ## hapless
 
 ![Checks](https://github.com/bmwant/hapless/actions/workflows/tests.yml/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/hapless)](https://pypi.org/project/hapless/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hapless)
+
+
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![EditorConfig](https://img.shields.io/badge/-EditorConfig-grey?logo=editorconfig)](https://editorconfig.org/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 > **hapless** (*adjective*) - (especially of a person) unfortunate. A developer who accidentally launched long-running process in the foreground.
 
 Simplest way of running and tracking processes in the background.
 
@@ -94,15 +91,11 @@
 
 ### See also
 
 * [Rich](https://rich.readthedocs.io/en/stable/introduction.html) console UI library.
 * [Supervisor](http://supervisord.org/) full-fledged process manager.
 * [podmena](https://github.com/bmwant/podmena) provides nice emoji icons to commit messages.
 
-### Support project, support 🇺🇦 Ukraine!
-
-🐶 `D7DA74qzZUyh9cctCxWovPTEovUSjGzL2S` this is [Dogecoin](https://dogecoin.com/) wallet to support the project.
-
-🇺🇦 All donations will go towards supporting Ukraine in the war.
+### Support 🇺🇦 Ukraine in the war!
 
-✉️ [Contact author](mailto:bmwant@gmail.com) directly in case you want to donate with some different payment option or check what has already been done.
+🇺🇦 Donate to [this foundation](https://prytulafoundation.org/en) in case you want to help. Every donation matter!
```

