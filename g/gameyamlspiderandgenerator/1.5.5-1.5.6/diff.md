# Comparing `tmp/gameyamlspiderandgenerator-1.5.5.tar.gz` & `tmp/gameyamlspiderandgenerator-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.5.5.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.5.6.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.5.5.tar` & `gameyamlspiderandgenerator-1.5.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.5/LICENSE
--rwxr-xr-x   0        0        0     1350 2023-05-22 00:40:10.043310 gameyamlspiderandgenerator-1.5.5/README.md
--rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1912 2023-06-07 14:28:50.774672 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      674 2023-06-05 12:09:09.231664 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     1476 2023-05-22 02:04:55.203167 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/openai.py
--rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      559 2023-05-22 00:40:10.056896 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3177 2023-06-07 14:30:32.807398 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7008 2023-06-07 14:12:02.952532 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7926 2023-06-07 14:12:05.775288 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1838 2023-05-22 00:40:10.090828 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2138 2023-05-22 02:19:44.858160 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2550 2023-06-05 12:09:09.321318 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      719 2023-06-05 12:11:33.226209 gameyamlspiderandgenerator-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.6/LICENSE
+-rwxr-xr-x   0        0        0     1350 2023-06-11 10:23:19.902922 gameyamlspiderandgenerator-1.5.6/README.md
+-rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1924 2023-06-11 10:27:03.919708 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      674 2023-06-11 10:23:19.904684 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     1476 2023-06-11 10:23:19.905735 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/openai.py
+-rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      559 2023-05-22 00:40:10.056896 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3177 2023-06-11 10:23:19.906828 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7008 2023-06-11 10:23:19.907881 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7926 2023-06-11 10:23:19.908516 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1838 2023-05-22 00:40:10.090828 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     2138 2023-06-11 10:23:19.909201 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2550 2023-06-11 10:23:19.910070 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      719 2023-06-11 10:25:08.585652 gameyamlspiderandgenerator-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.6/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.5.5/LICENSE` & `gameyamlspiderandgenerator-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/README.md` & `gameyamlspiderandgenerator-1.5.6/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,17 @@
   - steam
   - itchio
 hook:
   - search
   - validate
 # - openai
 # if you don't want to set proxy, please fill in {}
+proxy: { }
 # http: socks5://127.0.0.1:7891
 # https: socks5://127.0.0.1:7891
-proxy: { }
 gitToken: 'your token'
 api:
   google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
   apple: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
   openai: yourkey
 
 ```
```

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import argparse
 
 from yaml import safe_load
 
 from .util.config import config
+from .util.fgi import default_config
 from .util.fgi_yaml import get_valid_filename
 from .util.plugin_manager import pkg
 import sys
 from loguru import logger
 from gameyamlspiderandgenerator import produce_yaml
 
 parser = argparse.ArgumentParser()
 logger.remove()
 logger.add(sys.stderr, level="INFO")
 parser.add_argument(
     "-f",
     "--config",
     type=str,
-    default={"plugin": ["steam", "itchio"], "hook": ["search", "validate"]},
+    default=default_config,
     help="The location of config.yaml (default null)",
 )
 parser.add_argument(
     "-o",
     "--output",
     type=str,
     default=None,
@@ -30,24 +31,21 @@
     "--fast",
     action='store_true',
     default=False,
     help="Whether to disable all hooks (default: false)",
 )
 parser.add_argument("url", metavar="URL")
 args = parser.parse_args()
-
-
-
 if isinstance(args.config, str):
     with open(args.config) as f:
         setting = safe_load(f)
 else:
     setting = args.config
 if args.fast:
-     setting['hook'] = None
+    setting['hook'] = None
 config.update(setting)
 pkg.__init__()
 yml = produce_yaml(args.url)
 if args.output is None:
     print(yml)
 elif "." not in args.output:
     if args.output == "zip":
@@ -61,10 +59,12 @@
         with open(args.output, 'wb') as f:
             f.write(bytes(yml))
     elif "yaml" in args.output:
         with open(args.output, 'w') as f:
             f.write(str(yml))
     else:
         logger.error(f"unsupported file format: {args.output[args.output.rfind('.'):]}")
+        exit(3)
 
 else:
     logger.error(f"unsupported file format: {args.output[args.output.rfind('.'):]}")
+    exit(3)
```

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/openai.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/openai.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/hook/validate.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.5.6/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.5/pyproject.toml` & `gameyamlspiderandgenerator-1.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.5.5"
+version = "1.5.6"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.5.5/PKG-INFO` & `gameyamlspiderandgenerator-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.5.5
+Version: 1.5.6
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -40,17 +40,17 @@
   - steam
   - itchio
 hook:
   - search
   - validate
 # - openai
 # if you don't want to set proxy, please fill in {}
+proxy: { }
 # http: socks5://127.0.0.1:7891
 # https: socks5://127.0.0.1:7891
-proxy: { }
 gitToken: 'your token'
 api:
   google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
   apple: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
   openai: yourkey
 
 ```
```

