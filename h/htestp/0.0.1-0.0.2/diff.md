# Comparing `tmp/htestp-0.0.1.tar.gz` & `tmp/htestp-0.0.2.tar.gz`

## Comparing `htestp-0.0.1.tar` & `htestp-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 htestp-0.0.1/src/htestp/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 htestp-0.0.1/src/htestp/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 htestp-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 htestp-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 htestp-0.0.1/README.md
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 htestp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 htestp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 htestp-0.0.2/src/htestp/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 htestp-0.0.2/src/htestp/__init__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 htestp-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 htestp-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 htestp-0.0.2/README.md
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 htestp-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 htestp-0.0.2/PKG-INFO
```

### Comparing `htestp-0.0.1/LICENSE.txt` & `htestp-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `htestp-0.0.1/pyproject.toml` & `htestp-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [
+    "solc-select"]
 
 [project.urls]
 Documentation = "https://github.com/unknown/htestp#readme"
 Issues = "https://github.com/unknown/htestp/issues"
 Source = "https://github.com/unknown/htestp"
 
 [tool.hatch.version]
```

### Comparing `htestp-0.0.1/PKG-INFO` & `htestp-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htestp
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/unknown/htestp#readme
 Project-URL: Issues, https://github.com/unknown/htestp/issues
 Project-URL: Source, https://github.com/unknown/htestp
 Author-email: NioTheFirst <bzhangprogramming@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: solc-select
 Description-Content-Type: text/markdown
 
 # htestp
 
 [![PyPI - Version](https://img.shields.io/pypi/v/htestp.svg)](https://pypi.org/project/htestp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/htestp.svg)](https://pypi.org/project/htestp)
```

