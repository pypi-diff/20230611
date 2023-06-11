# Comparing `tmp/pycommons_base-0.0.3.tar.gz` & `tmp/pycommons_base-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycommons_base-0.0.3.tar", max compression
+gzip compressed data, was "pycommons_base-0.0.4.tar", max compression
```

## Comparing `pycommons_base-0.0.3.tar` & `pycommons_base-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11346 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/LICENSE
--rw-r--r--   0        0        0     1082 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/__init__.py
--rw-r--r--   0        0        0      431 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/__init__.py
--rw-r--r--   0        0        0      153 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/atomic/__init__.py
--rw-r--r--   0        0        0      759 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/atomic/atomic.py
--rw-r--r--   0        0        0      768 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/atomic/boolean.py
--rw-r--r--   0        0        0     1791 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/atomic/integer.py
--rw-r--r--   0        0        0     5648 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/char.py
--rw-r--r--   0        0        0      235 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/container/__init__.py
--rw-r--r--   0        0        0      813 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/container/boolean.py
--rw-r--r--   0        0        0      849 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/container/container.py
--rw-r--r--   0        0        0     1469 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/container/integer.py
--rw-r--r--   0        0        0     4457 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/container/optional.py
--rw-r--r--   0        0        0       88 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/exception/__init__.py
--rw-r--r--   0        0        0      367 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/exception/no_such_element_error.py
--rw-r--r--   0        0        0      320 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/function/__init__.py
--rw-r--r--   0        0        0     1266 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/function/comparator.py
--rw-r--r--   0        0        0     1454 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/function/consumer.py
--rw-r--r--   0        0        0      594 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/function/function.py
--rw-r--r--   0        0        0     2249 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/function/predicate.py
--rw-r--r--   0        0        0      496 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/function/runnable.py
--rw-r--r--   0        0        0      532 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/function/supplier.py
--rw-r--r--   0        0        0      144 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/streams/__init__.py
--rw-r--r--   0        0        0     6823 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/streams/iterator.py
--rw-r--r--   0        0        0     2264 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/streams/stream.py
--rw-r--r--   0        0        0      725 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/streams/streams.py
--rw-r--r--   0        0        0      987 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/synchronized.py
--rw-r--r--   0        0        0       64 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/utils/__init__.py
--rw-r--r--   0        0        0      587 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/utils/objectutils.py
--rw-r--r--   0        0        0      119 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/base/utils/utils.py
--rw-r--r--   0        0        0        0 2023-06-11 13:47:56.611003 pycommons_base-0.0.3/pycommons/py.typed
--rw-r--r--   0        0        0     1828 2023-06-11 13:48:08.539059 pycommons_base-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 pycommons_base-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1082 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/README.md
+-rw-r--r--   0        0        0      431 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/__init__.py
+-rw-r--r--   0        0        0      431 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/atomic/__init__.py
+-rw-r--r--   0        0        0      759 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/atomic/atomic.py
+-rw-r--r--   0        0        0      768 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/atomic/boolean.py
+-rw-r--r--   0        0        0     1791 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/atomic/integer.py
+-rw-r--r--   0        0        0     5648 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/char.py
+-rw-r--r--   0        0        0      235 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/container/__init__.py
+-rw-r--r--   0        0        0      813 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/container/boolean.py
+-rw-r--r--   0        0        0      849 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/container/container.py
+-rw-r--r--   0        0        0     1469 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/container/integer.py
+-rw-r--r--   0        0        0     4457 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/container/optional.py
+-rw-r--r--   0        0        0       88 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/exception/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/exception/no_such_element_error.py
+-rw-r--r--   0        0        0      320 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/function/__init__.py
+-rw-r--r--   0        0        0     1266 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/function/comparator.py
+-rw-r--r--   0        0        0     1454 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/function/consumer.py
+-rw-r--r--   0        0        0      594 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/function/function.py
+-rw-r--r--   0        0        0     2249 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/function/predicate.py
+-rw-r--r--   0        0        0      496 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/function/runnable.py
+-rw-r--r--   0        0        0      532 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/function/supplier.py
+-rw-r--r--   0        0        0      144 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/streams/__init__.py
+-rw-r--r--   0        0        0     6823 2023-06-11 14:01:01.425839 pycommons_base-0.0.4/pycommons/base/streams/iterator.py
+-rw-r--r--   0        0        0     2264 2023-06-11 14:01:01.429839 pycommons_base-0.0.4/pycommons/base/streams/stream.py
+-rw-r--r--   0        0        0      725 2023-06-11 14:01:01.429839 pycommons_base-0.0.4/pycommons/base/streams/streams.py
+-rw-r--r--   0        0        0      987 2023-06-11 14:01:01.429839 pycommons_base-0.0.4/pycommons/base/synchronized.py
+-rw-r--r--   0        0        0       64 2023-06-11 14:01:01.429839 pycommons_base-0.0.4/pycommons/base/utils/__init__.py
+-rw-r--r--   0        0        0      587 2023-06-11 14:01:01.429839 pycommons_base-0.0.4/pycommons/base/utils/objectutils.py
+-rw-r--r--   0        0        0      119 2023-06-11 14:01:01.429839 pycommons_base-0.0.4/pycommons/base/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:01:01.429839 pycommons_base-0.0.4/pycommons/py.typed
+-rw-r--r--   0        0        0     1828 2023-06-11 14:01:15.094015 pycommons_base-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 pycommons_base-0.0.4/PKG-INFO
```

### Comparing `pycommons_base-0.0.3/LICENSE` & `pycommons_base-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/README.md` & `pycommons_base-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/atomic/atomic.py` & `pycommons_base-0.0.4/pycommons/base/atomic/atomic.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/atomic/boolean.py` & `pycommons_base-0.0.4/pycommons/base/atomic/boolean.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/atomic/integer.py` & `pycommons_base-0.0.4/pycommons/base/atomic/integer.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/char.py` & `pycommons_base-0.0.4/pycommons/base/char.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/container/boolean.py` & `pycommons_base-0.0.4/pycommons/base/container/boolean.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/container/container.py` & `pycommons_base-0.0.4/pycommons/base/container/container.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/container/integer.py` & `pycommons_base-0.0.4/pycommons/base/container/integer.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/container/optional.py` & `pycommons_base-0.0.4/pycommons/base/container/optional.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/function/comparator.py` & `pycommons_base-0.0.4/pycommons/base/function/comparator.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/function/consumer.py` & `pycommons_base-0.0.4/pycommons/base/function/consumer.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/function/function.py` & `pycommons_base-0.0.4/pycommons/base/function/function.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/function/predicate.py` & `pycommons_base-0.0.4/pycommons/base/function/predicate.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/function/supplier.py` & `pycommons_base-0.0.4/pycommons/base/function/supplier.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/streams/iterator.py` & `pycommons_base-0.0.4/pycommons/base/streams/iterator.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/streams/stream.py` & `pycommons_base-0.0.4/pycommons/base/streams/stream.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/streams/streams.py` & `pycommons_base-0.0.4/pycommons/base/streams/streams.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/synchronized.py` & `pycommons_base-0.0.4/pycommons/base/synchronized.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pycommons/base/utils/objectutils.py` & `pycommons_base-0.0.4/pycommons/base/utils/objectutils.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.3/pyproject.toml` & `pycommons_base-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool]
 
 [tool.poetry]
 name = "pycommons.base"
-version = "0.0.3"
+version = "0.0.4"
 homepage = "https://github.com/shashankrnr32/pycommons-base"
 description = "Python Commons Base"
 authors = ["Shashank Sharma <shashankrnr32@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `pycommons_base-0.0.3/PKG-INFO` & `pycommons_base-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycommons-base
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Commons Base
 Home-page: https://github.com/shashankrnr32/pycommons-base
 License: Apache-2.0
 Author: Shashank Sharma
 Author-email: shashankrnr32@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

