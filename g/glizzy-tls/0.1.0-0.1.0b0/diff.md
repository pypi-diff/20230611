# Comparing `tmp/glizzy_tls-0.1.0.tar.gz` & `tmp/glizzy_tls-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glizzy_tls-0.1.0.tar", last modified: Sun Jun 11 19:22:52 2023, max compression
+gzip compressed data, was "glizzy_tls-0.1.0b0.tar", last modified: Sun Jun 11 20:57:46 2023, max compression
```

## Comparing `glizzy_tls-0.1.0.tar` & `glizzy_tls-0.1.0b0.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 19:22:52.670546 glizzy_tls-0.1.0/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-06-11 19:12:41.000000 glizzy_tls-0.1.0/LICENSE
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5934 2023-06-11 19:22:52.670361 glizzy_tls-0.1.0/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5166 2023-06-11 19:16:06.000000 glizzy_tls-0.1.0/README.md
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 19:22:52.669151 glizzy_tls-0.1.0/glizzy_tls/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      200 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0/glizzy_tls/__init__.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      264 2023-06-11 18:22:27.000000 glizzy_tls-0.1.0/glizzy_tls/exceptions.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1644 2023-06-11 18:36:50.000000 glizzy_tls-0.1.0/glizzy_tls/models.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1149 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0/glizzy_tls/request.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     4930 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0/glizzy_tls/session.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 19:22:52.670077 glizzy_tls-0.1.0/glizzy_tls.egg-info/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5934 2023-06-11 19:22:52.000000 glizzy_tls-0.1.0/glizzy_tls.egg-info/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      275 2023-06-11 19:22:52.000000 glizzy_tls-0.1.0/glizzy_tls.egg-info/SOURCES.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 19:22:52.000000 glizzy_tls-0.1.0/glizzy_tls.egg-info/dependency_links.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2023-06-11 19:22:52.000000 glizzy_tls-0.1.0/glizzy_tls.egg-info/top_level.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 19:22:52.670602 glizzy_tls-0.1.0/setup.cfg
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1669 2023-06-11 19:21:01.000000 glizzy_tls-0.1.0/setup.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 20:57:46.244671 glizzy_tls-0.1.0b0/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-06-11 19:12:41.000000 glizzy_tls-0.1.0b0/LICENSE
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       56 2023-06-11 20:50:35.000000 glizzy_tls-0.1.0b0/MANIFEST.in
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5965 2023-06-11 20:57:46.244448 glizzy_tls-0.1.0b0/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5195 2023-06-11 19:38:56.000000 glizzy_tls-0.1.0b0/README.md
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 20:57:46.241152 glizzy_tls-0.1.0b0/glizzy_tls/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      200 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0b0/glizzy_tls/__init__.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 20:57:46.243866 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       27 2023-06-11 20:56:23.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/__init__.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1580 2023-06-11 20:54:44.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/build_go.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      531 2023-06-11 18:28:11.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/go.mod
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2175 2023-06-11 18:28:11.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/go.sum
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5104 2023-06-11 18:19:01.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/tls_client.go
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      264 2023-06-11 18:22:27.000000 glizzy_tls-0.1.0b0/glizzy_tls/exceptions.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1644 2023-06-11 18:36:50.000000 glizzy_tls-0.1.0b0/glizzy_tls/models.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1149 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0b0/glizzy_tls/request.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     4970 2023-06-11 20:56:28.000000 glizzy_tls-0.1.0b0/glizzy_tls/session.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 20:57:46.242114 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5965 2023-06-11 20:57:46.000000 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      459 2023-06-11 20:57:46.000000 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 20:57:46.000000 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2023-06-11 20:57:46.000000 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/top_level.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 20:57:46.244739 glizzy_tls-0.1.0b0/setup.cfg
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1332 2023-06-11 20:57:04.000000 glizzy_tls-0.1.0b0/setup.py
```

### Comparing `glizzy_tls-0.1.0/LICENSE` & `glizzy_tls-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0/PKG-INFO` & `glizzy_tls-0.1.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glizzy_tls
-Version: 0.1.0
+Version: 0.1.0b0
 Summary: A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.
 Home-page: https://github.com/glizzykingdreko/glizzy_tls
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Glizzy TLS
 
+![Banner](./image/logo.png)
+
 Glizzy TLS is a Python module that brings the power and flexibility of Go's TLS implementation to Python. It's designed to offer TLS (Transport Layer Security) capabilities in Python while taking advantage of the performance benefits of Go.
 
 ## Table of Contents
 - [Glizzy TLS](#glizzy-tls)
   - [Disclaimer](#disclaimer)
   - [What is TLS?](#what-is-tls)
   - [Why Glizzy TLS?](#why-glizzy-tls)
```

### Comparing `glizzy_tls-0.1.0/README.md` & `glizzy_tls-0.1.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Glizzy TLS
 
+![Banner](./image/logo.png)
+
 Glizzy TLS is a Python module that brings the power and flexibility of Go's TLS implementation to Python. It's designed to offer TLS (Transport Layer Security) capabilities in Python while taking advantage of the performance benefits of Go.
 
 ## Table of Contents
 - [Glizzy TLS](#glizzy-tls)
   - [Disclaimer](#disclaimer)
   - [What is TLS?](#what-is-tls)
   - [Why Glizzy TLS?](#why-glizzy-tls)
```

### Comparing `glizzy_tls-0.1.0/glizzy_tls/models.py` & `glizzy_tls-0.1.0b0/glizzy_tls/models.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0/glizzy_tls/request.py` & `glizzy_tls-0.1.0b0/glizzy_tls/request.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0/glizzy_tls/session.py` & `glizzy_tls-0.1.0b0/glizzy_tls/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from json import dumps
 from typing import Union
 import ctypes, os
 
 from .exceptions import ExceptionSendingRequest, MissingGlizzyTlsLibrary
 from .models import RequestDetails, Response
+from .dependencies import build
 
 # Load the shared library
+build()
 diectory = os.path.dirname(os.path.abspath(__file__))
 try: lib = ctypes.cdll.LoadLibrary(f"{diectory}/libraries/libtls_client.so")
 except OSError: raise MissingGlizzyTlsLibrary("Could not load the shared library")
 
 # Specify the argument types for the SendTlsRequest function
 lib.SendTlsRequest.argtypes = [
     ctypes.c_char_p,  # method
```

### Comparing `glizzy_tls-0.1.0/glizzy_tls.egg-info/PKG-INFO` & `glizzy_tls-0.1.0b0/glizzy_tls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glizzy-tls
-Version: 0.1.0
+Version: 0.1.0b0
 Summary: A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.
 Home-page: https://github.com/glizzykingdreko/glizzy_tls
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Glizzy TLS
 
+![Banner](./image/logo.png)
+
 Glizzy TLS is a Python module that brings the power and flexibility of Go's TLS implementation to Python. It's designed to offer TLS (Transport Layer Security) capabilities in Python while taking advantage of the performance benefits of Go.
 
 ## Table of Contents
 - [Glizzy TLS](#glizzy-tls)
   - [Disclaimer](#disclaimer)
   - [What is TLS?](#what-is-tls)
   - [Why Glizzy TLS?](#why-glizzy-tls)
```

### Comparing `glizzy_tls-0.1.0/setup.py` & `glizzy_tls-0.1.0b0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import subprocess
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-class PostInstallCommand(install):
-    """Post-installation for installation mode."""
-    def run(self):
-        try:
-            subprocess.check_call(['python', 'build_go.py'])
-        except subprocess.CalledProcessError as e:
-            print("Error building go files: ", e.output)
-            raise e
-        install.run(self)
-
 setup(
     name='glizzy_tls',
-    version='0.1.0',
+    version='0.1.0-b',
     description='A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/glizzykingdreko/glizzy_tls',
     author='glizzykingdreko',
     author_email='glizzykingdreko@protonmail.com',
     license='MIT',
     packages=find_packages(),
+    include_package_data=True, 
     install_requires=[
         # Add your python dependencies here
     ],
     package_data={
         # Include any files found in the 'libraries' directory:
-        'glizzy_tls': ['libraries/*'],
+        'glizzy_tls': ['dependencies/**/*', 'libraries/**/*'],
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    cmdclass={
-        'install': PostInstallCommand,
-    },
     python_requires='>=3.7',
 )
```

