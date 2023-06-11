# Comparing `tmp/garmin_ace-0.0.1a7.tar.gz` & `tmp/garmin_ace-0.0.1a8.tar.gz`

## Comparing `garmin_ace-0.0.1a7.tar` & `garmin_ace-0.0.1a8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/Makefile
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/Pipfile
--rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/Pipfile.lock
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/data/app_example.ace
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/data/pa18.ace
--rw-r--r--   0        0        0   206963 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/data/pa18.html
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/data/pa18.org
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/constants.py
--rwxr-xr-x   0        0        0     6044 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/convert.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/decoder.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/encoder.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/models.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/utils.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/html/style.css
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/tests/test_convert.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/tests/test_decode_encode.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/.gitignore
--rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/LICENSE
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/pyproject.toml
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/PKG-INFO
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/Makefile
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/Pipfile
+-rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/Pipfile.lock
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/data/app_example.ace
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/data/pa18.ace
+-rw-r--r--   0        0        0   206963 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/data/pa18.html
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/data/pa18.org
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/constants.py
+-rwxr-xr-x   0        0        0     6044 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/convert.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/decoder.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/encoder.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/models.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/utils.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/html/style.css
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/tests/test_convert.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/tests/test_decode_encode.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/.gitignore
+-rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/LICENSE
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/README.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/pyproject.toml
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/PKG-INFO
```

### Comparing `garmin_ace-0.0.1a7/Pipfile.lock` & `garmin_ace-0.0.1a8/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/data/pa18.ace` & `garmin_ace-0.0.1a8/data/pa18.ace`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/data/pa18.html` & `garmin_ace-0.0.1a8/data/pa18.html`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/data/pa18.org` & `garmin_ace-0.0.1a8/data/pa18.org`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/src/garmin_ace/convert.py` & `garmin_ace-0.0.1a8/src/garmin_ace/convert.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/src/garmin_ace/decoder.py` & `garmin_ace-0.0.1a8/src/garmin_ace/decoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/src/garmin_ace/encoder.py` & `garmin_ace-0.0.1a8/src/garmin_ace/encoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/src/garmin_ace/models.py` & `garmin_ace-0.0.1a8/src/garmin_ace/models.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/src/garmin_ace/utils.py` & `garmin_ace-0.0.1a8/src/garmin_ace/utils.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/tests/test_convert.py` & `garmin_ace-0.0.1a8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/tests/test_decode_encode.py` & `garmin_ace-0.0.1a8/tests/test_decode_encode.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/LICENSE` & `garmin_ace-0.0.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/README.md` & `garmin_ace-0.0.1a8/README.md`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a7/pyproject.toml` & `garmin_ace-0.0.1a8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "garmin_ace"
-version = "0.0.1a7"
+version = "0.0.1a8"
 authors = [
   { name="Xavier Antoviaque", email="xavier@antoviaque.org" },
 ]
 description = "Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "orgparse",
 ]
+include = [
+  "src/html/*",
+]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/antoviaque/garmin-ace"
 "Bug Tracker" = "https://gitlab.com/antoviaque/garmin-ace/-/issues"
 
 [project.scripts]
 ace-convert = "garmin_ace.convert:main"
```

### Comparing `garmin_ace-0.0.1a7/PKG-INFO` & `garmin_ace-0.0.1a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin_ace
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python
 Project-URL: Homepage, https://gitlab.com/antoviaque/garmin-ace
 Project-URL: Bug Tracker, https://gitlab.com/antoviaque/garmin-ace/-/issues
 Author-email: Xavier Antoviaque <xavier@antoviaque.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

