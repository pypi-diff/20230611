# Comparing `tmp/garmin_ace-0.0.1a8.tar.gz` & `tmp/garmin_ace-0.0.1a9.tar.gz`

## Comparing `garmin_ace-0.0.1a8.tar` & `garmin_ace-0.0.1a9.tar`

### file list

```diff
@@ -1,22 +1,6 @@
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/Makefile
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/Pipfile
--rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/Pipfile.lock
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/data/app_example.ace
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/data/pa18.ace
--rw-r--r--   0        0        0   206963 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/data/pa18.html
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/data/pa18.org
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/constants.py
--rwxr-xr-x   0        0        0     6044 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/convert.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/decoder.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/encoder.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/models.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/garmin_ace/utils.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/src/html/style.css
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/tests/test_convert.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/tests/test_decode_encode.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/.gitignore
--rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/LICENSE
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/README.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/pyproject.toml
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a8/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a9/src/html/style.css
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a9/.gitignore
+-rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a9/LICENSE
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a9/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a9/pyproject.toml
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a9/PKG-INFO
```

### Comparing `garmin_ace-0.0.1a8/LICENSE` & `garmin_ace-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a8/README.md` & `garmin_ace-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a8/pyproject.toml` & `garmin_ace-0.0.1a9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "garmin_ace"
-version = "0.0.1a8"
+version = "0.0.1a9"
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
+
+[tool.hatch.build]
 include = [
   "src/html/*",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/antoviaque/garmin-ace"
 "Bug Tracker" = "https://gitlab.com/antoviaque/garmin-ace/-/issues"
```

### Comparing `garmin_ace-0.0.1a8/PKG-INFO` & `garmin_ace-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin_ace
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python
 Project-URL: Homepage, https://gitlab.com/antoviaque/garmin-ace
 Project-URL: Bug Tracker, https://gitlab.com/antoviaque/garmin-ace/-/issues
 Author-email: Xavier Antoviaque <xavier@antoviaque.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

