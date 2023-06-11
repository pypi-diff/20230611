# Comparing `tmp/plex-tvdb-alt-orderer-0.2.1.tar.gz` & `tmp/plex-tvdb-alt-orderer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-tvdb-alt-orderer-0.2.1.tar", last modified: Fri Jun  9 21:40:09 2023, max compression
+gzip compressed data, was "plex-tvdb-alt-orderer-0.2.2.tar", last modified: Sun Jun 11 05:57:00 2023, max compression
```

## Comparing `plex-tvdb-alt-orderer-0.2.1.tar` & `plex-tvdb-alt-orderer-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 21:40:09.068298 plex-tvdb-alt-orderer-0.2.1/
--rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     5870 2023-06-09 21:40:09.065297 plex-tvdb-alt-orderer-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5250 2023-06-09 21:39:05.000000 plex-tvdb-alt-orderer-0.2.1/README.md
--rw-rw-rw-   0        0        0      877 2023-06-09 21:39:43.000000 plex-tvdb-alt-orderer-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 21:40:09.068298 plex-tvdb-alt-orderer-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 21:40:08.975751 plex-tvdb-alt-orderer-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 21:40:09.001753 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer/
--rw-rw-rw-   0        0        0     8107 2023-06-09 21:17:11.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:40:09.063297 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/
--rw-rw-rw-   0        0        0     5870 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-09 21:40:08.000000 plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 05:57:00.155590 plex-tvdb-alt-orderer-0.2.2/
+-rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     5870 2023-06-11 05:57:00.155590 plex-tvdb-alt-orderer-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5250 2023-06-09 21:39:05.000000 plex-tvdb-alt-orderer-0.2.2/README.md
+-rw-rw-rw-   0        0        0      877 2023-06-11 05:56:23.000000 plex-tvdb-alt-orderer-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 05:57:00.155590 plex-tvdb-alt-orderer-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 05:57:00.124971 plex-tvdb-alt-orderer-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 05:57:00.128968 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer/
+-rw-rw-rw-   0        0        0     8143 2023-06-11 05:50:24.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer/main.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:57:00.154590 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/
+-rw-rw-rw-   0        0        0     5870 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
```

### Comparing `plex-tvdb-alt-orderer-0.2.1/LICENSE` & `plex-tvdb-alt-orderer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.2.1/PKG-INFO` & `plex-tvdb-alt-orderer-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-tvdb-alt-orderer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A utility that applies alternate TVDB orders to Plex.
 Author: bpoxy
 Project-URL: Homepage, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Project-URL: Bug Tracker, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plex-tvdb-alt-orderer-0.2.1/README.md` & `plex-tvdb-alt-orderer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.2.1/pyproject.toml` & `plex-tvdb-alt-orderer-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plex-tvdb-alt-orderer"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="bpoxy" },
 ]
 description = "A utility that applies alternate TVDB orders to Plex."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["click", "inquirer", "plexapi", "progress", "termcolor", "tvdb_v4_official", "validators"]
```

### Comparing `plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer/main.py` & `plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import click
 import inquirer
 import re
 import validators
 from plexapi.myplex import MyPlexAccount, PlexServer
 from plexapi.library import ShowSection
 from plexapi.video import Episode, Show
```

### Comparing `plex-tvdb-alt-orderer-0.2.1/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO` & `plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-tvdb-alt-orderer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A utility that applies alternate TVDB orders to Plex.
 Author: bpoxy
 Project-URL: Homepage, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Project-URL: Bug Tracker, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

