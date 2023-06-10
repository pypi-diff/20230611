# Comparing `tmp/datasette_sqlite_path-0.2.0a3-py3-none-any.whl.zip` & `tmp/datasette_sqlite_path-0.2.0a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2173 bytes, number of entries: 7
--rw-r--r--  2.0 unx      266 b- defN 23-Jun-07 16:57 datasette_sqlite_path/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 16:57 datasette_sqlite_path/version.py
--rw-r--r--  2.0 unx      563 b- defN 23-Jun-07 16:57 datasette_sqlite_path-0.2.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 16:57 datasette_sqlite_path-0.2.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jun-07 16:57 datasette_sqlite_path-0.2.0a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-07 16:57 datasette_sqlite_path-0.2.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      648 b- defN 23-Jun-07 16:57 datasette_sqlite_path-0.2.0a3.dist-info/RECORD
-7 files, 1718 bytes uncompressed, 993 bytes compressed:  42.2%
+Zip file size: 2172 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      266 b- defN 23-Jun-10 22:08 datasette_sqlite_path/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 22:08 datasette_sqlite_path/version.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Jun-10 22:08 datasette_sqlite_path-0.2.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 22:08 datasette_sqlite_path-0.2.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-10 22:08 datasette_sqlite_path-0.2.0a4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-10 22:08 datasette_sqlite_path-0.2.0a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      648 b- defN 23-Jun-10 22:08 datasette_sqlite_path-0.2.0a4.dist-info/RECORD
+7 files, 1718 bytes uncompressed, 992 bytes compressed:  42.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_path/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_path/version.py
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.0a3.dist-info/METADATA
+Filename: datasette_sqlite_path-0.2.0a4.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.0a3.dist-info/WHEEL
+Filename: datasette_sqlite_path-0.2.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.0a3.dist-info/entry_points.txt
+Filename: datasette_sqlite_path-0.2.0a4.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.0a3.dist-info/top_level.txt
+Filename: datasette_sqlite_path-0.2.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_path-0.2.0a3.dist-info/RECORD
+Filename: datasette_sqlite_path-0.2.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_path/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.0-alpha.3"
+__version__ = "0.2.0-alpha.4"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_path-0.2.0a3.dist-info/METADATA` & `datasette_sqlite_path-0.2.0a4.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-path
-Version: 0.2.0a3
+Version: 0.2.0a4
 Home-page: https://github.com/asg017/sqlite-path
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-path/issues
 Project-URL: CI, https://github.com/asg017/sqlite-path/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-path/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_path-0.2.0a3.dist-info/RECORD` & `datasette_sqlite_path-0.2.0a4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_path/__init__.py,sha256=osdMTJPil1Ppcc-mJ4UMQp-oGKfMOPDyVWLGqPkkq78,266
-datasette_sqlite_path/version.py,sha256=DgA5ALFly94tMZVGijsqOogudNMmcgnIDpb3TTSinLY,79
-datasette_sqlite_path-0.2.0a3.dist-info/METADATA,sha256=IxHNtQdJkE-AYKOYpzEtufFV_t4ori_yo_NKoHgmw48,563
-datasette_sqlite_path-0.2.0a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_path-0.2.0a3.dist-info/entry_points.txt,sha256=t24lnlHZ_xRyjyQ6gDYJMK-UBRIjk54QxR3Yi79TWv4,48
-datasette_sqlite_path-0.2.0a3.dist-info/top_level.txt,sha256=EMfolA5zamEfjTvzMVKdVVZIsecWmN4shdy6e5m5QI8,22
-datasette_sqlite_path-0.2.0a3.dist-info/RECORD,,
+datasette_sqlite_path/version.py,sha256=3PpM5Qbs4lrFty8fDoUC1mvc6gHNQPIgm7BLqB6JpCk,79
+datasette_sqlite_path-0.2.0a4.dist-info/METADATA,sha256=PwgcpL07frcnW9uH9ceIDIQVmZRTeqiAtkoe8hwt9oI,563
+datasette_sqlite_path-0.2.0a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_path-0.2.0a4.dist-info/entry_points.txt,sha256=t24lnlHZ_xRyjyQ6gDYJMK-UBRIjk54QxR3Yi79TWv4,48
+datasette_sqlite_path-0.2.0a4.dist-info/top_level.txt,sha256=EMfolA5zamEfjTvzMVKdVVZIsecWmN4shdy6e5m5QI8,22
+datasette_sqlite_path-0.2.0a4.dist-info/RECORD,,
```

