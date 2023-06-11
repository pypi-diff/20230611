# Comparing `tmp/archeSetup-0.0.5.tar.gz` & `tmp/archeSetup-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archeSetup-0.0.5.tar", last modified: Sat May 20 14:14:57 2023, max compression
+gzip compressed data, was "archeSetup-0.0.7.tar", last modified: Sun Jun 11 15:19:57 2023, max compression
```

## Comparing `archeSetup-0.0.5.tar` & `archeSetup-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:14:57.421974 archeSetup-0.0.5/
--rw-rw-rw-   0        0        0       99 2023-05-20 14:12:07.000000 archeSetup-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      767 2023-05-20 14:14:57.421974 archeSetup-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       74 2023-05-20 13:47:05.000000 archeSetup-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 14:14:57.407971 archeSetup-0.0.5/archeSetup/
--rw-rw-rw-   0        0        0      221 2023-05-20 14:14:30.000000 archeSetup-0.0.5/archeSetup/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-05-20 13:47:35.000000 archeSetup-0.0.5/archeSetup/initApp.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:14:57.420974 archeSetup-0.0.5/archeSetup.egg-info/
--rw-rw-rw-   0        0        0      767 2023-05-20 14:14:57.000000 archeSetup-0.0.5/archeSetup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-20 14:14:57.000000 archeSetup-0.0.5/archeSetup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:14:57.000000 archeSetup-0.0.5/archeSetup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-20 14:14:57.000000 archeSetup-0.0.5/archeSetup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 14:14:57.422975 archeSetup-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-05-20 14:14:45.000000 archeSetup-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:19:57.510568 archeSetup-0.0.7/
+-rw-rw-rw-   0        0        0      174 2023-06-11 15:17:30.000000 archeSetup-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1156 2023-06-11 15:19:57.510568 archeSetup-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-11 15:09:08.000000 archeSetup-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 15:19:57.502567 archeSetup-0.0.7/archeSetup/
+-rw-rw-rw-   0        0        0      281 2023-06-11 15:14:26.000000 archeSetup-0.0.7/archeSetup/__init__.py
+-rw-rw-rw-   0        0        0     2569 2023-06-11 14:52:58.000000 archeSetup-0.0.7/archeSetup/browse_file.py
+-rw-rw-rw-   0        0        0     4346 2023-06-11 15:05:20.000000 archeSetup-0.0.7/archeSetup/data_conversion.py
+-rw-rw-rw-   0        0        0     2474 2023-06-11 14:43:24.000000 archeSetup-0.0.7/archeSetup/initApp.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:19:57.509567 archeSetup-0.0.7/archeSetup.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-06-11 15:19:57.000000 archeSetup-0.0.7/archeSetup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-11 15:19:57.000000 archeSetup-0.0.7/archeSetup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 15:19:57.000000 archeSetup-0.0.7/archeSetup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 15:19:57.000000 archeSetup-0.0.7/archeSetup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 15:19:57.510568 archeSetup-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      777 2023-06-11 15:19:52.000000 archeSetup-0.0.7/setup.py
```

### Comparing `archeSetup-0.0.5/LICENSE.txt` & `archeSetup-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.5/archeSetup/initApp.py` & `archeSetup-0.0.7/archeSetup/initApp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import urllib.request as req
 from datetime import datetime, timedelta
-
+from browse_file import *
 
 def connect():
     try:
         with  req.urlopen('http://just-the-time.appspot.com/') as response:
             data = response.read()
         return data
     except:
@@ -28,14 +28,15 @@
     dat = now.strftime("%d")
     mon = now.strftime("%m")
     yr = now.strftime("%Y")
 
    
     encryption_online = int((int(month) * 31*CONST) * (int(year) * 100*CONST))
     encryption_online =str(encryption_online)
+    
   
 
     if encryption_online==str(key):
         val_pass =True
         return val_pass
     else:
         val_pass = False
@@ -44,12 +45,69 @@
     ## Testing Block
     # print("the data from the link",temp)
     # print(month)
     # print(year)
     # print(key)
     # print(encryption_online)
    
+def checking2(key):
+    CONST = 2 * 3.1416 * 1000
+    data = connect()
+
+
+    temp = str(data)
+    year = temp[2:6]
+    month = temp[7:9]
+    date = temp[10:12]
+
+    now = datetime.now()
+    dt_string = now.strftime("%d%m%y")
+    dat = now.strftime("%d")
+    mon = now.strftime("%m")
+    yr = now.strftime("%Y")
+
+   
+    encryption_online = int((int(month) * 31*CONST) * (int(year) * 100*CONST))
+    encryption_online =str(encryption_online)
+  
+
+    if encryption_online==str(key):
+        val_pass =True
+        return val_pass
+    else:
+        val_pass = False
+        return val_pass
 
+def checking3(key):
+    CONST = 2 * 3.1416 * 1000
+    data = connect()
+
+
+    temp = str(data)
+    year = temp[2:6]
+    month = temp[7:9]
+    date = temp[10:12]
+
+    now = datetime.now()
+    dt_string = now.strftime("%d%m%y")
+    dat = now.strftime("%d")
+    mon = now.strftime("%m")
+    yr = now.strftime("%Y")
 
+   
+    encryption_online = int((int(date)*24)*(int(month) * 31*CONST) * (int(year) * 100*CONST))
+    encryption_online =str(encryption_online)
+    
+  ##Testing:
+    #print(encryption_online)
 
+    if encryption_online==str(key):
+        val_pass =True
+        return val_pass
+    else:
+        val_pass = False
+        return val_pass
+  
 
-# print("the license ouput:", ouput)
+## TESTING
+ouput =checking3(1233)
+print("the license ouput:", ouput)
```

### Comparing `archeSetup-0.0.5/setup.py` & `archeSetup-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 ]
 
 setup(
 
 name = 'archeSetup',
-version='0.0.5',
-description='This is the setup for the basic Application library',
+version='0.0.7',
+description='This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files',
 long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
 url='',
 author='Arche',
 author_email='rkdyava@gmail.com',
 classifiers=classifiers,
 keywords='Setup',
 packages=find_packages(),
```

