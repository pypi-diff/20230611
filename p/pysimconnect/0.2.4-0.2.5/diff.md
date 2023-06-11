# Comparing `tmp/pysimconnect-0.2.4.tar.gz` & `tmp/pysimconnect-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimconnect-0.2.4.tar", last modified: Tue Mar 29 14:38:21 2022, max compression
+gzip compressed data, was "pysimconnect-0.2.5.tar", last modified: Sun Jun 11 10:51:55 2023, max compression
```

## Comparing `pysimconnect-0.2.4.tar` & `pysimconnect-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 psurry     (503) staff       (20)        0 2022-03-29 14:38:21.635191 pysimconnect-0.2.4/
--rw-r--r--   0 psurry     (503) staff       (20)     1074 2022-02-03 19:09:57.000000 pysimconnect-0.2.4/LICENSE
--rw-r--r--   0 psurry     (503) staff       (20)       83 2022-02-03 19:28:12.000000 pysimconnect-0.2.4/MANIFEST.in
--rw-r--r--   0 psurry     (503) staff       (20)     8601 2022-03-29 14:38:21.635384 pysimconnect-0.2.4/PKG-INFO
--rw-r--r--   0 psurry     (503) staff       (20)     7917 2022-03-19 12:03:34.000000 pysimconnect-0.2.4/README.md
--rw-r--r--   0 psurry     (503) staff       (20)      104 2022-02-03 18:24:20.000000 pysimconnect-0.2.4/pyproject.toml
-drwxr-xr-x   0 psurry     (503) staff       (20)        0 2022-03-29 14:38:21.617109 pysimconnect-0.2.4/pysimconnect.egg-info/
--rw-r--r--   0 psurry     (503) staff       (20)     8601 2022-03-29 14:38:21.000000 pysimconnect-0.2.4/pysimconnect.egg-info/PKG-INFO
--rw-r--r--   0 psurry     (503) staff       (20)      732 2022-03-29 14:38:21.000000 pysimconnect-0.2.4/pysimconnect.egg-info/SOURCES.txt
--rw-r--r--   0 psurry     (503) staff       (20)        1 2022-03-29 14:38:21.000000 pysimconnect-0.2.4/pysimconnect.egg-info/dependency_links.txt
--rw-r--r--   0 psurry     (503) staff       (20)       58 2022-03-29 14:38:21.000000 pysimconnect-0.2.4/pysimconnect.egg-info/entry_points.txt
--rw-r--r--   0 psurry     (503) staff       (20)       31 2022-03-29 14:38:21.000000 pysimconnect-0.2.4/pysimconnect.egg-info/requires.txt
--rw-r--r--   0 psurry     (503) staff       (20)       11 2022-03-29 14:38:21.000000 pysimconnect-0.2.4/pysimconnect.egg-info/top_level.txt
-drwxr-xr-x   0 psurry     (503) staff       (20)        0 2022-03-29 14:38:21.619547 pysimconnect-0.2.4/scripts/
--rwx------   0 psurry     (503) staff       (20)    41357 2022-01-31 21:03:07.000000 pysimconnect-0.2.4/scripts/SimConnect.h
--rwx------   0 psurry     (503) staff       (20)    38267 2022-01-31 22:06:48.000000 pysimconnect-0.2.4/scripts/SimConnect_cpp.h
--rw-r--r--   0 psurry     (503) staff       (20)    11415 2022-02-13 13:03:10.000000 pysimconnect-0.2.4/scripts/all_units.json
--rwx------   0 psurry     (503) staff       (20)        0 2022-01-31 22:06:24.000000 pysimconnect-0.2.4/scripts/float.h
--rwxr-xr-x   0 psurry     (503) staff       (20)     6754 2022-02-19 16:09:30.000000 pysimconnect-0.2.4/scripts/genscdefs.py
--rw-r--r--   0 psurry     (503) staff       (20)     1107 2022-02-19 19:50:06.000000 pysimconnect-0.2.4/scripts/mkidx.py
--rw-r--r--   0 psurry     (503) staff       (20)     2511 2022-02-20 13:48:55.000000 pysimconnect-0.2.4/scripts/prepvars.py
--rw-r--r--   0 psurry     (503) staff       (20)     3704 2022-02-20 23:22:31.000000 pysimconnect-0.2.4/scripts/scrapevars.py
--rw-r--r--   0 psurry     (503) staff       (20)      925 2022-03-29 14:38:21.636003 pysimconnect-0.2.4/setup.cfg
-drwxr-xr-x   0 psurry     (503) staff       (20)        0 2022-03-29 14:38:21.634280 pysimconnect-0.2.4/simconnect/
--rwx------   0 psurry     (503) staff       (20)    60416 2022-01-30 22:57:36.000000 pysimconnect-0.2.4/simconnect/SimConnect.dll
--rw-r--r--   0 psurry     (503) staff       (20)      223 2022-02-13 20:55:07.000000 pysimconnect-0.2.4/simconnect/__init__.py
--rw-r--r--   0 psurry     (503) staff       (20)     2910 2022-02-26 12:42:37.000000 pysimconnect-0.2.4/simconnect/_typerpatch.py
--rw-r--r--   0 psurry     (503) staff       (20)     1959 2022-02-03 01:52:38.000000 pysimconnect-0.2.4/simconnect/changedict.py
--rw-r--r--   0 psurry     (503) staff       (20)     6679 2022-02-26 12:42:37.000000 pysimconnect-0.2.4/simconnect/cli.py
--rw-r--r--   0 psurry     (503) staff       (20)     5533 2022-02-19 16:08:46.000000 pysimconnect-0.2.4/simconnect/datadef.py
--rw-r--r--   0 psurry     (503) staff       (20)     2226 2022-02-06 14:32:24.000000 pysimconnect-0.2.4/simconnect/receiver.py
--rwxr-xr-x   0 psurry     (503) staff       (20)     8238 2022-02-19 14:14:09.000000 pysimconnect-0.2.4/simconnect/sc.py
--rwxr-xr-x   0 psurry     (503) staff       (20)    43985 2022-02-19 16:09:14.000000 pysimconnect-0.2.4/simconnect/scdefs.py
--rw-r--r--   0 psurry     (503) staff       (20)  1721798 2022-02-20 23:25:21.000000 pysimconnect-0.2.4/simconnect/scvars.json
--rw-r--r--   0 psurry     (503) staff       (20)     3895 2022-02-13 21:20:27.000000 pysimconnect-0.2.4/simconnect/scvars.py
--rw-r--r--   0 psurry     (503) staff       (20)  3712142 2022-02-20 23:25:36.000000 pysimconnect-0.2.4/simconnect/scvars_idx.json
--rw-r--r--   0 psurry     (503) staff       (20)      442 2022-02-19 16:14:25.000000 pysimconnect-0.2.4/simconnect/winstubs.py
+drwxr-xr-x   0 psurry     (503) staff       (20)        0 2023-06-11 10:51:55.091470 pysimconnect-0.2.5/
+-rw-r--r--   0 psurry     (503) staff       (20)     1074 2022-02-03 19:09:57.000000 pysimconnect-0.2.5/LICENSE
+-rw-r--r--   0 psurry     (503) staff       (20)       83 2022-02-03 19:28:12.000000 pysimconnect-0.2.5/MANIFEST.in
+-rw-r--r--   0 psurry     (503) staff       (20)     8564 2023-06-11 10:51:55.091623 pysimconnect-0.2.5/PKG-INFO
+-rw-r--r--   0 psurry     (503) staff       (20)     7917 2023-06-11 10:48:30.000000 pysimconnect-0.2.5/README.md
+-rw-r--r--   0 psurry     (503) staff       (20)      104 2022-02-03 18:24:20.000000 pysimconnect-0.2.5/pyproject.toml
+drwxr-xr-x   0 psurry     (503) staff       (20)        0 2023-06-11 10:51:55.072919 pysimconnect-0.2.5/pysimconnect.egg-info/
+-rw-r--r--   0 psurry     (503) staff       (20)     8564 2023-06-11 10:51:55.000000 pysimconnect-0.2.5/pysimconnect.egg-info/PKG-INFO
+-rw-r--r--   0 psurry     (503) staff       (20)      732 2023-06-11 10:51:55.000000 pysimconnect-0.2.5/pysimconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 psurry     (503) staff       (20)        1 2023-06-11 10:51:55.000000 pysimconnect-0.2.5/pysimconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 psurry     (503) staff       (20)       58 2023-06-11 10:51:55.000000 pysimconnect-0.2.5/pysimconnect.egg-info/entry_points.txt
+-rw-r--r--   0 psurry     (503) staff       (20)       27 2023-06-11 10:51:55.000000 pysimconnect-0.2.5/pysimconnect.egg-info/requires.txt
+-rw-r--r--   0 psurry     (503) staff       (20)       11 2023-06-11 10:51:55.000000 pysimconnect-0.2.5/pysimconnect.egg-info/top_level.txt
+drwxr-xr-x   0 psurry     (503) staff       (20)        0 2023-06-11 10:51:55.075835 pysimconnect-0.2.5/scripts/
+-rwx------   0 psurry     (503) staff       (20)    41357 2022-01-31 21:03:07.000000 pysimconnect-0.2.5/scripts/SimConnect.h
+-rwx------   0 psurry     (503) staff       (20)    38267 2022-01-31 22:06:48.000000 pysimconnect-0.2.5/scripts/SimConnect_cpp.h
+-rw-r--r--   0 psurry     (503) staff       (20)    11415 2022-02-13 13:03:10.000000 pysimconnect-0.2.5/scripts/all_units.json
+-rwx------   0 psurry     (503) staff       (20)        0 2022-01-31 22:06:24.000000 pysimconnect-0.2.5/scripts/float.h
+-rwxr-xr-x   0 psurry     (503) staff       (20)     6754 2022-02-19 16:09:30.000000 pysimconnect-0.2.5/scripts/genscdefs.py
+-rw-r--r--   0 psurry     (503) staff       (20)     1107 2022-02-19 19:50:06.000000 pysimconnect-0.2.5/scripts/mkidx.py
+-rw-r--r--   0 psurry     (503) staff       (20)     2511 2022-02-20 13:48:55.000000 pysimconnect-0.2.5/scripts/prepvars.py
+-rw-r--r--   0 psurry     (503) staff       (20)     3704 2022-02-20 23:22:31.000000 pysimconnect-0.2.5/scripts/scrapevars.py
+-rw-r--r--   0 psurry     (503) staff       (20)      921 2023-06-11 10:51:55.092107 pysimconnect-0.2.5/setup.cfg
+drwxr-xr-x   0 psurry     (503) staff       (20)        0 2023-06-11 10:51:55.090974 pysimconnect-0.2.5/simconnect/
+-rwx------   0 psurry     (503) staff       (20)    60416 2022-01-30 22:57:36.000000 pysimconnect-0.2.5/simconnect/SimConnect.dll
+-rw-r--r--   0 psurry     (503) staff       (20)      223 2022-02-13 20:55:07.000000 pysimconnect-0.2.5/simconnect/__init__.py
+-rw-r--r--   0 psurry     (503) staff       (20)     2918 2023-06-11 10:47:50.000000 pysimconnect-0.2.5/simconnect/_typerpatch.py
+-rw-r--r--   0 psurry     (503) staff       (20)     1959 2022-02-03 01:52:38.000000 pysimconnect-0.2.5/simconnect/changedict.py
+-rw-r--r--   0 psurry     (503) staff       (20)     6679 2022-02-26 12:42:37.000000 pysimconnect-0.2.5/simconnect/cli.py
+-rw-r--r--   0 psurry     (503) staff       (20)     5533 2022-02-19 16:08:46.000000 pysimconnect-0.2.5/simconnect/datadef.py
+-rw-r--r--   0 psurry     (503) staff       (20)     2226 2022-02-06 14:32:24.000000 pysimconnect-0.2.5/simconnect/receiver.py
+-rwxr-xr-x   0 psurry     (503) staff       (20)     8238 2022-02-19 14:14:09.000000 pysimconnect-0.2.5/simconnect/sc.py
+-rwxr-xr-x   0 psurry     (503) staff       (20)    43985 2022-02-19 16:09:14.000000 pysimconnect-0.2.5/simconnect/scdefs.py
+-rw-r--r--   0 psurry     (503) staff       (20)  1721798 2022-02-20 23:25:21.000000 pysimconnect-0.2.5/simconnect/scvars.json
+-rw-r--r--   0 psurry     (503) staff       (20)     3895 2022-02-13 21:20:27.000000 pysimconnect-0.2.5/simconnect/scvars.py
+-rw-r--r--   0 psurry     (503) staff       (20)  3712142 2022-02-20 23:25:36.000000 pysimconnect-0.2.5/simconnect/scvars_idx.json
+-rw-r--r--   0 psurry     (503) staff       (20)      442 2022-02-19 16:14:25.000000 pysimconnect-0.2.5/simconnect/winstubs.py
```

### Comparing `pysimconnect-0.2.4/LICENSE` & `pysimconnect-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/PKG-INFO` & `pysimconnect-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pysimconnect
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python wrapper for Microsoft FlightSimulator 2020 SimConnect SDK
 Home-page: https://github.com/patricksurry/pysimconnect
 Author: Patrick Surry
 Author-email: patrick.surry@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/patricksurry/pysimconnect/issues
 Keywords: pysimconnect,SimConnect,SimVars,ctypes,SDK,API,FS2020,Microsoft Flight Simulator
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -187,13 +185,11 @@
 ---
 
 Bump version in `setup.cfg` then following https://packaging.python.org/en/latest/tutorials/packaging-projects/
 
     python3 -m build
     git commit -am ...
     git push origin
-    git tag v0.1.1
+    git tag v0.2.5
     git push origin --tags
     python3 -m twine upload dist/*0.1.1*  # login with __token__ / pypi...
 
-
-
```

### Comparing `pysimconnect-0.2.4/README.md` & `pysimconnect-0.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -169,11 +169,11 @@
 ---
 
 Bump version in `setup.cfg` then following https://packaging.python.org/en/latest/tutorials/packaging-projects/
 
     python3 -m build
     git commit -am ...
     git push origin
-    git tag v0.1.1
+    git tag v0.2.5
     git push origin --tags
     python3 -m twine upload dist/*0.1.1*  # login with __token__ / pypi...
```

### Comparing `pysimconnect-0.2.4/pysimconnect.egg-info/PKG-INFO` & `pysimconnect-0.2.5/pysimconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pysimconnect
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python wrapper for Microsoft FlightSimulator 2020 SimConnect SDK
 Home-page: https://github.com/patricksurry/pysimconnect
 Author: Patrick Surry
 Author-email: patrick.surry@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/patricksurry/pysimconnect/issues
 Keywords: pysimconnect,SimConnect,SimVars,ctypes,SDK,API,FS2020,Microsoft Flight Simulator
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -187,13 +185,11 @@
 ---
 
 Bump version in `setup.cfg` then following https://packaging.python.org/en/latest/tutorials/packaging-projects/
 
     python3 -m build
     git commit -am ...
     git push origin
-    git tag v0.1.1
+    git tag v0.2.5
     git push origin --tags
     python3 -m twine upload dist/*0.1.1*  # login with __token__ / pypi...
 
-
-
```

### Comparing `pysimconnect-0.2.4/pysimconnect.egg-info/SOURCES.txt` & `pysimconnect-0.2.5/pysimconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/scripts/SimConnect.h` & `pysimconnect-0.2.5/scripts/SimConnect.h`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/scripts/SimConnect_cpp.h` & `pysimconnect-0.2.5/scripts/SimConnect_cpp.h`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/scripts/all_units.json` & `pysimconnect-0.2.5/scripts/all_units.json`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/scripts/genscdefs.py` & `pysimconnect-0.2.5/scripts/genscdefs.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/scripts/mkidx.py` & `pysimconnect-0.2.5/scripts/mkidx.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/scripts/prepvars.py` & `pysimconnect-0.2.5/scripts/prepvars.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/scripts/scrapevars.py` & `pysimconnect-0.2.5/scripts/scrapevars.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/setup.cfg` & `pysimconnect-0.2.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pysimconnect
-version = 0.2.4
+version = 0.2.5
 author = Patrick Surry
 author_email = patrick.surry@gmail.com
 description = Python wrapper for Microsoft FlightSimulator 2020 SimConnect SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = pysimconnect, SimConnect, SimVars, ctypes, SDK, API, FS2020, Microsoft Flight Simulator
 url = https://github.com/patricksurry/pysimconnect
@@ -15,16 +15,16 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = simconnect
 python_requires = >=3.6
 install_requires = 
-	typer >= 0.4.0
-	click >= 8.0.1
+	typer >= 0.9
+	click >= 8.1
 	lunr
 
 [options.entry_points]
 console_scripts = 
 	simconnect = simconnect.cli:app [typer]
 
 [options.package_data]
```

### Comparing `pysimconnect-0.2.4/simconnect/SimConnect.dll` & `pysimconnect-0.2.5/simconnect/SimConnect.dll`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/_typerpatch.py` & `pysimconnect-0.2.5/simconnect/_typerpatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Provides powershell fix from https://github.com/tiangolo/typer/pull/360 until new typer release
 
 from typing import List, Tuple
 import click
 import os
 from typer import _completion_shared
-from typer.utils import _get_click_major
+from typer._compat_utils import _get_click_major
 
 
 if '_TYPER_CURSOR_POSITION' not in _completion_shared.COMPLETION_SCRIPT_POWER_SHELL:
     _pwsh_script = """
 Import-Module PSReadLine
 Set-PSReadLineKeyHandler -Chord Tab -Function MenuComplete
 $scriptblock = {
```

### Comparing `pysimconnect-0.2.4/simconnect/changedict.py` & `pysimconnect-0.2.5/simconnect/changedict.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/cli.py` & `pysimconnect-0.2.5/simconnect/cli.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/datadef.py` & `pysimconnect-0.2.5/simconnect/datadef.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/receiver.py` & `pysimconnect-0.2.5/simconnect/receiver.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/sc.py` & `pysimconnect-0.2.5/simconnect/sc.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/scdefs.py` & `pysimconnect-0.2.5/simconnect/scdefs.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/scvars.json` & `pysimconnect-0.2.5/simconnect/scvars.json`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/scvars.py` & `pysimconnect-0.2.5/simconnect/scvars.py`

 * *Files identical despite different names*

### Comparing `pysimconnect-0.2.4/simconnect/scvars_idx.json` & `pysimconnect-0.2.5/simconnect/scvars_idx.json`

 * *Files identical despite different names*

