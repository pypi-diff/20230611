# Comparing `tmp/realtouch-0.1.7.tar.gz` & `tmp/realtouch-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtouch-0.1.7.tar", last modified: Fri May 19 16:11:32 2023, max compression
+gzip compressed data, was "realtouch-0.1.8.tar", last modified: Sun Jun 11 06:55:50 2023, max compression
```

## Comparing `realtouch-0.1.7.tar` & `realtouch-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-19 16:11:32.955582 realtouch-0.1.7/
--rw-r--r--   0 k          (501) staff       (20)    35148 2023-05-12 00:09:36.000000 realtouch-0.1.7/LICENSE
--rw-r--r--   0 k          (501) staff       (20)      539 2023-05-19 16:11:32.955251 realtouch-0.1.7/PKG-INFO
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-19 16:11:32.950146 realtouch-0.1.7/realtouch/
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-19 16:11:32.952076 realtouch-0.1.7/realtouch/src/
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-19 16:11:32.954507 realtouch-0.1.7/realtouch/src/realtouch.egg-info/
--rw-r--r--   0 k          (501) staff       (20)      539 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/PKG-INFO
--rw-r--r--   0 k          (501) staff       (20)      277 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/SOURCES.txt
--rw-r--r--   0 k          (501) staff       (20)        1 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/dependency_links.txt
--rw-r--r--   0 k          (501) staff       (20)       16 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/requires.txt
--rw-r--r--   0 k          (501) staff       (20)       10 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/top_level.txt
--rw-r--r--   0 k          (501) staff       (20)    23629 2023-05-19 15:41:55.000000 realtouch-0.1.7/realtouch/src/realtouch.py
--rw-r--r--   0 k          (501) staff       (20)       38 2023-05-19 16:11:32.955724 realtouch-0.1.7/setup.cfg
--rw-r--r--   0 k          (501) staff       (20)      852 2023-05-19 09:06:04.000000 realtouch-0.1.7/setup.py
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-06-11 06:55:50.759937 realtouch-0.1.8/
+-rw-r--r--   0 k          (501) staff       (20)    35148 2023-05-12 00:09:36.000000 realtouch-0.1.8/LICENSE
+-rw-r--r--   0 k          (501) staff       (20)      539 2023-06-11 06:55:50.759677 realtouch-0.1.8/PKG-INFO
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-06-11 06:55:50.755874 realtouch-0.1.8/realtouch/
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-06-11 06:55:50.757176 realtouch-0.1.8/realtouch/src/
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-06-11 06:55:50.759225 realtouch-0.1.8/realtouch/src/realtouch.egg-info/
+-rw-r--r--   0 k          (501) staff       (20)      539 2023-06-11 06:55:50.000000 realtouch-0.1.8/realtouch/src/realtouch.egg-info/PKG-INFO
+-rw-r--r--   0 k          (501) staff       (20)      277 2023-06-11 06:55:50.000000 realtouch-0.1.8/realtouch/src/realtouch.egg-info/SOURCES.txt
+-rw-r--r--   0 k          (501) staff       (20)        1 2023-06-11 06:55:50.000000 realtouch-0.1.8/realtouch/src/realtouch.egg-info/dependency_links.txt
+-rw-r--r--   0 k          (501) staff       (20)       16 2023-06-11 06:55:50.000000 realtouch-0.1.8/realtouch/src/realtouch.egg-info/requires.txt
+-rw-r--r--   0 k          (501) staff       (20)       10 2023-06-11 06:55:50.000000 realtouch-0.1.8/realtouch/src/realtouch.egg-info/top_level.txt
+-rw-r--r--   0 k          (501) staff       (20)    23742 2023-06-11 06:54:16.000000 realtouch-0.1.8/realtouch/src/realtouch.py
+-rw-r--r--   0 k          (501) staff       (20)       38 2023-06-11 06:55:50.760007 realtouch-0.1.8/setup.cfg
+-rw-r--r--   0 k          (501) staff       (20)      852 2023-06-11 06:54:51.000000 realtouch-0.1.8/setup.py
```

### Comparing `realtouch-0.1.7/LICENSE` & `realtouch-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `realtouch-0.1.7/PKG-INFO` & `realtouch-0.1.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtouch
-Version: 0.1.7
+Version: 0.1.8
 Summary: realTouch Robot SDK
 Home-page: https://realtouch.dev
 Author: realTouch Dev
 Author-email: contact@realtouch.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `realtouch-0.1.7/realtouch/src/realtouch.egg-info/PKG-INFO` & `realtouch-0.1.8/realtouch/src/realtouch.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtouch
-Version: 0.1.7
+Version: 0.1.8
 Summary: realTouch Robot SDK
 Home-page: https://realtouch.dev
 Author: realTouch Dev
 Author-email: contact@realtouch.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `realtouch-0.1.7/realtouch/src/realtouch.py` & `realtouch-0.1.8/realtouch/src/realtouch.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,14 +485,17 @@
         return self.enter_text(TextAction.KEYCODE_CLOSE)
 
     def waited_update(self, before=2, after=2):
         time.sleep(before)
         self.update()
         time.sleep(after)
 
+    def is_input_on(self):
+        return self.phone.robot.call_func(self.phone.position, 'screen/is_input_on')
+
 
 class Phone:
     def __init__(
             self,
             position: int,
             robot: Robot,
             data: dict
```

### Comparing `realtouch-0.1.7/setup.py` & `realtouch-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="realtouch",
-    version="0.1.7",
+    version="0.1.8",
     author="realTouch Dev",
     author_email="contact@realtouch.dev",
     description="realTouch Robot SDK",
     long_description="realTouch Robot SDK",
     long_description_content_type="text/markdown",
     url="https://realtouch.dev",
     packages=find_packages(),
```

