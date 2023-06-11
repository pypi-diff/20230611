# Comparing `tmp/pixelartconv-1.1.1.tar.gz` & `tmp/pixelartconv-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelartconv-1.1.1.tar", last modified: Sun Jun 11 20:36:52 2023, max compression
+gzip compressed data, was "pixelartconv-1.1.2.tar", last modified: Sun Jun 11 21:46:38 2023, max compression
```

## Comparing `pixelartconv-1.1.1.tar` & `pixelartconv-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)     3433 2023-06-11 20:24:18.000000 pixelartconv-1.1.1/README.md
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/pixelartconv/
--rw-r--r--   0 simon     (1000) simon     (1000)       73 2023-02-08 13:22:29.000000 pixelartconv-1.1.1/pixelartconv/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1050 2023-06-11 20:20:52.000000 pixelartconv-1.1.1/pixelartconv/__main__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     5167 2023-06-11 17:08:43.000000 pixelartconv-1.1.1/pixelartconv/file_management.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     4156 2023-06-11 20:17:04.000000 pixelartconv-1.1.1/pixelartconv/logic.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1752 2023-06-11 17:09:50.000000 pixelartconv-1.1.1/pixelartconv/script.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/pixelartconv.egg-info/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)      340 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       47 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/requires.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       13 2023-06-11 20:36:52.000000 pixelartconv-1.1.1/pixelartconv.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)      525 2023-06-11 20:36:32.000000 pixelartconv-1.1.1/pyproject.toml
--rw-rw-r--   0 simon     (1000) simon     (1000)      150 2023-06-11 20:36:52.489938 pixelartconv-1.1.1/setup.cfg
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 21:46:38.090834 pixelartconv-1.1.2/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 21:46:38.090834 pixelartconv-1.1.2/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3433 2023-06-11 20:24:18.000000 pixelartconv-1.1.2/README.md
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 21:46:38.090834 pixelartconv-1.1.2/pixelartconv/
+-rw-r--r--   0 simon     (1000) simon     (1000)       73 2023-02-08 13:22:29.000000 pixelartconv-1.1.2/pixelartconv/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1020 2023-06-11 21:30:22.000000 pixelartconv-1.1.2/pixelartconv/__main__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5214 2023-06-11 21:41:38.000000 pixelartconv-1.1.2/pixelartconv/file_management.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3909 2023-06-11 21:31:23.000000 pixelartconv-1.1.2/pixelartconv/logic.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1752 2023-06-11 17:09:50.000000 pixelartconv-1.1.2/pixelartconv/script.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-06-11 21:46:38.090834 pixelartconv-1.1.2/pixelartconv.egg-info/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3855 2023-06-11 21:46:38.000000 pixelartconv-1.1.2/pixelartconv.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)      340 2023-06-11 21:46:38.000000 pixelartconv-1.1.2/pixelartconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-06-11 21:46:38.000000 pixelartconv-1.1.2/pixelartconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       47 2023-06-11 21:46:38.000000 pixelartconv-1.1.2/pixelartconv.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       13 2023-06-11 21:46:38.000000 pixelartconv-1.1.2/pixelartconv.egg-info/top_level.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      525 2023-06-11 21:42:03.000000 pixelartconv-1.1.2/pyproject.toml
+-rw-rw-r--   0 simon     (1000) simon     (1000)      150 2023-06-11 21:46:38.094835 pixelartconv-1.1.2/setup.cfg
```

### Comparing `pixelartconv-1.1.1/PKG-INFO` & `pixelartconv-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelartconv
-Version: 1.1.1
+Version: 1.1.2
 Summary: PixelArtConv - Pixel Art Converter
 Author-email: Simon Ruzicka <sima.ruzicka@gmail.com>
 Project-URL: Homepage, https://github.com/ruzicka02/paconv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `pixelartconv-1.1.1/README.md` & `pixelartconv-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pixelartconv-1.1.1/pixelartconv/__main__.py` & `pixelartconv-1.1.2/pixelartconv/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import sys
 from pathlib import Path
 
 import pixelartconv.script
 
-print(pixelartconv.__path__)
-
 more_info = "For more info, type:\n    python -m pixelartconv --help"
 
 if len(sys.argv) not in [2, 3, 4]:
     print("""Invalid syntax, please use one of the following:
     python -m pixelartconv [file_name]
     python -m pixelartconv [file_name] [width] [height]
     """)
```

### Comparing `pixelartconv-1.1.1/pixelartconv/file_management.py` & `pixelartconv-1.1.2/pixelartconv/file_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,16 +136,17 @@
     :param str name: File name (or path).
     :param int color_count: Amount of colors to be generated.
     :return: List of tuples - (r, g, b).
     :raise FileNotFoundError: When image with given name/path is not found.
     :raise ValueError: Image with this name was found but was invalid.
     """
 
-    if name[-4:] != ".png":
+    if "." not in name:  # add .png suffix if image has no suffix
         name += ".png"
+        
     path = (Path() / name).resolve()
 
     if not path.is_file():
         raise FileNotFoundError(f"File not found at searched address: {path}")
 
     try:
         color_thief = ColorThief(path)
```

### Comparing `pixelartconv-1.1.1/pixelartconv/logic.py` & `pixelartconv-1.1.2/pixelartconv/logic.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,17 @@
     for color in colors:
         if compare_px(color, closest_match, color_ref):
             closest_match = color
 
     return closest_match
 
 
+# ======== only the function below is currently used =========
+
+
 def convert_img(img: np.ndarray, colors: list[tuple]) -> np.ndarray:
     """
     Finds the closest match for each pixel in the image. Returns a copy of the
     original image, where the pixels are replaced only with colors from the palette.
 
     :param img: Reference image.
     :param colors: Color palette.
@@ -109,29 +112,16 @@
     for color in colors:
         color_lab = cv2.cvtColor(color.reshape(1, 1, 3).astype(np.float32) / 255, cv2.COLOR_RGB2Lab)
         color_lab = color_lab * np.ones(img_lab.shape)  # copy the source image dimensions
 
         distances.append(np.sum((img_lab - color_lab) ** 2, axis=-1))  # Euclidean distances of LAB colors
 
     dist_array = np.array(distances)  # (height, width, colorcount)
-    print(dist_array.shape)
 
     indexes = np.argmin(dist_array, axis=0)  # (height, width)
-    # print(indexes)
-    # print(indexes.shape)
 
     res = np.zeros(img.shape)
     for i in range(img.shape[0]):
         for j in range(img.shape[1]):
             res[i, j] = colors[indexes[i, j]]
 
-    # img = img.copy()
-    # i, j = 0, 0
-    # for row in img:
-    #     for px in row:
-    #         new_color = find_closest_match(px, colors)
-    #         img[i, j] = new_color
-    #         j += 1
-    #     j = 0
-    #     i += 1
-
     return res
```

### Comparing `pixelartconv-1.1.1/pixelartconv/script.py` & `pixelartconv-1.1.2/pixelartconv/script.py`

 * *Files identical despite different names*

### Comparing `pixelartconv-1.1.1/pixelartconv.egg-info/PKG-INFO` & `pixelartconv-1.1.2/pixelartconv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelartconv
-Version: 1.1.1
+Version: 1.1.2
 Summary: PixelArtConv - Pixel Art Converter
 Author-email: Simon Ruzicka <sima.ruzicka@gmail.com>
 Project-URL: Homepage, https://github.com/ruzicka02/paconv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `pixelartconv-1.1.1/pyproject.toml` & `pixelartconv-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pixelartconv"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Simon Ruzicka", email="sima.ruzicka@gmail.com" },
 ]
 description = "PixelArtConv - Pixel Art Converter"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

