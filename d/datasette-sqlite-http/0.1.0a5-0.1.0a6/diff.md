# Comparing `tmp/datasette_sqlite_http-0.1.0a5-py3-none-any.whl.zip` & `tmp/datasette_sqlite_http-0.1.0a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2275 bytes, number of entries: 7
--rw-r--r--  2.0 unx      511 b- defN 23-Jun-06 23:38 datasette_sqlite_http/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-06 23:38 datasette_sqlite_http/version.py
--rw-r--r--  2.0 unx      563 b- defN 23-Jun-06 23:38 datasette_sqlite_http-0.1.0a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 23:38 datasette_sqlite_http-0.1.0a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jun-06 23:38 datasette_sqlite_http-0.1.0a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-06 23:38 datasette_sqlite_http-0.1.0a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      648 b- defN 23-Jun-06 23:38 datasette_sqlite_http-0.1.0a5.dist-info/RECORD
-7 files, 1963 bytes uncompressed, 1095 bytes compressed:  44.2%
+Zip file size: 2279 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      511 b- defN 23-Jun-10 22:09 datasette_sqlite_http/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 22:09 datasette_sqlite_http/version.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Jun-10 22:09 datasette_sqlite_http-0.1.0a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 22:09 datasette_sqlite_http-0.1.0a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-10 22:09 datasette_sqlite_http-0.1.0a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-10 22:09 datasette_sqlite_http-0.1.0a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      648 b- defN 23-Jun-10 22:09 datasette_sqlite_http-0.1.0a6.dist-info/RECORD
+7 files, 1963 bytes uncompressed, 1099 bytes compressed:  44.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_http/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_http/version.py
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a5.dist-info/METADATA
+Filename: datasette_sqlite_http-0.1.0a6.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a5.dist-info/WHEEL
+Filename: datasette_sqlite_http-0.1.0a6.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a5.dist-info/entry_points.txt
+Filename: datasette_sqlite_http-0.1.0a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a5.dist-info/top_level.txt
+Filename: datasette_sqlite_http-0.1.0a6.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_http-0.1.0a5.dist-info/RECORD
+Filename: datasette_sqlite_http-0.1.0a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_http/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.5"
+__version__ = "0.1.0-alpha.6"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_http-0.1.0a5.dist-info/METADATA` & `datasette_sqlite_http-0.1.0a6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-http
-Version: 0.1.0a5
+Version: 0.1.0a6
 Home-page: https://github.com/asg017/sqlite-http
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-http/issues
 Project-URL: CI, https://github.com/asg017/sqlite-http/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-http/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_http-0.1.0a5.dist-info/RECORD` & `datasette_sqlite_http-0.1.0a6.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_http/__init__.py,sha256=yyH-gLZb2W8MAo-KJ7Byl2ytA7PRSt4UFt5TRakD8Q8,511
-datasette_sqlite_http/version.py,sha256=FXO_R3AA__fvnfQ57SsvqaxFY_R7FrJr0heHPCFLg-s,79
-datasette_sqlite_http-0.1.0a5.dist-info/METADATA,sha256=4vrNylimyl_cMvomBlbF9UTmrDpPGGVLdDAMjZdt1C4,563
-datasette_sqlite_http-0.1.0a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_http-0.1.0a5.dist-info/entry_points.txt,sha256=eagqsxGPRP0kF8dCA4FybMi8h0xi1d9RPPDS28XGBNE,48
-datasette_sqlite_http-0.1.0a5.dist-info/top_level.txt,sha256=yD9WNDeOsdBxiIO5HKw_3PfSbHPmnDqR_LJn2EamJGU,22
-datasette_sqlite_http-0.1.0a5.dist-info/RECORD,,
+datasette_sqlite_http/version.py,sha256=HkXLQT0myTcEkHxJfwQLuIZOxYWf-mSukbpKcYbctp8,79
+datasette_sqlite_http-0.1.0a6.dist-info/METADATA,sha256=op7--czDyebW7USThkHATyLxvu9twqv7mMlEnD-y4nc,563
+datasette_sqlite_http-0.1.0a6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_http-0.1.0a6.dist-info/entry_points.txt,sha256=eagqsxGPRP0kF8dCA4FybMi8h0xi1d9RPPDS28XGBNE,48
+datasette_sqlite_http-0.1.0a6.dist-info/top_level.txt,sha256=yD9WNDeOsdBxiIO5HKw_3PfSbHPmnDqR_LJn2EamJGU,22
+datasette_sqlite_http-0.1.0a6.dist-info/RECORD,,
```

