# Comparing `tmp/uun-weatherstation-0.6.1.tar.gz` & `tmp/uun-weatherstation-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-weatherstation-0.6.1.tar", last modified: Thu Jan 26 11:53:05 2023, max compression
+gzip compressed data, was "uun-weatherstation-0.6.2.tar", last modified: Sun Jun 11 19:52:55 2023, max compression
```

## Comparing `uun-weatherstation-0.6.1.tar` & `uun-weatherstation-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:53:05.271321 uun-weatherstation-0.6.1/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:43.000000 uun-weatherstation-0.6.1/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      466 2023-01-26 11:53:05.271321 uun-weatherstation-0.6.1/PKG-INFO
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:53:05.271321 uun-weatherstation-0.6.1/bin/
--rwx------   0 hello     (1000) hello     (1000)     2332 2023-01-26 11:51:51.000000 uun-weatherstation-0.6.1/bin/uun-weatherstation
--rwx------   0 hello     (1000) hello     (1000)      505 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/bin/uun-weatherstation-install
--rw-------   0 hello     (1000) hello     (1000)       38 2023-01-26 11:53:05.271321 uun-weatherstation-0.6.1/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1065 2023-01-26 11:51:01.000000 uun-weatherstation-0.6.1/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:53:05.271321 uun-weatherstation-0.6.1/uun_weatherstation/
--rw-------   0 hello     (1000) hello     (1000)        1 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:53:05.271321 uun-weatherstation-0.6.1/uun_weatherstation/data/
--rw-------   0 hello     (1000) hello     (1000)     1657 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       70 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      292 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/data/systemd.service
--rw-------   0 hello     (1000) hello     (1000)      194 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/diagnostic.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:53:05.271321 uun-weatherstation-0.6.1/uun_weatherstation/modules/
--rw-------   0 hello     (1000) hello     (1000)      416 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/modules/HealthCheck.py
--rw-------   0 hello     (1000) hello     (1000)     8536 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/modules/WeatherConditions.py
--rw-------   0 hello     (1000) hello     (1000)     1722 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)      326 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.1/uun_weatherstation/utils.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:53:05.271321 uun-weatherstation-0.6.1/uun_weatherstation.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      466 2023-01-26 11:53:05.000000 uun-weatherstation-0.6.1/uun_weatherstation.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      619 2023-01-26 11:53:05.000000 uun-weatherstation-0.6.1/uun_weatherstation.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-01-26 11:53:05.000000 uun-weatherstation-0.6.1/uun_weatherstation.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       32 2023-01-26 11:53:05.000000 uun-weatherstation-0.6.1/uun_weatherstation.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       19 2023-01-26 11:53:05.000000 uun-weatherstation-0.6.1/uun_weatherstation.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:43.000000 uun-weatherstation-0.6.2/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      466 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/PKG-INFO
+drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.085318 uun-weatherstation-0.6.2/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2332 2023-06-11 19:49:30.000000 uun-weatherstation-0.6.2/bin/uun-weatherstation
+-rwx------   0 hello     (1000) hello     (1000)      505 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/bin/uun-weatherstation-install
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1065 2023-01-26 11:51:01.000000 uun-weatherstation-0.6.2/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.085318 uun-weatherstation-0.6.2/tests/
+-rw-------   0 hello     (1000) hello     (1000)     5995 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/tests/test_data_processing.py
+-rw-------   0 hello     (1000) hello     (1000)      139 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/tests/test_run_5s.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.085318 uun-weatherstation-0.6.2/uun_weatherstation/
+-rw-------   0 hello     (1000) hello     (1000)        1 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/uun_weatherstation/data/
+-rw-------   0 hello     (1000) hello     (1000)     1657 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       70 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      292 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/data/systemd.service
+-rw-------   0 hello     (1000) hello     (1000)      194 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/diagnostic.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/uun_weatherstation/modules/
+-rw-------   0 hello     (1000) hello     (1000)      416 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/modules/HealthCheck.py
+-rw-------   0 hello     (1000) hello     (1000)     8536 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/modules/WeatherConditions.py
+-rw-------   0 hello     (1000) hello     (1000)     2639 2023-06-11 19:34:00.000000 uun-weatherstation-0.6.2/uun_weatherstation/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)      326 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/utils.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      466 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      670 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       32 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       19 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/top_level.txt
```

### Comparing `uun-weatherstation-0.6.1/LICENSE.md` & `uun-weatherstation-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.1/bin/uun-weatherstation` & `uun-weatherstation-0.6.2/bin/uun-weatherstation`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import logging
 import time
 import argparse
 import sys
 import signal
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 __package__ = "uun_weatherstation"
 library = "uun_iot"
 
 def main():
     argp = argparse.ArgumentParser(prog=__package__, description='Connect to weatherlink weatherstation and process informations and send to server.')
     argp.add_argument('-v', '--version', action='version', version='%(prog) ' + __version__)
     argp.add_argument('-l', '--log', metavar='loglevel', dest='loglevel', type=str, help='level of logging: [DEBUG, INFO, WARNING, ERROR, CRITICAL]', default='WARNING')
```

### Comparing `uun-weatherstation-0.6.1/setup.py` & `uun-weatherstation-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.1/uun_weatherstation/data/sample-config.json` & `uun-weatherstation-0.6.2/uun_weatherstation/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.1/uun_weatherstation/modules/WeatherConditions.py` & `uun-weatherstation-0.6.2/uun_weatherstation/modules/WeatherConditions.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.1/uun_weatherstation/modules/__init__.py` & `uun-weatherstation-0.6.2/uun_weatherstation/modules/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,37 @@
 from uun_iot.diagnostic import DiagnosticEvent
 
 # module list in format { module_id: [module_instance, None], ... }
 def init(config, uuclient):
 
     gconfig = config["gateway"]
 
+    if "healthCheck" not in gconfig:
+        def cmd_weatherconditions(storage):
+            """ Send weather to uuApp and return entries that failed to be sent. Each entry is sent separately. """
+            uucmd = config["uuApp"]['uuCmdList']['weatherConditionsAdd']
+            s = UuCmdSession(uuclient, uucmd)
+            failed = []
+            len_storage = 0
+            len_failed = 0
+            for dto_in in storage:
+                len_storage += 1
+                try:
+                    r, ok = s.post(dto_in)
+                    r.raise_for_status()
+                except requests.exceptions.RequestException as e:
+                    loggerwc.info("Error in server communication: %s", e)
+                    len_failed += 1
+                    failed.append(dto_in)
+            return failed
+
+        return [
+            WeatherConditions(config=gconfig, uucmd=cmd_weatherconditions),
+        ]
+
     healthcheck = HealthCheck(gconfig)
     notify = healthcheck.notifier("weatherConditions")
 
     loggerwc = logging.getLogger(__name__+".WeatherCondtionsUuCmd")
     def cmd_weatherconditions(storage):
         """ Send weather to uuApp and return entries that failed to be sent. Each entry is sent separately. """
         uucmd = config["uuApp"]['uuCmdList']['weatherConditionsAdd']
```

