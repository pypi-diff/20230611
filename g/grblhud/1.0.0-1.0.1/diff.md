# Comparing `tmp/grblhud-1.0.0.tar.gz` & `tmp/grblhud-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grblhud-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "grblhud-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `grblhud-1.0.0.tar` & `grblhud-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1085 2023-06-10 12:49:32.174417 grblhud-1.0.0/LICENSE
--rw-r--r--   0        0        0     4801 2023-06-10 12:54:18.540823 grblhud-1.0.0/README.md
--rw-r--r--   0        0        0     4801 2023-06-10 12:55:49.202815 grblhud-1.0.0/grblhud/README.md
--rw-r--r--   0        0        0       81 2023-06-10 11:58:10.825254 grblhud-1.0.0/grblhud/__init__.py
--rwxr-xr-x   0        0        0     1476 2023-06-10 11:58:10.835254 grblhud-1.0.0/grblhud/__main__.py
--rw-r--r--   0        0        0    10748 2023-06-10 11:58:10.825254 grblhud-1.0.0/grblhud/grblbuffer.py
--rwxr-xr-x   0        0        0    30180 2023-06-10 11:58:10.825254 grblhud-1.0.0/grblhud/grblhudloop.py
--rw-r--r--   0        0        0     6053 2023-06-10 11:58:10.835254 grblhud-1.0.0/grblhud/grblmessages.py
--rw-r--r--   0        0        0     8040 2023-06-10 11:58:10.835254 grblhud-1.0.0/grblhud/lineinput.py
--rw-r--r--   0        0        0     2994 2023-06-10 11:58:10.825254 grblhud-1.0.0/grblhud/unblockedgetch.py
--rw-r--r--   0        0        0      645 2023-06-10 12:50:36.895883 grblhud-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5290 1970-01-01 00:00:00.000000 grblhud-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-10 12:49:32.174417 grblhud-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4814 2023-06-11 15:58:27.225029 grblhud-1.0.1/README.md
+-rw-r--r--   0        0        0     4801 2023-06-10 12:55:49.202815 grblhud-1.0.1/grblhud/README.md
+-rw-r--r--   0        0        0       81 2023-06-11 15:59:48.216787 grblhud-1.0.1/grblhud/__init__.py
+-rwxr-xr-x   0        0        0     1476 2023-06-10 11:58:10.835254 grblhud-1.0.1/grblhud/__main__.py
+-rw-r--r--   0        0        0    10748 2023-06-10 11:58:10.825254 grblhud-1.0.1/grblhud/grblbuffer.py
+-rwxr-xr-x   0        0        0    30180 2023-06-10 11:58:10.825254 grblhud-1.0.1/grblhud/grblhudloop.py
+-rw-r--r--   0        0        0     6053 2023-06-10 11:58:10.835254 grblhud-1.0.1/grblhud/grblmessages.py
+-rw-r--r--   0        0        0     8040 2023-06-10 11:58:10.835254 grblhud-1.0.1/grblhud/lineinput.py
+-rw-r--r--   0        0        0     2994 2023-06-10 11:58:10.825254 grblhud-1.0.1/grblhud/unblockedgetch.py
+-rw-r--r--   0        0        0      645 2023-06-10 12:50:36.895883 grblhud-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 grblhud-1.0.1/PKG-INFO
```

### Comparing `grblhud-1.0.0/LICENSE` & `grblhud-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/README.md` & `grblhud-1.0.1/grblhud/README.md`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/grblhud/README.md` & `grblhud-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Grblhub is tested on several platforms - arm64/intel - and operating systems - Linux/macosx and two grbl v1.1 devices (a lasercutter and a CNC router)
 
 Information on grbl commands: https://github.com/gnea/grbl/blob/master/doc/markdown/commands.md
 
 Note that image2gcode and svg2gcode can be used to convert images and vector graphics to gcode at the highest quality. gcode2image can be used to validate these conversions and verify the layout before using grblhud to send the code to your lasercutter or cnc machine. https://github.com/johannesnoordanus?tab=repositories
 
-WHILE DO syntax:
+### WHILE DO syntax:
 ```
     # Gcode:
     #    #100 = 1
     #    WHILE [#100 LE 5] DO1
     #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
     #    #100 = #100 + 1 (Increase #100 by 1 each iteration of the loop)
     #    END1
@@ -29,40 +29,40 @@
     #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
     #    ; DO <loopname>'               example: '; DO aloop123'
     #
     # Note that this is an annotation (quoted out so the grbl controller does not see it)
     # Note also that loopnames are all lowercase! And have a number (if any) at the end:
     # in regex '[a-z]+[0-9]*'
 ```
-Installation note:
+### Installation note:
 ``` 
 	- pyserial must be installed first ('pip install pyserial')
-    - inputimeout must be installed ('pip install inputimeout')
+	- inputimeout must be installed ('pip install inputimeout')
 	- pip install grblhud
 
 	To install additional tools:
 	- pip install image2gcode
 	- pip install svg2gcode
 	- pip install gcode2image 
 ```
-Grblhud help:
+### Grblhud help:
 ```
     $ ./grblhud.py --help
     usage: grblhud.py [-h] [--serialdevice /dev/<serial-tty-name>] [--status /dev/<terminal-tty-name>]
 
     Stream g-code using grbl's serial read buffer.
 
     options:
       -h, --help            show this help message and exit
       --serialdevice /dev/<serial-tty-name>
                             serial device on linux (default: /dev/ttyUSB0 115200 baud)
       --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
                             grbl status output (default: no output)
 ```
-Example run:
+### Example run:
 ```
 >
 > grblhud
 Opened serial port /dev/ttyUSB0 at 115200 bauds (bits/s)
 Initializing grbl...
 
 Status report every 0.1 seconds
```

### Comparing `grblhud-1.0.0/grblhud/__main__.py` & `grblhud-1.0.1/grblhud/__main__.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/grblhud/grblbuffer.py` & `grblhud-1.0.1/grblhud/grblbuffer.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/grblhud/grblhudloop.py` & `grblhud-1.0.1/grblhud/grblhudloop.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/grblhud/grblmessages.py` & `grblhud-1.0.1/grblhud/grblmessages.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/grblhud/lineinput.py` & `grblhud-1.0.1/grblhud/lineinput.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/grblhud/unblockedgetch.py` & `grblhud-1.0.1/grblhud/unblockedgetch.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/pyproject.toml` & `grblhud-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.0/PKG-INFO` & `grblhud-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grblhud
-Version: 1.0.0
+Version: 1.0.1
 Summary: grblhub: a command line tool to handle grbl code.
 Keywords: grbl,grblv1.1,hud,laser cutter,laser engraving
 Author-email: Johannes Noordanus <mailjohannes.mailnoordanus@gmail.com>
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: inputimeout >= 1.0.4
@@ -24,15 +24,15 @@
 
 Grblhub is tested on several platforms - arm64/intel - and operating systems - Linux/macosx and two grbl v1.1 devices (a lasercutter and a CNC router)
 
 Information on grbl commands: https://github.com/gnea/grbl/blob/master/doc/markdown/commands.md
 
 Note that image2gcode and svg2gcode can be used to convert images and vector graphics to gcode at the highest quality. gcode2image can be used to validate these conversions and verify the layout before using grblhud to send the code to your lasercutter or cnc machine. https://github.com/johannesnoordanus?tab=repositories
 
-WHILE DO syntax:
+### WHILE DO syntax:
 ```
     # Gcode:
     #    #100 = 1
     #    WHILE [#100 LE 5] DO1
     #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
     #    #100 = #100 + 1 (Increase #100 by 1 each iteration of the loop)
     #    END1
@@ -42,40 +42,40 @@
     #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
     #    ; DO <loopname>'               example: '; DO aloop123'
     #
     # Note that this is an annotation (quoted out so the grbl controller does not see it)
     # Note also that loopnames are all lowercase! And have a number (if any) at the end:
     # in regex '[a-z]+[0-9]*'
 ```
-Installation note:
+### Installation note:
 ``` 
 	- pyserial must be installed first ('pip install pyserial')
-    - inputimeout must be installed ('pip install inputimeout')
+	- inputimeout must be installed ('pip install inputimeout')
 	- pip install grblhud
 
 	To install additional tools:
 	- pip install image2gcode
 	- pip install svg2gcode
 	- pip install gcode2image 
 ```
-Grblhud help:
+### Grblhud help:
 ```
     $ ./grblhud.py --help
     usage: grblhud.py [-h] [--serialdevice /dev/<serial-tty-name>] [--status /dev/<terminal-tty-name>]
 
     Stream g-code using grbl's serial read buffer.
 
     options:
       -h, --help            show this help message and exit
       --serialdevice /dev/<serial-tty-name>
                             serial device on linux (default: /dev/ttyUSB0 115200 baud)
       --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
                             grbl status output (default: no output)
 ```
-Example run:
+### Example run:
 ```
 >
 > grblhud
 Opened serial port /dev/ttyUSB0 at 115200 bauds (bits/s)
 Initializing grbl...
 
 Status report every 0.1 seconds
```

