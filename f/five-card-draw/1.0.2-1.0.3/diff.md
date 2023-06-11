# Comparing `tmp/five_card_draw-1.0.2.tar.gz` & `tmp/five_card_draw-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_card_draw-1.0.2.tar", last modified: Sun Jun 11 21:06:49 2023, max compression
+gzip compressed data, was "five_card_draw-1.0.3.tar", last modified: Sun Jun 11 21:23:12 2023, max compression
```

## Comparing `five_card_draw-1.0.2.tar` & `five_card_draw-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 21:06:49.518463 five_card_draw-1.0.2/
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      663 2023-06-11 21:06:49.518463 five_card_draw-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6556 2023-06-09 00:30:17.000000 five_card_draw-1.0.2/README.md
--rw-rw-rw-   0        0        0      308 2023-06-11 21:06:49.519460 five_card_draw-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-06-11 21:05:51.000000 five_card_draw-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:06:49.498022 five_card_draw-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 21:06:49.505498 five_card_draw-1.0.2/src/5_card_draw/
--rw-rw-rw-   0        0        0       86 2023-06-09 00:29:43.000000 five_card_draw-1.0.2/src/5_card_draw/__init__.py
--rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.2/src/5_card_draw/fcd_functions.py
--rw-rw-rw-   0        0        0    15610 2023-06-10 22:08:20.000000 five_card_draw-1.0.2/src/5_card_draw/fcd_pagegui.py
--rw-rw-rw-   0        0        0      466 2023-06-09 00:21:15.000000 five_card_draw-1.0.2/src/5_card_draw/five_card_draw.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:06:49.517466 five_card_draw-1.0.2/src/five_card_draw.egg-info/
--rw-rw-rw-   0        0        0      663 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 21:23:12.696927 five_card_draw-1.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      653 2023-06-11 21:23:12.697924 five_card_draw-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6556 2023-06-09 00:30:17.000000 five_card_draw-1.0.3/README.md
+-rw-rw-rw-   0        0        0      308 2023-06-11 21:23:12.698922 five_card_draw-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1861 2023-06-11 21:23:04.000000 five_card_draw-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:23:12.681994 five_card_draw-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 21:23:12.689946 five_card_draw-1.0.3/src/5_card_draw/
+-rw-rw-rw-   0        0        0       89 2023-06-11 21:18:27.000000 five_card_draw-1.0.3/src/5_card_draw/__init__.py
+-rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.3/src/5_card_draw/fcd_functions.py
+-rw-rw-rw-   0        0        0    15610 2023-06-10 22:08:20.000000 five_card_draw-1.0.3/src/5_card_draw/fcd_pagegui.py
+-rw-rw-rw-   0        0        0      466 2023-06-09 00:21:15.000000 five_card_draw-1.0.3/src/5_card_draw/five_card_draw.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:23:12.696927 five_card_draw-1.0.3/src/five_card_draw.egg-info/
+-rw-rw-rw-   0        0        0      653 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/top_level.txt
```

### Comparing `five_card_draw-1.0.2/LICENSE.txt` & `five_card_draw-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.2/PKG-INFO` & `five_card_draw-1.0.3/src/five_card_draw.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: five_card_draw
-Version: 1.0.2
-Summary: Video Poker application for 5 Card Draw Poker
+Name: five-card-draw
+Version: 1.0.3
+Summary: 5 Card Draw Video Poker application
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
```

### Comparing `five_card_draw-1.0.2/README.md` & `five_card_draw-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.2/setup.py` & `five_card_draw-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 import setuptools
 
 requires = [
     'tk',
     'pathlib'
 ]
 scripts = [
-    str(Path('src/5_card_draw','five_card_draw.py'))
+    #str(Path('src/5_card_draw','five_card_draw.py'))
 ]
 
 #Package setuptools pypi install for local developer installs
 setuptools.setup(
     name = 'five_card_draw',
-    version = os.getenv('PACKAGE_VERSION', '1.0.2'),
-    description = 'Video Poker application for 5 Card Draw Poker',
+    version = os.getenv('PACKAGE_VERSION', '1.0.3'),
+    description = '5 Card Draw Video Poker application',
     author = 'Richard Albee',
     author_email='Ralbee1@iwu.edu',
     packages=setuptools.find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "five_card_draw": ["*.txt"],
         "five_card_draw.data": ["*.png"]
```

### Comparing `five_card_draw-1.0.2/src/5_card_draw/fcd_functions.py` & `five_card_draw-1.0.3/src/5_card_draw/fcd_functions.py`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.2/src/5_card_draw/fcd_pagegui.py` & `five_card_draw-1.0.3/src/5_card_draw/fcd_pagegui.py`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.2/src/five_card_draw.egg-info/PKG-INFO` & `five_card_draw-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: five-card-draw
-Version: 1.0.2
-Summary: Video Poker application for 5 Card Draw Poker
+Name: five_card_draw
+Version: 1.0.3
+Summary: 5 Card Draw Video Poker application
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
```

