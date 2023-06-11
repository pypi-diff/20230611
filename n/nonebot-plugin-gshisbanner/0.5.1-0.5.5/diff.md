# Comparing `tmp/nonebot_plugin_gshisbanner-0.5.1.tar.gz` & `tmp/nonebot_plugin_gshisbanner-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-0.5.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-0.5.5.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-0.5.1.tar` & `nonebot_plugin_gshisbanner-0.5.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/LICENSE
--rw-r--r--   0        0        0     5295 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/README.md
--rw-r--r--   0        0        0      389 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0     1030 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      427 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      292 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0     3280 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1232 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0     4622 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/main.py
--rw-r--r--   0        0        0     2654 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0      576 2023-05-10 13:29:48.700538 nonebot_plugin_gshisbanner-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5988 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-11 14:06:12.602589 nonebot_plugin_gshisbanner-0.5.5/LICENSE
+-rw-r--r--   0        0        0     5295 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/README.md
+-rw-r--r--   0        0        0      593 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0     1030 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      427 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      300 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0     3276 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1231 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     5270 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/main.py
+-rw-r--r--   0        0        0     2640 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0      600 2023-06-11 14:06:12.606588 nonebot_plugin_gshisbanner-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     5987 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.5.5/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-0.5.1/LICENSE` & `nonebot_plugin_gshisbanner-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.1/README.md` & `nonebot_plugin_gshisbanner-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/deal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from pathlib import Path
-from typing import Union, List, Dict
+from typing import Dict, List, Union
 
+from .config import plugin_config
 from .deal_json import load_json_from_url
-from .config import config
 
 path = Path.cwd() / "data" / "genshin_history"
 
 
 async def get_info_from_url(
     cha: bool, cache_dir: Path = path
 ) -> Union[Dict, List[Dict]]:
     """
     :param cha: 类型
     :param cache_dir: 本地缓存
     :return: Union[dict, list[dict]]
     """
     cache_dir.mkdir(parents=True, exist_ok=True)
-    url = f"https://{config.gshisbanner_json_url}/{'character' if cha else 'weapon'}.json"
+    url = f"https://{plugin_config.gshisbanner_json_url}/{'character' if cha else 'weapon'}.json"
     cache_path = cache_dir / ("character.json" if cha else "weapon.json")
     return await load_json_from_url(url, path=cache_path)
 
 
 async def deal_info_from_name(
     name: str, choose: str
 ) -> List[Dict[str, Union[str, List[str]]]]:
@@ -62,15 +62,15 @@
 ) -> List[Dict[str, Union[str, List[str]]]]:
     """
     :param version: 版本号
     :param is_all: 是否获取全部卡池
     :return: 获取到的历史卡池数据
     """
     # 获取所有卡池信息
-    json = await get_info_from_url(True) + await get_info_from_url(False)  # type: ignore
+    json = await get_info_from_url(True) + await get_info_from_url(False)
     # 卡池类型列表
     type_list = ["five_character", "four_character", "five_weapon", "four_weapon"]
     result = []
     for data in json:
         # 判断是否为指定版本
         if data["version"][:3] == version if is_all else data["version"] == version:
             # 构造卡池信息字典
@@ -87,9 +87,7 @@
                     for x in data["items"]
                     if x.get("rankType") == (5 if "five" in item else 4)
                     and x.get("itemType") == item.split("_")[1].capitalize()
                 ]
             result.append(temp)
     # 去除空值
     return [{k: v for k, v in data.items() if v} for data in result]
-
-
```

### Comparing `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+import json
 from json import JSONDecodeError
 from pathlib import Path
-from typing import Union, Dict, List
-
-import json
+from typing import Dict, List, Union
 
 from .api import get
 
 
 def save_json(
     data: Union[Dict, List[Dict]], path: Union[Path, str], encoding: str = "utf-8"
 ):
```

### Comparing `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/main.py` & `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+import contextlib
 from pathlib import Path
 from typing import Union
 
-from nonebot import on_regex, get_driver, logger
+from nonebot import get_driver, logger, on_regex
 from nonebot.adapters.onebot.v11 import (
-    MessageEvent,
-    GroupMessageEvent,
-    PrivateMessageEvent,
-    Bot,
     GROUP_ADMIN,
     GROUP_OWNER,
+    Bot,
+    GroupMessageEvent,
+    MessageEvent,
+    PrivateMessageEvent,
 )
 from nonebot.params import RegexDict
 from nonebot.permission import SUPERUSER
+
 from .alias import find_name
 from .api import get
-from .config import config
+from .config import plugin_config
 from .deal import deal_info_from_name, deal_info_from_version
 from .deal_json import load_json_from_url, save_json
 from .send import word_send_from_name, word_send_from_version
 
 old_gacha = on_regex(
     r"(?<!\w)(?P<name>[\u4e00-\u9fa5]+)(?<!刷新)(历史卡池|历史up)(?P<len>\d{0,2})(?!.)",
     priority=35,
@@ -35,97 +37,104 @@
     priority=13,
     block=False,
 )
 
 DRIVER = get_driver()
 gacha_info_path = Path.cwd() / "data" / "genshin_history"
 special_version = ["1.3"]  # 特殊三卡池版本
-forward_length = config.gshisbanner_forward_length  # 合并转发长度
+forward_length = plugin_config.gshisbanner_forward_length  # 合并转发长度
 
 
 @old_gacha.handle()
 async def _(
     bot: Bot,
     event: Union[GroupMessageEvent, PrivateMessageEvent],
-    regex_dict: dict = RegexDict(),
+    regex_dict: dict = RegexDict(),  # noqa: B008
 ):
     type_name = regex_dict["name"]
     if not isinstance(forward_length, int) or forward_length <= 0:
         await old_gacha.finish("合并转发长度设置错误")
     # regex_dict["len"]：表示合并转发的长度,由用户输入获取，未获取到则为默认值
     length = (
         int(regex_dict["len"])
         if regex_dict["len"]
-        else config.gshisbanner_forward_length
+        else plugin_config.gshisbanner_forward_length
     )
     # 获取角色真实名字
     real_name, real_type = find_name(type_name)
     if real_name is None or real_type not in ["角色", "武器"]:
         await old_gacha.finish("该角色/武器不存在或是从未up过")
     # 获取up信息
     info = await deal_info_from_name(real_name, "cha" if real_type == "角色" else "wep")
     if length > 0:
         await word_send_from_name(bot, event, real_name, info, length)
     await old_gacha.finish()
 
 
 @version_gacha.handle()
-async def _(bot: Bot, event: MessageEvent, regex_dict: dict = RegexDict()):
+async def _(
+    bot: Bot, event: MessageEvent, regex_dict: dict = RegexDict()  # noqa: B008
+):  # noqa: B008
     # 判断是否为三卡池的版本
     if regex_dict["version"] not in special_version and regex_dict["upordown"] == "3":
         await version_gacha.finish()
     # 获取版本信息
     real_version = (
         f"{regex_dict['version']}.{regex_dict['upordown']}"
         if regex_dict["upordown"]
         else regex_dict["version"]
     )
     # 根据版本获取up信息
-    info = await deal_info_from_version(
-        real_version, False if regex_dict["upordown"] else True
-    )
+    info = await deal_info_from_version(real_version, not regex_dict["upordown"])
     if info:
         await word_send_from_version(bot, event, real_version, info)
     await version_gacha.finish()
 
 
 @refresh.handle()
 async def _(
     event: MessageEvent,
-    regex_dict: dict = RegexDict(),
+    regex_dict: dict = RegexDict(),  # noqa: B008
 ):
     type_name = regex_dict["name"]
     types = ["character", "weapon"]
     if type_name == "历史卡池":
         for i in types:
-            url = f"https://{config.gshisbanner_json_url}/{i}.json"
+            url = f"https://{plugin_config.gshisbanner_json_url}/{i}.json"
             path = gacha_info_path / f"{i}.json"
             result = await load_json_from_url(url, path, True)
             if not result:
                 await refresh.finish(f"刷新{type_name}失败,可能是网络问题或api失效")
             save_json(result, path)
             logger.info(f"{i}.json文件保存成功")
     elif type_name == "别名":
-        if (await init_group_card()) is False:
+        if (await init_group_card(True)) is False:
             await refresh.finish(f"刷新{type_name}失败,可能是网络问题或api失效")
     await refresh.finish(f"刷新{type_name}成功")
 
 
 @DRIVER.on_startup
-async def init_group_card():
+async def init_group_card(force_refresh: bool = False) -> bool:
     if not gacha_info_path.exists():
         gacha_info_path.mkdir(parents=True)
-    url = "https://fastly.jsdelivr.net/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json"
-    if (gacha_info_path / "alias.json").exists():
+    urls = [
+        "https://jsd.cdn.zzko.cn/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json",
+        "https://raw.fastgit.org/forchannot/nonebot-plugin-gshisbanner/main/data/genshin_history/alias.json",
+        "https://cdn.jsdelivr.net/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json",
+        "https://cdn.staticaly.com/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json",
+        "https://fastly.jsdelivr.net/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json",
+    ]
+    if (gacha_info_path / "alias.json").exists() and not force_refresh:
         logger.info("alias.json文件已存在，跳过下载，如需更新请使用刷新别名功能")
-        return
-    try:
-        resp = await get(url)
-    except Exception as e:
-        logger.warning(f"alias.json文件下载失败,错误信息:{e}")
-        return
-    if resp.status_code != 200:
+        return False
+    for url in urls:
+        with contextlib.suppress(Exception):
+            resp = await get(url, follow_redirects=True)
+            if resp.status_code == 200:
+                break
+    else:
         logger.warning("alias.json文件下载失败")
-        return
+        return False
     data = resp.json()
     save_json(data=data, path=gacha_info_path / "alias.json")
     logger.info("alias.json文件保存成功")
+    return True
```

### Comparing `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-0.5.5/nonebot_plugin_gshisbanner/send.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from datetime import datetime
 
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, PrivateMessageEvent
 from nonebot import get_driver
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, PrivateMessageEvent
 
 DRIVER = get_driver()
 NICKNAME: str = (
     list(DRIVER.config.nickname)[0] if list(DRIVER.config.nickname) else "BOT"
 )
 
 
 # 角色历史卡池文字合并转发预处理
 async def word_send_from_name(bot, event, real_name, info, length):
     end_time = datetime.strptime(info[0]["end"], "%Y-%m-%d %H:%M:%S").date()
     end_t = (datetime.now().date() - end_time).days
     delta_time = f"最近一次up距离现在已有{end_t}天" if end_t > 0 else f"当前正在up中,距离结束还有约{-end_t}天"
     msg_content = f"{real_name}{delta_time}"
     for i in range(0, len(info), length):
-        if i == 0:
-            msg = msg_content
-        else:
-            msg = []
-        await send_banner_info(bot, event, msg, info[i: i + length])
+        msg = msg_content if i == 0 else []
+        await send_banner_info(bot, event, msg, info[i : i + length])
 
 
 # 版本卡池文字合并转发预处理
 async def word_send_from_version(bot, event, version, info):
     msg_content = f"{version}版本卡池"
     await send_banner_info(bot, event, msg_content, info)
 
@@ -65,12 +62,13 @@
         banner_four = " ".join(info.get("four_character", info.get("four_weapon", [])))
         msg.append(
             {
                 "type": "node",
                 "data": {
                     "name": NICKNAME,
                     "uin": event.self_id,
-                    "content": f"版本：{version}\n五星：{banner_five}\n四星：{banner_four}\nup时间：\n{start}~~{end}",
+                    "content": f"版本：{version}\n五星：{banner_five}"
+                    f"\n四星：{banner_four}\nup时间：\n{start}~~{end}",
                 },
             }
         )
-    await send_forward_msg(bot, event, msg)
+    await send_forward_msg(bot, event, msg)
```

### Comparing `nonebot_plugin_gshisbanner-0.5.1/PKG-INFO` & `nonebot_plugin_gshisbanner-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 0.5.1
+Version: 0.5.5
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1,<3.0)
-Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.5.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.5.5 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
 Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.1,<3.0) Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0) Description-Content-
+(>=2.2.2,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Description-Content-
 Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-gshisbanner _â¨
  æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ â¨_ [license]
                                [pypi] [python]
                                    [onebot]
```

