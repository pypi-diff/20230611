# Comparing `tmp/PySimplePolls-0.0.1.tar.gz` & `tmp/PySimplePolls-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySimplePolls-0.0.1.tar", last modified: Sun Jun 11 08:43:47 2023, max compression
+gzip compressed data, was "PySimplePolls-0.0.2.tar", last modified: Sun Jun 11 09:26:43 2023, max compression
```

## Comparing `PySimplePolls-0.0.1.tar` & `PySimplePolls-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 08:43:47.708850 PySimplePolls-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-06-11 08:27:56.000000 PySimplePolls-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      767 2023-06-11 08:43:47.708850 PySimplePolls-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-11 08:30:26.000000 PySimplePolls-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-11 08:36:30.000000 PySimplePolls-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      694 2023-06-11 08:43:47.712849 PySimplePolls-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 08:43:47.368759 PySimplePolls-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 08:43:47.610827 PySimplePolls-0.0.1/src/PySImplePolls/
--rw-rw-rw-   0        0        0     1691 2023-06-11 08:19:25.000000 PySimplePolls-0.0.1/src/PySImplePolls/SimplePolls.py
--rw-rw-rw-   0        0        0        0 2023-06-11 08:34:03.000000 PySimplePolls-0.0.1/src/PySImplePolls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 08:43:47.704833 PySimplePolls-0.0.1/src/PySimplePolls.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-11 08:43:47.000000 PySimplePolls-0.0.1/src/PySimplePolls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-11 08:43:47.000000 PySimplePolls-0.0.1/src/PySimplePolls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 08:43:47.000000 PySimplePolls-0.0.1/src/PySimplePolls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-11 08:43:47.000000 PySimplePolls-0.0.1/src/PySimplePolls.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 09:26:43.821260 PySimplePolls-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-06-11 08:27:56.000000 PySimplePolls-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      767 2023-06-11 09:26:43.822259 PySimplePolls-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-11 08:30:26.000000 PySimplePolls-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-11 08:36:30.000000 PySimplePolls-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      694 2023-06-11 09:26:43.834261 PySimplePolls-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 09:26:43.559259 PySimplePolls-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 09:26:43.739260 PySimplePolls-0.0.2/src/PySImplePolls/
+-rw-rw-rw-   0        0        0     1679 2023-06-11 09:23:28.000000 PySimplePolls-0.0.2/src/PySImplePolls/SimplePolls.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 08:34:03.000000 PySimplePolls-0.0.2/src/PySImplePolls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:26:43.808257 PySimplePolls-0.0.2/src/PySimplePolls.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-11 09:26:43.000000 PySimplePolls-0.0.2/src/PySimplePolls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-11 09:26:43.000000 PySimplePolls-0.0.2/src/PySimplePolls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 09:26:43.000000 PySimplePolls-0.0.2/src/PySimplePolls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-11 09:26:43.000000 PySimplePolls-0.0.2/src/PySimplePolls.egg-info/top_level.txt
```

### Comparing `PySimplePolls-0.0.1/LICENSE` & `PySimplePolls-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySimplePolls-0.0.1/PKG-INFO` & `PySimplePolls-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySimplePolls
-Version: 0.0.1
+Version: 0.0.2
 Summary: Seamless integration with SimplePolls API for easy poll management
 Home-page: https://github.com/mvishok/PySimplePolls
 Author: Vishok M
 Author-email: hello@vishok.tech
 Project-URL: Bug Tracker, https://github.com/mvishok/PySimplePolls/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PySimplePolls-0.0.1/setup.cfg` & `PySimplePolls-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7953 696d 706c 6550 6f6c 6c73   = PySimplePolls
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 310d 0a61 7574 686f 7220 3d20 5669 7368  1..author = Vish
+00000030: 320d 0a61 7574 686f 7220 3d20 5669 7368  2..author = Vish
 00000040: 6f6b 204d 0d0a 6175 7468 6f72 5f65 6d61  ok M..author_ema
 00000050: 696c 203d 2068 656c 6c6f 4076 6973 686f  il = hello@visho
 00000060: 6b2e 7465 6368 0d0a 6465 7363 7269 7074  k.tech..descript
 00000070: 696f 6e20 3d20 5365 616d 6c65 7373 2069  ion = Seamless i
 00000080: 6e74 6567 7261 7469 6f6e 2077 6974 6820  ntegration with 
 00000090: 5369 6d70 6c65 506f 6c6c 7320 4150 4920  SimplePolls API 
 000000a0: 666f 7220 6561 7379 2070 6f6c 6c20 6d61  for easy poll ma
```

### Comparing `PySimplePolls-0.0.1/src/PySImplePolls/SimplePolls.py` & `PySimplePolls-0.0.2/src/PySImplePolls/SimplePolls.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,40 +17,40 @@
         return response['poll_id']
     else:
         return response['message'], response['error']
     
 def find(pid):
     url = "https://polls.vishok.tech/api/poll"
     params = {
-        "poll_id": pid
+        "pid": pid
     }
     response = requests.get(url, params=params)
     response = response.json()
     if response['message'] == 'success':
         return response
     else:
         return response['message'], response['error']
 
 def vote(pid, vote):
     url = "https://polls.vishok.tech/api/vote"
     params = {
-        "poll_id": pid,
+        "pid": pid,
         "vote": vote
     }
     response = requests.get(url, params=params)
     response = response.json()
     if response['message'] == 'success':
         return response
     else:
         return response['message'], response['error']
 
 def delete(pid, api_key):
     url = "https://polls.vishok.tech/api/delete"
     params = {
-        "poll_id": pid,
+        "pid": pid,
         "api_key": api_key
     }
     response = requests.get(url, params=params)
     response = response.json()
     if response['message'] == 'success':
         return True
     else:
```

### Comparing `PySimplePolls-0.0.1/src/PySimplePolls.egg-info/PKG-INFO` & `PySimplePolls-0.0.2/src/PySimplePolls.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySimplePolls
-Version: 0.0.1
+Version: 0.0.2
 Summary: Seamless integration with SimplePolls API for easy poll management
 Home-page: https://github.com/mvishok/PySimplePolls
 Author: Vishok M
 Author-email: hello@vishok.tech
 Project-URL: Bug Tracker, https://github.com/mvishok/PySimplePolls/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

