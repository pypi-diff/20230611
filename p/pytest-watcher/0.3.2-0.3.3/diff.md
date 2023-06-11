# Comparing `tmp/pytest_watcher-0.3.2.tar.gz` & `tmp/pytest_watcher-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_watcher-0.3.2.tar", max compression
+gzip compressed data, was "pytest_watcher-0.3.3.tar", max compression
```

## Comparing `pytest_watcher-0.3.2.tar` & `pytest_watcher-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/LICENSE
--rw-r--r--   0        0        0     3330 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/README.md
--rw-r--r--   0        0        0     1563 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       76 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/pytest_watcher/__init__.py
--rw-r--r--   0        0        0       81 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/pytest_watcher/__main__.py
--rw-r--r--   0        0        0     5163 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/pytest_watcher/watcher.py
--rw-r--r--   0        0        0     4429 1970-01-01 00:00:00.000000 pytest_watcher-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4434 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/README.md
+-rw-r--r--   0        0        0     1590 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/__main__.py
+-rw-r--r--   0        0        0     2393 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/config.py
+-rw-r--r--   0        0        0       56 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/constants.py
+-rw-r--r--   0        0        0     4885 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/watcher.py
+-rw-r--r--   0        0        0     5533 1970-01-01 00:00:00.000000 pytest_watcher-0.3.3/PKG-INFO
```

### Comparing `pytest_watcher-0.3.2/LICENSE` & `pytest_watcher-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_watcher-0.3.2/README.md` & `pytest_watcher-0.3.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,52 @@
-# A simple watcher for pytest
+# Welcome to pytest-watcher
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-watcher)](https://pypi.org/project/pytest-watcher/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-watcher)](https://pypi.org/project/pytest-watcher/)
 [![GitHub](https://img.shields.io/github/license/olzhasar/pytest-watcher)](https://github.com/olzhasar/pytest-watcher/blob/master/LICENSE)
 
 ## Overview
 
 **pytest-watcher** is a tool to automatically rerun tests (using `pytest` by default) whenever your code changes.
 
 Works on Unix (Linux, MacOS, BSD) and Windows.
 
-## Table of Contents
+Example:
+
+![Preview](preview.gif)
+
+## Table of contents
 
 - [Motivation](#motivation)
 - [File Events](#file-events)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Using a different test runner](#using-a-different-test-runner)
 - [Watching different patterns](#watching-different-patterns)
 - [Delay](#delay)
+- [Configuring](#configuring)
+- [Differences with pytest-watch](#differences-with-pytest-watch)
 - [Compatibility](#compatibility)
 - [License](#license)
 
 ## Motivation
 
-### Why not general tools (e.g. `watchmedo`, `entr`)?
+### Why not general tools
 
 - Easy to use and remember
 - Works for most python projects out of the box
-- Minimum dependencies (`watchdog` is the only one)
-- Handles post-processing properly (see [delay](#delay))
+- Uses native system monitoring API instead of polling on supported systems (see [watchdog documentation](https://python-watchdog.readthedocs.io/en/stable/installation.html#supported-platforms-and-caveats))
+- Listens for new file, delete file, change and move events
+- Runs your tests with latest changes in case of post-processing events (see [delay](#delay))
+
+### What about pytest-watch
 
-### What about pytest-watch?
+[pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and doesn't work for many users. This project provides an alternative for it.
 
-[pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and does not work for many users. To provide a substitute, I developed this tool.
+See also: [Differences with pytest-watch](#differences-with-pytest-watch)
 
 ## File events
 
 By default `pytest-watcher` looks for the following events:
 
 - New `*.py` file created
 - Existing `*.py` file modified
@@ -50,74 +59,100 @@
 
 ```sh
 pip install pytest-watcher
 ```
 
 ## Usage
 
-Specify the path that you want to monitor:
+Specify the path that you want to watch:
 
 ```sh
 ptw .
 ```
 
 or
 
 ```sh
 ptw /home/repos/project
 ```
 
-Any arguments after `<path>` will be passed to the test runner (which is `pytest` by default). For example:
+`pytest-watcher` will pass any arguments after `<path>` to the test runner (which is `pytest` by default). For example:
 
 ```sh
 ptw . -x --lf --nf
 ```
 
 will call `pytest` with the following arguments:
 
 ```sh
 pytest -x --lf --nf
 ```
 
-## Using a different test runner
+### Using a different test runner
 
 You can specify an alternative test runner using the `--runner` flag:
 
 ```sh
 ptw . --runner tox
 ```
 
-## Watching different patterns
+### Watching different patterns
 
-You can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a comma. The default value is "\*.py".
+You can use the `--patterns` flag to specify file patterns that you want to watch. It accepts a list of Unix-style patterns separated by a comma. The default value is "\*.py"
 
 Example:
 
 ```sh
 ptw . --patterns '*.py,pyproject.toml'
 ```
 
 You can also **ignore** certain patterns using the `--ignore-patterns` flag:
 
 ```sh
 ptw . --ignore-patterns 'settings.py,db.py'
 ```
 
-## Delay
+### Delay
 
-`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., `black` plugin in your IDE). This ensures that tests will be run with the latest version of your code.
+`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (for example, `black` plugin in your IDE). This ensures that tests will run with the latest version of your code.
 
 You can control the actual delay value with the `--delay` flag:
 
 `ptw . --delay 0.2`
 
-To disable the delay altogether, you can provide zero as a value:
+To disable the delay altogether, you can set zero as a value:
 
 `ptw . --delay 0`
 
+### Differences with `pytest-watch`
+
+Even though this project was inspired by [`pytest-watch`](https://github.com/joeyespo/pytest-watch), it's not a fork of it. Therefore, there are **differences** in behavior:
+
+- `pytest-watch` needs you to specify a path to watch as a first argument:
+
+```
+ptw .
+```
+
+- `pytest-watch` doesn't start tests immediately by default. You can customize this behavior using `--now` flag.
+
+## Configuring
+
+You can configure `pytest-watcher` via `pyproject.toml` file. Here is the default configuration:
+
+```toml
+[tool.pytest-watcher]
+now = false
+delay = 0.2
+runner = "pytest"
+runner_args = []
+patterns = ["*.py"]
+ignore_patterns = []
+```
+
 ## Compatibility
 
-The code is tested for Python versions 3.7+
+The code is compatible with Python versions 3.7+
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `pytest_watcher-0.3.2/pyproject.toml` & `pytest_watcher-0.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-watcher"
-version = "0.3.2"
+version = "0.3.3"
 description = "Automatically rerun your tests on file modifications"
 authors = ["Olzhas Arystanov <o.arystanov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/olzhasar/pytest-watcher"
 repository = "https://github.com/olzhasar/pytest-watcher"
 keywords = ["pytest", "watch", "watcher"]
@@ -27,16 +27,16 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4.0.0"
 watchdog = ">=2.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
-flake8 = "*"
 black = "*"
+ruff = "*"
 mypy = "*"
 isort = "*"
 pytest-mock = "*"
 freezegun = "*"
 tox = "*"
 coverage = {extras = ["toml"], version = "*"}
 
@@ -66,11 +66,14 @@
     | \.venv
     | _build
     | buck-out
     | build
     )
 '''
 
+[tool.ruff]
+line-length = 89
+
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.7"
 ignore_missing_imports = true
 exclude = ".venv"
```

### Comparing `pytest_watcher-0.3.2/pytest_watcher/watcher.py` & `pytest_watcher-0.3.3/pytest_watcher/watcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,32 @@
 import argparse
 import logging
 import subprocess
 import sys
 import threading
 import time
-from dataclasses import dataclass
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import List, Optional, Sequence
+from typing import List, Optional, Sequence, Tuple
 
 from watchdog import events
 from watchdog.observers import Observer
 from watchdog.utils.patterns import match_any_paths
 
-VERSION = "0.3.2"
-DEFAULT_DELAY = 0.2
-LOOP_DELAY = 0.1
+from .config import Config
+from .constants import DEFAULT_DELAY, LOOP_DELAY, VERSION
 
 trigger_lock = threading.Lock()
 trigger = None
 
 
 logging.basicConfig(level=logging.INFO, format="[ptw] %(message)s")
 logger = logging.getLogger(__name__)
 
 
-@dataclass
-class ParsedArguments:
-    path: Path
-    now: bool
-    delay: float
-    runner: str
-    patterns: str
-    ignore_patterns: str
-    runner_args: Sequence[str]
-
-
 def emit_trigger():
     """
     Emits trigger to run pytest
     """
 
     global trigger
 
@@ -90,15 +77,15 @@
             logger.debug(f"IGNORED event: {event.event_type} src: {event.src_path}")
 
 
 def _invoke_runner(runner: str, args: Sequence[str]) -> None:
     subprocess.run([runner, *args])
 
 
-def parse_arguments(args: Sequence[str]) -> ParsedArguments:
+def parse_arguments(args: Sequence[str]) -> Tuple[argparse.Namespace, List[str]]:
     def _parse_patterns(arg: str):
         return arg.split(",")
 
     parser = argparse.ArgumentParser(
         prog="pytest_watcher",
         description="""
             Watch the <path> for file changes and trigger the test runner (pytest).\n
@@ -108,48 +95,41 @@
     parser.add_argument("path", type=Path, help="The path to watch for file changes.")
     parser.add_argument(
         "--now", action="store_true", help="Trigger the test run immediately"
     )
     parser.add_argument(
         "--delay",
         type=float,
-        default=DEFAULT_DELAY,
-        help=f"The delay (in seconds) before triggering the test run (default: {DEFAULT_DELAY})",
+        required=False,
+        help="The delay (in seconds) before triggering"
+        f"the test run (default: {DEFAULT_DELAY})",
     )
     parser.add_argument(
         "--runner",
         type=str,
-        default="pytest",
+        required=False,
         help="Specify the executable for running the tests (default: pytest)",
     )
     parser.add_argument(
         "--patterns",
-        default=["*.py"],
         type=_parse_patterns,
-        help="File patterns to watch, specified as comma-separated Unix-style patterns (default: '*.py')",
+        required=False,
+        help="File patterns to watch, specified as comma-separated"
+        "Unix-style patterns (default: '*.py')",
     )
     parser.add_argument(
         "--ignore-patterns",
-        default=[],
         type=_parse_patterns,
-        help="File patterns to ignore, specified as comma-separated Unix-style patterns (default: '')",
+        required=False,
+        help="File patterns to ignore, specified as comma-separated"
+        "Unix-style patterns (default: '')",
     )
     parser.add_argument("--version", action="version", version=VERSION)
 
-    namespace, runner_args = parser.parse_known_args(args)
-
-    return ParsedArguments(
-        path=namespace.path,
-        now=namespace.now,
-        delay=namespace.delay,
-        runner=namespace.runner,
-        patterns=namespace.patterns,
-        ignore_patterns=namespace.ignore_patterns,
-        runner_args=runner_args,
-    )
+    return parser.parse_known_args(args)
 
 
 def main_loop(*, runner: str, runner_args: Sequence[str], delay: float) -> None:
     global trigger
 
     now = datetime.now()
     if trigger and now - trigger > timedelta(seconds=delay):
@@ -158,31 +138,35 @@
         with trigger_lock:
             trigger = None
 
     time.sleep(LOOP_DELAY)
 
 
 def run():
-    args = parse_arguments(sys.argv[1:])
+    namespace, runner_args = parse_arguments(sys.argv[1:])
+
+    config = Config.create(namespace=namespace, extra_args=runner_args)
 
     event_handler = EventHandler(
-        patterns=args.patterns, ignore_patterns=args.ignore_patterns
+        patterns=config.patterns, ignore_patterns=config.ignore_patterns
     )
 
     observer = Observer()
 
-    observer.schedule(event_handler, args.path, recursive=True)
+    observer.schedule(event_handler, config.path, recursive=True)
     observer.start()
 
     sys.stdout.write(f"pytest-watcher version {VERSION}\n")
-    sys.stdout.write(f"Runner command: {args.runner} {' '.join(args.runner_args)}\n")
-    sys.stdout.write(f"Waiting for file changes in {args.path.absolute()}\n")
+    sys.stdout.write(f"Runner command: {config.runner} {' '.join(config.runner_args)}\n")
+    sys.stdout.write(f"Waiting for file changes in {config.path.absolute()}\n")
 
-    if args.now:
+    if config.now:
         emit_trigger()
 
     try:
         while True:
-            main_loop(runner=args.runner, runner_args=args.runner_args, delay=args.delay)
+            main_loop(
+                runner=config.runner, runner_args=config.runner_args, delay=config.delay
+            )
     finally:
         observer.stop()
         observer.join()
```

### Comparing `pytest_watcher-0.3.2/PKG-INFO` & `pytest_watcher-0.3.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-watcher
-Version: 0.3.2
+Version: 0.3.3
 Summary: Automatically rerun your tests on file modifications
 Home-page: https://github.com/olzhasar/pytest-watcher
 License: MIT
 Keywords: pytest,watch,watcher
 Author: Olzhas Arystanov
 Author-email: o.arystanov@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -22,50 +22,59 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: watchdog (>=2.0.0)
 Project-URL: Repository, https://github.com/olzhasar/pytest-watcher
 Description-Content-Type: text/markdown
 
-# A simple watcher for pytest
+# Welcome to pytest-watcher
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-watcher)](https://pypi.org/project/pytest-watcher/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-watcher)](https://pypi.org/project/pytest-watcher/)
 [![GitHub](https://img.shields.io/github/license/olzhasar/pytest-watcher)](https://github.com/olzhasar/pytest-watcher/blob/master/LICENSE)
 
 ## Overview
 
 **pytest-watcher** is a tool to automatically rerun tests (using `pytest` by default) whenever your code changes.
 
 Works on Unix (Linux, MacOS, BSD) and Windows.
 
-## Table of Contents
+Example:
+
+![Preview](preview.gif)
+
+## Table of contents
 
 - [Motivation](#motivation)
 - [File Events](#file-events)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Using a different test runner](#using-a-different-test-runner)
 - [Watching different patterns](#watching-different-patterns)
 - [Delay](#delay)
+- [Configuring](#configuring)
+- [Differences with pytest-watch](#differences-with-pytest-watch)
 - [Compatibility](#compatibility)
 - [License](#license)
 
 ## Motivation
 
-### Why not general tools (e.g. `watchmedo`, `entr`)?
+### Why not general tools
 
 - Easy to use and remember
 - Works for most python projects out of the box
-- Minimum dependencies (`watchdog` is the only one)
-- Handles post-processing properly (see [delay](#delay))
+- Uses native system monitoring API instead of polling on supported systems (see [watchdog documentation](https://python-watchdog.readthedocs.io/en/stable/installation.html#supported-platforms-and-caveats))
+- Listens for new file, delete file, change and move events
+- Runs your tests with latest changes in case of post-processing events (see [delay](#delay))
+
+### What about pytest-watch
 
-### What about pytest-watch?
+[pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and doesn't work for many users. This project provides an alternative for it.
 
-[pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and does not work for many users. To provide a substitute, I developed this tool.
+See also: [Differences with pytest-watch](#differences-with-pytest-watch)
 
 ## File events
 
 By default `pytest-watcher` looks for the following events:
 
 - New `*.py` file created
 - Existing `*.py` file modified
@@ -78,75 +87,101 @@
 
 ```sh
 pip install pytest-watcher
 ```
 
 ## Usage
 
-Specify the path that you want to monitor:
+Specify the path that you want to watch:
 
 ```sh
 ptw .
 ```
 
 or
 
 ```sh
 ptw /home/repos/project
 ```
 
-Any arguments after `<path>` will be passed to the test runner (which is `pytest` by default). For example:
+`pytest-watcher` will pass any arguments after `<path>` to the test runner (which is `pytest` by default). For example:
 
 ```sh
 ptw . -x --lf --nf
 ```
 
 will call `pytest` with the following arguments:
 
 ```sh
 pytest -x --lf --nf
 ```
 
-## Using a different test runner
+### Using a different test runner
 
 You can specify an alternative test runner using the `--runner` flag:
 
 ```sh
 ptw . --runner tox
 ```
 
-## Watching different patterns
+### Watching different patterns
 
-You can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a comma. The default value is "\*.py".
+You can use the `--patterns` flag to specify file patterns that you want to watch. It accepts a list of Unix-style patterns separated by a comma. The default value is "\*.py"
 
 Example:
 
 ```sh
 ptw . --patterns '*.py,pyproject.toml'
 ```
 
 You can also **ignore** certain patterns using the `--ignore-patterns` flag:
 
 ```sh
 ptw . --ignore-patterns 'settings.py,db.py'
 ```
 
-## Delay
+### Delay
 
-`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., `black` plugin in your IDE). This ensures that tests will be run with the latest version of your code.
+`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (for example, `black` plugin in your IDE). This ensures that tests will run with the latest version of your code.
 
 You can control the actual delay value with the `--delay` flag:
 
 `ptw . --delay 0.2`
 
-To disable the delay altogether, you can provide zero as a value:
+To disable the delay altogether, you can set zero as a value:
 
 `ptw . --delay 0`
 
+### Differences with `pytest-watch`
+
+Even though this project was inspired by [`pytest-watch`](https://github.com/joeyespo/pytest-watch), it's not a fork of it. Therefore, there are **differences** in behavior:
+
+- `pytest-watch` needs you to specify a path to watch as a first argument:
+
+```
+ptw .
+```
+
+- `pytest-watch` doesn't start tests immediately by default. You can customize this behavior using `--now` flag.
+
+## Configuring
+
+You can configure `pytest-watcher` via `pyproject.toml` file. Here is the default configuration:
+
+```toml
+[tool.pytest-watcher]
+now = false
+delay = 0.2
+runner = "pytest"
+runner_args = []
+patterns = ["*.py"]
+ignore_patterns = []
+```
+
 ## Compatibility
 
-The code is tested for Python versions 3.7+
+The code is compatible with Python versions 3.7+
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

