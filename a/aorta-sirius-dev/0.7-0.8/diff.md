# Comparing `tmp/aorta_sirius_dev-0.7.tar.gz` & `tmp/aorta_sirius_dev-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius_dev-0.7.tar", last modified: Sun Jun 11 04:17:46 2023, max compression
+gzip compressed data, was "aorta_sirius_dev-0.8.tar", last modified: Sun Jun 11 04:22:13 2023, max compression
```

## Comparing `aorta_sirius_dev-0.7.tar` & `aorta_sirius_dev-0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:46.409350 aorta_sirius_dev-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:17:46.409350 aorta_sirius_dev-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 04:17:31.000000 aorta_sirius_dev-0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:17:46.409350 aorta_sirius_dev-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-11 04:17:31.000000 aorta_sirius_dev-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:46.405350 aorta_sirius_dev-0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:46.405350 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:17:46.000000 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 04:17:46.000000 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:17:46.000000 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 04:17:46.000000 aorta_sirius_dev-0.7/src/aorta_sirius_dev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:46.405350 aorta_sirius_dev-0.7/src/sirius/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:17:31.000000 aorta_sirius_dev-0.7/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 04:21:57.000000 aorta_sirius_dev-0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-11 04:21:57.000000 aorta_sirius_dev-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-11 04:22:13.000000 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 04:22:13.000000 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:22:13.000000 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 04:22:13.000000 aorta_sirius_dev-0.8/src/aorta_sirius_dev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:22:13.323422 aorta_sirius_dev-0.8/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:21:57.000000 aorta_sirius_dev-0.8/src/sirius/__init__.py
```

### Comparing `aorta_sirius_dev-0.7/setup.py` & `aorta_sirius_dev-0.8/setup.py`

 * *Files identical despite different names*

