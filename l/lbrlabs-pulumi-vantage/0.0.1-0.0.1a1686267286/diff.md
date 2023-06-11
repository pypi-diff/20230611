# Comparing `tmp/lbrlabs_pulumi_vantage-0.0.1.tar.gz` & `tmp/lbrlabs_pulumi_vantage-0.0.1a1686267286.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbrlabs_pulumi_vantage-0.0.1.tar", last modified: Sun Jun 11 18:25:41 2023, max compression
+gzip compressed data, was "dist/lbrlabs_pulumi_vantage-0.0.1a1686267286.tar", last modified: Thu Jun  8 23:39:47 2023, max compression
```

## Comparing `lbrlabs_pulumi_vantage-0.0.1.tar` & `lbrlabs_pulumi_vantage-0.0.1a1686267286.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/aws_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/get_aws_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/get_aws_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-11 18:25:41.000000 lbrlabs_pulumi_vantage-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/aws_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/get_aws_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/get_aws_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:39:47.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-08 23:39:46.000000 lbrlabs_pulumi_vantage-0.0.1a1686267286/setup.py
```

### Comparing `lbrlabs_pulumi_vantage-0.0.1/PKG-INFO` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lbrlabs_pulumi_vantage
-Version: 0.0.1
+Name: lbrlabs-pulumi-vantage
+Version: 0.0.1a1686267286
 Summary: A Pulumi package to create resource in vantage.sh.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-vantage
 Description: 
         # Vantage Resource Provider
```

### Comparing `lbrlabs_pulumi_vantage-0.0.1/README.md` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/README.md`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/__init__.py` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/_utilities.py` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/_utilities.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/aws_provider.py` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/aws_provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/config/vars.py` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/config/vars.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/get_aws_provider.py` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/get_aws_provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/get_aws_provider_info.py` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/get_aws_provider_info.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage/provider.py` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage/provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/PKG-INFO` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lbrlabs-pulumi-vantage
-Version: 0.0.1
+Name: lbrlabs_pulumi_vantage
+Version: 0.0.1a1686267286
 Summary: A Pulumi package to create resource in vantage.sh.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-vantage
 Description: 
         # Vantage Resource Provider
```

### Comparing `lbrlabs_pulumi_vantage-0.0.1/lbrlabs_pulumi_vantage.egg-info/SOURCES.txt` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/lbrlabs_pulumi_vantage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_vantage-0.0.1/setup.py` & `lbrlabs_pulumi_vantage-0.0.1a1686267286/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.1"
-PLUGIN_VERSION = "0.0.1"
+VERSION = "0.0.1a1686267286"
+PLUGIN_VERSION = "0.0.1-alpha.1686267286+209cac5c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'vantage', PLUGIN_VERSION, '--server', 'github://api.github.com/lbrlabs'])
         except OSError as error:
```

