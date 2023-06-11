# Comparing `tmp/nutorious-0.1.4.tar.gz` & `tmp/nutorious-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutorious-0.1.4.tar", max compression
+gzip compressed data, was "nutorious-0.1.5.tar", max compression
```

## Comparing `nutorious-0.1.4.tar` & `nutorious-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      171 2023-06-11 07:36:34.901265 nutorious-0.1.4/README.md
--rw-r--r--   0        0        0      827 2023-06-11 07:36:34.901265 nutorious-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1173 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/__init__.py
--rw-r--r--   0        0        0      754 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/cli/__init__.py
--rw-r--r--   0        0        0     1187 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/config/__init__.py
--rw-r--r--   0        0        0      376 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/config/default.yml
--rw-r--r--   0        0        0      204 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/context/__init__.py
--rw-r--r--   0        0        0     4436 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/journal/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/report/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/report/base.py
--rw-r--r--   0        0        0     2556 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/report/daily.py
--rw-r--r--   0        0        0        0 2023-06-11 07:36:34.901265 nutorious-0.1.4/src/nutorious/report/diff.py
--rw-r--r--   0        0        0     1094 2023-06-11 07:36:34.905265 nutorious-0.1.4/src/nutorious/ui/__init__.py
--rw-r--r--   0        0        0      503 2023-06-11 07:36:34.905265 nutorious-0.1.4/src/nutorious/ui/ui.py
--rw-r--r--   0        0        0      337 2023-06-11 07:36:34.905265 nutorious-0.1.4/src/nutorious/utils/collections.py
--rw-r--r--   0        0        0      197 2023-06-11 07:36:34.905265 nutorious-0.1.4/src/nutorious/utils/commons.py
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 nutorious-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      171 2023-06-11 07:38:28.878531 nutorious-0.1.5/README.md
+-rw-r--r--   0        0        0      827 2023-06-11 07:38:28.878531 nutorious-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1173 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/__init__.py
+-rw-r--r--   0        0        0      754 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/cli/__init__.py
+-rw-r--r--   0        0        0     1187 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/config/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/config/default.yml
+-rw-r--r--   0        0        0      204 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/context/__init__.py
+-rw-r--r--   0        0        0     4436 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/journal/__init__.py
+-rw-r--r--   0        0        0     1994 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/report/__init__.py
+-rw-r--r--   0        0        0     1475 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/report/base.py
+-rw-r--r--   0        0        0     2556 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/report/daily.py
+-rw-r--r--   0        0        0        0 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/report/diff.py
+-rw-r--r--   0        0        0     1094 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/ui/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/ui/ui.py
+-rw-r--r--   0        0        0      337 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/utils/collections.py
+-rw-r--r--   0        0        0      197 2023-06-11 07:38:28.882531 nutorious-0.1.5/src/nutorious/utils/commons.py
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 nutorious-0.1.5/PKG-INFO
```

### Comparing `nutorious-0.1.4/pyproject.toml` & `nutorious-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nutorious"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Dzmitry Paulenka <paulenka.dk@gmail.com>"]
 readme = "README.md"
 # TODO: what does this next line actually do ?
 # packages = [{include = "nutorious"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nutorious-0.1.4/src/nutorious/__init__.py` & `nutorious-0.1.5/src/nutorious/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.4/src/nutorious/cli/__init__.py` & `nutorious-0.1.5/src/nutorious/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.4/src/nutorious/config/__init__.py` & `nutorious-0.1.5/src/nutorious/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.4/src/nutorious/journal/__init__.py` & `nutorious-0.1.5/src/nutorious/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.4/src/nutorious/model/__init__.py` & `nutorious-0.1.5/src/nutorious/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.4/src/nutorious/report/base.py` & `nutorious-0.1.5/src/nutorious/report/base.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.4/src/nutorious/report/daily.py` & `nutorious-0.1.5/src/nutorious/report/daily.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.4/src/nutorious/ui/__init__.py` & `nutorious-0.1.5/src/nutorious/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.4/PKG-INFO` & `nutorious-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutorious
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Dzmitry Paulenka
 Author-email: paulenka.dk@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

