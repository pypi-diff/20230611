# Comparing `tmp/tox_gh-1.0.0.tar.gz` & `tmp/tox_gh-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox_gh-1.0.0.tar", last modified: Fri Jan 13 16:09:23 2023, max compression
+gzip compressed data, was "tox_gh-1.1.0.tar", last modified: Sun Jun 11 14:28:04 2023, max compression
```

## Comparing `tox_gh-1.0.0.tar` & `tox_gh-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:09:23.179715 tox_gh-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:09:23.175715 tox_gh-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-13 16:09:15.000000 tox_gh-1.0.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-13 16:09:15.000000 tox_gh-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:09:23.175715 tox_gh-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-01-13 16:09:15.000000 tox_gh-1.0.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-13 16:09:15.000000 tox_gh-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-13 16:09:15.000000 tox_gh-1.0.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-13 16:09:15.000000 tox_gh-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-13 16:09:15.000000 tox_gh-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-13 16:09:15.000000 tox_gh-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-01-13 16:09:23.179715 tox_gh-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-01-13 16:09:15.000000 tox_gh-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-01-13 16:09:15.000000 tox_gh-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-01-13 16:09:23.179715 tox_gh-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-13 16:09:15.000000 tox_gh-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:09:23.175715 tox_gh-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:09:23.175715 tox_gh-1.0.0/src/tox_gh/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-13 16:09:15.000000 tox_gh-1.0.0/src/tox_gh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-01-13 16:09:15.000000 tox_gh-1.0.0/src/tox_gh/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 16:09:15.000000 tox_gh-1.0.0/src/tox_gh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-13 16:09:23.000000 tox_gh-1.0.0/src/tox_gh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:09:23.179715 tox_gh-1.0.0/src/tox_gh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-01-13 16:09:23.000000 tox_gh-1.0.0/src/tox_gh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-13 16:09:23.000000 tox_gh-1.0.0/src/tox_gh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 16:09:23.000000 tox_gh-1.0.0/src/tox_gh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-13 16:09:23.000000 tox_gh-1.0.0/src/tox_gh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-13 16:09:23.000000 tox_gh-1.0.0/src/tox_gh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-13 16:09:23.000000 tox_gh-1.0.0/src/tox_gh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 16:09:22.000000 tox_gh-1.0.0/src/tox_gh.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 16:09:23.179715 tox_gh-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-13 16:09:15.000000 tox_gh-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-01-13 16:09:15.000000 tox_gh-1.0.0/tests/test_tox_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-13 16:09:15.000000 tox_gh-1.0.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-01-13 16:09:15.000000 tox_gh-1.0.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-13 16:09:15.000000 tox_gh-1.0.0/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.723596 tox_gh-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.719596 tox_gh-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.719596 tox_gh-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 14:27:57.000000 tox_gh-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-11 14:27:57.000000 tox_gh-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-11 14:28:04.723596 tox_gh-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-11 14:27:57.000000 tox_gh-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-11 14:27:57.000000 tox_gh-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-11 14:28:04.723596 tox_gh-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-11 14:27:57.000000 tox_gh-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.719596 tox_gh-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.719596 tox_gh-1.1.0/src/tox_gh/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-11 14:27:57.000000 tox_gh-1.1.0/src/tox_gh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-11 14:27:57.000000 tox_gh-1.1.0/src/tox_gh/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 14:27:57.000000 tox_gh-1.1.0/src/tox_gh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.723596 tox_gh-1.1.0/src/tox_gh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.723596 tox_gh-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-11 14:27:57.000000 tox_gh-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-11 14:27:57.000000 tox_gh-1.1.0/tests/test_tox_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-11 14:27:57.000000 tox_gh-1.1.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-11 14:27:57.000000 tox_gh-1.1.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 14:27:57.000000 tox_gh-1.1.0/whitelist.txt
```

### Comparing `tox_gh-1.0.0/.github/workflows/check.yml` & `tox_gh-1.1.0/.github/workflows/check.yml`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   test:
     name: test with ${{ matrix.py }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         py:
+          - "3.12.0-beta.2"
           - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
         os:
           - ubuntu-22.04
@@ -69,29 +70,7 @@
       - name: Install tox
         run: python -m pip install tox
       - name: Setup test suite
         run: tox -vv --notest -e ${{ matrix.tox_env }}
       - name: Run test suite
         run: tox --skip-pkg-install -e ${{ matrix.tox_env }}
 
-  publish:
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-    needs: [check, test]
-    runs-on: ubuntu-22.04
-    steps:
-      - name: Setup python to build package
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.11"
-      - name: Install build
-        run: python -m pip install build
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Build sdist and wheel
-        run: python -m build -s -w . -o dist
-      - name: Publish to PyPi
-        uses: pypa/gh-action-pypi-publish@v1.6.4
-        with:
-          skip_existing: true
-          user: __token__
-          password: ${{ secrets.pypi_password }}
```

### Comparing `tox_gh-1.0.0/.pre-commit-config.yaml` & `tox_gh-1.1.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,45 +18,45 @@
         args: [--py36-plus]
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: ["--py37-plus"]
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: [--safe]
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==22.12]
+        additional_dependencies: [black==23.3]
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: "0.6.0"
+    rev: "1.3.0"
     hooks:
       - id: tox-ini-fmt
         args: ["-p", "fix"]
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
-          - flake8-bugbear==22.12.6
-          - flake8-comprehensions==3.10.1
-          - flake8-pytest-style==1.6
+          - flake8-bugbear==23.3.23
+          - flake8-comprehensions==3.12
+          - flake8-pytest-style==1.7.2
           - flake8-spellcheck==0.28
-          - flake8-unused-arguments==0.0.12
-          - flake8-noqa==1.3
+          - flake8-unused-arguments==0.0.13
+          - flake8-noqa==1.3.1
           - pep8-naming==0.13.3
-          - flake8-pyproject==1.2.2
+          - flake8-pyproject==1.2.3
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v2.7.1"
     hooks:
       - id: prettier
         additional_dependencies:
           - prettier@2.7.1
           - "@prettier/plugin-xml@2.2"
@@ -65,7 +65,11 @@
     rev: v0.33.0
     hooks:
       - id: markdownlint
   - repo: meta
     hooks:
       - id: check-hooks-apply
       - id: check-useless-excludes
+  - repo: https://github.com/tox-dev/pyproject-fmt
+    rev: "0.9.2"
+    hooks:
+      - id: pyproject-fmt
```

### Comparing `tox_gh-1.0.0/LICENSE` & `tox_gh-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox_gh-1.0.0/PKG-INFO` & `tox_gh-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox_gh
-Version: 1.0.0
+Version: 1.1.0
 Summary: Seamless integration of tox into GitHub Actions
 Home-page: https://github.com/tox-dev/tox-gh
 Author: Bernat Gabor
 Author-email: gaborjbernatv@gmail.com
 Maintainer: Bernat Gabor
 Maintainer-email: gaborjbernat@gmail.com
 License: MIT
@@ -94,15 +94,15 @@
       fail-fast: false
       matrix:
         os:
           - Ubuntu
           - Windows
           - MacOs
         py:
-          - "3.10.0-rc.1"
+          - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
           - "3.6"
     steps:
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v2
```

### Comparing `tox_gh-1.0.0/README.md` & `tox_gh-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
       fail-fast: false
       matrix:
         os:
           - Ubuntu
           - Windows
           - MacOs
         py:
-          - "3.10.0-rc.1"
+          - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
           - "3.6"
     steps:
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v2
```

### Comparing `tox_gh-1.0.0/pyproject.toml` & `tox_gh-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
-requires = ["setuptools>=65.7", "setuptools-scm>=7.1"]
 build-backend = 'setuptools.build_meta'
+requires = [
+  "setuptools>=67.6.1",
+  "setuptools-scm>=7.1",
+]
+
+[tool.setuptools_scm]
+write_to = "src/tox_gh/version.py"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 line_length = 120
 profile = "black"
 known_first_party = ["tox_gh"]
 
-[tool.setuptools_scm]
-write_to = "src/tox_gh/version.py"
+[tool.flake8]
+max-complexity = 22
+max-line-length = 120
+unused-arguments-ignore-abstract-functions = true
+noqa-require-code = true
+dictionaries = ["en_US", "python", "technical", "django"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.mypy]
 python_version = "3.9"
 strict = true
-
-[tool.flake8]
-max-complexity = 22
-max-line-length = 120
-unused-arguments-ignore-abstract-functions = true
-noqa-require-code = true
-dictionaries = ["en_US", "python", "technical", "django"]
```

### Comparing `tox_gh-1.0.0/setup.cfg` & `tox_gh-1.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	Source=https://github.com/tox-dev/tox-gh
 	Tracker=https://github.com/tox-dev/tox-gh/issues
 	Changelog=https://github.com/tox-dev/tox-gh/blob/main/CHANGELOG.md
 
 [options]
 packages = find:
 install_requires = 
-	tox>=4.2.8
+	tox>=4.4.12
 python_requires = >=3.7
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = True
 
 [options.packages.find]
@@ -45,17 +45,17 @@
 
 [options.entry_points]
 tox = 
 	tox-gh = tox_gh.plugin
 
 [options.extras_require]
 test = 
-	covdefaults>=2.2.2
+	covdefaults>=2.3
 	devpi-process>=0.3
-	pytest>=7.2
+	pytest>=7.3.1
 	pytest-cov>=4
 	pytest-mock>=3.10
 
 [options.package_data]
 tox_gh = py.typed
 
 [egg_info]
```

### Comparing `tox_gh-1.0.0/src/tox_gh/plugin.py` & `tox_gh-1.1.0/src/tox_gh/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 import logging
 import os
+import pathlib
 import shutil
 import sys
 from typing import Dict
 
 from tox.config.loader.memory import MemoryLoader
 from tox.config.loader.section import Section
 from tox.config.sets import ConfigSet
 from tox.config.types import EnvList
 from tox.execute import Outcome
 from tox.plugin import impl
 from tox.session.state import State
 from tox.tox_env.api import ToxEnv
 from virtualenv.discovery.py_info import PythonInfo  # type: ignore # no types defined
 
+GITHUB_STEP_SUMMARY = os.getenv("GITHUB_STEP_SUMMARY")
+
 
 def is_running_on_actions() -> bool:
     """:return: True if running on Github Actions platform"""
     # https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables
     return os.environ.get("GITHUB_ACTIONS") == "true"
 
 
@@ -71,7 +74,18 @@
         print(f"::group::tox:{tox_env.name}")
 
 
 @impl
 def tox_after_run_commands(tox_env: ToxEnv, exit_code: int, outcomes: list[Outcome]) -> None:  # noqa: U100
     if tox_env.core["is_on_gh_action"]:
         print("::endgroup::")
+        write_to_summary(exit_code == Outcome.OK, tox_env.name)
+
+
+def write_to_summary(success: bool, message: str) -> None:
+    """Write a success or failure value to the github step summary if it exists"""
+    if not GITHUB_STEP_SUMMARY:
+        return
+    summary_path = pathlib.Path(GITHUB_STEP_SUMMARY)
+    success_str = ":white_check_mark:" if success else ":negative_squared_cross_mark:"
+    with summary_path.open("a+") as summary_file:
+        print(f"{success_str}: {message}", file=summary_file)
```

### Comparing `tox_gh-1.0.0/src/tox_gh.egg-info/PKG-INFO` & `tox_gh-1.1.0/src/tox_gh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-gh
-Version: 1.0.0
+Version: 1.1.0
 Summary: Seamless integration of tox into GitHub Actions
 Home-page: https://github.com/tox-dev/tox-gh
 Author: Bernat Gabor
 Author-email: gaborjbernatv@gmail.com
 Maintainer: Bernat Gabor
 Maintainer-email: gaborjbernat@gmail.com
 License: MIT
@@ -94,15 +94,15 @@
       fail-fast: false
       matrix:
         os:
           - Ubuntu
           - Windows
           - MacOs
         py:
-          - "3.10.0-rc.1"
+          - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
           - "3.6"
     steps:
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v2
```

### Comparing `tox_gh-1.0.0/tox.ini` & `tox_gh-1.1.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
     py310
     py39
     py38
     py37
     type
     readme
-isolated_build = true
 skip_missing_interpreters = true
-minversion = 4.0.0b2
 
 [testenv]
 description = run the unit tests with pytest under {basepython}
-setenv =
-    COVERAGE_FILE = {toxworkdir}{/}.coverage.{envname}
+package = wheel
+wheel_build_env = .pkg
 extras =
     test
+set_env =
+    COVERAGE_FILE = {toxworkdir}{/}.coverage.{envname}
 commands =
     pytest {tty:--color=yes} {posargs: \
       --cov {envsitepackagesdir}{/}tox_gh --cov {toxinidir}{/}tests --cov-fail-under=95 --cov-context=test \
       --no-cov-on-fail  --cov-config {toxinidir}{/}setup.cfg \
       --cov-report term-missing:skip-covered  --junitxml {toxworkdir}{/}junit.{envname}.xml \
       --cov-report html:{envtmpdir}{/}htmlcov \
       tests}
-package = wheel
-wheel_build_env = .pkg
 
 [testenv:fix]
 description = run static analysis and style check using flake8
-passenv =
-    HOMEPATH
-    PROGRAMDATA
 skip_install = true
 deps =
-    pre-commit>=2.21
+    pre-commit>=3.2.2
+pass_env =
+    HOMEPATH
+    PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:type]
 description = run type check on code base
-setenv =
-    {tty:MYPY_FORCE_COLOR = 1}
 deps =
-    mypy==0.991
-    types-docutils>=0.19.1.1
+    mypy==1.2
+    types-docutils>=0.19.1.7
+set_env =
+    {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy src {posargs}
     mypy tests {posargs}
 
 [testenv:readme]
 description = check that the package metadata is correct
-setenv =
-    {tty:FORCE_COLOR = 1}
 skip_install = true
 deps =
     build[virtualenv]>=0.10
     twine>=4.0.2
-changedir = {toxinidir}
+set_env =
+    {tty:FORCE_COLOR = 1}
+change_dir = {toxinidir}
 commands =
     python -m build --sdist --wheel -o {envtmpdir} .
     twine check {envtmpdir}{/}*
 
 [testenv:dev]
 description = generate a DEV environment
-usedevelop = true
+package = editable
 extras =
     test
 commands =
     python -m pip list --format=columns
     python -c 'import sys; print(sys.executable)'
 
 [gh]
```

