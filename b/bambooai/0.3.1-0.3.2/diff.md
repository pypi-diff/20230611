# Comparing `tmp/bambooai-0.3.1.tar.gz` & `tmp/bambooai-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.3.1.tar", last modified: Sun Jun 11 02:17:41 2023, max compression
+gzip compressed data, was "bambooai-0.3.2.tar", last modified: Sun Jun 11 02:42:05 2023, max compression
```

## Comparing `bambooai-0.3.1.tar` & `bambooai-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 02:17:41.681735 bambooai-0.3.1/
--rw-rw-rw-   0        0        0     8017 2023-06-11 02:17:41.680504 bambooai-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     7483 2023-06-11 02:09:10.000000 bambooai-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 02:17:41.643658 bambooai-0.3.1/bambooai/
--rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.3.1/bambooai/__init__.py
--rw-rw-rw-   0        0        0    25060 2023-06-11 01:47:27.000000 bambooai-0.3.1/bambooai/bambooai.py
--rw-rw-rw-   0        0        0     8600 2023-06-11 00:55:58.000000 bambooai-0.3.1/bambooai/prompts.py
-drwxrwxrwx   0        0        0        0 2023-06-11 02:17:41.678220 bambooai-0.3.1/bambooai.egg-info/
--rw-rw-rw-   0        0        0     8017 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 02:17:41.000000 bambooai-0.3.1/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 02:17:41.681870 bambooai-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-06-11 02:10:15.000000 bambooai-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 02:42:05.006149 bambooai-0.3.2/
+-rw-rw-rw-   0        0        0     8017 2023-06-11 02:42:05.005149 bambooai-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7483 2023-06-11 02:09:10.000000 bambooai-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 02:42:04.973152 bambooai-0.3.2/bambooai/
+-rw-rw-rw-   0        0        0       61 2023-06-11 02:37:51.000000 bambooai-0.3.2/bambooai/__init__.py
+-rw-rw-rw-   0        0        0    25060 2023-06-11 02:38:22.000000 bambooai-0.3.2/bambooai/bambooai.py
+-rw-rw-rw-   0        0        0     8600 2023-06-11 00:55:58.000000 bambooai-0.3.2/bambooai/prompts.py
+drwxrwxrwx   0        0        0        0 2023-06-11 02:42:05.004199 bambooai-0.3.2/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     8017 2023-06-11 02:42:04.000000 bambooai-0.3.2/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-06-11 02:42:04.000000 bambooai-0.3.2/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 02:42:04.000000 bambooai-0.3.2/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-11 02:42:04.000000 bambooai-0.3.2/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 02:42:04.000000 bambooai-0.3.2/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 02:42:05.006149 bambooai-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-06-11 02:40:09.000000 bambooai-0.3.2/setup.py
```

### Comparing `bambooai-0.3.1/PKG-INFO` & `bambooai-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.3.1
+Version: 0.3.2
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bambooai-0.3.1/README.md` & `bambooai-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bambooai-0.3.1/bambooai/bambooai.py` & `bambooai-0.3.2/bambooai/bambooai.py`

 * *Files identical despite different names*

### Comparing `bambooai-0.3.1/bambooai/prompts.py` & `bambooai-0.3.2/bambooai/prompts.py`

 * *Files identical despite different names*

### Comparing `bambooai-0.3.1/bambooai.egg-info/PKG-INFO` & `bambooai-0.3.2/bambooai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.3.1
+Version: 0.3.2
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bambooai-0.3.1/setup.py` & `bambooai-0.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='bambooai',
-    version='0.3.1',
+    version='0.3.2',
     description='A lightweight library for working with pandas dataframes using natural language queries',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Palo Galko',
     packages=find_packages(),
     install_requires=[
         'openai',
```

