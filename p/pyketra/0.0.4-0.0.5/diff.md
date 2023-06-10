# Comparing `tmp/pyketra-0.0.4.tar.gz` & `tmp/pyketra-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyketra-0.0.4.tar", last modified: Sat Jun 10 22:49:57 2023, max compression
+gzip compressed data, was "pyketra-0.0.5.tar", last modified: Sat Jun 10 23:08:28 2023, max compression
```

## Comparing `pyketra-0.0.4.tar` & `pyketra-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 22:49:57.530971 pyketra-0.0.4/
--rw-r--r--   0 greg       (501) staff       (20)     1091 2023-06-10 22:00:08.000000 pyketra-0.0.4/LICENSE
--rw-r--r--   0 greg       (501) staff       (20)      576 2023-06-10 22:49:57.531101 pyketra-0.0.4/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      510 2023-06-10 22:46:10.000000 pyketra-0.0.4/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 22:49:57.528087 pyketra-0.0.4/pyketra/
--rw-r--r--   0 greg       (501) staff       (20)    27172 2023-06-10 22:46:21.000000 pyketra-0.0.4/pyketra/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 22:49:57.530614 pyketra-0.0.4/pyketra.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      576 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      236 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       19 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/requires.txt
--rw-r--r--   0 greg       (501) staff       (20)        8 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2023-06-10 22:49:57.531505 pyketra-0.0.4/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      764 2023-06-10 22:46:21.000000 pyketra-0.0.4/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 23:08:28.778459 pyketra-0.0.5/
+-rw-r--r--   0 greg       (501) staff       (20)     1091 2023-06-10 22:00:08.000000 pyketra-0.0.5/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      576 2023-06-10 23:08:28.778546 pyketra-0.0.5/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      510 2023-06-10 22:46:10.000000 pyketra-0.0.5/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 23:08:28.775749 pyketra-0.0.5/pyketra/
+-rw-r--r--   0 greg       (501) staff       (20)    27171 2023-06-10 23:02:28.000000 pyketra-0.0.5/pyketra/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 23:08:28.778161 pyketra-0.0.5/pyketra.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      576 2023-06-10 23:08:28.000000 pyketra-0.0.5/pyketra.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      236 2023-06-10 23:08:28.000000 pyketra-0.0.5/pyketra.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 23:08:28.000000 pyketra-0.0.5/pyketra.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       19 2023-06-10 23:08:28.000000 pyketra-0.0.5/pyketra.egg-info/requires.txt
+-rw-r--r--   0 greg       (501) staff       (20)        8 2023-06-10 23:08:28.000000 pyketra-0.0.5/pyketra.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 22:49:57.000000 pyketra-0.0.5/pyketra.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-06-10 23:08:28.778922 pyketra-0.0.5/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      764 2023-06-10 23:02:37.000000 pyketra-0.0.5/setup.py
```

### Comparing `pyketra-0.0.4/LICENSE` & `pyketra-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyketra-0.0.4/PKG-INFO` & `pyketra-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyketra
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for Ketra Controller
 Home-page: http://github.com/gjbadros/pyketra
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyketra-0.0.4/pyketra/__init__.py` & `pyketra-0.0.5/pyketra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,15 +553,15 @@
         lightURL = ('https://' + self._ketra._host +
                     '/ketra.cgi/api/v1/Groups/' + quote(self._name) + "/State")
         _LOGGER.warning("Sending Ketra %s", json.dumps(dictionary))
         # TODO: make an option to do NOOP sends -- for now just comment out if you don't want to hit
         # the Ketra N4 with the request
         if not self._ketra._noop_set_state:
             ketra_session.mount(lightURL, KetraHttpAdapter())
-            ketra_sessions.put(lightURL, data=json.dumps(dictionary),
+            ketra_session.put(lightURL, data=json.dumps(dictionary),
                          auth=('', self._ketra._password), verify=False)
         else:
             _LOGGER.warning("NOT ACTUALLY MAKING REQUEST TO KETRA N4")
 
 
     @level.setter
     def level(self, new_level):
```

### Comparing `pyketra-0.0.4/pyketra.egg-info/PKG-INFO` & `pyketra-0.0.5/pyketra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyketra
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for Ketra Controller
 Home-page: http://github.com/gjbadros/pyketra
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyketra-0.0.4/setup.py` & `pyketra-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyketra',
-    version='0.0.4',
+    version='0.0.5',
     license='MIT',
     description='Python library for Ketra Controller',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyketra',
     packages=find_packages(),
     classifiers=[
```

