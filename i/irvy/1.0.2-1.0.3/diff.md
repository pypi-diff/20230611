# Comparing `tmp/irvy-1.0.2.tar.gz` & `tmp/irvy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irvy-1.0.2.tar", last modified: Sat Jun 10 20:32:58 2023, max compression
+gzip compressed data, was "irvy-1.0.3.tar", last modified: Sun Jun 11 10:08:07 2023, max compression
```

## Comparing `irvy-1.0.2.tar` & `irvy-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-10 20:32:58.028215 irvy-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-10 20:32:48.000000 irvy-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/irvy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/irvy/generators/
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/generators/PlaywrightGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/generators/SeleniumGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/irvy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/irvy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:48.000000 irvy-1.0.2/irvy/utils/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:32:58.028215 irvy-1.0.2/irvy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 20:32:58.000000 irvy-1.0.2/irvy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 20:32:58.032214 irvy-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 20:32:48.000000 irvy-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.957610 irvy-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-11 10:08:07.957610 irvy-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-11 10:07:45.000000 irvy-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.953609 irvy-1.0.3/irvy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.953609 irvy-1.0.3/irvy/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/generators/PlaywrightGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/generators/SeleniumGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/irvy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.953609 irvy-1.0.3/irvy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/utils/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.953609 irvy-1.0.3/irvy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 10:08:07.957610 irvy-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-11 10:07:45.000000 irvy-1.0.3/setup.py
```

### Comparing `irvy-1.0.2/irvy/generators/PlaywrightGenerator.py` & `irvy-1.0.3/irvy/generators/PlaywrightGenerator.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.2/irvy/generators/SeleniumGenerator.py` & `irvy-1.0.3/irvy/generators/SeleniumGenerator.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.2/irvy/irvy.py` & `irvy-1.0.3/irvy/irvy.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.2/setup.py` & `irvy-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Open the README file.
 with open(file="README.md", mode="r") as readme_handle:
     long_description = readme_handle.read()
 
 setup(
     name='irvy',
-    version='1.0.2',
+    version='1.0.3',
     description='A brief description of your project',  # add this
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),  # this should automatically find your packages
     include_package_data=True,
     install_requires=[
         # list of dependencies
```

