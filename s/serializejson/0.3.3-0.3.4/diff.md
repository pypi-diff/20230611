# Comparing `tmp/serializejson-0.3.3.tar.gz` & `tmp/serializejson-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializejson-0.3.3.tar", last modified: Sun Jun 11 21:05:38 2023, max compression
+gzip compressed data, was "serializejson-0.3.4.tar", last modified: Sun Jun 11 21:15:16 2023, max compression
```

## Comparing `serializejson-0.3.3.tar` & `serializejson-0.3.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-11 21:04:58.000000 serializejson-0.3.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-11 21:04:58.000000 serializejson-0.3.3/LICENSE-APACHE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-11 21:04:58.000000 serializejson-0.3.3/LICENSE-PATRON.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-11 21:04:58.000000 serializejson-0.3.3/LICENSE-PROSPERITY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-11 21:04:58.000000 serializejson-0.3.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-11 21:05:38.620777 serializejson-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-06-11 21:04:58.000000 serializejson-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.616777 serializejson-0.3.3/SmartFramework/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.616777 serializejson-0.3.3/SmartFramework/files/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.616777 serializejson-0.3.3/SmartFramework/image/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/image/image_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/SmartFramework/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/serialize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/SmartFramework/string/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/string/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/SmartFramework/string/encodings/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/string/encodings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/string/encodings/ascii_printables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/SmartFramework/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/tools/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/tools/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/tools/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 21:04:58.000000 serializejson-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.616777 serializejson-0.3.3/rapidjson/
--rw-r--r--   0 runner    (1001) docker     (123)   133923 2023-06-11 21:04:58.000000 serializejson-0.3.3/rapidjson/rapidjson.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/serializejson/
--rw-r--r--   0 runner    (1001) docker     (123)   105036 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/serializejson/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/module_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/pickle_PyQt5_PySide2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31233 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_PyQt5_PySide2.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/serialize_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/simple_exemple.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/simple_exemple_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    57616 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/serializejson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-11 21:05:38.620777 serializejson-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-11 21:04:58.000000 serializejson-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-11 21:04:58.000000 serializejson-0.3.3/tests/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23679 2023-06-11 21:04:58.000000 serializejson-0.3.3/tests/test_serialize_vs_pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-11 21:14:36.000000 serializejson-0.3.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-11 21:14:36.000000 serializejson-0.3.4/LICENSE-APACHE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-11 21:14:36.000000 serializejson-0.3.4/LICENSE-PATRON.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-11 21:14:36.000000 serializejson-0.3.4/LICENSE-PROSPERITY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-11 21:14:36.000000 serializejson-0.3.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-06-11 21:15:16.462173 serializejson-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-06-11 21:14:36.000000 serializejson-0.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/SmartFramework/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/SmartFramework/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/SmartFramework/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/image/image_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/SmartFramework/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/serialize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/SmartFramework/string/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/string/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/SmartFramework/string/encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/string/encodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/string/encodings/ascii_printables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/SmartFramework/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/tools/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/tools/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-06-11 21:14:36.000000 serializejson-0.3.4/SmartFramework/tools/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 21:14:36.000000 serializejson-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.454173 serializejson-0.3.4/rapidjson/
+-rw-r--r--   0 runner    (1001) docker     (123)   133923 2023-06-11 21:14:36.000000 serializejson-0.3.4/rapidjson/rapidjson.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/serializejson/
+-rw-r--r--   0 runner    (1001) docker     (123)   105036 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/serializejson/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/plugins/module_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/plugins/pickle_PyQt5_PySide2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31233 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/plugins/serializejson_PyQt5_PySide2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/plugins/serializejson_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/plugins/serializejson_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/plugins/serializejson_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/plugins/serializejson_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/serialize_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/simple_exemple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/simple_exemple_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57616 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/serializejson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-06-11 21:15:16.000000 serializejson-0.3.4/serializejson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-11 21:15:16.000000 serializejson-0.3.4/serializejson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:15:16.000000 serializejson-0.3.4/serializejson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:14:36.000000 serializejson-0.3.4/serializejson.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 21:15:16.000000 serializejson-0.3.4/serializejson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-11 21:15:16.000000 serializejson-0.3.4/serializejson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-11 21:15:16.462173 serializejson-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-11 21:14:36.000000 serializejson-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:15:16.458173 serializejson-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-11 21:14:36.000000 serializejson-0.3.4/tests/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23679 2023-06-11 21:14:36.000000 serializejson-0.3.4/tests/test_serialize_vs_pickle.py
```

### Comparing `serializejson-0.3.3/CHANGELOG.rst` & `serializejson-0.3.4/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Version 0.3.4
+-------------
+:Date: 2023-06-11
+
+* Restore ducumentation
+
+
 Version 0.3.3
 -------------
 :Date: 2022-10-18
 
 * Big speed improvement for bytes and numpy array serialization
 
 Version 0.3.2
@@ -32,8 +39,8 @@
 -------------
 :Date: 2020-11-24
 	
 * API changed
 * add plugins support
 * add bytes, bytearray and numpy.array compression with blosc zstd
 * fix itertive append and decode (not fully tested).
-* fix dump of numpy types without conversion to python types(not yet numpy.float64)
+* fix dump of numpy types without conversion to python types(not yet numpy.float64)
```

### Comparing `serializejson-0.3.3/LICENSE-APACHE.rst` & `serializejson-0.3.4/LICENSE-APACHE.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/LICENSE-PATRON.rst` & `serializejson-0.3.4/LICENSE-PATRON.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/LICENSE-PROSPERITY.rst` & `serializejson-0.3.4/LICENSE-PROSPERITY.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/LICENSE.rst` & `serializejson-0.3.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/PKG-INFO` & `serializejson-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serializejson
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python library for fast serialization and deserialization of complex Python objects into JSON.
 Home-page: https://github.com/SmartAudioTools/serializejson
 Download-URL: https://github.com/SmartAudioTools/serializejson/tarball/master
 Author: Baptiste de La Gorce
 Author-email: baptiste.delagorce@smartaudiotools.com
 License: Prosperity Public License 3.0.0 and Patron License 1.0.0
 Project-URL: Documentation, https://smartaudiotools.github.io/serializejson
@@ -193,14 +193,21 @@
 For non limited commercial use, this project is licensed under the `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_.
 To acquire a license please `contact me <mailto:contact@smartaudiotools.com>`_, or just `sponsor me on GitHub <https://github.com/sponsors/SmartAudioTools>`_ under the appropriate tier ! This funding model helps me making my work sustainable and compensates me for the work it took to write this crate!
 
 Third-party contributions are licensed under `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_ and belong to their respective authors.
 History
 =======
 
+Version 0.3.4
+-------------
+:Date: 2023-06-11
+
+* Restore ducumentation
+
+
 Version 0.3.3
 -------------
 :Date: 2022-10-18
 
 * Big speed improvement for bytes and numpy array serialization
 
 Version 0.3.2
```

### Comparing `serializejson-0.3.3/README.rst` & `serializejson-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/SmartFramework/files/__init__.py` & `serializejson-0.3.4/SmartFramework/files/__init__.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/SmartFramework/image/image_conversion.py` & `serializejson-0.3.4/SmartFramework/image/image_conversion.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/SmartFramework/string/encodings/ascii_printables.py` & `serializejson-0.3.4/SmartFramework/string/encodings/ascii_printables.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/SmartFramework/tools/dictionaries.py` & `serializejson-0.3.4/SmartFramework/tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/SmartFramework/tools/objects.py` & `serializejson-0.3.4/SmartFramework/tools/objects.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/rapidjson/rapidjson.cpp` & `serializejson-0.3.4/rapidjson/rapidjson.cpp`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/__init__.py` & `serializejson-0.3.4/serializejson/__init__.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/plugins/module_name.py` & `serializejson-0.3.4/serializejson/plugins/module_name.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/plugins/pickle_PyQt5_PySide2.py` & `serializejson-0.3.4/serializejson/plugins/pickle_PyQt5_PySide2.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/plugins/serializejson_PyQt5_PySide2.py` & `serializejson-0.3.4/serializejson/plugins/serializejson_PyQt5_PySide2.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/plugins/serializejson_array.py` & `serializejson-0.3.4/serializejson/plugins/serializejson_array.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/plugins/serializejson_builtins.py` & `serializejson-0.3.4/serializejson/plugins/serializejson_builtins.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/plugins/serializejson_datetime.py` & `serializejson-0.3.4/serializejson/plugins/serializejson_datetime.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/plugins/serializejson_numpy.py` & `serializejson-0.3.4/serializejson/plugins/serializejson_numpy.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/serialize_parameters.py` & `serializejson-0.3.4/serializejson/serialize_parameters.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/simple_exemple_update.py` & `serializejson-0.3.4/serializejson/simple_exemple_update.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson/tools.py` & `serializejson-0.3.4/serializejson/tools.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/serializejson.egg-info/PKG-INFO` & `serializejson-0.3.4/serializejson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serializejson
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python library for fast serialization and deserialization of complex Python objects into JSON.
 Home-page: https://github.com/SmartAudioTools/serializejson
 Download-URL: https://github.com/SmartAudioTools/serializejson/tarball/master
 Author: Baptiste de La Gorce
 Author-email: baptiste.delagorce@smartaudiotools.com
 License: Prosperity Public License 3.0.0 and Patron License 1.0.0
 Project-URL: Documentation, https://smartaudiotools.github.io/serializejson
@@ -193,14 +193,21 @@
 For non limited commercial use, this project is licensed under the `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_.
 To acquire a license please `contact me <mailto:contact@smartaudiotools.com>`_, or just `sponsor me on GitHub <https://github.com/sponsors/SmartAudioTools>`_ under the appropriate tier ! This funding model helps me making my work sustainable and compensates me for the work it took to write this crate!
 
 Third-party contributions are licensed under `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_ and belong to their respective authors.
 History
 =======
 
+Version 0.3.4
+-------------
+:Date: 2023-06-11
+
+* Restore ducumentation
+
+
 Version 0.3.3
 -------------
 :Date: 2022-10-18
 
 * Big speed improvement for bytes and numpy array serialization
 
 Version 0.3.2
```

### Comparing `serializejson-0.3.3/serializejson.egg-info/SOURCES.txt` & `serializejson-0.3.4/serializejson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/setup.py` & `serializejson-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/tests/test_iterator.py` & `serializejson-0.3.4/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.3/tests/test_serialize_vs_pickle.py` & `serializejson-0.3.4/tests/test_serialize_vs_pickle.py`

 * *Files identical despite different names*

