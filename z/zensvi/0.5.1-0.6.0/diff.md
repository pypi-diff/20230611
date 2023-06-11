# Comparing `tmp/zensvi-0.5.1.tar.gz` & `tmp/zensvi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.5.1.tar", max compression
+gzip compressed data, was "zensvi-0.6.0.tar", max compression
```

## Comparing `zensvi-0.5.1.tar` & `zensvi-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.5.1/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.5.1/README.md
--rwxr-xr-x   0        0        0      712 2023-06-07 07:54:52.881620 zensvi-0.5.1/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.5.1/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.5.1/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.5.1/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    39841 2023-06-05 07:31:29.453652 zensvi-0.5.1/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.5.1/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    46074 2023-06-05 08:53:58.000000 zensvi-0.5.1/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.5.1/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.5.1/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.5.1/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.5.1/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.5.1/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     6747 2023-06-05 08:53:58.000000 zensvi-0.5.1/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.5.1/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.5.1/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.5.1/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.5.1/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 zensvi-0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.0/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.0/README.md
+-rwxr-xr-x   0        0        0      728 2023-06-11 12:09:56.406906 zensvi-0.6.0/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.0/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.0/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.0/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    45667 2023-06-11 12:09:56.407566 zensvi-0.6.0/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.0/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    46074 2023-06-05 08:53:58.000000 zensvi-0.6.0/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.0/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.0/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.0/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.0/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.0/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     6747 2023-06-05 08:53:58.000000 zensvi-0.6.0/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.0/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.0/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.0/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.0/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 zensvi-0.6.0/PKG-INFO
```

### Comparing `zensvi-0.5.1/LICENSE` & `zensvi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/README.md` & `zensvi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/pyproject.toml` & `zensvi-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.5.1"
-description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
+version = "0.6.0"
+description = "This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.7,<3.11"
 Pillow = ">=8.3.2,<9.6"
 geopandas = "^0.9.0"
 geopy = "^2.2.0"
-numpy = ">=1.21.0"
+numpy = ">=1.16.5,<1.23.0"
 opencv_python = "^4.5.3"
 osmnx = "^1.1.1"
 pandas = "^1.3.3"
 requests = "^2.25.1"
 setuptools = "^64.0.3"
 Shapely=">=1.8.1"
 torch = "^2.0.0"
 tqdm = "^4.0.0"
 transformers = "^4.10.2"
 scipy = "1.7.3"
 networkx="^3.1"
-mapillary="^1.0.11"
+mapillary="1.0.11"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zensvi-0.5.1/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.6.0/src/zensvi/cv/segmentation/segmentation.py`

 * *Files 13% similar despite different names*

```diff
@@ -104,81 +104,80 @@
 def create_mapillary_vistas_label_colormap():
     """Creates a label colormap used in Mapillary Vistas segmentation benchmark.
     Returns:
         A list of labels for visualizing segmentation results.
     """
 
     labels = [
-        #       name                id  trainId  category            catId  hasInstances  ignoreInEval  color
-        Label('Bird',               0,      0, 'animal',             0,      True,         False,        (165, 42, 42)),
-        Label('Ground Animal',      1,      1, 'animal',             0,      True,         False,        (0, 192, 0)),
-        Label('Curb',               2,      2, 'construction',       1,      False,        False,        (196, 196, 196)),
-        Label('Fence',              3,      3, 'construction',       1,      False,        False,        (190, 153, 153)),
-        Label('Guard Rail',         4,      4, 'construction',       1,      False,        False,        (180, 165, 180)),
-        Label('Barrier',            5,      5, 'construction',       1,      False,        False,        (102, 102, 156)),
-        Label('Wall',               6,      6, 'construction',       1,      False,        False,        (102, 102, 156)),
-        Label('Bike Lane',          7,      7, 'flat',               2,      False,        False,        (128, 64, 255)),
-        Label('Crosswalk - Plain',  8,      8, 'flat',               2,      False,        False,        (140, 140, 200)),
-        Label('Curb Cut',           9,      9, 'flat',               2,      False,        False,        (170, 170, 170)),
-        Label('Parking',           10,     10, 'flat',               2,      False,        False,        (250, 170, 160)),
-        Label('Pedestrian Area',   11,     11, 'flat',               2,      False,        False,        (96, 96, 96)),
-        Label('Rail Track',        12,     12, 'flat',               2,      False,        False,        (230, 150, 140)),
-        Label('Road',              13,     13, 'flat',               2,      False,        False,        (128, 64, 128)),
-        Label('Service Lane',      14,     14, 'flat',               2,      False,        False,        (110, 110, 110)),
-        Label('Sidewalk',          15,     15, 'flat',               2,      False,        False,        (244, 35, 232)),
-        Label('Bridge',            16,     16, 'construction',       1,      False,        False,        (150, 100, 100)),
-        Label('Building',           17,     17, 'construction',       1,      False,        False,        (70, 70, 70)),
-        Label('Tunnel',             18,     18, 'construction',       1,      False,        False,        (150, 120, 90)),
-        Label('Person',             19,     19, 'human',              3,      True,         False,        (220, 20, 60)),
-        Label('Bicyclist',          20,     20, 'human',              3,      True,         False,        (255, 0, 0)),
-        Label('Motorcyclist',       21,     21, 'human',              3,      True,         False,        (255, 0, 0)),
-        Label('Other Rider',        22,     22, 'human',              3,      True,         False,        (255, 0, 0)),
-        Label('Lane Marking - Crosswalk', 23, 23, 'marking',         4,      False,        False,        (200, 128, 128)),
-        Label('Lane Marking - General', 24, 24, 'marking',           4,      False,        False,        (255, 255, 255)),
-        Label('Mountain',           25,     25, 'nature',             5,      False,        False,        (64, 170, 64)),
-        Label('Sand',               26,     26, 'nature',             5,      False,        False,        (230, 160, 50)),
-        Label('Sky',                27,     27, 'nature',             5,      False,        False,        (70, 130, 180)),
-        Label('Snow',               28,     28, 'nature',             5,      False,        False,        (190, 255, 255)),
-        Label('Terrain',            29,     29, 'nature',             5,      False,        False,        (152, 251, 152)),
-        Label('Vegetation',         30,     30, 'nature',             5,      False,        False,        (107, 142, 35)),
-        Label('Water',              31,     31, 'nature',             5,      False,        False,        (0, 170, 30)),
-        Label('Banner',             32,     32, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Bench',              33,     33, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Bike Rack',          34,     34, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Billboard',          35,     35, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Catch Basin',        36,     36, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('CCTV Camera',        37,     37, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Fire Hydrant',       38,     38, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Junction Box',       39,     39, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Mailbox',            40,     40, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Manhole',            41,     41, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Phone Booth',        42,     42, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Pothole',            43,     43, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Street Light',       44,     44, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Traffic Cone',       45,     45, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Traffic Device',     46,     46, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Traffic Light',      47,     47, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Traffic Sign',       48,     48, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Traffic Sign Frame', 49,     49, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Trash Can',          50,     50, 'object',             6,      False,        False,        (255, 255, 128)),
-        Label('Bicycle',            51,     51, 'vehicle',            7,      True,         False,        (119, 11, 32)),
-        Label('Boat',               52,     52, 'vehicle',            7,      True,         False,        (0, 0, 142)),
-        Label('Bus',                53,     53, 'vehicle',            7,      True,         False,        (0, 60, 100)),
-        Label('Car',                54,     54, 'vehicle',            7,      True,         False,        (0, 0, 142)),
-        Label('Caravan',            55,     55, 'vehicle',            7,      True,         False,        (0, 0, 90)),
-        Label('Motorcycle',         56,     56, 'vehicle',            7,      True,         False,        (0, 0, 230)),
-        Label('On Rails',           57,     57, 'vehicle',            7,      True,         False,        (0, 80, 100)),
-        Label('Other Vehicle',      58,     58, 'vehicle',            7,      True,         False,        (128, 64, 128)),
-        Label('Trailer',            59,     59, 'vehicle',            7,      True,         False,        (0, 0, 110)),
-        Label('Truck',              60,     60, 'vehicle',            7,      True,         False,        (0, 0, 70)),
-        Label('Wheeled Slow',       61,     61, 'vehicle',            7,      True,         False,        (0, 0, 192)),
-        Label('Car Mount',          62,     62, 'vehicle',            7,      False,        False,        (32, 32, 32)),
-        Label('Ego Vehicle',        63,     63, 'vehicle',            7,      False,        False,        (120, 10, 10))
+        Label('Bird',                   0,      0, 'animal',             0,      True,         False,        (165, 42, 42)),
+        Label('Ground Animal',          1,      1, 'animal',             0,      True,         False,        (0, 192, 0)),
+        Label('Curb',                   2,      2, 'construction',       1,      False,        False,        (196, 196, 196)),
+        Label('Fence',                  3,      3, 'construction',       1,      False,        False,        (190, 153, 153)),
+        Label('Guard Rail',             4,      4, 'construction',       1,      False,        False,        (180, 165, 180)),
+        Label('Barrier',                5,      5, 'construction',       1,      False,        False,        (102, 102, 156)),
+        Label('Wall',                   6,      6, 'construction',       1,      False,        False,        (102, 102, 156)),
+        Label('Bike Lane',              7,      7, 'flat',               2,      False,        False,        (128, 64, 255)),
+        Label('Crosswalk - Plain',      8,      8, 'flat',               2,      False,        False,        (140, 140, 200)),
+        Label('Curb Cut',               9,      9, 'flat',               2,      False,        False,        (170, 170, 170)),
+        Label('Parking',               10,     10, 'flat',               2,      False,        False,        (250, 170, 160)),
+        Label('Pedestrian Area',       11,     11, 'flat',               2,      False,        False,        (96, 96, 96)),
+        Label('Rail Track',            12,     12, 'flat',               2,      False,        False,        (230, 150, 140)),
+        Label('Road',                  13,     13, 'flat',               2,      False,        False,        (128, 64, 128)),
+        Label('Service Lane',          14,     14, 'flat',               2,      False,        False,        (110, 110, 110)),
+        Label('Sidewalk',              15,     15, 'flat',               2,      False,        False,        (244, 35, 232)),
+        Label('Bridge',                16,     16, 'construction',       1,      False,        False,        (150, 100, 100)),
+        Label('Building',              17,     17, 'construction',       1,      False,        False,        (70, 70, 70)),
+        Label('Tunnel',                18,     18, 'construction',       1,      False,        False,        (150, 120, 90)),
+        Label('Person',                19,     19, 'human',              3,      True,         False,        (220, 20, 60)),
+        Label('Bicyclist',             20,     20, 'human',              3,      True,         False,        (255, 0, 0)),
+        Label('Motorcyclist',          21,     21, 'human',              3,      True,         False,        (255, 0, 0)),
+        Label('Other Rider',           22,     22, 'human',              3,      True,         False,        (255, 0, 0)),
+        Label('Lane Marking - Crosswalk',23,  23, 'marking',            4,      False,        True,         (200, 128, 128)),
+        Label('Lane Marking - General',24,     24, 'marking',            4,      True,         False,        (255, 255, 255)),
+        Label('Mountain',              25,     25, 'nature',             5,      False,        False,        (64, 170, 64)),
+        Label('Sand',                  26,     26, 'nature',             5,      False,        False,        (230, 160, 50)),
+        Label('Sky',                   27,     27, 'sky',                6,      False,        False,        (70, 130, 180)),
+        Label('Snow',                  28,     28, 'nature',             5,      False,        False,        (190, 255, 255)),
+        Label('Terrain',               29,     29, 'nature',             5,      False,        False,        (152, 251, 152)),
+        Label('Vegetation',            30,     30, 'nature',             5,      False,        False,        (107, 142, 35)),
+        Label('Water',                 31,     31, 'water',              7,      False,        False,        (0, 170, 30)),
+        Label('Banner',                32,     32, 'object',             8,      False,        False,        (255, 220, 0)),
+        Label('Bench',                 33,     33, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Bike Rack',             34,     34, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Billboard',             35,     35, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Catch Basin',           36,     36, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('CCTV Camera',           37,     37, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Fire Hydrant',          38,     38, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Junction Box',          39,     39, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Mailbox',               40,     40, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Manhole',               41,     41, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Phone Booth',           42,     42, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Pothole',               43,     43, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Street Light',          44,     44, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Pole',                  45,     45, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Traffic Sign Frame',    46,     46, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Utility Pole',          47,     47, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Traffic Light',         48,     48, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Traffic Sign (Back)',   49,     49, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Traffic Sign (Front)',  50,     50, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Trash Can',             51,     51, 'object',             8,      False,        False,        (255, 0, 0)),
+        Label('Bicycle',               52,     52, 'vehicle',            9,      True,         False,        (119, 11, 32)),
+        Label('Boat',                  53,     53, 'vehicle',            9,      False,        False,        (0, 0, 142)),
+        Label('Bus',                   54,     54, 'vehicle',            9,      True,         False,        (0, 60, 100)),
+        Label('Car',                   55,     55, 'vehicle',            9,      True,         False,        (0, 0, 142)),
+        Label('Caravan',               56,     56, 'vehicle',            9,      True,         False,        (0, 0, 90)),
+        Label('Motorcycle',            57,     57, 'vehicle',            9,      True,         False,        (0, 0, 230)),
+        Label('On Rails',              58,     58, 'vehicle',            9,      False,        False,        (0, 80, 100)),
+        Label('Other Vehicle',         59,     59, 'vehicle',            9,      True,         False,        (128, 64, 64)),
+        Label('Trailer',               60,     60, 'vehicle',            9,      True,         False,        (0, 0, 110)),
+        Label('Truck',                 61,     61, 'vehicle',            9,      True,         False,        (0, 0, 70)),
+        Label('Wheeled Slow',          62,     62, 'vehicle',            9,      False,        False,        (0, 0, 192)),
+        Label('Car Mount',             63,     63, 'vehicle',            9,      True,         False,        (32, 32, 32)),
+        Label('Ego Vehicle',           64,     64, 'vehicle',            9,      True,         False,        (120, 10, 10))
     ]
-
     return labels
 
 def get_resized_dimensions(image: cv2.Mat, max_size: int = 2048) -> Tuple[int, int]:
     """
     Get the resized dimensions of an image based on a maximum size.
 
     Args:
@@ -258,26 +257,44 @@
         Returns:
             Tuple[List[str], List[cv2.Mat], List[Tuple[int, int]]]: Tuple containing lists of image file paths, image data, and original image dimensions.
         """
         image_files, images, original_img_shape = zip(*data)
         return list(image_files), list(images), list(original_img_shape)
 
 class Segmenter:
-    def __init__(self, model_name="facebook/mask2former-swin-tiny-cityscapes-semantic", dataset="cityscapes"):
+    def __init__(self, dataset="cityscapes", task = "semantic"):
         """
         Initialize the Segmenter with a model and dataset.
 
         Args:
             model_name (str): The name of the pre-trained model.
             dataset (str): The name of the dataset.
         """
         self.device = self._get_device()
-        self.model, self.processor = self._get_model_processor(model_name)
+        self.dataset = dataset
+        self.task = task
+        self.model_name = self._get_model_name(self.dataset, self.task)
+        self.model, self.processor = self._get_model_processor(self.model_name)
         self.color_map = self._create_color_map(dataset)
         self.label_map = self._create_label_map(dataset)
+        self.id_to_name_map = self._create_id_to_name_map(dataset)
+    
+    def _get_model_name(self, dataset, task):
+        if dataset == "cityscapes":
+            if task == "semantic":
+                return "facebook/mask2former-swin-tiny-cityscapes-semantic"
+            elif task == "panoptic":
+                return "facebook/mask2former-swin-tiny-cityscapes-panoptic"
+        elif dataset == "mapillary":
+            if task == "semantic":
+                return "facebook/mask2former-swin-large-mapillary-vistas-semantic"
+            elif task == "panoptic":
+                return "facebook/mask2former-swin-large-mapillary-vistas-panoptic"
+        else:
+            raise ValueError(f"Unknown dataset: {dataset}")
 
     def _get_model_processor(self, model_name):
         """
         Get the model and processor for the given model name.
 
         Args:
             model_name (str): The name of the pre-trained model.
@@ -340,14 +357,21 @@
         color_to_label = {}
         for label in labels:
             color = label.color
             color_to_label[color] = label
 
         return color_to_label
 
+    def _create_id_to_name_map(self, dataset):
+        if dataset == "cityscapes":
+            labels = create_cityscapes_label_colormap()
+        elif dataset == "mapillary":
+            labels = create_mapillary_vistas_label_colormap()
+        return {label.trainId: label.name for label in labels}
+    
     def _get_device(self) -> torch.device:
         """
         Get the appropriate device for running the model.
 
         Returns:
             torch.device: The device to use for running the model.
         """
@@ -370,41 +394,43 @@
         """
         unique, counts = np.unique(segmented_img, return_counts=True)
         total_pixels = np.sum(counts)
         pixel_ratios = {self.train_id_to_name[train_id]: count / total_pixels for train_id, count in zip(unique, counts)}
 
         return pixel_ratios
 
-    def _save_pixel_ratios_as_csv(self, pixel_ratio_dict, dir_output):
-        """
-        Save pixel ratios dictionary as a CSV file.
+    def _save_as_csv(self, input_dict, dir_output, value_name, csv_format):
+        if csv_format == "long":
+            df_list = [pd.DataFrame({'filename_key': [filename_key], 'label_name': [key], value_name: [value] if value is not None else [0]}) 
+                    for filename_key, inner_dict in input_dict.items() 
+                    for key, value in inner_dict.items()]
+
+            pixel_ratios_df = pd.concat(df_list, ignore_index=True)
+
+        elif csv_format == "wide":
+            pixel_ratios_df = pd.DataFrame(input_dict).transpose().fillna(0)
+            pixel_ratios_df.index.names = ["filename_key"]
+
+        pixel_ratios_df.to_csv(dir_output / Path(value_name + ".csv"), index=False)
 
-        Args:
-            pixel_ratio_dict (dict): Dictionary with class names as keys and pixel ratios as values.
-            dir_output (pathlib.Path): Output directory path.
-        """
-        pixel_ratios_df = pd.DataFrame(pixel_ratio_dict).transpose()
-        pixel_ratios_df.fillna(0, inplace=True)
-        pixel_ratios_df.index.names = ["filename_key"]
-        pixel_ratios_df.to_csv(dir_output / "pixel_ratios.csv")
 
     def _panoptic_segmentation(self, images, original_img_shape):
         """
         Perform panoptic segmentation on the given images.
 
         Args:
             images (list): List of input images.
             original_img_shape (tuple): Original image shape.
 
         Returns:
             list: List of panoptic segmentation outputs.
         """
         inputs = self.processor(images=images, task_inputs=["panoptic"], return_tensors="pt").to(self.model.device)
         outputs = self.model(**inputs)
-        return self.processor.post_process_panoptic_segmentation(outputs, target_sizes=original_img_shape)
+        return self.processor.post_process_panoptic_segmentation(outputs, target_sizes=original_img_shape, label_ids_to_fuse = set([]))
 
     def _semantic_segmentation(self, images, original_img_shape):
         """
         Perform semantic segmentation on the given images.
 
         Args:
             images (list): List of input images.
@@ -413,18 +439,15 @@
         Returns:
             tuple: Tuple containing list of semantic segmentation outputs and list of pixel ratios.
         """
         inputs = self.processor(images=images, return_tensors="pt").to(self.model.device)
         with torch.no_grad():
             outputs = self.model(**inputs)
         segmentations = self.processor.post_process_semantic_segmentation(outputs, target_sizes=original_img_shape)
-
-        pixel_ratios = [self._calculate_pixel_ratios(segmentation.cpu().numpy()) for segmentation in segmentations]
-
-        return segmentations, pixel_ratios
+        return segmentations
 
     def _trainid_to_color(self, segmented_img):
         """
         Convert segmented image with train IDs to a colored image.
 
         Args:
             segmented_img (numpy.ndarray): Segmented image with train IDs.
@@ -441,23 +464,42 @@
 
         Args:
             image_file (str): The input image file path.
             img (np.array): The input image in the format of a NumPy array.
             dir_output (Path): The output directory path to save the blended image.
             output (dict): The output dictionary containing the segmentation data.
         """
-        img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-        segmented_img = output["segmentation"].cpu().numpy()
-        colored_segmented_img = self._trainid_to_color(segmented_img)
-        
+        colored_segmented_img = self._trainid_to_color(output['label_segmentation'].cpu().numpy())
         alpha = 0.5
         blend_img = cv2.addWeighted(img, alpha, colored_segmented_img, 1 - alpha, 0)
 
+        # Add annotations for each segment
+        for segment_info in output['segments_info']:
+            segment_id = segment_info['id']
+            label_id = segment_info['label_id']
+            score = segment_info['score']
+            
+            # Use the label name instead of the label_id
+            label_name = self.id_to_name_map.get(label_id)
+            
+            # Find the center of the segment for the label placement
+            y, x = np.where(output['segmentation'].cpu().numpy() == segment_id)
+            center_x, center_y = np.mean(x), np.mean(y)
+            
+            # Add the annotation
+            text = f"{label_name}-{score:.2f}"
+            cv2.putText(blend_img, text, (int(center_x), int(center_y)), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255, 255, 255), 1, cv2.LINE_AA)
+
         output_file = dir_output / Path(image_file).name
-        cv2.imwrite(str(output_file), cv2.cvtColor(blend_img, cv2.COLOR_RGB2BGR))
+        
+        # Save images based on specified options
+        if "segmented_image" in self.save_image_options:
+            cv2.imwrite(str(output_file.with_name(output_file.stem + "_colored_segmented.png")), cv2.cvtColor(colored_segmented_img, cv2.COLOR_RGB2BGR))
+        if "blend_image" in self.save_image_options:
+            cv2.imwrite(str(output_file.with_name(output_file.stem + "_blend.png")), cv2.cvtColor(blend_img, cv2.COLOR_RGB2BGR))
         
     def _save_semantic_segmentation_image(self, image_file, img, dir_output, output):
         """
         Save the semantic segmentation image as a colored segmented image and/or a blended image with the original input image.
 
         Args:
             image_file (str): The input image file path.
@@ -473,31 +515,52 @@
         
         # Save images based on specified options
         if "segmented_image" in self.save_image_options:
             cv2.imwrite(str(output_file.with_name(output_file.stem + "_colored_segmented.png")), cv2.cvtColor(colored_segmented_img, cv2.COLOR_RGB2BGR))
         if "blend_image" in self.save_image_options:
             cv2.imwrite(str(output_file.with_name(output_file.stem + "_blend.png")), cv2.cvtColor(blend_img, cv2.COLOR_RGB2BGR))
 
-    def _save_segmentation_image(self, task, image_file, img, dir_output, output):
-        """
-        Save the segmentation image based on the given task.
+    def _panoptic_count_labels(self, output):
+        label_counts = {}
 
-        Args:
-            task (str): The segmentation task, either "panoptic" or "semantic".
-            image_file (str): The input image file path.
-            img (np.array): The input image in the format of a NumPy array.
-            dir_output (Path): The output directory path to save the segmentation images.
-            output (dict or Tensor): The output data containing the segmentation results.
-        """
-        if task == "panoptic":
-            self._save_panoptic_segmentation_image(image_file, img, dir_output, output)
-        elif task == "semantic":
-            self._save_semantic_segmentation_image(image_file, img, dir_output, output)
+        # Loop through each segment in the image
+        segments_info_list = output['segments_info']
+        for segments_info in segments_info_list:
+            # Convert label_id to label_name
+            label_name = self.id_to_name_map.get(segments_info["label_id"])
+            # Increment the count for the name in label_counts
+            if label_name in label_counts:
+                label_counts[label_name] += 1
+            else:
+                label_counts[label_name] = 1
+        return label_counts
+    
+    def _panoptic_segment_to_label(self, output):
+        """
+        This function converts the output of post_process_panoptic_segmentation function
+        from segment_id to label_id.
+        :param output: The output dictionary from the post_process_panoptic_segmentation function
+        :return: segmentation with label_ids instead of segment_ids
+        """
+        # Extract the segmentation and segments_info from the output
+        segmentation = output['segmentation']
+        segments_info = output['segments_info']
+
+        # Create a mapping from segment_id to label_id
+        id_map = {segment['id']: segment['label_id'] for segment in segments_info}
+
+        # Use the map to convert the segmentation tensor from segment_ids to label_ids
+        new_segmentation = segmentation.clone()
+
+        for seg_id, label_id in id_map.items():
+            new_segmentation[segmentation == seg_id] = label_id
 
-    def _process_images(self, task, image_files, images, dir_output, pixel_ratio_dict, original_img_shape):
+        return new_segmentation
+
+    def _process_images(self, task, image_files, images, dir_output, pixel_ratio_dict, original_img_shape, panoptic_dict=None):
         """
         Process the input images for segmentation and save the output images.
 
         Args:
             task (str): The segmentation task to perform, either "panoptic" or "semantic".
             image_files (List[str]): The list of file paths of the input images.
             images (List[ndarray]): The list of input images in the form of numpy arrays.
@@ -505,58 +568,69 @@
             pixel_ratio_dict (defaultdict): A dictionary to store the pixel ratios of the segmented images.
             original_img_shape (List[Tuple[int, int]]): The original shapes of the input images.
 
         Returns:
             None
         """
         outputs = None
-        pixel_ratios = None
         if task == "panoptic":
             outputs = self._panoptic_segmentation(images, original_img_shape)
+            if outputs is not None:
+                for image_file, img, output in zip(image_files, images, outputs):
+                    # create a new segmentation with label_ids instead of segment_ids
+                    output["label_segmentation"] = self._panoptic_segment_to_label(output)
+                    if (len(self.save_image_options) > 0) & (dir_output is not None):
+                        self._save_panoptic_segmentation_image(image_file, img, dir_output, output)
+                    pixel_ratio = self._calculate_pixel_ratios(output["label_segmentation"].cpu().numpy()) 
+                    label_counts = self._panoptic_count_labels(output)
+                    image_file_key = Path(image_file).stem
+                    pixel_ratio_dict[image_file_key] = pixel_ratio
+                    panoptic_dict[image_file_key] = label_counts
+                    
         elif task == "semantic":
-            outputs, pixel_ratios = self._semantic_segmentation(images, original_img_shape)
-
-        if outputs is not None:
-            for image_file, img, output, pixel_ratio in zip(image_files, images, outputs, pixel_ratios):
-                if (len(self.save_image_options) > 0) & (dir_output is not None):
-                    self._save_segmentation_image(task, image_file, img, dir_output, output)
-                image_file_key = Path(image_file).stem
-                pixel_ratio_dict[image_file_key] = pixel_ratio
+            segmentations = self._semantic_segmentation(images, original_img_shape)
+            if segmentations is not None:
+                for image_file, img, segmentation in zip(image_files, images, segmentations):
+                    if (len(self.save_image_options) > 0) & (dir_output is not None):
+                        self._save_semantic_segmentation_image(image_file, img, dir_output, segmentation)
+                    pixel_ratio = self._calculate_pixel_ratios(segmentation.cpu().numpy())
+                    image_file_key = Path(image_file).stem
+                    pixel_ratio_dict[image_file_key] = pixel_ratio
 
     # Modify the segment method inside the Segmenter class
     def segment(self, dir_input: Union[str, Path], 
                 dir_image_output: Union[str, Path, None] = None, 
-                dir_pixel_ratio_output: Union[str, Path, None] = None, 
-                task="semantic", 
+                dir_segmentation_summary_output: Union[str, Path, None] = None, 
                 batch_size=1, 
                 save_image_options = ["segmented_image", "blend_image"], 
                 pixel_ratio_save_format = ["json", "csv"],
+                csv_format = "long", # "long" or "wide"
                 max_workers: Union[int, None] = None):
-        # make sure that at least one of dir_image_output and dir_pixel_ratio_output is not None
-        if (dir_image_output is None) & (dir_pixel_ratio_output is None):
-            raise ValueError("At least one of dir_image_output and dir_pixel_ratio_output must not be None.")
+        # make sure that at least one of dir_image_output and dir_segmentation_summary_output is not None
+        if (dir_image_output is None) & (dir_segmentation_summary_output is None):
+            raise ValueError("At least one of dir_image_output and dir_segmentation_summary_output must not be None.")
         
         # save_image_options as a property of the class
         self.save_image_options = save_image_options
         
         # make directory
         dir_input = Path(dir_input)
-        dir_cache_pixel_ratio = None
+        dir_cache_segmentation_summary = None
         if dir_image_output is not None:
             dir_image_output = Path(dir_image_output)
             dir_image_output.mkdir(parents=True, exist_ok=True)
-        if dir_pixel_ratio_output is not None:
-            dir_pixel_ratio_output = Path(dir_pixel_ratio_output)
-            dir_pixel_ratio_output.mkdir(parents=True, exist_ok=True)
+        if dir_segmentation_summary_output is not None:
+            dir_segmentation_summary_output = Path(dir_segmentation_summary_output)
+            dir_segmentation_summary_output.mkdir(parents=True, exist_ok=True)
             # Create a new directory called "pixel_ratio_checkpoints"
-            dir_cache_pixel_ratio = dir_pixel_ratio_output / 'pixel_ratio_checkpoints'
-            dir_cache_pixel_ratio.mkdir(parents=True, exist_ok=True)
+            dir_cache_segmentation_summary = dir_segmentation_summary_output / 'pixel_ratio_checkpoints'
+            dir_cache_segmentation_summary.mkdir(parents=True, exist_ok=True)
 
             # Load all the checkpoint json files
-            checkpoints = glob.glob(str(dir_cache_pixel_ratio / '*.json'))
+            checkpoints = glob.glob(str(dir_cache_segmentation_summary / '*.json'))
             checkpoint_start_index = len(checkpoints)
 
             completed_image_files = set()  # completed_image_files will store the keys in the pixel_ratio_dict
             if checkpoint_start_index > 0:
                 for checkpoint in checkpoints:
                     with open(checkpoint, 'r') as f:
                         checkpoint_dict = json.load(f)
@@ -575,49 +649,72 @@
         for i in tqdm(range(num_outer_batches), desc=f"Processing outer batches of size {min(outer_batch_size * batch_size, len(image_file_list))}"):
             # Get the image files for the current outer batch
             outer_batch_image_file_list = image_file_list[i * outer_batch_size * batch_size : (i+1) * outer_batch_size * batch_size]
 
             dataset = ImageDataset(outer_batch_image_file_list)
             dataloader = DataLoader(dataset, batch_size=batch_size, collate_fn=dataset.collate_fn)
 
+            # set up pixel_ratio_dict for the current outer batch
             pixel_ratio_dict = defaultdict(dict)  # reset pixel_ratio_dict for each outer batch
-
+            panoptic_dict = defaultdict(dict)  # reset panoptic_dict for each outer batch
             with ThreadPoolExecutor(max_workers=max_workers) as executor:
                 futures = []
 
                 for batch in dataloader:
                     image_files, images, original_img_shape = batch
-                    future = executor.submit(self._process_images, task, image_files, images, dir_image_output, pixel_ratio_dict, original_img_shape)
+                    if self.task == "panoptic":
+                        future = executor.submit(self._process_images, self.task, image_files, images, dir_image_output, pixel_ratio_dict, original_img_shape, panoptic_dict)
+                    elif self.task == "semantic":
+                        future = executor.submit(self._process_images, self.task, image_files, images, dir_image_output, pixel_ratio_dict, original_img_shape)
                     futures.append(future)
 
                 for completed_future in tqdm(as_completed(futures), total=len(futures), desc=f"Processing outer batch #{i+1}"):
                     completed_future.result()
 
                 # Save checkpoint for each outer batch
-                with open(f'{dir_cache_pixel_ratio}/checkpoint_batch_{checkpoint_start_index+i+1}.json', 'w') as f:
+                with open(f'{dir_cache_segmentation_summary}/checkpoint_batch_{checkpoint_start_index+i+1}_pixel_ratio.json', 'w') as f:
                     json.dump(pixel_ratio_dict, f)
+                    
+                if self.task == "panoptic":
+                    with open(f'{dir_cache_segmentation_summary}/checkpoint_batch_{checkpoint_start_index+i+1}_panoptic.json', 'w') as f:
+                        json.dump(panoptic_dict, f)
 
         # Merge all checkpoints into a single pixel_ratio_dict
         pixel_ratio_dict = defaultdict(dict)
-        for checkpoint in glob.glob(str(dir_cache_pixel_ratio / '*.json')):
+        for checkpoint in glob.glob(str(dir_cache_segmentation_summary / '*_pixel_ratio.json')):
             with open(checkpoint, 'r') as f:
                 checkpoint_dict = json.load(f)
                 for key, value in checkpoint_dict.items():
                     pixel_ratio_dict[key] = value
+        
+        # Merge all checkpoints into a single panoptic_dict
+        if self.task == "panoptic":
+            panoptic_dict = defaultdict(dict)
+            for checkpoint in glob.glob(str(dir_cache_segmentation_summary / '*_panoptic.json')):
+                with open(checkpoint, 'r') as f:
+                    checkpoint_dict = json.load(f)
+                    for key, value in checkpoint_dict.items():
+                        panoptic_dict[key] = value
 
         # Save pixel_ratio_dict as a JSON or CSV file
         if "json" in pixel_ratio_save_format:
-            with open(dir_pixel_ratio_output / "pixel_ratios.json", "w") as f:
+            with open(dir_segmentation_summary_output / "pixel_ratios.json", "w") as f:
                 json.dump(pixel_ratio_dict, f)
+            if self.task == "panoptic":
+                with open(dir_segmentation_summary_output / "label_counts.json", "w") as f:
+                    json.dump(panoptic_dict, f)
         if "csv" in pixel_ratio_save_format:
-            self._save_pixel_ratios_as_csv(pixel_ratio_dict, dir_pixel_ratio_output)
+            self._save_as_csv(pixel_ratio_dict, dir_segmentation_summary_output, "pixel_ratios", csv_format)
+            if self.task == "panoptic":
+                self._save_as_csv(panoptic_dict, dir_segmentation_summary_output, "label_counts", csv_format)
+                
             
         # Delete the "pixel_ratio_checkpoints" directory
-        if dir_pixel_ratio_output is not None:
-            shutil.rmtree(dir_cache_pixel_ratio)
+        if dir_segmentation_summary_output is not None:
+            shutil.rmtree(dir_cache_segmentation_summary)
 
             
     def calculate_pixel_ratio_post_process(self, dir_input, dir_output, pixel_ratio_save_format = ["json", "csv"]):
         """
         Calculates the pixel ratio of different classes present in the segmented images and saves the results in either JSON or CSV format.
 
         Args:
```

### Comparing `zensvi-0.5.1/src/zensvi/download/streetview_downloader.py` & `zensvi-0.6.0/src/zensvi/download/streetview_downloader.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.6.0/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.6.0/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/src/zensvi/download/utils/get_pids.py` & `zensvi-0.6.0/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/src/zensvi/download/utils/helpers.py` & `zensvi-0.6.0/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/src/zensvi/download/utils/imtool.py` & `zensvi-0.6.0/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/src/zensvi/download/utils/proxies.csv` & `zensvi-0.6.0/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/src/zensvi/transform/transform_image.py` & `zensvi-0.6.0/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.5.1/PKG-INFO` & `zensvi-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.5.1
-Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
+Version: 0.6.0
+Summary: This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner.
 License: MIT
 Author: koito19960406
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=8.3.2,<9.6)
 Requires-Dist: Shapely (>=1.8.1)
 Requires-Dist: geopandas (>=0.9.0,<0.10.0)
 Requires-Dist: geopy (>=2.2.0,<3.0.0)
-Requires-Dist: mapillary (>=1.0.11,<2.0.0)
+Requires-Dist: mapillary (==1.0.11)
 Requires-Dist: networkx (>=3.1,<4.0)
-Requires-Dist: numpy (>=1.21.0)
+Requires-Dist: numpy (>=1.16.5,<1.23.0)
 Requires-Dist: opencv_python (>=4.5.3,<5.0.0)
 Requires-Dist: osmnx (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: scipy (==1.7.3)
 Requires-Dist: setuptools (>=64.0.3,<65.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
```

