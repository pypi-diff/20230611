# Comparing `tmp/asv_runner-0.0.3.tar.gz` & `tmp/asv_runner-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asv_runner-0.0.3.tar", last modified: Mon Jun  5 03:29:58 2023, max compression
+gzip compressed data, was "asv_runner-0.0.4.tar", last modified: Sun Jun 11 15:20:24 2023, max compression
```

## Comparing `asv_runner-0.0.3.tar` & `asv_runner-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      286 2023-06-05 03:29:51.801955 asv_runner-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/__init__.py
--rw-r--r--   0        0        0     2759 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/aux.py
--rw-r--r--   0        0        0      585 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/__init__.py
--rw-r--r--   0        0        0    10646 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/_base.py
--rw-r--r--   0        0        0      183 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/_exceptions.py
--rw-r--r--   0        0        0     3404 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/_maxrss.py
--rw-r--r--   0        0        0      817 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/mem.py
--rw-r--r--   0        0        0      587 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/peakmem.py
--rw-r--r--   0        0        0     5400 2023-06-05 03:29:51.801955 asv_runner-0.0.3/asv_runner/benchmarks/time.py
--rw-r--r--   0        0        0     1759 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/benchmarks/timeraw.py
--rw-r--r--   0        0        0      581 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/benchmarks/track.py
--rw-r--r--   0        0        0      317 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/check.py
--rw-r--r--   0        0        0    11444 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/console.py
--rw-r--r--   0        0        0     5865 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/discovery.py
--rw-r--r--   0        0        0     1117 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/run.py
--rw-r--r--   0        0        0     5209 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/server.py
--rw-r--r--   0        0        0      473 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/setup_cache.py
--rw-r--r--   0        0        0     9809 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/statistics.py
--rw-r--r--   0        0        0     1941 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/timing.py
--rw-r--r--   0        0        0     3467 2023-06-05 03:29:51.805956 asv_runner-0.0.3/asv_runner/util.py
--rw-r--r--   0        0        0      838 2023-06-05 03:29:58.218110 asv_runner-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 asv_runner-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      286 2023-06-11 15:20:15.306004 asv_runner-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/__init__.py
+-rw-r--r--   0        0        0     2759 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/_aux.py
+-rw-r--r--   0        0        0      585 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/__init__.py
+-rw-r--r--   0        0        0    10646 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/_base.py
+-rw-r--r--   0        0        0      183 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/_exceptions.py
+-rw-r--r--   0        0        0     3404 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/_maxrss.py
+-rw-r--r--   0        0        0      817 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/mem.py
+-rw-r--r--   0        0        0      587 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/peakmem.py
+-rw-r--r--   0        0        0     5400 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/time.py
+-rw-r--r--   0        0        0     1759 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/timeraw.py
+-rw-r--r--   0        0        0      581 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/track.py
+-rw-r--r--   0        0        0      318 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/check.py
+-rw-r--r--   0        0        0    11444 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/console.py
+-rw-r--r--   0        0        0     5866 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/discovery.py
+-rw-r--r--   0        0        0     1118 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/run.py
+-rw-r--r--   0        0        0     5210 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/server.py
+-rw-r--r--   0        0        0      474 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/setup_cache.py
+-rw-r--r--   0        0        0     9809 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/statistics.py
+-rw-r--r--   0        0        0     1941 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/timing.py
+-rw-r--r--   0        0        0     3467 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/util.py
+-rw-r--r--   0        0        0      838 2023-06-11 15:20:24.173978 asv_runner-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 asv_runner-0.0.4/PKG-INFO
```

### Comparing `asv_runner-0.0.3/asv_runner/aux.py` & `asv_runner-0.0.4/asv_runner/_aux.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/benchmarks/__init__.py` & `asv_runner-0.0.4/asv_runner/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/benchmarks/_base.py` & `asv_runner-0.0.4/asv_runner/benchmarks/_base.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/benchmarks/_maxrss.py` & `asv_runner-0.0.4/asv_runner/benchmarks/_maxrss.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/benchmarks/mem.py` & `asv_runner-0.0.4/asv_runner/benchmarks/mem.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/benchmarks/peakmem.py` & `asv_runner-0.0.4/asv_runner/benchmarks/peakmem.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/benchmarks/time.py` & `asv_runner-0.0.4/asv_runner/benchmarks/time.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/benchmarks/timeraw.py` & `asv_runner-0.0.4/asv_runner/benchmarks/timeraw.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/benchmarks/track.py` & `asv_runner-0.0.4/asv_runner/benchmarks/track.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/console.py` & `asv_runner-0.0.4/asv_runner/console.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/discovery.py` & `asv_runner-0.0.4/asv_runner/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 import inspect
 import json
 import os
 import pkgutil
 import traceback
 
-from .aux import update_sys_path
+from ._aux import update_sys_path
 from .benchmarks import benchmark_types
 
 
 def _get_benchmark(attr_name, module, klass, func):
     try:
         name = func.benchmark_name
     except AttributeError:
```

### Comparing `asv_runner-0.0.3/asv_runner/run.py` & `asv_runner-0.0.4/asv_runner/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import math
 import pickle
 
-from .aux import set_cpu_affinity_from_params
+from ._aux import set_cpu_affinity_from_params
 from .discovery import get_benchmark_from_name
 
 
 def _run(args):
     (benchmark_dir, benchmark_id, params_str, profile_path, result_file) = args
 
     extra_params = json.loads(params_str)
```

### Comparing `asv_runner-0.0.3/asv_runner/server.py` & `asv_runner-0.0.4/asv_runner/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import struct
 import sys
 import tempfile
 import time
 import timeit
 
-from .aux import posix_redirect_output, update_sys_path
+from ._aux import posix_redirect_output, update_sys_path
 from .discovery import disc_benchmarks
 from .run import _run
 
 wall_timer = timeit.default_timer
 
 
 def recvall(sock, size):
```

### Comparing `asv_runner-0.0.3/asv_runner/statistics.py` & `asv_runner-0.0.4/asv_runner/statistics.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/timing.py` & `asv_runner-0.0.4/asv_runner/timing.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/asv_runner/util.py` & `asv_runner-0.0.4/asv_runner/util.py`

 * *Files identical despite different names*

### Comparing `asv_runner-0.0.3/pyproject.toml` & `asv_runner-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 description = "Core Python benchmark code for ASV"
 authors = [
     { name = "Rohit Goswami", email = "rog32@hi.is" },
 ]
 maintainers = [
     { name = "Rohit Goswami", email = "rog32@hi.is" },
 ]
-version = "0.0.3"
+version = "0.0.4"
 dependencies = []
 requires-python = ">=3.7"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `asv_runner-0.0.3/PKG-INFO` & `asv_runner-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asv-runner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Core Python benchmark code for ASV
 Author-Email: Rohit Goswami <rog32@hi.is>
 Maintainer-Email: Rohit Goswami <rog32@hi.is>
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: lint
 Requires-Dist: ruff>=0.0.265; extra == "lint"
```

