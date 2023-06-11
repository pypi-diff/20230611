# Comparing `tmp/tox_gh-1.1.0.tar.gz` & `tmp/tox_gh-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox_gh-1.1.0.tar", last modified: Sun Jun 11 14:28:04 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `tox_gh-1.1.0.tar` & `tox_gh-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.723596 tox_gh-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.719596 tox_gh-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.719596 tox_gh-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-11 14:27:57.000000 tox_gh-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 14:27:57.000000 tox_gh-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-11 14:27:57.000000 tox_gh-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-11 14:28:04.723596 tox_gh-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-11 14:27:57.000000 tox_gh-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-11 14:27:57.000000 tox_gh-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-11 14:28:04.723596 tox_gh-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-11 14:27:57.000000 tox_gh-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.719596 tox_gh-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.719596 tox_gh-1.1.0/src/tox_gh/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-11 14:27:57.000000 tox_gh-1.1.0/src/tox_gh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-11 14:27:57.000000 tox_gh-1.1.0/src/tox_gh/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 14:27:57.000000 tox_gh-1.1.0/src/tox_gh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.723596 tox_gh-1.1.0/src/tox_gh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:28:04.000000 tox_gh-1.1.0/src/tox_gh.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:28:04.723596 tox_gh-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-11 14:27:57.000000 tox_gh-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-11 14:27:57.000000 tox_gh-1.1.0/tests/test_tox_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-11 14:27:57.000000 tox_gh-1.1.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-11 14:27:57.000000 tox_gh-1.1.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 14:27:57.000000 tox_gh-1.1.0/whitelist.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox_gh-1.2.0/src/tox_gh/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 tox_gh-1.2.0/src/tox_gh/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_gh-1.2.0/src/tox_gh/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox_gh-1.2.0/src/tox_gh/version.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tox_gh-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 tox_gh-1.2.0/tests/test_tox_gh.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tox_gh-1.2.0/tests/test_version.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_gh-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_gh-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 tox_gh-1.2.0/README.md
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 tox_gh-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tox_gh-1.2.0/PKG-INFO
```

### Comparing `tox_gh-1.1.0/LICENSE` & `tox_gh-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox_gh-1.1.0/PKG-INFO` & `tox_gh-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
-Name: tox_gh
-Version: 1.1.0
-Summary: Seamless integration of tox into GitHub Actions
-Home-page: https://github.com/tox-dev/tox-gh
-Author: Bernat Gabor
-Author-email: gaborjbernatv@gmail.com
-Maintainer: Bernat Gabor
-Maintainer-email: gaborjbernat@gmail.com
-License: MIT
+Name: tox-gh
+Version: 1.2.0
+Summary: Seamless integration of tox into GitHub Actions.
+Project-URL: Documentation, https://github.com/tox-dev/tox-gh#tox-gh
+Project-URL: Homepage, https://github.com/tox-dev/tox-gh
 Project-URL: Source, https://github.com/tox-dev/tox-gh
 Project-URL: Tracker, https://github.com/tox-dev/tox-gh/issues
-Project-URL: Changelog, https://github.com/tox-dev/tox-gh/blob/main/CHANGELOG.md
-Keywords: virtual,environments,isolated,testing
-Platform: any
+Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: environments,isolated,testing,virtual
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Framework :: Sphinx
-Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Documentation
-Classifier: Topic :: Documentation :: Sphinx
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: tox>=4.6
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: covdefaults>=2.3; extra == 'test'
+Requires-Dist: devpi-process>=0.3; extra == 'test'
+Requires-Dist: pytest-cov>=4.1; extra == 'test'
+Requires-Dist: pytest-mock>=3.10; extra == 'test'
+Requires-Dist: pytest>=7.3.2; extra == 'test'
+Description-Content-Type: text/markdown
 
 # tox-gh
 
 [![PyPI version](https://badge.fury.io/py/tox-gh.svg)](https://badge.fury.io/py/tox-gh)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/tox-gh.svg)](https://pypi.python.org/pypi/tox-gh/)
 [![check](https://github.com/tox-dev/tox-gh/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/tox-gh/actions/workflows/check.yml)
 
@@ -57,26 +62,30 @@
 ### Basic Example
 
 Add `[gh]` section to the same file as tox configuration. If you're using `tox.ini`:
 
 ```ini
 [gh]
 python =
-    3.6 = py36
-    3.7 = py37
+    3.12 = py312
+    3.11 = py311, type
+    3.10 = py310
+    3.9 = py39
     3.8 = py38
-    3.9 = py39, type
+    3.7 = py37
 ```
 
 This will run different set of tox environments on different python versions set up via GitHub `setup-python` action:
 
-- on Python 3.6 job, tox runs `py36` environment,
 - on Python 3.7 job, tox runs `py37` environment,
 - on Python 3.8 job, tox runs `py38` environment,
-- in Python 3.9 job, tox runs `py39` and `type` environments.
+- on Python 3.9 job, tox runs `py39` environment,
+- on Python 3.10 job, tox runs `py310` environment,
+- in Python 3.11 job, tox runs `py311` and `type` environments,
+- on Python 3.12 job, tox runs `py312` environment.
 
 #### Workflow Configuration
 
 `.github/workflows/check.yml`:
 
 ```yaml
 name: check
@@ -94,19 +103,20 @@
       fail-fast: false
       matrix:
         os:
           - Ubuntu
           - Windows
           - MacOs
         py:
+          - "3.12"
+          - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
-          - "3.6"
     steps:
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.py }}
       - uses: actions/checkout@v2
       - name: Install tox-gh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tox_gh-1.1.0/README.md` & `tox_gh-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -25,26 +25,30 @@
 ### Basic Example
 
 Add `[gh]` section to the same file as tox configuration. If you're using `tox.ini`:
 
 ```ini
 [gh]
 python =
-    3.6 = py36
-    3.7 = py37
+    3.12 = py312
+    3.11 = py311, type
+    3.10 = py310
+    3.9 = py39
     3.8 = py38
-    3.9 = py39, type
+    3.7 = py37
 ```
 
 This will run different set of tox environments on different python versions set up via GitHub `setup-python` action:
 
-- on Python 3.6 job, tox runs `py36` environment,
 - on Python 3.7 job, tox runs `py37` environment,
 - on Python 3.8 job, tox runs `py38` environment,
-- in Python 3.9 job, tox runs `py39` and `type` environments.
+- on Python 3.9 job, tox runs `py39` environment,
+- on Python 3.10 job, tox runs `py310` environment,
+- in Python 3.11 job, tox runs `py311` and `type` environments,
+- on Python 3.12 job, tox runs `py312` environment.
 
 #### Workflow Configuration
 
 `.github/workflows/check.yml`:
 
 ```yaml
 name: check
@@ -62,19 +66,20 @@
       fail-fast: false
       matrix:
         os:
           - Ubuntu
           - Windows
           - MacOs
         py:
+          - "3.12"
+          - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
-          - "3.6"
     steps:
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.py }}
       - uses: actions/checkout@v2
       - name: Install tox-gh
```

### Comparing `tox_gh-1.1.0/src/tox_gh/plugin.py` & `tox_gh-1.2.0/src/tox_gh/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,68 @@
+"""GitHub Actions integration."""
 from __future__ import annotations
 
 import logging
 import os
 import pathlib
 import shutil
 import sys
-from typing import Dict
+from typing import TYPE_CHECKING, Dict
 
 from tox.config.loader.memory import MemoryLoader
 from tox.config.loader.section import Section
 from tox.config.sets import ConfigSet
 from tox.config.types import EnvList
 from tox.execute import Outcome
 from tox.plugin import impl
-from tox.session.state import State
-from tox.tox_env.api import ToxEnv
-from virtualenv.discovery.py_info import PythonInfo  # type: ignore # no types defined
+from virtualenv.discovery.py_info import PythonInfo  # type: ignore[import] # no types defined
+
+if TYPE_CHECKING:
+    from tox.session.state import State
+    from tox.tox_env.api import ToxEnv
 
 GITHUB_STEP_SUMMARY = os.getenv("GITHUB_STEP_SUMMARY")
 
 
 def is_running_on_actions() -> bool:
-    """:return: True if running on Github Actions platform"""
+    """:return: True if running on GitHub Actions platform"""
     # https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables
     return os.environ.get("GITHUB_ACTIONS") == "true"
 
 
 def get_python_version_keys() -> list[str]:
     """:return: python spec for the python interpreter"""
     python_exe = shutil.which("python") or sys.executable
     info = PythonInfo.from_exe(exe=python_exe)
     major_version = str(info.version_info[0])
     major_minor_version = ".".join([str(i) for i in info.version_info[:2]])
-    if "PyPy" == info.implementation:
+    if info.implementation == "PyPy":
         return [f"pypy-{major_minor_version}", f"pypy-{major_version}", f"pypy{major_version}"]
-    elif hasattr(sys, "pyston_version_info"):  # Pyston
+    if hasattr(sys, "pyston_version_info"):  # Pyston
         return [f"piston-{major_minor_version}", f"pyston-{major_version}"]
-    else:  # Assume this is running on CPython
-        return [major_minor_version, major_version]
+    # Assume this is running on CPython
+    return [major_minor_version, major_version]
 
 
 class GhActionsConfigSet(ConfigSet):
+    """GitHub Actions config set."""
+
     def register_config(self) -> None:
+        """Register the configurations."""
         self.add_config("python", of_type=Dict[str, EnvList], default={}, desc="python version to mapping")
 
 
 @impl
 def tox_add_core_config(core_conf: ConfigSet, state: State) -> None:
+    """
+    Add core configuration flags.
+
+    :param core_conf: the core configuration
+    :param state: tox state object
+    """
     core_conf.add_constant(keys="is_on_gh_action", desc="flag for running on Github", value=is_running_on_actions())
 
     bail_reason = None
     if not core_conf["is_on_gh_action"]:
         bail_reason = "tox is not running in GitHub Actions"
     elif getattr(state.conf.options.env, "is_default_list", False) is False:
         bail_reason = f"envlist is explicitly given via {'TOXENV'if os.environ.get('TOXENV') else '-e flag'}"
@@ -66,26 +78,39 @@
     if env_list is not None:  # override the env_list core configuration with our values
         logging.warning("tox-gh set %s", ", ".join(env_list))
         state.conf.core.loaders.insert(0, MemoryLoader(env_list=env_list))
 
 
 @impl
 def tox_before_run_commands(tox_env: ToxEnv) -> None:
+    """
+    Run logic before tox run commands.
+
+    :param tox_env: the tox environment
+    """
     if tox_env.core["is_on_gh_action"]:
-        print(f"::group::tox:{tox_env.name}")
+        print(f"::group::tox:{tox_env.name}")  # noqa: T201
 
 
 @impl
-def tox_after_run_commands(tox_env: ToxEnv, exit_code: int, outcomes: list[Outcome]) -> None:  # noqa: U100
+def tox_after_run_commands(tox_env: ToxEnv, exit_code: int, outcomes: list[Outcome]) -> None:  # noqa: ARG001
+    """
+    Run logic before after run commands.
+
+
+    :param tox_env: the tox environment
+    :param exit_code: command exit code
+    :param outcomes: list of outcomes
+    """
     if tox_env.core["is_on_gh_action"]:
-        print("::endgroup::")
+        print("::endgroup::")  # noqa: T201
         write_to_summary(exit_code == Outcome.OK, tox_env.name)
 
 
-def write_to_summary(success: bool, message: str) -> None:
-    """Write a success or failure value to the github step summary if it exists"""
+def write_to_summary(success: bool, message: str) -> None:  # noqa: FBT001
+    """Write a success or failure value to the GitHub step summary if it exists."""
     if not GITHUB_STEP_SUMMARY:
         return
     summary_path = pathlib.Path(GITHUB_STEP_SUMMARY)
     success_str = ":white_check_mark:" if success else ":negative_squared_cross_mark:"
     with summary_path.open("a+") as summary_file:
         print(f"{success_str}: {message}", file=summary_file)
```

### Comparing `tox_gh-1.1.0/tests/test_tox_gh.py` & `tox_gh-1.2.0/tests/test_tox_gh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
-import pathlib
 import sys
+from typing import TYPE_CHECKING
 from unittest.mock import ANY
 
-from tox.pytest import MonkeyPatch, ToxProjectCreator
-
 from tox_gh import plugin
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import MonkeyPatch, ToxProjectCreator
+
 
 def test_gh_not_in_actions(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator) -> None:
     monkeypatch.delenv("GITHUB_ACTIONS", raising=False)
     project = tox_project({"tox.ini": "[testenv]\npackage=skip"})
     result = project.run()
     result.assert_success()
     assert "ROOT: tox-gh won't override envlist because tox is not running in GitHub Actions" in result.out
@@ -31,15 +34,15 @@
     monkeypatch.setenv("TOXENV", "py")
     project = tox_project({"tox.ini": "[testenv]\npackage=skip"})
     result = project.run()
     result.assert_success()
     assert "tox-gh won't override envlist because envlist is explicitly given via TOXENV" in result.out
 
 
-def test_gh_ok(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator, tmp_path: pathlib.Path) -> None:
+def test_gh_ok(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator, tmp_path: Path) -> None:
     step_output_file = tmp_path / "gh_out"
     step_output_file.touch()
     monkeypatch.setenv("GITHUB_ACTIONS", "true")
     monkeypatch.delenv("TOXENV", raising=False)
     monkeypatch.setattr(plugin, "GITHUB_STEP_SUMMARY", str(step_output_file))
     ini = f"""
     [testenv]
@@ -73,15 +76,15 @@
     assert "b: OK" in result.out
 
     summary_text = step_output_file.read_text()
     assert ":white_check_mark:: a" in summary_text
     assert ":white_check_mark:: b" in summary_text
 
 
-def test_gh_fail(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator, tmp_path: pathlib.Path) -> None:
+def test_gh_fail(monkeypatch: MonkeyPatch, tox_project: ToxProjectCreator, tmp_path: Path) -> None:
     step_output_file = tmp_path / "gh_out"
     step_output_file.touch()
     monkeypatch.setenv("GITHUB_ACTIONS", "true")
     monkeypatch.delenv("TOXENV", raising=False)
     monkeypatch.setattr(plugin, "GITHUB_STEP_SUMMARY", str(step_output_file))
     ini = f"""
     [testenv]
```

