# Comparing `tmp/scratchattach-1.2.2.tar.gz` & `tmp/scratchattach-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.2.2.tar", last modified: Sat Jun 10 20:00:58 2023, max compression
+gzip compressed data, was "scratchattach-1.2.3.tar", last modified: Sun Jun 11 01:35:30 2023, max compression
```

## Comparing `scratchattach-1.2.2.tar` & `scratchattach-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 20:00:58.637782 scratchattach-1.2.2/
--rw-rw-rw-   0        0        0    22094 2023-06-10 20:00:58.636781 scratchattach-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    20730 2023-06-10 15:56:43.000000 scratchattach-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 20:00:58.614599 scratchattach-1.2.2/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.2/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    13680 2023-06-10 19:50:37.000000 scratchattach-1.2.2/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    18193 2023-06-10 20:00:46.000000 scratchattach-1.2.2/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.2/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.2/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.2/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.2/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.2/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.2/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.2/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-06-10 20:00:58.635781 scratchattach-1.2.2/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22094 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 20:00:58.637782 scratchattach-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-06-10 19:51:52.000000 scratchattach-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:35:30.871492 scratchattach-1.2.3/
+-rw-rw-rw-   0        0        0    22094 2023-06-11 01:35:30.870149 scratchattach-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    20730 2023-06-10 15:56:43.000000 scratchattach-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 01:35:30.855619 scratchattach-1.2.3/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.3/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-06-10 19:50:37.000000 scratchattach-1.2.3/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    18222 2023-06-11 01:35:04.000000 scratchattach-1.2.3/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.3/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.3/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.3/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.3/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.3/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.3/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.3/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:35:30.870149 scratchattach-1.2.3/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22094 2023-06-11 01:35:30.000000 scratchattach-1.2.3/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-11 01:35:30.000000 scratchattach-1.2.3/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 01:35:30.000000 scratchattach-1.2.3/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-11 01:35:30.000000 scratchattach-1.2.3/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-11 01:35:30.000000 scratchattach-1.2.3/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 01:35:30.871492 scratchattach-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-06-11 01:35:24.000000 scratchattach-1.2.3/setup.py
```

### Comparing `scratchattach-1.2.2/PKG-INFO` & `scratchattach-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.2
+Version: 1.2.3
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Platform: UNKNOWN
```

### Comparing `scratchattach-1.2.2/README.md` & `scratchattach-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach/_cloud.py` & `scratchattach-1.2.3/scratchattach/_cloud.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach/_cloud_requests.py` & `scratchattach-1.2.3/scratchattach/_cloud_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,14 +427,16 @@
                 for request_id in output_ids:
                     output = self.outputs[request_id]["output"]
                     request = self.outputs[request_id]["request"]["name"]
                     req_obj = self.outputs[request_id]["request"]
                     self._parse_output(output, request, req_obj, request_id)
                     self.outputs.pop(request_id)
 
+            time.sleep(0)
+
 
 class TwCloudRequests(CloudRequests):
     def __init__(self,
                  cloud_connection,
                  *,
                  used_cloud_vars=["1", "2", "3", "4", "5", "6", "7", "8", "9"],
                  ignore_exceptions=True,
```

### Comparing `scratchattach-1.2.2/scratchattach/_encoder.py` & `scratchattach-1.2.3/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach/_exceptions.py` & `scratchattach-1.2.3/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach/_forum.py` & `scratchattach-1.2.3/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach/_project.py` & `scratchattach-1.2.3/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach/_session.py` & `scratchattach-1.2.3/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach/_studio.py` & `scratchattach-1.2.3/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach/_user.py` & `scratchattach-1.2.3/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.2/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.2.3/scratchattach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.2
+Version: 1.2.3
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Platform: UNKNOWN
```

### Comparing `scratchattach-1.2.2/setup.py` & `scratchattach-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.2.2'
+VERSION = '1.2.3'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

