# Comparing `tmp/tabNamesCat-0.1.0.tar.gz` & `tmp/tabNamesCat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabNamesCat-0.1.0.tar", last modified: Fri Jun  9 12:13:10 2023, max compression
+gzip compressed data, was "tabNamesCat-0.1.1.tar", last modified: Sun Jun 11 20:27:10 2023, max compression
```

## Comparing `tabNamesCat-0.1.0.tar` & `tabNamesCat-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-09 12:13:10.641018 tabNamesCat-0.1.0/
--rw-r--r--   0 denis     (1000) denis     (1001)     1066 2023-06-09 11:36:08.000000 tabNamesCat-0.1.0/LICENSE
--rw-r--r--   0 denis     (1000) denis     (1001)      773 2023-06-09 12:13:10.641018 tabNamesCat-0.1.0/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1001)       38 2023-06-09 12:13:10.641018 tabNamesCat-0.1.0/setup.cfg
--rw-r--r--   0 denis     (1000) denis     (1001)      898 2023-06-09 12:12:07.000000 tabNamesCat-0.1.0/setup.py
-drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-09 12:13:10.641018 tabNamesCat-0.1.0/tabNamesCat/
--rw-r--r--   0 denis     (1000) denis     (1001)      196 2023-06-09 12:07:22.000000 tabNamesCat-0.1.0/tabNamesCat/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1001)     1110 2023-06-09 12:07:22.000000 tabNamesCat-0.1.0/tabNamesCat/main.py
-drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-09 12:13:10.641018 tabNamesCat-0.1.0/tabNamesCat.egg-info/
--rw-r--r--   0 denis     (1000) denis     (1001)      773 2023-06-09 12:13:10.000000 tabNamesCat-0.1.0/tabNamesCat.egg-info/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1001)      234 2023-06-09 12:13:10.000000 tabNamesCat-0.1.0/tabNamesCat.egg-info/SOURCES.txt
--rw-r--r--   0 denis     (1000) denis     (1001)        1 2023-06-09 12:13:10.000000 tabNamesCat-0.1.0/tabNamesCat.egg-info/dependency_links.txt
--rw-r--r--   0 denis     (1000) denis     (1001)       20 2023-06-09 12:13:10.000000 tabNamesCat-0.1.0/tabNamesCat.egg-info/requires.txt
--rw-r--r--   0 denis     (1000) denis     (1001)       12 2023-06-09 12:13:10.000000 tabNamesCat-0.1.0/tabNamesCat.egg-info/top_level.txt
+drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:27:10.859692 tabNamesCat-0.1.1/
+-rw-r--r--   0 denis     (1000) denis     (1001)     1066 2023-06-09 11:36:08.000000 tabNamesCat-0.1.1/LICENSE
+-rw-r--r--   0 denis     (1000) denis     (1001)      773 2023-06-11 20:27:10.859692 tabNamesCat-0.1.1/PKG-INFO
+-rw-r--r--   0 denis     (1000) denis     (1001)       38 2023-06-11 20:27:10.859692 tabNamesCat-0.1.1/setup.cfg
+-rw-r--r--   0 denis     (1000) denis     (1001)      913 2023-06-11 20:19:09.000000 tabNamesCat-0.1.1/setup.py
+drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:27:10.856358 tabNamesCat-0.1.1/tabNamesCat/
+-rw-r--r--   0 denis     (1000) denis     (1001)      221 2023-06-11 20:23:30.000000 tabNamesCat-0.1.1/tabNamesCat/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1001)     2571 2023-06-11 20:25:54.000000 tabNamesCat-0.1.1/tabNamesCat/main.py
+drwxr-xr-x   0 denis     (1000) denis     (1001)        0 2023-06-11 20:27:10.859692 tabNamesCat-0.1.1/tabNamesCat.egg-info/
+-rw-r--r--   0 denis     (1000) denis     (1001)      773 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/PKG-INFO
+-rw-r--r--   0 denis     (1000) denis     (1001)      234 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/SOURCES.txt
+-rw-r--r--   0 denis     (1000) denis     (1001)        1 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/dependency_links.txt
+-rw-r--r--   0 denis     (1000) denis     (1001)       29 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/requires.txt
+-rw-r--r--   0 denis     (1000) denis     (1001)       12 2023-06-11 20:27:10.000000 tabNamesCat-0.1.1/tabNamesCat.egg-info/top_level.txt
```

### Comparing `tabNamesCat-0.1.0/LICENSE` & `tabNamesCat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabNamesCat-0.1.0/PKG-INFO` & `tabNamesCat-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabNamesCat
-Version: 0.1.0
+Version: 0.1.1
 Summary: CategorizationTabNames
 Home-page: https://github.com/Denisalik/TabNamesCat
 Author: Denisalik
 Author-email: schgletovdenis@mail.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tabNamesCat-0.1.0/setup.py` & `tabNamesCat-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 
 setup(
     name='tabNamesCat',
-    version='0.1.0',
+    version='0.1.1',
     description='CategorizationTabNames',
     url='https://github.com/Denisalik/TabNamesCat',
     author='Denisalik',
     author_email='schgletovdenis@mail.ru',
     license='MIT',
     packages=['tabNamesCat'],
-    install_requires=['scikit-learn>=1.2.2'],
+    install_requires=['scikit-learn', 'langdetect', 'nltk'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
```

### Comparing `tabNamesCat-0.1.0/tabNamesCat.egg-info/PKG-INFO` & `tabNamesCat-0.1.1/tabNamesCat.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabNamesCat
-Version: 0.1.0
+Version: 0.1.1
 Summary: CategorizationTabNames
 Home-page: https://github.com/Denisalik/TabNamesCat
 Author: Denisalik
 Author-email: schgletovdenis@mail.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

