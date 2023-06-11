# Comparing `tmp/hive-archeology-bot-0.1.6.tar.gz` & `tmp/hive-archeology-bot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-archeology-bot-0.1.6.tar", last modified: Tue May 30 22:33:57 2023, max compression
+gzip compressed data, was "hive-archeology-bot-0.1.7.tar", last modified: Sun Jun 11 15:38:35 2023, max compression
```

## Comparing `hive-archeology-bot-0.1.6.tar` & `hive-archeology-bot-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 22:33:57.147211 hive-archeology-bot-0.1.6/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.6/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 22:33:57.147211 hive-archeology-bot-0.1.6/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2104 2023-05-19 19:43:04.000000 hive-archeology-bot-0.1.6/README.md
--rwxr-xr-x   0 rob       (1000) rob       (1000)    20940 2023-05-30 22:33:49.000000 hive-archeology-bot-0.1.6/hive_archeology.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 22:33:57.147211 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 22:33:56.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-30 22:33:57.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-30 22:33:56.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-30 22:33:56.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       26 2023-05-30 22:33:56.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-30 22:33:57.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-30 22:33:57.147211 hive-archeology-bot-0.1.6/setup.cfg
--rwxr-xr-x   0 rob       (1000) rob       (1000)     1144 2023-05-30 22:33:37.000000 hive-archeology-bot-0.1.6/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-06-11 15:38:35.083017 hive-archeology-bot-0.1.7/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.7/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-06-11 15:38:35.083017 hive-archeology-bot-0.1.7/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2104 2023-05-19 19:43:04.000000 hive-archeology-bot-0.1.7/README.md
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    21070 2023-06-11 15:36:01.000000 hive-archeology-bot-0.1.7/hive_archeology.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-06-11 15:38:35.083017 hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-06-11 15:38:34.000000 hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-06-11 15:38:35.000000 hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-06-11 15:38:34.000000 hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-06-11 15:38:34.000000 hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       26 2023-06-11 15:38:34.000000 hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-06-11 15:38:34.000000 hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-06-11 15:38:35.083017 hive-archeology-bot-0.1.7/setup.cfg
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     1144 2023-05-30 22:48:13.000000 hive-archeology-bot-0.1.7/setup.py
```

### Comparing `hive-archeology-bot-0.1.6/LICENSE` & `hive-archeology-bot-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.6/PKG-INFO` & `hive-archeology-bot-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.6
+Version: 0.1.7
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
 Platform: UNKNOWN
```

### Comparing `hive-archeology-bot-0.1.6/README.md` & `hive-archeology-bot-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.6/hive_archeology.py` & `hive-archeology-bot-0.1.7/hive_archeology.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import operator
 from datetime import datetime
 from dateutil.parser import parse, _parser  # pylint: disable=import-private-name
 from lighthive.client import Client
 from lighthive.datastructures import Operation
 from lighthive.exceptions import RPCNodeException
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 AUTHORS = {}
 AUTHORS["hive-archology"] = ["pibara", "croupierbot"]
 AUTHORS["lighthive"] = ["emrebeyler", "emrebeyler"]
 
 def make_body(author, benef, curation_rewards):
     """Construct the proxy comment"""
     ben2prod = {}
@@ -346,16 +346,19 @@
     def run(self):
         """Main run function for the bot"""
         while True:  # pylint: disable=while-used
             # Process all blocks upto head
             duration = self.upto_head()
             # If processing took less than 10 seconds, sleep for a bit
             if (sleeptime := 100 - duration if self.slow else 10 - duration):
-                self.prnt.info("waiting for :", sleeptime)
-                time.sleep(sleeptime)
+                if sleeptime > 0:
+                    self.prnt.info("waiting for :", sleeptime)
+                    time.sleep(sleeptime)
+                else:
+                    self.prnt.info("no wait needed :", sleeptime)
             # Do at most one pending vote that is waiting long enough
             self.voter.tick()
 
 class Print:
     """Utility class for simple logging"""
     def __init__(self, printlevel):
         self.printlevel = printlevel
```

### Comparing `hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/PKG-INFO` & `hive-archeology-bot-0.1.7/hive_archeology_bot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.6
+Version: 0.1.7
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
 Platform: UNKNOWN
```

### Comparing `hive-archeology-bot-0.1.6/setup.py` & `hive-archeology-bot-0.1.7/setup.py`

 * *Files identical despite different names*

