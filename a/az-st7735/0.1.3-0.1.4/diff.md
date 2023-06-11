# Comparing `tmp/az-st7735-0.1.3.tar.gz` & `tmp/az-st7735-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "az-st7735-0.1.3.tar", last modified: Sat Jun 10 13:16:55 2023, max compression
+gzip compressed data, was "az-st7735-0.1.4.tar", last modified: Sun Jun 11 10:06:08 2023, max compression
```

## Comparing `az-st7735-0.1.3.tar` & `az-st7735-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:16:55.213199 az-st7735-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 13:16:26.000000 az-st7735-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 13:16:55.213199 az-st7735-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 13:16:26.000000 az-st7735-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-10 13:16:26.000000 az-st7735-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-10 13:16:55.213199 az-st7735-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:16:55.209199 az-st7735-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:16:55.209199 az-st7735-0.1.3/src/az_st7735.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 13:16:55.000000 az-st7735-0.1.3/src/az_st7735.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-10 13:16:55.000000 az-st7735-0.1.3/src/az_st7735.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:16:55.000000 az-st7735-0.1.3/src/az_st7735.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 13:16:55.000000 az-st7735-0.1.3/src/az_st7735.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:16:55.213199 az-st7735-0.1.3/src/azst7735/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 13:16:26.000000 az-st7735-0.1.3/src/azst7735/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-06-10 13:16:26.000000 az-st7735-0.1.3/src/azst7735/st7735.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:06:08.489839 az-st7735-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-11 10:05:36.000000 az-st7735-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-11 10:06:08.489839 az-st7735-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-11 10:05:36.000000 az-st7735-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-11 10:05:36.000000 az-st7735-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-11 10:06:08.489839 az-st7735-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:06:08.485839 az-st7735-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:06:08.489839 az-st7735-0.1.4/src/az_st7735.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-11 10:06:08.000000 az-st7735-0.1.4/src/az_st7735.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-11 10:06:08.000000 az-st7735-0.1.4/src/az_st7735.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:06:08.000000 az-st7735-0.1.4/src/az_st7735.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 10:06:08.000000 az-st7735-0.1.4/src/az_st7735.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:06:08.489839 az-st7735-0.1.4/src/azst7735/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:05:36.000000 az-st7735-0.1.4/src/azst7735/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-06-11 10:05:36.000000 az-st7735-0.1.4/src/azst7735/st7735.py
```

### Comparing `az-st7735-0.1.3/LICENSE` & `az-st7735-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `az-st7735-0.1.3/PKG-INFO` & `az-st7735-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: az-st7735
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library for the ST7735 controlled 1.8inch display from AZ-Delivery
 Home-page: https://github.com/mrbluesky125/az-st7735
 Author: Timo Zimmermann
 Author-email: github@timozimmermann.de
 Project-URL: Bug Tracker, https://github.com/mrbluesky125/az-st7735/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `az-st7735-0.1.3/setup.cfg` & `az-st7735-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = az-st7735
-version = 0.1.3
+version = 0.1.4
 author = Timo Zimmermann
 author_email = github@timozimmermann.de
 description = Python library for the ST7735 controlled 1.8inch display from AZ-Delivery
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mrbluesky125/az-st7735
 project_urls =
```

### Comparing `az-st7735-0.1.3/src/az_st7735.egg-info/PKG-INFO` & `az-st7735-0.1.4/src/az_st7735.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: az-st7735
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library for the ST7735 controlled 1.8inch display from AZ-Delivery
 Home-page: https://github.com/mrbluesky125/az-st7735
 Author: Timo Zimmermann
 Author-email: github@timozimmermann.de
 Project-URL: Bug Tracker, https://github.com/mrbluesky125/az-st7735/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `az-st7735-0.1.3/src/azst7735/st7735.py` & `az-st7735-0.1.4/src/azst7735/st7735.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numbers
 import time
 import numpy as np
 
 import spidev
 import RPi.GPIO as GPIO
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 SPI_CLOCK_HZ = 16000000
 
 # Constants for interacting with display registers.
 ST7735_TFTWIDTH = 128
 ST7735_TFTHEIGHT = 160
 
@@ -88,36 +88,27 @@
 ST7735_RED = 0xF800  # 0b 11111 000000 00000
 ST7735_CYAN = 0x07FF  # 0b 00000 111111 11111
 ST7735_MAGENTA = 0xF81F  # 0b 11111 000000 11111
 ST7735_YELLOW = 0xFFE0  # 0b 11111 111111 00000
 ST7735_WHITE = 0xFFFF  # 0b 11111 111111 11111
 
 
-def image_to_data(image, rotation=0):
-    """Generator function to convert a PIL image to 16-bit 565 RGB bytes."""
-    # NumPy is much faster at doing this. NumPy code provided by:
-    # Keith (https://www.blogger.com/profile/02555547344016007163)
-    pb = np.rot90(np.array(image.convert('RGB')), rotation // 90).astype('uint16')
-    color = ((pb[:, :, 0] & 0xF8) << 8) | ((pb[:, :, 1] & 0xFC) << 3) | (pb[:, :, 2] >> 3)
-    return np.dstack(((color >> 8) & 0xFF, color & 0xFF)).flatten().tolist()
-
-
 class ST7735(object):
     """Representation of an ST7735 TFT LCD."""
 
     def __init__(self, port, cs, dc, rst=None, width=ST7735_TFTWIDTH,
-                 height=ST7735_TFTHEIGHT, invert=True, spi_speed_hz=4000000):
+                 height=ST7735_TFTHEIGHT, invert=True, spi_speed_hz=SPI_CLOCK_HZ):
         """Create an instance of the display using SPI communication.
 
         Must provide the GPIO pin number for the D/C pin and the SPI driver.
 
         Can optionally provide the GPIO pin number for the reset pin as the rst parameter.
 
         :param port: SPI port number
-        :param cs: SPI chip-select number (0 or 1 for BCM
+        :param cs: SPI chip-select number (0 or 1 for BCM) or any usable GPIO
         :param backlight: Pin for controlling backlight
         :param rst: Reset pin for ST7735
         :param width: Width of display connected to ST7735
         :param height: Height of display connected to ST7735
         :param invert: Invert display
         :param spi_speed_hz: SPI speed (in Hz)
 
@@ -149,14 +140,15 @@
         # Setup reset as output (if provided).
         if rst is not None:
             GPIO.setup(rst, GPIO.OUT)
 
         if self._cs is not None:
             GPIO.setup(self._cs, GPIO.OUT)
             GPIO.output(self._cs, 1)
+            self._spi.no_cs = True
 
         self.reset()
         self._init()
 
     def send(self, data, is_data=True, chunk_size=4096):
         """Write a byte or array of bytes to the display. Is_data parameter
         controls if byte should be interpreted as display data (True) or command
@@ -319,18 +311,26 @@
 
         self.command(ST7735_NORON)      # Normal display on
         time.sleep(0.10)                # 10 ms
 
         self.command(ST7735_DISPON)     # Display on
         time.sleep(0.100)               # 100 ms
 
+    def image_to_data(self, image):
+        """Generator function to convert a PIL image to hardware specific 16-bit 565 RGB bytes."""
+        # NumPy is much faster at doing this. NumPy code provided by:
+        # Keith (https://www.blogger.com/profile/02555547344016007163)
+        pb = np.array(image.resize((self._width,self._height)).convert('RGB')).astype('uint16')
+        color = ((pb[:, :, 2] & 0xF8) << 8) | ((pb[:, :, 1] & 0xFC) << 3) | (pb[:, :, 0] >> 3)
+        return np.dstack(((color >> 8) & 0xFF, color & 0xFF)).flatten().tolist()
+
     def display(self, image):
         """Write the provided image to the hardware.
 
-        :param image: Should be RGB format and the same dimensions as the display hardware.
+        :param image: Should be RGB format and the same aspect ratio as the display hardware.
 
         """
         self.command(ST7735_RAMWR)       # write to RAM
         # Convert image to array of 16bit 565 RGB data bytes.
         # Unfortunate that this copy has to occur, but the SPI byte writing
         # function needs to take an array of bytes and PIL doesn't natively
         # store images in 16-bit 565 RGB format.
```

