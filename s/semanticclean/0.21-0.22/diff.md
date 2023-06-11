# Comparing `tmp/semanticclean-0.21.tar.gz` & `tmp/semanticclean-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticclean-0.21.tar", last modified: Sun Jun 11 12:42:04 2023, max compression
+gzip compressed data, was "semanticclean-0.22.tar", last modified: Sun Jun 11 12:45:45 2023, max compression
```

## Comparing `semanticclean-0.21.tar` & `semanticclean-0.22.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:42:04.610825 semanticclean-0.21/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 12:42:04.610825 semanticclean-0.21/PKG-INFO
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       16 2023-06-11 11:49:28.000000 semanticclean-0.21/README.md
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:42:04.610825 semanticclean-0.21/semanticclean/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 11:22:27.000000 semanticclean-0.21/semanticclean/__init__.py
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:42:04.610825 semanticclean-0.21/semanticclean.egg-info/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 12:42:04.000000 semanticclean-0.21/semanticclean.egg-info/PKG-INFO
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      228 2023-06-11 12:42:04.000000 semanticclean-0.21/semanticclean.egg-info/SOURCES.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:42:04.000000 semanticclean-0.21/semanticclean.egg-info/dependency_links.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:42:04.000000 semanticclean-0.21/semanticclean.egg-info/not-zip-safe
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       14 2023-06-11 12:42:04.000000 semanticclean-0.21/semanticclean.egg-info/top_level.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 12:42:04.610825 semanticclean-0.21/setup.cfg
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      303 2023-06-11 12:41:31.000000 semanticclean-0.21/setup.py
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:45:45.037999 semanticclean-0.22/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 12:45:45.037999 semanticclean-0.22/PKG-INFO
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       16 2023-06-11 11:49:28.000000 semanticclean-0.22/README.md
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:45:45.034000 semanticclean-0.22/semanticclean/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 11:22:27.000000 semanticclean-0.22/semanticclean/__init__.py
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:45:45.034000 semanticclean-0.22/semanticclean.egg-info/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 12:45:45.000000 semanticclean-0.22/semanticclean.egg-info/PKG-INFO
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      228 2023-06-11 12:45:45.000000 semanticclean-0.22/semanticclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:45:45.000000 semanticclean-0.22/semanticclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:45:45.000000 semanticclean-0.22/semanticclean.egg-info/not-zip-safe
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       14 2023-06-11 12:45:45.000000 semanticclean-0.22/semanticclean.egg-info/top_level.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 12:45:45.037999 semanticclean-0.22/setup.cfg
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      303 2023-06-11 12:45:31.000000 semanticclean-0.22/setup.py
```

