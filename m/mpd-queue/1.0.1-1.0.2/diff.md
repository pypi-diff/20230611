# Comparing `tmp/mpd-queue-1.0.1.tar.gz` & `tmp/mpd-queue-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpd-queue-1.0.1.tar", last modified: Sun Jun 11 09:21:24 2023, max compression
+gzip compressed data, was "dist/mpd-queue-1.0.2.tar", last modified: Sun Jun 11 09:29:52 2023, max compression
```

## Comparing `mpd-queue-1.0.1.tar` & `mpd-queue-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2023-06-11 05:15:44.000000 mpd-queue-1.0.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1512 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      776 2023-06-11 09:19:17.000000 mpd-queue-1.0.1/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/beetsplug/
--rw-r--r--   0 user      (1000) user      (1000)       75 2023-06-11 06:23:26.000000 mpd-queue-1.0.1/beetsplug/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      932 2023-06-11 09:11:20.000000 mpd-queue-1.0.1/beetsplug/mpd-queue.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1512 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      235 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/mpd_queue.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-11 09:21:24.000000 mpd-queue-1.0.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1102 2023-06-11 09:19:17.000000 mpd-queue-1.0.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/
+-rw-r--r--   0 user      (1000) user      (1000)    35149 2023-06-11 05:15:44.000000 mpd-queue-1.0.2/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     1627 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      891 2023-06-11 09:27:44.000000 mpd-queue-1.0.2/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/beetsplug/
+-rw-r--r--   0 user      (1000) user      (1000)       75 2023-06-11 06:23:26.000000 mpd-queue-1.0.2/beetsplug/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      932 2023-06-11 09:11:20.000000 mpd-queue-1.0.2/beetsplug/mpd-queue.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/mpd_queue.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1627 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/mpd_queue.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      235 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/mpd_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/mpd_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/mpd_queue.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/mpd_queue.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-11 09:29:52.000000 mpd-queue-1.0.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1102 2023-06-11 09:29:42.000000 mpd-queue-1.0.2/setup.py
```

### Comparing `mpd-queue-1.0.1/LICENSE` & `mpd-queue-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpd-queue-1.0.1/PKG-INFO` & `mpd-queue-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-queue
-Version: 1.0.1
+Version: 1.0.2
 Summary: Beets plugin to add all imported tracks to an MPD server's queue
 Home-page: https://github.com/ui-1/mpd-queue
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
@@ -16,16 +16,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpd-queue
 
-- - -
-
 A small [Beets](https://github.com/beetbox/beets) plugin to add newly imported tracks to the queue of your [MPD](https://github.com/MusicPlayerDaemon/MPD) server.
 
 ## Installation
 
 To install the plugin, simply run the following:
 ```python
 pip install mpd-queue
@@ -43,7 +41,11 @@
 
 ### Options
 
 | Key  | Description                 | Default value |
 |------|-----------------------------|---------------|
 | host | Hostname of the MPD server  | localhost     |
 | port | Port to use when connecting | 6600          |
+
+## Usage
+
+Simply run `beet import` as you normally would. Any imported files should (quietly) be added to the MPD queue.
```

### Comparing `mpd-queue-1.0.1/README.md` & `mpd-queue-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # mpd-queue
 
-- - -
-
 A small [Beets](https://github.com/beetbox/beets) plugin to add newly imported tracks to the queue of your [MPD](https://github.com/MusicPlayerDaemon/MPD) server.
 
 ## Installation
 
 To install the plugin, simply run the following:
 ```python
 pip install mpd-queue
@@ -23,7 +21,11 @@
 
 ### Options
 
 | Key  | Description                 | Default value |
 |------|-----------------------------|---------------|
 | host | Hostname of the MPD server  | localhost     |
 | port | Port to use when connecting | 6600          |
+
+## Usage
+
+Simply run `beet import` as you normally would. Any imported files should (quietly) be added to the MPD queue.
```

### Comparing `mpd-queue-1.0.1/beetsplug/mpd-queue.py` & `mpd-queue-1.0.2/beetsplug/mpd-queue.py`

 * *Files identical despite different names*

### Comparing `mpd-queue-1.0.1/mpd_queue.egg-info/PKG-INFO` & `mpd-queue-1.0.2/mpd_queue.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-queue
-Version: 1.0.1
+Version: 1.0.2
 Summary: Beets plugin to add all imported tracks to an MPD server's queue
 Home-page: https://github.com/ui-1/mpd-queue
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
@@ -16,16 +16,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpd-queue
 
-- - -
-
 A small [Beets](https://github.com/beetbox/beets) plugin to add newly imported tracks to the queue of your [MPD](https://github.com/MusicPlayerDaemon/MPD) server.
 
 ## Installation
 
 To install the plugin, simply run the following:
 ```python
 pip install mpd-queue
@@ -43,7 +41,11 @@
 
 ### Options
 
 | Key  | Description                 | Default value |
 |------|-----------------------------|---------------|
 | host | Hostname of the MPD server  | localhost     |
 | port | Port to use when connecting | 6600          |
+
+## Usage
+
+Simply run `beet import` as you normally would. Any imported files should (quietly) be added to the MPD queue.
```

### Comparing `mpd-queue-1.0.1/setup.py` & `mpd-queue-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mpd-queue',
-    version='1.0.1',
+    version='1.0.2',
     description='Beets plugin to add all imported tracks to an MPD server\'s queue',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ui-1/mpd-queue',
     author='ui-1',
     author_email='ui-1@posteo.org',
     license='GPLv3',
```

