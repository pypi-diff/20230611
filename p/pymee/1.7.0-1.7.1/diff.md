# Comparing `tmp/pymee-1.7.0.tar.gz` & `tmp/pymee-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymee-1.7.0.tar", last modified: Fri May  5 07:03:39 2023, max compression
+gzip compressed data, was "pymee-1.7.1.tar", last modified: Sun Jun 11 20:05:50 2023, max compression
```

## Comparing `pymee-1.7.0.tar` & `pymee-1.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:03:39.354405 pymee-1.7.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-05 07:03:36.000000 pymee-1.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6037 2023-05-05 07:03:39.354405 pymee-1.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5627 2023-05-05 07:03:36.000000 pymee-1.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:03:39.354405 pymee-1.7.0/pymee/
--rw-r--r--   0 root         (0) root         (0)    16359 2023-05-05 07:03:36.000000 pymee-1.7.0/pymee/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26751 2023-05-05 07:03:36.000000 pymee-1.7.0/pymee/const.py
--rw-r--r--   0 root         (0) root         (0)    10984 2023-05-05 07:03:36.000000 pymee-1.7.0/pymee/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:03:39.354405 pymee-1.7.0/pymee.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6037 2023-05-05 07:03:39.000000 pymee-1.7.0/pymee.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-05 07:03:39.000000 pymee-1.7.0/pymee.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 07:03:39.000000 pymee-1.7.0/pymee.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-05 07:03:39.000000 pymee-1.7.0/pymee.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-05 07:03:39.354405 pymee-1.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      647 2023-05-05 07:03:37.000000 pymee-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 20:05:50.986852 pymee-1.7.1/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-06-11 20:05:47.000000 pymee-1.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-06-11 20:05:50.986852 pymee-1.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5627 2023-06-11 20:05:47.000000 pymee-1.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 20:05:50.986852 pymee-1.7.1/pymee/
+-rw-r--r--   0 root         (0) root         (0)    16494 2023-06-11 20:05:47.000000 pymee-1.7.1/pymee/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26751 2023-06-11 20:05:47.000000 pymee-1.7.1/pymee/const.py
+-rw-r--r--   0 root         (0) root         (0)    10984 2023-06-11 20:05:47.000000 pymee-1.7.1/pymee/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 20:05:50.986852 pymee-1.7.1/pymee.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-06-11 20:05:50.000000 pymee-1.7.1/pymee.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-11 20:05:50.000000 pymee-1.7.1/pymee.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 20:05:50.000000 pymee-1.7.1/pymee.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-11 20:05:50.000000 pymee-1.7.1/pymee.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-11 20:05:50.986852 pymee-1.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      647 2023-06-11 20:05:48.000000 pymee-1.7.1/setup.py
```

### Comparing `pymee-1.7.0/LICENSE` & `pymee-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymee-1.7.0/PKG-INFO` & `pymee-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymee
-Version: 1.7.0
+Version: 1.7.1
 Summary: a python library to interact with homee
 Home-page: https://github.com/FreshlyBrewedCode/pymee
 Author: FreshlyBrewedCode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pymee-1.7.0/README.md` & `pymee-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pymee-1.7.0/pymee/__init__.py` & `pymee-1.7.1/pymee/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,18 @@
                             exceptions.append(task.exception())
 
                         if exceptions and exceptions[0] is not None:
                             raise exceptions[0]
 
                     except websockets.exceptions.ConnectionClosed as e:
                         self.connected = False
-                        ws.abort_pings()
+                        try:
+                            ws.abort_pings()
+                        except Exception as e:
+                            await self._ws_on_error(e)
                         await self.on_disconnected()
         except Exception as e:
             await self._ws_on_error(e)
 
         self.retries += 1
         await self._ws_on_close()
```

### Comparing `pymee-1.7.0/pymee/const.py` & `pymee-1.7.1/pymee/const.py`

 * *Files identical despite different names*

### Comparing `pymee-1.7.0/pymee/model.py` & `pymee-1.7.1/pymee/model.py`

 * *Files identical despite different names*

### Comparing `pymee-1.7.0/pymee.egg-info/PKG-INFO` & `pymee-1.7.1/pymee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymee
-Version: 1.7.0
+Version: 1.7.1
 Summary: a python library to interact with homee
 Home-page: https://github.com/FreshlyBrewedCode/pymee
 Author: FreshlyBrewedCode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pymee-1.7.0/setup.py` & `pymee-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymee",
     version=__version__,
```

