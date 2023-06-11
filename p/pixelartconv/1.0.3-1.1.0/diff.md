# Comparing `tmp/pixelartconv-1.0.3.tar.gz` & `tmp/pixelartconv-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelartconv-1.0.3.tar", last modified: Wed Feb  8 14:48:35 2023, max compression
+gzip compressed data, was "pixelartconv-1.1.0.tar", last modified: Sun Jun 11 20:21:17 2023, max compression
```

## Comparing `pixelartconv-1.0.3.tar` & `pixelartconv-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-02-08 14:48:35.700642 pixelartconv-1.0.3/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-02-08 14:48:35.700642 pixelartconv-1.0.3/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)     3433 2023-02-08 14:41:43.000000 pixelartconv-1.0.3/README.md
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-02-08 14:48:35.700642 pixelartconv-1.0.3/pixelartconv/
--rw-r--r--   0 simon     (1000) simon     (1000)       73 2023-02-08 13:22:29.000000 pixelartconv-1.0.3/pixelartconv/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1001 2023-02-08 14:23:05.000000 pixelartconv-1.0.3/pixelartconv/__main__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     4991 2023-02-08 12:20:35.000000 pixelartconv-1.0.3/pixelartconv/file_management.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     3189 2023-02-08 11:50:28.000000 pixelartconv-1.0.3/pixelartconv/logic.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1656 2023-02-08 14:23:05.000000 pixelartconv-1.0.3/pixelartconv/script.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-02-08 14:48:35.700642 pixelartconv-1.0.3/pixelartconv.egg-info/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-02-08 14:48:35.000000 pixelartconv-1.0.3/pixelartconv.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)      340 2023-02-08 14:48:35.000000 pixelartconv-1.0.3/pixelartconv.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-02-08 14:48:35.000000 pixelartconv-1.0.3/pixelartconv.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       33 2023-02-08 14:48:35.000000 pixelartconv-1.0.3/pixelartconv.egg-info/requires.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       13 2023-02-08 14:48:35.000000 pixelartconv-1.0.3/pixelartconv.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)      525 2023-02-08 14:47:53.000000 pixelartconv-1.0.3/pyproject.toml
--rw-rw-r--   0 simon     (1000) simon     (1000)      135 2023-02-08 14:48:35.700642 pixelartconv-1.0.3/setup.cfg
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3433 2023-02-08 14:41:43.000000 pixelartconv-1.1.0/README.md
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/pixelartconv/
+-rw-r--r--   0 simon     (1000) simon     (1000)       73 2023-02-08 13:22:29.000000 pixelartconv-1.1.0/pixelartconv/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1050 2023-06-11 20:20:52.000000 pixelartconv-1.1.0/pixelartconv/__main__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5167 2023-06-11 17:08:43.000000 pixelartconv-1.1.0/pixelartconv/file_management.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4156 2023-06-11 20:17:04.000000 pixelartconv-1.1.0/pixelartconv/logic.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1752 2023-06-11 17:09:50.000000 pixelartconv-1.1.0/pixelartconv/script.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/pixelartconv.egg-info/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)      340 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       37 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       13 2023-06-11 20:21:17.000000 pixelartconv-1.1.0/pixelartconv.egg-info/top_level.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      525 2023-06-11 20:19:48.000000 pixelartconv-1.1.0/pyproject.toml
+-rw-rw-r--   0 simon     (1000) simon     (1000)      140 2023-06-11 20:21:17.248993 pixelartconv-1.1.0/setup.cfg
```

### Comparing `pixelartconv-1.0.3/PKG-INFO` & `pixelartconv-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelartconv
-Version: 1.0.3
+Version: 1.1.0
 Summary: PixelArtConv - Pixel Art Converter
 Author-email: Simon Ruzicka <sima.ruzicka@gmail.com>
 Project-URL: Homepage, https://github.com/ruzicka02/paconv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `pixelartconv-1.0.3/README.md` & `pixelartconv-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pixelartconv-1.0.3/pixelartconv/__main__.py` & `pixelartconv-1.1.0/pixelartconv/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import sys
 from pathlib import Path
 
 import pixelartconv.script
 
+print(pixelartconv.__path__)
+
 more_info = "For more info, type:\n    python -m pixelartconv --help"
 
 if len(sys.argv) not in [2, 3, 4]:
     print("""Invalid syntax, please use one of the following:
     python -m pixelartconv [file_name]
     python -m pixelartconv [file_name] [width] [height]
     """)
     print(more_info)
     sys.exit(1)
 
 file_name = sys.argv[1]
-height = int(sys.argv[2]) if len(sys.argv) > 2 else 16
+height = int(sys.argv[2]) if len(sys.argv) > 2 else 64
 width = int(sys.argv[3]) if len(sys.argv) > 3 else None  # else... will be calculated when image is loaded
 dims = (width, height)
 
-if file_name == "--help":
+if "--help" in sys.argv or "-h" in sys.argv:
     path = (Path(__file__).parent / "help.txt").resolve()
     with open(path) as f:
         print(f.read())
     sys.exit(2)
 
 if file_name[0] == '-':
     print("Unknown command option.")
```

### Comparing `pixelartconv-1.0.3/pixelartconv/file_management.py` & `pixelartconv-1.1.0/pixelartconv/file_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,25 +34,26 @@
     assert image.shape == (dims[1], dims[0], 3), "Issues encountered when converting image to matrix."
 
     return image
 
 
 def load_image(name: str, dims: tuple):
     """
-    Loads a PNG image from the current path, performs various operations
+    Loads an image from the current path, performs various operations
     and returns it as an array. In case something goes wrong, raises an exception.
 
     :param str name: File name.
     :param tuple dims: Pair of target image dimensions (width, height).
     :return: Image as a numpy.ndarray
     :raise FileNotFoundError: Image not found on given path.
     :raise ValueError: File with this name was found but was invalid.
     """
-    if name[-4:] != ".png":
+    if "." not in name:  # add .png suffix if image has no suffix
         name += ".png"
+    
     path = (Path() / name).resolve()
 
     if not path.is_file():
         raise FileNotFoundError(f"File not found at searched address: {path}")
 
     try:
         image = image_prepare(path, dims)
@@ -70,16 +71,16 @@
     to which file has been saved.
 
     :param np.ndarray data: Source image data.
     :param bool show: EXPERIMENTAL - Shows the image with built-in Pillow function when set as True.
     :param str name: File name.
     :return: Resulting file path.
     """
-    if name[-4:] == ".png":
-        name = name[:-4]
+    if "." in name:  # strip the current suffix (expected .png)
+        name = ".".join(name.split(".")[:-1])
 
     path = (Path() / (name + ".png")).resolve()
     name = name.split("/")[-1]  # remove potential directories in path
 
     image = Image.fromarray(np.uint8(data)).convert('RGB')
     image.save(path)
 
@@ -102,16 +103,18 @@
 
     :param str name: File name (or path).
     :return: List of tuples - (r, g, b).
     :raise FileNotFoundError: When file with given name/path is not found.
     :raise ValueError: File with this name was found but was invalid.
     """
 
-    if name[-4:] != ".txt":
-        name += ".txt"
+    if "." in name:  # strip the current suffix (expected .png)
+        name = ".".join(name.split(".")[:-1])
+    name += ".txt"
+
     path = (Path() / name).resolve()
 
     if not path.is_file():
         raise FileNotFoundError(f"File not found at searched address: {path}")
 
     with open(path, 'r') as file:
         lines = [line.rstrip().lstrip('#') for line in file]
```

### Comparing `pixelartconv-1.0.3/pixelartconv/script.py` & `pixelartconv-1.1.0/pixelartconv/script.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,29 @@
     :param palette_size: Amount of colors in case the palette has to be generated.
     :return: Time duration of conversion (seconds).
     :raise FileNotFoundError: Image not found on given path.
     :raise ValueError: File with this name was found but was invalid.
     """
     start_time = time()
 
-    print(f"Searched path is: {(Path().absolute() / Path(file_name)).parent.resolve()}")
+    print(f"Searched path is: {(Path().absolute() / Path(file_name)).resolve()}")
 
     try:
         img = file_management.load_image(file_name, dims)
     except (ValueError, FileNotFoundError) as err:
         print(err)
         print("For more info, type:\n    python -m pixelartconv --help")
         raise
 
     try:
         colors = file_management.load_colors(file_name)
+        print("Colors loaded from a text file")
     except FileNotFoundError:
         colors = file_management.generate_colors(file_name, color_count=palette_size)
+        print("Colors autogenerated using Colorthief")
     except ValueError as err:
         print(err)
         print("For more info, type:\n    python -m pixelartconv --help\nFallback to generated color palette...")
         colors = file_management.generate_colors(file_name, color_count=palette_size)
         # raise
 
     res = logic.convert_img(img, colors)
```

### Comparing `pixelartconv-1.0.3/pixelartconv.egg-info/PKG-INFO` & `pixelartconv-1.1.0/pixelartconv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelartconv
-Version: 1.0.3
+Version: 1.1.0
 Summary: PixelArtConv - Pixel Art Converter
 Author-email: Simon Ruzicka <sima.ruzicka@gmail.com>
 Project-URL: Homepage, https://github.com/ruzicka02/paconv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `pixelartconv-1.0.3/pyproject.toml` & `pixelartconv-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pixelartconv"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="Simon Ruzicka", email="sima.ruzicka@gmail.com" },
 ]
 description = "PixelArtConv - Pixel Art Converter"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

