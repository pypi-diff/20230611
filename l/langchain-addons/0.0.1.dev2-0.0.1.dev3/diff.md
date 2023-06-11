# Comparing `tmp/langchain_addons-0.0.1.dev2.tar.gz` & `tmp/langchain_addons-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_addons-0.0.1.dev2.tar", last modified: Sun Jun 11 02:23:41 2023, max compression
+gzip compressed data, was "langchain_addons-0.0.1.dev3.tar", last modified: Sun Jun 11 02:35:12 2023, max compression
```

## Comparing `langchain_addons-0.0.1.dev2.tar` & `langchain_addons-0.0.1.dev3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 02:23:41.688173 langchain_addons-0.0.1.dev2/
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1286 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev2/LICENSE
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)       16 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev2/MANIFEST.in
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1984 2023-06-11 02:23:41.684172 langchain_addons-0.0.1.dev2/PKG-INFO
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)       44 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev2/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 02:23:41.684172 langchain_addons-0.0.1.dev2/langchain_addons/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       50 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev2/langchain_addons/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       26 2023-06-11 02:23:37.000000 langchain_addons-0.0.1.dev2/langchain_addons/_version.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      159 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev2/langchain_addons/utils.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 02:23:41.684172 langchain_addons-0.0.1.dev2/langchain_addons.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1984 2023-06-11 02:23:41.000000 langchain_addons-0.0.1.dev2/langchain_addons.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      344 2023-06-11 02:23:41.000000 langchain_addons-0.0.1.dev2/langchain_addons.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-06-11 02:23:41.000000 langchain_addons-0.0.1.dev2/langchain_addons.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      103 2023-06-11 02:23:41.000000 langchain_addons-0.0.1.dev2/langchain_addons.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       17 2023-06-11 02:23:41.000000 langchain_addons-0.0.1.dev2/langchain_addons.egg-info/top_level.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      858 2023-06-11 02:04:06.000000 langchain_addons-0.0.1.dev2/pyproject.toml
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)      102 2023-06-11 02:14:15.000000 langchain_addons-0.0.1.dev2/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-06-11 02:23:41.688173 langchain_addons-0.0.1.dev2/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 02:35:12.164815 langchain_addons-0.0.1.dev3/
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1286 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev3/LICENSE
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)       16 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev3/MANIFEST.in
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1984 2023-06-11 02:35:12.164815 langchain_addons-0.0.1.dev3/PKG-INFO
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)       44 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev3/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 02:35:12.164815 langchain_addons-0.0.1.dev3/langchain_addons/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       50 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev3/langchain_addons/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       26 2023-06-11 02:35:07.000000 langchain_addons-0.0.1.dev3/langchain_addons/_version.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      159 2023-06-11 02:02:33.000000 langchain_addons-0.0.1.dev3/langchain_addons/utils.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-11 02:35:12.164815 langchain_addons-0.0.1.dev3/langchain_addons.egg-info/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1984 2023-06-11 02:35:12.000000 langchain_addons-0.0.1.dev3/langchain_addons.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      344 2023-06-11 02:35:12.000000 langchain_addons-0.0.1.dev3/langchain_addons.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-06-11 02:35:12.000000 langchain_addons-0.0.1.dev3/langchain_addons.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      103 2023-06-11 02:35:12.000000 langchain_addons-0.0.1.dev3/langchain_addons.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       17 2023-06-11 02:35:12.000000 langchain_addons-0.0.1.dev3/langchain_addons.egg-info/top_level.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      858 2023-06-11 02:35:04.000000 langchain_addons-0.0.1.dev3/pyproject.toml
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)      102 2023-06-11 02:14:15.000000 langchain_addons-0.0.1.dev3/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-06-11 02:35:12.164815 langchain_addons-0.0.1.dev3/setup.cfg
```

### Comparing `langchain_addons-0.0.1.dev2/LICENSE` & `langchain_addons-0.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_addons-0.0.1.dev2/PKG-INFO` & `langchain_addons-0.0.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_addons
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Extensions to langchain
 Author-email: Eduardo Morais <emdemor415@gmail.com>
 License: Copyright (c) 2023, Eduardo Morais
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `langchain_addons-0.0.1.dev2/langchain_addons.egg-info/PKG-INFO` & `langchain_addons-0.0.1.dev3/langchain_addons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-addons
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Extensions to langchain
 Author-email: Eduardo Morais <emdemor415@gmail.com>
 License: Copyright (c) 2023, Eduardo Morais
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `langchain_addons-0.0.1.dev2/pyproject.toml` & `langchain_addons-0.0.1.dev3/pyproject.toml`

 * *Files identical despite different names*

