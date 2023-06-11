# Comparing `tmp/bumbo_lera-0.0.1.tar.gz` & `tmp/bumbo_lera-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bumbo_lera-0.0.1.tar", last modified: Sun Jun 11 06:16:35 2023, max compression
+gzip compressed data, was "dist\bumbo_lera-0.0.2.tar", last modified: Sun Jun 11 07:02:11 2023, max compression
```

## Comparing `bumbo_lera-0.0.1.tar` & `bumbo_lera-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 06:16:35.000000 bumbo_lera-0.0.1/
--rw-rw-rw-   0        0        0      433 2023-06-11 06:16:35.000000 bumbo_lera-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 06:16:35.000000 bumbo_lera-0.0.1/bumbo/
--rw-rw-rw-   0        0        0        0 2023-06-10 22:28:18.000000 bumbo_lera-0.0.1/bumbo/__init__.py
--rw-rw-rw-   0        0        0     3896 2023-06-11 05:57:07.000000 bumbo_lera-0.0.1/bumbo/api.py
--rw-rw-rw-   0        0        0      702 2023-06-10 19:19:26.000000 bumbo_lera-0.0.1/bumbo/middleware.py
--rw-rw-rw-   0        0        0      990 2023-06-10 21:52:51.000000 bumbo_lera-0.0.1/bumbo/response.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:16:35.000000 bumbo_lera-0.0.1/bumbo_lera.egg-info/
--rw-rw-rw-   0        0        0      433 2023-06-11 06:16:34.000000 bumbo_lera-0.0.1/bumbo_lera.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-11 06:16:34.000000 bumbo_lera-0.0.1/bumbo_lera.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 06:16:34.000000 bumbo_lera-0.0.1/bumbo_lera.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-06-11 06:16:34.000000 bumbo_lera-0.0.1/bumbo_lera.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-11 06:16:34.000000 bumbo_lera-0.0.1/bumbo_lera.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 06:16:35.000000 bumbo_lera-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1872 2023-06-11 06:03:22.000000 bumbo_lera-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/
+-rw-rw-rw-   0        0        0      433 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/bumbo/
+-rw-rw-rw-   0        0        0        0 2023-06-10 22:28:18.000000 bumbo_lera-0.0.2/bumbo/__init__.py
+-rw-rw-rw-   0        0        0     3896 2023-06-11 05:57:07.000000 bumbo_lera-0.0.2/bumbo/api.py
+-rw-rw-rw-   0        0        0      702 2023-06-10 19:19:26.000000 bumbo_lera-0.0.2/bumbo/middleware.py
+-rw-rw-rw-   0        0        0      990 2023-06-10 21:52:51.000000 bumbo_lera-0.0.2/bumbo/response.py
+drwxrwxrwx   0        0        0        0 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/bumbo_lera.egg-info/
+-rw-rw-rw-   0        0        0      433 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/bumbo_lera.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/bumbo_lera.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/bumbo_lera.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/bumbo_lera.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/bumbo_lera.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 07:02:11.000000 bumbo_lera-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2023-06-11 07:00:48.000000 bumbo_lera-0.0.2/setup.py
```

### Comparing `bumbo_lera-0.0.1/bumbo/api.py` & `bumbo_lera-0.0.2/bumbo/api.py`

 * *Files identical despite different names*

### Comparing `bumbo_lera-0.0.1/bumbo/middleware.py` & `bumbo_lera-0.0.2/bumbo/middleware.py`

 * *Files identical despite different names*

### Comparing `bumbo_lera-0.0.1/bumbo/response.py` & `bumbo_lera-0.0.2/bumbo/response.py`

 * *Files identical despite different names*

### Comparing `bumbo_lera-0.0.1/setup.py` & `bumbo_lera-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "bumbo_lera"
 DESCRIPTION = "Bumbo Python Web Framework built for learning purposes."
 EMAIL = "barsukova_valeria@mail.com"
 AUTHOR = "Valeria Barsukova"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==2.10.3",
     "parse==1.12.1",
     "requests==2.22.0",
     "requests-wsgi-adapter==0.4.1",
```

