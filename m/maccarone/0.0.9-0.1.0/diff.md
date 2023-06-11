# Comparing `tmp/maccarone-0.0.9.tar.gz` & `tmp/maccarone-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maccarone-0.0.9.tar", last modified: Thu Jun  1 17:08:36 2023, max compression
+gzip compressed data, was "maccarone-0.1.0.tar", last modified: Sun Jun 11 00:08:16 2023, max compression
```

## Comparing `maccarone-0.0.9.tar` & `maccarone-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.682607 maccarone-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.678607 maccarone-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.678607 maccarone-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-01 17:08:05.000000 maccarone-0.0.9/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-01 17:08:05.000000 maccarone-0.0.9/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-01 17:08:05.000000 maccarone-0.0.9/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-01 17:08:05.000000 maccarone-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 17:08:05.000000 maccarone-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-01 17:08:36.682607 maccarone-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-01 17:08:05.000000 maccarone-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-01 17:08:05.000000 maccarone-0.0.9/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.682607 maccarone-0.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 17:08:05.000000 maccarone-0.0.9/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-01 17:08:05.000000 maccarone-0.0.9/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 17:08:05.000000 maccarone-0.0.9/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 17:08:05.000000 maccarone-0.0.9/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 17:08:05.000000 maccarone-0.0.9/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-01 17:08:05.000000 maccarone-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:08:36.682607 maccarone-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.678607 maccarone-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.682607 maccarone-0.0.9/src/maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-01 17:08:05.000000 maccarone-0.0.9/src/maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-01 17:08:05.000000 maccarone-0.0.9/src/maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-01 17:08:05.000000 maccarone-0.0.9/src/maccarone/loader.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-01 17:08:18.000000 maccarone-0.0.9/src/maccarone/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-01 17:08:05.000000 maccarone-0.0.9/src/maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-01 17:08:05.000000 maccarone-0.0.9/src/maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.682607 maccarone-0.0.9/src/maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-01 17:08:05.000000 maccarone-0.0.9/src/maccarone/scripts/preprocess.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-01 17:08:27.000000 maccarone-0.0.9/src/maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.682607 maccarone-0.0.9/src/maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-01 17:08:05.000000 maccarone-0.0.9/src/maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-01 17:08:05.000000 maccarone-0.0.9/src/maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.682607 maccarone-0.0.9/src/maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-01 17:08:36.000000 maccarone-0.0.9/src/maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-01 17:08:36.000000 maccarone-0.0.9/src/maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:08:36.000000 maccarone-0.0.9/src/maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 17:08:36.000000 maccarone-0.0.9/src/maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 17:08:36.000000 maccarone-0.0.9/src/maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 17:08:36.000000 maccarone-0.0.9/src/maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:08:36.682607 maccarone-0.0.9/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-01 17:08:05.000000 maccarone-0.0.9/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.676154 maccarone-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.668154 maccarone-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-11 00:07:48.000000 maccarone-0.1.0/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-11 00:07:48.000000 maccarone-0.1.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-11 00:07:48.000000 maccarone-0.1.0/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-11 00:07:48.000000 maccarone-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-11 00:07:48.000000 maccarone-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-11 00:08:16.676154 maccarone-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-11 00:07:48.000000 maccarone-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-11 00:07:48.000000 maccarone-0.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/add.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/file_sizes.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/file_sizes.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/fizzbuzz.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/todo.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 00:07:48.000000 maccarone-0.1.0/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-11 00:07:48.000000 maccarone-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 00:08:16.676154 maccarone-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.668154 maccarone-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/caching.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/caching.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-11 00:08:08.000000 maccarone-0.1.0/src/maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/loader.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/loader.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-11 00:08:08.000000 maccarone-0.1.0/src/maccarone/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/scripts/preprocess.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-11 00:08:08.000000 maccarone-0.1.0/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.676154 maccarone-0.1.0/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/src/maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.676154 maccarone-0.1.0/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-11 00:07:48.000000 maccarone-0.1.0/support/rename_to_stale.sh
```

### Comparing `maccarone-0.0.9/.github/workflows/publish-to-pypi-stale.yml` & `maccarone-0.1.0/.github/workflows/publish-to-pypi-stale.yml`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,16 @@
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - run: python -m pip install --upgrade pip
       - name: Preprocess with stale_maccarone
         run: |
-          pip install stale_maccarone
-          python -m stale_maccarone.scripts.preprocess src/maccarone
-          pip uninstall -y stale_maccarone
+          pip install -e .[dev]
+          stale_maccarone src/maccarone
         env:
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
       - name: Rename to `stale_maccarone`
         run: |
           support/rename_to_stale.sh
       - name: Build package
         run: |
```

### Comparing `maccarone-0.0.9/.github/workflows/publish-to-pypi.yml` & `maccarone-0.1.0/.github/workflows/publish-to-pypi.yml`

 * *Files 23% similar despite different names*

```diff
@@ -12,17 +12,16 @@
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - run: python -m pip install --upgrade pip
       - name: Preprocess with stale_maccarone
         run: |
-          pip install stale_maccarone
-          python -m stale_maccarone.scripts.preprocess src/maccarone
-          pip uninstall -y stale_maccarone
+          pip install -e .[dev]
+          stale_maccarone src/maccarone
         env:
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
       - name: Build package
         run: |
           pip install build
           python -m build
       - name: Publish package
```

### Comparing `maccarone-0.0.9/.github/workflows/run-pytest.yml` & `maccarone-0.1.0/.github/workflows/run-pytest.yml`

 * *Files 26% similar despite different names*

```diff
@@ -8,20 +8,18 @@
         python-version: ["3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - run: python -m pip install --upgrade pip
+      - name: Install package
+        run: |
+          pip install .[dev]
       - name: Preprocess with stale_maccarone
         run: |
-          pip install stale_maccarone
           stale_maccarone src/maccarone
-          pip uninstall -y stale_maccarone
         env:
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
-      - name: Install package
-        run: |
-          pip install .
       - name: Run pytest
         run: |
           pytest
```

### Comparing `maccarone-0.0.9/.gitignore` & `maccarone-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.9/LICENSE` & `maccarone-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.9/dev-requirements.txt` & `maccarone-0.1.0/dev-requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     #   stale-maccarone
 requests==2.30.0
     # via openai
 six==1.16.0
     # via asttokens
 stack-data==0.6.2
     # via ipython
-stale-maccarone==0.0.8
+stale-maccarone==0.0.12
     # via maccarone (pyproject.toml)
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
     #   pytest
 tqdm==4.65.0
```

### Comparing `maccarone-0.0.9/pyproject.toml` & `maccarone-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 "Homepage" = "https://github.com/bsilverthorn/maccarone"
 "Repository" = "https://github.com/bsilverthorn/maccarone"
 
 [project.optional-dependencies]
 dev = [
     "ipython",
     "pip-tools",
-    "stale_maccarone==0.0.8",
+    "stale_maccarone==0.0.12",
 ]
 
 [project.scripts]
 maccarone = "maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
```

### Comparing `maccarone-0.0.9/src/maccarone/loader.mn.py` & `maccarone-0.1.0/src/maccarone/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 from importlib.abc import (
     MetaPathFinder,
     SourceLoader,
 )
 from importlib.machinery import ModuleSpec
 from fnmatch import fnmatchcase
 
+from maccarone.openai import CachedChatAPI
 from maccarone.preprocessor import preprocess_maccarone
 
+SNIPPET_START = "#" + "<<"
+
 class ImportFinder(MetaPathFinder):
     def __init__(
             self,
             py_string_matching: bool,
             include_pattern: str | None,
             exclude_pattern: str | None,
         ) -> None:
@@ -41,43 +44,48 @@
                 is_package=False
             )
 
         if path is None or path == '':
             path = [os.getcwd()]  # top level import 
 
         for entry in path:
-            parts = fullname.split(".")
-            basename = parts[-1]
-            package_path = parts[1:-1]
-            base_filename = os.path.join(entry, *package_path, basename)
+            basename = fullname.split(".")[-1]
+            base_filename = os.path.join(entry, basename)
             py_filename = base_filename + '.py'
             mn_filename = base_filename + '.mn.py'
 
             if os.path.exists(mn_filename):
                 return make_modulespec(mn_filename)
             elif self.py_string_matching and os.path.exists(py_filename):
                 with open(py_filename, "rt") as file:
-                    if "#<<" in file.read():
+                    if SNIPPET_START in file.read():
                         return make_modulespec(py_filename)
 
         return None  # we don't know how to import this
 
+def py_path_to_cache_path(py_path):
+    return py_path.replace(".py", ".json")
+
+
 class ImportLoader(SourceLoader):
     def __init__(self, fullname, path):
         self.fullname = fullname
         self.path = path
 
     def get_filename(self, fullname):
         return self.path
 
     def get_data(self, filename):
         with open(self.path, 'r') as file:
             in_source = file.read()
 
-        return preprocess_maccarone(in_source)
+        cache_path = py_path_to_cache_path(self.path)
+        chat_api = CachedChatAPI(cache_path)
+
+        return preprocess_maccarone(in_source, chat_api)
 
 def enable(
         py_string_matching=True,
         include_pattern=None,
         exclude_pattern=None,
     ):
     """Exclude patterns take precedence over include patterns."""
```

### Comparing `maccarone-0.0.9/src/maccarone/loader.py` & `maccarone-0.1.0/src/maccarone/loader.mn.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 from importlib.abc import (
     MetaPathFinder,
     SourceLoader,
 )
 from importlib.machinery import ModuleSpec
 from fnmatch import fnmatchcase
 
+from maccarone.openai import CachedChatAPI
 from maccarone.preprocessor import preprocess_maccarone
 
+SNIPPET_START = "#" + "<<"
+
 class ImportFinder(MetaPathFinder):
     def __init__(
             self,
             py_string_matching: bool,
             include_pattern: str | None,
             exclude_pattern: str | None,
         ) -> None:
@@ -41,43 +44,47 @@
                 is_package=False
             )
 
         if path is None or path == '':
             path = [os.getcwd()]  # top level import 
 
         for entry in path:
-            parts = fullname.split(".")
-            basename = parts[-1]
-            package_path = parts[1:-1]
-            base_filename = os.path.join(entry, *package_path, basename)
+            basename = fullname.split(".")[-1]
+            base_filename = os.path.join(entry, basename)
             py_filename = base_filename + '.py'
             mn_filename = base_filename + '.mn.py'
 
             if os.path.exists(mn_filename):
                 return make_modulespec(mn_filename)
             elif self.py_string_matching and os.path.exists(py_filename):
                 with open(py_filename, "rt") as file:
-                    if "#<<" in file.read():
+                    if SNIPPET_START in file.read():
                         return make_modulespec(py_filename)
 
         return None  # we don't know how to import this
 
+def py_path_to_cache_path(py_path):
+    #<<replace regex: r"\.py$" -> ".json">>
+
 class ImportLoader(SourceLoader):
     def __init__(self, fullname, path):
         self.fullname = fullname
         self.path = path
 
     def get_filename(self, fullname):
         return self.path
 
     def get_data(self, filename):
         with open(self.path, 'r') as file:
             in_source = file.read()
 
-        return preprocess_maccarone(in_source)
+        cache_path = py_path_to_cache_path(self.path)
+        chat_api = CachedChatAPI(cache_path)
+
+        return preprocess_maccarone(in_source, chat_api)
 
 def enable(
         py_string_matching=True,
         include_pattern=None,
         exclude_pattern=None,
     ):
     """Exclude patterns take precedence over include patterns."""
```

### Comparing `maccarone-0.0.9/src/maccarone/preprocessor.py` & `maccarone-0.1.0/src/maccarone/preprocessor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import logging
 
 from dataclasses import dataclass
 
-from maccarone.openai import complete_chat_with_cache
+from maccarone.openai import CachedChatAPI
 
 logger = logging.getLogger(__name__)
 
 class Piece:
     pass
 
 @dataclass
@@ -55,15 +55,15 @@
             case _:
                 raise TypeError("unknown piece type", piece)
 
     logger.debug("tagged input ↓\n%s", tag_source)
 
     return tag_source
 
-def tagged_input_to_tagged_output(tagged_input: str) -> str:
+def tagged_input_to_tagged_output(tagged_input: str, chat_api: CachedChatAPI) -> str:
     system_prompt = """
 You are an expert programmer working on contract. Your client has written a partial program, but left pieces for you to complete. They have marked those with `<write_this>` tags inside Python comments, e.g.:
 
 ```
 def add_two_numbers(x, y):
     # <write_this id="0">
     # add the two numbers
@@ -92,15 +92,15 @@
 
 This formatting is very important. The client uses a custom tool to process your work product, and their tool requires this format. Follow this format exactly and do not copy anything outside a `<write_this>` tag.
 """
     chat_messages = [
         {"role": "system", "content": system_prompt},
         {"role": "user", "content": tagged_input},
     ]
-    tagged_output = complete_chat_with_cache(chat_messages)
+    tagged_output = chat_api.complete_chat("tagged_input_to_tagged_output", chat_messages)
 
     logger.debug("tagged output ↓\n%s", tagged_output)
 
     return tagged_output
 
 def tagged_output_to_completed_pieces(tagged_output: str) -> dict[int, str]:
     pattern = re.compile(r'<completed id="(?P<id>\d+)">\n(?P<content>.+?)</>', re.DOTALL)
@@ -127,15 +127,15 @@
             case _:
                 raise TypeError("unknown piece type", raw)
 
     logger.debug("final source ↓\n%s", final_source)
 
     return final_source
 
-def preprocess_maccarone(raw_source: str) -> str:
+def preprocess_maccarone(raw_source: str, chat_api: CachedChatAPI) -> str:
     raw_pieces = raw_source_to_pieces(raw_source)
     tagged_input = raw_pieces_to_tagged_input(raw_pieces)
-    tagged_output = tagged_input_to_tagged_output(tagged_input)
+    tagged_output = tagged_input_to_tagged_output(tagged_input, chat_api)
     completed_pieces = tagged_output_to_completed_pieces(tagged_output)
     final_source = pieces_to_final_source(raw_pieces, completed_pieces)
 
     return final_source
```

### Comparing `maccarone-0.0.9/src/maccarone/scripts/preprocess.mn.py` & `maccarone-0.1.0/src/maccarone/scripts/preprocess.mn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,60 @@
+import os
 import glob
 import logging
 
-from argparse import (
-    ArgumentParser,
-    Namespace,
-)
+from argparse import Namespace
 
+from maccarone.openai import CachedChatAPI
 from maccarone.preprocessor import preprocess_maccarone
 
 logger = logging.getLogger(__name__)
 
-def preprocess(mn_path: str, suffix=".mn.py") -> None:
-    # replace suffix with `.py`
-    assert mn_path.endswith(suffix)
+def preprocess(mn_path: str, print_: bool, write: bool, suffix: str) -> None:
+    # produce Python source
+    logger.info("preprocessing %s", mn_path)
 
-    py_path = mn_path[:-len(suffix)] + ".py"
+    cache_path = mn_path.replace(suffix, ".mn.json")
+    chat_api = CachedChatAPI(cache_path)
 
-    # produce Python source
-    logger.info("preprocessing %s → %s", mn_path, py_path)
+    #<<mn_source = read mn_path>>
+
+    py_source = preprocess_maccarone(mn_source, chat_api)
+
+    if write:
+        #<<py_path = regex replace mn_path: f"{suffix}$" -> ".py">>
+
+        logger.info("writing %s", py_path)
+
+        if py_path == mn_path:
+            raise ValueError("won't overwrite input file", mn_path)
+
+        #<<write py_source to py_path>>
 
-    with open(mn_path, "rt") as mn_file:
-        mn_source = mn_file.read()
-        py_source = preprocess_maccarone(mn_source)
+    if print_:
+        print(py_source)
 
-    with open(py_path, "wt") as file:
-        file.write(py_source)
+def main(path: str, print_: bool, write: bool, suffix: str) -> None:
+    """Preprocess files with Maccarone snippets."""
 
-def main(root_path: str):
-    """Preprocess maccarone files into Python."""
+    if os.path.isdir(path):
+        mn_files = glob.glob(
+            os.path.join(path, f"**/*{suffix}"),
+            recursive=True,
+        )
+    else:
+        mn_files = [path]
 
-    for path in glob.glob(root_path + "/**/*.mn.py", recursive=True):
-        preprocess(path)
+    #<<preprocess mn_files>>
 
 def parse_args() -> Namespace:
-    #<<use argparse to handle `script ROOT_PATH`>>
+    #<<
+    # get args for main() and return; use argparse
+    # default suffix: ".mn.py"
+    #>>
 
 def script_main():
     logging.basicConfig(level=logging.INFO)
 
     return main(**vars(parse_args()))
 
 if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `maccarone-0.0.9/src/maccarone/test/test_preprocessor.py` & `maccarone-0.1.0/src/maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.9/src/maccarone.egg-info/SOURCES.txt` & `maccarone-0.1.0/src/maccarone.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,36 @@
 dev-requirements.txt
 local-dev-requirements.txt
 pyproject.toml
 .github/workflows/publish-to-pypi-stale.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/run-pytest.yml
 examples/__init__.py
+examples/add.mn.json
 examples/add.mn.py
+examples/file_sizes.mn.json
+examples/file_sizes.mn.py
+examples/fizzbuzz.mn.json
 examples/fizzbuzz.mn.py
+examples/todo.mn.json
 examples/todo.mn.py
 src/maccarone/__init__.py
+src/maccarone/caching.mn.json
+src/maccarone/caching.mn.py
 src/maccarone/caching.py
+src/maccarone/loader.mn.json
 src/maccarone/loader.mn.py
 src/maccarone/loader.py
 src/maccarone/openai.py
 src/maccarone/preprocessor.py
 src/maccarone.egg-info/PKG-INFO
 src/maccarone.egg-info/SOURCES.txt
 src/maccarone.egg-info/dependency_links.txt
 src/maccarone.egg-info/entry_points.txt
 src/maccarone.egg-info/requires.txt
 src/maccarone.egg-info/top_level.txt
+src/maccarone/scripts/preprocess.mn.json
 src/maccarone/scripts/preprocess.mn.py
 src/maccarone/scripts/preprocess.py
 src/maccarone/test/test_caching.py
 src/maccarone/test/test_preprocessor.py
 support/rename_to_stale.sh
```

### Comparing `maccarone-0.0.9/support/rename_to_stale.sh` & `maccarone-0.1.0/support/rename_to_stale.sh`

 * *Files identical despite different names*

