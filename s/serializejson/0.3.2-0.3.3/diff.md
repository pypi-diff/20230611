# Comparing `tmp/serializejson-0.3.2.tar.gz` & `tmp/serializejson-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializejson-0.3.2.tar", last modified: Sun Oct  2 09:57:30 2022, max compression
+gzip compressed data, was "serializejson-0.3.3.tar", last modified: Sun Jun 11 21:05:38 2023, max compression
```

## Comparing `serializejson-0.3.2.tar` & `serializejson-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.889913 serializejson-0.3.2/
--rw-rw-rw-   0        0        0      816 2022-10-02 09:53:50.000000 serializejson-0.3.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0      644 2020-11-26 19:10:22.000000 serializejson-0.3.2/LICENSE-APACHE.rst
--rw-rw-rw-   0        0        0     3563 2020-11-26 19:31:52.000000 serializejson-0.3.2/LICENSE-PATRON.rst
--rw-rw-rw-   0        0        0     3154 2020-11-28 09:47:57.000000 serializejson-0.3.2/LICENSE-PROSPERITY.rst
--rw-rw-rw-   0        0        0      984 2020-11-27 12:27:20.000000 serializejson-0.3.2/LICENSE.rst
--rw-rw-rw-   0        0        0    12548 2022-10-02 09:57:30.889913 serializejson-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    10286 2022-10-02 09:17:56.000000 serializejson-0.3.2/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.809913 serializejson-0.3.2/SmartFramework/
--rw-rw-rw-   0        0        0        3 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.809913 serializejson-0.3.2/SmartFramework/files/
--rw-rw-rw-   0        0        0      929 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/files/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.819913 serializejson-0.3.2/SmartFramework/image/
--rw-rw-rw-   0        0        0        3 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/image/__init__.py
--rw-rw-rw-   0        0        0     5729 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/image/image_conversion.py
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.829913 serializejson-0.3.2/SmartFramework/serialize/
--rw-rw-rw-   0        0        0      284 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/serialize/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.829913 serializejson-0.3.2/SmartFramework/string/
--rw-rw-rw-   0        0        0        3 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/string/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.839913 serializejson-0.3.2/SmartFramework/string/encodings/
--rw-rw-rw-   0        0        0        3 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/string/encodings/__init__.py
--rw-rw-rw-   0        0        0    12750 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/string/encodings/ascii_printables.py
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.849913 serializejson-0.3.2/SmartFramework/tools/
--rw-rw-rw-   0        0        0        3 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/tools/__init__.py
--rw-rw-rw-   0        0        0     4636 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/tools/dictionaries.py
--rw-rw-rw-   0        0        0      385 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/tools/functions.py
--rw-rw-rw-   0        0        0     9700 2021-04-22 15:04:18.000000 serializejson-0.3.2/SmartFramework/tools/objects.py
--rw-rw-rw-   0        0        0       89 2020-11-26 19:10:22.000000 serializejson-0.3.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.869913 serializejson-0.3.2/serializejson/
--rw-rw-rw-   0        0        0   104751 2022-10-02 09:52:29.000000 serializejson-0.3.2/serializejson/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.889913 serializejson-0.3.2/serializejson/plugins/
--rw-rw-rw-   0        0        0      283 2021-04-22 15:04:24.000000 serializejson-0.3.2/serializejson/plugins/__init__.py
--rw-rw-rw-   0        0        0     1814 2021-04-22 15:04:24.000000 serializejson-0.3.2/serializejson/plugins/module_name.py
--rw-rw-rw-   0        0        0     3011 2021-04-22 15:04:24.000000 serializejson-0.3.2/serializejson/plugins/pickle_PyQt5_PySide2.py
--rw-rw-rw-   0        0        0    31233 2022-09-28 22:11:59.000000 serializejson-0.3.2/serializejson/plugins/serializejson_PyQt5_PySide2.py
--rw-rw-rw-   0        0        0      968 2021-04-22 15:04:24.000000 serializejson-0.3.2/serializejson/plugins/serializejson_array.py
--rw-rw-rw-   0        0        0     4453 2022-09-28 18:40:55.000000 serializejson-0.3.2/serializejson/plugins/serializejson_builtins.py
--rw-rw-rw-   0        0        0      741 2022-09-28 18:41:05.000000 serializejson-0.3.2/serializejson/plugins/serializejson_datetime.py
--rw-rw-rw-   0        0        0     9802 2022-09-30 06:32:52.000000 serializejson-0.3.2/serializejson/plugins/serializejson_numpy.py
--rw-rw-rw-   0        0        0     5030 2021-04-22 15:04:24.000000 serializejson-0.3.2/serializejson/serialize_parameters.py
--rw-rw-rw-   0        0        0      417 2021-04-22 15:04:24.000000 serializejson-0.3.2/serializejson/simple_exemple.py
--rw-rw-rw-   0        0        0      832 2021-04-22 15:04:24.000000 serializejson-0.3.2/serializejson/simple_exemple_update.py
--rw-rw-rw-   0        0        0    57504 2022-10-01 01:38:24.000000 serializejson-0.3.2/serializejson/tools.py
-drwxrwxrwx   0        0        0        0 2022-10-02 09:57:30.889913 serializejson-0.3.2/serializejson.egg-info/
--rw-rw-rw-   0        0        0    12548 2022-10-02 09:57:30.000000 serializejson-0.3.2/serializejson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1302 2022-10-02 09:57:30.000000 serializejson-0.3.2/serializejson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-02 09:57:30.000000 serializejson-0.3.2/serializejson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-11-28 09:44:08.000000 serializejson-0.3.2/serializejson.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      148 2022-10-02 09:57:30.000000 serializejson-0.3.2/serializejson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2022-10-02 09:57:30.000000 serializejson-0.3.2/serializejson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      189 2022-10-02 09:57:30.899913 serializejson-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     3030 2022-10-02 09:41:17.000000 serializejson-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-11 21:04:58.000000 serializejson-0.3.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-11 21:04:58.000000 serializejson-0.3.3/LICENSE-APACHE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-11 21:04:58.000000 serializejson-0.3.3/LICENSE-PATRON.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-11 21:04:58.000000 serializejson-0.3.3/LICENSE-PROSPERITY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-11 21:04:58.000000 serializejson-0.3.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-11 21:05:38.620777 serializejson-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-06-11 21:04:58.000000 serializejson-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.616777 serializejson-0.3.3/SmartFramework/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.616777 serializejson-0.3.3/SmartFramework/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.616777 serializejson-0.3.3/SmartFramework/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/image/image_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/SmartFramework/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/serialize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/SmartFramework/string/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/string/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/SmartFramework/string/encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/string/encodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/string/encodings/ascii_printables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/SmartFramework/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/tools/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/tools/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-06-11 21:04:58.000000 serializejson-0.3.3/SmartFramework/tools/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 21:04:58.000000 serializejson-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.616777 serializejson-0.3.3/rapidjson/
+-rw-r--r--   0 runner    (1001) docker     (123)   133923 2023-06-11 21:04:58.000000 serializejson-0.3.3/rapidjson/rapidjson.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/serializejson/
+-rw-r--r--   0 runner    (1001) docker     (123)   105036 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/serializejson/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/module_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/pickle_PyQt5_PySide2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31233 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_PyQt5_PySide2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/plugins/serializejson_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/serialize_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/simple_exemple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/simple_exemple_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57616 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/serializejson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:04:58.000000 serializejson-0.3.3/serializejson.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-11 21:05:38.000000 serializejson-0.3.3/serializejson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-11 21:05:38.620777 serializejson-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-11 21:04:58.000000 serializejson-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:05:38.620777 serializejson-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-11 21:04:58.000000 serializejson-0.3.3/tests/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23679 2023-06-11 21:04:58.000000 serializejson-0.3.3/tests/test_serialize_vs_pickle.py
```

### Comparing `serializejson-0.3.2/CHANGELOG.rst` & `serializejson-0.3.3/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Version 0.3.3
+-------------
+:Date: 2022-10-18
+
+* Big speed improvement for bytes and numpy array serialization
+
 Version 0.3.2
 -------------
 :Date: 2022-10-01
 
 * API changed
 * add better support for cicular reférences and duplicates with {"$ref": ...}
```

### Comparing `serializejson-0.3.2/LICENSE-APACHE.rst` & `serializejson-0.3.3/LICENSE-APACHE.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/LICENSE-PATRON.rst` & `serializejson-0.3.3/LICENSE-PATRON.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/LICENSE-PROSPERITY.rst` & `serializejson-0.3.3/LICENSE-PROSPERITY.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/LICENSE.rst` & `serializejson-0.3.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/PKG-INFO` & `serializejson-0.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,233 +1,238 @@
-Metadata-Version: 2.1
-Name: serializejson
-Version: 0.3.2
-Summary: A python library for fast serialization and deserialization of complex Python objects into JSON.
-Home-page: https://github.com/SmartAudioTools/serializejson
-Author: Baptiste de La Gorce
-Author-email: baptiste.delagorce@smartaudiotools.com
-License: Prosperity Public License 3.0.0 and Patron License 1.0.0
-Download-URL: https://github.com/SmartAudioTools/serializejson/tarball/master
-Project-URL: Documentation, https://smartaudiotools.github.io/serializejson
-Project-URL: Funding, https://github.com/sponsors/SmartAudioTools
-Project-URL: Source, https://github.com/SmartAudioTools/serializejson
-Project-URL: Tracker, https://github.com/SmartAudioTools/serializejson/issues
-Keywords: pickle json serialize dump dumps rapidjson base64
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: Free for non-commercial use
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE-APACHE.rst
-License-File: LICENSE-PATRON.rst
-License-File: LICENSE-PROSPERITY.rst
-License-File: LICENSE.rst
-
-serializejson
-=============
-
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Authors**               | `Baptiste de La Gorce <contact@smartaudiotools.com>`_                                                                    |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **PyPI**                  | https://pypi.org/project/serializejson                                                                                   |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Documentation**         | https://smartaudiotools.github.io/serializejson                                                                          |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Sources**               | https://github.com/SmartAudioTools/serializejson                                                                         |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Issues**                | https://github.com/SmartAudioTools/serializejson/issues                                                                  |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Noncommercial license** | `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_ |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Commercial license**    | `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_                |
-|                           | `Sponsor me ! <https://github.com/sponsors/SmartAudioTools>`_ or `contact me ! <contact@smartaudiotools.com>`_           |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-
-
-**serializejson**  is a python library for fast serialization and deserialization
-of python objects in `JSON <http://json.org>`_  designed as a safe, interoperable and human-readable drop-in replacement for the Python `pickle <https://docs.python.org/3/library/pickle.html>`_ package.
-Complex python object hierarchies are serializable, deserializable or updatable in once, allowing for example to save or restore a complete application state in few lines of code.
-The library is build upon
-`python-rapidjson <https://github.com/python-rapidjson/python-rapidjson>`_,
-`pybase64 <https://github.com/mayeut/pybase64>`_ and
-`blosc <https://github.com/Blosc/python-blosc>`_  for optional `zstandard <https://github.com/facebook/zstd>`_ compression.
-
-Some of the main features:
-
-- supports Python 3.7 (maybe lower) or greater.
-- serializes arbitrary python objects into a dictionary by adding `__class__` ,and eventually `__init__`, `__new__`, `__state__`, `__items__` keys.
-- calls the same objects methods as pickle. Therefore almost all pickable objects are serializable with serializejson without any modification.
-- for not already pickable object, you will allways be able to serialize it by adding methodes to the object or creating plugins for pickle or serializejson.
-- generally 2x slower than pickle for dumping and 3x slower than pickle for loading (on your benchmark) except for big arrays (optimisation will soon be done).
-- serializes and deserializes bytes and bytearray very quickly in base64 thanks to `pybase64 <https://github.com/mayeut/pybase64>`_ and lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
-- serialize properties and attributes with getters and setters if wanted (unlike pickle).
-- json data will still be directly loadable if you have transform some attributes in slots or properties in your code since your last serialization. (unlike pickle)
-- can serialize `__init__(self,..)` arguments by name instead of positions, allowing to skip arguments with defauts values and making json datas robust to a change of `__init__` parameters order.
-- serialized objects take generally less space than when serialized with pickle: for binary data, the 30% increase due to base64 encoding is in general largely compensated using the lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
-- serialized objects are human-readable and easy to read. Unlike pickled data, your data will never become unreadable if your code evolves: you will always be able to modify your datas with a text editor (with find & replace for example if you change an attribut name).
-- serialized objects are text and therefore versionable and comparable with versionning and comparaison tools.
-- can safely load untrusted / unauthenticated sources if authorized_classes list parameter is set carefully with strictly necessary objects (unlike pickle).
-- can update existing objects recursively instead of override them. serializejson can be used to save and restore in place a complete application state (? not yet well tested).
-- filters attribute starting with "_" by default (unlike pickle). You can keep them if wanted with `filter_ = False`.
-- numpy arrays can be serialized as lists with automatic conversion in both ways or in a conservative way.
-- supports circular references and serialize only once duplicated objects, using "$ref" key an path to the first occurance in the json : `{"$ref": "root.xxx.elt"}` (? not yet if the object is a list or dictionary).
-- accepts json with comment (// and /\* \*/) if `accept_comments = True`.
-- can automatically recognize objects in json from keys names and recreate them, without the need of `__class__` key, if passed in `recognized_classes`.
-- serializejson is easly interoperable outside of the Python ecosystem with this recognition of objects from keys names or with `__class__` translation between python and other language classes.
-- dump and load support string path.
-- can iteratively encode (with append) and decode (with iterator) a list in json file, which helps saving memory space during the process of serialization and deserialization and useful for logs.
-
-.. warning::
-
-    **?** Do not load serializejson files from untrusted / unauthenticated sources without carefully setting the load authorized_classes parameter.
-
-    **?** Never dump a dictionary with the `__class__` key, otherwise serializejson will attempt to reconstruct an object when loading the json.
-    Be careful not to allow a user to manually enter a dictionary key somewhere without checking that it is not `__class__`.
-    Due to current limitation of rapidjson we cannot we cannot at the moment efficiently detect dictionaries with the `__class__` key to raise an error.
-
-
-Installation
-============
-
-**Last offical release**
-
-.. code-block::
-
-    pip install serializejson
-
-**Developpement version unreleased**
-
-.. code-block::
-
-    pip install git+https://github.com/SmartAudioTools/serializejson.git
-
-Examples
-================
-
-**Serialization with fonctions API**
-
-.. code-block:: python
-
-    import serializejson
-
-    #serialize in string
-    object1 = set([1,2])
-    dumped1 = serializejson.dumps(object1)
-    loaded1 = serializejson.loads(dumped1)
-    print(dumped1)
-    >{
-    >        "__class__": "set",
-    >        "__init__": [1,2]
-    >}
-
-
-    #serialize in file
-    object2 = set([3,4])
-    serializejson.dump(object2,"dumped2.json")
-    loaded2 = serializejson.load("dumped2.json")
-
-**Serialization with classes based API.**
-
-.. code-block:: python
-
-    import serializejson
-    encoder = serializejson.Encoder()
-    decoder = serializejson.Decoder()
-
-    # serialize in string
-
-    object1 = set([1,2])
-    dumped1 = encoder.dumps(object1)
-    loaded1 = decoder.loads(dumped1)
-    print(dumped1)
-
-    # serialize in file
-    object2 = set([3,4])
-    encoder.dump(object2,"dumped2.json")
-    loaded2 = decoder.load("dumped2.json")
-
-**Update existing object**
-
-.. code-block:: python
-
-    import serializejson
-    object1 = set([1,2])
-    object2 = set([3,4])
-    dumped1 = serializejson.dumps(object1)
-    print(f"id {id(object2)} :  {object2}")
-    serializejson.loads(dumped1,obj = object2, updatables_classes = [set])
-    print(f"id {id(object2)} :  {object2}")
-
-**Iterative serialization and deserialization**
-
-.. code-block:: python
-
-    import serializejson
-    encoder = serializejson.Encoder("my_list.json",indent = None)
-    for elt in range(3):
-        encoder.append(elt)
-    print(open("my_list.json").read())
-    for elt in serializejson.Decoder("my_list.json"):
-        print(elt)
-    >[0,1,2]
-    >0
-    >1
-    >2
-
-More examples and complete documentation `here <https://smartaudiotools.github.io/serializejson/>`_
-
-License
-=======
-
-Copyright 2020 Baptiste de La Gorce
-
-For noncommercial use or thirty-day limited free-trial period commercial use, this project is licensed under the `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_.
-
-For non limited commercial use, this project is licensed under the `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_.
-To acquire a license please `contact me <mailto:contact@smartaudiotools.com>`_, or just `sponsor me on GitHub <https://github.com/sponsors/SmartAudioTools>`_ under the appropriate tier ! This funding model helps me making my work sustainable and compensates me for the work it took to write this crate!
-
-Third-party contributions are licensed under `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_ and belong to their respective authors.
-
-History
-=======
-
-Version 0.3.2
--------------
-:Date: 2022-10-01
-
-* API changed
-* add better support for cicular refÃ©rences and duplicates with {"$ref": ...}
-
-Version 0.2.0
--------------
-:Date: 2021-02-18
-
-* API changed
-* can serialize dict with no-string keys
-* add support for cicular refÃ©rences and duplicates with {"$ref": ...}
-
-
-Version 0.1.0
--------------
-:Date: 2020-11-28
-
-* change description for pipy
-* add license for pipy
-* enable load of tuple, time.struct_time, Counter, OrderedDict and defaultdict
-
-Version 0.0.4
--------------
-:Date: 2020-11-24
-	
-* API changed
-* add plugins support
-* add bytes, bytearray and numpy.array compression with blosc zstd
-* fix itertive append and decode (not fully tested).
-* fix dump of numpy types without conversion to python types(not yet numpy.float64)
-
+Metadata-Version: 2.1
+Name: serializejson
+Version: 0.3.3
+Summary: A python library for fast serialization and deserialization of complex Python objects into JSON.
+Home-page: https://github.com/SmartAudioTools/serializejson
+Download-URL: https://github.com/SmartAudioTools/serializejson/tarball/master
+Author: Baptiste de La Gorce
+Author-email: baptiste.delagorce@smartaudiotools.com
+License: Prosperity Public License 3.0.0 and Patron License 1.0.0
+Project-URL: Documentation, https://smartaudiotools.github.io/serializejson
+Project-URL: Funding, https://github.com/sponsors/SmartAudioTools
+Project-URL: Source, https://github.com/SmartAudioTools/serializejson
+Project-URL: Tracker, https://github.com/SmartAudioTools/serializejson/issues
+Keywords: pickle json serialize dump dumps rapidjson base64
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Free for non-commercial use
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE-APACHE.rst
+License-File: LICENSE-PATRON.rst
+License-File: LICENSE-PROSPERITY.rst
+License-File: LICENSE.rst
+
+serializejson
+=============
+
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Authors**               | `Baptiste de La Gorce <contact@smartaudiotools.com>`_                                                                    |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **PyPI**                  | https://pypi.org/project/serializejson                                                                                   |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Documentation**         | https://smartaudiotools.github.io/serializejson                                                                          |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Sources**               | https://github.com/SmartAudioTools/serializejson                                                                         |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Issues**                | https://github.com/SmartAudioTools/serializejson/issues                                                                  |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Noncommercial license** | `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_ |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Commercial license**    | `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_                |
+|                           | ⇒ `Sponsor me ! <https://github.com/sponsors/SmartAudioTools>`_ or `contact me ! <contact@smartaudiotools.com>`_         |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+
+
+**serializejson**  is a python library for fast serialization and deserialization
+of python objects in `JSON <http://json.org>`_  designed as a safe, interoperable and human-readable drop-in replacement for the Python `pickle <https://docs.python.org/3/library/pickle.html>`_ package.
+Complex python object hierarchies are serializable, deserializable or updatable in once, allowing for example to save or restore a complete application state in few lines of code.
+The library is build upon
+`python-rapidjson <https://github.com/python-rapidjson/python-rapidjson>`_,
+`pybase64 <https://github.com/mayeut/pybase64>`_ and
+`blosc <https://github.com/Blosc/python-blosc>`_  for optional `zstandard <https://github.com/facebook/zstd>`_ compression.
+
+Some of the main features:
+
+- supports Python 3.7 (maybe lower) or greater.
+- serializes arbitrary python objects into a dictionary by adding `__class__` ,and eventually `__init__`, `__new__`, `__state__`, `__items__` keys.
+- calls the same objects methods as pickle. Therefore almost all pickable objects are serializable with serializejson without any modification.
+- for not already pickable object, you will allways be able to serialize it by adding methodes to the object or creating plugins for pickle or serializejson.
+- generally 2x slower than pickle for dumping and 3x slower than pickle for loading (on your benchmark) except for big arrays (optimisation will soon be done).
+- serializes and deserializes bytes and bytearray very quickly in base64 thanks to `pybase64 <https://github.com/mayeut/pybase64>`_ and lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
+- serialize properties and attributes with getters and setters if wanted (unlike pickle).
+- json data will still be directly loadable if you have transform some attributes in slots or properties in your code since your last serialization. (unlike pickle)
+- can serialize `__init__(self,..)` arguments by name instead of positions, allowing to skip arguments with defauts values and making json datas robust to a change of `__init__` parameters order.
+- serialized objects take generally less space than when serialized with pickle: for binary data, the 30% increase due to base64 encoding is in general largely compensated using the lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
+- serialized objects are human-readable and easy to read. Unlike pickled data, your data will never become unreadable if your code evolves: you will always be able to modify your datas with a text editor (with find & replace for example if you change an attribut name).
+- serialized objects are text and therefore versionable and comparable with versionning and comparaison tools.
+- can safely load untrusted / unauthenticated sources if authorized_classes list parameter is set carefully with strictly necessary objects (unlike pickle).
+- can update existing objects recursively instead of override them. serializejson can be used to save and restore in place a complete application state (⚠ not yet well tested).
+- filters attribute starting with "_" by default (unlike pickle). You can keep them if wanted with `filter_ = False`.
+- numpy arrays can be serialized as lists with automatic conversion in both ways or in a conservative way.
+- supports circular references and serialize only once duplicated objects, using "$ref" key an path to the first occurance in the json : `{"$ref": "root.xxx.elt"}` (⚠ not yet if the object is a list or dictionary).
+- accepts json with comment (// and /\* \*/) if `accept_comments = True`.
+- can automatically recognize objects in json from keys names and recreate them, without the need of `__class__` key, if passed in `recognized_classes`.
+- serializejson is easly interoperable outside of the Python ecosystem with this recognition of objects from keys names or with `__class__` translation between python and other language classes.
+- dump and load support string path.
+- can iteratively encode (with append) and decode (with iterator) a list in json file, which helps saving memory space during the process of serialization and deserialization and useful for logs.
+
+.. warning::
+
+    **⚠** Do not load serializejson files from untrusted / unauthenticated sources without carefully setting the load authorized_classes parameter.
+
+    **⚠** Never dump a dictionary with the `__class__` key, otherwise serializejson will attempt to reconstruct an object when loading the json.
+    Be careful not to allow a user to manually enter a dictionary key somewhere without checking that it is not `__class__`.
+    Due to current limitation of rapidjson we cannot we cannot at the moment efficiently detect dictionaries with the `__class__` key to raise an error.
+
+
+Installation
+============
+
+**Last offical release**
+
+.. code-block::
+
+    pip install serializejson
+
+**Developpement version unreleased**
+
+.. code-block::
+
+    pip install git+https://github.com/SmartAudioTools/serializejson.git
+
+Examples
+================
+
+**Serialization with fonctions API**
+
+.. code-block:: python
+
+    import serializejson
+
+    # serialize in string
+    object1 = set([1,2])
+    dumped1 = serializejson.dumps(object1)
+    loaded1 = serializejson.loads(dumped1)
+    print(dumped1)
+    >{
+    >        "__class__": "set",
+    >        "__init__": [1,2]
+    >}
+
+
+    # serialize in file
+    object2 = set([3,4])
+    serializejson.dump(object2,"dumped2.json")
+    loaded2 = serializejson.load("dumped2.json")
+
+**Serialization with classes based API.**
+
+.. code-block:: python
+
+    import serializejson
+    encoder = serializejson.Encoder()
+    decoder = serializejson.Decoder()
+
+    # serialize in string
+
+    object1 = set([1,2])
+    dumped1 = encoder.dumps(object1)
+    loaded1 = decoder.loads(dumped1)
+    print(dumped1)
+
+    # serialize in file
+    object2 = set([3,4])
+    encoder.dump(object2,"dumped2.json")
+    loaded2 = decoder.load("dumped2.json")
+
+**Update existing object**
+
+.. code-block:: python
+
+    import serializejson
+    object1 = set([1,2])
+    object2 = set([3,4])
+    dumped1 = serializejson.dumps(object1)
+    print(f"id {id(object2)} :  {object2}")
+    serializejson.loads(dumped1,obj = object2, updatables_classes = [set])
+    print(f"id {id(object2)} :  {object2}")
+
+**Iterative serialization and deserialization**
+
+.. code-block:: python
+
+    import serializejson
+    encoder = serializejson.Encoder("my_list.json",indent = None)
+    for elt in range(3):
+        encoder.append(elt)
+    print(open("my_list.json").read())
+    for elt in serializejson.Decoder("my_list.json"):
+        print(elt)
+    >[0,1,2]
+    >0
+    >1
+    >2
+
+More examples and complete documentation `here <https://smartaudiotools.github.io/serializejson/>`_
+
+License
+=======
+
+Copyright 2020 Baptiste de La Gorce
+
+For noncommercial use or thirty-day limited free-trial period commercial use, this project is licensed under the `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_.
+
+For non limited commercial use, this project is licensed under the `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_.
+To acquire a license please `contact me <mailto:contact@smartaudiotools.com>`_, or just `sponsor me on GitHub <https://github.com/sponsors/SmartAudioTools>`_ under the appropriate tier ! This funding model helps me making my work sustainable and compensates me for the work it took to write this crate!
+
+Third-party contributions are licensed under `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_ and belong to their respective authors.
+History
+=======
+
+Version 0.3.3
+-------------
+:Date: 2022-10-18
+
+* Big speed improvement for bytes and numpy array serialization
+
+Version 0.3.2
+-------------
+:Date: 2022-10-01
+
+* API changed
+* add better support for cicular reférences and duplicates with {"$ref": ...}
+
+Version 0.2.0
+-------------
+:Date: 2021-02-18
+
+* API changed
+* can serialize dict with no-string keys
+* add support for cicular reférences and duplicates with {"$ref": ...}
+
+
+Version 0.1.0
+-------------
+:Date: 2020-11-28
+
+* change description for pipy
+* add license for pipy
+* enable load of tuple, time.struct_time, Counter, OrderedDict and defaultdict
+
+Version 0.0.4
+-------------
+:Date: 2020-11-24
+	
+* API changed
+* add plugins support
+* add bytes, bytearray and numpy.array compression with blosc zstd
+* fix itertive append and decode (not fully tested).
+* fix dump of numpy types without conversion to python types(not yet numpy.float64)
```

### Comparing `serializejson-0.3.2/README.rst` & `serializejson-0.3.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 | **Sources**               | https://github.com/SmartAudioTools/serializejson                                                                         |
 +---------------------------+--------------------------------------------------------------------------------------------------------------------------+
 | **Issues**                | https://github.com/SmartAudioTools/serializejson/issues                                                                  |
 +---------------------------+--------------------------------------------------------------------------------------------------------------------------+
 | **Noncommercial license** | `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_ |
 +---------------------------+--------------------------------------------------------------------------------------------------------------------------+
 | **Commercial license**    | `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_                |
-|                           | `Sponsor me ! <https://github.com/sponsors/SmartAudioTools>`_ or `contact me ! <contact@smartaudiotools.com>`_           |
+|                           | ⇒ `Sponsor me ! <https://github.com/sponsors/SmartAudioTools>`_ or `contact me ! <contact@smartaudiotools.com>`_         |
 +---------------------------+--------------------------------------------------------------------------------------------------------------------------+
 
 
 **serializejson**  is a python library for fast serialization and deserialization
 of python objects in `JSON <http://json.org>`_  designed as a safe, interoperable and human-readable drop-in replacement for the Python `pickle <https://docs.python.org/3/library/pickle.html>`_ package.
 Complex python object hierarchies are serializable, deserializable or updatable in once, allowing for example to save or restore a complete application state in few lines of code.
 The library is build upon
@@ -38,29 +38,29 @@
 - serialize properties and attributes with getters and setters if wanted (unlike pickle).
 - json data will still be directly loadable if you have transform some attributes in slots or properties in your code since your last serialization. (unlike pickle)
 - can serialize `__init__(self,..)` arguments by name instead of positions, allowing to skip arguments with defauts values and making json datas robust to a change of `__init__` parameters order.
 - serialized objects take generally less space than when serialized with pickle: for binary data, the 30% increase due to base64 encoding is in general largely compensated using the lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
 - serialized objects are human-readable and easy to read. Unlike pickled data, your data will never become unreadable if your code evolves: you will always be able to modify your datas with a text editor (with find & replace for example if you change an attribut name).
 - serialized objects are text and therefore versionable and comparable with versionning and comparaison tools.
 - can safely load untrusted / unauthenticated sources if authorized_classes list parameter is set carefully with strictly necessary objects (unlike pickle).
-- can update existing objects recursively instead of override them. serializejson can be used to save and restore in place a complete application state (? not yet well tested).
+- can update existing objects recursively instead of override them. serializejson can be used to save and restore in place a complete application state (⚠ not yet well tested).
 - filters attribute starting with "_" by default (unlike pickle). You can keep them if wanted with `filter_ = False`.
 - numpy arrays can be serialized as lists with automatic conversion in both ways or in a conservative way.
-- supports circular references and serialize only once duplicated objects, using "$ref" key an path to the first occurance in the json : `{"$ref": "root.xxx.elt"}` (? not yet if the object is a list or dictionary).
+- supports circular references and serialize only once duplicated objects, using "$ref" key an path to the first occurance in the json : `{"$ref": "root.xxx.elt"}` (⚠ not yet if the object is a list or dictionary).
 - accepts json with comment (// and /\* \*/) if `accept_comments = True`.
 - can automatically recognize objects in json from keys names and recreate them, without the need of `__class__` key, if passed in `recognized_classes`.
 - serializejson is easly interoperable outside of the Python ecosystem with this recognition of objects from keys names or with `__class__` translation between python and other language classes.
 - dump and load support string path.
 - can iteratively encode (with append) and decode (with iterator) a list in json file, which helps saving memory space during the process of serialization and deserialization and useful for logs.
 
 .. warning::
 
-    **?** Do not load serializejson files from untrusted / unauthenticated sources without carefully setting the load authorized_classes parameter.
+    **⚠** Do not load serializejson files from untrusted / unauthenticated sources without carefully setting the load authorized_classes parameter.
 
-    **?** Never dump a dictionary with the `__class__` key, otherwise serializejson will attempt to reconstruct an object when loading the json.
+    **⚠** Never dump a dictionary with the `__class__` key, otherwise serializejson will attempt to reconstruct an object when loading the json.
     Be careful not to allow a user to manually enter a dictionary key somewhere without checking that it is not `__class__`.
     Due to current limitation of rapidjson we cannot we cannot at the moment efficiently detect dictionaries with the `__class__` key to raise an error.
 
 
 Installation
 ============
 
@@ -81,26 +81,26 @@
 
 **Serialization with fonctions API**
 
 .. code-block:: python
 
     import serializejson
 
-    #serialize in string
+    # serialize in string
     object1 = set([1,2])
     dumped1 = serializejson.dumps(object1)
     loaded1 = serializejson.loads(dumped1)
     print(dumped1)
     >{
     >        "__class__": "set",
     >        "__init__": [1,2]
     >}
 
 
-    #serialize in file
+    # serialize in file
     object2 = set([3,4])
     serializejson.dump(object2,"dumped2.json")
     loaded2 = serializejson.load("dumped2.json")
 
 **Serialization with classes based API.**
 
 .. code-block:: python
@@ -157,8 +157,8 @@
 Copyright 2020 Baptiste de La Gorce
 
 For noncommercial use or thirty-day limited free-trial period commercial use, this project is licensed under the `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_.
 
 For non limited commercial use, this project is licensed under the `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_.
 To acquire a license please `contact me <mailto:contact@smartaudiotools.com>`_, or just `sponsor me on GitHub <https://github.com/sponsors/SmartAudioTools>`_ under the appropriate tier ! This funding model helps me making my work sustainable and compensates me for the work it took to write this crate!
 
-Third-party contributions are licensed under `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_ and belong to their respective authors.
+Third-party contributions are licensed under `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_ and belong to their respective authors.
```

#### encoding

```diff
@@ -1 +1 @@
-iso-8859-1
+utf-8
```

### Comparing `serializejson-0.3.2/SmartFramework/files/__init__.py` & `serializejson-0.3.3/SmartFramework/files/__init__.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/SmartFramework/image/image_conversion.py` & `serializejson-0.3.3/SmartFramework/image/image_conversion.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/SmartFramework/string/encodings/ascii_printables.py` & `serializejson-0.3.3/SmartFramework/string/encodings/ascii_printables.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/SmartFramework/tools/dictionaries.py` & `serializejson-0.3.3/SmartFramework/tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/SmartFramework/tools/objects.py` & `serializejson-0.3.3/SmartFramework/tools/objects.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/__init__.py` & `serializejson-0.3.3/serializejson/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 `python-rapidjson <https://github.com/python-rapidjson/python-rapidjson>`_,
 `pybase64 <https://github.com/mayeut/pybase64>`_ and
 `blosc <https://github.com/Blosc/python-blosc>`_  for optional `zstandard <https://github.com/facebook/zstd>`_ compression.
 
 Some of the main features:
 
 - supports Python 3.7 (maybe lower) or greater.
-- serializes arbitrary python objects into a dictionary by adding `__class__` ,and eventually `__init__`, `__new__`, `__state__`, `__items__` keys.
+- serializes arbitrary python objects into a dictionary by adding `__class__` ,and eventually `__init__`, `__new__`, `__state__`, `__items__` keys.
 - calls the same objects methods as pickle. Therefore almost all pickable objects are serializable with serializejson without any modification.
 - for not already pickable object, you will allways be able to serialize it by adding methodes to the object or creating plugins for pickle or serializejson.
 - generally 2x slower than pickle for dumping and 3x slower than pickle for loading (on your benchmark) except for big arrays (optimisation will soon be done).
 - serializes and deserializes bytes and bytearray very quickly in base64 thanks to `pybase64 <https://github.com/mayeut/pybase64>`_ and lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
 - serialize properties and attributes with getters and setters if wanted (unlike pickle).
 - json data will still be directly loadable if you have transform some attributes in slots or properties in your code since your last serialization. (unlike pickle)
 - can serialize `__init__(self,..)` arguments by name instead of positions, allowing to skip arguments with defauts values and making json datas robust to a change of `__init__` parameters order.
@@ -44,15 +44,15 @@
 - serialized objects are text and therefore versionable and comparable with versionning and comparaison tools.
 - can safely load untrusted / unauthenticated sources if authorized_classes list parameter is set carefully with strictly necessary objects (unlike pickle).
 - can update existing objects recursively instead of override them. serializejson can be used to save and restore in place a complete application state (⚠ not yet well tested).
 - filters attribute starting with "_" by default (unlike pickle). You can keep them if wanted with `filter_ = False`.
 - numpy arrays can be serialized as lists with automatic conversion in both ways or in a conservative way.
 - supports circular references and serialize only once duplicated objects, using "$ref" key an path to the first occurance in the json : `{"$ref": "root.xxx.elt"}` (⚠ not yet if the object is a list or dictionary).
 - accepts json with comment (// and /\* \*/) if `accept_comments = True`.
-- can automatically recognize objects in json from keys names and recreate them, without the need of `__class__` key, if passed in `recognized_classes`.
+- can automatically recognize objects in json from keys names and recreate them, without the need of `__class__` key, if passed in `recognized_classes`.
 - serializejson is easly interoperable outside of the Python ecosystem with this recognition of objects from keys names or with `__class__` translation between python and other language classes.
 - dump and load support string path.
 - can iteratively encode (with append) and decode (with iterator) a list in json file, which helps saving memory space during the process of serialization and deserialization and useful for logs.
 
 .. warning::
 
     **⚠** Do not load serializejson files from untrusted / unauthenticated sources without carefully setting the load authorized_classes parameter.
@@ -179,21 +179,24 @@
 import rapidjson
 import gc
 import blosc
 import errno
 from collections import deque
 from pybase64 import b64decode, b64encode_as_string
 from _collections_abc import list_iterator
+
 try:
     import numpy
     from numpy import ndarray
+
     use_numpy = True
 except ModuleNotFoundError:
     use_numpy = False
 from . import serialize_parameters
+from enum import Enum
 
 
 # def add_authorized_classes(*classes):
 #    if len(classes) == 0 and type(classes[0]) in (tuple,list,set):
 #        classes = classes[0]
 #    for elt in classes:
 #        if not type(elt) is str:
@@ -283,26 +286,26 @@
     your should ether replace `pickle.dumps` calls by `serializejson.dumpb` calls
     or make an `from serializejson import dumpb as dumps` at the start of your script
 
     Args:
         obj: object to dump.
         **argsDict: parameters passed to the Encoder (see documentation).
     """
-    return Encoder(**argsDict)(obj, return_bytes=False)
+    return Encoder(return_bytes=False, **argsDict)(obj)
 
 
 def dumpb(obj, **argsDict):
     """
     Dump object into json bytes.
 
     Args:
         obj: object to dump.
         **argsDict: parameters passed to the Encoder (see documentation).
     """
-    return Encoder(**argsDict)(obj, return_bytes=False).encode("utf_8")
+    return Encoder(return_bytes=True, **argsDict)(obj)
 
 
 def append(obj, file=None, *, indent="\t", **argsDict):
     """
     Append an object into json file.
 
     Args:
@@ -534,15 +537,15 @@
 
         numpy_array_to_list:
             whether numpy array should be serialized as list.
 
             .. warning::
 
                 This should be used only for interoperability with other json libraries.
-                If you want readable  values in your json, we recommend to use instead
+                If you want readable  values in your json, we recommend to use instead
                 `numpy_array_readable_max_size` which is not destructive.
 
                 With `numpy_array_to_list` set to `True`:
 
                 - numpy arrays will be indistinctable from list in json.
                 - `Decoder(numpy_array_from_list=True)` will recreate numpy array from lists of bool, int or float, if not an `__init__` args list, with the the risque of unwanted convertion of lists to numpy arrays.
                 - dtype of the numpy array will be loosed if not bool, int32 or float64 and converted to the bool, int32 or float64 when loading
@@ -588,15 +591,15 @@
     """
 
     def __new__(
         cls,
         file=None,
         *,
         strict_pickle=False,
-        return_bytes=False,
+        return_bytes=True,
         attributes_filter=True,
         properties=False,
         getters=False,
         remove_default_values=False,
         chunk_size=65536,
         ensure_ascii=False,
         indent="\t",
@@ -633,24 +636,25 @@
             cls,
             ensure_ascii=ensure_ascii,
             indent=indent,
             sort_keys=sort_keys,
             bytes_mode=rapidjson.BM_NONE,
             number_mode=rapidjson.NM_NAN,
             iterable_mode=rapidjson.IM_ONLY_LISTS,
-            mapping_mode=rapidjson.MM_ONLY_DICTS
+            mapping_mode=rapidjson.MM_ONLY_DICTS,
+            return_bytes=return_bytes
             # **argsDict
         )
+        self.use_tuple_for_numpy_shape = False
         self.protocol = protocol
         self.attributes_filter = bool_or_set(attributes_filter)
         self.properties = _get_properties(properties)
         self.getters = _get_getters(getters)
         self.remove_default_values = bool_or_set(remove_default_values)
         self.file = file
-        self.return_bytes = return_bytes
         if indent is None:
             self.single_line_list_numbers = False
             self.single_line_init = False
             self.single_line_new = False
         else:
             self.single_line_list_numbers = single_line_list_numbers
             self.single_line_init = single_line_init
@@ -793,17 +797,18 @@
         return self.dumped_classes
 
     # @profile
     def default(self, inst):
         # Equivalent au calback "default" qu'on peut passer à dump ou dumps
         id_ = id(inst)
         if id_ in self._already_serialized:
-            path = self._get_path(inst, already_explored=set([id(locals())]))
-            if path is not None:
-                return rapidjson.RawJSON(f'{"$ref": "{path}"}')
+            if not isinstance(inst, Enum):
+                path = self._get_path(inst, already_explored=set([id(locals())]))
+                if path is not None:
+                    return rapidjson.RawString(f'{{"$ref": "{path}"}}')
         else:
             self._already_serialized.add(id_)
         type_inst = type(inst)
         if self.numpy_types_to_python_types and type_inst in _numpy_types:
             return _numpy_dtypes_to_python_types[type_inst](inst)
         if use_numpy and type_inst is ndarray and self.numpy_array_to_list:
             if self._dump_one_line or not self.single_line_list_numbers:
@@ -811,41 +816,41 @@
                     inst.tolist()
                 )  # A REVOIR : pas génial... va tester si nombres tous du meme type et ne pas pas utiliser rapidjson.NM_NATIVE?
             if inst.dtype in _numpy_float_dtypes:
                 number_mode = self.number_mode
             else:
                 number_mode = rapidjson.NM_NATIVE  # permet décceler pas mal
             if inst.ndim == 1:
-                return rapidjson.RawJSON(
-                    rapidjson.dumps(
+                return rapidjson.RawBytes(
+                    rapidjson.dumpb(
                         inst.tolist(),
                         ensure_ascii=False,
                         number_mode=number_mode,
                         iterable_mode=rapidjson.IM_ONLY_LISTS,
                         mapping_mode=rapidjson.MM_ONLY_DICTS,
                     )
                 )
             return [
-                rapidjson.RawJSON(
-                    rapidjson.dumps(
+                rapidjson.RawBytes(
+                    rapidjson.dumpb(
                         elt.tolist(),
                         ensure_ascii=False,
                         number_mode=number_mode,
                         iterable_mode=rapidjson.IM_ONLY_LISTS,
                         mapping_mode=rapidjson.MM_ONLY_DICTS,
                     )
                 )
                 for elt in inst
             ]  # inst.tolist()
         if type_inst is tuple:
             # isinstance(inst,tuple) attrape les struct_time # je l'ai mis là plutot que dans tuple_from_instance car très spécifique à json et les tuples n'ont pas de réduce contrairement à set , qui lui est pour l'instant traité dans dict_from_instance -> tuple_from_instance
             self.dumped_classes.add(tuple)
             dic = {"__class__": "tuple", "__new__": list(inst)}
         elif type_inst is Reference:
-            return rapidjson.RawJSON(
+            return rapidjson.RawString(
                 '{"$ref": "%s%s"}'
                 % (
                     self._get_path(inst.obj, already_explored=set([id(inst.__dict__)])),
                     inst.sup_str,
                 )
             )
         else:
@@ -854,16 +859,16 @@
             )  # 8.6 % (correspond au temps pour conversion en b64 avec pybase64.b64encode) du temps sur obj = bytes(numpy.arange(2**20,dtype=numpy.float64).data)
 
         if not self._dump_one_line:
             if self.single_line_init:
                 args = dic.get("__init__", None)
                 if isinstance(args, list):
                     # 91.2 % du temps avec obj = bytes(numpy.arange(2**20,dtype=numpy.float64).data)
-                    dic["__init__"] = rapidjson.RawJSON(
-                        rapidjson.dumps(
+                    dic["__init__"] = rapidjson.RawBytes(
+                        rapidjson.dumpb(
                             args,
                             ensure_ascii=self.ensure_ascii,
                             default=self._default_one_line,
                             sort_keys=self.sort_keys,
                             bytes_mode=self.bytes_mode,
                             number_mode=self.number_mode,
                             iterable_mode=rapidjson.IM_ONLY_LISTS,
@@ -873,16 +878,16 @@
                     )
             if self.single_line_new:
                 args = dic.get("__new__", None)
                 if type(args) is list:
                     dic[
                         "__new__"
                         # 91.2 % du temps avec obj = bytes(numpy.arange(2**20,dtype=numpy.float64).data)
-                    ] = rapidjson.RawJSON(
-                        rapidjson.dumps(
+                    ] = rapidjson.RawBytes(
+                        rapidjson.dumpb(
                             args,
                             ensure_ascii=self.ensure_ascii,
                             default=self._default_one_line,
                             sort_keys=self.sort_keys,
                             bytes_mode=self.bytes_mode,
                             number_mode=self.number_mode,
                             iterable_mode=rapidjson.IM_ONLY_LISTS,
@@ -897,16 +902,16 @@
                         key != "__class__"
                         and (key != "__init__" or not self.single_line_init)
                         and (key != "__new__" or not self.single_line_new)
                         and type(value) is list
                         and _onlyOneDimSameTypeNumbers(value)
                     ):
 
-                        dic[key] = rapidjson.RawJSON(
-                            rapidjson.dumps(
+                        dic[key] = rapidjson.RawBytes(
+                            rapidjson.dumpb(
                                 value,
                                 ensure_ascii=self.ensure_ascii,
                                 default=self._default_one_line,
                                 bytes_mode=self.bytes_mode,
                                 number_mode=self.number_mode,
                                 iterable_mode=rapidjson.IM_ONLY_LISTS,
                                 mapping_mode=rapidjson.MM_ONLY_DICTS
@@ -1059,15 +1064,15 @@
                 obj,
                 ensure_ascii=False,
                 default=self._default_one_line,
                 bytes_mode=self.bytes_mode,
                 number_mode=self.number_mode,
                 iterable_mode=rapidjson.IM_ONLY_LISTS,
                 mapping_mode=rapidjson.MM_ONLY_DICTS,
-                # return_bytes = return_bytes
+                return_bytes=return_bytes
                 # **self.kargs
             )
         self._update_serialize_parameters()
         self._reset()
         self._root = obj
         encoded = rapidjson.Encoder.__call__(
             self, obj, stream=fp, chunk_size=self.chunk_size
@@ -1167,15 +1172,15 @@
         already_explored.add(id(locals()))
         pathElements = self._searchSerializedParent(
             obj, already_explored=already_explored
         )
         if not pathElements:
             return None
             # return f'impossible to find a path from root object for {obj}'
-            #raise Exception("impossible to find a path from root object for %s" % obj)
+            # raise Exception("impossible to find a path from root object for %s" % obj)
             # print("!",pathElements)
             # return pathElements[0][0]
 
         return "".join([e for e in sorted(pathElements)[0][0] if isinstance(e, str)])
 
 
 class Decoder(rapidjson.Decoder):
@@ -1548,16 +1553,15 @@
         elif "$ref" in inst and len(inst) == 1:
             if self.root:
                 # try:
                 inst_potential = from_name(
                     inst["$ref"], accept_dict_as_object=True, root=self.root
                 )  # essaye de remplacer tout de suite si possible
                 if inst is inst_potential:
-                    raise Exception('{"$ref": "%s"} pointing to himself' %
-                                    inst["$ref"])
+                    raise Exception('{"$ref": "%s"} pointing to himself' % inst["$ref"])
                 if not type(inst_potential) is dict:
                     # verifie que ce n'est pas un objet qui n'a pas encore été recré
                     return inst_potential
                 if "__class__" not in inst_potential:
                     return inst_potential
                 inst_potential_epured = {
                     key: inst_potential[key]
@@ -1621,14 +1625,15 @@
         """
         blosc.set_nthreads(blosc.ncores)
         serialize_parameters.strict_pickle = self.strict_pickle
         serialize_parameters.setters = self.setters
         serialize_parameters.properties = self.properties
         self.converted_numpy_array_from_lists = set()
         # self._counter = 0
+        self.not_authorized_classes = set()
         self._updating = False
         # for duplicates -----------
         self.root = None
         if isinstance(json, str):
             self.json_startswith_curly = json.startswith("{")
         elif isinstance(json, bytes):
             self.json_startswith_curly = json.startswith(b"{")
@@ -1648,25 +1653,28 @@
             loaded_dict = rapidjson.Decoder.__call__(
                 self, json, chunk_size=self.chunk_size
             )
             loaded = self._exploreToUpdate(obj, loaded_dict)
         # on restaure doublons qu'on a pu restaurer pendant deserialisation (dans une liste ou doublon referencant un parent)
         duplicates_to_replace = self.duplicates_to_replace
         if duplicates_to_replace:
-            gc.collect()  # pas sur qu'indispensable mais dans le doute  https://docs.python.org/3/library/gc.html#gc.get_referrers
+            # pas sur qu'indispensable mais dans le doute  https://docs.python.org/3/library/gc.html#gc.get_referrers:
+            gc.collect()
             while duplicates_to_replace:
                 duplicate_to_replace = duplicates_to_replace.pop()
                 referenced = from_name(
                     duplicate_to_replace["$ref"],
                     accept_dict_as_object=True,
                     root=loaded,
                 )
                 if referenced is duplicate_to_replace:
-                    raise Exception('{"$ref": "%s"} pointing to himself' %
-                                    duplicate_to_replace["$ref"])
+                    raise Exception(
+                        '{"$ref": "%s"} pointing to himself'
+                        % duplicate_to_replace["$ref"]
+                    )
                 refs = gc.get_referrers(duplicate_to_replace)
                 skip = (locals(), refs)
                 for parent in refs:
                     if parent not in skip:
                         if type(parent) is dict:
                             for key, value in parent.items():
                                 if value is duplicate_to_replace:
@@ -1722,32 +1730,35 @@
 
             if (
                 inst["__class__"] == "dict_non_str_keys"
             ):  # je l'ai mis ici car trop specifique à json pour etre dans tools (qui est partagé avec serializePython et serializeRepr)
                 return dict_non_str_keys(inst)
             return instance(**inst)
         if self.unauthorized_classes_as_dict:
+            class_str = inst["__class__"]
+            self.not_authorized_classes.add(class_str)
             if self.dotdict:
                 warnings.warn(
-                    f"{inst['__class__']} not in authorized_classes leaved as docdict",
+                    f"{class_str} not in authorized_classes leaved as docdict",
                     Warning,
                 )
                 return dotdict(inst)
             warnings.warn(
-                f"{inst['__class__']} not in authorized_classes leaved as dict", Warning
+                f"{class_str} not in authorized_classes leaved as dict", Warning
             )
             return inst
         raise TypeError(f"{inst['__class__']} is not in authorized_classes")
 
     # @profile
     def _exploreToUpdate(self, obj, loaded_node):
 
         # gère le cas où loaded_node est un dictionnaire ----------------------
         if isinstance(loaded_node, dict):
-            obj_keys = None  # plutot que set vide un objet peut ne pas avoir d'attributes ni de slots initialisés
+            # plutot que set vide un objet peut ne pas avoir d'attributes ni de slots initialisés:
+            obj_keys = None
             obj_class = obj.__class__
             if obj_class is dict and ("dict" in self.updatableClassStrs):
                 is_dict = True
                 obj_keys = set(obj)
                 obj
             else:  # s'assure que c'est une instance
                 is_dict = False
@@ -1829,15 +1840,15 @@
             return self._exploreDictToReCreateObjects(loaded_node)
 
         # gère le cas où loaded_node est une liste ---------------------------
         if isinstance(loaded_node, list):
             if isinstance(obj, list) and ("list" in self.updatableClassStrs):
                 # update dans le cas où l'objet pré-existant est une liste
                 len_obj = len(obj)
-                del obj[len(loaded_node):]
+                del obj[len(loaded_node) :]
                 for i, value in enumerate(loaded_node):
                     if i < len_obj and isinstance(value, (list, dict)):
                         obj[i] = self._exploreToUpdate(obj[i], value)
                     else:
                         if isinstance(value, dict):
                             value = self._exploreDictToReCreateObjects(value)
                         elif isinstance(value, list):
@@ -2084,15 +2095,15 @@
                         fp = open(path, "r+", encoding="utf_32_le")
                     else:
                         fp = open(path, "r+", encoding="utf_16_le")
             # remove last ]
             remove_last_square_close = True
 
         else:
-            fp = open(path, "wb+") # pour test_iterator.py
+            fp = open(path, "wb+")  # pour test_iterator.py
             remove_last_square_close = False
     elif fp is None:
         raise Exception("Incorrect file (file, str ou unicode)")
     if remove_last_square_close:
         fp.seek(0, 2)
         length = fp.tell()
         if length == 1:
@@ -2264,15 +2275,16 @@
             elif ch in interesting:
                 check = False
                 if in_quotes:
                     if backslash_escape:
                         # we must have just seen a backslash; reset that flag and continue
                         backslash_escape = False
                     elif ch == backslash:
-                        backslash_escape = True  # we are in a quote and we see a backslash; escape next char
+                        # we are in a quote and we see a backslash; escape next char:
+                        backslash_escape = True
                     elif ch == doublecote:
                         in_quotes = False
                         # signale qu'on sort d'un truc et qu'il faudra checker
                         check = True
                 elif ch == doublecote:  # "
                     in_quotes = True
                     in_object = True
@@ -2301,15 +2313,15 @@
                     self.in_chunk_start = (i + 1) % len(s)
                     self.in_quotes = False
                     self.in_curlys = False
                     self.in_squares = in_squares
                     self.in_simple = False
                     self.in_object = False
                     # print("read(3): ",s[in_chunk_start: i + 1])
-                    return s[in_chunk_start: i + 1]
+                    return s[in_chunk_start : i + 1]
             elif not in_object:
                 if ch in separators:
                     in_chunk_start = i + 1
                 else:
                     in_simple = True
         self.in_quotes = in_quotes
         self.in_curlys = in_curlys
```

### Comparing `serializejson-0.3.2/serializejson/plugins/module_name.py` & `serializejson-0.3.3/serializejson/plugins/module_name.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/plugins/pickle_PyQt5_PySide2.py` & `serializejson-0.3.3/serializejson/plugins/pickle_PyQt5_PySide2.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/plugins/serializejson_PyQt5_PySide2.py` & `serializejson-0.3.3/serializejson/plugins/serializejson_PyQt5_PySide2.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/plugins/serializejson_array.py` & `serializejson-0.3.3/serializejson/plugins/serializejson_array.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/plugins/serializejson_builtins.py` & `serializejson-0.3.3/serializejson/plugins/serializejson_builtins.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/plugins/serializejson_datetime.py` & `serializejson-0.3.3/serializejson/plugins/serializejson_datetime.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/plugins/serializejson_numpy.py` & `serializejson-0.3.3/serializejson/plugins/serializejson_numpy.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/serialize_parameters.py` & `serializejson-0.3.3/serializejson/serialize_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 # use_bytesB64        = True	    # précise si on doit utiliser mon constructeur SmartFramework.bytesB64() pour les bytes rendant alors le json dependant de ma bibliotheque ou base64.b64decode . l'avantage de bytesB64 est d'utilsier pyBase64 beaucoup plus rapide que base64 et de déclancher une erreure si y'a un caracter qui est pas dans la base .
 
 # a laisser là  on y toucher à priori pas -----------------------
 
 # base64_for_bytes = True  # dit si doit utiliser l'encodage en base64 pour l'encodage des bytes et bytes array, si pas ascii printables. Ce paramètre n'est modifiable que directement ici. Attention s'il est mis à False, si serialize en json plantera sur les bytes avec des valeures < 128 dans tuple_from_bytes => le laisser toujours True ?
 strict_pickle = False
 do_checks = True
-numpyB64_convert_int64_to_int32_and_align_in_Python_32Bit = True  # dis si numpyB64 doit deserialiser les tableau int64 en int32 quand utilise python 32 bits (pour prendre moins de place? ou pour pouvoir deserialiser les classifiers en python 32 bit ?
+# dis si numpyB64 doit deserialiser les tableau int64 en int32 quand utilise python 32 bits (pour prendre moins de place? ou pour pouvoir deserialiser les classifiers en python 32 bit ?:
+numpyB64_convert_int64_to_int32_and_align_in_Python_32Bit = True
 
 # noms de fichiers ----------------------------
-forceRelativePath = False  # force noms de fichier en chemin relatif ,utilisé que dans serializeRepr.py dans la fonction reprFile et en plus mal codé. Ce paramètre n'est modifiable que directement ici
-forceAbsolutPath = False  # force noms de fichier en chemin absolut ,utilisé que dans serializeRepr.py dans la fonction reprFile. Ce paramètre n'est modifiable que directemen ici
+# force noms de fichier en chemin relatif ,utilisé que dans serializeRepr.py dans la fonction reprFile et en plus mal codé. Ce paramètre n'est modifiable que directement ici:
+forceRelativePath = False
+# force noms de fichier en chemin absolut ,utilisé que dans serializeRepr.py dans la fonction reprFile. Ce paramètre n'est modifiable que directemen ici:
+forceAbsolutPath = False
 
 # serialisation des objets -----------------------------------------
 # attributes_filter   = "_"        #  dit si doit filtrer les attribute commencant par la chaine stocke dans filtre.
 # call_setters      = True       # dit si doit tenter d'appeler setter pour la restauration des attributes.
 # False :  		    + conforme au comportement de pickle (si on n'utiliser pas de filtre "_")
 # True  :  		    + permet d'effectuer des traitements, de mettre en place des choses (par ex interface I/O) ,
 #             	    +  permet de rafraichir UI
```

### Comparing `serializejson-0.3.2/serializejson/simple_exemple_update.py` & `serializejson-0.3.3/serializejson/simple_exemple_update.py`

 * *Files identical despite different names*

### Comparing `serializejson-0.3.2/serializejson/tools.py` & `serializejson-0.3.3/serializejson/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,16 @@
                 elif key not in remove:
                     try:
                         value = _getattribute(getter_name)()
                         if remove_types and (type(value) in remove_types):
                             continue
                         state_slots[key] = value
                     except TypeError:
-                        pass  # n'arrive pas à regler le pb avec inspect qui n'arrive pas à parser arguement du getter
+                        # n'arrive pas à regler le pb avec inspect qui n'arrive pas à parser arguement du getter:
+                        pass
 
         # get __slots__ attributs ----------------
         check_prop_getters = bool(state_slots)
         if has_slots:
             if remove or filter_ or check_prop_getters or remove_types:
                 for key in slots:
                     if (
@@ -269,15 +270,16 @@
                 ):
                     value = _dict[key]
                     if remove_types and (type(value) in remove_types):
                         continue
                     state_dict[key] = value
         else:
             if not state_slots or splited_dict_slots:
-                state_dict = _dict  # no copie   A REVOIR , ON SPLIT DICT ET SLOT MEME SI PAS SPLITE A LA BASE
+                # no copie   A REVOIR , ON SPLIT DICT ET SLOT MEME SI PAS SPLITE A LA BASE:
+                state_dict = _dict
             else:
                 state_dict.update(_dict)
 
     if remove_default_values is True:
         if default_values is None:
             default_values = default_state_from_class(type(self))
         for key, default_value in default_values.items():
@@ -824,15 +826,16 @@
                             state = state.copy()
                         for key, getter_name in _getters.items():
                             try:
                                 state[key] = _getattribute(getter_name)()
                             except TypeError:
                                 pass
 
-                    """# remove default values (Je l'ai viré car il faut faire appel au __init__ et donc avoir recodé le reduce() pour pouvoir se permetre d'enlever les valeures par défaut)
+                    # remove default values (Je l'ai viré car il faut faire appel au __init__ et donc avoir recodé le reduce() pour pouvoir se permetre d'enlever les valeures par défaut):
+                    """
                     ##remove_default_values = serialize_parameters.remove_default_values
                     ##if type(remove_default_values) is set :
                     ##    remove_default_values = (class_ in remove_default_values)
                     ##if remove_default_values:
                     ##    _dict = getattr(obj, "__dict__",None)
                     ##    default_values = default_state_from_class(class_)
                     ##    for key, default_value in default_values.items() :
@@ -1219,25 +1222,27 @@
                     else:
                         raise Exception("%s is not a valid path in json")
                 elif in_simple_quotes:
                     if backslash_escape:
                         # we must have just seen a backslash; reset that flag and continue
                         backslash_escape = False
                     elif ch == "\\":  # \
-                        backslash_escape = True  # we are in a quote and we see a backslash; escape next char
+                        # we are in a quote and we see a backslash; escape next char:
+                        backslash_escape = True
                     elif ch == "'":
                         in_simple_quotes = False
                     else:
                         element_chars.append(ch)
                 elif in_double_quotes:
                     if backslash_escape:
                         # we must have just seen a backslash; reset that flag and continue
                         backslash_escape = False
                     elif ch == "\\":  # \
-                        backslash_escape = True  # we are in a quote and we see a backslash; escape next char
+                        # we are in a quote and we see a backslash; escape next char:
+                        backslash_escape = True
                     elif ch == '"':
                         in_double_quotes = False
                     else:
                         element_chars.append(ch)
                 elif ch == "]":
                     if element_chars:
                         key = "".join(element_chars)
@@ -1356,15 +1361,15 @@
             current = _getattr(
                 current, element, accept_dict_as_object
             )  # permet de marcher avec slot et properties,mais pas getters
     return current
 
 
 def _getattr(obj, attribut, accept_dict_as_object):
-    if accept_dict_as_object and type(obj) is dict and "__class__" in obj:
+    if accept_dict_as_object and type(obj) is dict :#and "__class__" in obj:
         return obj[attribut]
     else:
         try:
             # permet de marcher avec slot et properties,mais pas getters
             return getattr(obj, attribut)
         except:
             for methode in [
```

### Comparing `serializejson-0.3.2/serializejson.egg-info/PKG-INFO` & `serializejson-0.3.3/serializejson.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,233 +1,238 @@
-Metadata-Version: 2.1
-Name: serializejson
-Version: 0.3.2
-Summary: A python library for fast serialization and deserialization of complex Python objects into JSON.
-Home-page: https://github.com/SmartAudioTools/serializejson
-Author: Baptiste de La Gorce
-Author-email: baptiste.delagorce@smartaudiotools.com
-License: Prosperity Public License 3.0.0 and Patron License 1.0.0
-Download-URL: https://github.com/SmartAudioTools/serializejson/tarball/master
-Project-URL: Documentation, https://smartaudiotools.github.io/serializejson
-Project-URL: Funding, https://github.com/sponsors/SmartAudioTools
-Project-URL: Source, https://github.com/SmartAudioTools/serializejson
-Project-URL: Tracker, https://github.com/SmartAudioTools/serializejson/issues
-Keywords: pickle json serialize dump dumps rapidjson base64
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: Free for non-commercial use
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE-APACHE.rst
-License-File: LICENSE-PATRON.rst
-License-File: LICENSE-PROSPERITY.rst
-License-File: LICENSE.rst
-
-serializejson
-=============
-
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Authors**               | `Baptiste de La Gorce <contact@smartaudiotools.com>`_                                                                    |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **PyPI**                  | https://pypi.org/project/serializejson                                                                                   |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Documentation**         | https://smartaudiotools.github.io/serializejson                                                                          |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Sources**               | https://github.com/SmartAudioTools/serializejson                                                                         |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Issues**                | https://github.com/SmartAudioTools/serializejson/issues                                                                  |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Noncommercial license** | `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_ |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-| **Commercial license**    | `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_                |
-|                           | `Sponsor me ! <https://github.com/sponsors/SmartAudioTools>`_ or `contact me ! <contact@smartaudiotools.com>`_           |
-+---------------------------+--------------------------------------------------------------------------------------------------------------------------+
-
-
-**serializejson**  is a python library for fast serialization and deserialization
-of python objects in `JSON <http://json.org>`_  designed as a safe, interoperable and human-readable drop-in replacement for the Python `pickle <https://docs.python.org/3/library/pickle.html>`_ package.
-Complex python object hierarchies are serializable, deserializable or updatable in once, allowing for example to save or restore a complete application state in few lines of code.
-The library is build upon
-`python-rapidjson <https://github.com/python-rapidjson/python-rapidjson>`_,
-`pybase64 <https://github.com/mayeut/pybase64>`_ and
-`blosc <https://github.com/Blosc/python-blosc>`_  for optional `zstandard <https://github.com/facebook/zstd>`_ compression.
-
-Some of the main features:
-
-- supports Python 3.7 (maybe lower) or greater.
-- serializes arbitrary python objects into a dictionary by adding `__class__` ,and eventually `__init__`, `__new__`, `__state__`, `__items__` keys.
-- calls the same objects methods as pickle. Therefore almost all pickable objects are serializable with serializejson without any modification.
-- for not already pickable object, you will allways be able to serialize it by adding methodes to the object or creating plugins for pickle or serializejson.
-- generally 2x slower than pickle for dumping and 3x slower than pickle for loading (on your benchmark) except for big arrays (optimisation will soon be done).
-- serializes and deserializes bytes and bytearray very quickly in base64 thanks to `pybase64 <https://github.com/mayeut/pybase64>`_ and lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
-- serialize properties and attributes with getters and setters if wanted (unlike pickle).
-- json data will still be directly loadable if you have transform some attributes in slots or properties in your code since your last serialization. (unlike pickle)
-- can serialize `__init__(self,..)` arguments by name instead of positions, allowing to skip arguments with defauts values and making json datas robust to a change of `__init__` parameters order.
-- serialized objects take generally less space than when serialized with pickle: for binary data, the 30% increase due to base64 encoding is in general largely compensated using the lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
-- serialized objects are human-readable and easy to read. Unlike pickled data, your data will never become unreadable if your code evolves: you will always be able to modify your datas with a text editor (with find & replace for example if you change an attribut name).
-- serialized objects are text and therefore versionable and comparable with versionning and comparaison tools.
-- can safely load untrusted / unauthenticated sources if authorized_classes list parameter is set carefully with strictly necessary objects (unlike pickle).
-- can update existing objects recursively instead of override them. serializejson can be used to save and restore in place a complete application state (? not yet well tested).
-- filters attribute starting with "_" by default (unlike pickle). You can keep them if wanted with `filter_ = False`.
-- numpy arrays can be serialized as lists with automatic conversion in both ways or in a conservative way.
-- supports circular references and serialize only once duplicated objects, using "$ref" key an path to the first occurance in the json : `{"$ref": "root.xxx.elt"}` (? not yet if the object is a list or dictionary).
-- accepts json with comment (// and /\* \*/) if `accept_comments = True`.
-- can automatically recognize objects in json from keys names and recreate them, without the need of `__class__` key, if passed in `recognized_classes`.
-- serializejson is easly interoperable outside of the Python ecosystem with this recognition of objects from keys names or with `__class__` translation between python and other language classes.
-- dump and load support string path.
-- can iteratively encode (with append) and decode (with iterator) a list in json file, which helps saving memory space during the process of serialization and deserialization and useful for logs.
-
-.. warning::
-
-    **?** Do not load serializejson files from untrusted / unauthenticated sources without carefully setting the load authorized_classes parameter.
-
-    **?** Never dump a dictionary with the `__class__` key, otherwise serializejson will attempt to reconstruct an object when loading the json.
-    Be careful not to allow a user to manually enter a dictionary key somewhere without checking that it is not `__class__`.
-    Due to current limitation of rapidjson we cannot we cannot at the moment efficiently detect dictionaries with the `__class__` key to raise an error.
-
-
-Installation
-============
-
-**Last offical release**
-
-.. code-block::
-
-    pip install serializejson
-
-**Developpement version unreleased**
-
-.. code-block::
-
-    pip install git+https://github.com/SmartAudioTools/serializejson.git
-
-Examples
-================
-
-**Serialization with fonctions API**
-
-.. code-block:: python
-
-    import serializejson
-
-    #serialize in string
-    object1 = set([1,2])
-    dumped1 = serializejson.dumps(object1)
-    loaded1 = serializejson.loads(dumped1)
-    print(dumped1)
-    >{
-    >        "__class__": "set",
-    >        "__init__": [1,2]
-    >}
-
-
-    #serialize in file
-    object2 = set([3,4])
-    serializejson.dump(object2,"dumped2.json")
-    loaded2 = serializejson.load("dumped2.json")
-
-**Serialization with classes based API.**
-
-.. code-block:: python
-
-    import serializejson
-    encoder = serializejson.Encoder()
-    decoder = serializejson.Decoder()
-
-    # serialize in string
-
-    object1 = set([1,2])
-    dumped1 = encoder.dumps(object1)
-    loaded1 = decoder.loads(dumped1)
-    print(dumped1)
-
-    # serialize in file
-    object2 = set([3,4])
-    encoder.dump(object2,"dumped2.json")
-    loaded2 = decoder.load("dumped2.json")
-
-**Update existing object**
-
-.. code-block:: python
-
-    import serializejson
-    object1 = set([1,2])
-    object2 = set([3,4])
-    dumped1 = serializejson.dumps(object1)
-    print(f"id {id(object2)} :  {object2}")
-    serializejson.loads(dumped1,obj = object2, updatables_classes = [set])
-    print(f"id {id(object2)} :  {object2}")
-
-**Iterative serialization and deserialization**
-
-.. code-block:: python
-
-    import serializejson
-    encoder = serializejson.Encoder("my_list.json",indent = None)
-    for elt in range(3):
-        encoder.append(elt)
-    print(open("my_list.json").read())
-    for elt in serializejson.Decoder("my_list.json"):
-        print(elt)
-    >[0,1,2]
-    >0
-    >1
-    >2
-
-More examples and complete documentation `here <https://smartaudiotools.github.io/serializejson/>`_
-
-License
-=======
-
-Copyright 2020 Baptiste de La Gorce
-
-For noncommercial use or thirty-day limited free-trial period commercial use, this project is licensed under the `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_.
-
-For non limited commercial use, this project is licensed under the `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_.
-To acquire a license please `contact me <mailto:contact@smartaudiotools.com>`_, or just `sponsor me on GitHub <https://github.com/sponsors/SmartAudioTools>`_ under the appropriate tier ! This funding model helps me making my work sustainable and compensates me for the work it took to write this crate!
-
-Third-party contributions are licensed under `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_ and belong to their respective authors.
-
-History
-=======
-
-Version 0.3.2
--------------
-:Date: 2022-10-01
-
-* API changed
-* add better support for cicular refÃ©rences and duplicates with {"$ref": ...}
-
-Version 0.2.0
--------------
-:Date: 2021-02-18
-
-* API changed
-* can serialize dict with no-string keys
-* add support for cicular refÃ©rences and duplicates with {"$ref": ...}
-
-
-Version 0.1.0
--------------
-:Date: 2020-11-28
-
-* change description for pipy
-* add license for pipy
-* enable load of tuple, time.struct_time, Counter, OrderedDict and defaultdict
-
-Version 0.0.4
--------------
-:Date: 2020-11-24
-	
-* API changed
-* add plugins support
-* add bytes, bytearray and numpy.array compression with blosc zstd
-* fix itertive append and decode (not fully tested).
-* fix dump of numpy types without conversion to python types(not yet numpy.float64)
-
+Metadata-Version: 2.1
+Name: serializejson
+Version: 0.3.3
+Summary: A python library for fast serialization and deserialization of complex Python objects into JSON.
+Home-page: https://github.com/SmartAudioTools/serializejson
+Download-URL: https://github.com/SmartAudioTools/serializejson/tarball/master
+Author: Baptiste de La Gorce
+Author-email: baptiste.delagorce@smartaudiotools.com
+License: Prosperity Public License 3.0.0 and Patron License 1.0.0
+Project-URL: Documentation, https://smartaudiotools.github.io/serializejson
+Project-URL: Funding, https://github.com/sponsors/SmartAudioTools
+Project-URL: Source, https://github.com/SmartAudioTools/serializejson
+Project-URL: Tracker, https://github.com/SmartAudioTools/serializejson/issues
+Keywords: pickle json serialize dump dumps rapidjson base64
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Free for non-commercial use
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE-APACHE.rst
+License-File: LICENSE-PATRON.rst
+License-File: LICENSE-PROSPERITY.rst
+License-File: LICENSE.rst
+
+serializejson
+=============
+
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Authors**               | `Baptiste de La Gorce <contact@smartaudiotools.com>`_                                                                    |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **PyPI**                  | https://pypi.org/project/serializejson                                                                                   |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Documentation**         | https://smartaudiotools.github.io/serializejson                                                                          |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Sources**               | https://github.com/SmartAudioTools/serializejson                                                                         |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Issues**                | https://github.com/SmartAudioTools/serializejson/issues                                                                  |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Noncommercial license** | `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_ |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+| **Commercial license**    | `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_                |
+|                           | ⇒ `Sponsor me ! <https://github.com/sponsors/SmartAudioTools>`_ or `contact me ! <contact@smartaudiotools.com>`_         |
++---------------------------+--------------------------------------------------------------------------------------------------------------------------+
+
+
+**serializejson**  is a python library for fast serialization and deserialization
+of python objects in `JSON <http://json.org>`_  designed as a safe, interoperable and human-readable drop-in replacement for the Python `pickle <https://docs.python.org/3/library/pickle.html>`_ package.
+Complex python object hierarchies are serializable, deserializable or updatable in once, allowing for example to save or restore a complete application state in few lines of code.
+The library is build upon
+`python-rapidjson <https://github.com/python-rapidjson/python-rapidjson>`_,
+`pybase64 <https://github.com/mayeut/pybase64>`_ and
+`blosc <https://github.com/Blosc/python-blosc>`_  for optional `zstandard <https://github.com/facebook/zstd>`_ compression.
+
+Some of the main features:
+
+- supports Python 3.7 (maybe lower) or greater.
+- serializes arbitrary python objects into a dictionary by adding `__class__` ,and eventually `__init__`, `__new__`, `__state__`, `__items__` keys.
+- calls the same objects methods as pickle. Therefore almost all pickable objects are serializable with serializejson without any modification.
+- for not already pickable object, you will allways be able to serialize it by adding methodes to the object or creating plugins for pickle or serializejson.
+- generally 2x slower than pickle for dumping and 3x slower than pickle for loading (on your benchmark) except for big arrays (optimisation will soon be done).
+- serializes and deserializes bytes and bytearray very quickly in base64 thanks to `pybase64 <https://github.com/mayeut/pybase64>`_ and lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
+- serialize properties and attributes with getters and setters if wanted (unlike pickle).
+- json data will still be directly loadable if you have transform some attributes in slots or properties in your code since your last serialization. (unlike pickle)
+- can serialize `__init__(self,..)` arguments by name instead of positions, allowing to skip arguments with defauts values and making json datas robust to a change of `__init__` parameters order.
+- serialized objects take generally less space than when serialized with pickle: for binary data, the 30% increase due to base64 encoding is in general largely compensated using the lossless `blosc <https://github.com/Blosc/python-blosc>`_ compression.
+- serialized objects are human-readable and easy to read. Unlike pickled data, your data will never become unreadable if your code evolves: you will always be able to modify your datas with a text editor (with find & replace for example if you change an attribut name).
+- serialized objects are text and therefore versionable and comparable with versionning and comparaison tools.
+- can safely load untrusted / unauthenticated sources if authorized_classes list parameter is set carefully with strictly necessary objects (unlike pickle).
+- can update existing objects recursively instead of override them. serializejson can be used to save and restore in place a complete application state (⚠ not yet well tested).
+- filters attribute starting with "_" by default (unlike pickle). You can keep them if wanted with `filter_ = False`.
+- numpy arrays can be serialized as lists with automatic conversion in both ways or in a conservative way.
+- supports circular references and serialize only once duplicated objects, using "$ref" key an path to the first occurance in the json : `{"$ref": "root.xxx.elt"}` (⚠ not yet if the object is a list or dictionary).
+- accepts json with comment (// and /\* \*/) if `accept_comments = True`.
+- can automatically recognize objects in json from keys names and recreate them, without the need of `__class__` key, if passed in `recognized_classes`.
+- serializejson is easly interoperable outside of the Python ecosystem with this recognition of objects from keys names or with `__class__` translation between python and other language classes.
+- dump and load support string path.
+- can iteratively encode (with append) and decode (with iterator) a list in json file, which helps saving memory space during the process of serialization and deserialization and useful for logs.
+
+.. warning::
+
+    **⚠** Do not load serializejson files from untrusted / unauthenticated sources without carefully setting the load authorized_classes parameter.
+
+    **⚠** Never dump a dictionary with the `__class__` key, otherwise serializejson will attempt to reconstruct an object when loading the json.
+    Be careful not to allow a user to manually enter a dictionary key somewhere without checking that it is not `__class__`.
+    Due to current limitation of rapidjson we cannot we cannot at the moment efficiently detect dictionaries with the `__class__` key to raise an error.
+
+
+Installation
+============
+
+**Last offical release**
+
+.. code-block::
+
+    pip install serializejson
+
+**Developpement version unreleased**
+
+.. code-block::
+
+    pip install git+https://github.com/SmartAudioTools/serializejson.git
+
+Examples
+================
+
+**Serialization with fonctions API**
+
+.. code-block:: python
+
+    import serializejson
+
+    # serialize in string
+    object1 = set([1,2])
+    dumped1 = serializejson.dumps(object1)
+    loaded1 = serializejson.loads(dumped1)
+    print(dumped1)
+    >{
+    >        "__class__": "set",
+    >        "__init__": [1,2]
+    >}
+
+
+    # serialize in file
+    object2 = set([3,4])
+    serializejson.dump(object2,"dumped2.json")
+    loaded2 = serializejson.load("dumped2.json")
+
+**Serialization with classes based API.**
+
+.. code-block:: python
+
+    import serializejson
+    encoder = serializejson.Encoder()
+    decoder = serializejson.Decoder()
+
+    # serialize in string
+
+    object1 = set([1,2])
+    dumped1 = encoder.dumps(object1)
+    loaded1 = decoder.loads(dumped1)
+    print(dumped1)
+
+    # serialize in file
+    object2 = set([3,4])
+    encoder.dump(object2,"dumped2.json")
+    loaded2 = decoder.load("dumped2.json")
+
+**Update existing object**
+
+.. code-block:: python
+
+    import serializejson
+    object1 = set([1,2])
+    object2 = set([3,4])
+    dumped1 = serializejson.dumps(object1)
+    print(f"id {id(object2)} :  {object2}")
+    serializejson.loads(dumped1,obj = object2, updatables_classes = [set])
+    print(f"id {id(object2)} :  {object2}")
+
+**Iterative serialization and deserialization**
+
+.. code-block:: python
+
+    import serializejson
+    encoder = serializejson.Encoder("my_list.json",indent = None)
+    for elt in range(3):
+        encoder.append(elt)
+    print(open("my_list.json").read())
+    for elt in serializejson.Decoder("my_list.json"):
+        print(elt)
+    >[0,1,2]
+    >0
+    >1
+    >2
+
+More examples and complete documentation `here <https://smartaudiotools.github.io/serializejson/>`_
+
+License
+=======
+
+Copyright 2020 Baptiste de La Gorce
+
+For noncommercial use or thirty-day limited free-trial period commercial use, this project is licensed under the `Prosperity Public License 3.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PROSPERITY.rst>`_.
+
+For non limited commercial use, this project is licensed under the `Patron License 1.0.0 <https://github.com/SmartAudioTools/serializejson/blob/master/LICENSE-PATRON.rst>`_.
+To acquire a license please `contact me <mailto:contact@smartaudiotools.com>`_, or just `sponsor me on GitHub <https://github.com/sponsors/SmartAudioTools>`_ under the appropriate tier ! This funding model helps me making my work sustainable and compensates me for the work it took to write this crate!
+
+Third-party contributions are licensed under `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_ and belong to their respective authors.
+History
+=======
+
+Version 0.3.3
+-------------
+:Date: 2022-10-18
+
+* Big speed improvement for bytes and numpy array serialization
+
+Version 0.3.2
+-------------
+:Date: 2022-10-01
+
+* API changed
+* add better support for cicular reférences and duplicates with {"$ref": ...}
+
+Version 0.2.0
+-------------
+:Date: 2021-02-18
+
+* API changed
+* can serialize dict with no-string keys
+* add support for cicular reférences and duplicates with {"$ref": ...}
+
+
+Version 0.1.0
+-------------
+:Date: 2020-11-28
+
+* change description for pipy
+* add license for pipy
+* enable load of tuple, time.struct_time, Counter, OrderedDict and defaultdict
+
+Version 0.0.4
+-------------
+:Date: 2020-11-24
+	
+* API changed
+* add plugins support
+* add bytes, bytearray and numpy.array compression with blosc zstd
+* fix itertive append and decode (not fully tested).
+* fix dump of numpy types without conversion to python types(not yet numpy.float64)
```

### Comparing `serializejson-0.3.2/serializejson.egg-info/SOURCES.txt` & `serializejson-0.3.3/serializejson.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE-PATRON.rst
 LICENSE-PROSPERITY.rst
 LICENSE.rst
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+./rapidjson/rapidjson.cpp
 SmartFramework/__init__.py
 SmartFramework/files/__init__.py
 SmartFramework/image/__init__.py
 SmartFramework/image/image_conversion.py
 SmartFramework/serialize/__init__.py
 SmartFramework/string/__init__.py
 SmartFramework/string/encodings/__init__.py
@@ -33,8 +34,10 @@
 serializejson/plugins/__init__.py
 serializejson/plugins/module_name.py
 serializejson/plugins/pickle_PyQt5_PySide2.py
 serializejson/plugins/serializejson_PyQt5_PySide2.py
 serializejson/plugins/serializejson_array.py
 serializejson/plugins/serializejson_builtins.py
 serializejson/plugins/serializejson_datetime.py
-serializejson/plugins/serializejson_numpy.py
+serializejson/plugins/serializejson_numpy.py
+tests/test_iterator.py
+tests/test_serialize_vs_pickle.py
```

