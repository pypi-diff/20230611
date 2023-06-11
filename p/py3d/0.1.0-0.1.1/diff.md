# Comparing `tmp/py3d-0.1.0.tar.gz` & `tmp/py3d-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.0.tar", last modified: Fri Jun  9 00:54:13 2023, max compression
+gzip compressed data, was "py3d-0.1.1.tar", last modified: Sun Jun 11 15:16:41 2023, max compression
```

## Comparing `py3d-0.1.0.tar` & `py3d-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:54:13.035212 py3d-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-09 00:54:13.035212 py3d-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-09 00:53:51.000000 py3d-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:54:13.035212 py3d-0.1.0/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-09 00:53:09.000000 py3d-0.1.0/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28585 2023-06-09 00:53:09.000000 py3d-0.1.0/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-06-09 00:53:09.000000 py3d-0.1.0/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:54:13.035212 py3d-0.1.0/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 00:54:13.035212 py3d-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-09 00:53:09.000000 py3d-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 15:16:41.660717 py3d-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-11 15:16:41.660717 py3d-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-11 15:16:21.000000 py3d-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 15:16:41.660717 py3d-0.1.1/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-11 15:15:38.000000 py3d-0.1.1/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28565 2023-06-11 15:15:38.000000 py3d-0.1.1/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-06-11 15:15:38.000000 py3d-0.1.1/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 15:16:41.660717 py3d-0.1.1/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-11 15:16:41.000000 py3d-0.1.1/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-11 15:16:41.660717 py3d-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-11 15:15:38.000000 py3d-0.1.1/setup.py
```

### Comparing `py3d-0.1.0/PKG-INFO` & `py3d-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.0
+Version: 0.1.1
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.0/README.md` & `py3d-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.0/py3d/core.py` & `py3d-0.1.1/py3d/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,16 @@
         self[..., 0:3] = v
 
     @property
     def U(self) -> Vector | Vector2 | Vector3 | Vector4:
         '''
         unit vector, direction vector
         '''
-        n = self.L
-        return numpy.divide(self, n, where=n != 0)
+        l = numpy.linalg.norm(self, axis=self.ndim - 1, keepdims=True)
+        return numpy.divide(self, l, where=l != 0)
 
     @property
     def H(self) -> Vector | Vector2 | Vector3 | Vector4:
         '''
         Homogeneous vector
         '''
         ret = numpy.insert(self, self.shape[-1], 1, axis=self.ndim-1)
@@ -249,15 +249,15 @@
     def M(self) -> Vector | Vector2 | Vector3 | Vector4:
         # mean vector
         return super().mean(axis=self.ndim-2)
 
     @property
     def L(self) -> Vector:
         # length
-        return numpy.linalg.norm(self, axis=self.ndim - 1, keepdims=True)
+        return numpy.linalg.norm(self, axis=self.ndim - 1)
 
     def min(self) -> Vector:
         return super().min(axis=self.ndim-2)
 
     def max(self) -> Vector:
         return super().max(axis=self.ndim-2)
 
@@ -330,22 +330,19 @@
         a = numpy.linspace(0, 2*numpy.pi, segments, False)
         return cls(x=radius * numpy.sin(a), y=radius * numpy.cos(a))
 
     def __matmul__(self, value: Transform) -> Vector3:
         if type(value) is Transform:
             return numpy.matmul(self.H, value)[..., 0:3].view(Vector3)
         else:
-            return self.__matmul__(value)
+            return super().__matmul__(value)
 
-    def dot(self, v) -> Vector3:
-        if type(v) is Vector3:
-            product = self * v
-            return product.sum(axis=product.ndim - 1, keepdims=True).view(numpy.ndarray)
-        else:
-            return numpy.dot(self, v)
+    def dot(self, v) -> Vector:
+        product = self * v
+        return numpy.sum(product, axis=product.ndim - 1).view(Vector)
 
     def cross(self, v: numpy.ndarray) -> Vector3:
         return numpy.cross(self, v).view(self.__class__)
 
     def angle_to_vector(self, to: numpy.ndarray) -> Vector3:
         cos = self.dot(to) / self.L / Vector3(to).L
         return numpy.arccos(cos)
@@ -362,18 +359,19 @@
     def is_perpendicular_to_vector(self, v: numpy.ndarray) -> bool:
         return self.dot(v) == 0
 
     def is_perpendicular_to_plane(self, normal: numpy.ndarray) -> bool:
         return self.is_parallel_to_vector(normal)
 
     def scalar_projection(self, v: numpy.ndarray) -> float:
-        return self.dot(v) / v.L
+        return self.dot(v) / Vector3(v).L
 
     def vector_projection(self, v: numpy.ndarray) -> Vector3:
-        return self.scalar_projection(v) * v / v.L
+        s = self.scalar_projection(v) / Vector3(v).L
+        return s.reshape(-1, 1) * v
 
     def distance_to_line(self, p0: numpy.ndarray, p1: numpy.ndarray) -> float:
         v0 = p1 - p0
         v1 = self - p0
         return v0.cross(v1).L / v0.L
 
     def distance_to_plane(self, n: numpy.ndarray, p: numpy.ndarray) -> float:
```

### Comparing `py3d-0.1.0/py3d/viewer.html` & `py3d-0.1.1/py3d/viewer.html`

 * *Files identical despite different names*

### Comparing `py3d-0.1.0/py3d.egg-info/PKG-INFO` & `py3d-0.1.1/py3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.0
+Version: 0.1.1
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.0/setup.py` & `py3d-0.1.1/setup.py`

 * *Files identical despite different names*

