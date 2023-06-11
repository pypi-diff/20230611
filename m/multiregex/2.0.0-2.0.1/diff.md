# Comparing `tmp/multiregex-2.0.0.tar.gz` & `tmp/multiregex-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiregex-2.0.0.tar", last modified: Fri Mar 10 15:22:03 2023, max compression
+gzip compressed data, was "multiregex-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `multiregex-2.0.0.tar` & `multiregex-2.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      340 2023-02-28 16:13:25.191347 multiregex-2.0.0/.flake8
--rw-r--r--   0        0        0       87 2023-02-28 16:13:25.191474 multiregex-2.0.0/.gitattributes
--rw-r--r--   0        0        0       13 2023-02-28 16:13:25.191642 multiregex-2.0.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      204 2023-02-28 16:13:25.191773 multiregex-2.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      154 2023-02-28 16:13:25.191893 multiregex-2.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1904 2023-03-10 15:18:35.560271 multiregex-2.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      814 2023-03-10 15:11:47.869468 multiregex-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      683 2023-03-10 15:18:35.560561 multiregex-2.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1456 2023-02-28 16:13:25.192643 multiregex-2.0.0/LICENSE
--rw-r--r--   0        0        0     3563 2023-03-10 15:11:47.869879 multiregex-2.0.0/README.md
--rw-r--r--   0        0        0      634 2023-02-28 16:13:25.193193 multiregex-2.0.0/docs/Makefile
--rw-r--r--   0        0        0      341 2023-02-28 16:13:25.193321 multiregex-2.0.0/docs/changelog.rst
--rw-r--r--   0        0        0     3001 2023-02-28 16:13:25.193473 multiregex-2.0.0/docs/conf.py
--rw-r--r--   0        0        0      257 2023-02-28 16:13:25.193598 multiregex-2.0.0/docs/index.rst
--rw-r--r--   0        0        0      793 2023-02-28 16:13:25.193758 multiregex-2.0.0/docs/make.bat
--rw-r--r--   0        0        0      328 2023-03-10 15:18:35.560841 multiregex-2.0.0/environment.yml
--rw-r--r--   0        0        0     1373 2023-03-10 15:18:35.561154 multiregex-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      833 2023-02-28 16:13:25.194132 multiregex-2.0.0/setup.cfg
--rw-r--r--   0        0        0       38 2023-02-28 16:13:25.194241 multiregex-2.0.0/setup.py
--rw-r--r--   0        0        0      257 2023-02-28 16:13:25.194423 multiregex-2.0.0/src/ahocorasick.pyi
--rw-r--r--   0        0        0    12425 2023-03-10 15:18:43.182347 multiregex-2.0.0/src/multiregex/__init__.py
--rw-r--r--   0        0        0      274 2023-02-28 16:13:25.194904 multiregex-2.0.0/test_utils/__init__.py
--rw-r--r--   0        0        0    26689 2023-02-28 16:13:25.195190 multiregex-2.0.0/test_utils/cpython_test_re.py
--rw-r--r--   0        0        0      147 2023-02-28 16:13:25.195377 multiregex-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     2068 2023-02-28 16:13:25.195518 multiregex-2.0.0/tests/test_bench.py
--rw-r--r--   0        0        0     1700 2023-03-10 15:11:47.870923 multiregex-2.0.0/tests/test_cpython_tests.py
--rw-r--r--   0        0        0     2655 2023-03-10 15:11:47.871125 multiregex-2.0.0/tests/test_multiregex.py
--rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 multiregex-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-05-19 20:49:42.665965 multiregex-2.0.1/.flake8
+-rw-r--r--   0        0        0       87 2023-05-19 20:49:42.666037 multiregex-2.0.1/.gitattributes
+-rw-r--r--   0        0        0       13 2023-05-19 20:49:42.666152 multiregex-2.0.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      204 2023-05-19 20:49:42.666236 multiregex-2.0.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      154 2023-05-19 20:49:42.666306 multiregex-2.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1405 2023-05-19 20:49:42.666427 multiregex-2.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      814 2023-06-11 16:55:47.232106 multiregex-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      802 2023-06-11 17:25:41.840034 multiregex-2.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1456 2023-05-19 20:49:42.666735 multiregex-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3977 2023-05-19 20:49:42.666825 multiregex-2.0.1/README.md
+-rw-r--r--   0        0        0      634 2023-05-19 20:49:42.666943 multiregex-2.0.1/docs/Makefile
+-rw-r--r--   0        0        0      341 2023-05-19 20:49:42.667012 multiregex-2.0.1/docs/changelog.rst
+-rw-r--r--   0        0        0     3001 2023-05-19 20:49:42.667091 multiregex-2.0.1/docs/conf.py
+-rw-r--r--   0        0        0      257 2023-05-19 20:49:42.667148 multiregex-2.0.1/docs/index.rst
+-rw-r--r--   0        0        0      793 2023-05-19 20:49:42.667240 multiregex-2.0.1/docs/make.bat
+-rw-r--r--   0        0        0      328 2023-05-19 20:49:42.667307 multiregex-2.0.1/environment.yml
+-rw-r--r--   0        0        0     1329 2023-05-19 20:49:42.667396 multiregex-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      792 2023-05-19 20:49:42.667473 multiregex-2.0.1/setup.cfg
+-rw-r--r--   0        0        0       38 2023-05-19 20:49:42.667531 multiregex-2.0.1/setup.py
+-rw-r--r--   0        0        0      257 2023-05-19 20:49:42.667626 multiregex-2.0.1/src/ahocorasick.pyi
+-rw-r--r--   0        0        0    12552 2023-06-11 17:25:50.232318 multiregex-2.0.1/src/multiregex/__init__.py
+-rw-r--r--   0        0        0      274 2023-05-19 20:49:42.667880 multiregex-2.0.1/test_utils/__init__.py
+-rw-r--r--   0        0        0    26689 2023-05-19 20:49:42.668028 multiregex-2.0.1/test_utils/cpython_test_re.py
+-rw-r--r--   0        0        0      147 2023-05-19 20:49:42.668128 multiregex-2.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     2068 2023-05-19 20:49:42.668194 multiregex-2.0.1/tests/test_bench.py
+-rw-r--r--   0        0        0     1700 2023-05-19 20:49:42.668274 multiregex-2.0.1/tests/test_cpython_tests.py
+-rw-r--r--   0        0        0     2746 2023-06-11 17:25:41.840429 multiregex-2.0.1/tests/test_multiregex.py
+-rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 multiregex-2.0.1/PKG-INFO
```

### Comparing `multiregex-2.0.0/.github/workflows/ci.yml` & `multiregex-2.0.1/.github/workflows/ci.yml`

 * *Files 21% similar despite different names*

```diff
@@ -13,46 +13,32 @@
   tests:
     name: Tests - Python ${{ matrix.python-version }} - ${{ matrix.os }}
     timeout-minutes: 10
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        include:
-          - { python-version: "3.4", os: ubuntu-18.04 }
-          - { python-version: "3.6", os: windows-2019 }
-          - { python-version: "3.8", os: windows-latest }
-          - { python-version: "3.10", os: ubuntu-latest }
-          - { python-version: "3.11", os: ubuntu-latest }
+        python-version: ['3.6', '3.7', '3.8', '3.9', '3.10', '3.11']
+        os: ['ubuntu-latest', 'windows-latest', 'macos-latest']
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
       - name: Fetch full git history
         run: git fetch --prune --unshallow
-      - name: Set up Conda env
-        uses: mamba-org/provision-with-micromamba@e2b397b12d0a38069451664382b769c9456e3d6d
+      - name: Set up Micromamba env
+        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
         with:
-          extra-specs: |
+          environment-file: environment.yml
+          create-args: >-
             python=${{ matrix.python-version }}
-        if: matrix.python-version != '3.4'
-      - name: "Install Python 3.4"
-        uses: actions/setup-python@v4
-        with:
-          python-version: 3.4
-        if: matrix.python-version == '3.4'
       - name: Run tests
         run: |
-          if [ ${{ matrix.python-version }} = 3.4 ]; then
-            pip install pytest pyahocorasick
-            export PYTHONPATH=src
-          else
-            pip install -e .
-          fi
+          pip install -e .
           pytest -v tests/
 
   pre-commit-checks:
     name: pre-commit checks
     timeout-minutes: 10
     runs-on: ubuntu-latest
     steps:
```

### Comparing `multiregex-2.0.0/.pre-commit-config.yaml` & `multiregex-2.0.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/Quantco/pre-commit-mirrors-black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black-conda
         args:
           - --safe
           - --target-version=py36
   - repo: https://github.com/Quantco/pre-commit-mirrors-flake8
     rev: 6.0.0
@@ -12,17 +12,17 @@
       - id: flake8-conda
   - repo: https://github.com/Quantco/pre-commit-mirrors-isort
     rev: 5.12.0
     hooks:
       - id: isort-conda
         additional_dependencies: [-c, conda-forge, toml=0.10.2]
   - repo: https://github.com/Quantco/pre-commit-mirrors-mypy
-    rev: 1.0.1
+    rev: 1.3.0
     hooks:
       - id: mypy-conda
         additional_dependencies: [-c, conda-forge, types-setuptools]
   - repo: https://github.com/Quantco/pre-commit-mirrors-pyupgrade
-    rev: 3.3.1
+    rev: 3.4.0
     hooks:
       - id: pyupgrade-conda
         args:
           - --py3-plus
```

### Comparing `multiregex-2.0.0/LICENSE` & `multiregex-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.0/README.md` & `multiregex-2.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # multiregex
 
 [![CI](https://github.com/Quantco/multiregex/actions/workflows/ci.yml/badge.svg)](https://github.com/Quantco/multiregex/actions/workflows/ci.yml)
 [![Documentation](https://img.shields.io/badge/docs-latest-success?style=plastic)](https://docs.dev.quantco.cloud/qc-github-artifacts/Quantco/multiregex/latest/index.html)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/multiregex?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/multiregex)
+[![pypi-version](https://img.shields.io/pypi/v/multiregex.svg?logo=pypi&logoColor=white)](https://pypi.org/project/multiregex)
+[![python-version](https://img.shields.io/pypi/pyversions/multiregex?logoColor=white&logo=python)](https://pypi.org/project/multiregex)
 
 Quickly match many regexes against a string. Provides 2-10x speedups over naïve regex matching.
 
 ## Installation
 
 You can install the package in development mode using:
```

### Comparing `multiregex-2.0.0/docs/Makefile` & `multiregex-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.0/docs/conf.py` & `multiregex-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.0/docs/make.bat` & `multiregex-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.0/pyproject.toml` & `multiregex-2.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 name = "multiregex"
 authors = [{name="QuantCo, Inc.", email="noreply@quantco.com"}]
 
 maintainers = [{name = "Jonas Haag", email = "jonas.haag@quantco.com"}]
 
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.4",
-    "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
 ]
 
 readme = "README.md"
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://github.com/quantco/multiregex"
```

### Comparing `multiregex-2.0.0/setup.cfg` & `multiregex-2.0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Quantco/multiregex
 author = QuantCo, Inc.
 author_email = noreply@quantco.com
 classifiers =
     Programming Language :: Python :: 3
-    Programming Language :: Python :: 3.4
-    Programming Language :: Python :: 3.5
     Programming Language :: Python :: 3.6
     Programming Language :: Python :: 3.7
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.9
     Programming Language :: Python :: 3.10
+    Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = true
 install_requires = pyahocorasick
-python_requires = >=3.4
+python_requires = >=3.6
 package_dir=
     =src
 packages = find:
 
 [options.packages.find]
 where = src
```

### Comparing `multiregex-2.0.0/src/multiregex/__init__.py` & `multiregex-2.0.1/src/multiregex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     TypeVar,
     Union,
     cast,
 )
 
 import ahocorasick
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 
 V = TypeVar("V")
 PatternOrStr = Union[Pattern, str]
 Prematchers = Set[str]
 FalsePositivesCounter = Dict[str, int]
 
@@ -79,18 +79,21 @@
             the input strings given to ``search``, ``match``, and ``fullmatch``.
             Use ``format_prematcher_false_positives`` to retrieve the profile.
         """
         patterns = self._normalize_patterns(patterns)
         patterns = self._generate_missing_prematchers(patterns)
         self.patterns = [pattern for pattern, _ in patterns]
         self.prematchers = dict(patterns)
+        enumerated_patterns = list(enumerate(patterns))
         self.patterns_without_prematchers = {
-            pattern for pattern, prematchers in patterns if not prematchers
+            (idx, pattern)
+            for idx, (pattern, prematchers) in enumerated_patterns
+            if not prematchers
         }
-        self.automaton = self._make_automaton(patterns)
+        self.automaton = self._make_automaton(enumerated_patterns)
 
         self.count_prematcher_false_positives = count_prematcher_false_positives
         if count_prematcher_false_positives:
             self.prematcher_false_positives = {
                 pattern: {"positives": 0, "false_positives": 0}
                 for pattern in self.patterns
             }
@@ -138,18 +141,18 @@
         ]
         for _, prematchers in patterns:
             for prematcher in prematchers:
                 validate_prematcher(prematcher)
         return patterns
 
     @staticmethod
-    def _make_automaton(patterns):
+    def _make_automaton(enumerated_patterns):
         """Create the pyahocorasick automaton."""
         pattern_candidates_by_prematchers = collections.defaultdict(set)
-        for pattern_idx, (pattern, prematchers) in enumerate(patterns):
+        for pattern_idx, (pattern, prematchers) in enumerated_patterns:
             for prematcher in prematchers:
                 # `pattern_idx` is used for keeping patterns in order, see `get_pattern_candidates`.
                 pattern_candidates_by_prematchers[prematcher].add(
                     (pattern_idx, pattern)
                 )
         return _ahocorasick_make_automaton(pattern_candidates_by_prematchers)
```

### Comparing `multiregex-2.0.0/test_utils/cpython_test_re.py` & `multiregex-2.0.1/test_utils/cpython_test_re.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.0/tests/test_bench.py` & `multiregex-2.0.1/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.0/tests/test_cpython_tests.py` & `multiregex-2.0.1/tests/test_cpython_tests.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.0/tests/test_multiregex.py` & `multiregex-2.0.1/tests/test_multiregex.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,19 +34,21 @@
     assert not matcher.match("abc")
     assert matcher.match("b")
     assert not matcher.fullmatch("bb")
     assert matcher.fullmatch("b")
 
 
 def test_ordered():
-    patterns = [re.compile(c) for c in "abcdef"]
+    patterns = [
+        (re.compile(c), None if i % 2 == 0 else []) for i, c in enumerate("abcdef")
+    ]  # type: ignore
     random.shuffle(patterns)
     matcher = RegexMatcher(patterns)
-    matches = matcher.search("abcdef")
-    assert [p for p, _ in matches] == patterns
+    matches = matcher.search("abcdefg")
+    assert [p for p, _ in matches] == [p for p, _ in patterns]
 
 
 @pytest.mark.parametrize(
     "pattern, prematcher",
     [
         ("a", {"a"}),
         ("[a]", {"a"}),
```

### Comparing `multiregex-2.0.0/PKG-INFO` & `multiregex-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: multiregex
-Version: 2.0.0
+Version: 2.0.1
 Summary: Speed up regex matching with non-regex substring "prematchers", similar to Bloom filters.
 Author-email: "QuantCo, Inc." <noreply@quantco.com>
 Maintainer-email: Jonas Haag <jonas.haag@quantco.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Home, https://github.com/quantco/multiregex
 
 # multiregex
 
 [![CI](https://github.com/Quantco/multiregex/actions/workflows/ci.yml/badge.svg)](https://github.com/Quantco/multiregex/actions/workflows/ci.yml)
 [![Documentation](https://img.shields.io/badge/docs-latest-success?style=plastic)](https://docs.dev.quantco.cloud/qc-github-artifacts/Quantco/multiregex/latest/index.html)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/multiregex?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/multiregex)
+[![pypi-version](https://img.shields.io/pypi/v/multiregex.svg?logo=pypi&logoColor=white)](https://pypi.org/project/multiregex)
+[![python-version](https://img.shields.io/pypi/pyversions/multiregex?logoColor=white&logo=python)](https://pypi.org/project/multiregex)
 
 Quickly match many regexes against a string. Provides 2-10x speedups over naïve regex matching.
 
 ## Installation
 
 You can install the package in development mode using:
```

