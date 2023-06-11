# Comparing `tmp/garmin_ace-0.0.1a6.tar.gz` & `tmp/garmin_ace-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-DOS/MBR boot sector; partition 1 : ID=0xee, active 0xf0, start-CHS (0x1b5,183,58), end-CHS (0xf9,254,57), startsector 531624835, 4237903599 sectors; partition 3 : ID=0xca, active 0xf0, start-CHS (0x352,3,42), end-CHS (0x3f5,179,46), startsector 265264560, 3469524191 sectors
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `garmin_ace-0.0.1a6.tar` & `garmin_ace-0.0.1a7.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/Makefile
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/Pipfile
--rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/Pipfile.lock
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/data/checklist.ace
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/data/test.org
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/constants.py
--rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/convert.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/decoder.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/encoder.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/models.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/tests.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/.gitignore
--rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/LICENSE
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/pyproject.toml
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/PKG-INFO
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/Makefile
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/Pipfile
+-rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/Pipfile.lock
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/data/app_example.ace
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/data/pa18.ace
+-rw-r--r--   0        0        0   206963 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/data/pa18.html
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/data/pa18.org
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/constants.py
+-rwxr-xr-x   0        0        0     6044 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/convert.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/decoder.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/encoder.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/models.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/garmin_ace/utils.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/src/html/style.css
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/tests/test_convert.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/tests/test_decode_encode.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/.gitignore
+-rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/LICENSE
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/pyproject.toml
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a7/PKG-INFO
```

### Comparing `garmin_ace-0.0.1a6/Pipfile.lock` & `garmin_ace-0.0.1a7/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a6/src/garmin_ace/decoder.py` & `garmin_ace-0.0.1a7/src/garmin_ace/decoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a6/src/garmin_ace/encoder.py` & `garmin_ace-0.0.1a7/src/garmin_ace/encoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a6/src/garmin_ace/models.py` & `garmin_ace-0.0.1a7/src/garmin_ace/models.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a6/src/garmin_ace/utils.py` & `garmin_ace-0.0.1a7/src/garmin_ace/utils.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a6/LICENSE` & `garmin_ace-0.0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a6/README.md` & `garmin_ace-0.0.1a7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,87 @@
+Metadata-Version: 2.1
+Name: garmin_ace
+Version: 0.0.1a7
+Summary: Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python
+Project-URL: Homepage, https://gitlab.com/antoviaque/garmin-ace
+Project-URL: Bug Tracker, https://gitlab.com/antoviaque/garmin-ace/-/issues
+Author-email: Xavier Antoviaque <xavier@antoviaque.org>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: orgparse
+Description-Content-Type: text/markdown
+
 Garmin Aviation Checklist Editor (ACE) - Python Module
 ======================================================
 
-Parse and write ACE files from Python.
+Convert ACE files to/from various formats (HTML, orgmode). Parse and write ACE files from Python.
 
 ## Installation
 
 ```
 $ pip install garmin_ace
 ```
 
 ## Usage
 
-### Converting orgmode checklists to the ACE format
+Display the available formats:
+
+```
+$ ace-convert
+Convert source file to destination file
+Usage: ace-convert <source> <dest>
+Supported source formats are: .org, .ace
+Supported destination formats are: .ace, .html
+```
+
+### Example: Converting an ACE file to HTML and PDF
+
+```
+$ ace-convert checklist.ace checklist.html
+```
+
+You can further convert the HTML document to a PDF file with https://wkhtmltopdf.org/downloads.html
+
+```
+$ wkhtmltopdf checklist.html checklist.pdf
+```
+
+### Example: Converting orgmode checklists to the ACE format
+
+Org mode is a plaintext format, which can be easier to edit and manipulate than the Garmin Checklist Editor app. It expects a simple structure:
+
+```
+* Pre-flight checklist
+** Master: on
+** Lights: on
+** Master: off
+* Startup checklist
+** Master: on
+...
+```
+
+The top level bullet points are the checklist names, and subitems are the checklist items.
+
+To convert it to the other available formats:
 
 ```
 $ ace-convert checklist.org checklist.ace
 ```
 
+or 
+
+```
+$ ace-convert checklist.org checklist.html
+```
+
+See https://orgmode.org/worg/org-syntax.html for details on the format. 
+
 ### Decoding a ACE file to Python objects
 
 ```
 from garmin_ace import ACEFileDecoder
 
 checklists_obj = ACEFileDecoder.read_from_file('checklist.ace')
 ```
```

### Comparing `garmin_ace-0.0.1a6/pyproject.toml` & `garmin_ace-0.0.1a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "garmin_ace"
-version = "0.0.1a6"
+version = "0.0.1a7"
 authors = [
   { name="Xavier Antoviaque", email="xavier@antoviaque.org" },
 ]
 description = "Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

