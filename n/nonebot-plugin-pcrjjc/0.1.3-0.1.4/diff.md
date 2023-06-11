# Comparing `tmp/nonebot-plugin-pcrjjc-0.1.3.tar.gz` & `tmp/nonebot-plugin-pcrjjc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-pcrjjc-0.1.3.tar", last modified: Sat Jun 10 13:17:40 2023, max compression
+gzip compressed data, was "nonebot-plugin-pcrjjc-0.1.4.tar", last modified: Sun Jun 11 00:32:49 2023, max compression
```

## Comparing `nonebot-plugin-pcrjjc-0.1.3.tar` & `nonebot-plugin-pcrjjc-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 13:17:40.155259 nonebot-plugin-pcrjjc-0.1.3/
--rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2699 2023-06-10 13:17:40.153247 nonebot-plugin-pcrjjc-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1835 2023-06-10 08:28:10.000000 nonebot-plugin-pcrjjc-0.1.3/README.md
--rw-rw-rw-   0        0        0     1583 2023-06-10 13:08:23.000000 nonebot-plugin-pcrjjc-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 13:17:40.155259 nonebot-plugin-pcrjjc-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 13:17:40.037580 nonebot-plugin-pcrjjc-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 13:17:40.098115 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/
--rw-rw-rw-   0        0        0    38840 2023-06-10 12:27:03.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/aiorequests.py
--rw-rw-rw-   0        0        0     6481 2023-06-09 05:09:18.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/bsgamesdk.py
--rw-rw-rw-   0        0        0      806 2023-06-10 12:25:03.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/config.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:17:40.128260 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/fonts/
--rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
--rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/pcrclient.py
--rw-rw-rw-   0        0        0     7646 2023-06-10 12:26:23.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/query.py
--rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/rsacr.py
--rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/text2img.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:17:40.124246 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc.egg-info/
--rw-rw-rw-   0        0        0     2699 2023-06-10 13:17:39.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-06-10 13:17:40.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 13:17:39.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-10 13:17:39.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-10 13:17:39.000000 nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.692000 nonebot-plugin-pcrjjc-0.1.4/
+-rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2699 2023-06-11 00:32:49.690003 nonebot-plugin-pcrjjc-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1835 2023-06-10 08:28:10.000000 nonebot-plugin-pcrjjc-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1583 2023-06-10 23:49:20.000000 nonebot-plugin-pcrjjc-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 00:32:49.692000 nonebot-plugin-pcrjjc-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.533373 nonebot-plugin-pcrjjc-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.564375 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/
+-rw-rw-rw-   0        0        0    39200 2023-06-11 00:18:38.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/aiorequests.py
+-rw-rw-rw-   0        0        0     6481 2023-06-09 05:09:18.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/bsgamesdk.py
+-rw-rw-rw-   0        0        0      840 2023-06-10 23:26:37.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/config.py
+drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.678996 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/fonts/
+-rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
+-rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/pcrclient.py
+-rw-rw-rw-   0        0        0     7647 2023-06-11 00:18:38.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/query.py
+-rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/rsacr.py
+-rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/text2img.py
+drwxrwxrwx   0        0        0        0 2023-06-11 00:32:49.676020 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/
+-rw-rw-rw-   0        0        0     2699 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-11 00:32:49.000000 nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
```

### Comparing `nonebot-plugin-pcrjjc-0.1.3/LICENSE` & `nonebot-plugin-pcrjjc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.3/PKG-INFO` & `nonebot-plugin-pcrjjc-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.1.3
+Version: 0.1.4
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `nonebot-plugin-pcrjjc-0.1.3/README.md` & `nonebot-plugin-pcrjjc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.3/pyproject.toml` & `nonebot-plugin-pcrjjc-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pcrjjc"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     {name="reine-ishyanami", email="2402979195@qq.com"}
 ]
 description = "pcrjjc排名监测插件"
 readme = "README.md"
 license = { text = "AGPL-3" }
 requires-python = ">=3.10, <4.0"
```

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/__init__.py` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,24 +23,35 @@
     PrivateMessageEvent,
     FriendAddNoticeEvent,
     GroupDecreaseNoticeEvent
 )
 from nonebot.internal.matcher import Matcher
 from nonebot.params import RegexGroup
 from nonebot.permission import SUPERUSER
+from nonebot.plugin import PluginMetadata
 
 from .config import Config
 from .pcrclient import ApiException
 from .query import queue, path
 from .text2img import image_draw
 
 require("nonebot_plugin_apscheduler")
 
 from nonebot_plugin_apscheduler import scheduler
 
+__plugin_meta__ = PluginMetadata(
+    name="pcrjjc",
+    description="公主连结（国服）排名监测工具",
+    usage="发送 竞技场帮助 获取详细使用说明",
+    type="application",
+    homepage="https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc",
+    supported_adapters={"~onebot.v11"}
+)
+
+
 driver = get_driver()
 config = Config.parse_obj(driver.config)
 
 MAX_PRI = config.max_pri
 MAX_PCRID = config.max_pcrid
 MAX_HISTORY = config.max_history
 NOTICE_CD_MIN = config.notice_cd_min
@@ -85,16 +96,15 @@
 4）pcrjjc关闭排名上升
 '''
 
 # 数据库对象初始化
 # JJCH = JJCHistoryStorage()
 friend_list = []
 pcrid_list = []
-if len(config.superusers) > 0:
-    admin = int(config.superusers[0])
+admin = int(config.superusers[0]) if len(config.superusers) > 0 else 0
 config = join(path, 'binds.json')
 root = {'arena_bind': {}}
 if exists(config):
     with open(config) as fp:
         root = load(fp)
 lck = Lock()
 lck_friend_list = Lock()
```

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/aiorequests.py` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/aiorequests.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/bsgamesdk.py` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/bsgamesdk.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/config.py` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from os.path import join
+
 from pydantic import BaseModel, Extra
 
 
 class Config(BaseModel, extra=Extra.ignore):
     """Plugin Config Here"""
     apscheduler_log_level: int = 30
-    data_path: str = "data\\pcrjjc"  # 数据存储目录
+    data_path: str = join("data", "pcrjjc")  # 数据存储目录
     superusers: list[str]  # 超级用户列表，建议只填一个，填多个可能导致后续用户指令失效
     otto: bool = False  # 是否自动过验证码，因自动过码失效，改为手动过码
     version: str = "6.2.0"  # 游戏版本号
     max_pri: int = 0  # 最大私聊人数
     max_pcrid: int = 8  # 每个QQ号绑定的最多数量
     max_history: int = 50  # 每个QQ号保存的最多击剑记录
     notice_cd_min: int = 10  # 上线推送频率
```

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/pcrclient.py` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/pcrclient.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/query.py` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 otto = config.otto
 ordd = 'x'
 validate = None
 validating = False
 ac_first = False
 client = None
 captcha_cnt = 0
-if len(config.superusers) > 0:
-    admin = int(config.superusers[0])
+admin = int(config.superusers[0]) if len(config.superusers) > 0 else 0
 data_path = config.data_path
 path = join(str(Path()), data_path)
 ac_info = []
 binds_info = {}
 account_json_template = [
     {
         "account": "account1",
```

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc/text2img.py` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc/text2img.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.1.3
+Version: 0.1.4
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `nonebot-plugin-pcrjjc-0.1.3/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt` & `nonebot-plugin-pcrjjc-0.1.4/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

