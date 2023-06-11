# Comparing `tmp/crdp-gcp-0.0.3.tar.gz` & `tmp/crdp-gcp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crdp-gcp-0.0.3.tar", last modified: Sun Jun 11 13:14:15 2023, max compression
+gzip compressed data, was "crdp-gcp-0.0.4.tar", last modified: Sun Jun 11 13:21:27 2023, max compression
```

## Comparing `crdp-gcp-0.0.3.tar` & `crdp-gcp-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-06-11 13:14:15.094321 crdp-gcp-0.0.3/
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1071 2023-06-11 12:46:02.000000 crdp-gcp-0.0.3/LICENSE.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       39 2023-06-11 12:46:02.000000 crdp-gcp-0.0.3/MANIFEST.in
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2813 2023-06-11 13:14:15.094321 crdp-gcp-0.0.3/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2260 2023-06-11 12:46:02.000000 crdp-gcp-0.0.3/README.md
--rw-r--r--   0 vtec      (1000) vtec      (1000)   166146 2023-06-11 12:48:18.000000 crdp-gcp-0.0.3/crdp.c
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1383 2023-06-11 12:46:02.000000 crdp-gcp-0.0.3/crdp.pyx
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-06-11 13:14:15.094321 crdp-gcp-0.0.3/crdp_gcp.egg-info/
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2813 2023-06-11 13:14:15.000000 crdp-gcp-0.0.3/crdp_gcp.egg-info/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)      217 2023-06-11 13:14:15.000000 crdp-gcp-0.0.3/crdp_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-06-11 13:14:15.000000 crdp-gcp-0.0.3/crdp_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       21 2023-06-11 13:14:15.000000 crdp-gcp-0.0.3/crdp_gcp.egg-info/requires.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        5 2023-06-11 13:14:15.000000 crdp-gcp-0.0.3/crdp_gcp.egg-info/top_level.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-06-11 13:14:15.094321 crdp-gcp-0.0.3/setup.cfg
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1261 2023-06-11 13:13:56.000000 crdp-gcp-0.0.3/setup.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-06-11 13:21:27.954321 crdp-gcp-0.0.4/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1071 2023-06-11 12:46:02.000000 crdp-gcp-0.0.4/LICENSE.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       39 2023-06-11 12:46:02.000000 crdp-gcp-0.0.4/MANIFEST.in
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1043 2023-06-11 13:21:27.944321 crdp-gcp-0.0.4/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      489 2023-06-11 13:20:40.000000 crdp-gcp-0.0.4/README.md
+-rw-r--r--   0 vtec      (1000) vtec      (1000)   166146 2023-06-11 12:48:18.000000 crdp-gcp-0.0.4/crdp.c
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1383 2023-06-11 12:46:02.000000 crdp-gcp-0.0.4/crdp.pyx
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-06-11 13:21:27.944321 crdp-gcp-0.0.4/crdp_gcp.egg-info/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1043 2023-06-11 13:21:27.000000 crdp-gcp-0.0.4/crdp_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      217 2023-06-11 13:21:27.000000 crdp-gcp-0.0.4/crdp_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-06-11 13:21:27.000000 crdp-gcp-0.0.4/crdp_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       21 2023-06-11 13:21:27.000000 crdp-gcp-0.0.4/crdp_gcp.egg-info/requires.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        5 2023-06-11 13:21:27.000000 crdp-gcp-0.0.4/crdp_gcp.egg-info/top_level.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-06-11 13:21:27.954321 crdp-gcp-0.0.4/setup.cfg
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1261 2023-06-11 13:21:02.000000 crdp-gcp-0.0.4/setup.py
```

### Comparing `crdp-gcp-0.0.3/LICENSE.txt` & `crdp-gcp-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crdp-gcp-0.0.3/crdp.c` & `crdp-gcp-0.0.4/crdp.c`

 * *Files identical despite different names*

### Comparing `crdp-gcp-0.0.3/crdp.pyx` & `crdp-gcp-0.0.4/crdp.pyx`

 * *Files identical despite different names*

### Comparing `crdp-gcp-0.0.3/setup.py` & `crdp-gcp-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="crdp-gcp",
-    version="0.0.3",
+    version="0.0.4",
     author="Ran Bi",
     author_email="biran0079@gmail.com",
     description="A fast Ramer-Douglas-Peucker algorithm implementation. Updated for GCP cloud function",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vtecftwy/crdp-gcp",
     keywords="rdp ramer douglas peucker line simplification cython",
```

