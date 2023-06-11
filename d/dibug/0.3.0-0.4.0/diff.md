# Comparing `tmp/dibug-0.3.0.tar.gz` & `tmp/dibug-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dibug-0.3.0.tar", max compression
+gzip compressed data, was "dibug-0.4.0.tar", max compression
```

## Comparing `dibug-0.3.0.tar` & `dibug-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1076 2023-06-04 09:00:55.995692 dibug-0.3.0/LICENSE
--rw-r--r--   0        0        0     1190 2023-06-04 09:00:55.995692 dibug-0.3.0/README.md
--rw-r--r--   0        0        0       66 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/__init__.py
--rw-r--r--   0        0        0       62 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/abc/__init__.py
--rw-r--r--   0        0        0      283 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/abc/command.py
--rw-r--r--   0        0        0      150 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/commands/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/commands/eval.py
--rw-r--r--   0        0        0     1682 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/commands/info.py
--rw-r--r--   0        0        0     1384 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/commands/shell.py
--rw-r--r--   0        0        0     1624 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/dibugger.py
--rw-r--r--   0        0        0        0 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/py.typed
--rw-r--r--   0        0        0      144 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/utils/__init__.py
--rw-r--r--   0        0        0      470 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/utils/chunk.py
--rw-r--r--   0        0        0      628 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/utils/embed.py
--rw-r--r--   0        0        0      808 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/utils/inspect.py
--rw-r--r--   0        0        0      696 2023-06-04 09:00:55.995692 dibug-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 dibug-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-11 04:47:47.416881 dibug-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1450 2023-06-11 04:47:47.416881 dibug-0.4.0/README.md
+-rw-r--r--   0        0        0       66 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/__init__.py
+-rw-r--r--   0        0        0      286 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/abc.py
+-rw-r--r--   0        0        0      195 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/__init__.py
+-rw-r--r--   0        0        0     1740 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/eval.py
+-rw-r--r--   0        0        0     1688 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/info.py
+-rw-r--r--   0        0        0      361 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/kill.py
+-rw-r--r--   0        0        0     1392 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/shell.py
+-rw-r--r--   0        0        0     4206 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/dibugger.py
+-rw-r--r--   0        0        0        0 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/py.typed
+-rw-r--r--   0        0        0      143 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/utils/__init__.py
+-rw-r--r--   0        0        0      470 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/utils/chunk.py
+-rw-r--r--   0        0        0      641 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/utils/embed.py
+-rw-r--r--   0        0        0      808 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/utils/object.py
+-rw-r--r--   0        0        0      780 2023-06-11 04:47:47.416881 dibug-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 dibug-0.4.0/PKG-INFO
```

### Comparing `dibug-0.3.0/LICENSE` & `dibug-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dibug-0.3.0/README.md` & `dibug-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/star0202/dibug/release.yml?branch=stable&style=flat-square)
-![GitHub](https://img.shields.io/github/license/star0202/dibug?style=flat-square)
-![PyPI](https://img.shields.io/pypi/v/dibug?style=flat-square)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dibug?style=flat-square)
+[![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/star0202/dibug/release.yml?branch=stable&style=flat-square)](https://github.com/star0202/dibug/actions/workflows/release.yml)
+[![GitHub](https://img.shields.io/github/license/star0202/dibug?style=flat-square)](https://github.com/star0202/dibug/blob/master/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/dibug?style=flat-square)](https://pypi.org/project/dibug)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dibug?style=flat-square)](https://pypi.org/project/dibug)
 
 # dibug
 
 Debugging Tool for discord.py
 
 # Installation
 
@@ -18,33 +18,37 @@
 # Usage
 
 ```py
 from discord import Client, Intents, Message
 
 from dibug import Dibugger
 
-owners = [798690702635827200]
+owners = [1234567890]  # owners id
+
+
+async def user_has_perm(msg: Message) -> bool:
+    return msg.author.id in owners
 
 
 class Bot(Client):
     def __init__(self) -> None:
         intents = Intents.default()
         intents.message_content = True  # dibug requires message content intent
         super().__init__(intents=intents)
 
-        self.dibugger = Dibugger(self, lambda id: id in owners)
-
-    async def on_message(self, msg: Message) -> None:
-        await self.dibugger.handle_msg(msg)
-
 
 bot = Bot()
 
+dibugger = Dibugger(bot, user_has_perm)
+
 bot.run("token")
 ```
 
 # Commands
 
 ### Default Prefix: `!dbg`
 
+- `<prefix>` | `<prefix> info | i`: Show bot info
+
 - `<prefix> eval | e | python | py <code>`: Evaluate python code
+- `<prefix> kill | k | shutdown`: Kill bot process
 - `<prefix> shell | sh <code>`: Execute shell command
```

### Comparing `dibug-0.3.0/dibug/commands/eval.py` & `dibug-0.4.0/dibug/commands/eval.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from traceback import format_exception
 
 from async_eval import eval
 from discord import Client, Message
 
-from ..abc import DibugCommand
+from ..abc import DibugCommandABC
 from ..utils import DibugEmbed, inspect
 
 
-class EvalCommand(DibugCommand):
+class EvalCommand(DibugCommandABC):
     def __init__(self, name: list[str], client: Client) -> None:
         self.name = name
 
         self.__client = client
 
     async def execute(self, msg: Message, args: str) -> None:
         if not args:
```

### Comparing `dibug-0.3.0/dibug/commands/info.py` & `dibug-0.4.0/dibug/commands/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from platform import release, system
 from sys import platform, version
 
 from discord import Client, Message, __version__
 from pkg_resources import get_distribution
 from psutil import Process
 
-from ..abc import DibugCommand
+from ..abc import DibugCommandABC
 
 
-class InfoCommand(DibugCommand):
+class InfoCommand(DibugCommandABC):
     def __init__(self, name: list[str], client: Client) -> None:
         self.name = name
 
         self.__client = client
 
     async def execute(self, msg: Message, args: str) -> None:
         lines: list[str] = []
```

### Comparing `dibug-0.3.0/dibug/commands/shell.py` & `dibug-0.4.0/dibug/commands/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from subprocess import run
 
 from discord import Message
 
-from ..abc import DibugCommand
+from ..abc import DibugCommandABC
 from ..utils import DibugEmbed
 
 
-class ShellCommand(DibugCommand):
+class ShellCommand(DibugCommandABC):
     def __init__(self, name: list[str]) -> None:
         self.name = name
 
     async def execute(self, msg: Message, args: str) -> None:
         if not args:
             await msg.reply("Missing code")
             return
@@ -46,12 +46,12 @@
                 "Input",
                 args,
                 "sh",
             )
             .chunked_fields(
                 "Output",
                 result.stdout,
-                "sh",
+                "ansi",
             )
         )
 
         await res.edit(content=None, embed=embed)
```

### Comparing `dibug-0.3.0/dibug/utils/embed.py` & `dibug-0.4.0/dibug/utils/embed.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         self,
         title: str,
         error: bool = False,
     ):
         super().__init__(title=title, color=0xFF0000 if error else 0x2B2D31)
 
     def chunked_fields(self, name: str, value: str, lang: str) -> "DibugEmbed":
-        chunked = chunk_string(value, 1024 - 10)
+        chunked = chunk_string(value, 1024 - (8 + len(lang)))
         for idx in range(len(chunked)):
             self.add_field(
                 name=f"{name} ({idx + 1}/{len(chunked)})",
                 value=f"```{lang}\n{chunked[idx]}```",
                 inline=False,
             )
```

### Comparing `dibug-0.3.0/dibug/utils/inspect.py` & `dibug-0.4.0/dibug/utils/object.py`

 * *Files identical despite different names*

### Comparing `dibug-0.3.0/pyproject.toml` & `dibug-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dibug"
-version = "0.3.0"
+version = "0.4.0"
 description = "Debugging Tool for discord.py"
 authors = ["Starcea <stardev.uwu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/star0202/dibug"
 
 [tool.poetry.dependencies]
@@ -18,14 +18,18 @@
 isort = "^5.12.0"
 
 [tool.poetry.group.type.dependencies]
 mypy = "^1.3.0"
 types-setuptools = "^67.8.0.0"
 types-psutil = "^5.9.5.13"
 
+[tool.poetry.group.docs.dependencies]
+sphinx = "6.2.1"
+sphinx-rtd-theme = "^1.2.1"
+
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 files = ["dibug", "typings"]
 strict = true
```

### Comparing `dibug-0.3.0/PKG-INFO` & `dibug-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dibug
-Version: 0.3.0
+Version: 0.4.0
 Summary: Debugging Tool for discord.py
 Home-page: https://github.com/star0202/dibug
 License: MIT
 Author: Starcea
 Author-email: stardev.uwu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: async-eval (>=0.1.11,<0.2.0)
 Requires-Dist: discord-py (>=2.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Project-URL: Repository, https://github.com/star0202/dibug
 Description-Content-Type: text/markdown
 
-![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/star0202/dibug/release.yml?branch=stable&style=flat-square)
-![GitHub](https://img.shields.io/github/license/star0202/dibug?style=flat-square)
-![PyPI](https://img.shields.io/pypi/v/dibug?style=flat-square)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dibug?style=flat-square)
+[![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/star0202/dibug/release.yml?branch=stable&style=flat-square)](https://github.com/star0202/dibug/actions/workflows/release.yml)
+[![GitHub](https://img.shields.io/github/license/star0202/dibug?style=flat-square)](https://github.com/star0202/dibug/blob/master/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/dibug?style=flat-square)](https://pypi.org/project/dibug)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dibug?style=flat-square)](https://pypi.org/project/dibug)
 
 # dibug
 
 Debugging Tool for discord.py
 
 # Installation
 
@@ -37,34 +37,38 @@
 # Usage
 
 ```py
 from discord import Client, Intents, Message
 
 from dibug import Dibugger
 
-owners = [798690702635827200]
+owners = [1234567890]  # owners id
+
+
+async def user_has_perm(msg: Message) -> bool:
+    return msg.author.id in owners
 
 
 class Bot(Client):
     def __init__(self) -> None:
         intents = Intents.default()
         intents.message_content = True  # dibug requires message content intent
         super().__init__(intents=intents)
 
-        self.dibugger = Dibugger(self, lambda id: id in owners)
-
-    async def on_message(self, msg: Message) -> None:
-        await self.dibugger.handle_msg(msg)
-
 
 bot = Bot()
 
+dibugger = Dibugger(bot, user_has_perm)
+
 bot.run("token")
 ```
 
 # Commands
 
 ### Default Prefix: `!dbg`
 
+- `<prefix>` | `<prefix> info | i`: Show bot info
+
 - `<prefix> eval | e | python | py <code>`: Evaluate python code
+- `<prefix> kill | k | shutdown`: Kill bot process
 - `<prefix> shell | sh <code>`: Execute shell command
```

