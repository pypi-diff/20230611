# Comparing `tmp/aug-tool-0.0.4.tar.gz` & `tmp/aug-tool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug-tool-0.0.4.tar", last modified: Tue May 23 17:43:30 2023, max compression
+gzip compressed data, was "aug-tool-0.0.5.tar", last modified: Sun Jun 11 18:35:47 2023, max compression
```

## Comparing `aug-tool-0.0.4.tar` & `aug-tool-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.708980 aug-tool-0.0.4/
--rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug-tool-0.0.4/LICENCE
--rw-rw-rw-   0        0        0       20 2023-05-13 18:17:23.000000 aug-tool-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2616 2023-05-23 17:43:30.708980 aug-tool-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2059 2023-05-13 18:17:23.000000 aug-tool-0.0.4/README.md
--rw-rw-rw-   0        0        0      108 2023-05-13 18:17:23.000000 aug-tool-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      696 2023-05-23 17:43:30.710974 aug-tool-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.649273 aug-tool-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.661009 aug-tool-0.0.4/src/aug-tool/
--rw-rw-rw-   0        0        0        0 2023-05-12 19:34:11.000000 aug-tool-0.0.4/src/aug-tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.669354 aug-tool-0.0.4/src/aug-tool/dataAugmentor/
--rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/annAug.py
--rw-rw-rw-   0        0        0      505 2023-05-17 20:04:01.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/dataAug.py
--rw-rw-rw-   0        0        0     1975 2023-05-16 18:30:28.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/imgAug.py
--rw-rw-rw-   0        0        0      954 2023-05-17 20:04:00.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/txtAug.py
--rw-rw-rw-   0        0        0     1738 2023-05-17 19:15:02.000000 aug-tool-0.0.4/src/aug-tool/dataAugmentor/xmlAug.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.686499 aug-tool-0.0.4/src/aug-tool/dataOpener/
--rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/__init__.py
--rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/annOp.py
--rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/dataOp.py
--rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/imgOp.py
--rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/txtOp.py
--rw-rw-rw-   0        0        0     1535 2023-05-15 19:34:16.000000 aug-tool-0.0.4/src/aug-tool/dataOpener/xmlOp.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.701464 aug-tool-0.0.4/src/aug-tool/dataSaver/
--rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/__init__.py
--rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/annSav.py
--rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/dataSav.py
--rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/imgSav.py
--rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/txtSav.py
--rw-rw-rw-   0        0        0      473 2023-05-14 10:12:53.000000 aug-tool-0.0.4/src/aug-tool/dataSaver/xmlSav.py
--rw-rw-rw-   0        0        0      518 2023-05-17 20:04:00.000000 aug-tool-0.0.4/src/aug-tool/deneme.py
--rw-rw-rw-   0        0        0     5523 2023-05-23 17:32:49.000000 aug-tool-0.0.4/src/aug-tool/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:43:30.707980 aug-tool-0.0.4/src/aug_tool.egg-info/
--rw-rw-rw-   0        0        0     2616 2023-05-23 17:43:30.000000 aug-tool-0.0.4/src/aug_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      898 2023-05-23 17:43:30.000000 aug-tool-0.0.4/src/aug_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 17:43:30.000000 aug-tool-0.0.4/src/aug_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 17:43:30.000000 aug-tool-0.0.4/src/aug_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.647193 aug-tool-0.0.5/
+-rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug-tool-0.0.5/LICENCE
+-rw-rw-rw-   0        0        0       20 2023-05-13 18:17:23.000000 aug-tool-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    10121 2023-06-11 18:35:47.648189 aug-tool-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9564 2023-06-10 15:10:39.000000 aug-tool-0.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-13 18:17:23.000000 aug-tool-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      696 2023-06-11 18:35:47.649190 aug-tool-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.479237 aug-tool-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.504686 aug-tool-0.0.5/src/aug-tool/
+-rw-rw-rw-   0        0        0        0 2023-05-12 19:34:11.000000 aug-tool-0.0.5/src/aug-tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.532098 aug-tool-0.0.5/src/aug-tool/dataAugmentor/
+-rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/annAug.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 10:38:27.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/dataAug.py
+-rw-rw-rw-   0        0        0     2146 2023-06-11 10:59:25.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/imgAug.py
+-rw-rw-rw-   0        0        0     1043 2023-06-11 08:53:47.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/txtAug.py
+-rw-rw-rw-   0        0        0     2708 2023-06-11 10:59:24.000000 aug-tool-0.0.5/src/aug-tool/dataAugmentor/xmlAug.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.586738 aug-tool-0.0.5/src/aug-tool/dataOpener/
+-rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/__init__.py
+-rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/annOp.py
+-rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/dataOp.py
+-rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/imgOp.py
+-rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/txtOp.py
+-rw-rw-rw-   0        0        0     1586 2023-06-09 18:46:29.000000 aug-tool-0.0.5/src/aug-tool/dataOpener/xmlOp.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.639164 aug-tool-0.0.5/src/aug-tool/dataSaver/
+-rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/annSav.py
+-rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/dataSav.py
+-rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/imgSav.py
+-rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/txtSav.py
+-rw-rw-rw-   0        0        0      541 2023-06-11 10:59:24.000000 aug-tool-0.0.5/src/aug-tool/dataSaver/xmlSav.py
+-rw-rw-rw-   0        0        0      699 2023-06-10 09:47:20.000000 aug-tool-0.0.5/src/aug-tool/deneme.py
+-rw-rw-rw-   0        0        0     7262 2023-06-11 18:31:13.000000 aug-tool-0.0.5/src/aug-tool/factory.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:35:47.646200 aug-tool-0.0.5/src/aug_tool.egg-info/
+-rw-rw-rw-   0        0        0    10121 2023-06-11 18:35:47.000000 aug-tool-0.0.5/src/aug_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      898 2023-06-11 18:35:47.000000 aug-tool-0.0.5/src/aug_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 18:35:47.000000 aug-tool-0.0.5/src/aug_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 18:35:47.000000 aug-tool-0.0.5/src/aug_tool.egg-info/top_level.txt
```

### Comparing `aug-tool-0.0.4/LICENCE` & `aug-tool-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.4/setup.cfg` & `aug-tool-0.0.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7567 2d74 6f6f 6c0d 0a76 6572   = aug-tool..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e34 0d0a 6175  sion = 0.0.4..au
+00000020: 7369 6f6e 203d 2030 2e30 2e35 0d0a 6175  sion = 0.0.5..au
 00000030: 7468 6f72 203d 2048 616b 616e 2041 6b74  thor = Hakan Akt
 00000040: 61c5 9f0d 0a61 7574 686f 725f 656d 6169  a....author_emai
 00000050: 6c20 3d20 6861 6b61 6e61 6b74 6173 3435  l = hakanaktas45
 00000060: 3431 4067 6d61 696c 2e63 6f6d 0d0a 6465  41@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 736d  scription = A sm
 00000080: 616c 6c20 7061 636b 6167 6520 746f 2069  all package to i
 00000090: 6e63 7265 6173 6520 796f 7572 2064 6174  ncrease your dat
```

### Comparing `aug-tool-0.0.4/src/aug-tool/dataAugmentor/imgAug.py` & `aug-tool-0.0.5/src/aug-tool/dataAugmentor/imgAug.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 import random
 from PIL import ImageEnhance, ImageFilter
 
 class ImgAug(DataAug):
     
     rotate_rate = None
     
-    def __init__(self, image, x_shift: int, y_shift: int, contrast:bool = False, brigness:bool = False, sharpen:bool = False ) -> None:
-        super().__init__(None, image, None, x_shift, y_shift)
+    def __init__(self, image, x_shift: int, y_shift: int, random_x:int, random_y:int, contrast:bool = False, brigness:bool = False, sharpen:bool = False) -> None:
+        super().__init__(None, None, None, x_shift, y_shift)
+        self.image = image
         self.contrast = contrast
         self.brigness = brigness
         self.sharpen = sharpen
-        self.image_aug = None   
+        self.image_aug = None
+        self.x_shift = x_shift
+        self.y_shift = y_shift
+        self.random_x = random_x
+        self.random_y = random_y
         self.carve_out()
         self.apply_adj()
         
-
-
         
     def carve_out(self):
         
         self.image_aug = self.image.copy()
         self.image_aug = self.image_aug.filter(ImageFilter.BoxBlur(5))
 
         width, height = self.image.size
         
         self.image = self.image.crop((int(self.x_shift), int(self.y_shift),
                             width - int(self.x_shift), height - int(self.y_shift)))
         # img1 = img1.rotate(5, fillcolor=(1,0,0), expand=False)
 
-        self.image_aug.paste(self.image, (int(self.get_random_x), int(self.get_random_y)))
+        self.image_aug.paste(self.image, (int(self.random_x), int(self.random_y)))
     
     def apply_adj(self):
         
         queue = []
 
         if self.contrast:
             queue.append("Contrast")
```

### Comparing `aug-tool-0.0.4/src/aug-tool/dataAugmentor/txtAug.py` & `aug-tool-0.0.5/src/aug-tool/dataAugmentor/txtAug.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from .annAug import AnnAug
 
 class TxtAug(AnnAug):
-    def __init__(self, annotate, x_shift: int, y_shift: int, width,height) -> None:
+    def __init__(self, annotate, x_shift: int, y_shift: int, width, height, random_x:int, random_y:int) -> None:
         super().__init__(None, annotate, x_shift, y_shift)
         self.aug_anotate = self.create_new_cords(width, height)
+        self.random_x = random_x
+        self.random_y = random_y
         
     def create_new_cords(self, width, height):
         lines = self.annotate.readlines() 
         self.annotate.seek(0)
         aug_values = []
         for line in lines:
     
             values = line.strip().split()
 
-            aug_x_center = float(values[1]) + (self.get_random_x - int(self.x_shift))/width
-            aug_y_center = float(values[2]) + (self.get_random_y - int(self.y_shift))/height
+            aug_x_center = float(values[1]) + (self.random_x - int(self.x_shift))/width
+            aug_y_center = float(values[2]) + (self.random_y - int(self.y_shift))/height
             values[1] = str(aug_x_center)
             values[2] = str(aug_y_center)
 
             aug_line = " ".join(values)
             
             aug_values.append(aug_line)
```

### Comparing `aug-tool-0.0.4/src/aug-tool/dataAugmentor/xmlAug.py` & `aug-tool-0.0.5/src/aug-tool/dataAugmentor/xmlAug.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 from .annAug import AnnAug
 
+import random
+
 class XmlAug(AnnAug):
-    def __init__(self, name: str, annotate, x_shift: int, y_shift: int) -> None:
+    def __init__(self, name: str, annotate, x_shift: int, y_shift: int, random_x:int, random_y:int) -> None:
         super().__init__(name, annotate, x_shift, y_shift)
+        self.name = name
+        self.annotate = annotate
         self.x_min_new = []
         self.x_max_new = []
         self.y_min_new = []
         self.y_max_new = []
+        self.x_shift = x_shift
+        self.y_shift = y_shift
+        self.random_x = random_x
+        self.random_y = random_y
+        self.create_new_cords()
+        self.write_new_cords()
         
+
     def create_new_cords(self):
         
+        random_noise  = random.randint(-2, 2)
+        
         for i in self.annotate.find_all('xmin'):
-            self.x_min_new.append(int(i.text) + (self.get_random_x - int(self.x_shift)))
+            self.x_min_new.append(int(i.text) + (self.random_x - int(self.x_shift)) + random_noise)
         for i in self.annotate.find_all('xmax'):
-            self.x_max_ne.append(int(i.text) + (self.get_random_x - int(self.x_shift)))
+            self.x_max_new.append(int(i.text) + (self.random_x - int(self.x_shift)) + random_noise)
         for i in self.annotate.find_all('ymin'):
-            self.y_min_new.append(int(i.text) + (self.get_random_y - int(self.y_shift)))
+            self.y_min_new.append(int(i.text) + (self.random_y - int(self.y_shift)) + random_noise)
         for i in self.annotate.find_all('ymax'):
-            self.y_max_new.append(int(i.text) + (self.get_random_y - int(self.y_shift)))
+            self.y_max_new.append(int(i.text) + (self.random_y - int(self.y_shift)) + random_noise)
+
+
+        # for i in self.annotate.find_all('xmin'):
+        #     self.x_min_new.append(int(i.text) + (self.random_x - int(self.x_shift)))
+        # for i in self.annotate.find_all('xmax'):
+        #     self.x_max_new.append(int(i.text) + (self.random_x - int(self.x_shift)))
+        # for i in self.annotate.find_all('ymin'):
+        #     self.y_min_new.append(int(i.text) + (self.random_y - int(self.y_shift)))
+        # for i in self.annotate.find_all('ymax'):
+        #     self.y_max_new.append(int(i.text) + (self.random_y - int(self.y_shift)))
 
     def write_new_cords(self):
         
         for count in range(len(self.annotate.find_all('xmin'))):
             self.annotate.find_all('xmin')[count].string = str(self.x_min_new[count])
 
         for count in range(len(self.annotate.find_all('xmax'))):
```

### Comparing `aug-tool-0.0.4/src/aug-tool/dataOpener/dataOp.py` & `aug-tool-0.0.5/src/aug-tool/dataOpener/dataOp.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.4/src/aug-tool/dataOpener/imgOp.py` & `aug-tool-0.0.5/src/aug-tool/dataOpener/imgOp.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.4/src/aug-tool/dataOpener/txtOp.py` & `aug-tool-0.0.5/src/aug-tool/dataOpener/txtOp.py`

 * *Files identical despite different names*

### Comparing `aug-tool-0.0.4/src/aug-tool/dataOpener/xmlOp.py` & `aug-tool-0.0.5/src/aug-tool/dataOpener/xmlOp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import IO
 from .annOp import AnnotationOpener
-
+from bs4 import BeautifulSoup
 
 # The XmlFileOpener class is a subclass of AnnotationOpener used for opening XML files.
 class XmlFileOpener(AnnotationOpener):
 
     def __init__(self, open_file_name: str) -> None:
         """
         This is a constructor function that initializes an object with a given file name, sets the file
@@ -27,15 +27,15 @@
     def open_data(self) -> IO:
         """
         This function returns an IO object for reading data.
         """
         try:
             with open(self.data_name, self.mode) as f:
                 xml_data = f.read()
-            return xml_data
+            return BeautifulSoup(xml_data, "xml")
         
         except Exception as e:
             print(f"An error occurred while opening file {self.data_name}: {e}")
             return None
         
     def __repr__(self) -> str:
         """
```

### Comparing `aug-tool-0.0.4/src/aug_tool.egg-info/SOURCES.txt` & `aug-tool-0.0.5/src/aug_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

