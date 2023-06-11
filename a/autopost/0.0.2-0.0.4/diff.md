# Comparing `tmp/autopost-0.0.2.tar.gz` & `tmp/autopost-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopost-0.0.2.tar", last modified: Wed Dec 14 14:30:02 2022, max compression
+gzip compressed data, was "autopost-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autopost-0.0.2.tar` & `autopost-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1109 2022-12-14 01:42:29.082261 autopost-0.0.2/LICENSE
--rw-r--r--   0        0        0     2163 2022-12-14 01:45:37.337439 autopost-0.0.2/README.md
--rw-r--r--   0        0        0       22 2022-12-14 14:29:25.790006 autopost-0.0.2/autopost/__init__.py
--rw-r--r--   0        0        0      132 2022-11-08 18:42:43.870323 autopost-0.0.2/autopost/_backend/__init__.py
--rw-r--r--   0        0        0      450 2022-12-14 01:27:06.597569 autopost-0.0.2/autopost/_backend/interface.py
--rw-r--r--   0        0        0     1740 2022-12-14 01:27:53.461432 autopost-0.0.2/autopost/_backend/mastodon.py
--rw-r--r--   0        0        0     1398 2022-12-14 01:34:14.516337 autopost-0.0.2/autopost/_backend/reddit.py
--rw-r--r--   0        0        0     1397 2022-12-14 01:28:13.757373 autopost-0.0.2/autopost/_backend/twitter.py
--rw-r--r--   0        0        0     4140 2022-12-14 14:27:26.126884 autopost-0.0.2/autopost/_cli.py
--rw-r--r--   0        0        0     1741 2022-12-14 01:26:23.949695 autopost-0.0.2/autopost/_config.py
--rw-r--r--   0        0        0     1970 2022-12-09 04:19:14.632710 autopost-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 autopost-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-06-11 04:08:00.990919 autopost-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2163 2023-06-11 04:08:00.990919 autopost-0.0.4/README.md
+-rw-r--r--   0        0        0       22 2023-06-11 04:08:00.990919 autopost-0.0.4/autopost/__init__.py
+-rw-r--r--   0        0        0      132 2023-06-11 04:08:00.990919 autopost-0.0.4/autopost/_backend/__init__.py
+-rw-r--r--   0        0        0      450 2023-06-11 04:08:00.990919 autopost-0.0.4/autopost/_backend/interface.py
+-rw-r--r--   0        0        0     1526 2023-06-11 04:08:00.990919 autopost-0.0.4/autopost/_backend/mastodon.py
+-rw-r--r--   0        0        0     1398 2023-06-11 04:08:00.990919 autopost-0.0.4/autopost/_backend/reddit.py
+-rw-r--r--   0        0        0     1397 2023-06-11 04:08:00.990919 autopost-0.0.4/autopost/_backend/twitter.py
+-rw-r--r--   0        0        0     4600 2023-06-11 04:08:00.990919 autopost-0.0.4/autopost/_cli.py
+-rw-r--r--   0        0        0     1736 2023-06-11 04:08:00.990919 autopost-0.0.4/autopost/_config.py
+-rw-r--r--   0        0        0     2044 2023-06-11 04:08:00.990919 autopost-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 autopost-0.0.4/PKG-INFO
```

### Comparing `autopost-0.0.2/LICENSE` & `autopost-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autopost-0.0.2/README.md` & `autopost-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `autopost-0.0.2/autopost/_backend/mastodon.py` & `autopost-0.0.4/autopost/_backend/mastodon.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,19 +34,14 @@
             return Err(f"{self._config.server} failed instance health check")
         except Exception as e:
             return Err(str(e))
 
     def post(self, content: str, url: str, *, tags: list[str] = []) -> Result[Url, str]:
         tags = [f"#{tag}" for tag in tags]
 
-        # If moa_crosspost is set, explicitly add the `#xp` tag to tell
-        # Moa Bridge that we'd like to crosspost this post to Twitter.
-        if self._config.moa_crosspost:
-            tags.append("#xp")
-
         status = dedent(
             f"""
             {content}
 
             {url}
 
             {' '.join(tags)}
```

### Comparing `autopost-0.0.2/autopost/_backend/reddit.py` & `autopost-0.0.4/autopost/_backend/reddit.py`

 * *Files identical despite different names*

### Comparing `autopost-0.0.2/autopost/_backend/twitter.py` & `autopost-0.0.4/autopost/_backend/twitter.py`

 * *Files identical despite different names*

### Comparing `autopost-0.0.2/autopost/_cli.py` & `autopost-0.0.4/autopost/_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import argparse
+import json
 import logging
 import os
 import sys
+import tomllib
+from collections.abc import Iterator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Iterator
 
 import feedparser
-import tomllib
 from result import Err, Ok
 from rich import traceback
 from rich.console import Console
 from rich.logging import RichHandler
 
 from autopost import __version__
 from autopost._config import Config
@@ -45,14 +46,16 @@
     parser.add_argument("--dry-run", action="store_true", help="perform a dry-run")
     parser.add_argument(
         "--config-file",
         type=Path,
         help="the file to load for configuration",
         default=Path(os.getenv("AUTOPOST_CONFIG_FILE", _DEFAULT_CONFIG)),
     )
+    parser.add_argument("--json", action="store_true", help="write output as JSON")
+
     subcommands = parser.add_subparsers(dest="subcommand", required=True)
 
     manual = subcommands.add_parser(
         "manual",
         help="auto-post manually",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
@@ -125,14 +128,25 @@
             if not status:
                 sys.exit(1)
 
         if args.dry_run:
             console.print(f"dry run: would have posted {content} with URL: {url} and tags: {tags}")
             sys.exit(0)
 
+        results = []
         for backend in backends:
-            res = backend.post(content, url, tags=tags)
-            match res:
+            status = backend.post(content, url, tags=tags)
+            result = {
+                "backend": backend.__class__.__name__,
+                "name": backend.name,
+            }
+            match status:
                 case Ok(link):
                     console.print(f":tada: {backend.name}: {link}")
+                    result["link"] = str(link)
                 case Err(msg):
                     console.print(f":skull: {backend.name}: {msg}")
+                    result["failure"] = msg
+            results.append(result)
+
+    if args.json:
+        print(json.dumps(results), file=sys.stdout)
```

### Comparing `autopost-0.0.2/autopost/_config.py` & `autopost-0.0.4/autopost/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
-from typing import Annotated, Iterator, Literal
+from collections.abc import Iterator
+from typing import Annotated, Literal
 
 from pydantic import BaseModel, Field, SecretStr, StrictStr
 
 from autopost._backend.interface import Backend
 
 
 class Embedded(BaseModel):
@@ -47,15 +48,14 @@
 class MastodonConfig(BaseModel):
     type_: Literal["Mastodon"] = Field(alias="type")
     name: str
     server: str
     client_secret: Credential
     client_key: Credential
     access_token: Credential
-    moa_crosspost: bool = False
 
 
 BackendConfig = Annotated[
     RedditConfig | TwitterConfig | MastodonConfig, Field(discriminator="type_")
 ]
```

### Comparing `autopost-0.0.2/pyproject.toml` & `autopost-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -4,93 +4,81 @@
 
 [project]
 name = "autopost"
 dynamic = ["version"]
 description = "Auto-posts social media updates"
 readme = "README.md"
 license = { file = "LICENSE" }
-authors = [
-  { name = "William Woodruff", email = "william@yossarian.net" }
-]
+authors = [{ name = "William Woodruff", email = "william@yossarian.net" }]
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Topic :: Security",
 ]
 dependencies = [
   "feedparser ~= 6.0",
-  "praw ~= 7.6.1",
-  "Mastodon.py ~= 1.7.0",
+  "praw >= 7.6.1,< 7.8.0",
+  "Mastodon.py >= 1.7,< 1.9",
   "pydantic ~= 1.10",
   "python-frontmatter ~= 1.0",
   "result ~= 0.8",
-  "rich >= 12.5.1,< 12.7.0",
+  "rich >= 12.5.1,< 13.5.0",
   "python-twitter ~= 3.5",
 ]
 requires-python = ">=3.11"
 
 [project.urls]
 Homepage = "https://pypi.org/project/autopost/"
 Issues = "https://github.com/woodruffw/autopost/issues"
 Source = "https://github.com/woodruffw/autopost"
 
 [project.scripts]
 autopost = "autopost._cli:main"
 
 [project.optional-dependencies]
-test = [
-  "pytest",
-  "pytest-cov",
-  "pretend",
-]
-lint = [
-  "bandit",
-  "flake8",
-  "black",
-  "isort",
-  "interrogate",
-  "mypy",
-]
-dev = [
-  "build",
-  "autopost[test,lint]",
-]
+test = ["pytest", "pytest-cov", "pretend"]
+lint = ["bandit", "black", "interrogate", "mypy", "ruff"]
+dev = ["build", "autopost[test,lint]"]
 
 [tool.isort]
 multi_line_output = 3
 known_first_party = "autopost"
 include_trailing_comma = true
 
 [tool.interrogate]
 exclude = ["env", "test", "codegen"]
 ignore-semiprivate = true
 fail-under = 100
 
 [tool.mypy]
-plugins = [
-  "pydantic.mypy"
-]
+plugins = ["pydantic.mypy"]
 
 allow_redefinition = true
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 ignore_missing_imports = true
 no_implicit_optional = true
 show_error_codes = true
+sqlite_cache = true
 strict_equality = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.bandit]
 exclude_dirs = ["./test"]
 
 [tool.black]
 line-length = 100
+
+[tool.ruff]
+line-length = 100
+select = ["E", "F", "I", "W", "UP"]
+target-version = "py311"
```

### Comparing `autopost-0.0.2/PKG-INFO` & `autopost-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: autopost
-Version: 0.0.2
+Version: 0.0.4
 Summary: Auto-posts social media updates
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Requires-Dist: feedparser ~= 6.0
-Requires-Dist: praw ~= 7.6.1
-Requires-Dist: Mastodon.py ~= 1.7.0
+Requires-Dist: praw >= 7.6.1,< 7.8.0
+Requires-Dist: Mastodon.py >= 1.7,< 1.9
 Requires-Dist: pydantic ~= 1.10
 Requires-Dist: python-frontmatter ~= 1.0
 Requires-Dist: result ~= 0.8
-Requires-Dist: rich >= 12.5.1,< 12.7.0
+Requires-Dist: rich >= 12.5.1,< 13.5.0
 Requires-Dist: python-twitter ~= 3.5
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: autopost[test,lint] ; extra == "dev"
 Requires-Dist: bandit ; extra == "lint"
-Requires-Dist: flake8 ; extra == "lint"
 Requires-Dist: black ; extra == "lint"
-Requires-Dist: isort ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
+Requires-Dist: ruff ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
 Project-URL: Homepage, https://pypi.org/project/autopost/
 Project-URL: Issues, https://github.com/woodruffw/autopost/issues
 Project-URL: Source, https://github.com/woodruffw/autopost
 Provides-Extra: dev
```

