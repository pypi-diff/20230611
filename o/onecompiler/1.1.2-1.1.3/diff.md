# Comparing `tmp/onecompiler-1.1.2.tar.gz` & `tmp/onecompiler-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onecompiler-1.1.2.tar", max compression
+gzip compressed data, was "onecompiler-1.1.3.tar", max compression
```

## Comparing `onecompiler-1.1.2.tar` & `onecompiler-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-1.1.2/LICENSE
--rw-r--r--   0        0        0     1036 2023-06-11 17:03:52.315001 onecompiler-1.1.2/README.md
--rw-r--r--   0        0        0      134 2023-06-11 17:03:52.319001 onecompiler-1.1.2/onecompiler/__init__.py
--rw-r--r--   0        0        0      143 2023-06-11 17:03:52.323001 onecompiler-1.1.2/onecompiler/api/__init__.py
--rw-r--r--   0        0        0     1752 2023-06-11 17:03:52.323001 onecompiler-1.1.2/onecompiler/api/async_compiler.py
--rw-r--r--   0        0        0     1645 2023-06-11 17:03:52.327001 onecompiler-1.1.2/onecompiler/api/compiler.py
--rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-1.1.2/onecompiler/base_errors/LangNotFound.py
--rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-1.1.2/onecompiler/base_errors/__init__.py
--rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-1.1.2/onecompiler/base_models/__init__.py
--rw-r--r--   0        0        0     1781 2023-06-11 17:03:52.327001 onecompiler-1.1.2/onecompiler/base_models/base_compiler.py
--rw-r--r--   0        0        0     2493 2023-06-11 17:03:52.331001 onecompiler-1.1.2/onecompiler/data.py
--rw-r--r--   0        0        0      175 2023-06-11 17:03:52.331001 onecompiler-1.1.2/onecompiler/pydantic_models/__init__.py
--rw-r--r--   0        0        0      602 2023-06-11 17:03:52.335001 onecompiler-1.1.2/onecompiler/pydantic_models/lang.py
--rw-r--r--   0        0        0      791 2023-06-11 17:03:52.335001 onecompiler-1.1.2/onecompiler/pydantic_models/response.py
--rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-1.1.2/onecompiler/requirements.txt
--rw-r--r--   0        0        0      325 2023-06-11 17:04:03.223001 onecompiler-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 onecompiler-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1036 2023-06-11 17:03:52.315001 onecompiler-1.1.3/README.md
+-rw-r--r--   0        0        0      134 2023-06-11 17:03:52.319001 onecompiler-1.1.3/onecompiler/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-11 17:03:52.323001 onecompiler-1.1.3/onecompiler/api/__init__.py
+-rw-r--r--   0        0        0     1752 2023-06-11 17:03:52.323001 onecompiler-1.1.3/onecompiler/api/async_compiler.py
+-rw-r--r--   0        0        0     1645 2023-06-11 17:03:52.327001 onecompiler-1.1.3/onecompiler/api/compiler.py
+-rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-1.1.3/onecompiler/base_errors/LangNotFound.py
+-rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-1.1.3/onecompiler/base_errors/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-1.1.3/onecompiler/base_models/__init__.py
+-rw-r--r--   0        0        0     1781 2023-06-11 17:03:52.327001 onecompiler-1.1.3/onecompiler/base_models/base_compiler.py
+-rw-r--r--   0        0        0     2493 2023-06-11 17:03:52.331001 onecompiler-1.1.3/onecompiler/data.py
+-rw-r--r--   0        0        0      175 2023-06-11 17:03:52.331001 onecompiler-1.1.3/onecompiler/pydantic_models/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-11 17:03:52.335001 onecompiler-1.1.3/onecompiler/pydantic_models/lang.py
+-rw-r--r--   0        0        0      791 2023-06-11 17:03:52.335001 onecompiler-1.1.3/onecompiler/pydantic_models/response.py
+-rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-1.1.3/onecompiler/requirements.txt
+-rw-r--r--   0        0        0      381 2023-06-11 17:08:00.795001 onecompiler-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 onecompiler-1.1.3/PKG-INFO
```

### Comparing `onecompiler-1.1.2/LICENSE` & `onecompiler-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.2/README.md` & `onecompiler-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.2/onecompiler/api/async_compiler.py` & `onecompiler-1.1.3/onecompiler/api/async_compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.2/onecompiler/api/compiler.py` & `onecompiler-1.1.3/onecompiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.2/onecompiler/base_models/base_compiler.py` & `onecompiler-1.1.3/onecompiler/base_models/base_compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.2/onecompiler/data.py` & `onecompiler-1.1.3/onecompiler/data.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.2/onecompiler/pydantic_models/lang.py` & `onecompiler-1.1.3/onecompiler/pydantic_models/lang.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.2/onecompiler/pydantic_models/response.py` & `onecompiler-1.1.3/onecompiler/pydantic_models/response.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.2/PKG-INFO` & `onecompiler-1.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: onecompiler
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
+Home-page: https://github.com/pokedim13/OneCompiler
 License: Apache
 Author: pokedim13
 Author-email: skinxedovich@vk.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Project-URL: Repository, https://github.com/pokedim13/OneCompiler
 Description-Content-Type: text/markdown
 
 # OneCompiler
 ### Compilation of many languages in Python!
 
 - [Project on PyPi](https://pypi.org/project/onecompiler/)
```

