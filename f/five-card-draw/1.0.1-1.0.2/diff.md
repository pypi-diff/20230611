# Comparing `tmp/five_card_draw-1.0.1.tar.gz` & `tmp/five_card_draw-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_card_draw-1.0.1.tar", last modified: Fri Jun  9 00:32:44 2023, max compression
+gzip compressed data, was "five_card_draw-1.0.2.tar", last modified: Sun Jun 11 21:06:49 2023, max compression
```

## Comparing `five_card_draw-1.0.1.tar` & `five_card_draw-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 00:32:44.656040 five_card_draw-1.0.1/
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      663 2023-06-09 00:32:44.657037 five_card_draw-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6556 2023-06-09 00:30:17.000000 five_card_draw-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 00:32:44.645068 five_card_draw-1.0.1/five_card_draw/
--rw-rw-rw-   0        0        0        4 2023-06-09 00:26:49.000000 five_card_draw-1.0.1/five_card_draw/fcd_bank.txt
--rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.1/five_card_draw/fcd_functions.py
--rw-rw-rw-   0        0        0    15612 2023-06-09 00:26:57.000000 five_card_draw-1.0.1/five_card_draw/fcd_pagegui.py
--rw-rw-rw-   0        0        0      466 2023-06-09 00:21:15.000000 five_card_draw-1.0.1/five_card_draw/five_card_draw.py
-drwxrwxrwx   0        0        0        0 2023-06-09 00:32:44.656040 five_card_draw-1.0.1/five_card_draw.egg-info/
--rw-rw-rw-   0        0        0      663 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 00:32:44.000000 five_card_draw-1.0.1/five_card_draw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      308 2023-06-09 00:32:44.658034 five_card_draw-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1832 2023-06-09 00:32:33.000000 five_card_draw-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:06:49.518463 five_card_draw-1.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      663 2023-06-11 21:06:49.518463 five_card_draw-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6556 2023-06-09 00:30:17.000000 five_card_draw-1.0.2/README.md
+-rw-rw-rw-   0        0        0      308 2023-06-11 21:06:49.519460 five_card_draw-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-06-11 21:05:51.000000 five_card_draw-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:06:49.498022 five_card_draw-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 21:06:49.505498 five_card_draw-1.0.2/src/5_card_draw/
+-rw-rw-rw-   0        0        0       86 2023-06-09 00:29:43.000000 five_card_draw-1.0.2/src/5_card_draw/__init__.py
+-rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.2/src/5_card_draw/fcd_functions.py
+-rw-rw-rw-   0        0        0    15610 2023-06-10 22:08:20.000000 five_card_draw-1.0.2/src/5_card_draw/fcd_pagegui.py
+-rw-rw-rw-   0        0        0      466 2023-06-09 00:21:15.000000 five_card_draw-1.0.2/src/5_card_draw/five_card_draw.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:06:49.517466 five_card_draw-1.0.2/src/five_card_draw.egg-info/
+-rw-rw-rw-   0        0        0      663 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-11 21:06:49.000000 five_card_draw-1.0.2/src/five_card_draw.egg-info/top_level.txt
```

### Comparing `five_card_draw-1.0.1/LICENSE.txt` & `five_card_draw-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.1/PKG-INFO` & `five_card_draw-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: five_card_draw
-Version: 1.0.1
+Version: 1.0.2
 Summary: Video Poker application for 5 Card Draw Poker
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `five_card_draw-1.0.1/README.md` & `five_card_draw-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.1/five_card_draw/fcd_functions.py` & `five_card_draw-1.0.2/src/5_card_draw/fcd_functions.py`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.1/five_card_draw/fcd_pagegui.py` & `five_card_draw-1.0.2/src/5_card_draw/fcd_pagegui.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 except ImportError:
     import tkinter as tk
 
 import five_card_draw
 import fcd_functions
 
 local_file_directory = os.path.dirname(os.path.realpath(__file__))
-asset_file_directory = os.path.join(local_file_directory + '\Assets')
+asset_file_directory = os.path.join(local_file_directory + '\data')
 
 def vp_start_gui():
     '''Starting point when module is the main routine.'''
     global root
     global prog_location
     prog_call = sys.argv[0]
     prog_location = os.path.split(prog_call)[0]
```

### Comparing `five_card_draw-1.0.1/five_card_draw.egg-info/PKG-INFO` & `five_card_draw-1.0.2/src/five_card_draw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: five-card-draw
-Version: 1.0.1
+Version: 1.0.2
 Summary: Video Poker application for 5 Card Draw Poker
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `five_card_draw-1.0.1/setup.py` & `five_card_draw-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,41 +7,43 @@
 OR
 Developer Install: "py -m pip install -e ." from this folder.
 
 Publish a Pip Version to PyPi:
 0. Create an account https://pypi.org/account/register/
 1. Install Prequisites: py -m pip install --upgrade pip setuptools wheel twine build
 2. py setup.py sdist bdist_wheel
-3. py twine upload dist/*
+3. py -m twine upload dist/*
 
 '''
 import os
 from pathlib import Path
 import setuptools
 
 requires = [
     'tk',
     'pathlib'
 ]
-
 scripts = [
-    str(Path('five_card_draw','five_card_draw.py')),
-    str(Path('five_card_draw','fcd_pagegui.py')),
-    str(Path('five_card_draw','fcd_functions.py')),
-    str(Path('five_card_draw','fcd_bank.txt'))
+    str(Path('src/5_card_draw','five_card_draw.py'))
 ]
 
 #Package setuptools pypi install for local developer installs
 setuptools.setup(
     name = 'five_card_draw',
-    version = os.getenv('PACKAGE_VERSION', '1.0.1'),
+    version = os.getenv('PACKAGE_VERSION', '1.0.2'),
     description = 'Video Poker application for 5 Card Draw Poker',
     author = 'Richard Albee',
     author_email='Ralbee1@iwu.edu',
-    packages = setuptools.find_packages(),
+    packages=setuptools.find_namespace_packages(where="src"),
+    package_dir={"": "src"},
+    package_data={
+        "five_card_draw": ["*.txt"],
+        "five_card_draw.data": ["*.png"]
+    },
+    include_package_data=True,
     install_requires = requires,
     scripts = scripts,
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Programming Language :: Python',
```

