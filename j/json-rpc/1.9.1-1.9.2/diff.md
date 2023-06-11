# Comparing `tmp/json-rpc-1.9.1.tar.gz` & `tmp/json-rpc-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-rpc-1.9.1.tar", last modified: Tue May  5 08:20:00 2015, max compression
+gzip compressed data, was "dist/json-rpc-1.9.2.tar", last modified: Tue Jun  2 16:54:24 2015, max compression
```

## Comparing `json-rpc-1.9.1.tar` & `json-rpc-1.9.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 pavlov99   (503) staff       (20)        0 2015-05-05 08:20:00.000000 json-rpc-1.9.1/
-drwxr-xr-x   0 pavlov99   (503) staff       (20)        0 2015-05-05 08:20:00.000000 json-rpc-1.9.1/json_rpc.egg-info/
--rw-r--r--   0 pavlov99   (503) staff       (20)        1 2015-05-05 08:19:59.000000 json-rpc-1.9.1/json_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 pavlov99   (503) staff       (20)     5186 2015-05-05 08:19:59.000000 json-rpc-1.9.1/json_rpc.egg-info/PKG-INFO
--rw-r--r--   0 pavlov99   (503) staff       (20)      884 2015-05-05 08:19:59.000000 json-rpc-1.9.1/json_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 pavlov99   (503) staff       (20)        8 2015-05-05 08:19:59.000000 json-rpc-1.9.1/json_rpc.egg-info/top_level.txt
-drwxr-xr-x   0 pavlov99   (503) staff       (20)        0 2015-05-05 08:20:00.000000 json-rpc-1.9.1/jsonrpc/
--rw-r--r--   0 pavlov99   (503) staff       (20)      244 2015-05-05 08:18:49.000000 json-rpc-1.9.1/jsonrpc/__init__.py
-drwxr-xr-x   0 pavlov99   (503) staff       (20)        0 2015-05-05 08:20:00.000000 json-rpc-1.9.1/jsonrpc/backend/
--rw-r--r--   0 pavlov99   (503) staff       (20)        0 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/backend/__init__.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     2395 2015-05-05 08:18:37.000000 json-rpc-1.9.1/jsonrpc/backend/django.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     1842 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/base.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     2693 2015-05-05 08:11:35.000000 json-rpc-1.9.1/jsonrpc/dispatcher.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     4292 2015-05-05 08:11:35.000000 json-rpc-1.9.1/jsonrpc/exceptions.py
--rw-r--r--   0 pavlov99   (503) staff       (20)      698 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/jsonrpc.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     4211 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/jsonrpc1.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     8412 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/jsonrpc2.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     4156 2015-05-05 08:16:04.000000 json-rpc-1.9.1/jsonrpc/manager.py
--rw-r--r--   0 pavlov99   (503) staff       (20)    21078 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/six.py
-drwxr-xr-x   0 pavlov99   (503) staff       (20)        0 2015-05-05 08:20:00.000000 json-rpc-1.9.1/jsonrpc/tests/
--rw-r--r--   0 pavlov99   (503) staff       (20)        0 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/__init__.py
-drwxr-xr-x   0 pavlov99   (503) staff       (20)        0 2015-05-05 08:20:00.000000 json-rpc-1.9.1/jsonrpc/tests/test_backend_django/
--rw-r--r--   0 pavlov99   (503) staff       (20)        0 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_backend_django/__init__.py
--rw-r--r--   0 pavlov99   (503) staff       (20)      271 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_backend_django/settings.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     2297 2015-03-20 03:23:26.000000 json-rpc-1.9.1/jsonrpc/tests/test_backend_django/tests.py
--rw-r--r--   0 pavlov99   (503) staff       (20)      198 2015-03-20 03:23:26.000000 json-rpc-1.9.1/jsonrpc/tests/test_backend_django/urls.py
--rw-r--r--   0 pavlov99   (503) staff       (20)      935 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_base.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     1957 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_dispatcher.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     6869 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_examples20.py
--rw-r--r--   0 pavlov99   (503) staff       (20)       38 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_jsonrpc.py
--rw-r--r--   0 pavlov99   (503) staff       (20)    13518 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_jsonrpc1.py
--rw-r--r--   0 pavlov99   (503) staff       (20)    23425 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_jsonrpc2.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     4639 2015-03-19 09:57:18.000000 json-rpc-1.9.1/jsonrpc/tests/test_jsonrpc_errors.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     8049 2015-03-24 02:24:13.000000 json-rpc-1.9.1/jsonrpc/tests/test_manager.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     3230 2015-03-24 02:24:13.000000 json-rpc-1.9.1/jsonrpc/tests/test_utils.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     2110 2015-03-24 02:24:13.000000 json-rpc-1.9.1/jsonrpc/utils.py
--rw-r--r--   0 pavlov99   (503) staff       (20)     5186 2015-05-05 08:20:00.000000 json-rpc-1.9.1/PKG-INFO
--rw-r--r--   0 pavlov99   (503) staff       (20)     3373 2015-03-20 03:31:50.000000 json-rpc-1.9.1/README.rst
--rw-r--r--   0 pavlov99   (503) staff       (20)       88 2015-05-05 08:20:00.000000 json-rpc-1.9.1/setup.cfg
--rw-r--r--   0 pavlov99   (503) staff       (20)     1734 2015-03-19 09:57:18.000000 json-rpc-1.9.1/setup.py
+drwxrwxr-x   0 pavlov99  (1000) pavlov99  (1000)        0 2015-06-02 16:54:24.000000 json-rpc-1.9.2/
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     1734 2015-03-05 01:59:34.000000 json-rpc-1.9.2/setup.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     3610 2015-06-02 16:48:47.000000 json-rpc-1.9.2/README.rst
+drwxrwxr-x   0 pavlov99  (1000) pavlov99  (1000)        0 2015-06-02 16:54:24.000000 json-rpc-1.9.2/jsonrpc/
+drwxrwxr-x   0 pavlov99  (1000) pavlov99  (1000)        0 2015-06-02 16:54:24.000000 json-rpc-1.9.2/jsonrpc/tests/
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)    13518 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/tests/test_jsonrpc1.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     4639 2014-09-04 01:11:38.000000 json-rpc-1.9.2/jsonrpc/tests/test_jsonrpc_errors.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     8049 2015-03-28 03:37:28.000000 json-rpc-1.9.2/jsonrpc/tests/test_manager.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     6869 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/tests/test_examples20.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)        0 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/tests/__init__.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)    23425 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/tests/test_jsonrpc2.py
+drwxrwxr-x   0 pavlov99  (1000) pavlov99  (1000)        0 2015-06-02 16:54:24.000000 json-rpc-1.9.2/jsonrpc/tests/test_backend_django/
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)      271 2015-03-03 13:26:08.000000 json-rpc-1.9.2/jsonrpc/tests/test_backend_django/settings.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)      198 2015-03-28 03:37:28.000000 json-rpc-1.9.2/jsonrpc/tests/test_backend_django/urls.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)        0 2015-03-03 13:23:37.000000 json-rpc-1.9.2/jsonrpc/tests/test_backend_django/__init__.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     2297 2015-03-28 03:37:28.000000 json-rpc-1.9.2/jsonrpc/tests/test_backend_django/tests.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     3230 2015-03-28 03:37:28.000000 json-rpc-1.9.2/jsonrpc/tests/test_utils.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     2793 2015-06-02 16:53:37.000000 json-rpc-1.9.2/jsonrpc/tests/test_dispatcher.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)      935 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/tests/test_base.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)       38 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/tests/test_jsonrpc.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     3156 2015-06-02 16:53:37.000000 json-rpc-1.9.2/jsonrpc/dispatcher.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     2110 2015-03-28 03:37:28.000000 json-rpc-1.9.2/jsonrpc/utils.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     4292 2015-03-29 14:35:50.000000 json-rpc-1.9.2/jsonrpc/exceptions.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     1842 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/base.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     4211 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/jsonrpc1.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)      244 2015-06-02 16:53:46.000000 json-rpc-1.9.2/jsonrpc/__init__.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)      698 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/jsonrpc.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     4156 2015-03-28 03:37:28.000000 json-rpc-1.9.2/jsonrpc/manager.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)    21078 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/six.py
+drwxrwxr-x   0 pavlov99  (1000) pavlov99  (1000)        0 2015-06-02 16:54:24.000000 json-rpc-1.9.2/jsonrpc/backend/
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     2395 2015-06-02 16:48:47.000000 json-rpc-1.9.2/jsonrpc/backend/django.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)        0 2015-03-03 13:23:37.000000 json-rpc-1.9.2/jsonrpc/backend/__init__.py
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     8412 2014-09-03 12:50:23.000000 json-rpc-1.9.2/jsonrpc/jsonrpc2.py
+drwxrwxr-x   0 pavlov99  (1000) pavlov99  (1000)        0 2015-06-02 16:54:24.000000 json-rpc-1.9.2/json_rpc.egg-info/
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)        8 2015-06-02 16:54:23.000000 json-rpc-1.9.2/json_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)        1 2015-06-02 16:54:23.000000 json-rpc-1.9.2/json_rpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)      884 2015-06-02 16:54:23.000000 json-rpc-1.9.2/json_rpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     5455 2015-06-02 16:54:23.000000 json-rpc-1.9.2/json_rpc.egg-info/PKG-INFO
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)     5455 2015-06-02 16:54:24.000000 json-rpc-1.9.2/PKG-INFO
+-rw-rw-r--   0 pavlov99  (1000) pavlov99  (1000)       88 2015-06-02 16:54:24.000000 json-rpc-1.9.2/setup.cfg
```

### Comparing `json-rpc-1.9.1/json_rpc.egg-info/PKG-INFO` & `json-rpc-1.9.2/json_rpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 1.1
 Name: json-rpc
-Version: 1.9.1
+Version: 1.9.2
 Summary: JSON-RPC transport realisation
 Home-page: https://github.com/pavlov99/json-rpc
 Author: Kirill Pavlov
 Author-email: kirill.pavlov@phystech.edu
 License: MIT
 Description: json-rpc
         ========
         
+        .. image:: https://badges.gitter.im/Join%20Chat.svg
+           :alt: Join the chat at https://gitter.im/pavlov99/json-rpc
+           :target: https://gitter.im/pavlov99/json-rpc?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        
         .. image:: https://travis-ci.org/pavlov99/json-rpc.png
             :target: https://travis-ci.org/pavlov99/json-rpc
             :alt: Build Status
         
         .. image:: https://coveralls.io/repos/pavlov99/json-rpc/badge.png
             :target: https://coveralls.io/r/pavlov99/json-rpc
             :alt: Coverage Status
```

### Comparing `json-rpc-1.9.1/json_rpc.egg-info/SOURCES.txt` & `json-rpc-1.9.2/json_rpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/backend/django.py` & `json-rpc-1.9.2/jsonrpc/backend/django.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/base.py` & `json-rpc-1.9.2/jsonrpc/base.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/dispatcher.py` & `json-rpc-1.9.2/jsonrpc/dispatcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,14 +46,27 @@
 
     def __iter__(self):
         return iter(self.method_map)
 
     def __repr__(self):
         return repr(self.method_map)
 
+    def add_class(self, cls):
+        prefix = cls.__name__.lower() + '.'
+        self.build_method_map(cls(), prefix)
+
+    def add_object(self, obj):
+        prefix = obj.__class__.__name__.lower() + '.'
+        self.build_method_map(obj, prefix)
+
+    def add_dict(self, dict, prefix=''):
+        if prefix:
+            prefix += '.'
+        self.build_method_map(dict, prefix)
+
     def add_method(self, f, name=None):
         """ Add a method to the dispatcher.
 
         Parameters
         ----------
         f : callable
             Callable to be added.
@@ -80,28 +93,30 @@
             def mymethod(*args, **kwargs):
                 print(args, kwargs)
 
         """
         self.method_map[name or f.__name__] = f
         return f
 
-    def build_method_map(self, prototype):
+    def build_method_map(self, prototype, prefix=''):
         """ Add prototype methods to the dispatcher.
 
         Parameters
         ----------
         prototype : object or dict
             Initial method mapping.
             If given prototype is a dictionary then all callable objects will
             be added to dispatcher.
             If given prototype is an object then all public methods will
             be used.
+        prefix: string, optional
+            Prefix of methods
 
         """
         if not isinstance(prototype, dict):
             prototype = dict((method, getattr(prototype, method))
                              for method in dir(prototype)
                              if not method.startswith('_'))
 
         for attr, method in prototype.items():
             if callable(method):
-                self[attr] = method
+                self[prefix + attr] = method
```

### Comparing `json-rpc-1.9.1/jsonrpc/exceptions.py` & `json-rpc-1.9.2/jsonrpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/jsonrpc.py` & `json-rpc-1.9.2/jsonrpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/jsonrpc1.py` & `json-rpc-1.9.2/jsonrpc/jsonrpc1.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/jsonrpc2.py` & `json-rpc-1.9.2/jsonrpc/jsonrpc2.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/manager.py` & `json-rpc-1.9.2/jsonrpc/manager.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/six.py` & `json-rpc-1.9.2/jsonrpc/six.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_backend_django/tests.py` & `json-rpc-1.9.2/jsonrpc/tests/test_backend_django/tests.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_base.py` & `json-rpc-1.9.2/jsonrpc/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_dispatcher.py` & `json-rpc-1.9.2/jsonrpc/tests/test_dispatcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 import sys
 if sys.version_info < (2, 7):
     import unittest2 as unittest
 else:
     import unittest
 
 
+class Math:
+
+    def sum(self, a, b):
+        return a + b
+
+    def diff(self, a, b):
+        return a - b
+
+
 class TestDispatcher(unittest.TestCase):
 
     """ Test Dispatcher functionality."""
 
     def test_getter(self):
         d = Dispatcher()
 
@@ -30,14 +39,39 @@
         @d.add_method
         def add(x, y):
             return x + y
 
         self.assertIn("add", d)
         self.assertEqual(d["add"](1, 1), 2)
 
+    def test_add_class(self):
+        d = Dispatcher()
+        d.add_class(Math)
+
+        self.assertIn("math.sum", d)
+        self.assertIn("math.diff", d)
+        self.assertEqual(d["math.sum"](3, 8), 11)
+        self.assertEqual(d["math.diff"](6, 9), -3)
+
+    def test_add_object(self):
+        d = Dispatcher()
+        d.add_object(Math())
+
+        self.assertIn("math.sum", d)
+        self.assertIn("math.diff", d)
+        self.assertEqual(d["math.sum"](5, 2), 7)
+        self.assertEqual(d["math.diff"](15, 9), 6)
+
+    def test_add_dict(self):
+        d = Dispatcher()
+        d.add_dict({"sum": lambda *args: sum(args)}, "util")
+
+        self.assertIn("util.sum", d)
+        self.assertEqual(d["util.sum"](13, -2), 11)
+
     def test_add_method_keep_function_definitions(self):
 
         d = Dispatcher()
 
         @d.add_method
         def one(x):
             return x
```

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_examples20.py` & `json-rpc-1.9.2/jsonrpc/tests/test_examples20.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_jsonrpc1.py` & `json-rpc-1.9.2/jsonrpc/tests/test_jsonrpc1.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_jsonrpc2.py` & `json-rpc-1.9.2/jsonrpc/tests/test_jsonrpc2.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_jsonrpc_errors.py` & `json-rpc-1.9.2/jsonrpc/tests/test_jsonrpc_errors.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_manager.py` & `json-rpc-1.9.2/jsonrpc/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/tests/test_utils.py` & `json-rpc-1.9.2/jsonrpc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/jsonrpc/utils.py` & `json-rpc-1.9.2/jsonrpc/utils.py`

 * *Files identical despite different names*

### Comparing `json-rpc-1.9.1/PKG-INFO` & `json-rpc-1.9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 1.1
 Name: json-rpc
-Version: 1.9.1
+Version: 1.9.2
 Summary: JSON-RPC transport realisation
 Home-page: https://github.com/pavlov99/json-rpc
 Author: Kirill Pavlov
 Author-email: kirill.pavlov@phystech.edu
 License: MIT
 Description: json-rpc
         ========
         
+        .. image:: https://badges.gitter.im/Join%20Chat.svg
+           :alt: Join the chat at https://gitter.im/pavlov99/json-rpc
+           :target: https://gitter.im/pavlov99/json-rpc?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        
         .. image:: https://travis-ci.org/pavlov99/json-rpc.png
             :target: https://travis-ci.org/pavlov99/json-rpc
             :alt: Build Status
         
         .. image:: https://coveralls.io/repos/pavlov99/json-rpc/badge.png
             :target: https://coveralls.io/r/pavlov99/json-rpc
             :alt: Coverage Status
```

### Comparing `json-rpc-1.9.1/README.rst` & `json-rpc-1.9.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 json-rpc
 ========
 
+.. image:: https://badges.gitter.im/Join%20Chat.svg
+   :alt: Join the chat at https://gitter.im/pavlov99/json-rpc
+   :target: https://gitter.im/pavlov99/json-rpc?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+
 .. image:: https://travis-ci.org/pavlov99/json-rpc.png
     :target: https://travis-ci.org/pavlov99/json-rpc
     :alt: Build Status
 
 .. image:: https://coveralls.io/repos/pavlov99/json-rpc/badge.png
     :target: https://coveralls.io/r/pavlov99/json-rpc
     :alt: Coverage Status
```

### Comparing `json-rpc-1.9.1/setup.py` & `json-rpc-1.9.2/setup.py`

 * *Files identical despite different names*

