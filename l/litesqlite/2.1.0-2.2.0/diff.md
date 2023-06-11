# Comparing `tmp/litesqlite-2.1.0.tar.gz` & `tmp/litesqlite-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.1.0.tar", last modified: Sun Jun 11 15:54:01 2023, max compression
+gzip compressed data, was "litesqlite-2.2.0.tar", last modified: Sun Jun 11 17:10:04 2023, max compression
```

## Comparing `litesqlite-2.1.0.tar` & `litesqlite-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 15:54:01.696967 litesqlite-2.1.0/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.1.0/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 15:54:01.696967 litesqlite-2.1.0/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.1.0/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 15:54:01.688967 litesqlite-2.1.0/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.1.0/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4363 2023-06-11 15:26:19.000000 litesqlite-2.1.0/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    10896 2023-06-11 15:52:53.000000 litesqlite-2.1.0/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 15:54:01.696967 litesqlite-2.1.0/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 15:54:01.000000 litesqlite-2.1.0/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-11 15:54:01.000000 litesqlite-2.1.0/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-11 15:54:01.000000 litesqlite-2.1.0/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-11 15:54:01.000000 litesqlite-2.1.0/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-11 15:54:01.000000 litesqlite-2.1.0/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-11 15:54:01.696967 litesqlite-2.1.0/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-11 15:53:56.000000 litesqlite-2.1.0/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 17:10:04.408700 litesqlite-2.2.0/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.2.0/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 17:10:04.404700 litesqlite-2.2.0/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.2.0/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 17:10:04.400699 litesqlite-2.2.0/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.2.0/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.2.0/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8418 2023-06-11 17:08:53.000000 litesqlite-2.2.0/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 17:10:04.404700 litesqlite-2.2.0/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 17:10:03.000000 litesqlite-2.2.0/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-11 17:10:03.000000 litesqlite-2.2.0/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-11 17:10:03.000000 litesqlite-2.2.0/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-11 17:10:03.000000 litesqlite-2.2.0/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-11 17:10:03.000000 litesqlite-2.2.0/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-11 17:10:04.408700 litesqlite-2.2.0/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-11 17:08:53.000000 litesqlite-2.2.0/setup.py
```

### Comparing `litesqlite-2.1.0/LICENSE` & `litesqlite-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.1.0/PKG-INFO` & `litesqlite-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.1.0
+Version: 2.2.0
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.1.0/README.md` & `litesqlite-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.1.0/litesqlite/datatypes.py` & `litesqlite-2.2.0/litesqlite/datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 class DataTypes:
 
     class Fetch:
         FETCHONE = 'fetchone'
         FETCHALL = 'fetchall'
-        FETCHMANY = 'fetchmany'
 
     class Collation:
         BINARY = 'BINARY'
         NOCASE = 'NOCASE'
         RTRIM = 'RTRIM'
         UTF16 = 'UTF16'
         UTF16CI = 'UTF16CI'
```

### Comparing `litesqlite-2.1.0/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.2.0/litesqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.1.0
+Version: 2.2.0
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.1.0/setup.py` & `litesqlite-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.1.0',
+    version='2.2.0',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

