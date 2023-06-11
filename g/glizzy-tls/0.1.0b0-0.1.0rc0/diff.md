# Comparing `tmp/glizzy_tls-0.1.0b0.tar.gz` & `tmp/glizzy_tls-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glizzy_tls-0.1.0b0.tar", last modified: Sun Jun 11 20:57:46 2023, max compression
+gzip compressed data, was "glizzy_tls-0.1.0rc0.tar", last modified: Sun Jun 11 21:01:21 2023, max compression
```

## Comparing `glizzy_tls-0.1.0b0.tar` & `glizzy_tls-0.1.0rc0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 20:57:46.244671 glizzy_tls-0.1.0b0/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-06-11 19:12:41.000000 glizzy_tls-0.1.0b0/LICENSE
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       56 2023-06-11 20:50:35.000000 glizzy_tls-0.1.0b0/MANIFEST.in
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5965 2023-06-11 20:57:46.244448 glizzy_tls-0.1.0b0/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5195 2023-06-11 19:38:56.000000 glizzy_tls-0.1.0b0/README.md
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 20:57:46.241152 glizzy_tls-0.1.0b0/glizzy_tls/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      200 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0b0/glizzy_tls/__init__.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 20:57:46.243866 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       27 2023-06-11 20:56:23.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/__init__.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1580 2023-06-11 20:54:44.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/build_go.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      531 2023-06-11 18:28:11.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/go.mod
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2175 2023-06-11 18:28:11.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/go.sum
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5104 2023-06-11 18:19:01.000000 glizzy_tls-0.1.0b0/glizzy_tls/dependencies/tls_client.go
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      264 2023-06-11 18:22:27.000000 glizzy_tls-0.1.0b0/glizzy_tls/exceptions.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1644 2023-06-11 18:36:50.000000 glizzy_tls-0.1.0b0/glizzy_tls/models.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1149 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0b0/glizzy_tls/request.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     4970 2023-06-11 20:56:28.000000 glizzy_tls-0.1.0b0/glizzy_tls/session.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 20:57:46.242114 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5965 2023-06-11 20:57:46.000000 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      459 2023-06-11 20:57:46.000000 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/SOURCES.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 20:57:46.000000 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/dependency_links.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2023-06-11 20:57:46.000000 glizzy_tls-0.1.0b0/glizzy_tls.egg-info/top_level.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 20:57:46.244739 glizzy_tls-0.1.0b0/setup.cfg
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1332 2023-06-11 20:57:04.000000 glizzy_tls-0.1.0b0/setup.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:01:21.012296 glizzy_tls-0.1.0rc0/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-06-11 19:12:41.000000 glizzy_tls-0.1.0rc0/LICENSE
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       56 2023-06-11 20:50:35.000000 glizzy_tls-0.1.0rc0/MANIFEST.in
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6096 2023-06-11 21:01:21.012101 glizzy_tls-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5325 2023-06-11 21:00:56.000000 glizzy_tls-0.1.0rc0/README.md
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:01:21.008985 glizzy_tls-0.1.0rc0/glizzy_tls/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      200 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0rc0/glizzy_tls/__init__.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:01:21.011697 glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       27 2023-06-11 20:56:23.000000 glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/__init__.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1580 2023-06-11 20:54:44.000000 glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/build_go.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      531 2023-06-11 18:28:11.000000 glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/go.mod
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2175 2023-06-11 18:28:11.000000 glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/go.sum
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     5104 2023-06-11 18:19:01.000000 glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/tls_client.go
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      264 2023-06-11 18:22:27.000000 glizzy_tls-0.1.0rc0/glizzy_tls/exceptions.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1644 2023-06-11 18:36:50.000000 glizzy_tls-0.1.0rc0/glizzy_tls/models.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1149 2023-06-11 18:58:24.000000 glizzy_tls-0.1.0rc0/glizzy_tls/request.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     4970 2023-06-11 20:56:28.000000 glizzy_tls-0.1.0rc0/glizzy_tls/session.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 21:01:21.009935 glizzy_tls-0.1.0rc0/glizzy_tls.egg-info/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     6096 2023-06-11 21:01:20.000000 glizzy_tls-0.1.0rc0/glizzy_tls.egg-info/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      459 2023-06-11 21:01:20.000000 glizzy_tls-0.1.0rc0/glizzy_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 21:01:20.000000 glizzy_tls-0.1.0rc0/glizzy_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       11 2023-06-11 21:01:20.000000 glizzy_tls-0.1.0rc0/glizzy_tls.egg-info/top_level.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 21:01:21.012351 glizzy_tls-0.1.0rc0/setup.cfg
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1332 2023-06-11 21:01:06.000000 glizzy_tls-0.1.0rc0/setup.py
```

### Comparing `glizzy_tls-0.1.0b0/LICENSE` & `glizzy_tls-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0b0/PKG-INFO` & `glizzy_tls-0.1.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glizzy_tls
-Version: 0.1.0b0
+Version: 0.1.0rc0
 Summary: A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.
 Home-page: https://github.com/glizzykingdreko/glizzy_tls
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,18 @@
 
 # Glizzy TLS
 
 ![Banner](./image/logo.png)
 
 Glizzy TLS is a Python module that brings the power and flexibility of Go's TLS implementation to Python. It's designed to offer TLS (Transport Layer Security) capabilities in Python while taking advantage of the performance benefits of Go.
 
-## Table of Contents
+
+## Table of Contents
 - [Glizzy TLS](#glizzy-tls)
+  - [Table of Contents](#table-of-contents)
   - [Disclaimer](#disclaimer)
   - [What is TLS?](#what-is-tls)
   - [Why Glizzy TLS?](#why-glizzy-tls)
   - [How is it done?](#how-is-it-done)
   - [Installation](#installation)
   - [Example Usage](#example-usage)
     - [Session Objects](#session-objects)
@@ -40,14 +42,16 @@
   - [License](#license)
   - [Contact Me](#contact-me)
   
 
 ## Disclaimer
 This is a first implementation of TLS in python for non supported platforms from other modules. I've quickly done it for a project I'm working on. I'll improve it by adding more features as soon as I can.
 
+Check out the [source code on GitHub](https://github.com/glizzykingdreko/Glizzy-TLS)
+
 ## What is TLS?
 
 Transport Layer Security (TLS) is a protocol that provides privacy and data integrity between two communicating applications. It's used for web browsers and other applications that require data to be securely exchanged over a network.
 
 ## Why Glizzy TLS?
 
 While there are existing Python libraries for TLS, they can sometimes fall short in terms of performance and compatibility. Go has a robust and performant TLS library, and by compiling Go code to a shared object (`.so`) file and interfacing with it using CPython's `ctypes` library, Glizzy TLS brings this power to Python.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `glizzy_tls-0.1.0b0/README.md` & `glizzy_tls-0.1.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Glizzy TLS
 
 ![Banner](./image/logo.png)
 
 Glizzy TLS is a Python module that brings the power and flexibility of Go's TLS implementation to Python. It's designed to offer TLS (Transport Layer Security) capabilities in Python while taking advantage of the performance benefits of Go.
 
-## Table of Contents
+
+## Table of Contents
 - [Glizzy TLS](#glizzy-tls)
+  - [Table of Contents](#table-of-contents)
   - [Disclaimer](#disclaimer)
   - [What is TLS?](#what-is-tls)
   - [Why Glizzy TLS?](#why-glizzy-tls)
   - [How is it done?](#how-is-it-done)
   - [Installation](#installation)
   - [Example Usage](#example-usage)
     - [Session Objects](#session-objects)
@@ -20,14 +22,16 @@
   - [License](#license)
   - [Contact Me](#contact-me)
   
 
 ## Disclaimer
 This is a first implementation of TLS in python for non supported platforms from other modules. I've quickly done it for a project I'm working on. I'll improve it by adding more features as soon as I can.
 
+Check out the [source code on GitHub](https://github.com/glizzykingdreko/Glizzy-TLS)
+
 ## What is TLS?
 
 Transport Layer Security (TLS) is a protocol that provides privacy and data integrity between two communicating applications. It's used for web browsers and other applications that require data to be securely exchanged over a network.
 
 ## Why Glizzy TLS?
 
 While there are existing Python libraries for TLS, they can sometimes fall short in terms of performance and compatibility. Go has a robust and performant TLS library, and by compiling Go code to a shared object (`.so`) file and interfacing with it using CPython's `ctypes` library, Glizzy TLS brings this power to Python.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `glizzy_tls-0.1.0b0/glizzy_tls/dependencies/build_go.py` & `glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/build_go.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0b0/glizzy_tls/dependencies/go.mod` & `glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/go.mod`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0b0/glizzy_tls/dependencies/go.sum` & `glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/go.sum`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0b0/glizzy_tls/dependencies/tls_client.go` & `glizzy_tls-0.1.0rc0/glizzy_tls/dependencies/tls_client.go`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0b0/glizzy_tls/models.py` & `glizzy_tls-0.1.0rc0/glizzy_tls/models.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0b0/glizzy_tls/request.py` & `glizzy_tls-0.1.0rc0/glizzy_tls/request.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0b0/glizzy_tls/session.py` & `glizzy_tls-0.1.0rc0/glizzy_tls/session.py`

 * *Files identical despite different names*

### Comparing `glizzy_tls-0.1.0b0/glizzy_tls.egg-info/PKG-INFO` & `glizzy_tls-0.1.0rc0/glizzy_tls.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glizzy-tls
-Version: 0.1.0b0
+Version: 0.1.0rc0
 Summary: A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.
 Home-page: https://github.com/glizzykingdreko/glizzy_tls
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,18 @@
 
 # Glizzy TLS
 
 ![Banner](./image/logo.png)
 
 Glizzy TLS is a Python module that brings the power and flexibility of Go's TLS implementation to Python. It's designed to offer TLS (Transport Layer Security) capabilities in Python while taking advantage of the performance benefits of Go.
 
-## Table of Contents
+
+## Table of Contents
 - [Glizzy TLS](#glizzy-tls)
+  - [Table of Contents](#table-of-contents)
   - [Disclaimer](#disclaimer)
   - [What is TLS?](#what-is-tls)
   - [Why Glizzy TLS?](#why-glizzy-tls)
   - [How is it done?](#how-is-it-done)
   - [Installation](#installation)
   - [Example Usage](#example-usage)
     - [Session Objects](#session-objects)
@@ -40,14 +42,16 @@
   - [License](#license)
   - [Contact Me](#contact-me)
   
 
 ## Disclaimer
 This is a first implementation of TLS in python for non supported platforms from other modules. I've quickly done it for a project I'm working on. I'll improve it by adding more features as soon as I can.
 
+Check out the [source code on GitHub](https://github.com/glizzykingdreko/Glizzy-TLS)
+
 ## What is TLS?
 
 Transport Layer Security (TLS) is a protocol that provides privacy and data integrity between two communicating applications. It's used for web browsers and other applications that require data to be securely exchanged over a network.
 
 ## Why Glizzy TLS?
 
 While there are existing Python libraries for TLS, they can sometimes fall short in terms of performance and compatibility. Go has a robust and performant TLS library, and by compiling Go code to a shared object (`.so`) file and interfacing with it using CPython's `ctypes` library, Glizzy TLS brings this power to Python.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `glizzy_tls-0.1.0b0/setup.py` & `glizzy_tls-0.1.0rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='glizzy_tls',
-    version='0.1.0-b',
+    version='0.1.0-c',
     description='A fully open-source, cross-platform TLS implementation in Python, leveraging GoLang.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/glizzykingdreko/glizzy_tls',
     author='glizzykingdreko',
     author_email='glizzykingdreko@protonmail.com',
     license='MIT',
```

