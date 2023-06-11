# Comparing `tmp/kdslibs-0.0.6.tar.gz` & `tmp/kdslibs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdslibs-0.0.6.tar", last modified: Sat Jun 10 16:59:33 2023, max compression
+gzip compressed data, was "kdslibs-0.0.7.tar", last modified: Sun Jun 11 14:07:25 2023, max compression
```

## Comparing `kdslibs-0.0.6.tar` & `kdslibs-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:59:33.162751 kdslibs-0.0.6/
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.6/LICENSE
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 16:59:33.162751 kdslibs-0.0.6/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.6/README.md
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:59:33.152751 kdslibs-0.0.6/kdslibs/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      701 2023-06-10 16:58:59.000000 kdslibs-0.0.6/kdslibs/__init__.py
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:59:33.162751 kdslibs-0.0.6/kdslibs.egg-info/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 16:59:33.000000 kdslibs-0.0.6/kdslibs.egg-info/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-10 16:59:33.000000 kdslibs-0.0.6/kdslibs.egg-info/SOURCES.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-10 16:59:33.000000 kdslibs-0.0.6/kdslibs.egg-info/dependency_links.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-10 16:59:33.000000 kdslibs-0.0.6/kdslibs.egg-info/top_level.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-10 16:59:33.162751 kdslibs-0.0.6/setup.cfg
--rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-10 16:59:22.000000 kdslibs-0.0.6/setup.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-11 14:07:25.052380 kdslibs-0.0.7/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.7/LICENSE
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-11 14:07:25.052380 kdslibs-0.0.7/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.7/README.md
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-11 14:07:25.042380 kdslibs-0.0.7/kdslibs/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      701 2023-06-10 16:58:59.000000 kdslibs-0.0.7/kdslibs/__init__.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-11 14:07:25.042380 kdslibs-0.0.7/kdslibs.egg-info/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-11 14:07:25.000000 kdslibs-0.0.7/kdslibs.egg-info/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-11 14:07:25.000000 kdslibs-0.0.7/kdslibs.egg-info/SOURCES.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-11 14:07:25.000000 kdslibs-0.0.7/kdslibs.egg-info/dependency_links.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-11 14:07:25.000000 kdslibs-0.0.7/kdslibs.egg-info/top_level.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-11 14:07:25.052380 kdslibs-0.0.7/setup.cfg
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-11 14:07:21.000000 kdslibs-0.0.7/setup.py
```

### Comparing `kdslibs-0.0.6/kdslibs/__init__.py` & `kdslibs-0.0.7/kdslibs/__init__.py`

 * *Files identical despite different names*

