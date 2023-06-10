# Comparing `tmp/datasette_sqlite_url-0.1.0a5-py3-none-any.whl.zip` & `tmp/datasette_sqlite_url-0.1.0a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2150 bytes, number of entries: 7
--rw-r--r--  2.0 unx      263 b- defN 23-Jun-07 17:02 datasette_sqlite_url/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 17:02 datasette_sqlite_url/version.py
--rw-r--r--  2.0 unx      557 b- defN 23-Jun-07 17:05 datasette_sqlite_url-0.1.0a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 17:05 datasette_sqlite_url-0.1.0a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-07 17:05 datasette_sqlite_url-0.1.0a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-07 17:05 datasette_sqlite_url-0.1.0a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 23-Jun-07 17:05 datasette_sqlite_url-0.1.0a5.dist-info/RECORD
-7 files, 1699 bytes uncompressed, 984 bytes compressed:  42.1%
+Zip file size: 2154 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-10 22:08 datasette_sqlite_url/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 22:08 datasette_sqlite_url/version.py
+-rw-r--r--  2.0 unx      557 b- defN 23-Jun-10 22:09 datasette_sqlite_url-0.1.0a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 22:09 datasette_sqlite_url-0.1.0a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-10 22:09 datasette_sqlite_url-0.1.0a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-10 22:09 datasette_sqlite_url-0.1.0a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      641 b- defN 23-Jun-10 22:09 datasette_sqlite_url-0.1.0a6.dist-info/RECORD
+7 files, 1699 bytes uncompressed, 988 bytes compressed:  41.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_url/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_url/version.py
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a5.dist-info/METADATA
+Filename: datasette_sqlite_url-0.1.0a6.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a5.dist-info/WHEEL
+Filename: datasette_sqlite_url-0.1.0a6.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a5.dist-info/entry_points.txt
+Filename: datasette_sqlite_url-0.1.0a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a5.dist-info/top_level.txt
+Filename: datasette_sqlite_url-0.1.0a6.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_url-0.1.0a5.dist-info/RECORD
+Filename: datasette_sqlite_url-0.1.0a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_url/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.5"
+__version__ = "0.1.0-alpha.6"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_url-0.1.0a5.dist-info/METADATA` & `datasette_sqlite_url-0.1.0a6.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-url
-Version: 0.1.0a5
+Version: 0.1.0a6
 Home-page: https://github.com/asg017/sqlite-url
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-url/issues
 Project-URL: CI, https://github.com/asg017/sqlite-url/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-url/releases
 Requires-Python: >=3.7
```

