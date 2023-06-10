# Comparing `tmp/nsedt-0.0.3.tar.gz` & `tmp/nsedt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsedt-0.0.3.tar", last modified: Fri Jun  2 13:56:06 2023, max compression
+gzip compressed data, was "nsedt-0.0.4.tar", last modified: Sat Jun 10 23:32:01 2023, max compression
```

## Comparing `nsedt-0.0.3.tar` & `nsedt-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 13:55:54.000000 nsedt-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-02 13:56:06.620614 nsedt-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-02 13:55:54.000000 nsedt-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/nsedt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/equity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/nsedt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/resources/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/nsedt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-02 13:55:54.000000 nsedt-0.0.3/nsedt/utils/data_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:56:06.620614 nsedt-0.0.3/nsedt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 13:56:06.000000 nsedt-0.0.3/nsedt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 13:56:06.620614 nsedt-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-02 13:55:54.000000 nsedt-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 23:31:52.000000 nsedt-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-10 23:32:01.667057 nsedt-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-10 23:31:52.000000 nsedt-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/nsedt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/equity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/nsedt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/resources/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/nsedt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/utils/data_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/nsedt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-10 23:32:01.671057 nsedt-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-10 23:31:52.000000 nsedt-0.0.4/setup.py
```

### Comparing `nsedt-0.0.3/LICENSE` & `nsedt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.3/nsedt/utils/__init__.py` & `nsedt-0.0.4/nsedt/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 def get_cookies():
     response = requests.get(base_url, timeout=30, headers=get_headers())
     if response.status_code != requests.codes.ok:
         raise ValueError("Retry again in a minute.")
     return response.cookies.get_dict()
 
 
-def fetch_url(url, cookies):
+def fetch_url(url, cookies, key="data"):
     response = requests.get(url, timeout=30, headers=get_headers(), cookies=cookies)
     if response.status_code == requests.codes.ok:
         json_response = json.loads(response.content)
         try:
-            return pd.DataFrame.from_dict(json_response["data"])
+            return pd.DataFrame.from_dict(json_response[key])
         except:
             return pd.DataFrame.from_dict(json_response)
     else:
         raise ValueError("Please try again in a minute.")
```

### Comparing `nsedt-0.0.3/nsedt/utils/data_format.py` & `nsedt-0.0.4/nsedt/utils/data_format.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.3/setup.py` & `nsedt-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name="nsedt",
-    version="0.0.3",
+    version="0.0.4",
     author="Pratik Anand",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Library to collect NSE data in pandas dataframe",
     packages=find_packages(),
     url="https://github.com/pratik141/nsedt",
     install_requires=[
```

