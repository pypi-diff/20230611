# Comparing `tmp/wrangles-1.2.1.tar.gz` & `tmp/wrangles-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrangles-1.2.1.tar", last modified: Fri Apr 14 19:34:10 2023, max compression
+gzip compressed data, was "wrangles-1.3.0.tar", last modified: Sun Jun 11 17:40:25 2023, max compression
```

## Comparing `wrangles-1.2.1.tar` & `wrangles-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.074519 wrangles-1.2.1/
--rw-rw-rw-   0        0        0     3615 2023-04-14 19:34:10.074519 wrangles-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3102 2023-03-30 14:19:22.000000 wrangles-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.051580 wrangles-1.2.1/Wrangles.egg-info/
--rw-rw-rw-   0        0        0     3615 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1538 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-14 19:34:10.075520 wrangles-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1205 2023-04-14 19:13:56.000000 wrangles-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.049586 wrangles-1.2.1/wrangles/
--rw-rw-rw-   0        0        0      565 2022-06-23 19:42:00.000000 wrangles-1.2.1/wrangles/__init__.py
--rw-rw-rw-   0        0        0     1681 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/auth.py
--rw-rw-rw-   0        0        0      840 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/batching.py
--rw-rw-rw-   0        0        0     2069 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/classify.py
--rw-rw-rw-   0        0        0      559 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/config.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.066540 wrangles-1.2.1/wrangles/connectors/
--rw-rw-rw-   0        0        0      449 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/connectors/__init__.py
--rw-rw-rw-   0        0        0     7100 2023-04-11 22:29:27.000000 wrangles-1.2.1/wrangles/connectors/akeneo.py
--rw-rw-rw-   0        0        0    11023 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/ckan.py
--rw-rw-rw-   0        0        0     7811 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/file.py
--rw-rw-rw-   0        0        0     2498 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/http.py
--rw-rw-rw-   0        0        0     1883 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/jinja.py
--rw-rw-rw-   0        0        0     4537 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/mongodb.py
--rw-rw-rw-   0        0        0     6136 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/mssql.py
--rw-rw-rw-   0        0        0     4372 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/mysql.py
--rw-rw-rw-   0        0        0     6328 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/notification.py
--rw-rw-rw-   0        0        0     5892 2022-06-23 19:42:00.000000 wrangles-1.2.1/wrangles/connectors/postgres.py
--rw-rw-rw-   0        0        0    16169 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/pricefx.py
--rw-rw-rw-   0        0        0     4534 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/recipe.py
--rw-rw-rw-   0        0        0     8530 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/s3.py
--rw-rw-rw-   0        0        0     4756 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/salesforce.py
--rw-rw-rw-   0        0        0     4442 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/sftp.py
--rw-rw-rw-   0        0        0     2430 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/ssh.py
--rw-rw-rw-   0        0        0     5651 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/test.py
--rw-rw-rw-   0        0        0     8040 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/train.py
--rw-rw-rw-   0        0        0     1899 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/console.py
--rw-rw-rw-   0        0        0     1592 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/data.py
--rw-rw-rw-   0        0        0    10183 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/extract.py
--rw-rw-rw-   0        0        0     4412 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/format.py
--rw-rw-rw-   0        0        0    19918 2023-04-14 15:48:30.000000 wrangles-1.2.1/wrangles/recipe.py
-drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.073521 wrangles-1.2.1/wrangles/recipe_wrangles/
--rw-rw-rw-   0        0        0      562 2022-06-23 19:42:00.000000 wrangles-1.2.1/wrangles/recipe_wrangles/__init__.py
--rw-rw-rw-   0        0        0     6878 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/recipe_wrangles/convert.py
--rw-rw-rw-   0        0        0     8582 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/recipe_wrangles/create.py
--rw-rw-rw-   0        0        0    20328 2023-04-14 19:14:11.000000 wrangles-1.2.1/wrangles/recipe_wrangles/extract.py
--rw-rw-rw-   0        0        0     8055 2023-04-10 17:05:21.000000 wrangles-1.2.1/wrangles/recipe_wrangles/format.py
--rw-rw-rw-   0        0        0    26422 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/recipe_wrangles/main.py
--rw-rw-rw-   0        0        0     8570 2023-04-10 17:05:21.000000 wrangles-1.2.1/wrangles/recipe_wrangles/merge.py
--rw-rw-rw-   0        0        0     7681 2023-04-10 17:05:21.000000 wrangles-1.2.1/wrangles/recipe_wrangles/select.py
--rw-rw-rw-   0        0        0     6435 2023-04-10 17:05:21.000000 wrangles-1.2.1/wrangles/recipe_wrangles/split.py
--rw-rw-rw-   0        0        0     1875 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/select.py
--rw-rw-rw-   0        0        0     2099 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/standardize.py
--rw-rw-rw-   0        0        0     6100 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/train.py
--rw-rw-rw-   0        0        0     3502 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/translate.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.675200 wrangles-1.3.0/
+-rw-rw-rw-   0        0        0    11558 2022-12-19 21:12:29.000000 wrangles-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4464 2023-06-11 17:40:25.675200 wrangles-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2023-03-31 00:02:07.000000 wrangles-1.3.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-11 17:40:25.676199 wrangles-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2023-06-11 17:16:14.000000 wrangles-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.630921 wrangles-1.3.0/wrangles/
+-rw-rw-rw-   0        0        0      565 2022-06-23 01:29:50.000000 wrangles-1.3.0/wrangles/__init__.py
+-rw-rw-rw-   0        0        0     1681 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/auth.py
+-rw-rw-rw-   0        0        0      840 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/batching.py
+-rw-rw-rw-   0        0        0     2069 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/classify.py
+-rw-rw-rw-   0        0        0      559 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/config.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.666230 wrangles-1.3.0/wrangles/connectors/
+-rw-rw-rw-   0        0        0      449 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7108 2023-06-11 17:29:44.000000 wrangles-1.3.0/wrangles/connectors/akeneo.py
+-rw-rw-rw-   0        0        0    11023 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/ckan.py
+-rw-rw-rw-   0        0        0     7811 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/file.py
+-rw-rw-rw-   0        0        0     2498 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/http.py
+-rw-rw-rw-   0        0        0     1883 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/jinja.py
+-rw-rw-rw-   0        0        0     4830 2023-06-11 17:30:43.000000 wrangles-1.3.0/wrangles/connectors/mongodb.py
+-rw-rw-rw-   0        0        0     6136 2022-12-19 21:12:29.000000 wrangles-1.3.0/wrangles/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4372 2022-12-19 21:12:29.000000 wrangles-1.3.0/wrangles/connectors/mysql.py
+-rw-rw-rw-   0        0        0     6328 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/notification.py
+-rw-rw-rw-   0        0        0     5892 2022-06-23 01:29:50.000000 wrangles-1.3.0/wrangles/connectors/postgres.py
+-rw-rw-rw-   0        0        0    16169 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/pricefx.py
+-rw-rw-rw-   0        0        0     4534 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/recipe.py
+-rw-rw-rw-   0        0        0     8527 2023-06-11 17:31:29.000000 wrangles-1.3.0/wrangles/connectors/s3.py
+-rw-rw-rw-   0        0        0     4754 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/connectors/salesforce.py
+-rw-rw-rw-   0        0        0     4442 2022-12-19 21:12:29.000000 wrangles-1.3.0/wrangles/connectors/sftp.py
+-rw-rw-rw-   0        0        0     2430 2022-12-19 21:12:29.000000 wrangles-1.3.0/wrangles/connectors/ssh.py
+-rw-rw-rw-   0        0        0     5651 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/test.py
+-rw-rw-rw-   0        0        0     8037 2023-06-11 17:20:06.000000 wrangles-1.3.0/wrangles/connectors/train.py
+-rw-rw-rw-   0        0        0     1899 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/console.py
+-rw-rw-rw-   0        0        0     1588 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/data.py
+-rw-rw-rw-   0        0        0    10100 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/extract.py
+-rw-rw-rw-   0        0        0     4412 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/format.py
+-rw-rw-rw-   0        0        0    21142 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.675200 wrangles-1.3.0/wrangles/recipe_wrangles/
+-rw-rw-rw-   0        0        0      585 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/convert.py
+-rw-rw-rw-   0        0        0     8695 2023-06-11 17:22:18.000000 wrangles-1.3.0/wrangles/recipe_wrangles/create.py
+-rw-rw-rw-   0        0        0    21176 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/extract.py
+-rw-rw-rw-   0        0        0     8126 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/format.py
+-rw-rw-rw-   0        0        0    27181 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/main.py
+-rw-rw-rw-   0        0        0     8584 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/merge.py
+-rw-rw-rw-   0        0        0     4041 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/pandas.py
+-rw-rw-rw-   0        0        0     8715 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/select.py
+-rw-rw-rw-   0        0        0     6791 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/split.py
+-rw-rw-rw-   0        0        0     1883 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/select.py
+-rw-rw-rw-   0        0        0     2099 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/standardize.py
+-rw-rw-rw-   0        0        0     6067 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/train.py
+-rw-rw-rw-   0        0        0     3502 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/translate.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.652861 wrangles-1.3.0/wrangles.egg-info/
+-rw-rw-rw-   0        0        0     4464 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1422 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      159 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/top_level.txt
```

### Comparing `wrangles-1.2.1/PKG-INFO` & `wrangles-1.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: wrangles
-Version: 1.2.1
-Summary: Wrangle your data into shape with machine learning
-Home-page: https://github.com/wrangleworks/WranglesPy
-Author: WrangleWorks
-Author-email: chris@wrangleworks.com
-License: Apache License 2.0
-Keywords: data,wrangling
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # Wrangles
 
 Full documentation available at [wrangles.io](https://wrangles.io/python).
 
 ## What are Wrangles?
 
 Wrangles are a set of modular transformations for data cleaning and enrichment. Each Wrangle is optimized for a particular job, many of which are backed by sophisticated machine learning models.
@@ -114,9 +99,7 @@
       input: my column
       case: upper
 
 write:
   - file:
       name: file.xlsx
 ```
-
-
```

### Comparing `wrangles-1.2.1/setup.py` & `wrangles-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     license_files = ('LICENSE.txt',),
     license = 'Apache License 2.0',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
-    version = '1.2.1',
+    version = '1.3.0',
     url = 'https://github.com/wrangleworks/WranglesPy',
     author = 'WrangleWorks',
     author_email = 'chris@wrangleworks.com',
     keywords = ['data','wrangling'],
     install_requires = requirements,
     entry_points ={
         'console_scripts': ['wrangles.recipe = wrangles.console:recipe']
```

### Comparing `wrangles-1.2.1/wrangles/__init__.py` & `wrangles-1.3.0/wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/auth.py` & `wrangles-1.3.0/wrangles/auth.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/batching.py` & `wrangles-1.3.0/wrangles/batching.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/classify.py` & `wrangles-1.3.0/wrangles/classify.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/config.py` & `wrangles-1.3.0/wrangles/config.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/akeneo.py` & `wrangles-1.3.0/wrangles/connectors/akeneo.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     else:
         json_response = _json.loads(response.text)
         raise ValueError(f"Status Code: {json_response['code']} Message: {json_response['message']}")
 
 
 _schema['write'] = """
 type: object
-description: Export data to a file
+description: Write data into an Akeneo PIM
 required:
   - host
   - user
   - password
   - client_id
   - client_secret
   - source
```

### Comparing `wrangles-1.2.1/wrangles/connectors/ckan.py` & `wrangles-1.3.0/wrangles/connectors/ckan.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/file.py` & `wrangles-1.3.0/wrangles/connectors/file.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/http.py` & `wrangles-1.3.0/wrangles/connectors/http.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/jinja.py` & `wrangles-1.3.0/wrangles/connectors/jinja.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/mongodb.py` & `wrangles-1.3.0/wrangles/connectors/mongodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as _pd
 import pymongo as _pymongo
 import logging as _logging
 from typing import Union as _Union
+from urllib.parse import quote_plus
 
 _schema = {}
 
 def read(user: str, password: str, database: str, collection: str, host: str, query: dict = {}, projection: dict = {}) -> _pd.DataFrame:
     """
     Import data from a MongoDB database
     
@@ -19,14 +20,18 @@
     :param host: mongoDB cluster-url
     :param query: mongoDB query
     :param projection: (Optional) Select which fields to include
     """
     
     _logging.info(f": Importing Data :: {database}.{collection}")
     
+    # Encoding password and username using percent encoding
+    user = quote_plus(user)
+    password = quote_plus(password)
+    
     conn = f"mongodb+srv://{user}:{password}@{host}/?retryWrites=true&w=majority"
     client = _pymongo.MongoClient(conn)
     db = client[database]
     col = db[collection]
     
     # checking if database and collections are in mongoDB
     if database not in client.list_database_names(): raise ValueError('MongoDB database not found.')
@@ -75,15 +80,15 @@
     type: string
     description: Select which fields to include
 """
 
 
 def write(df: _pd.DataFrame, user: str, password: str, database: str, collection: str, host: str, action: str, query: dict = None, update: dict=None, columns: _Union[str, list] = None) -> None:
     """
-    Write data into a monfoDB database
+    Write data into a mongoDB database
     
     >>> from wrangles.connectors import mongodb
     >>> df = mongodb.write(user='user, password='password', database='db', host='cluster0.mongodb.net', action: INSERT)
     
     :param df: Dataframe to be exported
     :param user: User with access to the database
     :param password: Password of user
@@ -91,14 +96,19 @@
     :param collection: Collection to be queried
     :param host: mongobd cluster-url
     :param action: actions supported INSERT, UPDATE
     :pram query: mongoDB query to search for value to update, only valid when using UPDATE
     :param update: mongoDB query value to update, only valid when using UPDATE
     
     """
+    
+    # Encoding password and username using percent encoding
+    user = quote_plus(user)
+    password = quote_plus(password)
+    
     conn = f"mongodb+srv://{user}:{password}@{host}/?retryWrites=true&w=majority"
     client = _pymongo.MongoClient(conn)
     db = client[database]
     col = db[collection]
     
     # Select only specific columns if user requests them
     if columns is not None: df = df[columns]
@@ -110,15 +120,15 @@
     
     try:
       client.close()
     except:
       pass
 _schema['write'] = """
 type: object
-description: insert, delete, or update data to a mongoDB Server
+description: Write data into a mongoDB database
 required:
   - user
   - password
   - database
   - collection
   - host
   - action
```

### Comparing `wrangles-1.2.1/wrangles/connectors/mssql.py` & `wrangles-1.3.0/wrangles/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/mysql.py` & `wrangles-1.3.0/wrangles/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/notification.py` & `wrangles-1.3.0/wrangles/connectors/notification.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/postgres.py` & `wrangles-1.3.0/wrangles/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/pricefx.py` & `wrangles-1.3.0/wrangles/connectors/pricefx.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/recipe.py` & `wrangles-1.3.0/wrangles/connectors/recipe.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/s3.py` & `wrangles-1.3.0/wrangles/connectors/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from . import file as _file
 
 
 _schema = {}
 
 def read(bucket: str, key: str, access_key: str = None, secret_access_key: str = None, **kwargs) -> _pd.DataFrame:
     """
-    Import a data from a file in AWS S3
+    Import data from a file in AWS S3
     
     :param bucket: The name of the bucket to download object from
     :param key: The name of the key to download from
     :param access_key: S3 access key
     :param secret_access_key: S3 secret access key
     :param kwargs: (Optional) Named arguments to pass to respective pandas read a file function.
     """
@@ -32,15 +32,15 @@
     response = _BytesIO(response.read())
     df = _file.read(key, file_object=response, **kwargs)    
  
     return df
     
 _schema['read'] = """
 type: object
-description: Import a data from a file in AWS S3
+description: Import data from a file in AWS S3
 required:
   - bucket
   - key
 properties:
   bucket:
     type: string
     description: The name of the bucket where file will be read
@@ -54,15 +54,15 @@
     type: string
     description: S3 secret access key
     
 """
 
 def write(df: _pd.DataFrame, bucket: str, key: str, access_key: str = None, secret_access_key: str = None, **kwargs):
     """
-    Write a file in AWS S3
+    Write a file to AWS S3
     
     :param df: Dataframe to be exported
     :param bucket: The name of the bucket where file will be written
     :param key: The name of the key to download from
     :param access_key: S3 access key
     :param secret_access_key: S3 secret access key
     :param kwargs: (Optional) Named arguments to pass to respective pandas write a file function.
@@ -79,15 +79,15 @@
     _file.write(df, name=key, file_object=memory_file, **kwargs)
     memory_file.seek(0, 0)
     _logging.info(f": Writing File :: {bucket}.{key}")
     s3.put_object(Bucket=bucket, Body=memory_file, Key=key)
     
 _schema['write'] = """
 type: object
-description: write files to AWS S3
+description: Write a file to AWS S3
 required:
   - bucket
   - key
 properties:
   bucket:
     type: string
     description: The name of the bucket where file will be written
```

### Comparing `wrangles-1.2.1/wrangles/connectors/salesforce.py` & `wrangles-1.3.0/wrangles/connectors/salesforce.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
   instance:
     type: string
     description: The salesforce instance to read from. e.g. <custom>.my.salesforce.com
   user:
     type: string
     description: User with read permission
   password:
-    type: integer
+    type: string
     description: Password for the user
   token:
     type: string
     description: Security token for the user
   object:
     type: string
     description: Object to read data from e.g. Contact
@@ -136,15 +136,15 @@
   instance:
     type: string
     description: The salesforce instance to write to e.g. <custom>.my.salesforce.com
   user:
     type: string
     description: User with write permission
   password:
-    type: integer
+    type: string
     description: Password for the user
   token:
     type: string
     description: Security token for the user
   object:
     type: string
     description: Object to write the data to e.g. Contact
```

### Comparing `wrangles-1.2.1/wrangles/connectors/sftp.py` & `wrangles-1.3.0/wrangles/connectors/sftp.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/ssh.py` & `wrangles-1.3.0/wrangles/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/test.py` & `wrangles-1.3.0/wrangles/connectors/test.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/connectors/train.py` & `wrangles-1.3.0/wrangles/connectors/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         else:
             raise ValueError("Classify Wrangle data should contain three columns. Check Wrangle data")
 
         return _pd.DataFrame(tmp_data, columns=columns)
 
     _schema["read"] = """
         type: object
-        description: Read the training data for a Standardize Wrangle
+        description: Read the training data for a Classify Wrangle
         additionalProperties: false
         required:
           - model_id
         properties:
           model_id:
             type: string
             description: Specific model to read
```

### Comparing `wrangles-1.2.1/wrangles/console.py` & `wrangles-1.3.0/wrangles/console.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/data.py` & `wrangles-1.3.0/wrangles/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,36 @@
         Get a list of the user's models
 
         :param type: (Optional) Specify the type of models. 'classify' or 'extract'
         :returns: List of user's model, each a dict of properties.
         """
         params = {}
         if type: params['type'] = type
-        response = _requests.get(f'{_config.api_host}/data/user/models', params=params, headers={'Authorization': f'Bearer {_auth.get_access_token()}'})
+        response = _requests.get(f'{_config.api_host}/user/models', params=params, headers={'Authorization': f'Bearer {_auth.get_access_token()}'})
         results = response.json()
         return results
 
 
 def model(id: str):
     """
     Get a model definition
     :param id: model ID
     :returns: Dict of model properties
     """
     params = {'id': id}
-    response = _requests.get(f'{_config.api_host}/data/model', params=params, headers={'Authorization': f'Bearer {_auth.get_access_token()}'})
+    response = _requests.get(f'{_config.api_host}/model/metadata', params=params, headers={'Authorization': f'Bearer {_auth.get_access_token()}'})
     results = response.json()
     return results
 
 
 def model_data(id: str, purpose: str) -> list:
     """
     Get the training data for a model
 
     :param id: Model ID
     :param purpose: classify, extract, standardize
     :return: Model data as a list of lists
     """
     params = {'model_id': id, 'type': purpose}
-    response = _requests.get(f'{_config.api_host}/user/model/train', params=params, headers={'Authorization': f'Bearer {_auth.get_access_token()}'})
+    response = _requests.get(f'{_config.api_host}/model/content', params=params, headers={'Authorization': f'Bearer {_auth.get_access_token()}'})
     results = response.json()
     return results['Data']
```

### Comparing `wrangles-1.2.1/wrangles/extract.py` & `wrangles-1.3.0/wrangles/extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,14 @@
     {'length': ['25m']}
 
     :param input: Input string or list of strings to be searched for attributes
     :param responseContent: (Optional, default Span) 'span' or 'object'. If span, returns original text, if object returns an object of value and dimension.
     :param type: (Optional) Specify which types of attributes to find. If omitted, a dict of all attributes types is returned
     :param bound: (Optional, default mid). When returning an object, if the input is a range. e.g. 10-20mm, set the value to return. min, mid or max.
     """
-    # Check that attribute_type is correct
-    attributes_type_list = ["angle","area","current","force","length","power","pressure","electric potential","volume","mass"]
-    if type != None and type.lower() not in attributes_type_list: raise ValueError(f'"{type}" is not a valid attribute_type value.')
     
     if isinstance(input, str): 
         json_data = [input]
     else:
         json_data = input
 
     url = f'{_config.api_host}/wrangles/extract/attributes'
@@ -97,15 +94,16 @@
     results = _batching.batch_api_calls(url, params, json_data, batch_size)
 
     if isinstance(input, str): results = results[0]
     
     return results
 
 
-def custom(input: _Union[str, list], model_id: str, first_element: bool = False) -> list:
+def custom(input: _Union[str, list], model_id: str, first_element: bool = False, use_labels: bool = False) -> list:
+
     """
     Extract entities using a custom model.
     Requires WrangleWorks Account and Subscription.
 
     :param input: A string or list of strings to searched for information.
     :param model_id: The model to be used to search for information.
     :return: A list of entities found.
@@ -125,29 +123,35 @@
     if isinstance(model_id, str): model_id = [model_id]
     for model in model_id:
         # Checking to see if GUID format is correct
         if [len(x) for x in model.split('-')] != [8, 4, 4]:
             raise ValueError('Incorrect or missing values in model_id. Check format is XXXXXXXX-XXXX-XXXX')
 
     url = f'{_config.api_host}/wrangles/extract/custom'
-    params = {'responseFormat': 'array', 'model_id': model_id}
+    params = {'responseFormat': 'array', 'model_id': model_id, 'use_labels': use_labels}
     model_properties = _data.model(model_id)
     # If model_id format is correct but no mode_id exists
     if model_properties.get('message', None) == 'error': raise ValueError('Incorrect model_id.\nmodel_id may be wrong or does not exists')
     batch_size = model_properties['batch_size'] or 10000
     
     # Using model_id in wrong function
     purpose = model_properties['purpose']
     if purpose != 'extract':
         raise ValueError(f'Using {purpose} model_id in an extract function.')
     
     results = _batching.batch_api_calls(url, params, json_data, batch_size)
 
-    if first_element:
+
+
+    if first_element and not use_labels:
         results = [x[0] if len(x) >= 1 else "" for x in results]
+    
+    if use_labels and first_element:
+        results = [{k:v[0] for (k, v) in zip(objs.keys(), objs.values())} for objs in results]
+    
 
     if isinstance(input, str): results = results[0]
     
     return results
 
 
 def html(input: _Union[str, list], dataType: str) -> list:
```

### Comparing `wrangles-1.2.1/wrangles/format.py` & `wrangles-1.3.0/wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/recipe.py` & `wrangles-1.3.0/wrangles/recipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,31 +289,48 @@
                 try:
                     custom_function = functions[wrangle[7:]]
                 except:
                     raise ValueError(f'Custom Wrangle function: "{wrangle}" not found')
 
                 # Get user's function arguments
                 function_args = _inspect.getfullargspec(custom_function).args
+                # Drop params from function_args
+                for arg in function_args:
+                    if arg in params.keys():
+                        function_args.remove(arg)
 
-                if function_args[0] == 'df':
+                # Check for function_args and df
+                if len(function_args) > 0 and 'df' in function_args:
                     # If user's first argument is df, pass them the whole dataframe
-                    df = functions[wrangle[7:]](df, **params)
-                elif function_args[0] == 'cell':
-                    # If user's first function is cell, pass them the cells defined by the parameter input individually
-                    input_column = params['input']
-                    params.pop('input')
-                    if params.get('output') is None:
-                        output_column = input_column
-                    else:
-                        output_column = params['output']
-                        params.pop('output')
-                    df[output_column] = [custom_function(cell, **params) for cell in df[input_column].to_list()]
+                    df = functions[wrangle[7:]](df=df, **params)
 
+                # Dealing with no function_args
                 else:
-                    df[params['output']] = df[function_args].apply(lambda x: custom_function(**x), axis=1, result_type='expand')
+                    df_temp = df
+
+                    if 'input' in params:
+                        params['input'] = _wildcard_expansion(all_columns=df.columns.tolist(), selected_columns=params['input'])
+                        df_temp = df_temp[params['input']]
+                    # Drop columns from df_temp that are not in function_args
+                    if function_args:
+                        try:
+                            df_temp = df_temp[function_args]
+                        except:
+                            raise KeyError(f"input/output passed without df. Pass df as a function variable or use the column header in place of input/output to fix this issue. See https://wrangles.io/python/recipes/custom-functions/wrangles for more information")
+                    # Create params_temp and drop input/output
+                    params_temp = params.copy()
+                    if 'input' in params_temp.keys():
+                        params_temp.pop('input')
+                    if 'output' in params_temp.keys():
+                        params_temp.pop('output')
+                    # {**x, **params_temp} deals with columns in function args and **params_temp without columns
+                    try:
+                        df[params['output']] = df_temp.apply(lambda x: custom_function(**{**x, **params_temp}), axis=1, result_type='expand')
+                    except:    
+                        df[params['output']] = df_temp.apply(lambda x: custom_function(**params_temp), axis=1, result_type='expand')
 
             else:
                 # Blacklist of Wrangles not to allow wildcards for
                 if wrangle not in ['math', 'maths', 'merge.key_value_pairs', 'split.text', 'split.list', 'split.dictionary'] and 'input' in params:
                     # Expand out any wildcards or regex in column names
                     params['input'] = _wildcard_expansion(all_columns=df.columns.tolist(), selected_columns=params['input'])
                         
@@ -344,15 +361,16 @@
     if columns:
         columns = _wildcard_expansion(df.columns.tolist(), columns)
         df = df[columns]
 
     # Remove any columns specified by the user
     if not_columns:
         not_columns = _wildcard_expansion(df.columns.tolist(), not_columns)
-        remaining_columns = list(set(df.columns) - set(not_columns))
+        # List comprehension is used below to preserve order of columns 
+        remaining_columns = [column for column in list(df.columns) if column not in not_columns]
         df = df[remaining_columns]
 
     if where:
         df = _recipe_wrangles.sql(
             df,
             f"""
             SELECT *
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/__init__.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 wrangles:
   - classify:
 
   - convert.case:
 
 """
 from .main import *
+from .pandas import *
 from . import convert
 from . import create
 from . import extract
 from . import format
 from . import merge
 from . import select
 from . import split
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/convert.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     # Get the requested case, default lower
     desired_case = case.lower()
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
+
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
         if desired_case == 'lower':
             df[output_column] = df[input_column].str.lower()
         elif desired_case == 'upper':
             df[output_column] = df[input_column].str.upper()
         elif desired_case == 'title':
@@ -91,15 +95,19 @@
     """
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
-        
+    
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
+
     # If the datatype is datetime
     if data_type == 'datetime':
         temp = _pd.to_datetime(df[input].stack(), **kwargs).unstack()
         df[output] = temp
 
     else:
         # Loop through and apply for all columns
@@ -133,14 +141,18 @@
     # Set the output column as input if not provided
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
     
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
+    
     for in_col, out_col in zip(input, output):
       results = []
       for item in df[in_col].astype(str):
           fractions = fractions = _re.finditer(r'\b\d+/\d+\b', item)
           replacement_list = []
           for match in fractions:
               fraction_str = match.group()
@@ -179,14 +191,18 @@
     """
     # Set output column as input if not provided
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
+    
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
         
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] = [_json.loads(x) for x in df[input_column]]
     
     return df
 
@@ -212,13 +228,17 @@
     """
     # Set output column as input if not provided
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
+    
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
         
     # Loop through and apply for all columns
     for input_columns, output_column in zip(input, output):
         df[output_column] = [_json.dumps(row) for row in df[input_columns].values.tolist()]
         
     return df
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/create.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from ..connectors.test import _generate_cell_values
 
 
 def bins(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], bins: _Union[int, list], labels: _Union[str, list] = None, **kwargs) -> _pd.DataFrame:
     """
     type: object
-    description: Creates a column that segment and sort data values into bins
+    description: Create a column that groups data into bins
     additionalProperties: false
     required:
       - input
       - output
       - bins
     properties:
       input:
@@ -44,14 +44,18 @@
         description: Labels for the returned bins
     """
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
+    
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
 
     for in_col, out_col in zip(input, output):
       # Dealing with positive infinity. At end of bins list
       if isinstance(bins, list):
           if bins[-1] == '+':
               bins[-1] = _math.inf
           
@@ -164,38 +168,36 @@
     # Loop through and create incremental index
     for output_column in output:
         df[output_column] = _np.arange(start, len(df) * step + start, step=step)
 
     return df
 
 
-def jinja(df: _pd.DataFrame, template: dict, output: _Union[str, list], input: str = None) -> _pd.DataFrame:
+def jinja(df: _pd.DataFrame, template: dict, output: list, input: str = None) -> _pd.DataFrame:
     """
     type: object
     description: Output text using a jinja template
     additionalProperties: false
     required:
       - output
       - template
     properties:
       input:
         type: string
         description: |
           Specify a name of column containing a dictionary of elements to be used in jinja template.
           Otherwise, the column headers will be used as keys.
       output:
-        type: 
-          - string
-          - array
+        type: string
         description: Name of the column to be output to.
       template:
         type: object
         description: |
           A dictionary which defines the template/location as well as the form which the template is input.
-          If any keys use a space, it must be replaced with an underscore.
+          If any keys use a space, they must be replaced with an underscore.
         additionalProperties: false
         properties:
           file:
             type: string
             description: A .jinja file containing the template
           column:
             type: string
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/extract.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     """
     type: object
     description: Extract parts of addresses. Requires WrangleWorks Account.
     additionalProperties: false
     required:
       - input
       - output
-      - dataType
     properties:
       input:
         type:
           - string
           - array
         description: Name of the input column.
       output:
@@ -41,20 +40,26 @@
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
-    # Ensure input and output are equal lengths
-    if len(input) != len(output):
-        raise ValueError('The lists for input and output must be the same length.')
-  
-    for input_column, output_column in zip(input, output):
-        df[output_column] = _extract.address(df[input_column].astype(str).tolist(), dataType)
+    # Ensure input and output lengths are compatible
+    if len(input) != len(output) and len(output) > 1:
+        raise ValueError('Extract must output to a single column or equal amount of columns as input.')
+
+    if len(output) == 1 and len(input) > 1:
+        df[output[0]] = _extract.address(
+            df[input].astype(str).aggregate(' '.join, axis=1).tolist(), dataType)
+    else:
+        # Loop through and apply for all columns
+        for input_column, output_column in zip(input, output):
+            df[output_column] = _extract.address(
+                df[input_column].astype(str).tolist(), dataType)
   
     return df
 
 
 def attributes(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], responseContent: str = 'span', attribute_type: str = None, desired_unit: str = None, bound: str = 'mid') -> _pd.DataFrame:
     """
     type: object
@@ -89,18 +94,21 @@
           - electrical resistance
           - energy
           - force
           - frequency
           - inductance
           - instance frequency
           - length
+          - luminous flux
           - mass
+          - weight
           - power
           - pressure
           - speed
+          - velocity
           - temperature
           - time
           - volume
           - volumetric flow
       responseContent:
         type: string
         description: span - returns the text found. object - returns an object with the value and unit
@@ -118,32 +126,41 @@
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
-    # Ensure input and output are equal lengths
-    if len(input) != len(output):
-        raise ValueError('The lists for input and output must be the same length.')
-
-    # Loop through and apply for all columns
-    for input_column, output_column in zip(input, output):
-        df[output_column] = _extract.attributes(
-            df[input_column].astype(str).tolist(),
-            responseContent,
-            attribute_type,
-            desired_unit,
-            bound
+    # Ensure input and output lengths are compatible
+    if len(input) != len(output) and len(output) > 1:
+        raise ValueError('Extract must output to a single column or equal amount of columns as input.')
+    
+    if len(output) == 1 and len(input) > 1:
+        # df[output[0]] = _extract.attributes(df[input].astype(str).aggregate(' AAA '.join, axis=1).tolist())
+        df[output[0]] = _extract.attributes(
+            df[input].astype(str).aggregate(' AAA '.join, axis=1).tolist(),
+              responseContent,
+              attribute_type,
+              desired_unit,
+              bound)
+    else:
+        # Loop through and apply for all columns
+        for input_column, output_column in zip(input, output):
+            df[output_column] = _extract.attributes(
+                df[input_column].astype(str).tolist(),
+                responseContent,
+                attribute_type,
+                desired_unit,
+                bound
         )
         
     return df
 
 
-def brackets(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list]) -> _pd.DataFrame:
+def brackets(df: _pd.DataFrame, input: str, output: str) -> _pd.DataFrame:
     """
     type: object
     description: Extract text properties in brackets from the input
     additionalProperties: false
     required:
       - input
       - output
@@ -162,21 +179,24 @@
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
-    # Ensure input and output are equal lengths
-    if len(input) != len(output):
-        raise ValueError('The lists for input and output must be the same length.')
+    # Ensure input and output lengths are compatible
+    if len(input) != len(output) and len(output) > 1:
+        raise ValueError('Extract must output to a single column or equal amount of columns as input.')
 
-    # Loop through and apply for all columns
-    for input_column, output_column in zip(input, output):
-        df[output_column] = _extract.brackets(df[input_column].astype(str).tolist())
+    if len(output) == 1 and len(input) > 1:
+        df[output[0]] = _extract.brackets(df[input].astype(str).aggregate(' '.join, axis=1).tolist())
+    else:
+        # Loop through and apply for all columns
+        for input_column, output_column in zip(input, output):
+            df[output_column] = _extract.brackets(df[input_column].astype(str).tolist())
 
     return df
 
 
 def codes(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list]) -> _pd.DataFrame:
     """
     type: object
@@ -200,33 +220,40 @@
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
+    # Ensure input and output lengths are compatible
+    if len(input) != len(output) and len(output) > 1:
+        raise ValueError('Extract must output to a single column or equal amount of columns as input.')
+
     if len(output) == 1 and len(input) > 1:
         df[output[0]] = _extract.codes(df[input].astype(str).aggregate(' AAA '.join, axis=1).tolist())
     else:
-        # Ensure input and output are equal lengths
-        if len(input) != len(output) and len(output) > 1:
-            raise ValueError('The lists for input and output must be the same length.')
-
         # Loop through and apply for all columns
         for input_column, output_column in zip(input, output):
             df[output_column] = _extract.codes(df[input_column].astype(str).tolist())
 
     return df
 
 
-def custom(df: _pd.DataFrame, input: _Union[str, list], model_id: _Union[str, list], output: _Union[str, list] = None, use_labels: bool = False, first_element: bool = False) -> _pd.DataFrame:
+def custom(
+        df: _pd.DataFrame,
+        input: _Union[str, list],
+        model_id: _Union[str, list],
+        output: _Union[str, list] = None,
+        use_labels: bool = False,
+        first_element: bool = False
+        ) -> _pd.DataFrame:
     """
     type: object
     description: Extract data from the input using a DIY or bespoke extraction wrangle. Requires WrangleWorks Account and Subscription.
-    additionalProperties: false
+    additionalProperties: true
     required:
       - input
       - model_id
     properties:
       input:
         type:
           - string
@@ -240,15 +267,15 @@
       model_id:
         type:
           - string
           - array
         description: The ID of the wrangle to use
       use_labels:
         type: boolean
-        description: Use Labels in the extract output {label: value}
+        description: "Use Labels in the extract output {label: value}"
       first_element:
         type: boolean
         description: Get the first element from results
     """
     if output is None: output = input
     
     # If a string provided, convert to list
@@ -256,81 +283,29 @@
     if not isinstance(output, list): output = [output]
     if not isinstance(model_id, list): model_id = [model_id]
     
     if len(input) == len(output) and len(model_id) == 1:
         # if one model_id, then use that model for all columns inputs and outputs
         model_id = [model_id[0] for _ in range(len(input))]
         for in_col, out_col, model in zip(input, output, model_id):
-            df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element)
+            df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element, use_labels=use_labels)
     
     elif len(input) > 1 and len(output) == 1 and len(model_id) == 1:
         # if there are multiple inputs and one output and one model_id. concatenate the inputs
-        df[output[0]] = _extract.custom(_format.concatenate(df[input].astype(str).values.tolist(), ' '), model_id=model_id, first_element=first_element)
+        df[output[0]] = _extract.custom(_format.concatenate(df[input].astype(str).values.tolist(), ' '), model_id=model_id, first_element=first_element, use_labels=use_labels)
     
     else:
         # Iterate through the inputs, outputs and model_ids
         for in_col, out_col, model in zip(input, output, model_id):
-            df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element)
-
-    # if use_labels is true and output is only one column
-    if (use_labels and len(output) == 1):
-        
-        # if first_element is checked, then the output must be converted to lists to iterate
-        if first_element: df[output[0]] = [[x] for x in df[output[0]]]
-        
-        # Run the custom dictionary maker after normal operation from extract
-        # This will be triggered only if a parameter is set
-        result = []
-        for out_row in df[output[0]]:
-        
-            dict_output = {'Unlabeled': []}
-            # Iterating over the results
-            for item in out_row:
-                
-                try:
-                    item = item.strip()
-                    # Check if the item contains a colon
-                    if (item.count(':') == 1 and item.split(':')[0] != ''):
-                        
-                        # get the key and value from item split
-                        key, value = map(str.strip, item.split(':', 1))
-                        
-                        if dict_output.get(key, ''):
-                            # if the keys is already present, then append to the list
-                            dict_output[key].append(value)
-
-                        else:
-                            dict_output[key] = [value]
-                            
-                    else:
-                        dict_output['Unlabeled'].append(item)
-                except:
-                    dict_output['Unlabeled'].append(item)
-            
-            # putting Unlabeled at the end of the dictionary
-            tmp_unlabeled = dict_output['Unlabeled']
-            del dict_output['Unlabeled']
-            output_dict = _OrderedDict(dict_output)
-            output_dict['Unlabeled'] = tmp_unlabeled
-            
-            # check if the Unlabeled key is empty if yes, delete the key
-            if len(output_dict['Unlabeled']) == 0: del output_dict['Unlabeled']
-            
-            # if first element is set then get the first value as string in dictionary, else return the dictionary
-            if first_element: output_dict = {list(dict(output_dict).keys())[0]: list(dict(output_dict).values())[0][0]}
-            else: output_dict = dict(output_dict)
-            
-            result.append(output_dict)
-            
-        df[output[0]] = result
+            df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element, use_labels=use_labels)
         
     return df
 
 
-def date_properties(df: _pd.DataFrame, input: _pd.Timestamp, property: str, output: _Union[str, list] = None) -> _pd.DataFrame:
+def date_properties(df: _pd.DataFrame, input: _pd.Timestamp, property: str, output: str = None) -> _pd.DataFrame:
     """
     type: object
     description: Extract date properties from a date (day, month, year, etc...)
     additionalProperties: false
     required:
       - input
       - property
@@ -361,51 +336,83 @@
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
-    # Ensure input and output are equal lengths
-    if len(input) != len(output):
-        raise ValueError('The lists for input and output must be the same length.')
-
-    # Loop through and apply for all columns
-    for input_column, output_column in zip(input, output):
-        # Converting data to datetime
-        df_temp = _pd.to_datetime(df[input_column])
-        
-        properties_object = {
-            'day': df_temp.dt.day,
-            'day_of_year': df_temp.dt.day_of_year,
-            'month': df_temp.dt.month,
-            'month_name': df_temp.dt.month_name(),
-            'weekday': df_temp.dt.weekday,
-            'week_day_name': df_temp.dt.day_name(),
-            'week_year': df_temp.dt.isocalendar()['week'],
-            'quarter': df_temp.dt.quarter,
-        }
-        
-        if property in properties_object.keys():
-            df[output_column] = properties_object[property]
-        else:
-            raise ValueError(f"\"{property}\" not a valid date property.")
+    # Ensure input and output lengths are compatible
+    if len(input) != len(output) and len(output) > 1:
+        raise ValueError('Extract must output to a single column or equal amount of columns as input.')
     
+    if len(output) == 1 and len(input) > 1:
+        output = [output[0] for i in range(len(input))]
+        # df_temp = df[input].apply(_pd.to_datetime)
+        temp = []
+        # for i in range(len(input)):
+            # Loop through and apply for all columns
+        for input_column, output_column in zip(input, output):
+            # Converting data to datetime
+            df_temp = _pd.to_datetime(df[input_column])
+            
+            properties_object = {
+                'day': df_temp.dt.day,
+                'day_of_year': df_temp.dt.day_of_year,
+                'month': df_temp.dt.month,
+                'month_name': df_temp.dt.month_name(),
+                'weekday': df_temp.dt.weekday,
+                'week_day_name': df_temp.dt.day_name(),
+                'week_year': df_temp.dt.isocalendar()['week'],
+                'quarter': df_temp.dt.quarter,
+            }
+            
+            if property in properties_object.keys() and temp == []:
+                temp.append([properties_object[property][0]])
+
+            elif property in properties_object.keys() and temp != []:
+                for j in range(len(df)):
+                    temp[j].append(properties_object[property][0])
+
+            else:
+                raise ValueError(f"\"{property}\" not a valid date property.")
+        df[output[0]] = temp
+    else:
+        # Loop through and apply for all columns
+        for input_column, output_column in zip(input, output):
+            # Converting data to datetime
+            df_temp = _pd.to_datetime(df[input_column])
+            
+            properties_object = {
+                'day': df_temp.dt.day,
+                'day_of_year': df_temp.dt.day_of_year,
+                'month': df_temp.dt.month,
+                'month_name': df_temp.dt.month_name(),
+                'weekday': df_temp.dt.weekday,
+                'week_day_name': df_temp.dt.day_name(),
+                'week_year': df_temp.dt.isocalendar()['week'],
+                'quarter': df_temp.dt.quarter,
+            }
+            
+            if property in properties_object.keys():
+                df[output_column] = properties_object[property]
+            else:
+                raise ValueError(f"\"{property}\" not a valid date property.")
     return df
 
 
 def date_range(df: _pd.DataFrame, start_time: _pd.Timestamp, end_time: _pd.Timestamp, output: str, range: str = 'day') -> _pd.DataFrame:
     """
     type: object
     description: Extract date range frequency from two dates
     additionalProperties: false
     required:
       - start_time
       - end_time
       - output
+      - range
     properties:
       start_time:
         type: string
         description: Name of the start date column
       end_time:
         type: string
         description: Name of the end date column
@@ -478,14 +485,15 @@
 def html(df: _pd.DataFrame, input: _Union[str, list], data_type: str, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Extract elements from strings containing html. Requires WrangleWorks Account.
     additionalProperties: false
     required:
       - input
+      - output
       - data_type
     properties:
       input:
         type:
           - string
           - array
         description: Name or list of input columns.
@@ -504,26 +512,26 @@
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
-    # Ensure input and output are equal lengths
-    if len(input) != len(output):
-        raise ValueError('The lists for input and output must be the same length.')
+    # Ensure input and output lengths are compatible
+    if len(input) != len(output) and len(output) > 1:
+        raise ValueError('Extract must output to a single column or equal amount of columns as input.')
     
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] = _extract.html(df[input_column].astype(str).tolist(), dataType=data_type)
             
     return df
 
 
-def properties(df: _pd.DataFrame, input: str, output: str, property_type: str = None, return_data_type: str = 'list') -> _pd.DataFrame:
+def properties(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], property_type: str = None, return_data_type: str = 'list') -> _pd.DataFrame:
     """
     type: object
     description: Extract text properties from the input. Requires WrangleWorks Account.
     additionalProperties: false
     required:
       - input
       - output
@@ -537,70 +545,79 @@
         type:
           - string
           - array
         description: Name of the output columns
       property_type:
         type: string
         description: The specific type of properties to extract
-      return_data_type:
-        type: string
-        description: The format to return the data, as a list or as a string
         enum:
           - Colours
           - Materials
           - Shapes
           - Standards
+      return_data_type:
+        type: string
+        description: The format to return the data, as a list or as a string
+        enum:
+          - list
+          - string
     """
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
-    # Ensure input and output are equal lengths
-    if len(input) != len(output):
-        raise ValueError('The lists for input and output must be the same length.')
-    
-    # Loop through and apply for all columns
-    for input_column, output_column in zip(input, output):
-        df[output_column] = _extract.properties(df[input_column].astype(str).tolist(), type=property_type, return_data_type=return_data_type)
+    # Ensure input and output lengths are compatible
+    if len(input) != len(output) and len(output) > 1:
+        raise ValueError('Extract must output to a single column or equal amount of columns as input.')
+
+    if len(output) == 1 and len(input) > 1:
+        df[output[0]] = _extract.properties(df[input].astype(str).aggregate(' '.join, axis=1).tolist(), type=property_type, return_data_type=return_data_type)
+    else:
+        # Loop through and apply for all columns
+        for input_column, output_column in zip(input, output):
+            df[output_column] = _extract.properties(df[input_column].astype(str).tolist(), type=property_type, return_data_type=return_data_type)
     
     return df
 
 
-def regex(df: _pd.DataFrame, input: str, find: str, output: str) -> _pd.DataFrame:
+def regex(df: _pd.DataFrame, input: _Union[str, list], find: str, output: _Union[str, list]) -> _pd.DataFrame:
     """
     type: object
     description: Extract single values using regex
     additionalProperties: false
     required:
       - input
       - output
-      - find
     properties:
       input:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the input column.
     output:
       type: string
       description: Name of the output column.
-    find:
-      type: string
-      description: Pattern to find using regex
+      find:
+        type: 
+          - string
+          - array
+        description: Pattern to find using regex
     """
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
-    # Ensure input and output are equal lengths
-    if len(input) != len(output):
-        raise ValueError('The lists for input and output must be the same length.')
+    # Ensure input and output lengths are compatible
+    if len(input) != len(output) and len(output) > 1:
+        raise ValueError('Extract must output to a single column or equal amount of columns as input.')
     
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].apply(lambda x: _re.findall(find, x))
     
     return df
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/format.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     for input_column, output_column in zip(input, output):
         # convert the column to timestamp type and format date
         df[output_column] = _pd.to_datetime(df[input_column]).dt.strftime(format)
     
     return df
     
     
-def pad(df: _pd.DataFrame, input: _Union[str, list], pad_length: int, side: str, char: _Union[str, int], output: _Union[str, list] =  None) -> _pd.DataFrame:
+def pad(df: _pd.DataFrame, input: _Union[str, list], pad_length: int, side: str, char: str, output: _Union[str, list] =  None) -> _pd.DataFrame:
     """
     type: object
     description: Pad a string to a fixed length
     additionalProperties: false
     required:
       - input
       - pad_length
@@ -74,22 +74,17 @@
         type:
           - number
         description: Length for the output
       side:
         type:
           - string
         description:  Side from which to fill resulting string
-        enum:
-          - left
-          - right
-          - both
       char:
         type:
           - string
-          - int
         description: The character to pad the input with
   """
     char = str(char)
     # If the output is not specified, overwrite input columns in place
     if output is None: output = input
     
     # If the input is a string
@@ -181,15 +176,15 @@
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] =  _format.remove_duplicates(df[input_column].values.tolist())
 
     return df
 
 
-def suffix(df: _pd.DataFrame, input: _Union[str, list], value: str, output: _Union[str, list] = None) -> _pd.DataFrame:
+def suffix(df: _pd.DataFrame, input: _Union[str, list], value: _Union[str, list], output: str = None) -> _pd.DataFrame:
     """
     type: object
     description: Add a suffix to a column
     additionalProperties: false
     required:
         - input
         - value
@@ -247,14 +242,18 @@
     """
     if output is None: output = input
 
     # If a string provided, convert to list
     if isinstance(input, str): input = [input]
     if isinstance(output, str): output = [output]
 
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
+
     # Loop through all requested columns
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].str.strip()
 
     return df
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/main.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         df[output_column] = results
 
     return df
 
 
 def filter(
           df: _pd.DataFrame,
-          input: list = [],
+          input: _Union[str, list] = [],
           equal: _Union[str, list] = None,
           not_equal: _Union[str, list] = None,
           is_in: _Union[str, list] = None,
           not_in: _Union[str, list] = None,
           greater_than: _Union[int, float] = None,
           greater_than_equal_to: _Union[int, float] = None,
           less_than: _Union[int, float] = None,
@@ -173,22 +173,20 @@
           - array
         description: |
           Name of the column to filter on.
           If multiple are provided, all must match the criteria.
       equal:
         type:
           - string
-          - integer
-          - number
+          - array
         description: Select rows where the values equal a given value.
       not_equal:
         type:
           - string
-          - integer
-          - number
+          - array
         description: Select rows where the values do not equal a given value.
       is_in:
         type:
           - array
           - string
         description: Select rows where the values are in a given list.
       not_in:
@@ -481,22 +479,23 @@
         df = df_temp
     else:
         df = original_df.merge(df_temp[output_columns], how='left', left_index=True, right_index=True)
         
     return df
 
 
-def remove_words(df: _pd.DataFrame, input: _Union[str, list], to_remove: _Union[str, list], output: _Union[str, list] = None, tokenize_to_remove: bool = False, ignore_case: bool = True) -> _pd.DataFrame:
+def remove_words(df: _pd.DataFrame, input: _Union[str, list], to_remove: str, output: _Union[str, list] = None, tokenize_to_remove: bool = False, ignore_case: bool = True) -> _pd.DataFrame:
     """
     type: object
     description: Remove all the elements that occur in one list from another.
     additionalProperties: false
     required:
       - input
       - to_remove
+      - output
     properties:
       input:
         type: 
           - string
           - array
         description: Name of column to remove words from
       to_remove:
@@ -570,21 +569,22 @@
         
         # Otherwise create a dict from input and output columns
         rename_dict = dict(zip(input, output))
 
     return df.rename(columns=rename_dict)
 
 
-def replace(df: _pd.DataFrame, input: _Union[str, list], find: str, replace: str, output: _Union[str, list] = None) -> _pd.DataFrame:
+def replace(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], find: str, replace: str) -> _pd.DataFrame:
     """
     type: object
     description: Quick find and replace for simple values. Can use regex in the find field.
     additionalProperties: false
     required:
       - input
+      - output
       - find
       - replace
     properties:
       input:
         type:
           - string
           - array
@@ -690,28 +690,51 @@
           - array
         description: Name or list of output columns
       model_id:
         type:
           - string
           - array
         description: The ID of the wrangle to use (do not include 'find' and 'replace')
+      find:
+        type:
+          - string
+        description: Pattern to find using regex (do not include model_id)
+      replace:
+        type:
+          - string
+        description: Value to replace the pattern found (do not include model_id)
     """
     # If user hasn't specified an output column, overwrite the input
     if output is None: output = input
 
     # If user provides a single string, convert all the arguments to lists for consistency
     if isinstance(input, str): input = [input]
     if isinstance(output, str): output = [output]
     if isinstance(model_id, str): model_id = [model_id]
 
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
+    
+    # If Several model ids applied to a column in place
+    if all(len(x) == 1 for x in [input, output]) and isinstance(model_id, list):
+        tmp_output = input
+        df_copy = df.loc[:, [input[0]]]
+        for model in model_id:
+            for input_column, output_column in zip(input, tmp_output):
+                df_copy[output_column] = _standardize(df_copy[output_column].astype(str).tolist(), model)
+        
+        # Adding the result of the df_copy to the original dataframe
+        df[output[0]] = df_copy[output_column]
+        return df
+
     for model in model_id:
         for input_column, output_column in zip(input, output):
             df[output_column] = _standardize(df[input_column].astype(str).tolist(), model)
-
-
+            
     return df
 
 
 def translate(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], target_language: str, source_language: str = 'AUTO', case: str = None) -> _pd.DataFrame:
     """
     type: object
     description: Translate the input to a different language. Requires WrangleWorks Account and DeepL API Key (A free account for up to 500,000 characters per month is available).
@@ -727,22 +750,14 @@
           - array
         description: Name of the column to translate
       output:
         type:
           - string
           - array
         description: Name of the output column
-      case:
-        type: string
-        description: Allow changing the case of the input prior to translation. lower, upper or title
-        enum:
-          - lower
-          - upper
-          - title
-          - sentence
       target_language:
         type: string
         description: Code of the language to translate to
         enum:
           - Bulgarian
           - Chinese
           - Czech
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/merge.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     """
     type: object
     description: Concatenate a list of columns or a list within a single column.
     additionalProperties: false
     required:
       - input
       - output
+      - char
     properties:
       input:
         type: 
           - array
           - string
         description: Either a single column name or list of columns
       output:
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/select.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,58 @@
 Functions to select data from within columns
 """
 from typing import Union as _Union
 import pandas as _pd
 from .. import select as _select
 
 
-def dictionary_element(df: _pd.DataFrame, input: _Union[str, list], element: str, output: _Union[str, list] = None,) -> _pd.DataFrame:
+def dictionary_element(
+    df: _pd.DataFrame,
+    input: _Union[str, list],
+    element: str,
+    output: _Union[str, list] = None,
+    default = ''
+) -> _pd.DataFrame:
     """
     type: object
     description: Select a named element of a dictionary.
     additionalProperties: false
     required:
       - input
+      - output
       - element
     properties:
       input:
-        type: string
+        type: 
+          - string
+          - array
         description: Name of the input column
       output:
-        type: string
+        type:
+          - string
+          - array
         description: Name of the output column
       element:
         type: string
         description: The key from the dictionary to select.
+      default:
+        description: Set the default value to return if the specified element doesn't exist.
     """
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
 
+    # Ensure input and output are equal lengths
     if len(input) != len(output):
         raise ValueError('The list of inputs and outputs must be the same length for select.dictionary_element')
     
     for in_col, out_col in zip(input, output):
-        df[out_col] = _select.dict_element(df[in_col].tolist(), element)
+        df[out_col] = _select.dict_element(df[in_col].tolist(), element, default=default)
     
     return df
 
 
 def highest_confidence(df: _pd.DataFrame, input: list, output: _Union[str, list]) -> _pd.DataFrame:
     """
     type: object
@@ -89,54 +103,63 @@
     # If user hasn't provided an output, replace input
     if output is None: output = input
 
     # If a string provided, convert to list
     if isinstance(input, str): input = [input]
     if isinstance(output, str): output = [output]
 
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
+
     # Loop through and get left characters of the length requested for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].str[:length]
 
     return df
 
 
-def list_element(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None, element: int = 0) -> _pd.DataFrame:
+def list_element(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None, element: int = 0, default = '') -> _pd.DataFrame:
     """
     type: object
     description: Select a numbered element of a list (zero indexed).
     additionalProperties: false
     required:
       - input
+      - output
+      - element
     properties:
       input:
         type: 
           - string
           - array
         description: Name of the input column
       output:
         type: 
           - string
           - array
         description: Name of the output column
       element:
         type: integer
         description: The numbered element of the list to select. Starts from zero
+      default:
+        description: Set the default value to return if the specified element doesn't exist.
     """
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
     
+    # Ensure input and output are equal lengths
     if len(input) != len(output):
         raise ValueError('The list of inputs and outputs must be the same length for select.list_element')
     
     for in_col, out_col in zip(input, output):
-        df[out_col] = _select.list_element(df[in_col].tolist(), element)
+        df[out_col] = _select.list_element(df[in_col].tolist(), element, default=default)
     
     return df
 
 
 def right(df: _pd.DataFrame, input: _Union[str, list], length: int, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
@@ -164,14 +187,18 @@
     # If user hasn't provided an output, replace input
     if output is None: output = input
 
     # If a string provided, convert to list
     if isinstance(input, str): input = [input]
     if isinstance(output, str): output = [output]
 
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
+
     # Loop through and get the right characters of the length requested for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].str[-length:]
 
     return df
 
 
@@ -207,14 +234,18 @@
     # If user hasn't provided an output, replace input
     if output is None: output = input
 
     # If a string provided, convert to list
     if isinstance(input, str): input = [input]
     if isinstance(output, str): output = [output]
 
+    # Ensure input and output are equal lengths
+    if len(input) != len(output):
+        raise ValueError('The lists for input and output must be the same length.')
+
     # Loop through and get the substring requested for all requested columns
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].str[start-1:start+length-1]
 
     return df
```

### Comparing `wrangles-1.2.1/wrangles/recipe_wrangles/split.py` & `wrangles-1.3.0/wrangles/recipe_wrangles/split.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 Split a single column to multiple columns
 """
 from typing import Union as _Union
 # Rename List to _list to be able to use function name list without clashing
 from typing import List as _list
 import pandas as _pd
 from .. import format as _format
+import json as _json
 
 
 def dictionary(df: _pd.DataFrame, input: str) -> _pd.DataFrame:
     """
     type: object
     description: Split a dictionary into columns. The dictionary keys will be used as the new column headers.
     additionalProperties: false
     required:
       - input
     properties:
       input:
         type: string
         description: Name of the column to be split
-    """
-    exploded_df = _pd.json_normalize(df[input], max_level=1).fillna('')
+    """ 
+    # storing data as df temp to prevent the original data to be changed
+    df_temp = df[input]
+    try:
+        df_temp = [_json.loads('{}') if x == '' else _json.loads(x) for x in df_temp]
+    except:
+        df_temp = [{} if x == None else x for x in df[input]]
+            
+    exploded_df = _pd.json_normalize(df_temp, max_level=1).fillna('')
     df[exploded_df.columns] = exploded_df
     return df
 
     
 def list(df: _pd.DataFrame, input: str, output: _Union[str, list]) -> _pd.DataFrame:
     """
     type: object
@@ -168,14 +176,15 @@
     """
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, _list): input = [input]
     if not isinstance(output, _list): output = [output]
 
+    # Ensure input and output are equal lengths
     if len(input) != len(output):
         raise ValueError('The list of inputs and outputs must be the same length for split.tokenize')
     
     for in_col, out_col in zip(input, output):
         df[out_col] = _format.tokenize(df[in_col].values.tolist())
             
     return df
```

### Comparing `wrangles-1.2.1/wrangles/select.py` & `wrangles-1.3.0/wrangles/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,26 +41,26 @@
                 results.append(cell_2[0])
             else:
                 results.append(cell_2)
             
     return results
 
 
-def list_element(input, n):
+def list_element(input, n, default = ""):
     """
     Select a numbered element of a list (zero indexed).
     """
     def check_if_possible(element, index):
         try:
             return element[index]
         except IndexError:
-            return ''
+            return default
         
-    return [check_if_possible(row, n) if isinstance(row, list) else '' for row in input]
+    return [check_if_possible(row, n) for row in input]
 
 
-def dict_element(input, key):
+def dict_element(input, key, default=""):
     """
     Select a named element of a dictionary
     """
-    return [row.get(key, '') if isinstance(row, dict) else '' for row in input]
+    return [row.get(key, default) if isinstance(row, dict) else default for row in input]
```

### Comparing `wrangles-1.2.1/wrangles/standardize.py` & `wrangles-1.3.0/wrangles/standardize.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.1/wrangles/train.py` & `wrangles-1.3.0/wrangles/train.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,17 +26,17 @@
                 raise ValueError(f'Training_data list must contain a list of two non-empty elements, plus optional Notes. Check element(s) {check_index} in training_list.\nFormat:\nFirst element is "Example"\nSecond Element is "Category" -- \'\' is not valid.\n'
                 "Example:[['Rice', 'Grain', '']]")
             # checking the first element in training list
             if training_data[0] != ['Example', 'Category', 'Notes']:
                 training_data = [['Example', 'Category', 'Notes']] + training_data
         
         if name:
-            response = _requests.post(f'{_config.api_host}/data/user/model/train', params={'type':'classify', 'name': name}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
+            response = _requests.post(f'{_config.api_host}/model/content', params={'type':'classify', 'name': name}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
         elif model_id:
-            response = _requests.put(f'{_config.api_host}/user/model/train', params={'type':'classify', 'model_id': model_id}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
+            response = _requests.put(f'{_config.api_host}/model/content', params={'type':'classify', 'model_id': model_id}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
         else:
             raise ValueError('Either a name or a model id must be provided')
 
         return response
 
     def extract(training_data: list, name: str = None, model_id: str = None):
         """
@@ -55,17 +55,17 @@
                 raise ValueError(f"Training_data list must contain a list of two elements, plus optional Notes. Check element(s) {check_index} in training_list.\nFormat:\nFirst element is 'Entity to Find'\nSecond Element is 'Variation', If no variation, use \'\'\n"
                 "Example:[['Television', 'TV', '']]")
             # checking the first element in training list
             if training_data[0] != ['Entity to Find', 'Variation (Optional)', 'Notes']:
                 training_data = [['Entity to Find', 'Variation (Optional)', 'Notes']] + training_data
         
         if name:
-            response = _requests.post(f'{_config.api_host}/data/user/model/train', params={'type':'extract', 'name': name}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
+            response = _requests.post(f'{_config.api_host}/model/content', params={'type':'extract', 'name': name}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
         elif model_id:
-            response = _requests.put(f'{_config.api_host}/user/model/train', params={'type':'extract', 'model_id': model_id}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
+            response = _requests.put(f'{_config.api_host}/model/content', params={'type':'extract', 'model_id': model_id}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
         else:
             raise ValueError('Either a name or a model id must be provided')
 
         return response
 
     def standardize(training_data: list, name: str = None, model_id: str = None):
         """
@@ -86,14 +86,14 @@
             # checking the first element in training list
             if training_data[0] != ['Find', 'Replace', 'Notes']:
                 training_data = [['Find', 'Replace', 'Notes']] + training_data
         else:
             raise ValueError('A list is expected for training_data')
         
         if name:
-            response = _requests.post(f'{_config.api_host}/data/user/model/train', params={'type':'standardize', 'name': name}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
+            response = _requests.post(f'{_config.api_host}/model/content', params={'type':'standardize', 'name': name}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
         elif model_id:
-            response = _requests.put(f'{_config.api_host}/user/model/train', params={'type':'standardize', 'model_id': model_id}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
+            response = _requests.put(f'{_config.api_host}/model/content', params={'type':'standardize', 'model_id': model_id}, headers={'Authorization': f'Bearer {_auth.get_access_token()}'}, json=training_data)
         else:
             raise ValueError('Either a name or a model id must be provided')
 
         return response
```

### Comparing `wrangles-1.2.1/wrangles/translate.py` & `wrangles-1.3.0/wrangles/translate.py`

 * *Files identical despite different names*

