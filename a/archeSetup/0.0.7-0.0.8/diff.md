# Comparing `tmp/archeSetup-0.0.7.tar.gz` & `tmp/archeSetup-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archeSetup-0.0.7.tar", last modified: Sun Jun 11 15:19:57 2023, max compression
+gzip compressed data, was "archeSetup-0.0.8.tar", last modified: Sun Jun 11 15:28:18 2023, max compression
```

## Comparing `archeSetup-0.0.7.tar` & `archeSetup-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 15:19:57.510568 archeSetup-0.0.7/
--rw-rw-rw-   0        0        0      174 2023-06-11 15:17:30.000000 archeSetup-0.0.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1156 2023-06-11 15:19:57.510568 archeSetup-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-11 15:09:08.000000 archeSetup-0.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 15:19:57.502567 archeSetup-0.0.7/archeSetup/
--rw-rw-rw-   0        0        0      281 2023-06-11 15:14:26.000000 archeSetup-0.0.7/archeSetup/__init__.py
--rw-rw-rw-   0        0        0     2569 2023-06-11 14:52:58.000000 archeSetup-0.0.7/archeSetup/browse_file.py
--rw-rw-rw-   0        0        0     4346 2023-06-11 15:05:20.000000 archeSetup-0.0.7/archeSetup/data_conversion.py
--rw-rw-rw-   0        0        0     2474 2023-06-11 14:43:24.000000 archeSetup-0.0.7/archeSetup/initApp.py
-drwxrwxrwx   0        0        0        0 2023-06-11 15:19:57.509567 archeSetup-0.0.7/archeSetup.egg-info/
--rw-rw-rw-   0        0        0     1156 2023-06-11 15:19:57.000000 archeSetup-0.0.7/archeSetup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-11 15:19:57.000000 archeSetup-0.0.7/archeSetup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 15:19:57.000000 archeSetup-0.0.7/archeSetup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 15:19:57.000000 archeSetup-0.0.7/archeSetup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 15:19:57.510568 archeSetup-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-06-11 15:19:52.000000 archeSetup-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:28:18.946081 archeSetup-0.0.8/
+-rw-rw-rw-   0        0        0      174 2023-06-11 15:17:30.000000 archeSetup-0.0.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1156 2023-06-11 15:28:18.945080 archeSetup-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-11 15:09:08.000000 archeSetup-0.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 15:28:18.938078 archeSetup-0.0.8/archeSetup/
+-rw-rw-rw-   0        0        0      281 2023-06-11 15:14:26.000000 archeSetup-0.0.8/archeSetup/__init__.py
+-rw-rw-rw-   0        0        0     2569 2023-06-11 14:52:58.000000 archeSetup-0.0.8/archeSetup/browse_file.py
+-rw-rw-rw-   0        0        0     4346 2023-06-11 15:05:20.000000 archeSetup-0.0.8/archeSetup/data_conversion.py
+-rw-rw-rw-   0        0        0     2480 2023-06-11 15:26:48.000000 archeSetup-0.0.8/archeSetup/initApp.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:28:18.945080 archeSetup-0.0.8/archeSetup.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-06-11 15:28:18.000000 archeSetup-0.0.8/archeSetup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-11 15:28:18.000000 archeSetup-0.0.8/archeSetup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 15:28:18.000000 archeSetup-0.0.8/archeSetup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 15:28:18.000000 archeSetup-0.0.8/archeSetup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 15:28:18.946081 archeSetup-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      777 2023-06-11 15:28:06.000000 archeSetup-0.0.8/setup.py
```

### Comparing `archeSetup-0.0.7/LICENSE.txt` & `archeSetup-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.7/PKG-INFO` & `archeSetup-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the  initialisation of the application and it will be use as check.
         This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files
```

### Comparing `archeSetup-0.0.7/archeSetup/browse_file.py` & `archeSetup-0.0.8/archeSetup/browse_file.py`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.7/archeSetup/data_conversion.py` & `archeSetup-0.0.8/archeSetup/data_conversion.py`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.7/archeSetup/initApp.py` & `archeSetup-0.0.8/archeSetup/initApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import urllib.request as req
 from datetime import datetime, timedelta
-from browse_file import *
+# from browse_file import *
 
 def connect():
     try:
         with  req.urlopen('http://just-the-time.appspot.com/') as response:
             data = response.read()
         return data
     except:
@@ -105,9 +105,9 @@
         return val_pass
     else:
         val_pass = False
         return val_pass
   
 
 ## TESTING
-ouput =checking3(1233)
-print("the license ouput:", ouput)
+# ouput =checking3(1233)
+# print("the license ouput:", ouput)
```

### Comparing `archeSetup-0.0.7/archeSetup.egg-info/PKG-INFO` & `archeSetup-0.0.8/archeSetup.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the  initialisation of the application and it will be use as check.
         This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files
```

### Comparing `archeSetup-0.0.7/setup.py` & `archeSetup-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 ]
 
 setup(
 
 name = 'archeSetup',
-version='0.0.7',
+version='0.0.8',
 description='This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files',
 long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
 url='',
 author='Arche',
 author_email='rkdyava@gmail.com',
 classifiers=classifiers,
 keywords='Setup',
```

