# Comparing `tmp/pytest-pyodide-0.52.0.tar.gz` & `tmp/pytest-pyodide-0.52.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-pyodide-0.52.0.tar", last modified: Fri Jun  2 01:02:27 2023, max compression
+gzip compressed data, was "pytest-pyodide-0.52.1.tar", last modified: Sun Jun 11 02:13:01 2023, max compression
```

## Comparing `pytest-pyodide-0.52.0.tar` & `pytest-pyodide-0.52.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/workflows/filtermatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.github/workflows/testall.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/COMPATIBILITY.md
--rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9769 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/examples/test_install_package.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/examples/wheels/
--rw-r--r--   0 runner    (1001) docker     (122)    93002 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/pytest_pyodide/
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/_decorator_in_pyodide.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.243264 pytest-pyodide-0.52.0/pytest_pyodide/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/_templates/module_test.html
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/_templates/test.html
--rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/copy_files_to_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8300 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/fixture.py
--rw-r--r--   0 runner    (1001) docker     (122)     9186 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/node_test_driver.js
--rw-r--r--   0 runner    (1001) docker     (122)     5171 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/run_tests_inside_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)    16829 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/pytest_pyodide/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 01:02:27.000000 pytest-pyodide-0.52.0/pytest_pyodide.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 01:02:27.247264 pytest-pyodide-0.52.0/tests/datafiles/
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/datafiles/in_pyodide_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     9613 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_copy_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_jsassert.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_run_in_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-02 01:02:04.000000 pytest-pyodide-0.52.0/tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.190020 pytest-pyodide-0.52.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.186020 pytest-pyodide-0.52.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.github/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.186020 pytest-pyodide-0.52.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.github/workflows/filtermatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.github/workflows/testall.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/COMPATIBILITY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-06-11 02:13:01.190020 pytest-pyodide-0.52.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9769 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.186020 pytest-pyodide-0.52.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/examples/test_install_package.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.186020 pytest-pyodide-0.52.1/examples/wheels/
+-rw-r--r--   0 runner    (1001) docker     (122)    93002 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.186020 pytest-pyodide-0.52.1/pytest_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/_decorator_in_pyodide.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.186020 pytest-pyodide-0.52.1/pytest_pyodide/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/_templates/module_test.html
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/_templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/copy_files_to_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13591 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8300 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9186 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/node_test_driver.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5171 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/run_tests_inside_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16893 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/pytest_pyodide/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.186020 pytest-pyodide-0.52.1/pytest_pyodide.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-06-11 02:13:01.000000 pytest-pyodide-0.52.1/pytest_pyodide.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-06-11 02:13:01.000000 pytest-pyodide-0.52.1/pytest_pyodide.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-11 02:13:01.000000 pytest-pyodide-0.52.1/pytest_pyodide.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-11 02:13:01.000000 pytest-pyodide-0.52.1/pytest_pyodide.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-11 02:13:01.000000 pytest-pyodide-0.52.1/pytest_pyodide.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-11 02:13:01.000000 pytest-pyodide-0.52.1/pytest_pyodide.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-06-11 02:13:01.190020 pytest-pyodide-0.52.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.190020 pytest-pyodide-0.52.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 02:13:01.190020 pytest-pyodide-0.52.1/tests/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/datafiles/in_pyodide_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9613 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_copy_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_jsassert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_run_in_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-11 02:12:38.000000 pytest-pyodide-0.52.1/tests/test_testing.py
```

### Comparing `pytest-pyodide-0.52.0/.github/workflows/build.yaml` & `pytest-pyodide-0.52.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/.github/workflows/filtermatrix.py` & `pytest-pyodide-0.52.1/.github/workflows/filtermatrix.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/.github/workflows/main.yaml` & `pytest-pyodide-0.52.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/.github/workflows/testall.yaml` & `pytest-pyodide-0.52.1/.github/workflows/testall.yaml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/.pre-commit-config.yaml` & `pytest-pyodide-0.52.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/CHANGELOG.md` & `pytest-pyodide-0.52.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [0.52.1] - 2023-06-10
+
+- Removed use of `executable_path` from selenium driver construction to make
+  pytest-pyodide compatible with Selenium v4.10.
+  [#93](https://github.com/pyodide/pytest-pyodide/pull/93)
+
+
 ## [0.52.0] - 2023-06-01
 
 - Removed `JsException` unpickle special case. This was fixed by
   [pyodide/pyodide#3387](https://github.com/pyodide/pyodide/pull/3387).
   [#91](https://github.com/pyodide/pytest-pyodide/pull/91)
 
 - Dropped support for Pyodide version `0.21.x`.
```

### Comparing `pytest-pyodide-0.52.0/PKG-INFO` & `pytest-pyodide-0.52.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pyodide
-Version: 0.52.0
+Version: 0.52.1
 Summary: "Pytest plugin for testing applications that use Pyodide"
 Home-page: https://github.com/pyodide/pytest-pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pytest-pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pytest-pyodide-0.52.0/README.md` & `pytest-pyodide-0.52.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/examples/test_install_package.py` & `pytest-pyodide-0.52.1/examples/test_install_package.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl` & `pytest-pyodide-0.52.1/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pyproject.toml` & `pytest-pyodide-0.52.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/__init__.py` & `pytest-pyodide-0.52.1/pytest_pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/_decorator_in_pyodide.py` & `pytest-pyodide-0.52.1/pytest_pyodide/_decorator_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/_templates/module_test.html` & `pytest-pyodide-0.52.1/pytest_pyodide/_templates/module_test.html`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/_templates/test.html` & `pytest-pyodide-0.52.1/pytest_pyodide/_templates/test.html`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/copy_files_to_pyodide.py` & `pytest-pyodide-0.52.1/pytest_pyodide/copy_files_to_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/decorator.py` & `pytest-pyodide-0.52.1/pytest_pyodide/decorator.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/fixture.py` & `pytest-pyodide-0.52.1/pytest_pyodide/fixture.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/hook.py` & `pytest-pyodide-0.52.1/pytest_pyodide/hook.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/hypothesis.py` & `pytest-pyodide-0.52.1/pytest_pyodide/hypothesis.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/node_test_driver.js` & `pytest-pyodide-0.52.1/pytest_pyodide/node_test_driver.js`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/run_tests_inside_pyodide.py` & `pytest-pyodide-0.52.1/pytest_pyodide/run_tests_inside_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/runner.py` & `pytest-pyodide-0.52.1/pytest_pyodide/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -411,21 +411,22 @@
 
 class SeleniumFirefoxRunner(_SeleniumBaseRunner):
     browser = "firefox"
 
     def get_driver(self):
         from selenium.webdriver import Firefox
         from selenium.webdriver.firefox.options import Options
+        from selenium.webdriver.firefox.service import Service
 
         options = Options()
         options.add_argument("--headless")
         for flag in FIREFOX_FLAGS:
             options.add_argument(flag)
 
-        return Firefox(executable_path="geckodriver", options=options)
+        return Firefox(service=Service("geckodriver"), options=options)
 
 
 class SeleniumChromeRunner(_SeleniumBaseRunner):
     browser = "chrome"
 
     def get_driver(self):
         from selenium.webdriver import Chrome
```

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/server.py` & `pytest-pyodide-0.52.1/pytest_pyodide/server.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide/utils.py` & `pytest-pyodide-0.52.1/pytest_pyodide/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide.egg-info/PKG-INFO` & `pytest-pyodide-0.52.1/pytest_pyodide.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pyodide
-Version: 0.52.0
+Version: 0.52.1
 Summary: "Pytest plugin for testing applications that use Pyodide"
 Home-page: https://github.com/pyodide/pytest-pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pytest-pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pytest-pyodide-0.52.0/pytest_pyodide.egg-info/SOURCES.txt` & `pytest-pyodide-0.52.1/pytest_pyodide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/setup.cfg` & `pytest-pyodide-0.52.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/datafiles/in_pyodide_tests.py` & `pytest-pyodide-0.52.1/tests/datafiles/in_pyodide_tests.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl` & `pytest-pyodide-0.52.1/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/test_copy_files.py` & `pytest-pyodide-0.52.1/tests/test_copy_files.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/test_decorator.py` & `pytest-pyodide-0.52.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/test_jsassert.py` & `pytest-pyodide-0.52.1/tests/test_jsassert.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/test_options.py` & `pytest-pyodide-0.52.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/test_run_in_pyodide.py` & `pytest-pyodide-0.52.1/tests/test_run_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/test_server.py` & `pytest-pyodide-0.52.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.52.0/tests/test_testing.py` & `pytest-pyodide-0.52.1/tests/test_testing.py`

 * *Files identical despite different names*

