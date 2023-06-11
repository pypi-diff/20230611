# Comparing `tmp/PyTableWiz-0.0.2.tar.gz` & `tmp/PyTableWiz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTableWiz-0.0.2.tar", last modified: Sat Jun 10 12:18:22 2023, max compression
+gzip compressed data, was "PyTableWiz-0.0.3.tar", last modified: Sun Jun 11 11:34:18 2023, max compression
```

## Comparing `PyTableWiz-0.0.2.tar` & `PyTableWiz-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:18:22.362879 PyTableWiz-0.0.2/
--rw-rw-rw-   0        0        0     1093 2023-06-10 05:07:14.000000 PyTableWiz-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2217 2023-06-10 12:18:22.360885 PyTableWiz-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 12:18:22.331962 PyTableWiz-0.0.2/PyTableWiz/
--rw-rw-rw-   0        0        0     7296 2023-06-07 05:47:51.000000 PyTableWiz-0.0.2/PyTableWiz/PythonTableWizard.py
--rw-rw-rw-   0        0        0        0 2023-06-10 05:36:12.000000 PyTableWiz-0.0.2/PyTableWiz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:18:22.357896 PyTableWiz-0.0.2/PyTableWiz.egg-info/
--rw-rw-rw-   0        0        0     2217 2023-06-10 12:18:22.000000 PyTableWiz-0.0.2/PyTableWiz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-10 12:18:22.000000 PyTableWiz-0.0.2/PyTableWiz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:18:22.000000 PyTableWiz-0.0.2/PyTableWiz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-10 12:18:22.000000 PyTableWiz-0.0.2/PyTableWiz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1721 2023-06-10 11:24:05.000000 PyTableWiz-0.0.2/README.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:18:22.362879 PyTableWiz-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-10 12:18:10.000000 PyTableWiz-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:34:18.595538 PyTableWiz-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2023-06-10 05:07:14.000000 PyTableWiz-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2199 2023-06-11 11:34:18.594541 PyTableWiz-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 11:34:18.574769 PyTableWiz-0.0.3/PyTableWiz/
+-rw-rw-rw-   0        0        0     7296 2023-06-07 05:47:51.000000 PyTableWiz-0.0.3/PyTableWiz/PythonTableWizard.py
+-rw-rw-rw-   0        0        0       32 2023-06-11 11:30:39.000000 PyTableWiz-0.0.3/PyTableWiz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:34:18.591545 PyTableWiz-0.0.3/PyTableWiz.egg-info/
+-rw-rw-rw-   0        0        0     2199 2023-06-11 11:34:18.000000 PyTableWiz-0.0.3/PyTableWiz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-06-11 11:34:18.000000 PyTableWiz-0.0.3/PyTableWiz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 11:34:18.000000 PyTableWiz-0.0.3/PyTableWiz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 11:34:18.000000 PyTableWiz-0.0.3/PyTableWiz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1704 2023-06-11 11:31:05.000000 PyTableWiz-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 11:34:18.595538 PyTableWiz-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-06-11 11:34:05.000000 PyTableWiz-0.0.3/setup.py
```

### Comparing `PyTableWiz-0.0.2/LICENSE.txt` & `PyTableWiz-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTableWiz-0.0.2/PKG-INFO` & `PyTableWiz-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTableWiz
-Version: 0.0.2
+Version: 0.0.3
 Summary: Creating tables for CSV data file
 Home-page: https://github.com/PramudithRangana/Table-Wizard.git
 Author: Pramudith Rangana
 Author-email: pramudithrangana@gmail.com
 License: MIT
 Keywords: CSV,table
 Classifier: Operating System :: Microsoft :: Windows
@@ -14,15 +14,15 @@
 License-File: LICENSE.txt
 
 # Table Creating for CSV Data File.
 
 - To run this program, it's need to call the class as follows.
 
 ```python
-from PyTableWiz.PythonTableWizard import TableWizard
+from PyTableWiz import TableWizard
 
 TableWizard("src/My filepath/to/datafile.csv")
 ```
 - Here take the file path of the data file which you need to create a table.
 - You can customize how many rows need to be belongs to the table by using *__limit__*  key word as an argument to provide a limitation. It will be get 100 rows by default.
 
 	E.g:
```

### Comparing `PyTableWiz-0.0.2/PyTableWiz/PythonTableWizard.py` & `PyTableWiz-0.0.3/PyTableWiz/PythonTableWizard.py`

 * *Files identical despite different names*

### Comparing `PyTableWiz-0.0.2/PyTableWiz.egg-info/PKG-INFO` & `PyTableWiz-0.0.3/PyTableWiz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTableWiz
-Version: 0.0.2
+Version: 0.0.3
 Summary: Creating tables for CSV data file
 Home-page: https://github.com/PramudithRangana/Table-Wizard.git
 Author: Pramudith Rangana
 Author-email: pramudithrangana@gmail.com
 License: MIT
 Keywords: CSV,table
 Classifier: Operating System :: Microsoft :: Windows
@@ -14,15 +14,15 @@
 License-File: LICENSE.txt
 
 # Table Creating for CSV Data File.
 
 - To run this program, it's need to call the class as follows.
 
 ```python
-from PyTableWiz.PythonTableWizard import TableWizard
+from PyTableWiz import TableWizard
 
 TableWizard("src/My filepath/to/datafile.csv")
 ```
 - Here take the file path of the data file which you need to create a table.
 - You can customize how many rows need to be belongs to the table by using *__limit__*  key word as an argument to provide a limitation. It will be get 100 rows by default.
 
 	E.g:
```

### Comparing `PyTableWiz-0.0.2/README.txt` & `PyTableWiz-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Table Creating for CSV Data File
+# Table Creating for CSV Data File.
 
 - To run this program, it's need to call the class as follows.
 
 ```python
-from PyTableWiz.PythonTableWizard import TableWizard
+from PyTableWiz import TableWizard
 
 TableWizard("src/My filepath/to/datafile.csv")
 ```
 - Here take the file path of the data file which you need to create a table.
 - You can customize how many rows need to be belongs to the table by using *__limit__*  key word as an argument to provide a limitation. It will be get 100 rows by default.
 
 	E.g:
```

### Comparing `PyTableWiz-0.0.2/setup.py` & `PyTableWiz-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
   'Operating System :: Microsoft :: Windows',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 with open("README.md", "r") as f:
   long_description = f.read()
- 
+
 setup(
   name='PyTableWiz',
-  version='0.0.2',
+  version='0.0.3',
   description='Creating tables for CSV data file',
   long_description=long_description,
   long_description_content_type = "text/markdown",
   url='https://github.com/PramudithRangana/Table-Wizard.git',
   author='Pramudith Rangana',
   author_email='pramudithrangana@gmail.com',
   license='MIT',
```

