# Comparing `tmp/gcode2image-1.1.0.tar.gz` & `tmp/gcode2image-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcode2image-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gcode2image-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gcode2image-1.1.0.tar` & `gcode2image-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1085 2023-06-10 15:37:36.380883 gcode2image-1.1.0/LICENSE
--rw-r--r--   0        0        0     1042 2023-06-10 15:30:03.262441 gcode2image-1.1.0/README.md
--rw-r--r--   0        0        0     9283 2023-06-10 15:41:27.935353 gcode2image-1.1.0/gcode2image.py
--rw-r--r--   0        0        0      709 2023-06-10 15:39:39.263246 gcode2image-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 gcode2image-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-10 15:37:36.380883 gcode2image-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1042 2023-06-10 15:30:03.262441 gcode2image-1.1.1/README.md
+-rw-r--r--   0        0        0     9284 2023-06-11 15:52:01.806611 gcode2image-1.1.1/gcode2image.py
+-rw-r--r--   0        0        0      709 2023-06-10 15:39:39.263246 gcode2image-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 gcode2image-1.1.1/PKG-INFO
```

### Comparing `gcode2image-1.1.0/LICENSE` & `gcode2image-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcode2image-1.1.0/README.md` & `gcode2image-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gcode2image-1.1.0/gcode2image.py` & `gcode2image-1.1.1/gcode2image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 """
-gcode2image: convert gode to image.
+gcode2image: convert gcode to image.
 """
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 import sys
 import re
 import argparse
 from PIL import Image
 from skimage.draw import line as drawline
 import numpy as np
```

### Comparing `gcode2image-1.1.0/pyproject.toml` & `gcode2image-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gcode2image-1.1.0/PKG-INFO` & `gcode2image-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gcode2image
-Version: 1.1.0
-Summary: gcode2image: convert gode to image.
+Version: 1.1.1
+Summary: gcode2image: convert gcode to image.
 Keywords: engraving,laser,image,laser engraving,PWM,gcode
 Author-email: Johannes Noordanus <mailjohannes.mailnoordanus@gmail.com>
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >= 1.24.3
 Requires-Dist: Pillow >= 9.5.0
```

