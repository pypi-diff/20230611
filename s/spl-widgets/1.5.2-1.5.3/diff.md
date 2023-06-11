# Comparing `tmp/spl_widgets-1.5.2.tar.gz` & `tmp/spl_widgets-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.5.2.tar", last modified: Fri May 26 16:47:58 2023, max compression
+gzip compressed data, was "spl_widgets-1.5.3.tar", last modified: Sun Jun 11 17:13:03 2023, max compression
```

## Comparing `spl_widgets-1.5.2.tar` & `spl_widgets-1.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:47:58.065102 spl_widgets-1.5.2/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.5.2/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-05-26 16:47:58.064074 spl_widgets-1.5.2/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.5.2/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.5.2/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-05-26 16:47:58.065443 spl_widgets-1.5.2/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1217 2023-05-26 16:47:48.000000 spl_widgets-1.5.2/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:47:57.955145 spl_widgets-1.5.2/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:47:57.985046 spl_widgets-1.5.2/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.5.2/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.5.2/src/spl_widgets/__main__.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:47:58.007470 spl_widgets-1.5.2/src/spl_widgets/autoscorer/
--rw-r--r--   0 colin      (501) staff       (20)    13677 2023-05-26 16:37:32.000000 spl_widgets-1.5.2/src/spl_widgets/autoscorer/autoscore.py
--rw-r--r--   0 colin      (501) staff       (20)    15285 2023-05-26 16:35:21.000000 spl_widgets-1.5.2/src/spl_widgets/autoscorer/autoscorer_gui.py
--rw-r--r--   0 colin      (501) staff       (20)     5387 2023-05-26 16:37:26.000000 spl_widgets-1.5.2/src/spl_widgets/autoscorer/tokenize_to_ipa.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.5.2/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:47:58.008929 spl_widgets-1.5.2/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.5.2/src/spl_widgets/data/cmudict.sqlite
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.5.2/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.5.2/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.5.2/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.5.2/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.5.2/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.5.2/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:47:58.061454 spl_widgets-1.5.2/src/spl_widgets/util/
--rw-r--r--   0 colin      (501) staff       (20)     1195 2023-05-26 16:25:13.000000 spl_widgets-1.5.2/src/spl_widgets/util/color_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3923 2023-05-26 16:25:12.000000 spl_widgets-1.5.2/src/spl_widgets/util/gui_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.5.2/src/spl_widgets/util/sqlite_db.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:47:57.998878 spl_widgets-1.5.2/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-05-26 16:47:57.000000 spl_widgets-1.5.2/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      803 2023-05-26 16:47:57.000000 spl_widgets-1.5.2/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-05-26 16:47:57.000000 spl_widgets-1.5.2/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-05-26 16:47:57.000000 spl_widgets-1.5.2/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)       19 2023-05-26 16:47:57.000000 spl_widgets-1.5.2/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-05-26 16:47:57.000000 spl_widgets-1.5.2/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.201003 spl_widgets-1.5.3/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.5.3/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-06-11 17:13:03.200852 spl_widgets-1.5.3/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.5.3/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.5.3/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-06-11 17:13:03.201047 spl_widgets-1.5.3/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1229 2023-06-11 17:12:37.000000 spl_widgets-1.5.3/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.191795 spl_widgets-1.5.3/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.193911 spl_widgets-1.5.3/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.5.3/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.5.3/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.195527 spl_widgets-1.5.3/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    13677 2023-05-26 16:37:32.000000 spl_widgets-1.5.3/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    15285 2023-05-26 16:35:21.000000 spl_widgets-1.5.3/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5387 2023-05-26 16:37:26.000000 spl_widgets-1.5.3/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.5.3/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.195658 spl_widgets-1.5.3/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.5.3/src/spl_widgets/data/cmudict.sqlite
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.5.3/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.5.3/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.5.3/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.5.3/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.5.3/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.5.3/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.200666 spl_widgets-1.5.3/src/spl_widgets/util/
+-rw-r--r--   0 colin      (501) staff       (20)     1169 2023-05-26 17:14:58.000000 spl_widgets-1.5.3/src/spl_widgets/util/color_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3923 2023-05-26 16:25:12.000000 spl_widgets-1.5.3/src/spl_widgets/util/gui_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.5.3/src/spl_widgets/util/sqlite_db.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-06-11 17:13:03.195089 spl_widgets-1.5.3/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      803 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       28 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-06-11 17:13:03.000000 spl_widgets-1.5.3/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.5.2/LICENSE` & `spl_widgets-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/README.md` & `spl_widgets-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/setup.py` & `spl_widgets-1.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.5.2",
+    version="1.5.3",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
     ],
     package_dir={"": "src"},
     packages=["spl_widgets", "spl_widgets.autoscorer", "spl_widgets.util"],
-    install_requires=['pandas', 'tkinterdnd2'],
+    install_requires=['pandas', 'tkinterdnd2', 'openpyxl'],
     python_requires=">=3.8",
     entry_points='''
         [console_scripts]
         gorilla_clean=spl_widgets.gorilla_clean:main
         tuner=spl_widgets.tuner:main
         stk_swx=spl_widgets.stk_swx:main
         batch_tune=spl_widgets.batch_tune:main
```

### Comparing `spl_widgets-1.5.2/src/spl_widgets/autoscorer/autoscore.py` & `spl_widgets-1.5.3/src/spl_widgets/autoscorer/autoscore.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/autoscorer/autoscorer_gui.py` & `spl_widgets-1.5.3/src/spl_widgets/autoscorer/autoscorer_gui.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/autoscorer/tokenize_to_ipa.py` & `spl_widgets-1.5.3/src/spl_widgets/autoscorer/tokenize_to_ipa.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/batch_tune.py` & `spl_widgets-1.5.3/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.5.3/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.5.3/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/jukemake.py` & `spl_widgets-1.5.3/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/misc_util.py` & `spl_widgets-1.5.3/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/stk_swx.py` & `spl_widgets-1.5.3/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/tune_freq.py` & `spl_widgets-1.5.3/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/tuner.py` & `spl_widgets-1.5.3/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/util/color_util.py` & `spl_widgets-1.5.3/src/spl_widgets/util/color_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from openpyxl.cell.rich_text import TextBlock, CellRichText
 from openpyxl.cell.text import InlineFont
 import re
 
-from pathlib import Path
-
 # This regex is largely simplified now & does not use exact ANSI escape codes
 # because there is literally no reason to, these will never be printed to terminal 
 
 # instead, I use an abbreviated version: \Rabc\C is a red "abc" instead of \x1b[31mabc\x1b[39m
 # because isn't that just so much better
 
 # to get a sense for this working use https://regex101.com/r/LjUtFx/1
```

### Comparing `spl_widgets-1.5.2/src/spl_widgets/util/gui_util.py` & `spl_widgets-1.5.3/src/spl_widgets/util/gui_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets/util/sqlite_db.py` & `spl_widgets-1.5.3/src/spl_widgets/util/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.5.2/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.5.3/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

