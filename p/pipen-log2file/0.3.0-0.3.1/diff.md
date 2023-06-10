# Comparing `tmp/pipen_log2file-0.3.0.tar.gz` & `tmp/pipen_log2file-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_log2file-0.3.0.tar", max compression
+gzip compressed data, was "pipen_log2file-0.3.1.tar", max compression
```

## Comparing `pipen_log2file-0.3.0.tar` & `pipen_log2file-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-06-08 23:03:59.573825 pipen_log2file-0.3.0/LICENSE
--rwxr-xr-x   0        0        0      984 2023-06-08 23:03:59.573825 pipen_log2file-0.3.0/README.md
--rwxr-xr-x   0        0        0     5928 2023-06-08 23:03:59.573825 pipen_log2file-0.3.0/pipen_log2file.py
--rwxr-xr-x   0        0        0      892 2023-06-08 23:03:59.573825 pipen_log2file-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pipen_log2file-0.3.0/setup.py
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 pipen_log2file-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-10 23:05:17.083322 pipen_log2file-0.3.1/LICENSE
+-rwxr-xr-x   0        0        0      984 2023-06-10 23:05:17.083322 pipen_log2file-0.3.1/README.md
+-rwxr-xr-x   0        0        0     5977 2023-06-10 23:05:17.083322 pipen_log2file-0.3.1/pipen_log2file.py
+-rwxr-xr-x   0        0        0      892 2023-06-10 23:05:17.083322 pipen_log2file-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pipen_log2file-0.3.1/setup.py
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 pipen_log2file-0.3.1/PKG-INFO
```

### Comparing `pipen_log2file-0.3.0/LICENSE` & `pipen_log2file-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_log2file-0.3.0/README.md` & `pipen_log2file-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pipen_log2file-0.3.0/pipen_log2file.py` & `pipen_log2file-0.3.1/pipen_log2file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """pipen-log2file plugin: Save running logs to file"""
 from __future__ import annotations
 
 import logging
 from math import ceil
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict, List
+from typing import TYPE_CHECKING, List
 
 from rich.markup import _parse
 from xqute.utils import logger as xqute_logger
 from pipen import plugin
 
 if TYPE_CHECKING:  # pragma: no cover
     from pipen import Pipen, Proc
     from pipen.job import Job
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 xqute_logger_handlers = xqute_logger.handlers
 
 
 def _remove_rich_tags(text: str) -> str:
     """Remove rich tags from text"""
     return "".join(text for _, text, _ in _parse(text) if text)
@@ -86,15 +86,15 @@
         )
         logfile.parent.mkdir(parents=True, exist_ok=True)
         latest_log = pipen.workdir.joinpath("run-latest.log")
         if latest_log.exists() or latest_log.is_symlink():
             latest_log.unlink()
         latest_log.symlink_to(logfile.relative_to(pipen.workdir))
 
-        self._handler = logging.FileHandler(logfile)
+        self._handler = logging.FileHandler(logfile, delay=True)
         self._handler.setFormatter(
             logging.Formatter(
                 "%(asctime)s %(levelname)-1.1s %(plugin_name)-7s %(message)s",
                 datefmt="%m-%d %H:%M:%S",
             )
         )
         self._handler.addFilter(_RemoveRichMarkupFilter())
@@ -124,28 +124,31 @@
         if not proc.plugin_opts.log2file_xqute:
             return
 
         logfile = proc.workdir.joinpath("proc.xqute.log")
         if not proc.plugin_opts.log2file_xqute_append and logfile.exists():
             logfile.unlink()
 
-        self._xqute_handler = logging.FileHandler(logfile)
+        self._xqute_handler = logging.FileHandler(logfile, delay=True)
         self._xqute_handler.setFormatter(
             logging.Formatter(
                 "%(asctime)s %(levelname)-7s %(message)s",
                 datefmt="%Y-%m-%d %H:%M:%S",
             )
         )
         # handler.addFilter(_RemoveRichMarkupFilter())
         xqute_logger.addHandler(self._xqute_handler)
         xqute_logger.setLevel(proc.plugin_opts.log2file_xqute_level.upper())
 
     @plugin.impl
     async def on_proc_done(self, proc: Proc, succeeded: bool | str):
-        if self._xqute_handler and self._xqute_handler in xqute_logger.handlers:
+        if (
+            self._xqute_handler
+            and self._xqute_handler in xqute_logger.handlers
+        ):
             xqute_logger.removeHandler(self._xqute_handler)
             self._xqute_handler = None
 
         if not self._handler:
             return
 
         self._emit_log_progress(proc.name)
```

### Comparing `pipen_log2file-0.3.0/pyproject.toml` & `pipen_log2file-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-log2file"
-version = "0.3.0"
+version = "0.3.1"
 description = "Add verbosal information in logs for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-log2file"
 repository = "https://github.com/pwwang/pipen-log2file"
```

### Comparing `pipen_log2file-0.3.0/setup.py` & `pipen_log2file-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ['pipen>=0.10.0,<0.11.0']
 
 entry_points = \
 {'pipen': ['log2file = pipen_log2file:log2file_plugin']}
 
 setup_kwargs = {
     'name': 'pipen-log2file',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Add verbosal information in logs for pipen.',
     'long_description': '# pipen-log2file\n\nSave running logs to file for [pipen][1].\n\nThe log file is saved to `<workdir>/<pipeline>/.logs/run-<date-time>.log` by default.\nA symlink `<workdir>/<pipeline>/run-latest.log` is created to the latest log file.\n\nThe xqute logs are also saved to `<workdir>/<pipeline>/<proc>/proc.xqute.log`\n\nNote that the original handler of xqute logger is removed during pipeline running.\n\n## Options\n\n- `plugin_opts.log2file_xqute`: Whether to save xqute logs. Default: `True`.\n    if False, the xqute logger will be kept intact.\n- `plugin_opts.log2file_xqute_level`: The log level for xqute logger. Default: `INFO`.\n- `plugin_opts.log2file_xqute_append`: Whether to append to the log file. Default: `False`.\n\n## Installation\n\n```\npip install -U pipen-log2file\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it:\n`plugins=[..., "no:log2file"]`, or uninstall this plugin.\n\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-log2file',
```

### Comparing `pipen_log2file-0.3.0/PKG-INFO` & `pipen_log2file-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-log2file
-Version: 0.3.0
+Version: 0.3.1
 Summary: Add verbosal information in logs for pipen.
 Home-page: https://github.com/pwwang/pipen-log2file
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

