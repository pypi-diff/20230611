# Comparing `tmp/text_adventures-0.0.2.tar.gz` & `tmp/text_adventures-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_adventures-0.0.2.tar", last modified: Sun Jun 11 06:53:03 2023, max compression
+gzip compressed data, was "text_adventures-0.0.3.tar", last modified: Sun Jun 11 06:56:55 2023, max compression
```

## Comparing `text_adventures-0.0.2.tar` & `text_adventures-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 06:53:03.684811 text_adventures-0.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-11 04:10:14.000000 text_adventures-0.0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1925 2023-06-11 06:53:03.680811 text_adventures-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1116 2023-06-11 06:40:25.000000 text_adventures-0.0.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 06:53:03.684811 text_adventures-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      856 2023-06-11 06:44:15.000000 text_adventures-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 06:53:03.680811 text_adventures-0.0.2/text_adventures/
--rw-r--r--   0 runner    (1000) runner    (1000)     6033 2023-06-11 06:47:22.000000 text_adventures-0.0.2/text_adventures/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      203 2023-06-11 06:34:42.000000 text_adventures-0.0.2/text_adventures/timing.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 06:53:03.680811 text_adventures-0.0.2/text_adventures.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1925 2023-06-11 06:53:03.000000 text_adventures-0.0.2/text_adventures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-06-11 06:53:03.000000 text_adventures-0.0.2/text_adventures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 06:53:03.000000 text_adventures-0.0.2/text_adventures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-11 06:53:03.000000 text_adventures-0.0.2/text_adventures.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-06-11 06:53:03.000000 text_adventures-0.0.2/text_adventures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 06:56:55.910077 text_adventures-0.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-11 04:10:14.000000 text_adventures-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1983 2023-06-11 06:56:55.910077 text_adventures-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1116 2023-06-11 06:40:25.000000 text_adventures-0.0.3/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 06:56:55.910077 text_adventures-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      856 2023-06-11 06:56:08.000000 text_adventures-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 06:56:55.906077 text_adventures-0.0.3/text_adventures/
+-rw-r--r--   0 runner    (1000) runner    (1000)     6033 2023-06-11 06:47:22.000000 text_adventures-0.0.3/text_adventures/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      203 2023-06-11 06:34:42.000000 text_adventures-0.0.3/text_adventures/timing.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 06:56:55.910077 text_adventures-0.0.3/text_adventures.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1983 2023-06-11 06:56:55.000000 text_adventures-0.0.3/text_adventures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-06-11 06:56:55.000000 text_adventures-0.0.3/text_adventures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 06:56:55.000000 text_adventures-0.0.3/text_adventures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-11 06:56:55.000000 text_adventures-0.0.3/text_adventures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-06-11 06:56:55.000000 text_adventures-0.0.3/text_adventures.egg-info/top_level.txt
```

### Comparing `text_adventures-0.0.2/LICENSE` & `text_adventures-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `text_adventures-0.0.2/PKG-INFO` & `text_adventures-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_adventures
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for easily making text adventure games.
 Home-page: https://github.com/Qwerty-Qwerty88/Text-Adventures
 Author: Qwerty Qwerty
 Author-email: personqwertyperson88@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -63,12 +63,18 @@
 - `Interaction`
 
 But you can expect more soon, or if you don't want to wait, you can make your own! There is a _very_ simple `Action` class that you can import to create your own `Action`s.
 
 
 # Change Log
 
-## v0.0.1 (6/10/2023)
-- First release
+## Alpha
+
+### v0.0.3 (6/11/2023)
+- Updated the CHANGELOG
 
-## v0.0.2 (6/11/2023)
-- Updated README to include how to install the package and added more links to the package on PyPI
+### v0.0.2 (6/11/2023)
+- Updated README to include how to install the package
+- Added more links to the package on PyPI
+
+### v0.0.1 (6/10/2023)
+- First release
```

### Comparing `text_adventures-0.0.2/README.md` & `text_adventures-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `text_adventures-0.0.2/setup.py` & `text_adventures-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Games/Entertainment"
 ]
  
 setup(
     name="text_adventures",
-    version="0.0.2",
+    version="0.0.3",
     description="A Python library for easily making text adventure games.",
     long_description=open("README.md").read() + "\n\n" + open("CHANGELOG.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Qwerty-Qwerty88/Text-Adventures",  
     author="Qwerty Qwerty",
     author_email="personqwertyperson88@gmail.com",
     license="MIT",
```

### Comparing `text_adventures-0.0.2/text_adventures/__init__.py` & `text_adventures-0.0.3/text_adventures/__init__.py`

 * *Files identical despite different names*

### Comparing `text_adventures-0.0.2/text_adventures.egg-info/PKG-INFO` & `text_adventures-0.0.3/text_adventures.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-adventures
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for easily making text adventure games.
 Home-page: https://github.com/Qwerty-Qwerty88/Text-Adventures
 Author: Qwerty Qwerty
 Author-email: personqwertyperson88@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -63,12 +63,18 @@
 - `Interaction`
 
 But you can expect more soon, or if you don't want to wait, you can make your own! There is a _very_ simple `Action` class that you can import to create your own `Action`s.
 
 
 # Change Log
 
-## v0.0.1 (6/10/2023)
-- First release
+## Alpha
+
+### v0.0.3 (6/11/2023)
+- Updated the CHANGELOG
 
-## v0.0.2 (6/11/2023)
-- Updated README to include how to install the package and added more links to the package on PyPI
+### v0.0.2 (6/11/2023)
+- Updated README to include how to install the package
+- Added more links to the package on PyPI
+
+### v0.0.1 (6/10/2023)
+- First release
```

