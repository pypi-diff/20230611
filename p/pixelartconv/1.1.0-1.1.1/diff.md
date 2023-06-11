# Comparing `tmp/pixelartconv-1.1.0.tar.gz` & `tmp/pixelartconv-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelartconv-1.1.0.tar", last modified: Sun Jun 11 20:21:17 2023, max compression
+gzip compressed data, was "pixelartconv-1.1.1.tar", last modified: Sun Jun 11 20:36:52 2023, max compression
```

## Comparing `pixelartconv-1.1.0.tar` & `pixelartconv-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)     3433 2023-02-08 14:41:43.000000 pixelartconv-1.1.0/README.md
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/pixelartconv/
--rw-r--r--   0 simon     (1000) simon     (1000)       73 2023-02-08 13:22:29.000000 pixelartconv-1.1.0/pixelartconv/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1050 2023-06-11 20:20:52.000000 pixelartconv-1.1.0/pixelartconv/__main__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     5167 2023-06-11 17:08:43.000000 pixelartconv-1.1.0/pixelartconv/file_management.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     4156 2023-06-11 20:17:04.000000 pixelartconv-1.1.0/pixelartconv/logic.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1752 2023-06-11 17:09:50.000000 pixelartconv-1.1.0/pixelartconv/script.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/pixelartconv.egg-info/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)      340 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       37 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/requires.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       13 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)      525 2023-06-11 20:19:48.000000 pixelartconv-1.1.0/pyproject.toml
--rw-rw-r--   0 simon     (1000) simon     (1000)      140 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/setup.cfg
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3433 2023-06-11 20:24:18.000000 pixelartconv-1.1.1/README.md
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/pixelartconv/
+-rw-r--r--   0 simon     (1000) simon     (1000)       73 2023-02-08 13:22:29.000000 pixelartconv-1.1.1/pixelartconv/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1050 2023-06-11 20:20:52.000000 pixelartconv-1.1.1/pixelartconv/__main__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5167 2023-06-11 17:08:43.000000 pixelartconv-1.1.1/pixelartconv/file_management.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4156 2023-06-11 20:17:04.000000 pixelartconv-1.1.1/pixelartconv/logic.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1752 2023-06-11 17:09:50.000000 pixelartconv-1.1.1/pixelartconv/script.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/pixelartconv.egg-info/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)      340 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       47 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       13 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/top_level.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      525 2023-06-11 20:36:32.000000 pixelartconv-1.1.1/pyproject.toml
+-rw-rw-r--   0 simon     (1000) simon     (1000)      150 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/setup.cfg
```

### Comparing `pixelartconv-1.1.0/PKG-INFO` & `pixelartconv-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelartconv
-Version: 1.1.0
+Version: 1.1.1
 Summary: PixelArtConv - Pixel Art Converter
 Author-email: Simon Ruzicka <sima.ruzicka@gmail.com>
 Project-URL: Homepage, https://github.com/ruzicka02/paconv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -59,15 +59,15 @@
 ```
 python -m pixelartconv [file_name]
 python -m pixelartconv [file_name] [height]
 python -m pixelartconv [file_name] [height] [width]
 ```
 
 The behavior of script is as follows:
-1) The resulting image will be 16 px in height - width will be automatically calculated from the original image ratio.
+1) The resulting image will be 64 px in height - width will be automatically calculated from the original image ratio.
 2) The resulting image will have given height - width will be automatically calculated from the original image ratio.
 3) The resulting image will have given height and width.
 
 ### Imported package
 
 Additionally, you can import the package from your code/interactive shell and use the `convert` function with following interface:
```

### Comparing `pixelartconv-1.1.0/README.md` & `pixelartconv-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ```
 python -m pixelartconv [file_name]
 python -m pixelartconv [file_name] [height]
 python -m pixelartconv [file_name] [height] [width]
 ```
 
 The behavior of script is as follows:
-1) The resulting image will be 16 px in height - width will be automatically calculated from the original image ratio.
+1) The resulting image will be 64 px in height - width will be automatically calculated from the original image ratio.
 2) The resulting image will have given height - width will be automatically calculated from the original image ratio.
 3) The resulting image will have given height and width.
 
 ### Imported package
 
 Additionally, you can import the package from your code/interactive shell and use the `convert` function with following interface:
```

### Comparing `pixelartconv-1.1.0/pixelartconv/__main__.py` & `pixelartconv-1.1.1/pixelartconv/__main__.py`

 * *Files identical despite different names*

### Comparing `pixelartconv-1.1.0/pixelartconv/file_management.py` & `pixelartconv-1.1.1/pixelartconv/file_management.py`

 * *Files identical despite different names*

### Comparing `pixelartconv-1.1.0/pixelartconv/logic.py` & `pixelartconv-1.1.1/pixelartconv/logic.py`

 * *Files identical despite different names*

### Comparing `pixelartconv-1.1.0/pixelartconv/script.py` & `pixelartconv-1.1.1/pixelartconv/script.py`

 * *Files identical despite different names*

### Comparing `pixelartconv-1.1.0/pixelartconv.egg-info/PKG-INFO` & `pixelartconv-1.1.1/pixelartconv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelartconv
-Version: 1.1.0
+Version: 1.1.1
 Summary: PixelArtConv - Pixel Art Converter
 Author-email: Simon Ruzicka <sima.ruzicka@gmail.com>
 Project-URL: Homepage, https://github.com/ruzicka02/paconv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -59,15 +59,15 @@
 ```
 python -m pixelartconv [file_name]
 python -m pixelartconv [file_name] [height]
 python -m pixelartconv [file_name] [height] [width]
 ```
 
 The behavior of script is as follows:
-1) The resulting image will be 16 px in height - width will be automatically calculated from the original image ratio.
+1) The resulting image will be 64 px in height - width will be automatically calculated from the original image ratio.
 2) The resulting image will have given height - width will be automatically calculated from the original image ratio.
 3) The resulting image will have given height and width.
 
 ### Imported package
 
 Additionally, you can import the package from your code/interactive shell and use the `convert` function with following interface:
```

### Comparing `pixelartconv-1.1.0/pyproject.toml` & `pixelartconv-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pixelartconv"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Simon Ruzicka", email="sima.ruzicka@gmail.com" },
 ]
 description = "PixelArtConv - Pixel Art Converter"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

