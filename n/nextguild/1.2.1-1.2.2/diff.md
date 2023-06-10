# Comparing `tmp/nextguild-1.2.1.tar.gz` & `tmp/nextguild-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.2.1.tar", last modified: Sat Jun 10 22:24:56 2023, max compression
+gzip compressed data, was "nextguild-1.2.2.tar", last modified: Sat Jun 10 22:31:43 2023, max compression
```

## Comparing `nextguild-1.2.1.tar` & `nextguild-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:24:56.982261 nextguild-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 22:24:46.000000 nextguild-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:24:56.982261 nextguild-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-10 22:24:46.000000 nextguild-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:24:56.978261 nextguild-1.2.1/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-10 22:24:46.000000 nextguild-1.2.1/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-06-10 22:24:46.000000 nextguild-1.2.1/nextguild/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    41054 2023-06-10 22:24:46.000000 nextguild-1.2.1/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-10 22:24:46.000000 nextguild-1.2.1/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    48069 2023-06-10 22:24:46.000000 nextguild-1.2.1/nextguild/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:24:56.982261 nextguild-1.2.1/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:24:56.000000 nextguild-1.2.1/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 22:24:56.000000 nextguild-1.2.1/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:24:56.000000 nextguild-1.2.1/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 22:24:56.000000 nextguild-1.2.1/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-10 22:24:46.000000 nextguild-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 22:24:56.982261 nextguild-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:31:43.986807 nextguild-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 22:31:28.000000 nextguild-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:31:43.986807 nextguild-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-10 22:31:28.000000 nextguild-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:31:43.982807 nextguild-1.2.2/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26735 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41054 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48069 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:31:43.986807 nextguild-1.2.2/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:31:43.000000 nextguild-1.2.2/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 22:31:43.000000 nextguild-1.2.2/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:31:43.000000 nextguild-1.2.2/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 22:31:43.000000 nextguild-1.2.2/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-10 22:31:28.000000 nextguild-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 22:31:43.986807 nextguild-1.2.2/setup.cfg
```

### Comparing `nextguild-1.2.1/LICENSE` & `nextguild-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.1/PKG-INFO` & `nextguild-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.1
+Version: 1.2.2
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.1/README.md` & `nextguild-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.1/nextguild/classes.py` & `nextguild-1.2.2/nextguild/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         scenarios = [
             ('serverId'),
             ('server', 'id'),
             ('message', 'serverId'),
             ('webhook', 'serverId'),
             ('doc', 'serverId'),
             ('calendarEvent', 'serverId'),
+            ('reaction', 'serverId')
         ]
         return self._scenario(event_data, scenarios)
             
     def _get_group_id(self, event_data: dict):
         scenarios = [
             ('group', 'id'),
             ('message', 'groupId'),
```

### Comparing `nextguild-1.2.1/nextguild/client.py` & `nextguild-1.2.2/nextguild/client.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.1/nextguild/embed.py` & `nextguild-1.2.2/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.1/nextguild/events.py` & `nextguild-1.2.2/nextguild/events.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.1/nextguild.egg-info/PKG-INFO` & `nextguild-1.2.2/nextguild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.1
+Version: 1.2.2
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.1/pyproject.toml` & `nextguild-1.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

