# Comparing `tmp/needed-libs-0.6.tar.gz` & `tmp/needed-libs-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "needed-libs-0.6.tar", last modified: Sat Jun 10 19:07:55 2023, max compression
+gzip compressed data, was "needed-libs-0.7.tar", last modified: Sun Jun 11 13:06:20 2023, max compression
```

## Comparing `needed-libs-0.6.tar` & `needed-libs-0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 19:07:55.283009 needed-libs-0.6/
--rw-rw-rw-   0        0        0       56 2023-06-10 19:07:55.283009 needed-libs-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 19:07:55.278012 needed-libs-0.6/needed_libs/
--rw-rw-rw-   0        0        0        0 2023-06-10 18:56:07.000000 needed-libs-0.6/needed_libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 19:07:55.282009 needed-libs-0.6/needed_libs.egg-info/
--rw-rw-rw-   0        0        0       56 2023-06-10 19:07:54.000000 needed-libs-0.6/needed_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-10 19:07:55.000000 needed-libs-0.6/needed_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 19:07:54.000000 needed-libs-0.6/needed_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2023-06-10 19:07:54.000000 needed-libs-0.6/needed_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-10 19:07:54.000000 needed-libs-0.6/needed_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-10 19:07:55.284008 needed-libs-0.6/setup.cfg
--rw-rw-rw-   0        0        0      955 2023-06-10 19:07:47.000000 needed-libs-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:06:20.604233 needed-libs-0.7/
+-rw-rw-rw-   0        0        0       56 2023-06-11 13:06:20.604233 needed-libs-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 13:06:20.599237 needed-libs-0.7/needed_libs/
+-rw-rw-rw-   0        0        0        0 2023-06-10 18:56:07.000000 needed-libs-0.7/needed_libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:06:20.603234 needed-libs-0.7/needed_libs.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      339 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-11 13:06:20.604233 needed-libs-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      920 2023-06-11 13:06:14.000000 needed-libs-0.7/setup.py
```

### Comparing `needed-libs-0.6/setup.py` & `needed-libs-0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name = 'needed-libs',
     packages = ['needed_libs'],
-    version = '0.6',
+    version = '0.7',
     install_requires = [
         # cc
         'websocket-client',
         'python_ghost_cursor',
         'price_parser',
         'requests',
 
@@ -23,15 +23,14 @@
         'moviepy',
         'telethon',
 
         # Scraping
         'bs4',
         'httpx',
         'selenium-shortcuts',
-        'undetected-chromedriver',
         'requestium',
         'feedparser',
 
         # Google
         'gspread',
         'google-api-python-client',
         'google-auth-httplib2',
```

