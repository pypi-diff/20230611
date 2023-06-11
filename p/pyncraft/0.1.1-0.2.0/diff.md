# Comparing `tmp/pyncraft-0.1.1.tar.gz` & `tmp/pyncraft-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncraft-0.1.1.tar", last modified: Wed Jun  7 04:13:54 2023, max compression
+gzip compressed data, was "pyncraft-0.2.0.tar", last modified: Sun Jun 11 03:08:48 2023, max compression
```

## Comparing `pyncraft-0.1.1.tar` & `pyncraft-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 04:13:54.760940 pyncraft-0.1.1/
--rw-rw-rw-   0        0        0    11558 2023-06-06 03:05:16.000000 pyncraft-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1334 2023-06-07 04:13:54.757962 pyncraft-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-06-07 01:53:06.000000 pyncraft-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 04:13:54.741295 pyncraft-0.1.1/pyncraft/
--rw-rw-rw-   0        0        0        0 2023-06-02 17:29:00.000000 pyncraft-0.1.1/pyncraft/__init__.py
--rw-rw-rw-   0        0        0     2993 2023-06-02 17:29:00.000000 pyncraft-0.1.1/pyncraft/block.py
--rw-rw-rw-   0        0        0     1956 2023-06-03 02:32:24.000000 pyncraft-0.1.1/pyncraft/connection.py
--rw-rw-rw-   0        0        0     3404 2023-06-02 17:29:01.000000 pyncraft-0.1.1/pyncraft/entity.py
--rw-rw-rw-   0        0        0     1807 2023-06-02 17:29:01.000000 pyncraft-0.1.1/pyncraft/event.py
--rw-rw-rw-   0        0        0      777 2023-06-02 18:21:46.000000 pyncraft-0.1.1/pyncraft/logger.py
--rw-rw-rw-   0        0        0    14665 2023-06-05 01:37:25.000000 pyncraft-0.1.1/pyncraft/minecraft.py
--rw-rw-rw-   0        0        0      159 2023-06-02 18:22:17.000000 pyncraft-0.1.1/pyncraft/settings.py
--rw-rw-rw-   0        0        0      487 2023-06-02 17:29:00.000000 pyncraft-0.1.1/pyncraft/util.py
--rw-rw-rw-   0        0        0     2458 2023-06-02 17:29:00.000000 pyncraft-0.1.1/pyncraft/vec3.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:13:54.755875 pyncraft-0.1.1/pyncraft.egg-info/
--rw-rw-rw-   0        0        0     1334 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 04:13:54.760940 pyncraft-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     9508 2023-06-07 04:09:23.000000 pyncraft-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 03:08:48.364900 pyncraft-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-06 03:05:16.000000 pyncraft-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1334 2023-06-11 03:08:48.363909 pyncraft-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-06-07 01:53:06.000000 pyncraft-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 03:08:48.318065 pyncraft-0.2.0/pyncraft/
+-rw-rw-rw-   0        0        0        0 2023-06-02 17:29:00.000000 pyncraft-0.2.0/pyncraft/__init__.py
+-rw-rw-rw-   0        0        0     2993 2023-06-02 17:29:00.000000 pyncraft-0.2.0/pyncraft/block.py
+-rw-rw-rw-   0        0        0     1956 2023-06-03 02:32:24.000000 pyncraft-0.2.0/pyncraft/connection.py
+-rw-rw-rw-   0        0        0     3404 2023-06-02 17:29:01.000000 pyncraft-0.2.0/pyncraft/entity.py
+-rw-rw-rw-   0        0        0     1807 2023-06-02 17:29:01.000000 pyncraft-0.2.0/pyncraft/event.py
+-rw-rw-rw-   0        0        0      777 2023-06-02 18:21:46.000000 pyncraft-0.2.0/pyncraft/logger.py
+-rw-rw-rw-   0        0        0    14748 2023-06-10 03:53:51.000000 pyncraft-0.2.0/pyncraft/minecraft.py
+-rw-rw-rw-   0        0        0      159 2023-06-02 18:22:17.000000 pyncraft-0.2.0/pyncraft/settings.py
+-rw-rw-rw-   0        0        0      487 2023-06-02 17:29:00.000000 pyncraft-0.2.0/pyncraft/util.py
+-rw-rw-rw-   0        0        0     2458 2023-06-02 17:29:00.000000 pyncraft-0.2.0/pyncraft/vec3.py
+drwxrwxrwx   0        0        0        0 2023-06-11 03:08:48.360463 pyncraft-0.2.0/pyncraft.egg-info/
+-rw-rw-rw-   0        0        0     1334 2023-06-11 03:08:47.000000 pyncraft-0.2.0/pyncraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-06-11 03:08:48.000000 pyncraft-0.2.0/pyncraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 03:08:47.000000 pyncraft-0.2.0/pyncraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-11 03:08:47.000000 pyncraft-0.2.0/pyncraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 03:08:47.000000 pyncraft-0.2.0/pyncraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 03:08:48.366954 pyncraft-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     9508 2023-06-11 02:56:37.000000 pyncraft-0.2.0/setup.py
```

### Comparing `pyncraft-0.1.1/LICENSE` & `pyncraft-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.1/PKG-INFO` & `pyncraft-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyncraft
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python interface to minecraft + pyncraft bukkit plugin
 Home-page: https://github.com/jdeast/pyncraft
 Author: Jason Eastman
 Author-email: jdeast@gmail.com
 License: UNKNOWN
 Keywords: minecraft,plugin,scratch,java,bukkit
 Platform: UNKNOWN
```

### Comparing `pyncraft-0.1.1/pyncraft/block.py` & `pyncraft-0.2.0/pyncraft/block.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.1/pyncraft/connection.py` & `pyncraft-0.2.0/pyncraft/connection.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.1/pyncraft/entity.py` & `pyncraft-0.2.0/pyncraft/entity.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.1/pyncraft/event.py` & `pyncraft-0.2.0/pyncraft/event.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.1/pyncraft/logger.py` & `pyncraft-0.2.0/pyncraft/logger.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.1/pyncraft/minecraft.py` & `pyncraft-0.2.0/pyncraft/minecraft.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,17 +237,18 @@
         for i in range(0,totalSize,xSize*ySize):
             curArr = []
             for j in range(0,xSize*ySize,xSize):
                 curArr.append(arr1d[i+j:i+j+xSize])
             arr3d.append(curArr)
         return arr3d
 
-    def setBlock(self, x:int, y:int, z:int, block:str) -> None:
-        """Set block (x,y,z,id,[data])"""
-        self.conn.send(b"world.setBlock", x, y, z, block)
+    # DIRECTION: NORTH SOUTH EAST WEST
+    # FACE: FLOOR, CEILING, WALL
+    def setBlock(self, x:int, y:int, z:int, block:str,direction:str="WEST",face:str="WALL") -> None:
+        self.conn.send(b"world.setBlock", x, y, z, block, direction,face)
 
     def setBlocks(self, x1:int, y1:int, z1:int, x2:int, y2:int, z2:int, block) -> None: 
         """Set a cuboid of blocks (x1,y1,z1,x2,y2,z2,id,[data])"""
         self.conn.send(b"world.setBlocks", x1, y1, z1, x2, y2, z2, block)
 
     def getHeight(self, x:int, z:int) -> int:
         """Get the height of the world (x,z) => int"""
```

### Comparing `pyncraft-0.1.1/pyncraft/vec3.py` & `pyncraft-0.2.0/pyncraft/vec3.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.1/pyncraft.egg-info/PKG-INFO` & `pyncraft-0.2.0/pyncraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyncraft
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python interface to minecraft + pyncraft bukkit plugin
 Home-page: https://github.com/jdeast/pyncraft
 Author: Jason Eastman
 Author-email: jdeast@gmail.com
 License: UNKNOWN
 Keywords: minecraft,plugin,scratch,java,bukkit
 Platform: UNKNOWN
```

### Comparing `pyncraft-0.1.1/setup.py` & `pyncraft-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.1.1',  # Required
+    version='0.2.0',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python interface to minecraft + pyncraft bukkit plugin',  # Optional
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
```

