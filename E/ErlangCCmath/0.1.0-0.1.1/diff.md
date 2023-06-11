# Comparing `tmp/ErlangCCmath-0.1.0.tar.gz` & `tmp/ErlangCCmath-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ErlangCCmath-0.1.0.tar", last modified: Wed May 31 13:57:33 2023, max compression
+gzip compressed data, was "ErlangCCmath-0.1.1.tar", last modified: Sun Jun 11 20:50:44 2023, max compression
```

## Comparing `ErlangCCmath-0.1.0.tar` & `ErlangCCmath-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 berkanarik   (501) staff       (20)        0 2023-05-31 13:57:33.812469 ErlangCCmath-0.1.0/
-drwxr-xr-x   0 berkanarik   (501) staff       (20)        0 2023-05-31 13:57:33.807979 ErlangCCmath-0.1.0/ERLANG/
--rw-r--r--   0 berkanarik   (501) staff       (20)     9329 2023-03-16 10:23:13.000000 ErlangCCmath-0.1.0/ERLANG/BL.py
--rw-r--r--   0 berkanarik   (501) staff       (20)    18435 2023-03-16 10:23:22.000000 ErlangCCmath-0.1.0/ERLANG/CHAT.py
--rw-r--r--   0 berkanarik   (501) staff       (20)    29359 2023-04-12 12:25:10.000000 ErlangCCmath-0.1.0/ERLANG/X.py
--rw-r--r--   0 berkanarik   (501) staff       (20)      287 2023-03-16 10:22:59.000000 ErlangCCmath-0.1.0/ERLANG/__init__.py
--rw-r--r--   0 berkanarik   (501) staff       (20)     2499 2023-03-16 14:06:56.000000 ErlangCCmath-0.1.0/ERLANG/settings.py
-drwxr-xr-x   0 berkanarik   (501) staff       (20)        0 2023-05-31 13:57:33.810668 ErlangCCmath-0.1.0/ErlangCCmath.egg-info/
--rw-r--r--   0 berkanarik   (501) staff       (20)     1701 2023-05-31 13:57:33.000000 ErlangCCmath-0.1.0/ErlangCCmath.egg-info/PKG-INFO
--rw-r--r--   0 berkanarik   (501) staff       (20)      288 2023-05-31 13:57:33.000000 ErlangCCmath-0.1.0/ErlangCCmath.egg-info/SOURCES.txt
--rw-r--r--   0 berkanarik   (501) staff       (20)        1 2023-05-31 13:57:33.000000 ErlangCCmath-0.1.0/ErlangCCmath.egg-info/dependency_links.txt
--rw-r--r--   0 berkanarik   (501) staff       (20)       18 2023-05-31 13:57:33.000000 ErlangCCmath-0.1.0/ErlangCCmath.egg-info/requires.txt
--rw-r--r--   0 berkanarik   (501) staff       (20)        7 2023-05-31 13:57:33.000000 ErlangCCmath-0.1.0/ErlangCCmath.egg-info/top_level.txt
--rw-r--r--   0 berkanarik   (501) staff       (20)     1049 2022-12-25 11:34:34.000000 ErlangCCmath-0.1.0/LICENSE.txt
--rw-r--r--   0 berkanarik   (501) staff       (20)     1701 2023-05-31 13:57:33.811711 ErlangCCmath-0.1.0/PKG-INFO
--rw-r--r--   0 berkanarik   (501) staff       (20)      837 2023-05-31 13:56:23.000000 ErlangCCmath-0.1.0/README.txt
--rw-r--r--   0 berkanarik   (501) staff       (20)       38 2023-05-31 13:57:33.812726 ErlangCCmath-0.1.0/setup.cfg
--rw-r--r--   0 berkanarik   (501) staff       (20)     1367 2023-05-31 13:57:15.000000 ErlangCCmath-0.1.0/setup.py
+drwxr-xr-x   0 berkanarik   (501) staff       (20)        0 2023-06-11 20:50:44.150820 ErlangCCmath-0.1.1/
+drwxr-xr-x   0 berkanarik   (501) staff       (20)        0 2023-06-11 20:50:44.147279 ErlangCCmath-0.1.1/ERLANG/
+-rw-r--r--   0 berkanarik   (501) staff       (20)     9329 2023-03-16 10:23:13.000000 ErlangCCmath-0.1.1/ERLANG/BL.py
+-rw-r--r--   0 berkanarik   (501) staff       (20)    18435 2023-03-16 10:23:22.000000 ErlangCCmath-0.1.1/ERLANG/CHAT.py
+-rw-r--r--   0 berkanarik   (501) staff       (20)    29359 2023-04-12 12:25:10.000000 ErlangCCmath-0.1.1/ERLANG/X.py
+-rw-r--r--   0 berkanarik   (501) staff       (20)      287 2023-03-16 10:22:59.000000 ErlangCCmath-0.1.1/ERLANG/__init__.py
+-rw-r--r--   0 berkanarik   (501) staff       (20)     2499 2023-03-16 14:06:56.000000 ErlangCCmath-0.1.1/ERLANG/settings.py
+drwxr-xr-x   0 berkanarik   (501) staff       (20)        0 2023-06-11 20:50:44.149848 ErlangCCmath-0.1.1/ErlangCCmath.egg-info/
+-rw-r--r--   0 berkanarik   (501) staff       (20)     1687 2023-06-11 20:50:44.000000 ErlangCCmath-0.1.1/ErlangCCmath.egg-info/PKG-INFO
+-rw-r--r--   0 berkanarik   (501) staff       (20)      288 2023-06-11 20:50:44.000000 ErlangCCmath-0.1.1/ErlangCCmath.egg-info/SOURCES.txt
+-rw-r--r--   0 berkanarik   (501) staff       (20)        1 2023-06-11 20:50:44.000000 ErlangCCmath-0.1.1/ErlangCCmath.egg-info/dependency_links.txt
+-rw-r--r--   0 berkanarik   (501) staff       (20)       18 2023-06-11 20:50:44.000000 ErlangCCmath-0.1.1/ErlangCCmath.egg-info/requires.txt
+-rw-r--r--   0 berkanarik   (501) staff       (20)        7 2023-06-11 20:50:44.000000 ErlangCCmath-0.1.1/ErlangCCmath.egg-info/top_level.txt
+-rw-r--r--   0 berkanarik   (501) staff       (20)     1049 2022-12-25 11:34:34.000000 ErlangCCmath-0.1.1/LICENSE.txt
+-rw-r--r--   0 berkanarik   (501) staff       (20)     1687 2023-06-11 20:50:44.150455 ErlangCCmath-0.1.1/PKG-INFO
+-rw-r--r--   0 berkanarik   (501) staff       (20)      823 2023-06-11 20:50:18.000000 ErlangCCmath-0.1.1/README.txt
+-rw-r--r--   0 berkanarik   (501) staff       (20)       38 2023-06-11 20:50:44.150940 ErlangCCmath-0.1.1/setup.cfg
+-rw-r--r--   0 berkanarik   (501) staff       (20)     1367 2023-06-11 20:50:02.000000 ErlangCCmath-0.1.1/setup.py
```

### Comparing `ErlangCCmath-0.1.0/ERLANG/BL.py` & `ErlangCCmath-0.1.1/ERLANG/BL.py`

 * *Files identical despite different names*

### Comparing `ErlangCCmath-0.1.0/ERLANG/CHAT.py` & `ErlangCCmath-0.1.1/ERLANG/CHAT.py`

 * *Files identical despite different names*

### Comparing `ErlangCCmath-0.1.0/ERLANG/X.py` & `ErlangCCmath-0.1.1/ERLANG/X.py`

 * *Files identical despite different names*

### Comparing `ErlangCCmath-0.1.0/ERLANG/settings.py` & `ErlangCCmath-0.1.1/ERLANG/settings.py`

 * *Files identical despite different names*

### Comparing `ErlangCCmath-0.1.0/ErlangCCmath.egg-info/PKG-INFO` & `ErlangCCmath-0.1.1/ErlangCCmath.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ErlangCCmath
-Version: 0.1.0
+Version: 0.1.1
 Summary: Erlang C, X, and Chat Functions for Python
 Home-page: https://github.com/ccmath/erlang/Erlang_Python
 Author: K. Berkan Arik
 Author-email: berkan@ccmath.com
 License: MIT
 Keywords: erlang,erlang c,erlang x,erlang chat
 Classifier: Development Status :: 3 - Alpha
@@ -37,11 +37,11 @@
 SOME PRELIMINARY STEPS:
 =============================================================================
 
 Please install the ErlangCCmath package by following steps:
 
 1- Open the terminal
 
-2- Write following command: " pip install ErlangCCmath==0.1.0 "
-or " pip3 install ErlangCCmath==0.1.0 " depending on your python version/directory and latest version of the package.
+2- Write following command: " pip install ErlangCCmath "
+or " pip3 install ErlangCCmath " depending on your python version/directory and latest version of the package.
 
 3- Import the package by typing "import ERLANG" in your python script.
```

### Comparing `ErlangCCmath-0.1.0/LICENSE.txt` & `ErlangCCmath-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ErlangCCmath-0.1.0/PKG-INFO` & `ErlangCCmath-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ErlangCCmath
-Version: 0.1.0
+Version: 0.1.1
 Summary: Erlang C, X, and Chat Functions for Python
 Home-page: https://github.com/ccmath/erlang/Erlang_Python
 Author: K. Berkan Arik
 Author-email: berkan@ccmath.com
 License: MIT
 Keywords: erlang,erlang c,erlang x,erlang chat
 Classifier: Development Status :: 3 - Alpha
@@ -37,11 +37,11 @@
 SOME PRELIMINARY STEPS:
 =============================================================================
 
 Please install the ErlangCCmath package by following steps:
 
 1- Open the terminal
 
-2- Write following command: " pip install ErlangCCmath==0.1.0 "
-or " pip3 install ErlangCCmath==0.1.0 " depending on your python version/directory and latest version of the package.
+2- Write following command: " pip install ErlangCCmath "
+or " pip3 install ErlangCCmath " depending on your python version/directory and latest version of the package.
 
 3- Import the package by typing "import ERLANG" in your python script.
```

### Comparing `ErlangCCmath-0.1.0/setup.py` & `ErlangCCmath-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     ]
   
 # calling the setup function 
 setup(name='ErlangCCmath',
-      version='0.1.0',
+      version='0.1.1',
       license='MIT',
       description='Erlang C, X, and Chat Functions for Python',
       url='https://github.com/ccmath/erlang/Erlang_Python',
       author='K. Berkan Arik',
       author_email='berkan@ccmath.com',
       packages=find_packages(),
       classifiers=CLASSIFIERS,
```

