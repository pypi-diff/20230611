# Comparing `tmp/aorta_sirius-0.0.3.tar.gz` & `tmp/aorta_sirius-2023.6.11.0.18.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.0.3.tar", last modified: Sun Jun 11 00:16:00 2023, max compression
+gzip compressed data, was "aorta_sirius-2023.6.11.0.18.27.tar", last modified: Sun Jun 11 00:18:28 2023, max compression
```

## Comparing `aorta_sirius-0.0.3.tar` & `aorta_sirius-2023.6.11.0.18.27.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 00:16:00.442904 aorta_sirius-0.0.3/
--rw-rw-rw-   0        0        0      185 2023-06-11 00:16:00.441925 aorta_sirius-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-06-10 22:53:52.000000 aorta_sirius-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 00:16:00.442904 aorta_sirius-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      381 2023-06-11 00:15:57.000000 aorta_sirius-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 00:16:00.415546 aorta_sirius-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 00:16:00.437761 aorta_sirius-0.0.3/src/aorta_sirius.egg-info/
--rw-rw-rw-   0        0        0      185 2023-06-11 00:16:00.000000 aorta_sirius-0.0.3/src/aorta_sirius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-11 00:16:00.000000 aorta_sirius-0.0.3/src/aorta_sirius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 00:16:00.000000 aorta_sirius-0.0.3/src/aorta_sirius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 00:16:00.000000 aorta_sirius-0.0.3/src/aorta_sirius.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 00:16:00.439936 aorta_sirius-0.0.3/src/sirius/
--rw-rw-rw-   0        0        0       44 2023-06-10 23:07:55.000000 aorta_sirius-0.0.3/src/sirius/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 00:18:28.037719 aorta_sirius-2023.6.11.0.18.27/
+-rw-rw-rw-   0        0        0      197 2023-06-11 00:18:28.036706 aorta_sirius-2023.6.11.0.18.27/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2023-06-10 22:53:52.000000 aorta_sirius-2023.6.11.0.18.27/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 00:18:28.038642 aorta_sirius-2023.6.11.0.18.27/setup.cfg
+-rw-rw-rw-   0        0        0      430 2023-06-11 00:18:25.000000 aorta_sirius-2023.6.11.0.18.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 00:18:28.008789 aorta_sirius-2023.6.11.0.18.27/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 00:18:28.031637 aorta_sirius-2023.6.11.0.18.27/src/aorta_sirius.egg-info/
+-rw-rw-rw-   0        0        0      197 2023-06-11 00:18:27.000000 aorta_sirius-2023.6.11.0.18.27/src/aorta_sirius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-11 00:18:27.000000 aorta_sirius-2023.6.11.0.18.27/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 00:18:27.000000 aorta_sirius-2023.6.11.0.18.27/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 00:18:27.000000 aorta_sirius-2023.6.11.0.18.27/src/aorta_sirius.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 00:18:28.033649 aorta_sirius-2023.6.11.0.18.27/src/sirius/
+-rw-rw-rw-   0        0        0       48 2023-06-11 00:18:25.000000 aorta_sirius-2023.6.11.0.18.27/src/sirius/__init__.py
```

