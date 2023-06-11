# Comparing `tmp/ascii_chiper-0.1.3.tar.gz` & `tmp/ascii_chiper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii_chiper-0.1.3.tar", last modified: Sat Mar 25 13:58:54 2023, max compression
+gzip compressed data, was "ascii_chiper-0.1.4.tar", last modified: Sun Jun 11 00:08:48 2023, max compression
```

## Comparing `ascii_chiper-0.1.3.tar` & `ascii_chiper-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-03-25 13:58:54.369452 ascii_chiper-0.1.3/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-03-24 13:39:45.000000 ascii_chiper-0.1.3/LICENSE
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    11640 2023-03-25 13:58:54.368862 ascii_chiper-0.1.3/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    10793 2023-03-25 13:54:17.000000 ascii_chiper-0.1.3/README.md
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-03-25 13:58:54.366361 ascii_chiper-0.1.3/ascii_chiper/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      745 2023-03-24 15:44:38.000000 ascii_chiper-0.1.3/ascii_chiper/__init__.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    14184 2023-03-25 13:53:32.000000 ascii_chiper-0.1.3/ascii_chiper/chiper.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      730 2023-03-24 10:15:37.000000 ascii_chiper-0.1.3/ascii_chiper/exceptions.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1969 2023-03-23 21:35:42.000000 ascii_chiper-0.1.3/ascii_chiper/key_generator.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2342 2023-03-25 11:53:51.000000 ascii_chiper-0.1.3/ascii_chiper/models.py
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    12561 2023-03-24 19:42:27.000000 ascii_chiper-0.1.3/ascii_chiper/utils.py
-drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-03-25 13:58:54.368155 ascii_chiper-0.1.3/ascii_chiper.egg-info/
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)    11640 2023-03-25 13:58:54.000000 ascii_chiper-0.1.3/ascii_chiper.egg-info/PKG-INFO
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)      355 2023-03-25 13:58:54.000000 ascii_chiper-0.1.3/ascii_chiper.egg-info/SOURCES.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-03-25 13:58:54.000000 ascii_chiper-0.1.3/ascii_chiper.egg-info/dependency_links.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)        6 2023-03-25 13:58:54.000000 ascii_chiper-0.1.3/ascii_chiper.egg-info/requires.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       13 2023-03-25 13:58:54.000000 ascii_chiper-0.1.3/ascii_chiper.egg-info/top_level.txt
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-03-25 13:58:54.369567 ascii_chiper-0.1.3/setup.cfg
--rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1124 2023-03-25 13:57:53.000000 ascii_chiper-0.1.3/setup.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 00:08:48.812150 ascii_chiper-0.1.4/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1071 2023-03-24 13:39:45.000000 ascii_chiper-0.1.4/LICENSE
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    11640 2023-06-11 00:08:48.811555 ascii_chiper-0.1.4/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    10793 2023-06-10 23:52:22.000000 ascii_chiper-0.1.4/README.md
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 00:08:48.808438 ascii_chiper-0.1.4/ascii_chiper/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      745 2023-03-24 15:44:38.000000 ascii_chiper-0.1.4/ascii_chiper/__init__.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    14184 2023-03-25 13:53:32.000000 ascii_chiper-0.1.4/ascii_chiper/chiper.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      730 2023-03-24 10:15:37.000000 ascii_chiper-0.1.4/ascii_chiper/exceptions.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      771 2023-06-10 23:48:34.000000 ascii_chiper-0.1.4/ascii_chiper/helpers.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2081 2023-06-10 23:49:33.000000 ascii_chiper-0.1.4/ascii_chiper/key_generator.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     2342 2023-03-25 11:53:51.000000 ascii_chiper-0.1.4/ascii_chiper/models.py
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    12561 2023-03-25 19:22:04.000000 ascii_chiper-0.1.4/ascii_chiper/utils.py
+drwxr-xr-x   0 glizzykingdreko   (501) staff       (20)        0 2023-06-11 00:08:48.810700 ascii_chiper-0.1.4/ascii_chiper.egg-info/
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)    11640 2023-06-11 00:08:48.000000 ascii_chiper-0.1.4/ascii_chiper.egg-info/PKG-INFO
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)      379 2023-06-11 00:08:48.000000 ascii_chiper-0.1.4/ascii_chiper.egg-info/SOURCES.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)        1 2023-06-11 00:08:48.000000 ascii_chiper-0.1.4/ascii_chiper.egg-info/dependency_links.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)        6 2023-06-11 00:08:48.000000 ascii_chiper-0.1.4/ascii_chiper.egg-info/requires.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       13 2023-06-11 00:08:48.000000 ascii_chiper-0.1.4/ascii_chiper.egg-info/top_level.txt
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)       38 2023-06-11 00:08:48.812333 ascii_chiper-0.1.4/setup.cfg
+-rw-r--r--   0 glizzykingdreko   (501) staff       (20)     1124 2023-06-11 00:01:32.000000 ascii_chiper-0.1.4/setup.py
```

### Comparing `ascii_chiper-0.1.3/LICENSE` & `ascii_chiper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii_chiper-0.1.3/PKG-INFO` & `ascii_chiper-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii_chiper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A versatile Python module for encrypting and decrypting strings, integers, and dictionaries using a variety of encryption techniques.
 Home-page: https://github.com/glizzykingdreko/ascii_chiper
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ascii_chiper
-`ascii_chiper `is a Python module for encrypting and decrypting strings, integers, and dictionaries using various encryption techniques. The module provides user-friendly and customizable encryption configurations to suit different use cases and levels of security.
+`ascii_chiper` is a Python module for encrypting and decrypting strings, integers, and dictionaries using various encryption techniques. The module provides user-friendly and customizable encryption configurations to suit different use cases and levels of security.
 
 ## Features
 - Accepts strings, integers, floats, lists and dictionaries as input for encryption
 - Supports multiple encryption techniques, including swapping, XOR shifting, interleaving, rotation, XOR base, XOR addition, and interleaving with key
 - Offers pre-configured encryption configurations for quick use
 - Allows users to create custom encryption configurations
```

### Comparing `ascii_chiper-0.1.3/README.md` & `ascii_chiper-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ascii_chiper
-`ascii_chiper `is a Python module for encrypting and decrypting strings, integers, and dictionaries using various encryption techniques. The module provides user-friendly and customizable encryption configurations to suit different use cases and levels of security.
+`ascii_chiper` is a Python module for encrypting and decrypting strings, integers, and dictionaries using various encryption techniques. The module provides user-friendly and customizable encryption configurations to suit different use cases and levels of security.
 
 ## Features
 - Accepts strings, integers, floats, lists and dictionaries as input for encryption
 - Supports multiple encryption techniques, including swapping, XOR shifting, interleaving, rotation, XOR base, XOR addition, and interleaving with key
 - Offers pre-configured encryption configurations for quick use
 - Allows users to create custom encryption configurations
```

### Comparing `ascii_chiper-0.1.3/ascii_chiper/__init__.py` & `ascii_chiper-0.1.4/ascii_chiper/__init__.py`

 * *Files identical despite different names*

### Comparing `ascii_chiper-0.1.3/ascii_chiper/chiper.py` & `ascii_chiper-0.1.4/ascii_chiper/chiper.py`

 * *Files identical despite different names*

### Comparing `ascii_chiper-0.1.3/ascii_chiper/exceptions.py` & `ascii_chiper-0.1.4/ascii_chiper/exceptions.py`

 * *Files identical despite different names*

### Comparing `ascii_chiper-0.1.3/ascii_chiper/models.py` & `ascii_chiper-0.1.4/ascii_chiper/models.py`

 * *Files identical despite different names*

### Comparing `ascii_chiper-0.1.3/ascii_chiper/utils.py` & `ascii_chiper-0.1.4/ascii_chiper/utils.py`

 * *Files identical despite different names*

### Comparing `ascii_chiper-0.1.3/ascii_chiper.egg-info/PKG-INFO` & `ascii_chiper-0.1.4/ascii_chiper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-chiper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A versatile Python module for encrypting and decrypting strings, integers, and dictionaries using a variety of encryption techniques.
 Home-page: https://github.com/glizzykingdreko/ascii_chiper
 Author: glizzykingdreko
 Author-email: glizzykingdreko@protonmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ascii_chiper
-`ascii_chiper `is a Python module for encrypting and decrypting strings, integers, and dictionaries using various encryption techniques. The module provides user-friendly and customizable encryption configurations to suit different use cases and levels of security.
+`ascii_chiper` is a Python module for encrypting and decrypting strings, integers, and dictionaries using various encryption techniques. The module provides user-friendly and customizable encryption configurations to suit different use cases and levels of security.
 
 ## Features
 - Accepts strings, integers, floats, lists and dictionaries as input for encryption
 - Supports multiple encryption techniques, including swapping, XOR shifting, interleaving, rotation, XOR base, XOR addition, and interleaving with key
 - Offers pre-configured encryption configurations for quick use
 - Allows users to create custom encryption configurations
```

### Comparing `ascii_chiper-0.1.3/setup.py` & `ascii_chiper-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ascii_chiper",
-    version="0.1.3",
+    version="0.1.4",
     author="glizzykingdreko",
     author_email="glizzykingdreko@protonmail.com",
     description="A versatile Python module for encrypting and decrypting strings, integers, and dictionaries using a variety of encryption techniques.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/glizzykingdreko/ascii_chiper",
     packages=find_packages(),
```

