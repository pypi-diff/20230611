# Comparing `tmp/abhi_general-0.0.1.tar.gz` & `tmp/abhi_general-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abhi_general-0.0.1.tar", last modified: Sun Jun 11 09:02:56 2023, max compression
+gzip compressed data, was "abhi_general-0.0.11.tar", last modified: Sun Jun 11 09:04:05 2023, max compression
```

## Comparing `abhi_general-0.0.1.tar` & `abhi_general-0.0.11.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 09:02:56.123035 abhi_general-0.0.1/
--rw-rw-rw-   0        0        0      497 2023-06-11 09:02:56.122037 abhi_general-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 09:02:56.118039 abhi_general-0.0.1/abhi_general.egg-info/
--rw-rw-rw-   0        0        0      497 2023-06-11 09:02:55.000000 abhi_general-0.0.1/abhi_general.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-06-11 09:02:56.000000 abhi_general-0.0.1/abhi_general.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 09:02:55.000000 abhi_general-0.0.1/abhi_general.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-11 09:02:55.000000 abhi_general-0.0.1/abhi_general.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-11 09:02:55.000000 abhi_general-0.0.1/abhi_general.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 09:02:56.121036 abhi_general-0.0.1/abhikashyap/
--rw-rw-rw-   0        0        0       36 2023-06-11 08:58:19.000000 abhi_general-0.0.1/abhikashyap/__init__.py
--rw-rw-rw-   0        0        0       33 2023-06-11 08:57:09.000000 abhi_general-0.0.1/abhikashyap/abhi_general.py
--rw-rw-rw-   0        0        0       42 2023-06-11 09:02:56.123035 abhi_general-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-06-11 09:02:49.000000 abhi_general-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:04:05.546364 abhi_general-0.0.11/
+-rw-rw-rw-   0        0        0      498 2023-06-11 09:04:05.545365 abhi_general-0.0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 09:04:05.539365 abhi_general-0.0.11/abhi_general.egg-info/
+-rw-rw-rw-   0        0        0      498 2023-06-11 09:04:05.000000 abhi_general-0.0.11/abhi_general.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-06-11 09:04:05.000000 abhi_general-0.0.11/abhi_general.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 09:04:05.000000 abhi_general-0.0.11/abhi_general.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-11 09:04:05.000000 abhi_general-0.0.11/abhi_general.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-11 09:04:05.000000 abhi_general-0.0.11/abhi_general.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 09:04:05.544368 abhi_general-0.0.11/abhikashyap/
+-rw-rw-rw-   0        0        0       36 2023-06-11 08:58:19.000000 abhi_general-0.0.11/abhikashyap/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-06-11 08:57:09.000000 abhi_general-0.0.11/abhikashyap/abhi_general.py
+-rw-rw-rw-   0        0        0       42 2023-06-11 09:04:05.546364 abhi_general-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      778 2023-06-11 09:03:57.000000 abhi_general-0.0.11/setup.py
```

### Comparing `abhi_general-0.0.1/setup.py` & `abhi_general-0.0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.11'
 DESCRIPTION = 'Trial custom package'
 
 # Setting up
 setup(
     name="abhi_general",
     version=VERSION,
     author="abhikashyap10",
```

