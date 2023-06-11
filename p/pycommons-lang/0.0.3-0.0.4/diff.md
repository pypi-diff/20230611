# Comparing `tmp/pycommons_lang-0.0.3.tar.gz` & `tmp/pycommons_lang-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycommons_lang-0.0.3.tar", max compression
+gzip compressed data, was "pycommons_lang-0.0.4.tar", max compression
```

## Comparing `pycommons_lang-0.0.3.tar` & `pycommons_lang-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,10 @@
--rw-r--r--   0        0        0    11346 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/LICENSE
--rw-r--r--   0        0        0     1343 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/README.md
--rw-r--r--   0        0        0      431 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/__init__.py
--rw-r--r--   0        0        0       65 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/base/__init__.py
--rw-r--r--   0        0        0     5648 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/base/char.py
--rw-r--r--   0        0        0       58 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/__init__.py
--rw-r--r--   0        0        0      754 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/boolean.py
--rw-r--r--   0        0        0      761 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/container.py
--rw-r--r--   0        0        0     1469 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/integer.py
--rw-r--r--   0        0        0     4457 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/optional.py
--rw-r--r--   0        0        0       88 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/exception/__init__.py
--rw-r--r--   0        0        0      367 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/exception/no_such_element_error.py
--rw-r--r--   0        0        0      320 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/__init__.py
--rw-r--r--   0        0        0     1266 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/comparator.py
--rw-r--r--   0        0        0     1454 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/consumer.py
--rw-r--r--   0        0        0      594 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/function.py
--rw-r--r--   0        0        0     2249 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/predicate.py
--rw-r--r--   0        0        0      496 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/runnable.py
--rw-r--r--   0        0        0      532 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/supplier.py
--rw-r--r--   0        0        0        0 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/streams/__init__.py
--rw-r--r--   0        0        0     6823 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/streams/iterator.py
--rw-r--r--   0        0        0     2264 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/streams/stream.py
--rw-r--r--   0        0        0      725 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/streams/streams.py
--rw-r--r--   0        0        0        0 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/__init__.py
--rw-r--r--   0        0        0      399 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/arrayutils.py
--rw-r--r--   0        0        0     2385 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/charutils.py
--rw-r--r--   0        0        0      520 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/objectutils.py
--rw-r--r--   0        0        0    11127 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/stringutils.py
--rw-r--r--   0        0        0      119 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/utils.py
--rw-r--r--   0        0        0        0 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/py.typed
--rw-r--r--   0        0        0     1780 2023-06-08 19:11:56.867698 pycommons_lang-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 pycommons_lang-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-11 16:12:10.109142 pycommons_lang-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1343 2023-06-11 16:12:10.109142 pycommons_lang-0.0.4/README.md
+-rw-r--r--   0        0        0      431 2023-06-11 16:12:10.109142 pycommons_lang-0.0.4/pycommons/lang/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 16:12:10.109142 pycommons_lang-0.0.4/pycommons/lang/utils/__init__.py
+-rw-r--r--   0        0        0      399 2023-06-11 16:12:10.113144 pycommons_lang-0.0.4/pycommons/lang/utils/arrayutils.py
+-rw-r--r--   0        0        0     2380 2023-06-11 16:12:10.113144 pycommons_lang-0.0.4/pycommons/lang/utils/charutils.py
+-rw-r--r--   0        0        0    11143 2023-06-11 16:12:10.113144 pycommons_lang-0.0.4/pycommons/lang/utils/stringutils.py
+-rw-r--r--   0        0        0        0 2023-06-11 16:12:10.113144 pycommons_lang-0.0.4/pycommons/py.typed
+-rw-r--r--   0        0        0     1823 2023-06-11 16:12:26.394337 pycommons_lang-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 pycommons_lang-0.0.4/PKG-INFO
```

### Comparing `pycommons_lang-0.0.3/LICENSE` & `pycommons_lang-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycommons_lang-0.0.3/README.md` & `pycommons_lang-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pycommons_lang-0.0.3/pycommons/lang/utils/charutils.py` & `pycommons_lang-0.0.4/pycommons/lang/utils/charutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import string
 from typing import Optional, Set
 
-from pycommons.lang.base.char import Char, CharType
+from pycommons.base.char import Char, CharType
 
 
 class CharUtils:
     ASCII_SPACE: Char = Char(" ")
 
     # region: Whitespaces
     WHITESPACES: Set[Char] = {Char(c) for c in string.whitespace}
```

### Comparing `pycommons_lang-0.0.3/pycommons/lang/utils/stringutils.py` & `pycommons_lang-0.0.4/pycommons/lang/utils/stringutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing
 from typing import Optional, List
 
-from pycommons.lang.base.char import Char
-from pycommons.lang.function import Supplier
+from pycommons.base.char import Char
+from pycommons.base.function import Supplier
+from pycommons.base.utils.utils import UtilityClass
+
 from .arrayutils import ArrayUtils
 from .charutils import CharUtils
-from .utils import UtilityClass
 
 
 class StringUtils(UtilityClass):
     """
     The StringUtils `UtilityClass` that holds the utility methods for string observation,
     manipulation, conversion etc. This class is inspired by the
     [`StringUtils`](https://commons.apache.org/proper/commons-lang/apidocs/index.html)
```

### Comparing `pycommons_lang-0.0.3/pyproject.toml` & `pycommons_lang-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool]
 
 [tool.poetry]
 name = "pycommons.lang"
-version = "0.0.3"
+version = "0.0.4"
 homepage = "https://github.com/shashankrnr32/pycommons-lang"
 description = "Python Commons Lang"
 authors = ["Shashank Sharma <shashankrnr32@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -21,25 +21,27 @@
     "LICENSE",
     "pycommons/py.typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 importlib_metadata = "*"
+pycommons-base = "0.0.5"
 
 [tool.poetry.dev-dependencies]
 mkdocs-material = ">7.0.0"
 mkdocstrings = { version = ">0.18", extras = ["python-legacy"] }
 mkdocs-awesome-pages-plugin = "*"
 markdown-include = "*"
 livereload = "*"
 poethepoet = "^0.20.0"
 
 pytest = ">=7.2.0"
 pytest-cov = "^2.10.1"
+mockito = "1.4.0"
 
 pylint = "^2.6.0"
 black = "22.3.0"
 mypy = "0.960"
 
 [tool.black]
 line-length = 100
```

### Comparing `pycommons_lang-0.0.3/PKG-INFO` & `pycommons_lang-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycommons-lang
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Commons Lang
 Home-page: https://github.com/shashankrnr32/pycommons-lang
 License: Apache-2.0
 Author: Shashank Sharma
 Author-email: shashankrnr32@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: importlib_metadata
+Requires-Dist: pycommons-base (==0.0.5)
 Description-Content-Type: text/markdown
 
 # pycommons-lang
 
 [![PyPI](https://img.shields.io/pypi/v/pycommons-lang)](https://pypi.org/project/pycommons-lang/)
 ![versions](https://img.shields.io/pypi/pyversions/pycommons-lang.svg)
 ![PyPI - License](https://img.shields.io/pypi/l/pycommons-lang)
```

