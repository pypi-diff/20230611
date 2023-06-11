# Comparing `tmp/nonebot-plugin-pcrjjc-0.1.4.tar.gz` & `tmp/nonebot-plugin-pcrjjc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-pcrjjc-0.1.4.tar", last modified: Sun Jun 11 00:32:49 2023, max compression
+gzip compressed data, was "nonebot-plugin-pcrjjc-0.1.5.tar", last modified: Sun Jun 11 05:29:11 2023, max compression
```

## Comparing `nonebot-plugin-pcrjjc-0.1.4.tar` & `nonebot-plugin-pcrjjc-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.692000 nonebot-plugin-pcrjjc-0.1.4/
--rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2699 2023-06-11 00:32:49.690003 nonebot-plugin-pcrjjc-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1835 2023-06-10 08:28:10.000000 nonebot-plugin-pcrjjc-0.1.4/README.md
--rw-rw-rw-   0        0        0     1583 2023-06-10 23:49:20.000000 nonebot-plugin-pcrjjc-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 00:32:49.692000 nonebot-plugin-pcrjjc-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.533373 nonebot-plugin-pcrjjc-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.564375 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/
--rw-rw-rw-   0        0        0    39200 2023-06-11 00:18:38.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/aiorequests.py
--rw-rw-rw-   0        0        0     6481 2023-06-09 05:09:18.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/bsgamesdk.py
--rw-rw-rw-   0        0        0      840 2023-06-10 23:26:37.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/config.py
-drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.678996 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/fonts/
--rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
--rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/pcrclient.py
--rw-rw-rw-   0        0        0     7647 2023-06-11 00:18:38.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/query.py
--rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/rsacr.py
--rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/text2img.py
-drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.676020 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/
--rw-rw-rw-   0        0        0     2699 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 05:29:11.683294 nonebot-plugin-pcrjjc-0.1.5/
+-rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2699 2023-06-11 05:29:11.681296 nonebot-plugin-pcrjjc-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1835 2023-06-10 08:28:10.000000 nonebot-plugin-pcrjjc-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1583 2023-06-11 05:28:34.000000 nonebot-plugin-pcrjjc-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 05:29:11.683294 nonebot-plugin-pcrjjc-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 05:29:11.567498 nonebot-plugin-pcrjjc-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 05:29:11.626505 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/
+-rw-rw-rw-   0        0        0    39219 2023-06-11 05:20:57.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/aiorequests.py
+-rw-rw-rw-   0        0        0     6481 2023-06-09 05:09:18.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/bsgamesdk.py
+-rw-rw-rw-   0        0        0      840 2023-06-10 23:26:37.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/config.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:29:11.656504 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/fonts/
+-rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
+-rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/pcrclient.py
+-rw-rw-rw-   0        0        0     7647 2023-06-11 00:18:38.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/query.py
+-rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/rsacr.py
+-rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/text2img.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:29:11.651505 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc.egg-info/
+-rw-rw-rw-   0        0        0     2699 2023-06-11 05:29:11.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-06-11 05:29:11.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 05:29:11.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-11 05:29:11.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-11 05:29:11.000000 nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
```

### Comparing `nonebot-plugin-pcrjjc-0.1.4/LICENSE` & `nonebot-plugin-pcrjjc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/PKG-INFO` & `nonebot-plugin-pcrjjc-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.1.4
+Version: 0.1.5
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `nonebot-plugin-pcrjjc-0.1.4/README.md` & `nonebot-plugin-pcrjjc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/pyproject.toml` & `nonebot-plugin-pcrjjc-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pcrjjc"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     {name="reine-ishyanami", email="2402979195@qq.com"}
 ]
 description = "pcrjjc排名监测插件"
 readme = "README.md"
 license = { text = "AGPL-3" }
 requires-python = ">=3.10, <4.0"
```

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/__init__.py` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 require("nonebot_plugin_apscheduler")
 
 from nonebot_plugin_apscheduler import scheduler
 
 __plugin_meta__ = PluginMetadata(
     name="pcrjjc",
+    config=Config,
     description="公主连结（国服）排名监测工具",
     usage="发送 竞技场帮助 获取详细使用说明",
     type="application",
     homepage="https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc",
     supported_adapters={"~onebot.v11"}
 )
```

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/aiorequests.py` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/aiorequests.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/bsgamesdk.py` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/bsgamesdk.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/config.py` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/pcrclient.py` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/pcrclient.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/query.py` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/query.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/text2img.py` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc/text2img.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.1.4
+Version: 0.1.5
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt` & `nonebot-plugin-pcrjjc-0.1.5/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

