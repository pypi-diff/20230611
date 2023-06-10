# Comparing `tmp/pyvantage-0.0.52.tar.gz` & `tmp/pyvantage-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvantage-0.0.52.tar", last modified: Sat Jun 10 21:07:00 2023, max compression
+gzip compressed data, was "pyvantage-0.0.54.tar", last modified: Sat Jun 10 23:36:02 2023, max compression
```

## Comparing `pyvantage-0.0.52.tar` & `pyvantage-0.0.54.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 21:07:00.890995 pyvantage-0.0.52/
--rw-r--r--   0 greg       (501) staff       (20)     1179 2021-06-03 17:37:04.000000 pyvantage-0.0.52/LICENSE
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-06-10 21:07:00.891090 pyvantage-0.0.52/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     2164 2023-04-23 17:44:30.000000 pyvantage-0.0.52/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 21:07:00.887921 pyvantage-0.0.52/pyvantage/
--rw-r--r--   0 greg       (501) staff       (20)   103182 2023-06-10 21:04:47.000000 pyvantage-0.0.52/pyvantage/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 21:07:00.890344 pyvantage-0.0.52/pyvantage.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-06-10 21:07:00.000000 pyvantage-0.0.52/pyvantage.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      218 2023-06-10 21:07:00.000000 pyvantage-0.0.52/pyvantage.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 21:07:00.000000 pyvantage-0.0.52/pyvantage.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       10 2023-06-10 21:07:00.000000 pyvantage-0.0.52/pyvantage.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-23 18:11:37.000000 pyvantage-0.0.52/pyvantage.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2023-06-10 21:07:00.891452 pyvantage-0.0.52/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      769 2023-06-10 20:46:11.000000 pyvantage-0.0.52/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 23:36:02.827789 pyvantage-0.0.54/
+-rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.54/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-06-10 23:36:02.828106 pyvantage-0.0.54/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.54/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 23:36:02.824722 pyvantage-0.0.54/pyvantage/
+-rw-r--r--   0 greg       (501) staff       (20)   103376 2023-06-10 23:35:46.000000 pyvantage-0.0.54/pyvantage/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 23:36:02.826852 pyvantage-0.0.54/pyvantage.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-06-10 23:36:02.000000 pyvantage-0.0.54/pyvantage.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      218 2023-06-10 23:36:02.000000 pyvantage-0.0.54/pyvantage.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 23:36:02.000000 pyvantage-0.0.54/pyvantage.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       10 2023-06-10 23:36:02.000000 pyvantage-0.0.54/pyvantage.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.54/pyvantage.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-06-10 23:36:02.828605 pyvantage-0.0.54/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      769 2023-06-10 23:35:46.000000 pyvantage-0.0.54/setup.py
```

### Comparing `pyvantage-0.0.52/LICENSE` & `pyvantage-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.52/PKG-INFO` & `pyvantage-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.52
+Version: 0.0.54
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.52/README.md` & `pyvantage-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.52/pyvantage/__init__.py` & `pyvantage-0.0.54/pyvantage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,21 @@
                     break
                 new_chunk = self._sockets[i].recv(1024)
                 if not new_chunk:
                     break
                 self._chunk += new_chunk
         except socket.timeout:
             pass
-        [data, self._chunk] = self._chunk.split(delimiter, 1)
+        data_and_rest = self._chunk.split(delimiter, 1)
+        if len(data_and_rest) == 1:
+            data = data_and_rest[0]
+            self._chunk = b''
+        else:
+            [data, self._chunk] = data_and_rest
+
         return data
 
     def _do_login_locked(self, i):
         """Executes the login procedure as well as setting up some
         connection defaults like turning off the prompt, etc."""
         while True:
             try:
@@ -1943,15 +1949,15 @@
         (r, g, b) = self._rgb
         ratio = self._level/100
         self._vantage.send("INVOKE", self._vid,
                            ("RGBLoad.SetRGBW %d %d %d %d" %
                             (round(r*ratio), round(g*ratio), round(b*ratio), 0)))
         if self._dmx_color and self._level > 0:
             _LOGGER.debug('_invoke_rgb calling rampload to ensure dmx change is triggered')
-            self._vantage.send("RAMPLOAD", self._vid, self._level, 0.1)
+            self._vantage.send("RAMPLOAD", self._vid, round(self._level), 0.1)
 
         if self._level > 0:
             self._rgb_is_dirty = False
 
     @property
     # hue is scaled 0-360, saturation is 0-100
     def hs(self):
@@ -1974,15 +1980,15 @@
         It's worth noting that HS still specifies a color even when the light is off."""
         (h, s) = self._hs
         self._vantage.send("INVOKE", self._vid,
                            ("RGBLoad.SetHSL %d %d %d" %
                             (h, s, self._level)))
         if self._dmx_color and self._level > 0:
             _LOGGER.debug('_invoke_hs calling rampload to ensure dmx change is triggered')
-            self._vantage.send("RAMPLOAD", self._vid, self._level, 0.1)
+            self._vantage.send("RAMPLOAD", self._vid, round(self._level), 0.1)
 
         if self._level > 0:
             self._rgb_is_dirty = False
 
     @property
     def color_temp(self):
         """Returns the current output level by querying the controller."""
@@ -1998,15 +2004,15 @@
             return
         if self._dmx_color or self._load_type == "DW":
             rgb = kelvin_to_rgb(new_color_temp)
             _LOGGER.debug("%s: Using rgb of %s for call to setter for color_temp "
                           "%s of dmx_color light", self, rgb, new_color_temp)
             self.rgb = rgb
         self._vantage.send("RAMPLOAD", self._color_control_vid,
-                            kelvin_to_level(new_color_temp),
+                            round(kelvin_to_level(new_color_temp)),
                             self._ramp_sec[2])
         self._color_temp = new_color_temp
 
 # At some later date, we may want to also specify fade and delay times
 #  def set_level(self, new_level, fade_time, delay):
 #    self._vantage.send(Vantage.OP_EXECUTE, Output.CMD_TYPE,
 #        Output.ACTION_ZONE_LEVEL, new_level, fade_time, delay)
@@ -2363,28 +2369,28 @@
         ratio = self._level/100
         for vid in self._load_vids:
             load = self._vantage._vid_to_load.get(vid)
             if load and (load._dmx_color or load._load_type == "DW"):
                 self._vantage.send("INVOKE", vid,
                                    ("RGBLoad.SetRGBW %d %d %d %d" %
                                     (r*ratio, g*ratio, b*ratio, 0)))
-                self._vantage.send("RAMPLOAD", vid, self._level, 0.1)
+                self._vantage.send("RAMPLOAD", vid, round(self._level), 0.1)
         if self._level > 0:
             self._rgb_is_dirty = False
 
     def _invoke_hs(self):
         """Update the RGB of the load group to self._rgb"""
         (h, s) = self._hs
         for vid in self._load_vids:
             load = self._vantage._vid_to_load.get(vid)
             if load and (load._dmx_color or load._load_type == "DW"):
                 self._vantage.send("INVOKE", vid,
                                    ("RGBLoad.SetHSL %d %d %d" %
                                     (h, s, self._level-1)))
-                self._vantage.send("RAMPLOAD", vid, self._level, 0.1)
+                self._vantage.send("RAMPLOAD", vid, round(self._level), 0.1)
 
     def __do_query_level(self):
         """Helper to perform the actual query the current dimmer level of the
         output. For pure on/off loads the result is either 0.0 or 100.0."""
         if self.support_color and not self._addedstatus:
             _LOGGER.debug("Using first color_vid = %s to ADDSTATUS for %s",
                           self._color_vids[0], self._vid)
```

### Comparing `pyvantage-0.0.52/pyvantage.egg-info/PKG-INFO` & `pyvantage-0.0.54/pyvantage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.52
+Version: 0.0.54
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.52/setup.py` & `pyvantage-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyvantage',
-    version='0.0.52',
+    version='0.0.54',
     license='MIT',
     description='Python library for Vantage Controller (for Home Assistant)',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyvantage',
     packages=find_packages(),
     classifiers=[
```

