# Comparing `tmp/pyketra-0.0.3.tar.gz` & `tmp/pyketra-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyketra-0.0.3.tar", last modified: Fri Jun  7 16:22:34 2019, max compression
+gzip compressed data, was "pyketra-0.0.4.tar", last modified: Sat Jun 10 22:49:57 2023, max compression
```

## Comparing `pyketra-0.0.3.tar` & `pyketra-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2019-06-07 16:22:34.000000 pyketra-0.0.3/
--rw-r--r--   0 greg       (501) staff       (20)      593 2019-06-07 16:22:34.000000 pyketra-0.0.3/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      514 2019-06-07 16:20:55.000000 pyketra-0.0.3/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2019-06-07 16:22:34.000000 pyketra-0.0.3/pyketra/
--rw-r--r--   0 greg       (501) staff       (20)    26402 2019-06-07 04:39:56.000000 pyketra-0.0.3/pyketra/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2019-06-07 16:22:34.000000 pyketra-0.0.3/pyketra.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      593 2019-06-07 16:22:34.000000 pyketra-0.0.3/pyketra.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      228 2019-06-07 16:22:34.000000 pyketra-0.0.3/pyketra.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2019-06-07 16:22:34.000000 pyketra-0.0.3/pyketra.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       10 2019-06-07 16:22:34.000000 pyketra-0.0.3/pyketra.egg-info/requires.txt
--rw-r--r--   0 greg       (501) staff       (20)        8 2019-06-07 16:22:34.000000 pyketra-0.0.3/pyketra.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2019-06-07 16:22:34.000000 pyketra-0.0.3/pyketra.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2019-06-07 16:22:34.000000 pyketra-0.0.3/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      752 2019-06-07 04:44:27.000000 pyketra-0.0.3/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 22:49:57.530971 pyketra-0.0.4/
+-rw-r--r--   0 greg       (501) staff       (20)     1091 2023-06-10 22:00:08.000000 pyketra-0.0.4/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      576 2023-06-10 22:49:57.531101 pyketra-0.0.4/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      510 2023-06-10 22:46:10.000000 pyketra-0.0.4/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 22:49:57.528087 pyketra-0.0.4/pyketra/
+-rw-r--r--   0 greg       (501) staff       (20)    27172 2023-06-10 22:46:21.000000 pyketra-0.0.4/pyketra/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 22:49:57.530614 pyketra-0.0.4/pyketra.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      576 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      236 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       19 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/requires.txt
+-rw-r--r--   0 greg       (501) staff       (20)        8 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 22:49:57.000000 pyketra-0.0.4/pyketra.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-06-10 22:49:57.531505 pyketra-0.0.4/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      764 2023-06-10 22:46:21.000000 pyketra-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyketra-0.0.3/PKG-INFO` & `pyketra-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyketra
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for Ketra Controller
 Home-page: http://github.com/gjbadros/pyketra
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
```

### Comparing `pyketra-0.0.3/pyketra/__init__.py` & `pyketra-0.0.4/pyketra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,35 @@
 from math import log
 from urllib.parse import quote
 # from urllib import disable_warnings
 from colormath.color_objects import LabColor, xyYColor, sRGBColor, HSVColor
 from colormath.color_conversions import convert_color
 import requests
 
+import ssl
+from urllib3.util.ssl_ import create_urllib3_context
+from urllib3.poolmanager import PoolManager
+from requests.adapters import HTTPAdapter
+
+ctx = create_urllib3_context()
+ctx.load_default_certs()
+ctx.options |= 0x4  # ssl.OP_LEGACY_SERVER_CONNECT
+print("ALLOW_LEGACY_SERVER_CONNECT")
+
 # urllib.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 _LOGGER = logging.getLogger(__name__)
 
+class KetraHttpAdapter(HTTPAdapter):
+    """"Transport adapter" that allows us to connect to Ketra"""
+
+    def init_poolmanager(self, connections, maxsize, block=False):
+        self.poolmanager = PoolManager(ssl_context=ctx)
+
+ketra_session = requests.Session()
+
 def xml_escape(s):
     """Escape XML meta characters '<' and '&'."""
     answer = s.replace("<", "&lt;")
     answer = answer.replace("&", "&amp;")
     return answer
 
 
@@ -348,17 +366,18 @@
                 _LOGGER.info("read cached ketra configuration file %s", filename)
                 f.close()
                 success = True
             except Exception as e:
                 _LOGGER.warning("Failed loading cached config file for ketra: %s", e)
 
         if not success:
-            _LOGGER.info("doing request for ketra configuration file")
             groupsUrl = 'https://' + self._host + '/ketra.cgi/api/v1/groups'
-            r = requests.get(groupsUrl, auth=('', self._password), verify=False)
+            _LOGGER.info("doing request for ketra configuration file ", groupsUrl)
+            ketra_session.mount(groupsUrl, KetraHttpAdapter())
+            r = ketra_session.get(groupsUrl, auth=('', self._password), verify=False)
             # convert the response into a JSON object
             responseEnvelope = r.json()
             # pull the relevant content out of the response envelope
             json_db = responseEnvelope['Content']
             try:
                 f = open(filename, "w")
                 f.write(r.content.decode('utf-8'))
@@ -506,15 +525,16 @@
                     'id': self._id, 'level': self._level, 'xy': self._xy})
 
     def __do_query_level(self):
         """Helper to perform the actual query the current dimmer level of the
         output. For pure on/off loads the result is either 0.0 or 100.0."""
         _LOGGER.info("__do_query_level(%s)", self.name)
         lightURL = 'https://' + self._ketra._host + '/ketra.cgi/api/v1/Groups/' + quote(self._name)
-        r = requests.get(lightURL, auth=('', self._ketra._password), verify=False)
+        ketra_session.mount(lightURL, KetraHttpAdapter())
+        r = ketra_session.get(lightURL, auth=('', self._ketra._password), verify=False)
         content = r.json()['Content']
         state = content['State']
         self._xy_chroma = [state['xChromaticity'], state['yChromaticity']]
         self._level = state['Brightness']
         return True
 
 
@@ -532,15 +552,16 @@
     def _set_state(self, dictionary):
         lightURL = ('https://' + self._ketra._host +
                     '/ketra.cgi/api/v1/Groups/' + quote(self._name) + "/State")
         _LOGGER.warning("Sending Ketra %s", json.dumps(dictionary))
         # TODO: make an option to do NOOP sends -- for now just comment out if you don't want to hit
         # the Ketra N4 with the request
         if not self._ketra._noop_set_state:
-            requests.put(lightURL, data=json.dumps(dictionary),
+            ketra_session.mount(lightURL, KetraHttpAdapter())
+            ketra_sessions.put(lightURL, data=json.dumps(dictionary),
                          auth=('', self._ketra._password), verify=False)
         else:
             _LOGGER.warning("NOT ACTUALLY MAKING REQUEST TO KETRA N4")
 
 
     @level.setter
     def level(self, new_level):
```

### Comparing `pyketra-0.0.3/pyketra.egg-info/PKG-INFO` & `pyketra-0.0.4/pyketra.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyketra
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for Ketra Controller
 Home-page: http://github.com/gjbadros/pyketra
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
```

### Comparing `pyketra-0.0.3/setup.py` & `pyketra-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyketra',
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     description='Python library for Ketra Controller',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyketra',
     packages=find_packages(),
     classifiers=[
@@ -16,10 +16,10 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.4',
         'Topic :: Home Automation',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    install_requires=['colormath'],
+    install_requires=['colormath', 'requests'],
     zip_safe=True,
 )
```

