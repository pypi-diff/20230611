# Comparing `tmp/mpd-queue-1.0.3.tar.gz` & `tmp/mpd-queue-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpd-queue-1.0.3.tar", last modified: Sun Jun 11 09:54:56 2023, max compression
+gzip compressed data, was "dist/mpd-queue-1.0.4.tar", last modified: Sun Jun 11 15:40:19 2023, max compression
```

## Comparing `mpd-queue-1.0.3.tar` & `mpd-queue-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2023-06-11 05:15:44.000000 mpd-queue-1.0.3/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1627 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      891 2023-06-11 09:47:29.000000 mpd-queue-1.0.3/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/beetsplug/
--rw-r--r--   0 user      (1000) user      (1000)       75 2023-06-11 06:23:26.000000 mpd-queue-1.0.3/beetsplug/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      932 2023-06-11 09:41:21.000000 mpd-queue-1.0.3/beetsplug/mpd-queue.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/mpd_queue.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1627 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/mpd_queue.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      235 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/mpd_queue.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/mpd_queue.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       18 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/mpd_queue.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/mpd_queue.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-11 09:54:56.000000 mpd-queue-1.0.3/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1103 2023-06-11 09:53:08.000000 mpd-queue-1.0.3/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/
+-rw-r--r--   0 user      (1000) user      (1000)    35149 2023-06-11 05:15:44.000000 mpd-queue-1.0.4/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     1741 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1005 2023-06-11 10:10:04.000000 mpd-queue-1.0.4/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/beetsplug/
+-rw-r--r--   0 user      (1000) user      (1000)       75 2023-06-11 06:23:26.000000 mpd-queue-1.0.4/beetsplug/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1531 2023-06-11 15:37:56.000000 mpd-queue-1.0.4/beetsplug/mpd-queue.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/mpd_queue.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1741 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/mpd_queue.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      235 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/mpd_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/mpd_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       18 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/mpd_queue.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/mpd_queue.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-11 15:40:19.000000 mpd-queue-1.0.4/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1103 2023-06-11 15:32:47.000000 mpd-queue-1.0.4/setup.py
```

### Comparing `mpd-queue-1.0.3/LICENSE` & `mpd-queue-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpd-queue-1.0.3/PKG-INFO` & `mpd-queue-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-queue
-Version: 1.0.3
+Version: 1.0.4
 Summary: Beets plugin to add all imported tracks to an MPD server's queue
 Home-page: https://github.com/ui-1/mpd-queue
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
@@ -16,14 +16,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpd-queue
 
+![GitHub](https://img.shields.io/github/license/ui-1/mpd-queue)
+![PyPI](https://img.shields.io/pypi/v/mpd-queue)
+
 A small [Beets](https://github.com/beetbox/beets) plugin to add newly imported tracks to the queue of your [MPD](https://github.com/MusicPlayerDaemon/MPD) server.
 
 ## Installation
 
 To install the plugin, simply run the following:
 ```python
 pip install mpd-queue
```

### Comparing `mpd-queue-1.0.3/README.md` & `mpd-queue-1.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # mpd-queue
 
+![GitHub](https://img.shields.io/github/license/ui-1/mpd-queue)
+![PyPI](https://img.shields.io/pypi/v/mpd-queue)
+
 A small [Beets](https://github.com/beetbox/beets) plugin to add newly imported tracks to the queue of your [MPD](https://github.com/MusicPlayerDaemon/MPD) server.
 
 ## Installation
 
 To install the plugin, simply run the following:
 ```python
 pip install mpd-queue
```

### Comparing `mpd-queue-1.0.3/beetsplug/mpd-queue.py` & `mpd-queue-1.0.4/beetsplug/mpd-queue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,45 @@
+import time
 import confuse.exceptions
 from beets.plugins import BeetsPlugin
 from mpd import MPDClient
 
 
 class MPDQueuePlugin(BeetsPlugin):
 
     def __init__(self):
         super(MPDQueuePlugin, self).__init__()
         self.register_listener('album_imported', self.gather_imported_files)
         self.register_listener('import', self.queue)
         self.paths = set()
+        self.client = MPDClient()
 
     def gather_imported_files(self, album):
         for item in album.items():
             songpath = item.destination(fragment=True)
             self.paths.add(songpath)
 
+    def block_until_update_finishes(self):
+        """MPDClient's update method only tells the MPD server to "start updating the database" without actually
+        waiting for it to finish. Trying to add a newly imported song to the queue before it's in the database results
+        in an exception, so we poll the client's status until the update *has* finished.
+        """
+        while True:
+            if 'updating_db' in self.client.status():
+                time.sleep(0.1)
+            else:
+                return
+
     def queue(self):
-        client = MPDClient()
 
         try: port = self.config['port'].get()
         except confuse.exceptions.NotFoundError: port = 6600
 
         try: host = self.config['host'].get()
         except confuse.exceptions.NotFoundError: host = 'localhost'
 
-        client.connect(host, port)
-        client.update()
+        self.client.connect(host, port)
+        self.client.update()
+        self.block_until_update_finishes()
 
         for path in sorted(self.paths):
-            client.add(path)
+            self.client.add(path)
```

### Comparing `mpd-queue-1.0.3/mpd_queue.egg-info/PKG-INFO` & `mpd-queue-1.0.4/mpd_queue.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-queue
-Version: 1.0.3
+Version: 1.0.4
 Summary: Beets plugin to add all imported tracks to an MPD server's queue
 Home-page: https://github.com/ui-1/mpd-queue
 Author: ui-1
 Author-email: ui-1@posteo.org
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
@@ -16,14 +16,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpd-queue
 
+![GitHub](https://img.shields.io/github/license/ui-1/mpd-queue)
+![PyPI](https://img.shields.io/pypi/v/mpd-queue)
+
 A small [Beets](https://github.com/beetbox/beets) plugin to add newly imported tracks to the queue of your [MPD](https://github.com/MusicPlayerDaemon/MPD) server.
 
 ## Installation
 
 To install the plugin, simply run the following:
 ```python
 pip install mpd-queue
```

### Comparing `mpd-queue-1.0.3/setup.py` & `mpd-queue-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mpd-queue',
-    version='1.0.3',
+    version='1.0.4',
     description='Beets plugin to add all imported tracks to an MPD server\'s queue',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ui-1/mpd-queue',
     author='ui-1',
     author_email='ui-1@posteo.org',
     license='GPLv3',
```

