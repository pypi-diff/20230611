# Comparing `tmp/digital_unit-1.6.0.tar.gz` & `tmp/digital_unit-1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_unit-1.6.0.tar", last modified: Sun Jun 11 06:44:17 2023, max compression
+gzip compressed data, was "digital_unit-1.6b0.tar", last modified: Sun May 28 08:18:06 2023, max compression
```

## Comparing `digital_unit-1.6.0.tar` & `digital_unit-1.6b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 06:44:17.105375 digital_unit-1.6.0/
--rw-rw-rw-   0        0        0     1668 2023-06-11 06:44:17.106375 digital_unit-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1383 2023-05-28 08:12:19.000000 digital_unit-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 06:44:17.081364 digital_unit-1.6.0/digital_unit/
--rw-rw-rw-   0        0        0     1166 2023-05-28 08:07:32.000000 digital_unit-1.6.0/digital_unit/Area.py
--rw-rw-rw-   0        0        0      925 2023-05-28 08:08:29.000000 digital_unit-1.6.0/digital_unit/Lenth.py
--rw-rw-rw-   0        0        0      570 2023-05-28 08:17:58.000000 digital_unit-1.6.0/digital_unit/Temperature.py
--rw-rw-rw-   0        0        0     1159 2023-05-28 08:06:54.000000 digital_unit-1.6.0/digital_unit/Volume.py
--rw-rw-rw-   0        0        0      175 2023-06-11 06:43:35.000000 digital_unit-1.6.0/digital_unit/__init__.py
--rw-rw-rw-   0        0        0     1115 2023-05-28 08:05:25.000000 digital_unit-1.6.0/digital_unit/root.py
--rw-rw-rw-   0        0        0      330 2023-05-28 08:11:42.000000 digital_unit-1.6.0/digital_unit/sample.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:44:17.099363 digital_unit-1.6.0/digital_unit.egg-info/
--rw-rw-rw-   0        0        0     1668 2023-06-11 06:44:16.000000 digital_unit-1.6.0/digital_unit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-06-11 06:44:16.000000 digital_unit-1.6.0/digital_unit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 06:44:16.000000 digital_unit-1.6.0/digital_unit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-11 06:44:16.000000 digital_unit-1.6.0/digital_unit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-11 06:44:17.109363 digital_unit-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-06-11 06:43:20.000000 digital_unit-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.072172 digital_unit-1.6b0/
+-rw-rw-rw-   0        0        0     1668 2023-05-28 08:18:06.072172 digital_unit-1.6b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1383 2023-05-28 08:12:19.000000 digital_unit-1.6b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.054184 digital_unit-1.6b0/digital_unit/
+-rw-rw-rw-   0        0        0     1166 2023-05-28 08:07:32.000000 digital_unit-1.6b0/digital_unit/Area.py
+-rw-rw-rw-   0        0        0      925 2023-05-28 08:08:29.000000 digital_unit-1.6b0/digital_unit/Lenth.py
+-rw-rw-rw-   0        0        0      570 2023-05-28 08:17:58.000000 digital_unit-1.6b0/digital_unit/Temperature.py
+-rw-rw-rw-   0        0        0     1159 2023-05-28 08:06:54.000000 digital_unit-1.6b0/digital_unit/Volume.py
+-rw-rw-rw-   0        0        0      209 2023-05-28 07:44:32.000000 digital_unit-1.6b0/digital_unit/__init__.py
+-rw-rw-rw-   0        0        0     1115 2023-05-28 08:05:25.000000 digital_unit-1.6b0/digital_unit/root.py
+-rw-rw-rw-   0        0        0      330 2023-05-28 08:11:42.000000 digital_unit-1.6b0/digital_unit/sample.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.068171 digital_unit-1.6b0/digital_unit.egg-info/
+-rw-rw-rw-   0        0        0     1668 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-28 08:18:06.074171 digital_unit-1.6b0/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-05-28 08:09:55.000000 digital_unit-1.6b0/setup.py
```

### Comparing `digital_unit-1.6.0/PKG-INFO` & `digital_unit-1.6b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital_unit
-Version: 1.6.0
+Version: 1.6b0
 Summary: number and units
 Author: st201109
 Author-email: st20110913@outlook.com
 License: MIT
 Keywords: SOME,MEANINGFULL,MATH
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `digital_unit-1.6.0/README.md` & `digital_unit-1.6b0/README.md`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6.0/digital_unit/Area.py` & `digital_unit-1.6b0/digital_unit/Area.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6.0/digital_unit/Lenth.py` & `digital_unit-1.6b0/digital_unit/Lenth.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6.0/digital_unit/Temperature.py` & `digital_unit-1.6b0/digital_unit/Temperature.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6.0/digital_unit/Volume.py` & `digital_unit-1.6b0/digital_unit/Volume.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6.0/digital_unit/root.py` & `digital_unit-1.6b0/digital_unit/root.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6.0/digital_unit.egg-info/PKG-INFO` & `digital_unit-1.6b0/digital_unit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-unit
-Version: 1.6.0
+Version: 1.6b0
 Summary: number and units
 Author: st201109
 Author-email: st20110913@outlook.com
 License: MIT
 Keywords: SOME,MEANINGFULL,MATH
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `digital_unit-1.6.0/setup.py` & `digital_unit-1.6b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
   name = 'digital_unit',         # How you named your package folder (MyLib)
   packages = ['digital_unit'],   # Chose the same as "name"
-  version = '1.6.0',      # Start with a small number and increase it with every change you make
+  version = '1.6b0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'number and units',   # Give a short description about your library
   author = 'st201109',                   # Type in your name
   author_email = 'st20110913@outlook.com',      # Type in your E-Mail
   
   keywords = ['SOME', 'MEANINGFULL', 'MATH'],   # Keywords that define your package best
   long_description = long_description,
```

