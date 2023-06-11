# Comparing `tmp/gen_func-1.0.0.tar.gz` & `tmp/gen_func-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_func-1.0.0.tar", last modified: Sun Jun 11 17:41:09 2023, max compression
+gzip compressed data, was "gen_func-1.0.1.tar", last modified: Sun Jun 11 18:00:02 2023, max compression
```

## Comparing `gen_func-1.0.0.tar` & `gen_func-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 morarivas02   (501) staff       (20)        0 2023-06-11 17:41:09.239287 gen_func-1.0.0/
--rw-r--r--   0 morarivas02   (501) staff       (20)      433 2023-06-11 17:41:09.238398 gen_func-1.0.0/PKG-INFO
--rw-r--r--   0 morarivas02   (501) staff       (20)        0 2023-05-15 18:17:19.000000 gen_func-1.0.0/README.md
-drwxr-xr-x   0 morarivas02   (501) staff       (20)        0 2023-06-11 17:41:09.235782 gen_func-1.0.0/gen_func/
--rw-r--r--   0 morarivas02   (501) staff       (20)      124 2023-06-11 16:04:34.000000 gen_func-1.0.0/gen_func/__init__.py
--rw-r--r--   0 morarivas02   (501) staff       (20)      758 2023-06-11 15:27:53.000000 gen_func-1.0.0/gen_func/gpt_actions.py
--rw-r--r--   0 morarivas02   (501) staff       (20)    10533 2023-06-11 15:42:50.000000 gen_func-1.0.0/gen_func/main.py
--rw-r--r--   0 morarivas02   (501) staff       (20)     3647 2023-06-11 15:42:00.000000 gen_func-1.0.0/gen_func/meta_parsing.py
--rw-r--r--   0 morarivas02   (501) staff       (20)    11411 2023-06-08 16:10:29.000000 gen_func-1.0.0/gen_func/prompts.py
--rw-r--r--   0 morarivas02   (501) staff       (20)     4203 2023-06-07 18:42:08.000000 gen_func-1.0.0/gen_func/validation.py
-drwxr-xr-x   0 morarivas02   (501) staff       (20)        0 2023-06-11 17:41:09.237805 gen_func-1.0.0/gen_func.egg-info/
--rw-r--r--   0 morarivas02   (501) staff       (20)      433 2023-06-11 17:41:09.000000 gen_func-1.0.0/gen_func.egg-info/PKG-INFO
--rw-r--r--   0 morarivas02   (501) staff       (20)      307 2023-06-11 17:41:09.000000 gen_func-1.0.0/gen_func.egg-info/SOURCES.txt
--rw-r--r--   0 morarivas02   (501) staff       (20)        1 2023-06-11 17:41:09.000000 gen_func-1.0.0/gen_func.egg-info/dependency_links.txt
--rw-r--r--   0 morarivas02   (501) staff       (20)       23 2023-06-11 17:41:09.000000 gen_func-1.0.0/gen_func.egg-info/requires.txt
--rw-r--r--   0 morarivas02   (501) staff       (20)        9 2023-06-11 17:41:09.000000 gen_func-1.0.0/gen_func.egg-info/top_level.txt
--rw-r--r--   0 morarivas02   (501) staff       (20)       38 2023-06-11 17:41:09.239684 gen_func-1.0.0/setup.cfg
--rw-r--r--   0 morarivas02   (501) staff       (20)      653 2023-06-11 17:20:14.000000 gen_func-1.0.0/setup.py
+drwxr-xr-x   0 morarivas02   (501) staff       (20)        0 2023-06-11 18:00:02.466497 gen_func-1.0.1/
+-rw-r--r--   0 morarivas02   (501) staff       (20)      433 2023-06-11 18:00:02.460568 gen_func-1.0.1/PKG-INFO
+-rw-r--r--   0 morarivas02   (501) staff       (20)        0 2023-05-15 18:17:19.000000 gen_func-1.0.1/README.md
+drwxr-xr-x   0 morarivas02   (501) staff       (20)        0 2023-06-11 18:00:02.458128 gen_func-1.0.1/gen_func/
+-rw-r--r--   0 morarivas02   (501) staff       (20)      124 2023-06-11 16:04:34.000000 gen_func-1.0.1/gen_func/__init__.py
+-rw-r--r--   0 morarivas02   (501) staff       (20)      758 2023-06-11 15:27:53.000000 gen_func-1.0.1/gen_func/gpt_actions.py
+-rw-r--r--   0 morarivas02   (501) staff       (20)    10532 2023-06-11 17:56:54.000000 gen_func-1.0.1/gen_func/main.py
+-rw-r--r--   0 morarivas02   (501) staff       (20)     3647 2023-06-11 15:42:00.000000 gen_func-1.0.1/gen_func/meta_parsing.py
+-rw-r--r--   0 morarivas02   (501) staff       (20)    11410 2023-06-11 17:56:54.000000 gen_func-1.0.1/gen_func/prompts.py
+-rw-r--r--   0 morarivas02   (501) staff       (20)     4203 2023-06-07 18:42:08.000000 gen_func-1.0.1/gen_func/validation.py
+drwxr-xr-x   0 morarivas02   (501) staff       (20)        0 2023-06-11 18:00:02.460142 gen_func-1.0.1/gen_func.egg-info/
+-rw-r--r--   0 morarivas02   (501) staff       (20)      433 2023-06-11 18:00:02.000000 gen_func-1.0.1/gen_func.egg-info/PKG-INFO
+-rw-r--r--   0 morarivas02   (501) staff       (20)      307 2023-06-11 18:00:02.000000 gen_func-1.0.1/gen_func.egg-info/SOURCES.txt
+-rw-r--r--   0 morarivas02   (501) staff       (20)        1 2023-06-11 18:00:02.000000 gen_func-1.0.1/gen_func.egg-info/dependency_links.txt
+-rw-r--r--   0 morarivas02   (501) staff       (20)       23 2023-06-11 18:00:02.000000 gen_func-1.0.1/gen_func.egg-info/requires.txt
+-rw-r--r--   0 morarivas02   (501) staff       (20)        9 2023-06-11 18:00:02.000000 gen_func-1.0.1/gen_func.egg-info/top_level.txt
+-rw-r--r--   0 morarivas02   (501) staff       (20)       38 2023-06-11 18:00:02.466616 gen_func-1.0.1/setup.cfg
+-rw-r--r--   0 morarivas02   (501) staff       (20)      653 2023-06-11 17:57:55.000000 gen_func-1.0.1/setup.py
```

### Comparing `gen_func-1.0.0/gen_func/gpt_actions.py` & `gen_func-1.0.1/gen_func/gpt_actions.py`

 * *Files identical despite different names*

### Comparing `gen_func-1.0.0/gen_func/main.py` & `gen_func-1.0.1/gen_func/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from prototype import (prompts, gpt_actions, meta_parsing)
+from gen_func import (prompts, gpt_actions, meta_parsing)
 import ast
 
 
 # Variables that must first be established - user input and file path to meta schema
 def generate_func(name, desc, tags, params, output, content, template, df_table_attr, df_table_def, df_file_def):
     """The master function that will generate the function body and total string length of
     all gpt requests and responses
```

### Comparing `gen_func-1.0.0/gen_func/meta_parsing.py` & `gen_func-1.0.1/gen_func/meta_parsing.py`

 * *Files identical despite different names*

### Comparing `gen_func-1.0.0/gen_func/prompts.py` & `gen_func-1.0.1/gen_func/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from prototype import validation
+from gen_func import validation
 
 
 def get_tables_prompt(name, desc, tags, params, output, content, template, table_def_schema):
     """Based on user input and the db schema, creates a request for gpt to narrow
     down the tables_def_schema dictionary to only the necessary tables
 
     @param name: The name of the function.
```

### Comparing `gen_func-1.0.0/gen_func/validation.py` & `gen_func-1.0.1/gen_func/validation.py`

 * *Files identical despite different names*

### Comparing `gen_func-1.0.0/setup.py` & `gen_func-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='gen_func',
-    version='1.0.0',
+    version='1.0.1',
     author='Maria Mora Rivas',
     author_email='morarivas02@gmail.com',
     description='The purpose of this package is to use the openai api to generate the body of a function that '
                 'performs some database action',
     packages=['gen_func'],
     classifiers=[
         'Development Status :: 1 - Planning',
```

