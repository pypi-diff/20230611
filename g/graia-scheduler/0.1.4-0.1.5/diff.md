# Comparing `tmp/graia-scheduler-0.1.4.tar.gz` & `tmp/graia-scheduler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graia-scheduler-0.1.4.tar", last modified: Tue Dec 27 06:23:45 2022, max compression
+gzip compressed data, was "graia-scheduler-0.1.5.tar", last modified: Sun Jun 11 07:23:10 2023, max compression
```

## Comparing `graia-scheduler-0.1.4.tar` & `graia-scheduler-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      991 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/saya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/saya/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/saya/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2022-12-27 06:23:28.703281 graia-scheduler-0.1.4/src/graia/scheduler/utilles.py
--rw-------   0 runner    (1001) docker     (123)     1093 2022-12-27 06:23:45.115131 graia-scheduler-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1273 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/README.md
+-rw-r--r--   0        0        0      991 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2521 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/src/graia/scheduler/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/src/graia/scheduler/exception.py
+-rw-r--r--   0        0        0      129 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/src/graia/scheduler/saya/__init__.py
+-rw-r--r--   0        0        0     1329 2023-06-11 07:22:51.068739 graia-scheduler-0.1.5/src/graia/scheduler/saya/behaviour.py
+-rw-r--r--   0        0        0      471 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/saya/schema.py
+-rw-r--r--   0        0        0     1113 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/service.py
+-rw-r--r--   0        0        0     4760 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/task.py
+-rw-r--r--   0        0        0     3679 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/timers.py
+-rw-r--r--   0        0        0     1524 2023-06-11 07:22:51.072739 graia-scheduler-0.1.5/src/graia/scheduler/utilles.py
+-rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 graia-scheduler-0.1.5/PKG-INFO
```

### Comparing `graia-scheduler-0.1.4/pyproject.toml` & `graia-scheduler-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 requires-python = ">=3.8,<4.0"
 dependencies = [
     "graia-broadcast>=0.19.0",
     "croniter<2.0.0,>=1.0.0",
     "launart<1.0.0,>=0.6.1",
 ]
 name = "graia-scheduler"
-version = "0.1.4"
+version = "0.1.5"
 description = "a scheduler for graia framework"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
```

### Comparing `graia-scheduler-0.1.4/src/graia/scheduler/__init__.py` & `graia-scheduler-0.1.5/src/graia/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.4/src/graia/scheduler/saya/behaviour.py` & `graia-scheduler-0.1.5/src/graia/scheduler/saya/behaviour.py`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.4/src/graia/scheduler/task.py` & `graia-scheduler-0.1.5/src/graia/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.4/src/graia/scheduler/timers.py` & `graia-scheduler-0.1.5/src/graia/scheduler/timers.py`

 * *Files identical despite different names*

### Comparing `graia-scheduler-0.1.4/src/graia/scheduler/utilles.py` & `graia-scheduler-0.1.5/src/graia/scheduler/utilles.py`

 * *Files identical despite different names*

