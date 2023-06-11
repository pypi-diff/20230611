# Comparing `tmp/RGBMatrixEmulator-0.8.4.tar.gz` & `tmp/RGBMatrixEmulator-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RGBMatrixEmulator-0.8.4.tar", last modified: Fri Apr 21 20:53:25 2023, max compression
+gzip compressed data, was "dist\RGBMatrixEmulator-0.9.0.tar", last modified: Sun Jun 11 21:36:37 2023, max compression
```

## Comparing `RGBMatrixEmulator-0.8.4.tar` & `RGBMatrixEmulator-0.9.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.694353 RGBMatrixEmulator-0.8.4/
--rw-rw-rw-   0        0        0     1076 2021-04-21 03:23:52.000000 RGBMatrixEmulator-0.8.4/LICENSE
--rw-rw-rw-   0        0        0      370 2022-05-05 17:49:25.000000 RGBMatrixEmulator-0.8.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1733 2023-04-21 20:53:25.693352 RGBMatrixEmulator-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     7066 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.534359 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/
--rw-rw-rw-   0        0        0      219 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.620351 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/
--rw-rw-rw-   0        0        0     1804 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/__init__.py
--rw-rw-rw-   0        0        0     2491 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/base.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.642352 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/
--rw-rw-rw-   0        0        0        0 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/__init__.py
--rw-rw-rw-   0        0        0     2063 2023-04-21 13:59:36.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/adapter.py
--rw-rw-rw-   0        0        0     2774 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/server.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.644352 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.656351 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/
--rw-rw-rw-   0        0        0     3812 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js
--rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico
--rw-rw-rw-   0        0        0      311 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/styles.css
--rw-rw-rw-   0        0        0     5068 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/index.html
--rw-rw-rw-   0        0        0      889 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py
--rw-rw-rw-   0        0        0     2547 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/pygame_adapter.py
--rw-rw-rw-   0        0        0     1387 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/terminal_adapter.py
--rw-rw-rw-   0        0        0     2666 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/tkinter_adapter.py
--rw-rw-rw-   0        0        0     3150 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/turtle_adapter.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.681352 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/
--rw-rw-rw-   0        0        0        0 2021-04-24 19:55:28.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/__init__.py
--rw-rw-rw-   0        0        0     1806 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/canvas.py
--rw-rw-rw-   0        0        0     1449 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/matrix.py
--rw-rw-rw-   0        0        0     7081 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/options.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.692355 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/
--rw-rw-rw-   0        0        0     4460 2023-04-21 13:59:14.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/__init__.py
--rw-rw-rw-   0        0        0      881 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/color.py
--rw-rw-rw-   0        0        0     1085 2022-05-05 19:55:29.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/font.py
--rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/icon.ico
--rw-rw-rw-   0        0        0     8514 2022-06-08 18:26:14.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/icon.png
--rw-rw-rw-   0        0        0      781 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/logger.py
--rw-rw-rw-   0        0        0      114 2023-04-21 13:59:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/version.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.569355 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/
--rw-rw-rw-   0        0        0     1733 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      760 2022-02-05 15:41:33.000000 RGBMatrixEmulator-0.8.4/description.md
--rw-rw-rw-   0        0        0       42 2023-04-21 20:53:25.694353 RGBMatrixEmulator-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0     2117 2022-09-05 03:56:29.000000 RGBMatrixEmulator-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.554601 RGBMatrixEmulator-0.9.0/
+-rw-rw-rw-   0        0        0     1076 2021-04-21 03:23:52.000000 RGBMatrixEmulator-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      370 2022-05-05 17:49:25.000000 RGBMatrixEmulator-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1733 2023-06-11 21:36:37.553600 RGBMatrixEmulator-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7247 2023-06-11 21:34:14.000000 RGBMatrixEmulator-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.463599 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/
+-rw-rw-rw-   0        0        0      219 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.502601 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/
+-rw-rw-rw-   0        0        0     1895 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/__init__.py
+-rw-rw-rw-   0        0        0     2491 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/base.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.508598 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/
+-rw-rw-rw-   0        0        0        0 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/__init__.py
+-rw-rw-rw-   0        0        0     2063 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/adapter.py
+-rw-rw-rw-   0        0        0     2774 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/server.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.517595 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.541597 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/
+-rw-rw-rw-   0        0        0     3812 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js
+-rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico
+-rw-rw-rw-   0        0        0      311 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/styles.css
+-rw-rw-rw-   0        0        0     5068 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/index.html
+-rw-rw-rw-   0        0        0      889 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py
+-rw-rw-rw-   0        0        0     2547 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/pygame_adapter.py
+-rw-rw-rw-   0        0        0     2859 2023-06-11 21:34:14.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/sixel_adapter.py
+-rw-rw-rw-   0        0        0     1387 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/terminal_adapter.py
+-rw-rw-rw-   0        0        0     2666 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/tkinter_adapter.py
+-rw-rw-rw-   0        0        0     3150 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/turtle_adapter.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.547605 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/
+-rw-rw-rw-   0        0        0        0 2021-04-24 19:55:28.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/__init__.py
+-rw-rw-rw-   0        0        0     1806 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/canvas.py
+-rw-rw-rw-   0        0        0     1449 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/matrix.py
+-rw-rw-rw-   0        0        0     7244 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/options.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.551601 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/
+-rw-rw-rw-   0        0        0     4460 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/__init__.py
+-rw-rw-rw-   0        0        0      881 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/color.py
+-rw-rw-rw-   0        0        0     1085 2022-05-05 19:55:29.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/font.py
+-rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/icon.ico
+-rw-rw-rw-   0        0        0     8514 2022-06-08 18:26:14.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/icon.png
+-rw-rw-rw-   0        0        0      781 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/logger.py
+-rw-rw-rw-   0        0        0      114 2023-06-11 21:34:28.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/version.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.490597 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/
+-rw-rw-rw-   0        0        0     1733 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      760 2022-02-05 15:41:33.000000 RGBMatrixEmulator-0.9.0/description.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 21:36:37.554601 RGBMatrixEmulator-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2153 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/setup.py
```

### Comparing `RGBMatrixEmulator-0.8.4/LICENSE` & `RGBMatrixEmulator-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/PKG-INFO` & `RGBMatrixEmulator-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RGBMatrixEmulator
-Version: 0.8.4
+Version: 0.9.0
 Summary: A PC emulator for Raspberry Pi LED matrices driven by rpi-rgb-led-matrix
 Home-page: https://github.com/ty-porter/RGBMatrixEmulator
 Author: Tyler Porter
 Author-email: tyler.b.porter@gmail.com
 License: MIT
 Description: # `RGBMatrixEmulator`
```

### Comparing `RGBMatrixEmulator-0.8.4/README.md` & `RGBMatrixEmulator-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 ## Customization
 
 The first time you run a script with the emulator enabled, a file called `emulator_config.json` will be created in the script's directory. This enables configurations to be customized on a per-script basis. The default configuration is as follows:
 
 ```json
 {
+  "pixel_outline": 0,
   "pixel_size": 16,
   "pixel_style": "square",
   "display_adapter": "pygame",
   "suppress_font_warnings": false,
   "suppress_adapter_load_errors": false,
   "browser": {
     "_comment": "For use with the browser adapter only.",
@@ -60,14 +61,15 @@
   "log_level": "info"
 }
 ```
 
 ### Configuration Options
 
 ```
+pixel_outline          (Integer): Size of the black border around each pixel. Only works on some adapters; others will ignore this configuration.
 pixel_size             (Integer): Size of the emulated LED. Helpful for emulating large matrices on small screens. Actual window size is the matrix size scaled by pixel size.
 pixel_style            (String):  Style of the emulated LED. Supported pixel styles are "square" and "circle". Some display adapters do not support all options and will revert to a supported style.
 display_adapter        (String):  Display adapter for the emulator. See Display Adapters section for details.
 suppress_font_warnings (Boolean): Suppress BDF font parsing errors, such as for missing characters.
 browser                (Dict):    Additional configuration options for the "browser" display adapter. Does nothing for other adapters.
   port                 (Integer): Port for the rendering server to attach to. Example: http://localhost:8888
   target_fps           (Integer): Target frames per second. Higher values may lead to lower performance.
@@ -87,14 +89,15 @@
 Currently supported display adapters are:
 
 * `browser` (default)
 * `pygame`
 * `terminal`
 * `tkinter`
 * `turtle`
+* `sixel`
 
 You can swap display adapters by changing the `display_adapter` value to one of the above in `emulator_config.json`.
 
 **Note:** Not all display adapters support all emulator features. Some adapters may require additional setup steps to install. For example, on OSX, it may be necessary to install `tkinter` via Homebrew (`brew install python-tk`).
 
 ### Browser Display Adapter
```

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/__init__.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import importlib, json
 
 from RGBMatrixEmulator.logger import Logger
 
 adapters = [
     {
-        'path': 'RGBMatrixEmulator.adapters.browser_adapter.adapter', 
-        'class': 'BrowserAdapter', 
+        'path': 'RGBMatrixEmulator.adapters.browser_adapter.adapter',
+        'class': 'BrowserAdapter',
         'type': 'browser'
     },
     {
-        'path': 'RGBMatrixEmulator.adapters.pygame_adapter',          
-        'class': 'PygameAdapter',  
+        'path': 'RGBMatrixEmulator.adapters.pygame_adapter',
+        'class': 'PygameAdapter',
         'type': 'pygame'
     },
     {
-        'path': 'RGBMatrixEmulator.adapters.terminal_adapter',        
+        'path': 'RGBMatrixEmulator.adapters.sixel_adapter',
+        'class': 'SixelAdapter',
+        'type': 'sixel'
+    },
+    {
+        'path': 'RGBMatrixEmulator.adapters.terminal_adapter',
         'class': 'TerminalAdapter',
         'type': 'terminal'
     },
     {
-        'path': 'RGBMatrixEmulator.adapters.tkinter_adapter',         
-        'class': 'TkinterAdapter', 
+        'path': 'RGBMatrixEmulator.adapters.tkinter_adapter',
+        'class': 'TkinterAdapter',
         'type': 'tkinter'
     },
     {
-        'path': 'RGBMatrixEmulator.adapters.turtle_adapter',          
-        'class': 'TurtleAdapter',  
+        'path': 'RGBMatrixEmulator.adapters.turtle_adapter',
+        'class': 'TurtleAdapter',
         'type': 'turtle'
     }
 ]
 
 ADAPTER_TYPES = {}
 
 try:
```

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/base.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/base.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/adapter.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/server.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/server.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/index.html` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/index.html`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/pygame_adapter.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/pygame_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/terminal_adapter.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/terminal_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/tkinter_adapter.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/tkinter_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/turtle_adapter.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/turtle_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/canvas.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/canvas.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/matrix.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/matrix.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/options.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
                     self.pixel_style = emulator_config.pixel_style
                 else:
                     Logger.warning('"{}" pixel style option is not supported by adapter "{}". Defaulting to "square"...'.format(config_pixel_style, emulator_config.display_adapter.lower()))
         else:
             Logger.warning('"{}" pixel style option not recognized. Valid options are "square", "circle". Defaulting to "square"...'.format(config_pixel_style))
 
         self.pixel_size = emulator_config.pixel_size
+        self.pixel_outline = emulator_config.DEFAULT_CONFIG['pixel_outline']
+        self.pixel_outline = emulator_config.pixel_outline
         self.browser = emulator_config.browser
 
         if emulator_config.suppress_font_warnings:
             import bdfparser
 
             bdfparser.warnings.simplefilter("ignore")
 
@@ -76,14 +78,15 @@
 
 class RGBMatrixEmulatorConfig:
 
     __CONFIG_PATH = 'emulator_config.json'
 
     VALID_PIXEL_STYLES = ['square', 'circle']
     DEFAULT_CONFIG = {
+        'pixel_outline': 0,
         'pixel_size': 16,
         'pixel_style': 'square',
         'display_adapter': 'browser',
         'suppress_font_warnings': False,
         'suppress_adapter_load_errors': False,
         'browser': {
             '_comment': 'For use with the browser adapter only.',
@@ -104,15 +107,15 @@
         RGBMatrixEmulatorConfig.Utils.set_attributes(self)
 
     def __load_config(self):
         if os.path.exists(self.__CONFIG_PATH):
             with open(self.__CONFIG_PATH) as f:
                 config = json.load(f)
 
-            return config    
+            return config
 
         with open(self.__CONFIG_PATH, 'w') as f:
             json.dump(self.DEFAULT_CONFIG, f, indent=4)
 
         return self.DEFAULT_CONFIG
 
     def __str__(self):
```

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/__init__.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/color.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/color.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/font.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/font.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/icon.ico` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/icon.ico`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/icon.png` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/icon.png`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/logger.py` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/logger.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/PKG-INFO` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RGBMatrixEmulator
-Version: 0.8.4
+Version: 0.9.0
 Summary: A PC emulator for Raspberry Pi LED matrices driven by rpi-rgb-led-matrix
 Home-page: https://github.com/ty-porter/RGBMatrixEmulator
 Author: Tyler Porter
 Author-email: tyler.b.porter@gmail.com
 License: MIT
 Description: # `RGBMatrixEmulator`
```

### Comparing `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/SOURCES.txt` & `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 RGBMatrixEmulator.egg-info/SOURCES.txt
 RGBMatrixEmulator.egg-info/dependency_links.txt
 RGBMatrixEmulator.egg-info/requires.txt
 RGBMatrixEmulator.egg-info/top_level.txt
 RGBMatrixEmulator/adapters/__init__.py
 RGBMatrixEmulator/adapters/base.py
 RGBMatrixEmulator/adapters/pygame_adapter.py
+RGBMatrixEmulator/adapters/sixel_adapter.py
 RGBMatrixEmulator/adapters/terminal_adapter.py
 RGBMatrixEmulator/adapters/tkinter_adapter.py
 RGBMatrixEmulator/adapters/turtle_adapter.py
 RGBMatrixEmulator/adapters/browser_adapter/__init__.py
 RGBMatrixEmulator/adapters/browser_adapter/adapter.py
 RGBMatrixEmulator/adapters/browser_adapter/server.py
 RGBMatrixEmulator/adapters/browser_adapter/web_socket.py
```

### Comparing `RGBMatrixEmulator-0.8.4/description.md` & `RGBMatrixEmulator-0.9.0/description.md`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.4/setup.py` & `RGBMatrixEmulator-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,11 +56,12 @@
             'RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico',
             'RGBMatrixEmulator/adapters/browser_adapter/static/assets/styles.css',
         ])
     ],
     install_requires=[
         'bdfparser<=2.2.0',
         'pygame>=2.0.1,<3',
-        'tornado>=6.1'
+        'tornado>=6.1',
+        'libsixel-python>=0.5.0',
     ],
     include_package_data=True
 )
```

