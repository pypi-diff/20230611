# Comparing `tmp/morel-1.0.0.tar.gz` & `tmp/morel-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.0.0.tar", last modified: Sun Jun 11 13:33:58 2023, max compression
+gzip compressed data, was "morel-1.1.0.tar", last modified: Sun Jun 11 15:01:42 2023, max compression
```

## Comparing `morel-1.0.0.tar` & `morel-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 13:33:58.303155 morel-1.0.0/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.0.0/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-11 13:33:58.302155 morel-1.0.0/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.0.0/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-11 13:33:21.000000 morel-1.0.0/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-11 13:33:58.303155 morel-1.0.0/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 13:33:58.300155 morel-1.0.0/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 13:33:58.301155 morel-1.0.0/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       48 2023-06-11 13:30:07.000000 morel-1.0.0/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     2363 2023-06-11 13:31:43.000000 morel-1.0.0/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      904 2023-06-11 13:31:40.000000 morel-1.0.0/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     2061 2023-06-11 13:20:57.000000 morel-1.0.0/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      687 2023-06-11 12:28:03.000000 morel-1.0.0/src/morel/template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 13:33:58.302155 morel-1.0.0/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      335 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-11 13:33:58.000000 morel-1.0.0/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 15:01:42.988043 morel-1.1.0/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.1.0/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-11 15:01:42.987043 morel-1.1.0/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.1.0/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-11 15:01:25.000000 morel-1.1.0/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-11 15:01:42.988043 morel-1.1.0/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 15:01:42.984043 morel-1.1.0/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 15:01:42.985043 morel-1.1.0/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       48 2023-06-11 13:30:07.000000 morel-1.1.0/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     2648 2023-06-11 14:59:29.000000 morel-1.1.0/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1013 2023-06-11 14:52:10.000000 morel-1.1.0/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.1.0/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      687 2023-06-11 12:28:03.000000 morel-1.1.0/src/morel/template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 15:01:42.987043 morel-1.1.0/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      335 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.0.0/LICENSE` & `morel-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.0.0/PKG-INFO` & `morel-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.0.0
+Version: 1.1.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.0.0/pyproject.toml` & `morel-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.0.0/src/morel/app.py` & `morel-1.1.0/src/morel/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,36 @@
-import importlib
-from multiprocessing import JoinableQueue
 import os
 import sys
-from threading import Thread
 import click
+import importlib
+
 from pathlib import Path
+from threading import Thread
 
-from .exploits import addlogger, launchAttack
+from .exploits import launchAttack
 
 with open(Path(Path(__file__).parent, "template.py")) as fs:
     temp = fs.read()
 
 
 @click.group()
-def app():
+@click.option("--logs-dir", "logs", type=click.STRING, envvar="MOREL_LOGS_DIR")
+@click.option(
+    "--flag-regex",
+    "regex",
+    type=click.STRING,
+    envvar="FLAG_REGEX",
+)
+def app(logs, regex):
     """Simple program to aid in the development and testing of exploits."""
-    # click.echo(f"Hello!")
+    if "MOREL_LOGS_DIR" not in os.environ and logs is None:
+        os.environ["MOREL_LOGS_DIR"] = "None"
+    if "FLAG_REGEX" not in os.environ and regex is None:
+        os.environ["FLAG_REGEX"] = "None"
+        click.echo("You may want to set the environment variable FLAG_REGEX")
 
 
 @app.command()
 @click.argument("filename", required=False, type=click.Path())
 def template(filename):
     """Generate a template for your exploit that is compatible with M1lkman"""
     confirmed = True
@@ -63,25 +74,20 @@
     try:
         spec = importlib.util.spec_from_file_location(name, filename.resolve())
         module = importlib.util.module_from_spec(spec)  # type: ignore
         sys.modules[name] = module
         spec.loader.exec_module(module)  # type: ignore
         exploitfun = getattr(sys.modules[name], "main")
     except Exception as e:
-        raise e(f"Error while importing {name}")
+        click.echo("There was an error import your exploit. Please check the syntax.")
+        return
 
-    gametickQueue = JoinableQueue()
-    addlogger(name)
     t = Thread(
         target=launchAttack,
         args=(
             exploitfun,
             target,
-            gametickQueue,
         ),
         name=f"{exploitfun.__module__}_{target}",
     )
-    gametickQueue.put("")
     t.start()
-    gametickQueue.join()
-    gametickQueue.close()
     t.join()
```

### Comparing `morel-1.0.0/src/morel/template.py` & `morel-1.1.0/src/morel/template.py`

 * *Files identical despite different names*

### Comparing `morel-1.0.0/src/morel.egg-info/PKG-INFO` & `morel-1.1.0/src/morel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.0.0
+Version: 1.1.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

