# Comparing `tmp/pipen_runinfo-0.1.0.tar.gz` & `tmp/pipen_runinfo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_runinfo-0.1.0.tar", max compression
+gzip compressed data, was "pipen_runinfo-0.1.1.tar", max compression
```

## Comparing `pipen_runinfo-0.1.0.tar` & `pipen_runinfo-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2755 2023-06-10 06:31:57.015234 pipen_runinfo-0.1.0/README.md
--rw-r--r--   0        0        0     6586 2023-06-10 06:31:57.015234 pipen_runinfo-0.1.0/pipen_runinfo.py
--rw-r--r--   0        0        0     1057 2023-06-10 06:31:57.015234 pipen_runinfo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 pipen_runinfo-0.1.0/setup.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 pipen_runinfo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2755 2023-06-10 21:59:57.160728 pipen_runinfo-0.1.1/README.md
+-rw-r--r--   0        0        0     6622 2023-06-10 21:59:57.160728 pipen_runinfo-0.1.1/pipen_runinfo.py
+-rw-r--r--   0        0        0     1057 2023-06-10 21:59:57.160728 pipen_runinfo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 pipen_runinfo-0.1.1/setup.py
+-rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 pipen_runinfo-0.1.1/PKG-INFO
```

### Comparing `pipen_runinfo-0.1.0/README.md` & `pipen_runinfo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pipen_runinfo-0.1.0/pipen_runinfo.py` & `pipen_runinfo-0.1.1/pipen_runinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 from typing import TYPE_CHECKING, List
 from pathlib import Path
 
 from pipen import plugin
 from pipen.job import Job
 
 if TYPE_CHECKING:
     from pipen import Proc, Pipen
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # Monkey-path Job.CMD_WRAPPER_TEMPLATE to time the script
 Job.CMD_WRAPPER_TEMPLATE = Job.CMD_WRAPPER_TEMPLATE.replace(
     "{job.strcmd}",
     "/usr/bin/time -o {job.metadir}/job.runinfo.time -v {job.strcmd}",
 ).replace(
     "{postscript}",
```

### Comparing `pipen_runinfo-0.1.0/pyproject.toml` & `pipen_runinfo-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-runinfo"
-version = "0.1.0"
+version = "0.1.1"
 description = "Generate running information for jobs in pipen pipelines"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pipen_runinfo-0.1.0/setup.py` & `pipen_runinfo-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ['pipen>=0.10.1,<0.11.0']
 
 entry_points = \
 {'pipen': ['runinfo = pipen_runinfo:PipenRuninfoPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-runinfo',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Generate running information for jobs in pipen pipelines',
     'long_description': '# pipen-runinfo\n\nGenerate running information for jobs in [pipen][1] pipelines.\n\nIncluding session info (packages and versions), time, and device info.\n\n## Install\n\n```bash\npip install -U pipen-runinfo\n```\n\n## Enable/Disable the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it: plugins=[..., "no:runinfo"], or uninstall this plugin.\n\n## Plugin options\n\n- `runinfo_lang`: The name of the language to run the job script for session info.\n    Default is `None`, which means it will be inferred from the `proc.lang`\n    This should be a process-level option, unless you only have one single\n    process in your pipeline.\n- `runinfo_path`: Whether to include paths for the modules in the session information.\n    Default is `True`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n- `runinfo_submod`: Whether to include submodules in the session information.\n    Default is `False`.\n    This option could be either specified in the process-level or the pipeline-level.\n    Only works for `python`.\n\n## Supported languages for session info\n\n`python`, `R`, `bash`, and `fish`.\n\n## Usage\n\nThe plugin will generate 3 files in the job directory of the pipeline.\n\n### `job.runinfo.session`\n\nThe session information of the job, including the interpreter, packages and their versions.\n\n#### Python\n\nGenerates a TSV file with the following columns:\n\n- `Name`: The name of the module, or python itself\n- `__version__`: The version fetched by `module.__version__` or `module.version`\n- `importlib.metadata`: The version fetched by `importlib.metadata.version(package)`\n- `Path`: The path of the module (only if `runinfo_path` is `True`)\n\n#### R\n\nGenerates a text file `sessionInfo()` output.\n\n#### Bash\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `BASH_VERSION`: The value of `$BASH_VERSION`\n- `BASH_ARGV0`: The value of `$BASH_ARGV0`\n- `BASH_SOURCE`: The value of `$BASH_SOURCE`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n#### Fish\n\nGenerates a TSV file with the following columns:\n\n- `SHELL`: The value of `$SHELL`\n- `FISH_VERSION`: The value of `$FISH_VERSION`\n- `proc-exe`: The real path of the executable from `/proc/<pid>/exe`\n- `proc-exe-version`: The version of the executable from `/proc/<pid>/exe --version`\n\n### `job.runinfo.time`\n\nThe time spent on the job, and more, generated by `time -v` command.\n\n### `job.runinfo.device`\n\nThe device information of the job, generated by `lshw` command.\nNote that only processor, memory, display and storage are included.\n\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_runinfo-0.1.0/PKG-INFO` & `pipen_runinfo-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-runinfo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate running information for jobs in pipen pipelines
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

