# Comparing `tmp/pypi_python_translator-1.0.0.tar.gz` & `tmp/pypi_python_translator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_python_translator-1.0.0.tar", last modified: Sun Jun 11 16:07:54 2023, max compression
+gzip compressed data, was "pypi_python_translator-1.0.1.tar", last modified: Sun Jun 11 16:13:58 2023, max compression
```

## Comparing `pypi_python_translator-1.0.0.tar` & `pypi_python_translator-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 16:07:54.519539 pypi_python_translator-1.0.0/
--rw-rw-rw-   0        0        0     3130 2023-06-11 16:07:54.518536 pypi_python_translator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-06-11 16:04:23.000000 pypi_python_translator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 16:07:54.496854 pypi_python_translator-1.0.0/pypi_python_translator.egg-info/
--rw-rw-rw-   0        0        0     3130 2023-06-11 16:07:54.000000 pypi_python_translator-1.0.0/pypi_python_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-11 16:07:54.000000 pypi_python_translator-1.0.0/pypi_python_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 16:07:54.000000 pypi_python_translator-1.0.0/pypi_python_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 16:07:54.000000 pypi_python_translator-1.0.0/pypi_python_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 16:07:54.519539 pypi_python_translator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-06-11 16:07:34.000000 pypi_python_translator-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:07:54.517542 pypi_python_translator-1.0.0/translator/
--rw-rw-rw-   0        0        0     3703 2023-06-11 15:51:10.000000 pypi_python_translator-1.0.0/translator/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-1.0.0/translator/languageExamples.py
--rw-rw-rw-   0        0        0      539 2023-06-11 15:51:15.000000 pypi_python_translator-1.0.0/translator/messages.py
--rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-1.0.0/translator/services.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:13:58.386652 pypi_python_translator-1.0.1/
+-rw-rw-rw-   0        0        0     3130 2023-06-11 16:13:58.385655 pypi_python_translator-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-06-11 16:04:23.000000 pypi_python_translator-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 16:13:58.371341 pypi_python_translator-1.0.1/pypi_python_translator.egg-info/
+-rw-rw-rw-   0        0        0     3130 2023-06-11 16:13:58.000000 pypi_python_translator-1.0.1/pypi_python_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-11 16:13:58.000000 pypi_python_translator-1.0.1/pypi_python_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 16:13:58.000000 pypi_python_translator-1.0.1/pypi_python_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 16:13:58.000000 pypi_python_translator-1.0.1/pypi_python_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 16:13:58.387653 pypi_python_translator-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-06-11 16:13:41.000000 pypi_python_translator-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:13:58.383533 pypi_python_translator-1.0.1/translator/
+-rw-rw-rw-   0        0        0     3736 2023-06-11 16:13:17.000000 pypi_python_translator-1.0.1/translator/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-1.0.1/translator/languageExamples.py
+-rw-rw-rw-   0        0        0      539 2023-06-11 15:51:15.000000 pypi_python_translator-1.0.1/translator/messages.py
+-rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-1.0.1/translator/services.py
```

### Comparing `pypi_python_translator-1.0.0/PKG-INFO` & `pypi_python_translator-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi_python_translator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypi_python_translator-1.0.0/README.md` & `pypi_python_translator-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-1.0.0/pypi_python_translator.egg-info/PKG-INFO` & `pypi_python_translator-1.0.1/pypi_python_translator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-python-translator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypi_python_translator-1.0.0/setup.py` & `pypi_python_translator-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypi_python_translator",
-    version="1.0.0",
+    version="1.0.1",
     author="SForces",
     author_email="osmntn08@gmail.com",
     description="A Python package for translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/pypi_python_translator",
     packages=["translator"],
```

### Comparing `pypi_python_translator-1.0.0/translator/__init__.py` & `pypi_python_translator-1.0.1/translator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
-from services import google_services
-from messages import *
-from languageExamples import *
+from translator.services import google_services
+from translator.messages import *
+from translator.languageExamples import *
 try:
     from googletrans import Translator
     from fuzzywuzzy import fuzz
 except ModuleNotFoundError:
     raise ModuleNotFoundError("To use this program, you need to download those libraries;\npip install googletrans==4.0.0-rc1\npip install fuzzywuzzy")
 def writeservices() -> None:
     """
```

### Comparing `pypi_python_translator-1.0.0/translator/messages.py` & `pypi_python_translator-1.0.1/translator/messages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-1.0.0/translator/services.py` & `pypi_python_translator-1.0.1/translator/services.py`

 * *Files identical despite different names*

