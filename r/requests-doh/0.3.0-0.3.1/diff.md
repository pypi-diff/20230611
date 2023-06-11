# Comparing `tmp/requests-doh-0.3.0.tar.gz` & `tmp/requests-doh-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests-doh-0.3.0.tar", last modified: Sun Feb 12 15:21:55 2023, max compression
+gzip compressed data, was "requests-doh-0.3.1.tar", last modified: Sun Jun 11 05:06:23 2023, max compression
```

## Comparing `requests-doh-0.3.0.tar` & `requests-doh-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:21:55.782502 requests-doh-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-12 15:21:44.000000 requests-doh-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-12 15:21:44.000000 requests-doh-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-02-12 15:21:55.782502 requests-doh-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-02-12 15:21:44.000000 requests-doh-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:21:55.782502 requests-doh-0.3.0/requests_doh/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requests_doh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requests_doh/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requests_doh/cachemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requests_doh/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requests_doh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requests_doh/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requests_doh/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:21:55.782502 requests-doh-0.3.0/requests_doh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-02-12 15:21:55.000000 requests-doh-0.3.0/requests_doh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-12 15:21:55.000000 requests-doh-0.3.0/requests_doh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 15:21:55.000000 requests-doh-0.3.0/requests_doh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-12 15:21:55.000000 requests-doh-0.3.0/requests_doh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-12 15:21:55.000000 requests-doh-0.3.0/requests_doh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-12 15:21:44.000000 requests-doh-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 15:21:55.782502 requests-doh-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-12 15:21:44.000000 requests-doh-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:06:23.849029 requests-doh-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-11 05:06:10.000000 requests-doh-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-11 05:06:10.000000 requests-doh-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-11 05:06:23.849029 requests-doh-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-11 05:06:10.000000 requests-doh-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:06:23.849029 requests-doh-0.3.1/requests_doh/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requests_doh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requests_doh/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requests_doh/cachemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requests_doh/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requests_doh/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requests_doh/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requests_doh/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:06:23.849029 requests-doh-0.3.1/requests_doh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-11 05:06:23.000000 requests-doh-0.3.1/requests_doh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-11 05:06:23.000000 requests-doh-0.3.1/requests_doh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 05:06:23.000000 requests-doh-0.3.1/requests_doh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-11 05:06:23.000000 requests-doh-0.3.1/requests_doh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 05:06:23.000000 requests-doh-0.3.1/requests_doh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-11 05:06:10.000000 requests-doh-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 05:06:23.849029 requests-doh-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-11 05:06:10.000000 requests-doh-0.3.1/setup.py
```

### Comparing `requests-doh-0.3.0/LICENSE` & `requests-doh-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-doh-0.3.0/PKG-INFO` & `requests-doh-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-doh
-Version: 0.3.0
+Version: 0.3.1
 Summary: DNS over HTTPS resolver for python requests
 Home-page: https://github.com/mansuf/requests-doh
 Author: Rahman Yusuf
 Author-email: danipart4@gmail.com
 License: MIT
 Keywords: requests,doh,dns,https,dns-over-https
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `requests-doh-0.3.0/README.md` & `requests-doh-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `requests-doh-0.3.0/requests_doh/adapter.py` & `requests-doh-0.3.1/requests_doh/adapter.py`

 * *Files identical despite different names*

### Comparing `requests-doh-0.3.0/requests_doh/cachemanager.py` & `requests-doh-0.3.1/requests_doh/cachemanager.py`

 * *Files identical despite different names*

### Comparing `requests-doh-0.3.0/requests_doh/connector.py` & `requests-doh-0.3.1/requests_doh/connector.py`

 * *Files identical despite different names*

### Comparing `requests-doh-0.3.0/requests_doh/resolver.py` & `requests-doh-0.3.1/requests_doh/resolver.py`

 * *Files identical despite different names*

### Comparing `requests-doh-0.3.0/requests_doh/session.py` & `requests-doh-0.3.1/requests_doh/session.py`

 * *Files identical despite different names*

### Comparing `requests-doh-0.3.0/requests_doh.egg-info/PKG-INFO` & `requests-doh-0.3.1/requests_doh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-doh
-Version: 0.3.0
+Version: 0.3.1
 Summary: DNS over HTTPS resolver for python requests
 Home-page: https://github.com/mansuf/requests-doh
 Author: Rahman Yusuf
 Author-email: danipart4@gmail.com
 License: MIT
 Keywords: requests,doh,dns,https,dns-over-https
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `requests-doh-0.3.0/setup.py` & `requests-doh-0.3.1/setup.py`

 * *Files identical despite different names*

