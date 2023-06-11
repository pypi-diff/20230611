# Comparing `tmp/mongoengine-jsonschema-0.1.0.tar.gz` & `tmp/mongoengine-jsonschema-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoengine-jsonschema-0.1.0.tar", last modified: Sun Jun 11 08:32:41 2023, max compression
+gzip compressed data, was "mongoengine-jsonschema-0.1.1.tar", last modified: Sun Jun 11 08:40:41 2023, max compression
```

## Comparing `mongoengine-jsonschema-0.1.0.tar` & `mongoengine-jsonschema-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:32:41.015277 mongoengine-jsonschema-0.1.0/
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     1069 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.0/LICENSE
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       32 2023-06-11 08:29:31.000000 mongoengine-jsonschema-0.1.0/MANIFEST.in
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     1283 2023-06-11 08:32:41.015277 mongoengine-jsonschema-0.1.0/PKG-INFO
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     4386 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.0/README.md
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        5 2023-06-11 08:04:58.000000 mongoengine-jsonschema-0.1.0/VERSION
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)      108 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.0/pyproject.toml
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       47 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.0/requirements.txt
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       38 2023-06-11 08:32:41.015277 mongoengine-jsonschema-0.1.0/setup.cfg
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     2433 2023-06-11 08:32:29.000000 mongoengine-jsonschema-0.1.0/setup.py
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:32:41.015277 mongoengine-jsonschema-0.1.0/src/
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:32:41.015277 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema/
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       35 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema/__init__.py
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)    12892 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema/mixin.py
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:32:41.015277 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema.egg-info/
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     1283 2023-06-11 08:32:41.000000 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema.egg-info/PKG-INFO
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)      477 2023-06-11 08:32:41.000000 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema.egg-info/SOURCES.txt
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        1 2023-06-11 08:32:41.000000 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema.egg-info/dependency_links.txt
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        1 2023-06-11 08:32:33.000000 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema.egg-info/not-zip-safe
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       48 2023-06-11 08:32:41.000000 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema.egg-info/requires.txt
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       23 2023-06-11 08:32:41.000000 mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema.egg-info/top_level.txt
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:32:41.015277 mongoengine-jsonschema-0.1.0/tests/
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)    31337 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.0/tests/test_json_schema.py
+drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     1069 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/LICENSE
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       42 2023-06-11 08:37:25.000000 mongoengine-jsonschema-0.1.1/MANIFEST.in
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     5383 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/PKG-INFO
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     4386 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/README.md
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        5 2023-06-11 08:40:29.000000 mongoengine-jsonschema-0.1.1/VERSION
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)      108 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/pyproject.toml
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       47 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/requirements.txt
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       38 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/setup.cfg
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     2251 2023-06-11 08:40:29.000000 mongoengine-jsonschema-0.1.1/setup.py
+drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/src/
+drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema/
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       35 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema/__init__.py
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)    12892 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema/mixin.py
+drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     5383 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/PKG-INFO
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)      477 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/SOURCES.txt
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        1 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/dependency_links.txt
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        1 2023-06-11 08:40:34.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/not-zip-safe
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       48 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/requires.txt
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       23 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/top_level.txt
+drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/tests/
+-rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)    31337 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/tests/test_json_schema.py
```

### Comparing `mongoengine-jsonschema-0.1.0/LICENSE` & `mongoengine-jsonschema-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoengine-jsonschema-0.1.0/README.md` & `mongoengine-jsonschema-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mongoengine-jsonschema-0.1.0/src/mongoengine_jsonschema/mixin.py` & `mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema/mixin.py`

 * *Files identical despite different names*

### Comparing `mongoengine-jsonschema-0.1.0/tests/test_json_schema.py` & `mongoengine-jsonschema-0.1.1/tests/test_json_schema.py`

 * *Files identical despite different names*

