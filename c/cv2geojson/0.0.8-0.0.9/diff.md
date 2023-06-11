# Comparing `tmp/cv2geojson-0.0.8.tar.gz` & `tmp/cv2geojson-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv2geojson-0.0.8.tar", last modified: Sat May 13 13:12:31 2023, max compression
+gzip compressed data, was "cv2geojson-0.0.9.tar", last modified: Sun Jun 11 21:27:02 2023, max compression
```

## Comparing `cv2geojson-0.0.8.tar` & `cv2geojson-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 13:12:31.246787 cv2geojson-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-04-04 10:50:06.000000 cv2geojson-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2778 2023-05-13 13:12:31.246787 cv2geojson-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2043 2023-05-13 13:11:22.000000 cv2geojson-0.0.8/README.md
--rw-rw-rw-   0        0        0      774 2023-05-13 13:12:00.000000 cv2geojson-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 13:12:31.246787 cv2geojson-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 13:12:31.225371 cv2geojson-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 13:12:31.225371 cv2geojson-0.0.8/src/cv2geojson/
--rw-rw-rw-   0        0        0    12518 2023-05-13 11:18:59.000000 cv2geojson-0.0.8/src/cv2geojson/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:12:31.246787 cv2geojson-0.0.8/src/cv2geojson.egg-info/
--rw-rw-rw-   0        0        0     2778 2023-05-13 13:12:31.000000 cv2geojson-0.0.8/src/cv2geojson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-13 13:12:31.000000 cv2geojson-0.0.8/src/cv2geojson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 13:12:31.000000 cv2geojson-0.0.8/src/cv2geojson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-13 13:12:31.000000 cv2geojson-0.0.8/src/cv2geojson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-13 13:12:31.000000 cv2geojson-0.0.8/src/cv2geojson.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 21:27:02.014672 cv2geojson-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-04-04 10:50:06.000000 cv2geojson-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    11615 2023-06-11 21:27:02.013669 cv2geojson-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10880 2023-06-11 21:22:14.000000 cv2geojson-0.0.9/README.md
+-rw-rw-rw-   0        0        0      774 2023-05-21 11:04:11.000000 cv2geojson-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 21:27:02.014672 cv2geojson-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 21:27:01.977584 cv2geojson-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 21:27:01.977584 cv2geojson-0.0.9/src/cv2geojson/
+-rw-rw-rw-   0        0        0    13743 2023-06-11 20:30:56.000000 cv2geojson-0.0.9/src/cv2geojson/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:27:02.012669 cv2geojson-0.0.9/src/cv2geojson.egg-info/
+-rw-rw-rw-   0        0        0    11615 2023-06-11 21:27:01.000000 cv2geojson-0.0.9/src/cv2geojson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-11 21:27:01.000000 cv2geojson-0.0.9/src/cv2geojson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:27:01.000000 cv2geojson-0.0.9/src/cv2geojson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-11 21:27:01.000000 cv2geojson-0.0.9/src/cv2geojson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 21:27:01.000000 cv2geojson-0.0.9/src/cv2geojson.egg-info/top_level.txt
```

### Comparing `cv2geojson-0.0.8/LICENSE` & `cv2geojson-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cv2geojson-0.0.8/pyproject.toml` & `cv2geojson-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cv2geojson"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Mohsen Farzi", email="mhnfarzi@gmail.com" },
 ]
 description = "Export contour annotations as geojson formatted data"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=['opencv-python', 'numpy', 'geojson']
```

### Comparing `cv2geojson-0.0.8/src/cv2geojson/__init__.py` & `cv2geojson-0.0.9/src/cv2geojson/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,15 @@
         elif geometry is not None:
             self.contours = self._geometry_to_contour(geometry)
             self.type = geometry['type']
         else:
             raise ValueError("Either contour or geometry must be provided.")
 
     def __repr__(self):
-        geometry = self.export_geometry()
-        return f'{geometry}'
+        return 'cv2geojson.GeoContour.{}'.format(self.type)
 
     @staticmethod
     def _get_geometry_type(contours):
         # define the geometry type
         area = cv.contourArea(contours[0])
         if len(contours) > 1 or area > 0:
             # this is a Polygon
@@ -99,49 +98,35 @@
         return geometry
 
     def export_feature(self, color=None, label=None, name=None):
         geometry = self.export_geometry()
         properties = {'object_type': 'annotation'}
         classification = {}
         if color is not None:
-            classification['colorRGB'] = pack_rgb(color)
+            classification['colorRGB'] = _pack_rgb(color)
         if label is not None:
             classification['name'] = label
         if len(classification) > 0:
             properties['classification'] = classification
         if name is not None:
             properties['name'] = name
         feature = geojson.Feature(geometry=geometry, properties=properties)
         return feature
 
-    def scale_down(self, ratio=None, offset=None):
+    def scale_down(self, ratio=1, offset=(0, 0)):
         # return a new GeoContour instance with the coordinates being downsampled
-        if ratio is None:
-            ratio = 1
-        if offset is None:
-            offset = [0, 0]
-        contours = []
-        for contour in self.contours:
-            contour = np.ndarray.astype(np.round((contour - offset) / ratio), dtype=np.int32)
-            contours.append(contour)
-        return GeoContour(contours=contours)
+        contours = [np.ndarray.astype(np.round((cnt - offset) / ratio), dtype=np.int32) for cnt in self.contours]
+        self.contours = contours
 
-    def scale_up(self, ratio=None, offset=None):
+    def scale_up(self, ratio=1, offset=(0, 0)):
         # return a new GeoContour instance with the coordinates being upsampled
-        if ratio is None:
-            ratio = 1
-        if offset is None:
-            offset = [0, 0]
-        contours = []
-        for contour in self.contours:
-            contour = np.ndarray.astype(np.round((contour * ratio) + offset), dtype=np.int32)
-            contours.append(contour)
-        return GeoContour(contours=contours)
+        contours = [np.ndarray.astype(np.round(cnt * ratio + offset), dtype=np.int32) for cnt in self.contours]
+        self.contours = contours
 
-    def area(self, resolution=1):
+    def area(self, resolution=1.0):
         if self.type in ['Point', 'LineString']:
             return 0
         else:
             area_list = [cv.contourArea(contour) for contour in self.contours]
             area = area_list[0] - np.sum(area_list[1:])
             return area * resolution * resolution
 
@@ -177,17 +162,47 @@
                 aspect_ratio = float(rect_width) / rect_height
             else:
                 aspect_ratio = float(rect_height) / rect_width
         else:
             aspect_ratio = 0
         return aspect_ratio
 
+    def elongation(self):
+        moments = cv.moments(self.contours[0])
+        x = moments['mu20'] + moments['mu02']
+        y = np.sqrt(4 * moments['mu11']**2 + (moments['mu20'] - moments['mu02'])**2)
+        elongation = (x - y) / (x + y)
+        return elongation
+
     def holes_num(self):
         return len(self.contours) - 1
 
+    def fill_hole(self, resolution=1.0, hole_size=-1.0):
+        # check if any holes exist
+        if self.holes_num() > 0:
+            if hole_size < 0:
+                # Remove all holes
+                self.contours = [self.contours[0]]
+            elif hole_size > 0:
+                # all holes smaller than hole_size will be removed
+                contours = [self.contours[0]]
+                for hole in self.contours[1:]:
+                    hole_area = cv.contourArea(hole) * resolution * resolution
+                    if hole_area > hole_size:
+                        contours.append(hole)
+                # update the contours
+                self.contours = contours
+            # otherwise do nothing
+
+    def copy(self):
+        return GeoContour(contours=self.contours)
+
+    def get_contours(self, scale=1, offset=(0, 0)):
+        return [np.ndarray.astype(np.round((cnt - offset) / scale), dtype=np.int32) for cnt in self.contours]
+
 
 def simplify(obj):
     """
     Convert a geojson object to a list of geometries with types Polygon, Point, or LineString
 
     :param obj: A geojson object
     :return geometries: A list of geometries of type geojson.Point or geojson.Polygon, or geojson.LineString
@@ -207,24 +222,32 @@
     if obj['type'] == 'MultiLineString':
         geometries = [geojson.LineString(coordinates) for coordinates in obj['coordinates']]
         return geometries
 
     if obj['type'] == 'GeometryCollection':
         geometries = []
         for geometry in obj['geometries']:
-            geometries.append(simplify(geometry))
+            g = simplify(geometry)
+            if type(g) == list:
+                geometries.extend(g)
+            else:
+                geometries.append(g)
         return geometries
 
     if obj['type'] == 'Feature':
         return simplify(obj['geometry'])
 
     if obj['type'] == 'FeatureCollection':
         geometries = []
         for feature in obj['features']:
-            geometries.append(simplify(feature['geometry']))
+            g = simplify(feature['geometry'])
+            if type(g) == list:
+                geometries.extend(g)
+            else:
+                geometries.append(g)
         return geometries
 
 
 def contour_to_geocontour(contours, hierarchy):
     """
     Convert contours extracted using cv.findCountours to cv2geojson.GeoContours
     """
@@ -238,38 +261,38 @@
             for child in children:
                 cnt.append(contours[child])
             geocontours.append(GeoContour(contours=cnt))
 
     return geocontours
 
 
-def load_annotations(path_to_file):
+def load_annotations(path_to_geojson):
     """
     return a list of geocontours from a geojson file
     """
-    with open(path_to_file, 'r') as reader:
+    with open(path_to_geojson, 'r') as reader:
         annotations = geojson.load(reader)
 
     geometries = simplify(annotations)
     geocontours = [GeoContour(geometry=geometry) for geometry in geometries]
     return geocontours
 
 
-def export_annotations(features, path_to_file):
+def export_annotations(features, path_to_geojson):
     """
     Export features formatted by geojson python package
     :param features: a list of 'geojson.Feature' objects
     :param path_to_file:
     """
     # check the validity of the feature list
     for feature in features:
         assert feature.is_valid, f'Input feature is not valid: {feature.errors()}.'
 
     annotations = geojson.FeatureCollection(features=features)
-    with open(path_to_file, 'w') as writer:
+    with open(path_to_geojson, 'w') as writer:
         geojson.dump(annotations, writer)
 
 
 def find_geocontours(mask, mode='opencv'):
     """
     Return GeoContours from input binary mask
     :param mask: A numpy array of selected ROI [either 255 or 0]
@@ -289,41 +312,41 @@
     else:
         raise ValueError('Invalid value for mode:.must be either opencv or imagej')
 
     geocontours = contour_to_geocontour(contours, hierarchy)
     return geocontours
 
 
-def draw_geocontours(mask, geocontours, mode='opencv'):
+def draw_geocontours(mask, geocontours, scale=1, offset=(0, 0), mode='opencv'):
     """
     Draw geocontours into the mask and return a new binary mask
     """
     assert mode == 'opencv' or mode == 'imagej', 'Invalid value for mode:.must be either opencv or imagej'
 
     if mode == 'opencv':
         for geometry in geocontours:
-            cv.drawContours(mask, geometry.contours, -1, 255, -1)
-        return mask
+            cv.drawContours(mask, geometry.get_contours(scale=scale, offset=offset), -1, 255, -1)
 
     if mode == 'imagej':
         mask2 = cv.resize(mask, dsize=(mask.shape[1]*2, mask.shape[0]*2), interpolation=cv.INTER_NEAREST)
-        geocontours2 = [geometry.scale_up(ratio=2, offset=[-1, -1]) for geometry in geocontours]
-        for geometry in geocontours2:
-            cv.drawContours(mask2, geometry.contours, -1, 255, -1)
-        mask = cv.resize(mask2, dsize=mask.shape, interpolation=cv.INTER_NEAREST)
-        return mask
+        for geometry in geocontours:
+            contours = geometry.get_contours(scale=scale, offset=offset)
+            contours = [np.ndarray.astype(np.round(cnt * 2 - [1, 1]), dtype=np.int32) for cnt in contours]
+            cv.drawContours(mask2, contours, -1, 255, -1)
+        mask1 = cv.resize(mask2, dsize=(mask.shape[1], mask.shape[0]), interpolation=cv.INTER_NEAREST)
+        mask[mask1 == 255] = 255
 
 
-def pack_rgb(color):
+def _pack_rgb(color):
     r, g, b = color
     value = (0xff << 24) + ((r & 0xff) << 16) + ((g & 0xff) << 8) + (b & 0xff)
     return value - 4294967296
 
 
-def get_rgb(value):
+def _get_rgb(value):
     value += 4294967296
     value -= (0xff << 24)
     b = value % 256
     value -= b
     value = int(value / 256)
     g = value % 256
     value -= g
```

