# Comparing `tmp/aorta_sirius-0.2.tar.gz` & `tmp/aorta_sirius-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.2.tar", last modified: Sun Jun 11 03:16:07 2023, max compression
+gzip compressed data, was "aorta_sirius-0.3.tar", last modified: Sun Jun 11 03:17:35 2023, max compression
```

## Comparing `aorta_sirius-0.2.tar` & `aorta_sirius-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 03:16:07.556450 aorta_sirius-0.2/
--rw-rw-rw-   0        0        0      183 2023-06-11 03:16:07.555467 aorta_sirius-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-06-10 22:53:52.000000 aorta_sirius-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 03:16:07.557430 aorta_sirius-0.2/setup.cfg
--rw-rw-rw-   0        0        0      840 2023-06-11 03:16:05.000000 aorta_sirius-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 03:16:07.530603 aorta_sirius-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 03:16:07.552052 aorta_sirius-0.2/src/aorta_sirius.egg-info/
--rw-rw-rw-   0        0        0      183 2023-06-11 03:16:07.000000 aorta_sirius-0.2/src/aorta_sirius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-11 03:16:07.000000 aorta_sirius-0.2/src/aorta_sirius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 03:16:07.000000 aorta_sirius-0.2/src/aorta_sirius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 03:16:07.000000 aorta_sirius-0.2/src/aorta_sirius.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 03:16:07.553429 aorta_sirius-0.2/src/sirius/
--rw-rw-rw-   0        0        0        0 2023-06-11 00:20:15.000000 aorta_sirius-0.2/src/sirius/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 03:17:35.704272 aorta_sirius-0.3/
+-rw-rw-rw-   0        0        0      183 2023-06-11 03:17:35.704272 aorta_sirius-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2023-06-10 22:53:52.000000 aorta_sirius-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 03:17:35.705276 aorta_sirius-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      840 2023-06-11 03:16:05.000000 aorta_sirius-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 03:17:35.687366 aorta_sirius-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 03:17:35.700279 aorta_sirius-0.3/src/aorta_sirius.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-06-11 03:17:35.000000 aorta_sirius-0.3/src/aorta_sirius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-11 03:17:35.000000 aorta_sirius-0.3/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 03:17:35.000000 aorta_sirius-0.3/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 03:17:35.000000 aorta_sirius-0.3/src/aorta_sirius.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 03:17:35.702301 aorta_sirius-0.3/src/sirius/
+-rw-rw-rw-   0        0        0        0 2023-06-11 00:20:15.000000 aorta_sirius-0.3/src/sirius/__init__.py
```

### Comparing `aorta_sirius-0.2/setup.py` & `aorta_sirius-0.3/setup.py`

 * *Files identical despite different names*

