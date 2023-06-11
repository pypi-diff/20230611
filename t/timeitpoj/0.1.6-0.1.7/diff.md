# Comparing `tmp/timeitpoj-0.1.6.tar.gz` & `tmp/timeitpoj-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeitpoj-0.1.6.tar", max compression
+gzip compressed data, was "timeitpoj-0.1.7.tar", max compression
```

## Comparing `timeitpoj-0.1.6.tar` & `timeitpoj-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1944 2023-06-06 07:05:21.764410 timeitpoj-0.1.6/README.md
--rwxr-xr-x   0        0        0      960 2023-06-08 06:56:25.804921 timeitpoj-0.1.6/pyproject.toml
--rwxr-xr-x   0        0        0       35 2023-06-06 06:50:58.047770 timeitpoj-0.1.6/timeitpoj/__init__.py
--rwxr-xr-x   0        0        0     4534 2023-06-05 12:28:55.944886 timeitpoj-0.1.6/timeitpoj/task_report.py
--rwxr-xr-x   0        0        0     6068 2023-06-08 06:56:21.058164 timeitpoj-0.1.6/timeitpoj/timeit.py
--rwxr-xr-x   0        0        0        0 2023-06-07 12:01:50.735335 timeitpoj-0.1.6/timeitpoj/timer/__init__.py
--rwxr-xr-x   0        0        0      498 2023-06-07 12:00:38.457110 timeitpoj-0.1.6/timeitpoj/timer/internal_timer.py
--rwxr-xr-x   0        0        0     3061 2023-06-07 14:15:45.437874 timeitpoj-0.1.6/timeitpoj/timer/timer.py
--rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.6/timeitpoj/utils/__init__.py
--rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.6/timeitpoj/utils/constants.py
--rwxr-xr-x   0        0        0     1141 2023-06-07 14:03:02.786124 timeitpoj-0.1.6/timeitpoj/utils/misc.py
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 timeitpoj-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1944 2023-06-11 08:33:52.325145 timeitpoj-0.1.7/README.md
+-rw-r--r--   0        0        0     1005 2023-06-11 11:39:17.539204 timeitpoj-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-06-11 08:33:52.325145 timeitpoj-0.1.7/timeitpoj/__init__.py
+-rw-r--r--   0        0        0     4540 2023-06-11 11:27:56.758114 timeitpoj-0.1.7/timeitpoj/task_report.py
+-rw-r--r--   0        0        0     6068 2023-06-11 11:17:54.230416 timeitpoj-0.1.7/timeitpoj/timeit.py
+-rw-r--r--   0        0        0        0 2023-06-11 08:33:52.325145 timeitpoj-0.1.7/timeitpoj/timer/__init__.py
+-rw-r--r--   0        0        0      498 2023-06-11 08:33:52.325145 timeitpoj-0.1.7/timeitpoj/timer/internal_timer.py
+-rw-r--r--   0        0        0     3061 2023-06-11 11:17:54.230416 timeitpoj-0.1.7/timeitpoj/timer/timer.py
+-rw-r--r--   0        0        0        0 2023-06-11 08:33:52.325145 timeitpoj-0.1.7/timeitpoj/utils/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-11 08:33:52.328478 timeitpoj-0.1.7/timeitpoj/utils/constants.py
+-rw-r--r--   0        0        0     1141 2023-06-11 08:33:52.328478 timeitpoj-0.1.7/timeitpoj/utils/misc.py
+-rw-r--r--   0        0        0     2944 1970-01-01 00:00:00.000000 timeitpoj-0.1.7/PKG-INFO
```

### Comparing `timeitpoj-0.1.6/README.md` & `timeitpoj-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.6/pyproject.toml` & `timeitpoj-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timeitpoj"
-version = "0.1.6"
+version = "0.1.7"
 description = "yet another random library for measuring python performance"
 authors = ["Jari Van Melckebeke <jarivanmelckebeke@gmail.com>"]
 maintainers = ["Jari Van Melckebeke <jarivanmelckebeke@gmail.com>"]
 repository = "https://github.com/jvanmelckebeke/timeitpoj"
 homepage = "https://github.com/jvanmelckebeke/timeitpoj"
 
 
@@ -12,21 +12,22 @@
 readme = "README.md"
 keywords = ["timeit", "performance", "benchmark", "time", "measure"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: System :: Logging",
     "Topic :: System :: Networking :: Monitoring",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `timeitpoj-0.1.6/timeitpoj/task_report.py` & `timeitpoj-0.1.7/timeitpoj/task_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Union
+from typing import Union, List
 
 from timeitpoj.utils import constants
 from timeitpoj.utils.misc import reformat_units, format_percentage, time_to_str
 
 PADDING_SECONDS = len("seconds")
 
 
 class TaskReport:
     def __init__(self,
                  name: str,
-                 times: Union[list[float], float],
+                 times: Union[List[float], float],
                  count: int,
                  ratio: float,
-                 children: list["TaskReport"],
+                 children: List["TaskReport"],
                  padding_name: int):
         self.name = name
         self.times = times if isinstance(times, list) else [times]
         self.count = count
         self.ratio = ratio
         self.children = children
```

### Comparing `timeitpoj-0.1.6/timeitpoj/timeit.py` & `timeitpoj-0.1.7/timeitpoj/timeit.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.6/timeitpoj/timer/timer.py` & `timeitpoj-0.1.7/timeitpoj/timer/timer.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.6/timeitpoj/utils/misc.py` & `timeitpoj-0.1.7/timeitpoj/utils/misc.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.6/PKG-INFO` & `timeitpoj-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: timeitpoj
-Version: 0.1.6
+Version: 0.1.7
 Summary: yet another random library for measuring python performance
 Home-page: https://github.com/jvanmelckebeke/timeitpoj
 License: MIT
 Keywords: timeit,performance,benchmark,time,measure
 Author: Jari Van Melckebeke
 Author-email: jarivanmelckebeke@gmail.com
 Maintainer: Jari Van Melckebeke
 Maintainer-email: jarivanmelckebeke@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Utilities
 Project-URL: Repository, https://github.com/jvanmelckebeke/timeitpoj
```

