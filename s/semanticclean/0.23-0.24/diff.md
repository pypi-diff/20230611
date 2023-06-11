# Comparing `tmp/semanticclean-0.23.tar.gz` & `tmp/semanticclean-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticclean-0.23.tar", last modified: Sun Jun 11 12:50:05 2023, max compression
+gzip compressed data, was "semanticclean-0.24.tar", last modified: Sun Jun 11 12:53:11 2023, max compression
```

## Comparing `semanticclean-0.23.tar` & `semanticclean-0.24.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:50:05.601685 semanticclean-0.23/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 12:50:05.601685 semanticclean-0.23/PKG-INFO
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       16 2023-06-11 11:49:28.000000 semanticclean-0.23/README.md
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:50:05.601685 semanticclean-0.23/semanticclean.egg-info/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 12:50:05.000000 semanticclean-0.23/semanticclean.egg-info/PKG-INFO
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      202 2023-06-11 12:50:05.000000 semanticclean-0.23/semanticclean.egg-info/SOURCES.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:50:05.000000 semanticclean-0.23/semanticclean.egg-info/dependency_links.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:50:05.000000 semanticclean-0.23/semanticclean.egg-info/not-zip-safe
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:50:05.000000 semanticclean-0.23/semanticclean.egg-info/top_level.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 12:50:05.601685 semanticclean-0.23/setup.cfg
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      303 2023-06-11 12:49:58.000000 semanticclean-0.23/setup.py
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:53:11.911198 semanticclean-0.24/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 12:53:11.911198 semanticclean-0.24/PKG-INFO
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       16 2023-06-11 11:49:28.000000 semanticclean-0.24/README.md
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:53:11.911198 semanticclean-0.24/semanticclean.egg-info/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 12:53:11.000000 semanticclean-0.24/semanticclean.egg-info/PKG-INFO
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      202 2023-06-11 12:53:11.000000 semanticclean-0.24/semanticclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:53:11.000000 semanticclean-0.24/semanticclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:53:11.000000 semanticclean-0.24/semanticclean.egg-info/not-zip-safe
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:53:11.000000 semanticclean-0.24/semanticclean.egg-info/top_level.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 12:53:11.911198 semanticclean-0.24/setup.cfg
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      303 2023-06-11 12:52:44.000000 semanticclean-0.24/setup.py
```

