# Comparing `tmp/mpd-queue-1.0.0.tar.gz` & `tmp/mpd-queue-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpd-queue-1.0.0.tar", last modified: Sun Jun 11 08:59:34 2023, max compression
+gzip compressed data, was "dist/mpd-queue-1.0.1.tar", last modified: Sun Jun 11 09:21:24 2023, max compression
```

## Comparing `mpd-queue-1.0.0.tar` & `mpd-queue-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2023-06-11 05:15:44.000000 mpd-queue-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1194 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      457 2023-06-11 08:45:27.000000 mpd-queue-1.0.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/beetsplug/
--rw-r--r--   0 user      (1000) user      (1000)       75 2023-06-11 06:23:26.000000 mpd-queue-1.0.0/beetsplug/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      764 2023-06-11 08:20:32.000000 mpd-queue-1.0.0/beetsplug/mpd-queue.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/mpd_queue.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1194 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/mpd_queue.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      235 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/mpd_queue.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/mpd_queue.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/mpd_queue.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/mpd_queue.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-11 08:59:34.000000 mpd-queue-1.0.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1102 2023-06-11 08:41:08.000000 mpd-queue-1.0.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/
+-rw-r--r--   0 user      (1000) user      (1000)    35149 2023-06-11 05:15:44.000000 mpd-queue-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     1512 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      776 2023-06-11 09:19:17.000000 mpd-queue-1.0.1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/beetsplug/
+-rw-r--r--   0 user      (1000) user      (1000)       75 2023-06-11 06:23:26.000000 mpd-queue-1.0.1/beetsplug/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      932 2023-06-11 09:11:20.000000 mpd-queue-1.0.1/beetsplug/mpd-queue.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1512 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      235 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1102 2023-06-11 09:19:17.000000 mpd-queue-1.0.1/setup.py
```

### Comparing `mpd-queue-1.0.0/LICENSE` & `mpd-queue-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpd-queue-1.0.0/PKG-INFO` & `mpd-queue-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-queue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Beets plugin to add all imported tracks to an MPD server's queue
 Home-page: https://github.com/ui-1/mpd-queue
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
@@ -30,9 +30,20 @@
 ```python
 pip install mpd-queue
 ```
 and then add `mpd-queue` to the list of enabled plugins in your Beets config.
 
 ## Configuration
 
-`host`: Hostname of the MPD server.  
-`port`: Port to use when connecting.
+Optionally, to specify a non-default location for the MPD server, add a configuration block like this:
+```yaml
+mpd-queue:
+  host: example.com
+  port: 6601
+```
+
+### Options
+
+| Key  | Description                 | Default value |
+|------|-----------------------------|---------------|
+| host | Hostname of the MPD server  | localhost     |
+| port | Port to use when connecting | 6600          |
```

### Comparing `mpd-queue-1.0.0/mpd_queue.egg-info/PKG-INFO` & `mpd-queue-1.0.1/mpd_queue.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-queue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Beets plugin to add all imported tracks to an MPD server's queue
 Home-page: https://github.com/ui-1/mpd-queue
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
@@ -30,9 +30,20 @@
 ```python
 pip install mpd-queue
 ```
 and then add `mpd-queue` to the list of enabled plugins in your Beets config.
 
 ## Configuration
 
-`host`: Hostname of the MPD server.  
-`port`: Port to use when connecting.
+Optionally, to specify a non-default location for the MPD server, add a configuration block like this:
+```yaml
+mpd-queue:
+  host: example.com
+  port: 6601
+```
+
+### Options
+
+| Key  | Description                 | Default value |
+|------|-----------------------------|---------------|
+| host | Hostname of the MPD server  | localhost     |
+| port | Port to use when connecting | 6600          |
```

### Comparing `mpd-queue-1.0.0/setup.py` & `mpd-queue-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mpd-queue',
-    version='1.0.0',
+    version='1.0.1',
     description='Beets plugin to add all imported tracks to an MPD server\'s queue',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ui-1/mpd-queue',
     author='ui-1',
     author_email='ui-1@posteo.org',
     license='GPLv3',
```

