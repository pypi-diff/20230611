# Comparing `tmp/araby-ai-0.0.1.tar.gz` & `tmp/araby-ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "araby-ai-0.0.1.tar", last modified: Sun Jun 11 13:10:14 2023, max compression
+gzip compressed data, was "araby-ai-0.0.2.tar", last modified: Sun Jun 11 14:05:27 2023, max compression
```

## Comparing `araby-ai-0.0.1.tar` & `araby-ai-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 13:10:14.268000 araby-ai-0.0.1/
--rw-rw----   0 root         (0) everybody  (9997)       20 2023-06-11 12:12:33.000000 araby-ai-0.0.1/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      336 2023-06-11 13:10:14.244000 araby-ai-0.0.1/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 13:10:14.120000 araby-ai-0.0.1/araby_ai/
--rw-rw----   0 root         (0) everybody  (9997)      818 2023-06-11 12:10:46.000000 araby-ai-0.0.1/araby_ai/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 13:10:14.224000 araby-ai-0.0.1/araby_ai.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      336 2023-06-11 13:10:13.000000 araby-ai-0.0.1/araby_ai.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      169 2023-06-11 13:10:13.000000 araby-ai-0.0.1/araby_ai.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-11 13:10:13.000000 araby-ai-0.0.1/araby_ai.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-11 13:10:13.000000 araby-ai-0.0.1/araby_ai.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-11 13:10:14.268000 araby-ai-0.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      377 2023-06-11 12:14:29.000000 araby-ai-0.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 14:05:27.596485 araby-ai-0.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)       20 2023-06-11 12:12:33.000000 araby-ai-0.0.2/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      336 2023-06-11 14:05:27.580485 araby-ai-0.0.2/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 14:05:27.472485 araby-ai-0.0.2/araby_ai/
+-rw-rw----   0 root         (0) everybody  (9997)      842 2023-06-11 14:04:50.000000 araby-ai-0.0.2/araby_ai/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     2656 2023-06-11 13:45:51.000000 araby-ai-0.0.2/araby_ai/writenow.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-11 14:05:27.560485 araby-ai-0.0.2/araby_ai.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      336 2023-06-11 14:05:27.000000 araby-ai-0.0.2/araby_ai.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      190 2023-06-11 14:05:27.000000 araby-ai-0.0.2/araby_ai.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-11 14:05:27.000000 araby-ai-0.0.2/araby_ai.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-11 14:05:27.000000 araby-ai-0.0.2/araby_ai.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-11 14:05:27.596485 araby-ai-0.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      377 2023-06-11 14:05:02.000000 araby-ai-0.0.2/setup.py
```

### Comparing `araby-ai-0.0.1/araby_ai/__init__.py` & `araby-ai-0.0.2/araby_ai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .writenow import *
 import requests
 
 class Client:
 	def __init__(self, email, password):
 		headers = {
 			"authority": "v1.prd.socket.araby.ai",
 			"accept": "application/json, text/plain, */*",
```

