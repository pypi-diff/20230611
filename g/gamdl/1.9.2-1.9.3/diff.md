# Comparing `tmp/gamdl-1.9.2.tar.gz` & `tmp/gamdl-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-1.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-1.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-1.9.2.tar` & `gamdl-1.9.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1137 2023-06-11 03:23:17.384751 gamdl-1.9.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       56 2023-06-11 03:23:17.384751 gamdl-1.9.2/.gitignore
--rw-r--r--   0        0        0     4010 2023-06-11 03:23:17.384751 gamdl-1.9.2/README.md
--rw-r--r--   0        0        0     7595 2023-06-11 03:23:17.384751 gamdl-1.9.2/gamdl/__init__.py
--rw-r--r--   0        0        0       58 2023-06-11 03:23:17.384751 gamdl-1.9.2/gamdl/__main__.py
--rw-r--r--   0        0        0    18456 2023-06-11 03:23:17.384751 gamdl-1.9.2/gamdl/gamdl.py
--rw-r--r--   0        0        0     2975 2023-06-11 03:23:17.384751 gamdl-1.9.2/gamdl/storefront_ids.py
--rw-r--r--   0        0        0      508 2023-06-11 03:23:17.384751 gamdl-1.9.2/pyproject.toml
--rw-r--r--   0        0        0       30 2023-06-11 03:23:17.384751 gamdl-1.9.2/requirements.txt
--rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 gamdl-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-06-11 04:10:19.102678 gamdl-1.9.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0       56 2023-06-11 04:10:19.102678 gamdl-1.9.3/.gitignore
+-rw-r--r--   0        0        0     4010 2023-06-11 04:10:19.102678 gamdl-1.9.3/README.md
+-rw-r--r--   0        0        0     7619 2023-06-11 04:10:19.106678 gamdl-1.9.3/gamdl/__init__.py
+-rw-r--r--   0        0        0       58 2023-06-11 04:10:19.106678 gamdl-1.9.3/gamdl/__main__.py
+-rw-r--r--   0        0        0    18456 2023-06-11 04:10:19.106678 gamdl-1.9.3/gamdl/gamdl.py
+-rw-r--r--   0        0        0     2975 2023-06-11 04:10:19.106678 gamdl-1.9.3/gamdl/storefront_ids.py
+-rw-r--r--   0        0        0      508 2023-06-11 04:10:19.106678 gamdl-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-06-11 04:10:19.106678 gamdl-1.9.3/requirements.txt
+-rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 gamdl-1.9.3/PKG-INFO
```

### Comparing `gamdl-1.9.2/.github/workflows/main.yml` & `gamdl-1.9.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-1.9.2/README.md` & `gamdl-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `gamdl-1.9.2/gamdl/__init__.py` & `gamdl-1.9.3/gamdl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import shutil
 import traceback
 
 from .gamdl import Gamdl
 
-__version__ = "1.9.2"
+__version__ = "1.9.3"
 
 
 def main():
     for tool in ("MP4Box", "mp4decrypt"):
         if not shutil.which(tool):
             raise Exception(f"{tool} is not on PATH")
     parser = argparse.ArgumentParser(
@@ -94,14 +94,15 @@
     )
     args = parser.parse_args()
     if args.urls_txt:
         _url = []
         for url_txt in args.url:
             with open(url_txt, "r", encoding="utf8") as f:
                 _url.extend(f.read().splitlines())
+        args.url = _url
     dl = Gamdl(
         args.wvd_location,
         args.cookies_location,
         args.disable_music_video_skip,
         args.prefer_hevc,
         args.temp_path,
         args.final_path,
```

### Comparing `gamdl-1.9.2/gamdl/gamdl.py` & `gamdl-1.9.3/gamdl/gamdl.py`

 * *Files identical despite different names*

### Comparing `gamdl-1.9.2/gamdl/storefront_ids.py` & `gamdl-1.9.3/gamdl/storefront_ids.py`

 * *Files identical despite different names*

### Comparing `gamdl-1.9.2/PKG-INFO` & `gamdl-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 1.9.2
+Version: 1.9.3
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pywidevine
 Requires-Dist: pyyaml
 Requires-Dist: m3u8
```

