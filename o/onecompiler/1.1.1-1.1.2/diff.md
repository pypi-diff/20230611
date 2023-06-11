# Comparing `tmp/onecompiler-1.1.1.tar.gz` & `tmp/onecompiler-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onecompiler-1.1.1.tar", max compression
+gzip compressed data, was "onecompiler-1.1.2.tar", max compression
```

## Comparing `onecompiler-1.1.1.tar` & `onecompiler-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-1.1.1/LICENSE
--rw-r--r--   0        0        0       37 2023-06-06 14:12:34.685634 onecompiler-1.1.1/README.md
--rw-r--r--   0        0        0      134 2023-06-08 17:50:43.546355 onecompiler-1.1.1/onecompiler/__init__.py
--rw-r--r--   0        0        0      143 2023-06-06 21:20:15.290434 onecompiler-1.1.1/onecompiler/api/__init__.py
--rw-r--r--   0        0        0     1752 2023-06-08 18:35:03.470355 onecompiler-1.1.1/onecompiler/api/async_compiler.py
--rw-r--r--   0        0        0     1645 2023-06-08 18:37:12.018355 onecompiler-1.1.1/onecompiler/api/compiler.py
--rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-1.1.1/onecompiler/base_errors/LangNotFound.py
--rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-1.1.1/onecompiler/base_errors/__init__.py
--rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-1.1.1/onecompiler/base_models/__init__.py
--rw-r--r--   0        0        0     1781 2023-06-08 18:37:52.434355 onecompiler-1.1.1/onecompiler/base_models/base_compiler.py
--rw-r--r--   0        0        0     2493 2023-06-08 17:47:40.234355 onecompiler-1.1.1/onecompiler/data.py
--rw-r--r--   0        0        0      175 2023-06-06 22:14:05.578435 onecompiler-1.1.1/onecompiler/pydantic_models/__init__.py
--rw-r--r--   0        0        0      602 2023-06-07 14:45:16.256433 onecompiler-1.1.1/onecompiler/pydantic_models/lang.py
--rw-r--r--   0        0        0      791 2023-06-08 16:18:50.561637 onecompiler-1.1.1/onecompiler/pydantic_models/response.py
--rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-1.1.1/onecompiler/requirements.txt
--rw-r--r--   0        0        0      325 2023-06-08 18:39:05.134355 onecompiler-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 onecompiler-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1036 2023-06-11 17:03:52.315001 onecompiler-1.1.2/README.md
+-rw-r--r--   0        0        0      134 2023-06-11 17:03:52.319001 onecompiler-1.1.2/onecompiler/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-11 17:03:52.323001 onecompiler-1.1.2/onecompiler/api/__init__.py
+-rw-r--r--   0        0        0     1752 2023-06-11 17:03:52.323001 onecompiler-1.1.2/onecompiler/api/async_compiler.py
+-rw-r--r--   0        0        0     1645 2023-06-11 17:03:52.327001 onecompiler-1.1.2/onecompiler/api/compiler.py
+-rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-1.1.2/onecompiler/base_errors/LangNotFound.py
+-rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-1.1.2/onecompiler/base_errors/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-1.1.2/onecompiler/base_models/__init__.py
+-rw-r--r--   0        0        0     1781 2023-06-11 17:03:52.327001 onecompiler-1.1.2/onecompiler/base_models/base_compiler.py
+-rw-r--r--   0        0        0     2493 2023-06-11 17:03:52.331001 onecompiler-1.1.2/onecompiler/data.py
+-rw-r--r--   0        0        0      175 2023-06-11 17:03:52.331001 onecompiler-1.1.2/onecompiler/pydantic_models/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-11 17:03:52.335001 onecompiler-1.1.2/onecompiler/pydantic_models/lang.py
+-rw-r--r--   0        0        0      791 2023-06-11 17:03:52.335001 onecompiler-1.1.2/onecompiler/pydantic_models/response.py
+-rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-1.1.2/onecompiler/requirements.txt
+-rw-r--r--   0        0        0      325 2023-06-11 17:04:03.223001 onecompiler-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 onecompiler-1.1.2/PKG-INFO
```

### Comparing `onecompiler-1.1.1/LICENSE` & `onecompiler-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.1/onecompiler/api/async_compiler.py` & `onecompiler-1.1.2/onecompiler/api/async_compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.1/onecompiler/api/compiler.py` & `onecompiler-1.1.2/onecompiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.1/onecompiler/base_models/base_compiler.py` & `onecompiler-1.1.2/onecompiler/base_models/base_compiler.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.1/onecompiler/data.py` & `onecompiler-1.1.2/onecompiler/data.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.1/onecompiler/pydantic_models/lang.py` & `onecompiler-1.1.2/onecompiler/pydantic_models/lang.py`

 * *Files identical despite different names*

### Comparing `onecompiler-1.1.1/onecompiler/pydantic_models/response.py` & `onecompiler-1.1.2/onecompiler/pydantic_models/response.py`

 * *Files identical despite different names*

