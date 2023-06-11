# Comparing `tmp/graph_z_c-0.0.9.macosx-10.9-universal2.tar.gz` & `tmp/graph_z_c-0.1.1.macosx-10.9-universal2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_z_c-0.0.9.macosx-10.9-universal2.tar", last modified: Sun Jun 11 11:40:56 2023, max compression
+gzip compressed data, was "graph_z_c-0.1.1.macosx-10.9-universal2.tar", last modified: Sun Jun 11 11:47:18 2023, max compression
```

## Comparing `graph_z_c-0.0.9.macosx-10.9-universal2.tar` & `graph_z_c-0.1.1.macosx-10.9-universal2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:40:56.373606 ./
-drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:40:56.373660 ./Library/
-drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:40:56.373713 ./Library/Python/
-drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:40:56.373836 ./Library/Python/3.9/
-drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:40:56.393778 ./Library/Python/3.9/site-packages/
-drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:40:56.374248 ./Library/Python/3.9/site-packages/graph_z/
+drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:47:18.399548 ./
+drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:47:18.399602 ./Library/
+drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:47:18.399655 ./Library/Python/
+drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:47:18.399708 ./Library/Python/3.9/
+drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:47:18.405969 ./Library/Python/3.9/site-packages/
+drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:47:18.400096 ./Library/Python/3.9/site-packages/graph_z/
 -rw-r--r--   0 tharunkothari   (501) staff       (20)       73 2023-06-11 11:37:19.000000 ./Library/Python/3.9/site-packages/graph_z/__init__.py
 -rw-r--r--   0 tharunkothari   (501) staff       (20)     7395 2023-06-11 11:40:17.000000 ./Library/Python/3.9/site-packages/graph_z/graph_z.py
-drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:40:56.394648 ./Library/Python/3.9/site-packages/graph_z_c-0.0.9-py3.9.egg-info/
--rw-r--r--   0 tharunkothari   (501) staff       (20)      157 2023-06-11 11:40:56.392392 ./Library/Python/3.9/site-packages/graph_z_c-0.0.9-py3.9.egg-info/PKG-INFO
--rw-r--r--   0 tharunkothari   (501) staff       (20)      189 2023-06-11 11:40:56.393657 ./Library/Python/3.9/site-packages/graph_z_c-0.0.9-py3.9.egg-info/SOURCES.txt
--rw-r--r--   0 tharunkothari   (501) staff       (20)        1 2023-06-11 11:40:56.392569 ./Library/Python/3.9/site-packages/graph_z_c-0.0.9-py3.9.egg-info/dependency_links.txt
--rw-r--r--   0 tharunkothari   (501) staff       (20)        8 2023-06-11 11:40:56.392716 ./Library/Python/3.9/site-packages/graph_z_c-0.0.9-py3.9.egg-info/top_level.txt
+drwxr-xr-x   0 tharunkothari   (501) staff       (20)        0 2023-06-11 11:47:18.406684 ./Library/Python/3.9/site-packages/graph_z_c-0.1.1-py3.9.egg-info/
+-rw-r--r--   0 tharunkothari   (501) staff       (20)      157 2023-06-11 11:47:18.404790 ./Library/Python/3.9/site-packages/graph_z_c-0.1.1-py3.9.egg-info/PKG-INFO
+-rw-r--r--   0 tharunkothari   (501) staff       (20)      189 2023-06-11 11:47:18.405850 ./Library/Python/3.9/site-packages/graph_z_c-0.1.1-py3.9.egg-info/SOURCES.txt
+-rw-r--r--   0 tharunkothari   (501) staff       (20)        1 2023-06-11 11:47:18.404883 ./Library/Python/3.9/site-packages/graph_z_c-0.1.1-py3.9.egg-info/dependency_links.txt
+-rw-r--r--   0 tharunkothari   (501) staff       (20)        8 2023-06-11 11:47:18.404996 ./Library/Python/3.9/site-packages/graph_z_c-0.1.1-py3.9.egg-info/top_level.txt
```

