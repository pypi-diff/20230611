# Comparing `tmp/py-sbatch-script-0.2.tar.gz` & `tmp/py-sbatch-script-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sbatch-script-0.2.tar", last modified: Sun Jun 11 18:01:03 2023, max compression
+gzip compressed data, was "py-sbatch-script-0.3.tar", last modified: Sun Jun 11 18:02:43 2023, max compression
```

## Comparing `py-sbatch-script-0.2.tar` & `py-sbatch-script-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-11 18:01:03.596246 py-sbatch-script-0.2/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1079 2023-06-11 14:11:02.000000 py-sbatch-script-0.2/LICENSE
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      600 2023-06-11 18:01:03.592913 py-sbatch-script-0.2/PKG-INFO
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      112 2023-06-11 17:39:28.000000 py-sbatch-script-0.2/README.rst
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      730 2023-06-11 18:00:59.000000 py-sbatch-script-0.2/pyproject.toml
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       38 2023-06-11 18:01:03.596246 py-sbatch-script-0.2/setup.cfg
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-06-11 17:39:56.000000 py-sbatch-script-0.2/setup.py
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-11 18:01:03.592913 py-sbatch-script-0.2/src/
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-11 18:01:03.592913 py-sbatch-script-0.2/src/py_sbatch_script/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      270 2023-06-11 17:35:59.000000 py-sbatch-script-0.2/src/py_sbatch_script/__init__.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2103 2023-06-11 18:00:47.000000 py-sbatch-script-0.2/src/py_sbatch_script/cli.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1709 2023-06-11 17:30:14.000000 py-sbatch-script-0.2/src/py_sbatch_script/pprint.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      671 2023-06-11 17:36:21.000000 py-sbatch-script-0.2/src/py_sbatch_script/prompt.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1816 2023-06-11 18:00:46.000000 py-sbatch-script-0.2/src/py_sbatch_script/sbatch_function.py
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-11 18:01:03.592913 py-sbatch-script-0.2/src/py_sbatch_script.egg-info/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      600 2023-06-11 18:01:03.000000 py-sbatch-script-0.2/src/py_sbatch_script.egg-info/PKG-INFO
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      471 2023-06-11 18:01:03.000000 py-sbatch-script-0.2/src/py_sbatch_script.egg-info/SOURCES.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2023-06-11 18:01:03.000000 py-sbatch-script-0.2/src/py_sbatch_script.egg-info/dependency_links.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       63 2023-06-11 18:01:03.000000 py-sbatch-script-0.2/src/py_sbatch_script.egg-info/entry_points.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       15 2023-06-11 18:01:03.000000 py-sbatch-script-0.2/src/py_sbatch_script.egg-info/requires.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       17 2023-06-11 18:01:03.000000 py-sbatch-script-0.2/src/py_sbatch_script.egg-info/top_level.txt
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-11 18:02:43.236241 py-sbatch-script-0.3/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1079 2023-06-11 14:11:02.000000 py-sbatch-script-0.3/LICENSE
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      600 2023-06-11 18:02:43.236241 py-sbatch-script-0.3/PKG-INFO
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      112 2023-06-11 17:39:28.000000 py-sbatch-script-0.3/README.rst
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      730 2023-06-11 18:02:39.000000 py-sbatch-script-0.3/pyproject.toml
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       38 2023-06-11 18:02:43.236241 py-sbatch-script-0.3/setup.cfg
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2023-06-11 17:39:56.000000 py-sbatch-script-0.3/setup.py
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-11 18:02:43.232908 py-sbatch-script-0.3/src/
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-11 18:02:43.232908 py-sbatch-script-0.3/src/py_sbatch_script/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      270 2023-06-11 17:35:59.000000 py-sbatch-script-0.3/src/py_sbatch_script/__init__.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2103 2023-06-11 18:00:47.000000 py-sbatch-script-0.3/src/py_sbatch_script/cli.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1709 2023-06-11 17:30:14.000000 py-sbatch-script-0.3/src/py_sbatch_script/pprint.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      671 2023-06-11 17:36:21.000000 py-sbatch-script-0.3/src/py_sbatch_script/prompt.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1818 2023-06-11 18:02:33.000000 py-sbatch-script-0.3/src/py_sbatch_script/sbatch_function.py
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2023-06-11 18:02:43.236241 py-sbatch-script-0.3/src/py_sbatch_script.egg-info/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      600 2023-06-11 18:02:43.000000 py-sbatch-script-0.3/src/py_sbatch_script.egg-info/PKG-INFO
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      471 2023-06-11 18:02:43.000000 py-sbatch-script-0.3/src/py_sbatch_script.egg-info/SOURCES.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2023-06-11 18:02:43.000000 py-sbatch-script-0.3/src/py_sbatch_script.egg-info/dependency_links.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       63 2023-06-11 18:02:43.000000 py-sbatch-script-0.3/src/py_sbatch_script.egg-info/entry_points.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       15 2023-06-11 18:02:43.000000 py-sbatch-script-0.3/src/py_sbatch_script.egg-info/requires.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       17 2023-06-11 18:02:43.000000 py-sbatch-script-0.3/src/py_sbatch_script.egg-info/top_level.txt
```

### Comparing `py-sbatch-script-0.2/LICENSE` & `py-sbatch-script-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sbatch-script-0.2/PKG-INFO` & `py-sbatch-script-0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sbatch-script
-Version: 0.2
+Version: 0.3
 Summary: Helper utilities for building nice sbatch scripts in Python.
 Author-email: Parantapa Bhattacharya <pb+pypi@parantapa.net>
 Project-URL: homepage, https://github.com/parantapa/py-sbatch-script
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `py-sbatch-script-0.2/pyproject.toml` & `py-sbatch-script-0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-sbatch-script"
-version = "0.2"
+version = "0.3"
 authors = [
   { name="Parantapa Bhattacharya", email="pb+pypi@parantapa.net" },
 ]
 description = "Helper utilities for building nice sbatch scripts in Python."
 readme = "README.rst"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `py-sbatch-script-0.2/src/py_sbatch_script/cli.py` & `py-sbatch-script-0.3/src/py_sbatch_script/cli.py`

 * *Files identical despite different names*

### Comparing `py-sbatch-script-0.2/src/py_sbatch_script/pprint.py` & `py-sbatch-script-0.3/src/py_sbatch_script/pprint.py`

 * *Files identical despite different names*

### Comparing `py-sbatch-script-0.2/src/py_sbatch_script/prompt.py` & `py-sbatch-script-0.3/src/py_sbatch_script/prompt.py`

 * *Files identical despite different names*

### Comparing `py-sbatch-script-0.2/src/py_sbatch_script/sbatch_function.py` & `py-sbatch-script-0.3/src/py_sbatch_script/sbatch_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.func = func
 
     def submit(self, sbatch_args: str, *func_args, **func_kwargs):
         save_func_call(self.func.__name__, func_args, func_kwargs)
 
         script_file = os.environ["PY_SBATCH_SCRIPT_FILE"]
         sbatch_args = dedent(sbatch_args).strip()
-        sbatch_cmd = f"sbatch\nsbatch_args\n{script_file}"
+        sbatch_cmd = f"sbatch\n{sbatch_args}\n{script_file}"
         pprint_info("Submitting slurm job:")
         pprint_cmd(sbatch_cmd)
 
         cmd = shlex.split(sbatch_cmd)
         proc = run(cmd, text=True, check=True, capture_output=True)
         if proc.stdout is not None and proc.stdout.strip():
             print("Stdout:", proc.stdout)
```

### Comparing `py-sbatch-script-0.2/src/py_sbatch_script.egg-info/PKG-INFO` & `py-sbatch-script-0.3/src/py_sbatch_script.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sbatch-script
-Version: 0.2
+Version: 0.3
 Summary: Helper utilities for building nice sbatch scripts in Python.
 Author-email: Parantapa Bhattacharya <pb+pypi@parantapa.net>
 Project-URL: homepage, https://github.com/parantapa/py-sbatch-script
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

