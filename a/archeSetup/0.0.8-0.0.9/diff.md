# Comparing `tmp/archeSetup-0.0.8.tar.gz` & `tmp/archeSetup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archeSetup-0.0.8.tar", last modified: Sun Jun 11 15:28:18 2023, max compression
+gzip compressed data, was "archeSetup-0.0.9.tar", last modified: Sun Jun 11 15:48:47 2023, max compression
```

## Comparing `archeSetup-0.0.8.tar` & `archeSetup-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 15:28:18.946081 archeSetup-0.0.8/
--rw-rw-rw-   0        0        0      174 2023-06-11 15:17:30.000000 archeSetup-0.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1156 2023-06-11 15:28:18.945080 archeSetup-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-11 15:09:08.000000 archeSetup-0.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 15:28:18.938078 archeSetup-0.0.8/archeSetup/
--rw-rw-rw-   0        0        0      281 2023-06-11 15:14:26.000000 archeSetup-0.0.8/archeSetup/__init__.py
--rw-rw-rw-   0        0        0     2569 2023-06-11 14:52:58.000000 archeSetup-0.0.8/archeSetup/browse_file.py
--rw-rw-rw-   0        0        0     4346 2023-06-11 15:05:20.000000 archeSetup-0.0.8/archeSetup/data_conversion.py
--rw-rw-rw-   0        0        0     2480 2023-06-11 15:26:48.000000 archeSetup-0.0.8/archeSetup/initApp.py
-drwxrwxrwx   0        0        0        0 2023-06-11 15:28:18.945080 archeSetup-0.0.8/archeSetup.egg-info/
--rw-rw-rw-   0        0        0     1156 2023-06-11 15:28:18.000000 archeSetup-0.0.8/archeSetup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-11 15:28:18.000000 archeSetup-0.0.8/archeSetup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 15:28:18.000000 archeSetup-0.0.8/archeSetup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 15:28:18.000000 archeSetup-0.0.8/archeSetup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 15:28:18.946081 archeSetup-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-06-11 15:28:06.000000 archeSetup-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:48:47.380488 archeSetup-0.0.9/
+-rw-rw-rw-   0        0        0      267 2023-06-11 15:48:14.000000 archeSetup-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1281 2023-06-11 15:48:47.379487 archeSetup-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-11 15:09:08.000000 archeSetup-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 15:48:47.372486 archeSetup-0.0.9/archeSetup/
+-rw-rw-rw-   0        0        0      284 2023-06-11 15:48:38.000000 archeSetup-0.0.9/archeSetup/__init__.py
+-rw-rw-rw-   0        0        0     3263 2023-06-11 15:46:47.000000 archeSetup-0.0.9/archeSetup/browse_file.py
+-rw-rw-rw-   0        0        0     4346 2023-06-11 15:05:20.000000 archeSetup-0.0.9/archeSetup/data_conversion.py
+-rw-rw-rw-   0        0        0     2480 2023-06-11 15:26:48.000000 archeSetup-0.0.9/archeSetup/initApp.py
+drwxrwxrwx   0        0        0        0 2023-06-11 15:48:47.379487 archeSetup-0.0.9/archeSetup.egg-info/
+-rw-rw-rw-   0        0        0     1281 2023-06-11 15:48:47.000000 archeSetup-0.0.9/archeSetup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-11 15:48:47.000000 archeSetup-0.0.9/archeSetup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 15:48:47.000000 archeSetup-0.0.9/archeSetup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 15:48:47.000000 archeSetup-0.0.9/archeSetup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 15:48:47.380488 archeSetup-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      777 2023-06-11 15:48:29.000000 archeSetup-0.0.9/setup.py
```

### Comparing `archeSetup-0.0.8/LICENSE.txt` & `archeSetup-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.8/PKG-INFO` & `archeSetup-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the  initialisation of the application and it will be use as check.
         This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files
@@ -16,14 +16,18 @@
         0.0.4 (20/05/2023)
         ------------------
         - 4th  Release after bug fixing
         
         0.0.7 (11/06/2023)
         ------------------
         - 7th  Release after bug fixing
+        
+        0.0.9 (11/06/2023)
+        ------------------
+        - 8th  Release after add absolute path of modules
 Keywords: Setup
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archeSetup-0.0.8/archeSetup/browse_file.py` & `archeSetup-0.0.9/archeSetup/browse_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,18 +28,46 @@
         tag = item[0].getAttribute("name")
         return tag
     
     @staticmethod
     def xml_write(path, token, xml_val):
         doc = xml.dom.minidom.parse(path)
         item = doc.getElementsByTagName(token)
-        lic = item[0].getAttribute("name")
-        return lic
+        value = item[0].getAttribute("name")
+        return value
 
     @staticmethod
+    def xml_write_tagReal(path, token, tag_val):
+
+        """
+        # token = string
+        # tag_val = float value
+    
+        """
+        doc = xml.dom.minidom.parse(path)
+        item = doc.getElementsByTagName(token)
+        value = item[0].firstChild.data =round(tag_val,5)
+        return value
+    
+
+    @staticmethod
+    def xml_write_tagString(path, token, tag_val):
+
+        """
+        # token = string
+        # tag_val = stringvalue
+    
+        """
+        doc = xml.dom.minidom.parse(path)
+        item = doc.getElementsByTagName(token)
+        value = item[0].firstChild.data =round(tag_val,5)
+        return value
+    
+    
+    @staticmethod
     def browse(file_filter):
         if file_filter == "csv":
             dlg = QtWidgets.QFileDialog()
             dlg.setNameFilters(["CSV Files (*.csv)"])
 
         elif file_filter == "log":
             dlg = QtWidgets.QFileDialog()
```

### Comparing `archeSetup-0.0.8/archeSetup/data_conversion.py` & `archeSetup-0.0.9/archeSetup/data_conversion.py`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.8/archeSetup/initApp.py` & `archeSetup-0.0.9/archeSetup/initApp.py`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.8/archeSetup.egg-info/PKG-INFO` & `archeSetup-0.0.9/archeSetup.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the  initialisation of the application and it will be use as check.
         This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files
@@ -16,14 +16,18 @@
         0.0.4 (20/05/2023)
         ------------------
         - 4th  Release after bug fixing
         
         0.0.7 (11/06/2023)
         ------------------
         - 7th  Release after bug fixing
+        
+        0.0.9 (11/06/2023)
+        ------------------
+        - 8th  Release after add absolute path of modules
 Keywords: Setup
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archeSetup-0.0.8/setup.py` & `archeSetup-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 ]
 
 setup(
 
 name = 'archeSetup',
-version='0.0.8',
+version='0.0.9',
 description='This is the setup for the basic Application library for reading the files and extract the data from the txt/lof files. Also, we can convert the data to csv files',
 long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
 url='',
 author='Arche',
 author_email='rkdyava@gmail.com',
 classifiers=classifiers,
 keywords='Setup',
```

