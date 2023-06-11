# Comparing `tmp/semanticclean-0.0.1.tar.gz` & `tmp/semanticclean-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticclean-0.0.1.tar", last modified: Sun Jun 11 11:58:38 2023, max compression
+gzip compressed data, was "semanticclean-0.2.tar", last modified: Sun Jun 11 12:32:14 2023, max compression
```

## Comparing `semanticclean-0.0.1.tar` & `semanticclean-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 11:58:38.457358 semanticclean-0.0.1/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      261 2023-06-11 11:58:38.457358 semanticclean-0.0.1/PKG-INFO
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       16 2023-06-11 11:49:28.000000 semanticclean-0.0.1/README.md
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 11:58:38.457358 semanticclean-0.0.1/semanticclean.egg-info/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      261 2023-06-11 11:58:38.000000 semanticclean-0.0.1/semanticclean.egg-info/PKG-INFO
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      202 2023-06-11 11:58:38.000000 semanticclean-0.0.1/semanticclean.egg-info/SOURCES.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 11:58:38.000000 semanticclean-0.0.1/semanticclean.egg-info/dependency_links.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       18 2023-06-11 11:58:38.000000 semanticclean-0.0.1/semanticclean.egg-info/requires.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 11:58:38.000000 semanticclean-0.0.1/semanticclean.egg-info/top_level.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 11:58:38.457358 semanticclean-0.0.1/setup.cfg
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)     1188 2023-06-11 11:55:05.000000 semanticclean-0.0.1/setup.py
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:32:14.590835 semanticclean-0.2/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      233 2023-06-11 12:32:14.590835 semanticclean-0.2/PKG-INFO
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       16 2023-06-11 11:49:28.000000 semanticclean-0.2/README.md
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 12:32:14.590835 semanticclean-0.2/semanticclean.egg-info/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      233 2023-06-11 12:32:14.000000 semanticclean-0.2/semanticclean.egg-info/PKG-INFO
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      202 2023-06-11 12:32:14.000000 semanticclean-0.2/semanticclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:32:14.000000 semanticclean-0.2/semanticclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:32:14.000000 semanticclean-0.2/semanticclean.egg-info/not-zip-safe
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 12:32:14.000000 semanticclean-0.2/semanticclean.egg-info/top_level.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 12:32:14.590835 semanticclean-0.2/setup.cfg
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      303 2023-06-11 12:28:06.000000 semanticclean-0.2/setup.py
```

