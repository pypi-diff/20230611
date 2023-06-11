# Comparing `tmp/langchain_addons-0.0.2.tar.gz` & `tmp/langchain_addons-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_addons-0.0.2.tar", last modified: Sun Jun 11 04:46:26 2023, max compression
+gzip compressed data, was "langchain_addons-0.0.2rc1.tar", last modified: Sun Jun 11 04:45:42 2023, max compression
```

## Comparing `langchain_addons-0.0.2.tar` & `langchain_addons-0.0.2rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 04:46:26.189825 langchain_addons-0.0.2/
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1286 2023-06-11 02:02:33.000000 langchain_addons-0.0.2/LICENSE
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)       16 2023-06-11 02:02:33.000000 langchain_addons-0.0.2/MANIFEST.in
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      341 2023-06-11 04:46:26.189825 langchain_addons-0.0.2/PKG-INFO
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)       44 2023-06-11 02:02:33.000000 langchain_addons-0.0.2/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 04:46:26.189825 langchain_addons-0.0.2/langchain_addons/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       21 2023-06-11 04:46:23.000000 langchain_addons-0.0.2/langchain_addons/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-06-11 04:08:56.000000 langchain_addons-0.0.2/langchain_addons/agents.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 04:46:26.189825 langchain_addons-0.0.2/langchain_addons.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      341 2023-06-11 04:46:26.000000 langchain_addons-0.0.2/langchain_addons.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      293 2023-06-11 04:46:26.000000 langchain_addons-0.0.2/langchain_addons.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-06-11 04:46:26.000000 langchain_addons-0.0.2/langchain_addons.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       10 2023-06-11 04:46:26.000000 langchain_addons-0.0.2/langchain_addons.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       17 2023-06-11 04:46:26.000000 langchain_addons-0.0.2/langchain_addons.egg-info/top_level.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-06-11 04:46:26.189825 langchain_addons-0.0.2/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      470 2023-06-11 04:46:12.000000 langchain_addons-0.0.2/setup.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 04:45:42.817442 langchain_addons-0.0.2rc1/
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1286 2023-06-11 02:02:33.000000 langchain_addons-0.0.2rc1/LICENSE
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)       16 2023-06-11 02:02:33.000000 langchain_addons-0.0.2rc1/MANIFEST.in
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      344 2023-06-11 04:45:42.817442 langchain_addons-0.0.2rc1/PKG-INFO
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)       44 2023-06-11 02:02:33.000000 langchain_addons-0.0.2rc1/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 04:45:42.817442 langchain_addons-0.0.2rc1/langchain_addons/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       25 2023-06-11 04:45:35.000000 langchain_addons-0.0.2rc1/langchain_addons/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-06-11 04:08:56.000000 langchain_addons-0.0.2rc1/langchain_addons/agents.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 04:45:42.817442 langchain_addons-0.0.2rc1/langchain_addons.egg-info/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      344 2023-06-11 04:45:42.000000 langchain_addons-0.0.2rc1/langchain_addons.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      293 2023-06-11 04:45:42.000000 langchain_addons-0.0.2rc1/langchain_addons.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-06-11 04:45:42.000000 langchain_addons-0.0.2rc1/langchain_addons.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       10 2023-06-11 04:45:42.000000 langchain_addons-0.0.2rc1/langchain_addons.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       17 2023-06-11 04:45:42.000000 langchain_addons-0.0.2rc1/langchain_addons.egg-info/top_level.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-06-11 04:45:42.817442 langchain_addons-0.0.2rc1/setup.cfg
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      474 2023-06-11 04:45:39.000000 langchain_addons-0.0.2rc1/setup.py
```

### Comparing `langchain_addons-0.0.2/LICENSE` & `langchain_addons-0.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_addons-0.0.2/langchain_addons/agents.py` & `langchain_addons-0.0.2rc1/langchain_addons/agents.py`

 * *Files identical despite different names*

