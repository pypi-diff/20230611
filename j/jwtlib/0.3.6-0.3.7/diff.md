# Comparing `tmp/jwtlib-0.3.6.tar.gz` & `tmp/jwtlib-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtlib-0.3.6.tar", max compression
+gzip compressed data, was "jwtlib-0.3.7.tar", max compression
```

## Comparing `jwtlib-0.3.6.tar` & `jwtlib-0.3.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      241 2023-06-11 14:30:07.207862 jwtlib-0.3.6/AUTHORS
--rw-r--r--   0        0        0    11357 2023-06-11 14:30:07.207862 jwtlib-0.3.6/LICENSE
--rw-r--r--   0        0        0      922 2023-06-11 14:30:07.207862 jwtlib-0.3.6/README.rst
--rw-r--r--   0        0        0     1675 2023-06-11 14:30:07.207862 jwtlib-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      209 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/__init__.py
--rw-r--r--   0        0        0      344 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/abstract.py
--rw-r--r--   0        0        0      857 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/exc.py
--rw-r--r--   0        0        0     7370 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/main.py
--rw-r--r--   0        0        0        0 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/py.typed
--rw-r--r--   0        0        0       87 2023-06-11 14:30:07.207862 jwtlib-0.3.6/src/jwtlib/types.py
--rw-r--r--   0        0        0     1688 2023-06-11 14:30:12.130131 jwtlib-0.3.6/setup.py
--rw-r--r--   0        0        0     1754 2023-06-11 14:30:12.130398 jwtlib-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-06-11 14:35:41.079530 jwtlib-0.3.7/AUTHORS
+-rw-r--r--   0        0        0    11357 2023-06-11 14:35:41.079530 jwtlib-0.3.7/LICENSE
+-rw-r--r--   0        0        0      924 2023-06-11 14:35:41.079530 jwtlib-0.3.7/README.rst
+-rw-r--r--   0        0        0     1676 2023-06-11 14:35:41.079530 jwtlib-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-06-11 14:35:41.079530 jwtlib-0.3.7/src/jwtlib/__init__.py
+-rw-r--r--   0        0        0      344 2023-06-11 14:35:41.079530 jwtlib-0.3.7/src/jwtlib/abstract.py
+-rw-r--r--   0        0        0      857 2023-06-11 14:35:41.079530 jwtlib-0.3.7/src/jwtlib/exc.py
+-rw-r--r--   0        0        0     7370 2023-06-11 14:35:41.079530 jwtlib-0.3.7/src/jwtlib/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:35:41.079530 jwtlib-0.3.7/src/jwtlib/py.typed
+-rw-r--r--   0        0        0       87 2023-06-11 14:35:41.079530 jwtlib-0.3.7/src/jwtlib/types.py
+-rw-r--r--   0        0        0     1689 2023-06-11 14:35:45.960256 jwtlib-0.3.7/setup.py
+-rw-r--r--   0        0        0     1756 2023-06-11 14:35:45.960526 jwtlib-0.3.7/PKG-INFO
```

### Comparing `jwtlib-0.3.6/LICENSE` & `jwtlib-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.6/pyproject.toml` & `jwtlib-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "jwtlib"
-version = "0.3.6"
+version = "0.3.7"
 description = "A little helper library to streamline working with JWT in python"
 readme = "README.rst"
 repository = "http://github.com/novopl/jwtlib"
 homepage = "http://novopl.github.com/jwtlib"
 documentation = "http://novopl.github.com/jwtlib"
 authors = ["Mateusz Klos <novopl@gmail.com>"]
 license = "Apache 2.0"
@@ -63,14 +63,15 @@
 
 
 
 
 
 
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 ##################
 #     PYTEST     #
```

### Comparing `jwtlib-0.3.6/src/jwtlib/exc.py` & `jwtlib-0.3.7/src/jwtlib/exc.py`

 * *Files identical despite different names*

### Comparing `jwtlib-0.3.6/src/jwtlib/main.py` & `jwtlib-0.3.7/src/jwtlib/main.py`

 * *Files identical despite different names*

