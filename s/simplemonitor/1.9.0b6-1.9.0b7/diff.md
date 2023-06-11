# Comparing `tmp/simplemonitor-1.9.0b6.tar.gz` & `tmp/simplemonitor-1.9.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplemonitor-1.9.0b6.tar", last modified: Sat Feb 22 11:31:00 2020, max compression
+gzip compressed data, was "dist/simplemonitor-1.9.0b7.tar", last modified: Sat Feb 22 11:33:01 2020, max compression
```

## Comparing `simplemonitor-1.9.0b6.tar` & `simplemonitor-1.9.0b7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/
--rw-r--r--   0 james      (501) staff       (20)     1631 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      771 2020-01-11 16:46:03.000000 simplemonitor-1.9.0b6/README.md
--rw-r--r--   0 james      (501) staff       (20)       38 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1600 2020-02-22 11:30:42.000000 simplemonitor-1.9.0b6/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/
--rw-r--r--   0 james      (501) staff       (20)       72 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     8471 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/alerter.py
--rw-r--r--   0 james      (501) staff       (20)     4240 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/bulksms.py
--rw-r--r--   0 james      (501) staff       (20)     2853 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/execute.py
--rw-r--r--   0 james      (501) staff       (20)     4379 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/fortysixelks.py
--rw-r--r--   0 james      (501) staff       (20)     5151 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/mail.py
--rw-r--r--   0 james      (501) staff       (20)     1759 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/nc.py
--rw-r--r--   0 james      (501) staff       (20)     4057 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/pushbullet.py
--rw-r--r--   0 james      (501) staff       (20)     4051 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/pushover.py
--rw-r--r--   0 james      (501) staff       (20)     5508 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/ses.py
--rw-r--r--   0 james      (501) staff       (20)     4627 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/slack.py
--rw-r--r--   0 james      (501) staff       (20)      591 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/syslogger.py
--rw-r--r--   0 james      (501) staff       (20)     3340 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Alerters/telegram.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor/Loggers/
--rw-r--r--   0 james      (501) staff       (20)       44 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/Loggers/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6414 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Loggers/db.py
--rw-r--r--   0 james      (501) staff       (20)    15987 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Loggers/file.py
--rw-r--r--   0 james      (501) staff       (20)     3357 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Loggers/logger.py
--rw-r--r--   0 james      (501) staff       (20)     4960 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Loggers/mqtt.py
--rw-r--r--   0 james      (501) staff       (20)     7453 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Loggers/network.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/
--rw-r--r--   0 james      (501) staff       (20)       52 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3827 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/compound.py
--rw-r--r--   0 james      (501) staff       (20)     1555 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/file.py
--rw-r--r--   0 james      (501) staff       (20)     2192 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/hass.py
--rw-r--r--   0 james      (501) staff       (20)    17885 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/host.py
--rw-r--r--   0 james      (501) staff       (20)    15572 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/monitor.py
--rw-r--r--   0 james      (501) staff       (20)    11810 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/network.py
--rw-r--r--   0 james      (501) staff       (20)     3828 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/ring.py
--rw-r--r--   0 james      (501) staff       (20)    13086 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/Monitors/service.py
--rw-r--r--   0 james      (501) staff       (20)        0 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor/html/
--rw-r--r--   0 james      (501) staff       (20)       96 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/html/footer.html
--rw-r--r--   0 james      (501) staff       (20)     1360 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/html/header.html
--rw-r--r--   0 james      (501) staff       (20)     1094 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b6/simplemonitor/html/style.css
--rw-r--r--   0 james      (501) staff       (20)    21575 2020-02-15 17:43:49.000000 simplemonitor-1.9.0b6/simplemonitor/monitor.py
--rw-r--r--   0 james      (501) staff       (20)    14479 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/simplemonitor.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor/util/
--rw-r--r--   0 james      (501) staff       (20)     6450 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/util/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2604 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/util/envconfig.py
--rw-r--r--   0 james      (501) staff       (20)       20 2020-02-22 11:30:22.000000 simplemonitor-1.9.0b6/simplemonitor/version.py
--rwxr-xr-x   0 james      (501) staff       (20)     3871 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b6/simplemonitor/winmonitor.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     1631 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1455 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      105 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)      157 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       14 2020-02-22 11:31:00.000000 simplemonitor-1.9.0b6/simplemonitor.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/
+-rw-r--r--   0 james      (501) staff       (20)     1631 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      771 2020-01-11 16:46:03.000000 simplemonitor-1.9.0b7/README.md
+-rw-r--r--   0 james      (501) staff       (20)       38 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1609 2020-02-22 11:32:38.000000 simplemonitor-1.9.0b7/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/simplemonitor/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/
+-rw-r--r--   0 james      (501) staff       (20)       72 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     8471 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/alerter.py
+-rw-r--r--   0 james      (501) staff       (20)     4240 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/bulksms.py
+-rw-r--r--   0 james      (501) staff       (20)     2853 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/execute.py
+-rw-r--r--   0 james      (501) staff       (20)     4379 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/fortysixelks.py
+-rw-r--r--   0 james      (501) staff       (20)     5151 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/mail.py
+-rw-r--r--   0 james      (501) staff       (20)     1759 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/nc.py
+-rw-r--r--   0 james      (501) staff       (20)     4057 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/pushbullet.py
+-rw-r--r--   0 james      (501) staff       (20)     4051 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/pushover.py
+-rw-r--r--   0 james      (501) staff       (20)     5508 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/ses.py
+-rw-r--r--   0 james      (501) staff       (20)     4627 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/slack.py
+-rw-r--r--   0 james      (501) staff       (20)      591 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/syslogger.py
+-rw-r--r--   0 james      (501) staff       (20)     3340 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Alerters/telegram.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/simplemonitor/Loggers/
+-rw-r--r--   0 james      (501) staff       (20)       44 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/Loggers/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6414 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Loggers/db.py
+-rw-r--r--   0 james      (501) staff       (20)    15987 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Loggers/file.py
+-rw-r--r--   0 james      (501) staff       (20)     3357 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Loggers/logger.py
+-rw-r--r--   0 james      (501) staff       (20)     4960 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Loggers/mqtt.py
+-rw-r--r--   0 james      (501) staff       (20)     7453 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Loggers/network.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/
+-rw-r--r--   0 james      (501) staff       (20)       52 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3827 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/compound.py
+-rw-r--r--   0 james      (501) staff       (20)     1555 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/file.py
+-rw-r--r--   0 james      (501) staff       (20)     2192 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/hass.py
+-rw-r--r--   0 james      (501) staff       (20)    17885 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/host.py
+-rw-r--r--   0 james      (501) staff       (20)    15572 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/monitor.py
+-rw-r--r--   0 james      (501) staff       (20)    11810 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/network.py
+-rw-r--r--   0 james      (501) staff       (20)     3828 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/ring.py
+-rw-r--r--   0 james      (501) staff       (20)    13086 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/Monitors/service.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/simplemonitor/html/
+-rw-r--r--   0 james      (501) staff       (20)       96 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/html/footer.html
+-rw-r--r--   0 james      (501) staff       (20)     1360 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/html/header.html
+-rw-r--r--   0 james      (501) staff       (20)     1094 2020-02-15 11:26:15.000000 simplemonitor-1.9.0b7/simplemonitor/html/style.css
+-rw-r--r--   0 james      (501) staff       (20)    21575 2020-02-15 17:43:49.000000 simplemonitor-1.9.0b7/simplemonitor/monitor.py
+-rw-r--r--   0 james      (501) staff       (20)    14479 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/simplemonitor.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/simplemonitor/util/
+-rw-r--r--   0 james      (501) staff       (20)     6450 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/util/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2604 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/util/envconfig.py
+-rw-r--r--   0 james      (501) staff       (20)       20 2020-02-22 11:32:51.000000 simplemonitor-1.9.0b7/simplemonitor/version.py
+-rwxr-xr-x   0 james      (501) staff       (20)     3871 2020-01-25 11:51:28.000000 simplemonitor-1.9.0b7/simplemonitor/winmonitor.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2020-02-22 11:33:01.000000 simplemonitor-1.9.0b7/simplemonitor.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     1631 2020-02-22 11:33:00.000000 simplemonitor-1.9.0b7/simplemonitor.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1455 2020-02-22 11:33:00.000000 simplemonitor-1.9.0b7/simplemonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2020-02-22 11:33:00.000000 simplemonitor-1.9.0b7/simplemonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      105 2020-02-22 11:33:00.000000 simplemonitor-1.9.0b7/simplemonitor.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      158 2020-02-22 11:33:00.000000 simplemonitor-1.9.0b7/simplemonitor.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       14 2020-02-22 11:33:00.000000 simplemonitor-1.9.0b7/simplemonitor.egg-info/top_level.txt
```

### Comparing `simplemonitor-1.9.0b6/PKG-INFO` & `simplemonitor-1.9.0b7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplemonitor
-Version: 1.9.0b6
+Version: 1.9.0b7
 Summary: A simple network and host monitor
 Home-page: https://github.com/jamesoff/simplemonitor
 Author: James Seward
 Author-email: james@jamesoff.net
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/jamesoff/simplemonitor.svg?branch=master)](https://travis-ci.org/jamesoff/simplemonitor) [![codecov](https://codecov.io/gh/jamesoff/simplemonitor/branch/master/graph/badge.svg)](https://codecov.io/gh/jamesoff/simplemonitor) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `simplemonitor-1.9.0b6/README.md` & `simplemonitor-1.9.0b7/README.md`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/setup.py` & `simplemonitor-1.9.0b7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,14 @@
         ]
     },
     extras_require={"ring": ["ring-doorbell>=0.6.0"]},
     install_requires=[
         "boto3",
         "colorlog",
         "paho-mqtt",
-        "psutil" "pyOpenSSL",
+        "psutil",
+        "pyOpenSSL",
         "requests",
         'pync; platform_system=="Darwin"',
         'pywin32; platform_system=="Windows"',
     ],
 )
```

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/alerter.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/alerter.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/bulksms.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/bulksms.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/execute.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/execute.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/fortysixelks.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/fortysixelks.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/mail.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/mail.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/nc.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/nc.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/pushbullet.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/pushbullet.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/pushover.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/pushover.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/ses.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/ses.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/slack.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/slack.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/syslogger.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/syslogger.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Alerters/telegram.py` & `simplemonitor-1.9.0b7/simplemonitor/Alerters/telegram.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Loggers/db.py` & `simplemonitor-1.9.0b7/simplemonitor/Loggers/db.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Loggers/file.py` & `simplemonitor-1.9.0b7/simplemonitor/Loggers/file.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Loggers/logger.py` & `simplemonitor-1.9.0b7/simplemonitor/Loggers/logger.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Loggers/mqtt.py` & `simplemonitor-1.9.0b7/simplemonitor/Loggers/mqtt.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Loggers/network.py` & `simplemonitor-1.9.0b7/simplemonitor/Loggers/network.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Monitors/compound.py` & `simplemonitor-1.9.0b7/simplemonitor/Monitors/compound.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Monitors/file.py` & `simplemonitor-1.9.0b7/simplemonitor/Monitors/file.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Monitors/hass.py` & `simplemonitor-1.9.0b7/simplemonitor/Monitors/hass.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Monitors/host.py` & `simplemonitor-1.9.0b7/simplemonitor/Monitors/host.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Monitors/monitor.py` & `simplemonitor-1.9.0b7/simplemonitor/Monitors/monitor.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Monitors/network.py` & `simplemonitor-1.9.0b7/simplemonitor/Monitors/network.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Monitors/ring.py` & `simplemonitor-1.9.0b7/simplemonitor/Monitors/ring.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/Monitors/service.py` & `simplemonitor-1.9.0b7/simplemonitor/Monitors/service.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/html/header.html` & `simplemonitor-1.9.0b7/simplemonitor/html/header.html`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/html/style.css` & `simplemonitor-1.9.0b7/simplemonitor/html/style.css`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/monitor.py` & `simplemonitor-1.9.0b7/simplemonitor/monitor.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/simplemonitor.py` & `simplemonitor-1.9.0b7/simplemonitor/simplemonitor.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/util/__init__.py` & `simplemonitor-1.9.0b7/simplemonitor/util/__init__.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/util/envconfig.py` & `simplemonitor-1.9.0b7/simplemonitor/util/envconfig.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor/winmonitor.py` & `simplemonitor-1.9.0b7/simplemonitor/winmonitor.py`

 * *Files identical despite different names*

### Comparing `simplemonitor-1.9.0b6/simplemonitor.egg-info/PKG-INFO` & `simplemonitor-1.9.0b7/simplemonitor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplemonitor
-Version: 1.9.0b6
+Version: 1.9.0b7
 Summary: A simple network and host monitor
 Home-page: https://github.com/jamesoff/simplemonitor
 Author: James Seward
 Author-email: james@jamesoff.net
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/jamesoff/simplemonitor.svg?branch=master)](https://travis-ci.org/jamesoff/simplemonitor) [![codecov](https://codecov.io/gh/jamesoff/simplemonitor/branch/master/graph/badge.svg)](https://codecov.io/gh/jamesoff/simplemonitor) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `simplemonitor-1.9.0b6/simplemonitor.egg-info/SOURCES.txt` & `simplemonitor-1.9.0b7/simplemonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

