# Comparing `tmp/epy-reader-2023.2.8.tar.gz` & `tmp/epy_reader-2023.6.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epy-reader-2023.2.8.tar", last modified: Wed Feb  8 15:29:33 2023, max compression
+gzip compressed data, was "epy_reader-2023.6.11.tar", max compression
```

## Comparing `epy-reader-2023.2.8.tar` & `epy_reader-2023.6.11.tar`

### file list

```diff
@@ -1,65 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:29:33.115171 epy-reader-2023.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-02-08 15:29:33.115171 epy-reader-2023.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 15:29:33.115171 epy-reader-2023.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:29:33.107171 epy-reader-2023.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:29:33.111171 epy-reader-2023.2.8/src/epy_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:29:33.111171 epy-reader-2023.2.8/src/epy_reader/ebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/ebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/ebooks/azw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/ebooks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/ebooks/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/ebooks/fictionbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/ebooks/mobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/ebooks/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    69791 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:29:33.115171 epy-reader-2023.2.8/src/epy_reader/speakers/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/speakers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/speakers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/speakers/mimic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/speakers/pico.py
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:29:33.115171 epy-reader-2023.2.8/src/epy_reader/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:29:33.115171 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9189 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/compatibility_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    44186 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/kindleunpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    38999 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_html.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    22375 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_k8proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_k8resc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_ncx.py
--rw-r--r--   0 runner    (1001) docker     (123)    31813 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_opf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_pagemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_sectioner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19270 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_uncompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19828 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobiml2xhtml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/unipath.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/unpack_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-02-08 15:29:11.000000 epy-reader-2023.2.8/src/epy_reader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:29:33.111171 epy-reader-2023.2.8/src/epy_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-02-08 15:29:33.000000 epy-reader-2023.2.8/src/epy_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-02-08 15:29:33.000000 epy-reader-2023.2.8/src/epy_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 15:29:33.000000 epy-reader-2023.2.8/src/epy_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-08 15:29:33.000000 epy-reader-2023.2.8/src/epy_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-08 15:29:33.000000 epy-reader-2023.2.8/src/epy_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-08 15:29:33.000000 epy-reader-2023.2.8/src/epy_reader.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35081 2022-01-25 03:15:01.528365 epy_reader-2023.6.11/LICENSE
+-rw-r--r--   0        0        0     6161 2023-06-11 05:07:05.548062 epy_reader-2023.6.11/README.md
+-rw-r--r--   0        0        0     1084 2023-06-11 05:07:43.015779 epy_reader-2023.6.11/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-06-11 05:07:26.457672 epy_reader-2023.6.11/src/epy_reader/__init__.py
+-rw-r--r--   0        0        0      560 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/__main__.py
+-rw-r--r--   0        0        0     6480 2023-02-08 15:24:23.626253 epy_reader-2023.6.11/src/epy_reader/board.py
+-rw-r--r--   0        0        0     5439 2022-10-04 02:29:33.058308 epy_reader-2023.6.11/src/epy_reader/cli.py
+-rw-r--r--   0        0        0     2754 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/config.py
+-rw-r--r--   0        0        0      344 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/ebooks/__init__.py
+-rw-r--r--   0        0        0      783 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/ebooks/azw.py
+-rw-r--r--   0        0        0     1484 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/ebooks/base.py
+-rw-r--r--   0        0        0     7787 2022-10-03 13:50:52.653886 epy_reader-2023.6.11/src/epy_reader/ebooks/epub.py
+-rw-r--r--   0        0        0     3029 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/ebooks/fictionbook.py
+-rw-r--r--   0        0        0     2462 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/ebooks/mobi.py
+-rw-r--r--   0        0        0     1517 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/ebooks/url.py
+-rw-r--r--   0        0        0     1804 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/lib.py
+-rw-r--r--   0        0        0     5967 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/models.py
+-rw-r--r--   0        0        0    16044 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/parser.py
+-rw-r--r--   0        0        0    69818 2023-06-11 05:09:32.451274 epy_reader-2023.6.11/src/epy_reader/reader.py
+-rw-r--r--   0        0        0     3467 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/settings.py
+-rw-r--r--   0        0        0      309 2023-06-11 05:07:05.548062 epy_reader-2023.6.11/src/epy_reader/speakers/__init__.py
+-rw-r--r--   0        0        0      598 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/speakers/base.py
+-rw-r--r--   0        0        0     1047 2023-06-11 05:07:05.548062 epy_reader-2023.6.11/src/epy_reader/speakers/gtts_mpv.py
+-rw-r--r--   0        0        0      776 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/speakers/mimic.py
+-rw-r--r--   0        0        0     1158 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/speakers/pico.py
+-rw-r--r--   0        0        0     6873 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/state.py
+-rw-r--r--   0        0        0       73 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/__init__.py
+-rwxr-xr-x   0        0        0     9189 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/compatibility_utils.py
+-rw-r--r--   0        0        0    44186 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/kindleunpack.py
+-rw-r--r--   0        0        0     8864 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_cover.py
+-rw-r--r--   0        0        0    16612 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_dict.py
+-rw-r--r--   0        0        0    38999 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_header.py
+-rw-r--r--   0        0        0    20849 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_html.py
+-rw-r--r--   0        0        0    11224 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_index.py
+-rw-r--r--   0        0        0    22375 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_k8proc.py
+-rw-r--r--   0        0        0    10163 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_k8resc.py
+-rw-r--r--   0        0        0     6813 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_nav.py
+-rw-r--r--   0        0        0     9838 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_ncx.py
+-rw-r--r--   0        0        0    31813 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_opf.py
+-rw-r--r--   0        0        0     5675 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_pagemap.py
+-rw-r--r--   0        0        0     5260 2022-10-02 14:21:00.134726 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_sectioner.py
+-rwxr-xr-x   0        0        0    19270 2022-10-02 14:21:00.138727 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_split.py
+-rw-r--r--   0        0        0     4309 2022-10-02 14:21:00.138727 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_uncompress.py
+-rw-r--r--   0        0        0     8654 2022-10-02 14:21:00.138727 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_utils.py
+-rwxr-xr-x   0        0        0    19828 2022-10-02 14:21:00.138727 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobiml2xhtml.py
+-rwxr-xr-x   0        0        0     3144 2022-10-02 14:21:00.138727 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/unipath.py
+-rw-r--r--   0        0        0     7158 2022-10-02 14:21:00.138727 epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/unpack_structure.py
+-rw-r--r--   0        0        0      122 2022-10-02 14:21:00.138727 epy_reader-2023.6.11/src/epy_reader/tools/__init__.py
+-rw-r--r--   0        0        0    14198 2023-06-11 05:07:05.548062 epy_reader-2023.6.11/src/epy_reader/utils.py
+-rw-r--r--   0        0        0     7288 1970-01-01 00:00:00.000000 epy_reader-2023.6.11/setup.py
+-rw-r--r--   0        0        0     6928 1970-01-01 00:00:00.000000 epy_reader-2023.6.11/PKG-INFO
```

### Comparing `epy-reader-2023.2.8/LICENSE` & `epy_reader-2023.6.11/LICENSE`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/PKG-INFO` & `epy_reader-2023.6.11/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: epy-reader
-Version: 2023.2.8
-Summary: Terminal/CLI Ebook (epub, fb2, mobi, azw3) Reader
+Version: 2023.6.11
+Summary: TUI Ebook Reader
 Home-page: https://github.com/wustho/epy
+License: GPL-3.0
+Keywords: ebook,epub,epub3,fb2,mobi,azw3,TUI,ebook reader
 Author: Benawi Adha
 Author-email: benawiadha@gmail.com
-License: GPL-3.0
-Keywords: epub,epub3,fb2,mobi,azw3,CLI,Terminal,Reader
-Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: windows-curses; platform_system == "Windows"
+Project-URL: Repository, https://github.com/wustho/epy
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # `$ epy`
 
 [![Downloads](https://static.pepy.tech/personalized-badge/epy-reader?period=month&units=none&left_color=grey&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/epy-reader)
 
 <a href='https://ko-fi.com/P5P4IDCX2' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi2.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 
@@ -53,15 +57,15 @@
   ```shell
   pip3 install git+https://github.com/wustho/epy
   ```
 
 - Via AUR
 
   ```shell
-  yay -S epy-git
+  yay -S epy-ereader-git
   ```
 
 - Windows Binary
 
   Standalone binary for Windows is available at [release page](https://github.com/wustho/epy/releases).
 
 ## Usage
@@ -152,14 +156,15 @@
 
 To get Text-to-Speech (TTS) support, external TTS engine is necessary.
 
 List of supported engines:
 
 - `mimic`
 - `pico2wave`
+- `gtts-mpv` (requires both [gTTS](https://pypi.org/project/gTTS) and [MPV](https://www.mpv.io))
 
 ## Dictionary
 
 To use "Define Word" you will have to install an external dictionary cli program (`sdcv`, `dict` or `wkdict`). After you've done that, it is recommended to manually modify the configuration.json file, and set your desired dictionary there, so everything works properly.
 
 After that you will be able to find definition of word by pressing `d`, and aprompt will appear to let you type in word to define.
 
@@ -180,7 +185,8 @@
 
 - `v2022.1.23`: Library implementation: ability to switch ebook from reading history
   inside epy (default key: `R`).
 
 - `v2022.2.5`: Fix process.join() issue for unstarted process.
 
 - `v2022.10.2`: Major breakdown `epy.py` module into package structure for easier development.
+
```

#### html2text {}

```diff
@@ -1,81 +1,86 @@
-Metadata-Version: 2.1 Name: epy-reader Version: 2023.2.8 Summary: Terminal/CLI
-Ebook (epub, fb2, mobi, azw3) Reader Home-page: https://github.com/wustho/epy
-Author: Benawi Adha Author-email: benawiadha@gmail.com License: GPL-3.0
-Keywords: epub,epub3,fb2,mobi,azw3,CLI,Terminal,Reader Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # `$ epy` [![Downloads](https://static.pepy.tech/personalized-badge/
+Metadata-Version: 2.1 Name: epy-reader Version: 2023.6.11 Summary: TUI Ebook
+Reader Home-page: https://github.com/wustho/epy License: GPL-3.0 Keywords:
+ebook,epub,epub3,fb2,mobi,azw3,TUI,ebook reader Author: Benawi Adha Author-
+email: benawiadha@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License ::
+OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: windows-curses; platform_system == "Windows" Project-URL:
+Repository, https://github.com/wustho/epy Description-Content-Type: text/
+markdown # `$ epy` [![Downloads](https://static.pepy.tech/personalized-badge/
 epy-
 reader?period=month&units=none&left_color=grey&right_color=brightgreen&left_text=downloads/
 month)](https://pepy.tech/project/epy-reader) [Buy_Me_a_Coffee_at_ko-fi.com] !
 [screenshot](https://raw.githubusercontent.com/wustho/epy/master/
 screenshot.png) CLI Ebook Reader. This is just a fork of [epr](https://
 github.com/wustho/epr) with these extra features: - Supported formats: - Epub
 (.epub, .epub3) - FictionBook (.fb2) - Mobi (.mobi) - AZW3 (.azw, .azw3) -
 [URL](#url-support) - Reading progress percentage - Bookmarks - External
 dictionary integration (`sdcv`, `dict` or `wkdict`) - Inline formats: **bold**
 and _italic_ (depend on terminal and font capability. Italic only supported in
 python>=3.7) - Text-to-Speech (with additional setup, read [below](#text-to-
 speech)) - [Double Spread](#double-spread) - Seamless (disabled by default,
 read [below](#reading-tips-using-epy)) ## Installation - Via PyPI (Linux and
 Mac OS) ```shell pip3 install epy-reader ``` - Via Pip+Git ```shell pip3
-install git+https://github.com/wustho/epy ``` - Via AUR ```shell yay -S epy-git
-``` - Windows Binary Standalone binary for Windows is available at [release
-page](https://github.com/wustho/epy/releases). ## Usage - `epy /path/to/your/
-book/book.epub` (Remember to make sure your book's title doesn't contain any
-spaces) - **c** Switching the color profile - **Shift + h** Previous chapter -
-**Shift + l** Next chapter - **Shift + g** Skip to the end of the chapter -
-**g** Skip to the beginning of the chapter - **Shift + m** Show metadata of the
-book - **t** Table of contents - **/** Search - **b** Add bookmark - **Shift +
-b** Show bookmarks - **q** Quit - **-** Shrink the text - **+** Enlarge the
-text - **o** Open an image - **s** Show or hide progress ## Color profiles In
-the config file you will see the following section. ``` "DarkColorFG": 47,
-"DarkColorBG": 235, "LightColorFG": 238, "LightColorBG": 253, ``` Change the
-values by using this image. (Make sure to ignore zeros at the beginning, it
-won't launch otherwise.) ![image](https://user-images.githubusercontent.com/
-108401269/198876974-c8420de1-b256-42fd-9a09-3a69c5019608.png) ## Reading Tips
-Using Epy When reading using `epy` you might occasionally find triple asteriks
-`***`. That means you reach the end of some section in your ebook and the next
-line (right after those three asteriks, which is in new section) will start at
-the top of the page. This might be disorienting, so the best way to get
-seamless reading experience is by using next-page control (`space`, `l` or
-`Right`) instead of next-line control (`j` or `Down`). If you really want to
-get seamless reading experience, you can set `SeamlessBetweenChapters` to
-`true` in configuration file. But it has its drawback with more memory usage,
-that's why it's disabled by default. ## Configuration File Config file is
-available in json format which is located at: - Linux and Mac OS: `~/.config/
-epy/configuration.json` or `~/.epy/configuration.json` - Windows:
-`%USERPROFILE%\.epy\configuration.json` ## URL Support You can read online
-books like: short stories, fan fiction, etc. using `epy` with an url as cli
-argument. Pretty useful when you want to read with less distraction. `epy` will
-also remember your reading progress online. eg. You can read [Moby Dick from
-gutenberg](https://www.gutenberg.org/files/2701/2701-h/2701-h.htm) directly
-with: ```shell $ epy https://www.gutenberg.org/files/2701/2701-h/2701-h.htm ```
-But note that `epy` will never be a web browser, it's simply a TUI program to
-read your favorite fiction stories in the comfort of a terminal. So please do
-not expect for web browser features to be implemented in `epy`. ## Using Mouse
-Although mouse support is useful when running `epy` on Termux Android, itâs
-disabled by default since most people find it intrusive when using `epy` in
-desktop. But you can enable it by setting `MouseSupport` to `true` in config
-file. | Key | Action | | --- | --- | | `Left Click` (right side of screen) |
-next page | | `Left Click` (left side of screen) | prev page | | `Right Click`
-| ToC | | `Scroll Up` | scroll up | | `Scroll Down` | scroll down | | `Ctrl` +
-`Scroll Up` | increase text width | | `Ctrl` + `Scroll Down` | decrease text
-width | ## Text-to-Speech To get Text-to-Speech (TTS) support, external TTS
-engine is necessary. List of supported engines: - `mimic` - `pico2wave` ##
-Dictionary To use "Define Word" you will have to install an external dictionary
-cli program (`sdcv`, `dict` or `wkdict`). After you've done that, it is
-recommended to manually modify the configuration.json file, and set your
-desired dictionary there, so everything works properly. After that you will be
-able to find definition of word by pressing `d`, and aprompt will appear to let
-you type in word to define. ## Double Spread Double spread is intended to mimic
-the behaviour of real book, so line scrolling navigation will act as scrolling
-page and textwidth is not adjustable. ## Changelog - `v2021.10.23`: Major
+install git+https://github.com/wustho/epy ``` - Via AUR ```shell yay -S epy-
+ereader-git ``` - Windows Binary Standalone binary for Windows is available at
+[release page](https://github.com/wustho/epy/releases). ## Usage - `epy /path/
+to/your/book/book.epub` (Remember to make sure your book's title doesn't
+contain any spaces) - **c** Switching the color profile - **Shift + h**
+Previous chapter - **Shift + l** Next chapter - **Shift + g** Skip to the end
+of the chapter - **g** Skip to the beginning of the chapter - **Shift + m**
+Show metadata of the book - **t** Table of contents - **/** Search - **b** Add
+bookmark - **Shift + b** Show bookmarks - **q** Quit - **-** Shrink the text -
+**+** Enlarge the text - **o** Open an image - **s** Show or hide progress ##
+Color profiles In the config file you will see the following section. ```
+"DarkColorFG": 47, "DarkColorBG": 235, "LightColorFG": 238, "LightColorBG":
+253, ``` Change the values by using this image. (Make sure to ignore zeros at
+the beginning, it won't launch otherwise.) ![image](https://user-
+images.githubusercontent.com/108401269/198876974-c8420de1-b256-42fd-9a09-
+3a69c5019608.png) ## Reading Tips Using Epy When reading using `epy` you might
+occasionally find triple asteriks `***`. That means you reach the end of some
+section in your ebook and the next line (right after those three asteriks,
+which is in new section) will start at the top of the page. This might be
+disorienting, so the best way to get seamless reading experience is by using
+next-page control (`space`, `l` or `Right`) instead of next-line control (`j`
+or `Down`). If you really want to get seamless reading experience, you can set
+`SeamlessBetweenChapters` to `true` in configuration file. But it has its
+drawback with more memory usage, that's why it's disabled by default. ##
+Configuration File Config file is available in json format which is located at:
+- Linux and Mac OS: `~/.config/epy/configuration.json` or `~/.epy/
+configuration.json` - Windows: `%USERPROFILE%\.epy\configuration.json` ## URL
+Support You can read online books like: short stories, fan fiction, etc. using
+`epy` with an url as cli argument. Pretty useful when you want to read with
+less distraction. `epy` will also remember your reading progress online. eg.
+You can read [Moby Dick from gutenberg](https://www.gutenberg.org/files/2701/
+2701-h/2701-h.htm) directly with: ```shell $ epy https://www.gutenberg.org/
+files/2701/2701-h/2701-h.htm ``` But note that `epy` will never be a web
+browser, it's simply a TUI program to read your favorite fiction stories in the
+comfort of a terminal. So please do not expect for web browser features to be
+implemented in `epy`. ## Using Mouse Although mouse support is useful when
+running `epy` on Termux Android, itâs disabled by default since most people
+find it intrusive when using `epy` in desktop. But you can enable it by setting
+`MouseSupport` to `true` in config file. | Key | Action | | --- | --- | | `Left
+Click` (right side of screen) | next page | | `Left Click` (left side of
+screen) | prev page | | `Right Click` | ToC | | `Scroll Up` | scroll up | |
+`Scroll Down` | scroll down | | `Ctrl` + `Scroll Up` | increase text width | |
+`Ctrl` + `Scroll Down` | decrease text width | ## Text-to-Speech To get Text-
+to-Speech (TTS) support, external TTS engine is necessary. List of supported
+engines: - `mimic` - `pico2wave` - `gtts-mpv` (requires both [gTTS](https://
+pypi.org/project/gTTS) and [MPV](https://www.mpv.io)) ## Dictionary To use
+"Define Word" you will have to install an external dictionary cli program
+(`sdcv`, `dict` or `wkdict`). After you've done that, it is recommended to
+manually modify the configuration.json file, and set your desired dictionary
+there, so everything works properly. After that you will be able to find
+definition of word by pressing `d`, and aprompt will appear to let you type in
+word to define. ## Double Spread Double spread is intended to mimic the
+behaviour of real book, so line scrolling navigation will act as scrolling page
+and textwidth is not adjustable. ## Changelog - `v2021.10.23`: Major
 refactoring which harness a lot of new stuff in `python>=3.7` and `epy` won't
 be backward compatible with older python version and older configuration. -
 `v2022.1.8`: Change in configuration and reading states schema that is not
 backward compatible. So if error is encountered, deleting the configuration and
 states file might fix the issue. - `v2022.1.15`: Early implementation of URL
 support, table of contents isn't available for now. - `v2022.1.23`: Library
 implementation: ability to switch ebook from reading history inside epy
```

### Comparing `epy-reader-2023.2.8/README.md` & `epy_reader-2023.6.11/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
   ```shell
   pip3 install git+https://github.com/wustho/epy
   ```
 
 - Via AUR
 
   ```shell
-  yay -S epy-git
+  yay -S epy-ereader-git
   ```
 
 - Windows Binary
 
   Standalone binary for Windows is available at [release page](https://github.com/wustho/epy/releases).
 
 ## Usage
@@ -136,14 +136,15 @@
 
 To get Text-to-Speech (TTS) support, external TTS engine is necessary.
 
 List of supported engines:
 
 - `mimic`
 - `pico2wave`
+- `gtts-mpv` (requires both [gTTS](https://pypi.org/project/gTTS) and [MPV](https://www.mpv.io))
 
 ## Dictionary
 
 To use "Define Word" you will have to install an external dictionary cli program (`sdcv`, `dict` or `wkdict`). After you've done that, it is recommended to manually modify the configuration.json file, and set your desired dictionary there, so everything works properly.
 
 After that you will be able to find definition of word by pressing `d`, and aprompt will appear to let you type in word to define.
```

#### html2text {}

```diff
@@ -8,66 +8,68 @@
 [URL](#url-support) - Reading progress percentage - Bookmarks - External
 dictionary integration (`sdcv`, `dict` or `wkdict`) - Inline formats: **bold**
 and _italic_ (depend on terminal and font capability. Italic only supported in
 python>=3.7) - Text-to-Speech (with additional setup, read [below](#text-to-
 speech)) - [Double Spread](#double-spread) - Seamless (disabled by default,
 read [below](#reading-tips-using-epy)) ## Installation - Via PyPI (Linux and
 Mac OS) ```shell pip3 install epy-reader ``` - Via Pip+Git ```shell pip3
-install git+https://github.com/wustho/epy ``` - Via AUR ```shell yay -S epy-git
-``` - Windows Binary Standalone binary for Windows is available at [release
-page](https://github.com/wustho/epy/releases). ## Usage - `epy /path/to/your/
-book/book.epub` (Remember to make sure your book's title doesn't contain any
-spaces) - **c** Switching the color profile - **Shift + h** Previous chapter -
-**Shift + l** Next chapter - **Shift + g** Skip to the end of the chapter -
-**g** Skip to the beginning of the chapter - **Shift + m** Show metadata of the
-book - **t** Table of contents - **/** Search - **b** Add bookmark - **Shift +
-b** Show bookmarks - **q** Quit - **-** Shrink the text - **+** Enlarge the
-text - **o** Open an image - **s** Show or hide progress ## Color profiles In
-the config file you will see the following section. ``` "DarkColorFG": 47,
-"DarkColorBG": 235, "LightColorFG": 238, "LightColorBG": 253, ``` Change the
-values by using this image. (Make sure to ignore zeros at the beginning, it
-won't launch otherwise.) ![image](https://user-images.githubusercontent.com/
-108401269/198876974-c8420de1-b256-42fd-9a09-3a69c5019608.png) ## Reading Tips
-Using Epy When reading using `epy` you might occasionally find triple asteriks
-`***`. That means you reach the end of some section in your ebook and the next
-line (right after those three asteriks, which is in new section) will start at
-the top of the page. This might be disorienting, so the best way to get
-seamless reading experience is by using next-page control (`space`, `l` or
-`Right`) instead of next-line control (`j` or `Down`). If you really want to
-get seamless reading experience, you can set `SeamlessBetweenChapters` to
-`true` in configuration file. But it has its drawback with more memory usage,
-that's why it's disabled by default. ## Configuration File Config file is
-available in json format which is located at: - Linux and Mac OS: `~/.config/
-epy/configuration.json` or `~/.epy/configuration.json` - Windows:
-`%USERPROFILE%\.epy\configuration.json` ## URL Support You can read online
-books like: short stories, fan fiction, etc. using `epy` with an url as cli
-argument. Pretty useful when you want to read with less distraction. `epy` will
-also remember your reading progress online. eg. You can read [Moby Dick from
-gutenberg](https://www.gutenberg.org/files/2701/2701-h/2701-h.htm) directly
-with: ```shell $ epy https://www.gutenberg.org/files/2701/2701-h/2701-h.htm ```
-But note that `epy` will never be a web browser, it's simply a TUI program to
-read your favorite fiction stories in the comfort of a terminal. So please do
-not expect for web browser features to be implemented in `epy`. ## Using Mouse
-Although mouse support is useful when running `epy` on Termux Android, itâs
-disabled by default since most people find it intrusive when using `epy` in
-desktop. But you can enable it by setting `MouseSupport` to `true` in config
-file. | Key | Action | | --- | --- | | `Left Click` (right side of screen) |
-next page | | `Left Click` (left side of screen) | prev page | | `Right Click`
-| ToC | | `Scroll Up` | scroll up | | `Scroll Down` | scroll down | | `Ctrl` +
-`Scroll Up` | increase text width | | `Ctrl` + `Scroll Down` | decrease text
-width | ## Text-to-Speech To get Text-to-Speech (TTS) support, external TTS
-engine is necessary. List of supported engines: - `mimic` - `pico2wave` ##
-Dictionary To use "Define Word" you will have to install an external dictionary
-cli program (`sdcv`, `dict` or `wkdict`). After you've done that, it is
-recommended to manually modify the configuration.json file, and set your
-desired dictionary there, so everything works properly. After that you will be
-able to find definition of word by pressing `d`, and aprompt will appear to let
-you type in word to define. ## Double Spread Double spread is intended to mimic
-the behaviour of real book, so line scrolling navigation will act as scrolling
-page and textwidth is not adjustable. ## Changelog - `v2021.10.23`: Major
+install git+https://github.com/wustho/epy ``` - Via AUR ```shell yay -S epy-
+ereader-git ``` - Windows Binary Standalone binary for Windows is available at
+[release page](https://github.com/wustho/epy/releases). ## Usage - `epy /path/
+to/your/book/book.epub` (Remember to make sure your book's title doesn't
+contain any spaces) - **c** Switching the color profile - **Shift + h**
+Previous chapter - **Shift + l** Next chapter - **Shift + g** Skip to the end
+of the chapter - **g** Skip to the beginning of the chapter - **Shift + m**
+Show metadata of the book - **t** Table of contents - **/** Search - **b** Add
+bookmark - **Shift + b** Show bookmarks - **q** Quit - **-** Shrink the text -
+**+** Enlarge the text - **o** Open an image - **s** Show or hide progress ##
+Color profiles In the config file you will see the following section. ```
+"DarkColorFG": 47, "DarkColorBG": 235, "LightColorFG": 238, "LightColorBG":
+253, ``` Change the values by using this image. (Make sure to ignore zeros at
+the beginning, it won't launch otherwise.) ![image](https://user-
+images.githubusercontent.com/108401269/198876974-c8420de1-b256-42fd-9a09-
+3a69c5019608.png) ## Reading Tips Using Epy When reading using `epy` you might
+occasionally find triple asteriks `***`. That means you reach the end of some
+section in your ebook and the next line (right after those three asteriks,
+which is in new section) will start at the top of the page. This might be
+disorienting, so the best way to get seamless reading experience is by using
+next-page control (`space`, `l` or `Right`) instead of next-line control (`j`
+or `Down`). If you really want to get seamless reading experience, you can set
+`SeamlessBetweenChapters` to `true` in configuration file. But it has its
+drawback with more memory usage, that's why it's disabled by default. ##
+Configuration File Config file is available in json format which is located at:
+- Linux and Mac OS: `~/.config/epy/configuration.json` or `~/.epy/
+configuration.json` - Windows: `%USERPROFILE%\.epy\configuration.json` ## URL
+Support You can read online books like: short stories, fan fiction, etc. using
+`epy` with an url as cli argument. Pretty useful when you want to read with
+less distraction. `epy` will also remember your reading progress online. eg.
+You can read [Moby Dick from gutenberg](https://www.gutenberg.org/files/2701/
+2701-h/2701-h.htm) directly with: ```shell $ epy https://www.gutenberg.org/
+files/2701/2701-h/2701-h.htm ``` But note that `epy` will never be a web
+browser, it's simply a TUI program to read your favorite fiction stories in the
+comfort of a terminal. So please do not expect for web browser features to be
+implemented in `epy`. ## Using Mouse Although mouse support is useful when
+running `epy` on Termux Android, itâs disabled by default since most people
+find it intrusive when using `epy` in desktop. But you can enable it by setting
+`MouseSupport` to `true` in config file. | Key | Action | | --- | --- | | `Left
+Click` (right side of screen) | next page | | `Left Click` (left side of
+screen) | prev page | | `Right Click` | ToC | | `Scroll Up` | scroll up | |
+`Scroll Down` | scroll down | | `Ctrl` + `Scroll Up` | increase text width | |
+`Ctrl` + `Scroll Down` | decrease text width | ## Text-to-Speech To get Text-
+to-Speech (TTS) support, external TTS engine is necessary. List of supported
+engines: - `mimic` - `pico2wave` - `gtts-mpv` (requires both [gTTS](https://
+pypi.org/project/gTTS) and [MPV](https://www.mpv.io)) ## Dictionary To use
+"Define Word" you will have to install an external dictionary cli program
+(`sdcv`, `dict` or `wkdict`). After you've done that, it is recommended to
+manually modify the configuration.json file, and set your desired dictionary
+there, so everything works properly. After that you will be able to find
+definition of word by pressing `d`, and aprompt will appear to let you type in
+word to define. ## Double Spread Double spread is intended to mimic the
+behaviour of real book, so line scrolling navigation will act as scrolling page
+and textwidth is not adjustable. ## Changelog - `v2021.10.23`: Major
 refactoring which harness a lot of new stuff in `python>=3.7` and `epy` won't
 be backward compatible with older python version and older configuration. -
 `v2022.1.8`: Change in configuration and reading states schema that is not
 backward compatible. So if error is encountered, deleting the configuration and
 states file might fix the issue. - `v2022.1.15`: Early implementation of URL
 support, table of contents isn't available for now. - `v2022.1.23`: Library
 implementation: ability to switch ebook from reading history inside epy
```

### Comparing `epy-reader-2023.2.8/pyproject.toml` & `epy_reader-2023.6.11/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epy-reader"
-version = "2023.2.8"
+version = "2023.6.11"
 description = "TUI Ebook Reader"
 authors = ["Benawi Adha <benawiadha@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/wustho/epy"
 keywords = ["ebook", "epub", "epub3", "fb2", "mobi", "azw3", "TUI", "ebook reader"]
 packages = [
```

### Comparing `epy-reader-2023.2.8/src/epy_reader/__main__.py` & `epy_reader-2023.6.11/src/epy_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/board.py` & `epy_reader-2023.6.11/src/epy_reader/board.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/cli.py` & `epy_reader-2023.6.11/src/epy_reader/cli.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/config.py` & `epy_reader-2023.6.11/src/epy_reader/config.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/ebooks/azw.py` & `epy_reader-2023.6.11/src/epy_reader/ebooks/azw.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/ebooks/base.py` & `epy_reader-2023.6.11/src/epy_reader/ebooks/base.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/ebooks/epub.py` & `epy_reader-2023.6.11/src/epy_reader/ebooks/epub.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/ebooks/fictionbook.py` & `epy_reader-2023.6.11/src/epy_reader/ebooks/fictionbook.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/ebooks/mobi.py` & `epy_reader-2023.6.11/src/epy_reader/ebooks/mobi.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/ebooks/url.py` & `epy_reader-2023.6.11/src/epy_reader/ebooks/url.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/lib.py` & `epy_reader-2023.6.11/src/epy_reader/lib.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/models.py` & `epy_reader-2023.6.11/src/epy_reader/models.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/parser.py` & `epy_reader-2023.6.11/src/epy_reader/parser.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/reader.py` & `epy_reader-2023.6.11/src/epy_reader/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import curses
 import dataclasses
 import multiprocessing
 import os
 import re
 import shutil
 import signal
@@ -142,15 +143,15 @@
     def run_counting_letters(self):
         if self._multiprocess_support:
             try:
                 self._proc_parent, self._proc_child = multiprocessing.Pipe()
                 self._process_counting_letter = multiprocessing.Process(
                     name="epy-subprocess-counting-letters",
                     target=count_letters_parallel,
-                    args=(self.ebook, self._proc_child),
+                    args=(copy.deepcopy(self.ebook), self._proc_child),
                 )
                 # forking will raise
                 # zlib.error: Error -3 while decompressing data: invalid distance too far back
                 self._process_counting_letter.start()
             except Exception as e:
                 if DEBUG:
                     raise e
```

### Comparing `epy-reader-2023.2.8/src/epy_reader/settings.py` & `epy_reader-2023.6.11/src/epy_reader/settings.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/speakers/base.py` & `epy_reader-2023.6.11/src/epy_reader/speakers/base.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/speakers/mimic.py` & `epy_reader-2023.6.11/src/epy_reader/speakers/mimic.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/speakers/pico.py` & `epy_reader-2023.6.11/src/epy_reader/speakers/pico.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/state.py` & `epy_reader-2023.6.11/src/epy_reader/state.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/compatibility_utils.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/compatibility_utils.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/kindleunpack.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/kindleunpack.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_cover.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_cover.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_dict.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_dict.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_header.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_header.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_html.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_html.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_index.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_index.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_k8proc.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_k8proc.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_k8resc.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_k8resc.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_nav.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_nav.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_ncx.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_ncx.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_opf.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_opf.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_pagemap.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_pagemap.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_sectioner.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_sectioner.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_split.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_split.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_uncompress.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_uncompress.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobi_utils.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobi_utils.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/mobiml2xhtml.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/mobiml2xhtml.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/unipath.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/unipath.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/tools/KindleUnpack/unpack_structure.py` & `epy_reader-2023.6.11/src/epy_reader/tools/KindleUnpack/unpack_structure.py`

 * *Files identical despite different names*

### Comparing `epy-reader-2023.2.8/src/epy_reader/utils.py` & `epy_reader-2023.6.11/src/epy_reader/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import wraps
 from typing import List, Mapping, Optional, Sequence, Tuple, Union
 
 from epy_reader.ebooks import URL, Azw, Ebook, Epub, FictionBook, Mobi
 from epy_reader.lib import is_url, tuple_subtract
 from epy_reader.models import Key, LettersCount, NoUpdate, ReadingState, TextStructure, TocEntry
 from epy_reader.parser import parse_html
-from epy_reader.speakers import SpeakerBaseModel, SpeakerMimic, SpeakerPico
+from epy_reader.speakers import SpeakerBaseModel, SpeakerMimic, SpeakerPico, SpeakerGttsMPV
 
 
 def get_ebook_obj(filepath: str) -> Ebook:
     file_ext = os.path.splitext(filepath)[1].lower()
     if is_url(filepath):
         return URL(filepath)
     elif file_ext in {".epub", ".epub3"}:
@@ -363,15 +363,15 @@
     child_conn.send(count_letters(ebook))
     child_conn.close()
 
 
 def construct_speaker(
     preferred: Optional[str] = None, args: List[str] = []
 ) -> Optional[SpeakerBaseModel]:
-    available_speakers = [SpeakerMimic, SpeakerPico]
+    available_speakers = [SpeakerMimic, SpeakerPico, SpeakerGttsMPV]
     sorted_speakers = (
         sorted(available_speakers, key=lambda x: int(x.cmd == preferred), reverse=True)
         if preferred
         else available_speakers
     )
     speaker = next((speaker for speaker in sorted_speakers if speaker.available), None)
     return speaker(args) if speaker else None
```

### Comparing `epy-reader-2023.2.8/src/epy_reader.egg-info/PKG-INFO` & `epy_reader-2023.6.11/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,186 +1,42 @@
-Metadata-Version: 2.1
-Name: epy-reader
-Version: 2023.2.8
-Summary: Terminal/CLI Ebook (epub, fb2, mobi, azw3) Reader
-Home-page: https://github.com/wustho/epy
-Author: Benawi Adha
-Author-email: benawiadha@gmail.com
-License: GPL-3.0
-Keywords: epub,epub3,fb2,mobi,azw3,CLI,Terminal,Reader
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-# `$ epy`
+package_dir = \
+{'': 'src'}
 
-[![Downloads](https://static.pepy.tech/personalized-badge/epy-reader?period=month&units=none&left_color=grey&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/epy-reader)
+packages = \
+['epy_reader',
+ 'epy_reader.ebooks',
+ 'epy_reader.speakers',
+ 'epy_reader.tools',
+ 'epy_reader.tools.KindleUnpack']
+
+package_data = \
+{'': ['*']}
+
+extras_require = \
+{':platform_system == "Windows"': ['windows-curses']}
+
+entry_points = \
+{'console_scripts': ['epy = epy_reader.__main__:main']}
+
+setup_kwargs = {
+    'name': 'epy-reader',
+    'version': '2023.6.11',
+    'description': 'TUI Ebook Reader',
+    'long_description': '# `$ epy`\n\n[![Downloads](https://static.pepy.tech/personalized-badge/epy-reader?period=month&units=none&left_color=grey&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/epy-reader)\n\n<a href=\'https://ko-fi.com/P5P4IDCX2\' target=\'_blank\'><img height=\'36\' style=\'border:0px;height:36px;\' src=\'https://storage.ko-fi.com/cdn/kofi2.png?v=3\' border=\'0\' alt=\'Buy Me a Coffee at ko-fi.com\' /></a>\n\n![screenshot](https://raw.githubusercontent.com/wustho/epy/master/screenshot.png)\n\nCLI Ebook Reader.\n\nThis is just a fork of [epr](https://github.com/wustho/epr) with these extra features:\n\n- Supported formats:\n  - Epub (.epub, .epub3)\n  - FictionBook (.fb2)\n  - Mobi (.mobi)\n  - AZW3 (.azw, .azw3)\n  - [URL](#url-support)\n- Reading progress percentage\n- Bookmarks\n- External dictionary integration (`sdcv`, `dict` or `wkdict`)\n- Inline formats: **bold** and _italic_ (depend on terminal and font capability. Italic only supported in python>=3.7)\n- Text-to-Speech (with additional setup, read [below](#text-to-speech))\n- [Double Spread](#double-spread)\n- Seamless (disabled by default, read [below](#reading-tips-using-epy))\n\n## Installation\n\n- Via PyPI (Linux and Mac OS)\n\n  ```shell\n  pip3 install epy-reader\n  ```\n\n- Via Pip+Git\n\n  ```shell\n  pip3 install git+https://github.com/wustho/epy\n  ```\n\n- Via AUR\n\n  ```shell\n  yay -S epy-ereader-git\n  ```\n\n- Windows Binary\n\n  Standalone binary for Windows is available at [release page](https://github.com/wustho/epy/releases).\n\n## Usage\n- `epy /path/to/your/book/book.epub` (Remember to make sure your book\'s title doesn\'t contain any spaces)\n- **c** Switching the color profile\n- **Shift + h** Previous chapter\n- **Shift + l** Next chapter\n- **Shift + g** Skip to the end of the chapter\n- **g** Skip to the beginning of the chapter\n- **Shift + m** Show metadata of the book\n- **t** Table of contents\n- **/** Search\n- **b** Add bookmark\n- **Shift + b** Show bookmarks\n- **q** Quit\n- **-** Shrink the text\n- **+** Enlarge the text\n- **o** Open an image\n- **s** Show or hide progress\n\n## Color profiles\nIn the config file you will see the following section.\n   ```\n    "DarkColorFG": 47,\n    "DarkColorBG": 235,\n    "LightColorFG": 238,\n    "LightColorBG": 253,\n   ```\n\nChange the values by using this image. (Make sure to ignore zeros at the beginning, it won\'t launch otherwise.)\n![image](https://user-images.githubusercontent.com/108401269/198876974-c8420de1-b256-42fd-9a09-3a69c5019608.png)\n\n## Reading Tips Using Epy\n\nWhen reading using `epy` you might occasionally find triple asteriks `***`.\nThat means you reach the end of some section in your ebook\nand the next line (right after those three asteriks, which is in new section)\nwill start at the top of the page.\nThis might be disorienting, so the best way to get seamless reading experience\nis by using next-page control (`space`, `l` or `Right`)\ninstead of next-line control (`j` or `Down`).\n\nIf you really want to get seamless reading experience, you can set `SeamlessBetweenChapters`\nto `true` in configuration file. But it has its drawback with more memory usage, that\'s why\nit\'s disabled by default.\n\n## Configuration File\n\nConfig file is available in json format which is located at:\n\n- Linux and Mac OS: `~/.config/epy/configuration.json` or `~/.epy/configuration.json`\n- Windows: `%USERPROFILE%\\.epy\\configuration.json`\n\n## URL Support\n\nYou can read online books like: short stories, fan fiction, etc. using `epy` with an url as cli argument.\nPretty useful when you want to read with less distraction.\n`epy` will also remember your reading progress online.\n\neg. You can read [Moby Dick from gutenberg](https://www.gutenberg.org/files/2701/2701-h/2701-h.htm)\ndirectly with:\n\n```shell\n$ epy https://www.gutenberg.org/files/2701/2701-h/2701-h.htm\n```\n\nBut note that `epy` will never be a web browser, it\'s simply a TUI program to read\nyour favorite fiction stories in the comfort of a terminal.\nSo please do not expect for web browser features to be implemented in `epy`.\n\n## Using Mouse\n\nAlthough mouse support is useful when running `epy` on Termux Android, it’s disabled by default\nsince most people find it intrusive when using `epy` in desktop.\nBut you can enable it by setting `MouseSupport` to `true` in config file.\n\n| Key | Action |\n| --- | --- |\n| `Left Click` (right side of screen) | next page |\n| `Left Click` (left side of screen) | prev page |\n| `Right Click` | ToC |\n| `Scroll Up` | scroll up |\n| `Scroll Down` | scroll down |\n| `Ctrl` + `Scroll Up` | increase text width |\n| `Ctrl` + `Scroll Down` | decrease text width |\n\n## Text-to-Speech\n\nTo get Text-to-Speech (TTS) support, external TTS engine is necessary.\n\nList of supported engines:\n\n- `mimic`\n- `pico2wave`\n- `gtts-mpv` (requires both [gTTS](https://pypi.org/project/gTTS) and [MPV](https://www.mpv.io))\n\n## Dictionary\n\nTo use "Define Word" you will have to install an external dictionary cli program (`sdcv`, `dict` or `wkdict`). After you\'ve done that, it is recommended to manually modify the configuration.json file, and set your desired dictionary there, so everything works properly.\n\nAfter that you will be able to find definition of word by pressing `d`, and aprompt will appear to let you type in word to define.\n\n## Double Spread\n\nDouble spread is intended to mimic the behaviour of real book,\nso line scrolling navigation will act as scrolling page and textwidth is not adjustable.\n\n## Changelog\n\n- `v2021.10.23`: Major refactoring which harness a lot of new stuff in `python>=3.7`\n  and `epy` won\'t be backward compatible with older python version and older configuration.\n\n- `v2022.1.8`: Change in configuration and reading states schema that is not backward compatible.\n  So if error is encountered, deleting the configuration and states file might fix the issue.\n\n- `v2022.1.15`: Early implementation of URL support, table of contents isn\'t available for now.\n\n- `v2022.1.23`: Library implementation: ability to switch ebook from reading history\n  inside epy (default key: `R`).\n\n- `v2022.2.5`: Fix process.join() issue for unstarted process.\n\n- `v2022.10.2`: Major breakdown `epy.py` module into package structure for easier development.\n',
+    'author': 'Benawi Adha',
+    'author_email': 'benawiadha@gmail.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/wustho/epy',
+    'package_dir': package_dir,
+    'packages': packages,
+    'package_data': package_data,
+    'extras_require': extras_require,
+    'entry_points': entry_points,
+    'python_requires': '>=3.8,<4.0',
+}
 
-<a href='https://ko-fi.com/P5P4IDCX2' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi2.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 
-![screenshot](https://raw.githubusercontent.com/wustho/epy/master/screenshot.png)
-
-CLI Ebook Reader.
-
-This is just a fork of [epr](https://github.com/wustho/epr) with these extra features:
-
-- Supported formats:
-  - Epub (.epub, .epub3)
-  - FictionBook (.fb2)
-  - Mobi (.mobi)
-  - AZW3 (.azw, .azw3)
-  - [URL](#url-support)
-- Reading progress percentage
-- Bookmarks
-- External dictionary integration (`sdcv`, `dict` or `wkdict`)
-- Inline formats: **bold** and _italic_ (depend on terminal and font capability. Italic only supported in python>=3.7)
-- Text-to-Speech (with additional setup, read [below](#text-to-speech))
-- [Double Spread](#double-spread)
-- Seamless (disabled by default, read [below](#reading-tips-using-epy))
-
-## Installation
-
-- Via PyPI (Linux and Mac OS)
-
-  ```shell
-  pip3 install epy-reader
-  ```
-
-- Via Pip+Git
-
-  ```shell
-  pip3 install git+https://github.com/wustho/epy
-  ```
-
-- Via AUR
-
-  ```shell
-  yay -S epy-git
-  ```
-
-- Windows Binary
-
-  Standalone binary for Windows is available at [release page](https://github.com/wustho/epy/releases).
-
-## Usage
-- `epy /path/to/your/book/book.epub` (Remember to make sure your book's title doesn't contain any spaces)
-- **c** Switching the color profile
-- **Shift + h** Previous chapter
-- **Shift + l** Next chapter
-- **Shift + g** Skip to the end of the chapter
-- **g** Skip to the beginning of the chapter
-- **Shift + m** Show metadata of the book
-- **t** Table of contents
-- **/** Search
-- **b** Add bookmark
-- **Shift + b** Show bookmarks
-- **q** Quit
-- **-** Shrink the text
-- **+** Enlarge the text
-- **o** Open an image
-- **s** Show or hide progress
-
-## Color profiles
-In the config file you will see the following section.
-   ```
-    "DarkColorFG": 47,
-    "DarkColorBG": 235,
-    "LightColorFG": 238,
-    "LightColorBG": 253,
-   ```
-
-Change the values by using this image. (Make sure to ignore zeros at the beginning, it won't launch otherwise.)
-![image](https://user-images.githubusercontent.com/108401269/198876974-c8420de1-b256-42fd-9a09-3a69c5019608.png)
-
-## Reading Tips Using Epy
-
-When reading using `epy` you might occasionally find triple asteriks `***`.
-That means you reach the end of some section in your ebook
-and the next line (right after those three asteriks, which is in new section)
-will start at the top of the page.
-This might be disorienting, so the best way to get seamless reading experience
-is by using next-page control (`space`, `l` or `Right`)
-instead of next-line control (`j` or `Down`).
-
-If you really want to get seamless reading experience, you can set `SeamlessBetweenChapters`
-to `true` in configuration file. But it has its drawback with more memory usage, that's why
-it's disabled by default.
-
-## Configuration File
-
-Config file is available in json format which is located at:
-
-- Linux and Mac OS: `~/.config/epy/configuration.json` or `~/.epy/configuration.json`
-- Windows: `%USERPROFILE%\.epy\configuration.json`
-
-## URL Support
-
-You can read online books like: short stories, fan fiction, etc. using `epy` with an url as cli argument.
-Pretty useful when you want to read with less distraction.
-`epy` will also remember your reading progress online.
-
-eg. You can read [Moby Dick from gutenberg](https://www.gutenberg.org/files/2701/2701-h/2701-h.htm)
-directly with:
-
-```shell
-$ epy https://www.gutenberg.org/files/2701/2701-h/2701-h.htm
-```
-
-But note that `epy` will never be a web browser, it's simply a TUI program to read
-your favorite fiction stories in the comfort of a terminal.
-So please do not expect for web browser features to be implemented in `epy`.
-
-## Using Mouse
-
-Although mouse support is useful when running `epy` on Termux Android, it’s disabled by default
-since most people find it intrusive when using `epy` in desktop.
-But you can enable it by setting `MouseSupport` to `true` in config file.
-
-| Key | Action |
-| --- | --- |
-| `Left Click` (right side of screen) | next page |
-| `Left Click` (left side of screen) | prev page |
-| `Right Click` | ToC |
-| `Scroll Up` | scroll up |
-| `Scroll Down` | scroll down |
-| `Ctrl` + `Scroll Up` | increase text width |
-| `Ctrl` + `Scroll Down` | decrease text width |
-
-## Text-to-Speech
-
-To get Text-to-Speech (TTS) support, external TTS engine is necessary.
-
-List of supported engines:
-
-- `mimic`
-- `pico2wave`
-
-## Dictionary
-
-To use "Define Word" you will have to install an external dictionary cli program (`sdcv`, `dict` or `wkdict`). After you've done that, it is recommended to manually modify the configuration.json file, and set your desired dictionary there, so everything works properly.
-
-After that you will be able to find definition of word by pressing `d`, and aprompt will appear to let you type in word to define.
-
-## Double Spread
-
-Double spread is intended to mimic the behaviour of real book,
-so line scrolling navigation will act as scrolling page and textwidth is not adjustable.
-
-## Changelog
-
-- `v2021.10.23`: Major refactoring which harness a lot of new stuff in `python>=3.7`
-  and `epy` won't be backward compatible with older python version and older configuration.
-
-- `v2022.1.8`: Change in configuration and reading states schema that is not backward compatible.
-  So if error is encountered, deleting the configuration and states file might fix the issue.
-
-- `v2022.1.15`: Early implementation of URL support, table of contents isn't available for now.
-
-- `v2022.1.23`: Library implementation: ability to switch ebook from reading history
-  inside epy (default key: `R`).
-
-- `v2022.2.5`: Fix process.join() issue for unstarted process.
-
-- `v2022.10.2`: Major breakdown `epy.py` module into package structure for easier development.
+setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,84 +1,94 @@
-Metadata-Version: 2.1 Name: epy-reader Version: 2023.2.8 Summary: Terminal/CLI
-Ebook (epub, fb2, mobi, azw3) Reader Home-page: https://github.com/wustho/epy
-Author: Benawi Adha Author-email: benawiadha@gmail.com License: GPL-3.0
-Keywords: epub,epub3,fb2,mobi,azw3,CLI,Terminal,Reader Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # `$ epy` [![Downloads](https://static.pepy.tech/personalized-badge/
-epy-
+# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
+'src'} packages = \ ['epy_reader', 'epy_reader.ebooks', 'epy_reader.speakers',
+'epy_reader.tools', 'epy_reader.tools.KindleUnpack'] package_data = \ {'':
+['*']} extras_require = \ {':platform_system == "Windows"': ['windows-curses']}
+entry_points = \ {'console_scripts': ['epy = epy_reader.__main__:main']}
+setup_kwargs = { 'name': 'epy-reader', 'version': '2023.6.11', 'description':
+'TUI Ebook Reader', 'long_description': '# `$ epy`\n\n[![Downloads](https://
+static.pepy.tech/personalized-badge/epy-
 reader?period=month&units=none&left_color=grey&right_color=brightgreen&left_text=downloads/
-month)](https://pepy.tech/project/epy-reader) [Buy_Me_a_Coffee_at_ko-fi.com] !
-[screenshot](https://raw.githubusercontent.com/wustho/epy/master/
-screenshot.png) CLI Ebook Reader. This is just a fork of [epr](https://
-github.com/wustho/epr) with these extra features: - Supported formats: - Epub
-(.epub, .epub3) - FictionBook (.fb2) - Mobi (.mobi) - AZW3 (.azw, .azw3) -
-[URL](#url-support) - Reading progress percentage - Bookmarks - External
-dictionary integration (`sdcv`, `dict` or `wkdict`) - Inline formats: **bold**
-and _italic_ (depend on terminal and font capability. Italic only supported in
-python>=3.7) - Text-to-Speech (with additional setup, read [below](#text-to-
-speech)) - [Double Spread](#double-spread) - Seamless (disabled by default,
-read [below](#reading-tips-using-epy)) ## Installation - Via PyPI (Linux and
-Mac OS) ```shell pip3 install epy-reader ``` - Via Pip+Git ```shell pip3
-install git+https://github.com/wustho/epy ``` - Via AUR ```shell yay -S epy-git
-``` - Windows Binary Standalone binary for Windows is available at [release
-page](https://github.com/wustho/epy/releases). ## Usage - `epy /path/to/your/
-book/book.epub` (Remember to make sure your book's title doesn't contain any
-spaces) - **c** Switching the color profile - **Shift + h** Previous chapter -
-**Shift + l** Next chapter - **Shift + g** Skip to the end of the chapter -
-**g** Skip to the beginning of the chapter - **Shift + m** Show metadata of the
-book - **t** Table of contents - **/** Search - **b** Add bookmark - **Shift +
-b** Show bookmarks - **q** Quit - **-** Shrink the text - **+** Enlarge the
-text - **o** Open an image - **s** Show or hide progress ## Color profiles In
-the config file you will see the following section. ``` "DarkColorFG": 47,
-"DarkColorBG": 235, "LightColorFG": 238, "LightColorBG": 253, ``` Change the
-values by using this image. (Make sure to ignore zeros at the beginning, it
-won't launch otherwise.) ![image](https://user-images.githubusercontent.com/
-108401269/198876974-c8420de1-b256-42fd-9a09-3a69c5019608.png) ## Reading Tips
-Using Epy When reading using `epy` you might occasionally find triple asteriks
-`***`. That means you reach the end of some section in your ebook and the next
-line (right after those three asteriks, which is in new section) will start at
-the top of the page. This might be disorienting, so the best way to get
-seamless reading experience is by using next-page control (`space`, `l` or
-`Right`) instead of next-line control (`j` or `Down`). If you really want to
-get seamless reading experience, you can set `SeamlessBetweenChapters` to
-`true` in configuration file. But it has its drawback with more memory usage,
-that's why it's disabled by default. ## Configuration File Config file is
-available in json format which is located at: - Linux and Mac OS: `~/.config/
-epy/configuration.json` or `~/.epy/configuration.json` - Windows:
-`%USERPROFILE%\.epy\configuration.json` ## URL Support You can read online
-books like: short stories, fan fiction, etc. using `epy` with an url as cli
-argument. Pretty useful when you want to read with less distraction. `epy` will
-also remember your reading progress online. eg. You can read [Moby Dick from
-gutenberg](https://www.gutenberg.org/files/2701/2701-h/2701-h.htm) directly
-with: ```shell $ epy https://www.gutenberg.org/files/2701/2701-h/2701-h.htm ```
-But note that `epy` will never be a web browser, it's simply a TUI program to
-read your favorite fiction stories in the comfort of a terminal. So please do
-not expect for web browser features to be implemented in `epy`. ## Using Mouse
-Although mouse support is useful when running `epy` on Termux Android, itâs
-disabled by default since most people find it intrusive when using `epy` in
-desktop. But you can enable it by setting `MouseSupport` to `true` in config
-file. | Key | Action | | --- | --- | | `Left Click` (right side of screen) |
-next page | | `Left Click` (left side of screen) | prev page | | `Right Click`
-| ToC | | `Scroll Up` | scroll up | | `Scroll Down` | scroll down | | `Ctrl` +
-`Scroll Up` | increase text width | | `Ctrl` + `Scroll Down` | decrease text
-width | ## Text-to-Speech To get Text-to-Speech (TTS) support, external TTS
-engine is necessary. List of supported engines: - `mimic` - `pico2wave` ##
-Dictionary To use "Define Word" you will have to install an external dictionary
-cli program (`sdcv`, `dict` or `wkdict`). After you've done that, it is
-recommended to manually modify the configuration.json file, and set your
-desired dictionary there, so everything works properly. After that you will be
-able to find definition of word by pressing `d`, and aprompt will appear to let
-you type in word to define. ## Double Spread Double spread is intended to mimic
-the behaviour of real book, so line scrolling navigation will act as scrolling
-page and textwidth is not adjustable. ## Changelog - `v2021.10.23`: Major
-refactoring which harness a lot of new stuff in `python>=3.7` and `epy` won't
-be backward compatible with older python version and older configuration. -
-`v2022.1.8`: Change in configuration and reading states schema that is not
-backward compatible. So if error is encountered, deleting the configuration and
-states file might fix the issue. - `v2022.1.15`: Early implementation of URL
-support, table of contents isn't available for now. - `v2022.1.23`: Library
-implementation: ability to switch ebook from reading history inside epy
-(default key: `R`). - `v2022.2.5`: Fix process.join() issue for unstarted
-process. - `v2022.10.2`: Major breakdown `epy.py` module into package structure
-for easier development.
+month)](https://pepy.tech/project/epy-reader)\n\n
+com\' />
+\n\n![screenshot](https://raw.githubusercontent.com/wustho/epy/master/
+screenshot.png)\n\nCLI Ebook Reader.\n\nThis is just a fork of [epr](https://
+github.com/wustho/epr) with these extra features:\n\n- Supported formats:\n -
+Epub (.epub, .epub3)\n - FictionBook (.fb2)\n - Mobi (.mobi)\n - AZW3 (.azw,
+.azw3)\n - [URL](#url-support)\n- Reading progress percentage\n- Bookmarks\n-
+External dictionary integration (`sdcv`, `dict` or `wkdict`)\n- Inline formats:
+**bold** and _italic_ (depend on terminal and font capability. Italic only
+supported in python>=3.7)\n- Text-to-Speech (with additional setup, read
+[below](#text-to-speech))\n- [Double Spread](#double-spread)\n- Seamless
+(disabled by default, read [below](#reading-tips-using-epy))\n\n##
+Installation\n\n- Via PyPI (Linux and Mac OS)\n\n ```shell\n pip3 install epy-
+reader\n ```\n\n- Via Pip+Git\n\n ```shell\n pip3 install git+https://
+github.com/wustho/epy\n ```\n\n- Via AUR\n\n ```shell\n yay -S epy-ereader-
+git\n ```\n\n- Windows Binary\n\n Standalone binary for Windows is available at
+[release page](https://github.com/wustho/epy/releases).\n\n## Usage\n- `epy /
+path/to/your/book/book.epub` (Remember to make sure your book\'s title doesn\'t
+contain any spaces)\n- **c** Switching the color profile\n- **Shift + h**
+Previous chapter\n- **Shift + l** Next chapter\n- **Shift + g** Skip to the end
+of the chapter\n- **g** Skip to the beginning of the chapter\n- **Shift + m**
+Show metadata of the book\n- **t** Table of contents\n- **/** Search\n- **b**
+Add bookmark\n- **Shift + b** Show bookmarks\n- **q** Quit\n- **-** Shrink the
+text\n- **+** Enlarge the text\n- **o** Open an image\n- **s** Show or hide
+progress\n\n## Color profiles\nIn the config file you will see the following
+section.\n ```\n "DarkColorFG": 47,\n "DarkColorBG": 235,\n "LightColorFG":
+238,\n "LightColorBG": 253,\n ```\n\nChange the values by using this image.
+(Make sure to ignore zeros at the beginning, it won\'t launch otherwise.)\n!
+[image](https://user-images.githubusercontent.com/108401269/198876974-c8420de1-
+b256-42fd-9a09-3a69c5019608.png)\n\n## Reading Tips Using Epy\n\nWhen reading
+using `epy` you might occasionally find triple asteriks `***`.\nThat means you
+reach the end of some section in your ebook\nand the next line (right after
+those three asteriks, which is in new section)\nwill start at the top of the
+page.\nThis might be disorienting, so the best way to get seamless reading
+experience\nis by using next-page control (`space`, `l` or `Right`)\ninstead of
+next-line control (`j` or `Down`).\n\nIf you really want to get seamless
+reading experience, you can set `SeamlessBetweenChapters`\nto `true` in
+configuration file. But it has its drawback with more memory usage, that\'s
+why\nit\'s disabled by default.\n\n## Configuration File\n\nConfig file is
+available in json format which is located at:\n\n- Linux and Mac OS:
+`~/.config/epy/configuration.json` or `~/.epy/configuration.json`\n- Windows:
+`%USERPROFILE%\\.epy\\configuration.json`\n\n## URL Support\n\nYou can read
+online books like: short stories, fan fiction, etc. using `epy` with an url as
+cli argument.\nPretty useful when you want to read with less
+distraction.\n`epy` will also remember your reading progress online.\n\neg. You
+can read [Moby Dick from gutenberg](https://www.gutenberg.org/files/2701/2701-
+h/2701-h.htm)\ndirectly with:\n\n```shell\n$ epy https://www.gutenberg.org/
+files/2701/2701-h/2701-h.htm\n```\n\nBut note that `epy` will never be a web
+browser, it\'s simply a TUI program to read\nyour favorite fiction stories in
+the comfort of a terminal.\nSo please do not expect for web browser features to
+be implemented in `epy`.\n\n## Using Mouse\n\nAlthough mouse support is useful
+when running `epy` on Termux Android, itâs disabled by default\nsince most
+people find it intrusive when using `epy` in desktop.\nBut you can enable it by
+setting `MouseSupport` to `true` in config file.\n\n| Key | Action |\n| --- | -
+-- |\n| `Left Click` (right side of screen) | next page |\n| `Left Click` (left
+side of screen) | prev page |\n| `Right Click` | ToC |\n| `Scroll Up` | scroll
+up |\n| `Scroll Down` | scroll down |\n| `Ctrl` + `Scroll Up` | increase text
+width |\n| `Ctrl` + `Scroll Down` | decrease text width |\n\n## Text-to-
+Speech\n\nTo get Text-to-Speech (TTS) support, external TTS engine is
+necessary.\n\nList of supported engines:\n\n- `mimic`\n- `pico2wave`\n- `gtts-
+mpv` (requires both [gTTS](https://pypi.org/project/gTTS) and [MPV](https://
+www.mpv.io))\n\n## Dictionary\n\nTo use "Define Word" you will have to install
+an external dictionary cli program (`sdcv`, `dict` or `wkdict`). After you\'ve
+done that, it is recommended to manually modify the configuration.json file,
+and set your desired dictionary there, so everything works properly.\n\nAfter
+that you will be able to find definition of word by pressing `d`, and aprompt
+will appear to let you type in word to define.\n\n## Double Spread\n\nDouble
+spread is intended to mimic the behaviour of real book,\nso line scrolling
+navigation will act as scrolling page and textwidth is not adjustable.\n\n##
+Changelog\n\n- `v2021.10.23`: Major refactoring which harness a lot of new
+stuff in `python>=3.7`\n and `epy` won\'t be backward compatible with older
+python version and older configuration.\n\n- `v2022.1.8`: Change in
+configuration and reading states schema that is not backward compatible.\n So
+if error is encountered, deleting the configuration and states file might fix
+the issue.\n\n- `v2022.1.15`: Early implementation of URL support, table of
+contents isn\'t available for now.\n\n- `v2022.1.23`: Library implementation:
+ability to switch ebook from reading history\n inside epy (default key:
+`R`).\n\n- `v2022.2.5`: Fix process.join() issue for unstarted process.\n\n-
+`v2022.10.2`: Major breakdown `epy.py` module into package structure for easier
+development.\n', 'author': 'Benawi Adha', 'author_email':
+'benawiadha@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
+'url': 'https://github.com/wustho/epy', 'package_dir': package_dir, 'packages':
+packages, 'package_data': package_data, 'extras_require': extras_require,
+'entry_points': entry_points, 'python_requires': '>=3.8,<4.0', } setup
+(**setup_kwargs)
```

