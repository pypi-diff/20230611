# Comparing `tmp/nonebot_plugin_random_draw-0.0.2.tar.gz` & `tmp/nonebot_plugin_random_draw-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_random_draw-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_random_draw-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_random_draw-0.0.2.tar` & `nonebot_plugin_random_draw-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_random_draw-0.0.2/LICENSE
--rw-r--r--   0        0        0    21050 2023-05-28 05:43:43.600557 nonebot_plugin_random_draw-0.0.2/nonebot_plugin_random_draw/__init__.py
--rw-r--r--   0        0        0      980 2023-05-28 06:27:47.158019 nonebot_plugin_random_draw-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5763 2023-05-28 05:40:33.394241 nonebot_plugin_random_draw-0.0.2/README.md
--rw-r--r--   0        0        0     6546 1970-01-01 00:00:00.000000 nonebot_plugin_random_draw-0.0.2/setup.py
--rw-r--r--   0        0        0     6512 1970-01-01 00:00:00.000000 nonebot_plugin_random_draw-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-11 15:57:38.513743 nonebot_plugin_random_draw-0.1.0/LICENSE
+-rw-r--r--   0        0        0    22573 2023-06-11 15:57:38.487736 nonebot_plugin_random_draw-0.1.0/nonebot_plugin_random_draw/__init__.py
+-rw-r--r--   0        0        0      980 2023-06-11 15:57:38.855820 nonebot_plugin_random_draw-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6239 2023-06-11 15:57:35.154227 nonebot_plugin_random_draw-0.1.0/README.md
+-rw-r--r--   0        0        0     6976 1970-01-01 00:00:00.000000 nonebot_plugin_random_draw-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_random_draw-0.0.2/LICENSE` & `nonebot_plugin_random_draw-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_random_draw-0.0.2/nonebot_plugin_random_draw/__init__.py` & `nonebot_plugin_random_draw-0.1.0/nonebot_plugin_random_draw/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from nonebot import require, on_command
 from nonebot.adapters.onebot.v11 import Bot, Event, GroupMessageEvent
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.adapters.onebot.v11 import GROUP_ADMIN, GROUP_OWNER
 from nonebot.permission import SUPERUSER
 from nonebot.params import CommandArg
 from nonebot.exception import FinishedException
+from nonebot.typing import T_State
 
 from nonebot.plugin import PluginMetadata
 
 
 help_text = f"""
 功能说明：命令列表（命令前缀自行匹配）
 获取帮助：随机抽取帮助
@@ -27,14 +28,22 @@
 删除指定随抽组中的待抽内容（可多个，用空格分隔）：随抽删除 <组号> <内容>
 删除指定组号的随抽组：随抽组删除 <组号>
 查看本群所有的随抽组内容（含组号和组名）：随抽组列表
 查看指定组号的所有待抽内容：随抽列表 <组号>
 在指定随抽组中随机抽取一个待抽内容：随抽 <组号>
 清空本群中所有的随抽组（慎用）：随抽组清空
 清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>
+
+
+注意：
+随抽内容必须配合文本描述，不能只是图片。
+批量添加待抽内容不支持图片批量，如果你硬这么用，就都是重复的图片。
+随抽删除只需要传入文本内容即可，不需要图片。
+查看随抽列表只返回文本内容。
+图片用的是tx的图床，所以一段时间后会挂。
 """.strip()
 
 __plugin_meta__ = PluginMetadata(
     name = '随机抽取设定内容插件',
     description = '适用于nonebot2 v11的随机抽取设定内容插件',
     usage = help_text
 )
@@ -135,18 +144,36 @@
         logger.info(e)
         msg = '创建失败！（请看后台日志排查问题）'
         await cmd1.finish(Message(f'{msg}'), reply_message=True)
 
 
 # 随抽添加 <组号> <内容>
 @cmd2.handle()
-async def _(bot: Bot, event: GroupMessageEvent, msg: Message = CommandArg()):
+async def _(bot: Bot, event: GroupMessageEvent, state: T_State, msg: Message = CommandArg()):
     content = msg.extract_plain_text()
     content = content.split()
 
+    print(content)
+
+    if msg:
+        state["src_img"] = msg
+    pass
+
+    # 获取图片部分
+    event_msg = event.get_plaintext()
+    event_msg: Message = state["src_img"]
+
+    # 暂时先拿tx当图床吧
+    img_url = ""
+
+    for msg_sag in event_msg:
+        if msg_sag.type == "image":
+            img_url = msg_sag.data["url"]
+            break
+
     group_id = event.group_id
 
     data_path = await check_data_file(group_id)
 
     if len(content) < 2:
         msg = '命令错误，命令：/随抽添加 <组号> <内容>'
         await cmd2.finish(Message(f'{msg}'), reply_message=True)
@@ -170,21 +197,28 @@
             if group_num not in data_json:
                 msg = "不存在此随抽组，请先创建随抽组。"
                 await cmd2.send(Message(f'{msg}'), reply_message=True)
 
             data_arr = []
 
             for data in content:
-                for users in data_json[group_num]["内容"]:
+                flag = 0
+                for tmp_data in data_json[group_num]["内容"]:
                     # 重复性检测
-                    if users == data:
+                    if tmp_data['文本'] == data:
+                        # print(f"{data}重复")
                         data_arr.append(data)
+
+                        flag = 1
                         break
 
-                data_json[group_num]["内容"].append(data)
+                if flag == 0:
+                    tmp = {"文本": data, "图片": img_url}
+                    data_json[group_num]["内容"].append(tmp)
+                    print(f"追加{json.dumps(tmp)}")
             
             if len(data_arr) != 0:
                 msg = '组号：' + group_num + "，已存在 "
                 for data in data_arr:
                     msg = msg + data + " "
                 msg = msg + "，请勿重复添加！"
                 await cmd2.send(Message(f'{msg}'), reply_message=True)
@@ -238,19 +272,20 @@
             if len(data_json[group_num]) == 0:
                 msg = '当前随抽组无内容，无需删除。'
                 await cmd3.finish(Message(f'{msg}'), reply_message=True)
 
             # qq = event.get_user_id()
 
             for content_str in content:
-                if content_str in data_json[group_num]["内容"]:
-                    data_json[group_num]["内容"].remove(content_str)
-                    # 将处理后的JSON数据写入文件
-                    with open(data_path, 'w', encoding="utf-8") as f:
-                        json.dump(data_json, f, ensure_ascii=False)
+                for text_and_img in data_json[group_num]["内容"]:
+                    if content_str == text_and_img["文本"]:
+                        data_json[group_num]["内容"].remove(text_and_img)
+                        # 将处理后的JSON数据写入文件
+                        with open(data_path, 'w', encoding="utf-8") as f:
+                            json.dump(data_json, f, ensure_ascii=False)
 
             msg = "随抽删除匹配的内容成功~"
             await cmd3.send(Message(f'{msg}'), reply_message=True)
     except FinishedException:
         pass
     except Exception as e:
         logger.info(e)
@@ -402,17 +437,17 @@
                 await cmd6.finish(Message(f'{msg}'), reply_message=True)
         
             # 如果是空数据
             if len(data_json) == 0:
                 await cmd6.finish('没有随抽组，请先创建。', reply_message=True)
 
         if content in data_json:
-            msg = "内容：\n"
+            msg = "内容(图片不展示)：\n"
             for data in data_json[content]['内容']:
-                msg = msg + data + '\n'
+                msg = msg + data['文本'] + '\n'
             await cmd6.finish(msg)
         else:
             await cmd6.finish('您查询的随抽组不存在，请先查询随抽组列表确认组号。', reply_message=True)
     except FinishedException:
         pass
     except Exception as e:
         logger.info(e)
@@ -451,15 +486,21 @@
         
             # 如果是空数据
             if len(data_json) == 0:
                 await cmd7.finish('没有随抽组，请先创建。', reply_message=True)
 
         if 0 != len(data_json[content]['内容']):
             # 随机抽一个
-            await cmd7.finish(data_json[content]['内容'][random.randint(0, len(data_json[content]['内容']) - 1)])
+            index = random.randint(0, len(data_json[content]['内容']) - 1)
+            text_seg = MessageSegment.text(data_json[content]['内容'][index]['文本'])
+            if data_json[content]['内容'][index]['图片'] != "":
+                img_seg = MessageSegment.image(file=data_json[content]['内容'][index]['图片'])
+                await cmd7.finish(Message(text_seg + img_seg))
+            else:
+                await cmd7.finish(Message(text_seg))
         else:
             await cmd7.finish('您抽的随抽组无内容，请先添加内容。', reply_message=True)
     except FinishedException:
         pass
     except Exception as e:
         logger.info(e)
         msg = '随抽失败！（请看后台日志排查问题）'
```

### Comparing `nonebot_plugin_random_draw-0.0.2/pyproject.toml` & `nonebot_plugin_random_draw-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-random_draw"
-version = "0.0.2"
+version = "0.1.0"
 description = "通过添加各种想要抽取的内容，最后进行随机抽取。"
 authors = ["Ikaros <327209194@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_random_draw"}]
 homepage = "https://github.com/Ikaros-521/nonebot_plugin_random_draw"
 repository = "https://github.com/Ikaros-521/nonebot_plugin_random_draw"
```

### Comparing `nonebot_plugin_random_draw-0.0.2/README.md` & `nonebot_plugin_random_draw-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -98,18 +98,26 @@
 删除指定随抽组中的待抽内容（可多个，用空格分隔）：随抽删除 <组号> <内容>
 删除指定组号的随抽组：随抽组删除 <组号>
 查看本群所有的随抽组内容（含组号和组名）：随抽组列表
 查看指定组号的所有待抽内容：随抽列表 <组号>
 在指定随抽组中随机抽取一个待抽内容：随抽 <组号>
 清空本群中所有的随抽组（慎用）：随抽组清空
 清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>
+
+注意：
+随抽内容必须配合文本描述，不能只是图片。
+批量添加待抽内容不支持图片批量，如果你硬这么用，就都是重复的图片。
+随抽删除只需要传入文本内容即可，不需要图片。
+查看随抽列表只返回文本内容。
+图片用的是tx的图床，所以一段时间后会挂。
 ```
 
 ### 其他命令懒得写了，直接看图吧
 ![](docs/result.png)
+![](docs/result2.png)
 
 ## ⚙ 拓展
  
 
 ## 📝 更新日志
 
 <details>
@@ -119,14 +127,18 @@
 
 - 插件初次发布  
 
 ### 0.0.2
 
 - 增加批量添加和删除内容的功能
 
+### 0.1.0
+
+- 增加 图片内容的兼容（仅单个添加的情况，必须配合文本描述）
+
 </details>
 
 ## 致谢
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
 
 ## 项目打包上传至pypi
```

#### html2text {}

```diff
@@ -34,19 +34,26 @@
 å é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½å é¤
 <ç»å·> <åå®¹> å é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤ <ç»å·>
 æ¥çæ¬ç¾¤ææçéæ½ç»åå®¹ï¼å«ç»å·åç»åï¼ï¼éæ½ç»åè¡¨
 æ¥çæå®ç»å·çææå¾æ½åå®¹ï¼éæ½åè¡¨ <ç»å·>
 å¨æå®éæ½ç»ä¸­éæºæ½åä¸ä¸ªå¾æ½åå®¹ï¼éæ½ <ç»å·>
 æ¸ç©ºæ¬ç¾¤ä¸­ææçéæ½ç»ï¼æç¨ï¼ï¼éæ½ç»æ¸ç©º
 æ¸ç©ºæå®éæ½ç»ä¸­ææçå¾æ½åå®¹ï¼æç¨ï¼ï¼éæ½æ¸ç©º
-<ç»å·> ``` ### å¶ä»å½ä»¤æå¾åäºï¼ç´æ¥çå¾å§ ![](docs/
-result.png) ## â æå± ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
-æä»¶åæ¬¡åå¸ ### 0.0.2 - å¢å æ¹éæ·»å åå é¤åå®¹çåè½  ##
-è´è°¢ - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-
-template) ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
+<ç»å·> æ³¨æï¼ éæ½åå®¹å¿é¡»éåææ¬æè¿°ï¼ä¸è½åªæ¯å¾çã
+æ¹éæ·»å å¾æ½åå®¹ä¸æ¯æå¾çæ¹éï¼å¦æä½ ç¡¬è¿ä¹ç¨ï¼å°±é½æ¯éå¤çå¾çã
+éæ½å é¤åªéè¦ä¼ å¥ææ¬åå®¹å³å¯ï¼ä¸éè¦å¾çã
+æ¥çéæ½åè¡¨åªè¿åææ¬åå®¹ã
+å¾çç¨çæ¯txçå¾åºï¼æä»¥ä¸æ®µæ¶é´åä¼æã ``` ###
+å¶ä»å½ä»¤æå¾åäºï¼ç´æ¥çå¾å§ ![](docs/result.png) ![](docs/
+result2.png) ## â æå± ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
+æä»¶åæ¬¡åå¸ ### 0.0.2 - å¢å æ¹éæ·»å åå é¤åå®¹çåè½ ###
+0.1.0 - å¢å 
+å¾çåå®¹çå¼å®¹ï¼ä»åä¸ªæ·»å çæåµï¼å¿é¡»éåææ¬æè¿°ï¼
+## è´è°¢ - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-
+plugin-template) ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
 ``` [distutils] index-servers=pypi [pypi] repository = https://upload.pypi.org/
 legacy/ username = ç¨æ·å password = å¯ç  ``` ### poetry ``` # åè
 https://www.freesion.com/article/58051228882/ # poetry config pypi-token.pypi #
 1ãå®è£poetry pip install poetry #
 2ãåå§åéç½®æä»¶ï¼æ ¹æ®æç¤ºå¡«åï¼ poetry init #
 3ãå¾®è°éç½®æä»¶pyproject.toml # 4ãè¿è¡ poetry install, å¯çæ
```

### Comparing `nonebot_plugin_random_draw-0.0.2/setup.py` & `nonebot_plugin_random_draw-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,219 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-random-draw
+Version: 0.1.0
+Summary: 通过添加各种想要抽取的内容，最后进行随机抽取。
+Home-page: https://github.com/Ikaros-521/nonebot_plugin_random_draw
+License: MIT
+Author: Ikaros
+Author-email: 327209194@qq.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0b5,<3.0.0)
+Project-URL: Documentation, https://github.com/Ikaros-521/nonebot_plugin_random_draw/blob/master/README.md
+Project-URL: Repository, https://github.com/Ikaros-521/nonebot_plugin_random_draw
+Description-Content-Type: text/markdown
+
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_random_draw
+
+_✨ NoneBot 随机抽取设定内容 插件 ✨_
+
+
+<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/stargazers">
+    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_random_draw?color=%09%2300BFFF&style=flat-square">
+</a>
+<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/issues">
+    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_random_draw?color=Emerald%20green&style=flat-square">
+</a>
+<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/network">
+    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_random_draw?color=%2300BFFF&style=flat-square">
+</a>
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_random_draw.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_random_draw">
+    <img src="https://img.shields.io/pypi/v/nonebot_plugin_random_draw.svg" alt="pypi">
+</a>
+<a href="https://www.python.org">
+    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</a>
+
+</div>
+
+## 📖 介绍
+
+通过添加各种想要抽取的内容，最后进行随机抽取。  
+
+## 🔧 开发环境
+Nonebot2：2.0.0rc3  
+python：3.8.13  
+操作系统：Windows10（Linux兼容性问题不大）  
+编辑器：VS Code  
+
+## 💿 安装  
+
+### 1. nb-cli安装
+
+在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  
+```
+nb plugin install nonebot_plugin_random_draw
+```
+
+### 2. 本地安装
+
+将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_random_draw`文件夹里的内容拷贝至上一级目录即可。  
+clone命令参考（得先装`git`，懂的都懂）：
+```
+git clone https://github.com/Ikaros-521/nonebot_plugin_random_draw.git
+``` 
+也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_random_draw`至上一级目录。  
+目录结构： ```你的bot/src/plugins/nonebot_plugin_random_draw/__init__.py```  
+
+
+### 3. pip安装
+```
+pip install nonebot_plugin_random_draw
+```  
+打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  
+```nonebot.load_plugin('nonebot_plugin_random_draw')```  
+当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_random_draw```即可  
+pyproject.toml配置例如：  
+``` 
+[tool.nonebot]
+plugin_dirs = ["src/plugins"]
+plugins = ["nonebot_plugin_random_draw"]
+``` 
+
+
+## 🔧 配置
+
+
+## 🎉 功能
+  
+
+## 👉 命令
+
+### /随抽帮助
+命令结构：```/随抽帮助```  
+例如：```/随抽帮助```  
+功能：返回所有命令的使用方式。  
+bot返回内容：  
+```
+功能说明：命令列表（命令前缀自行匹配）
+获取帮助：随抽帮助
+创建随抽组，一个群可以有多个组：随抽组创建 <组名>
+往指定的随抽组中添加待抽内容（可多个，用空格分隔）：随抽添加 <组号> <内容>
+删除指定随抽组中的待抽内容（可多个，用空格分隔）：随抽删除 <组号> <内容>
+删除指定组号的随抽组：随抽组删除 <组号>
+查看本群所有的随抽组内容（含组号和组名）：随抽组列表
+查看指定组号的所有待抽内容：随抽列表 <组号>
+在指定随抽组中随机抽取一个待抽内容：随抽 <组号>
+清空本群中所有的随抽组（慎用）：随抽组清空
+清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>
+
+注意：
+随抽内容必须配合文本描述，不能只是图片。
+批量添加待抽内容不支持图片批量，如果你硬这么用，就都是重复的图片。
+随抽删除只需要传入文本内容即可，不需要图片。
+查看随抽列表只返回文本内容。
+图片用的是tx的图床，所以一段时间后会挂。
+```
+
+### 其他命令懒得写了，直接看图吧
+![](docs/result.png)
+![](docs/result2.png)
+
+## ⚙ 拓展
+ 
+
+## 📝 更新日志
+
+<details>
+<summary>展开/收起</summary>
+
+### 0.0.1
+
+- 插件初次发布  
+
+### 0.0.2
+
+- 增加批量添加和删除内容的功能
+
+### 0.1.0
+
+- 增加 图片内容的兼容（仅单个添加的情况，必须配合文本描述）
+
+</details>
+
+## 致谢
+- [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)
+
+## 项目打包上传至pypi
+
+官网：https://pypi.org，注册账号，在系统用户根目录下创建`.pypirc`，配置  
+``` 
+[distutils] 
+index-servers=pypi 
+ 
+[pypi] repository = https://upload.pypi.org/legacy/ 
+username = 用户名 
+password = 密码
+```
+
+### poetry
+
+```
+# 参考 https://www.freesion.com/article/58051228882/
+# poetry config pypi-token.pypi
+
+# 1、安装poetry
+pip install poetry
+
+# 2、初始化配置文件（根据提示填写）
+poetry init
+
+# 3、微调配置文件pyproject.toml
+
+# 4、运行 poetry install, 可生成 “poetry.lock” 文件（可跳过）
+poetry install
+
+# 5、编译，生成dist
+poetry build
+
+# 6、发布(poetry config pypi-token.pypi 配置token)
+poetry publish
+
+```
+
+### twine
+
+```
+# 参考 https://www.cnblogs.com/danhuai/p/14915042.html
+#创建setup.py文件 填写相关信息
+
+# 1、可以先升级打包工具
+pip install --upgrade setuptools wheel twine
+
+# 2、打包
+python setup.py sdist bdist_wheel
+
+# 3、可以先检查一下包
+twine check dist/*
+
+# 4、上传包到pypi（需输入用户名、密码）
+twine upload dist/*
+```
 
-packages = \
-['nonebot_plugin_random_draw']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['nonebot-adapter-onebot>=2.1.3,<3.0.0', 'nonebot2>=2.0.0b5,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-random-draw',
-    'version': '0.0.2',
-    'description': '通过添加各种想要抽取的内容，最后进行随机抽取。',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_random_draw\n\n_✨ NoneBot 随机抽取设定内容 插件 ✨_\n\n\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/stargazers">\n    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_random_draw?color=%09%2300BFFF&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/issues">\n    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_random_draw?color=Emerald%20green&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_draw/network">\n    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_random_draw?color=%2300BFFF&style=flat-square">\n</a>\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_random_draw.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_random_draw">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_random_draw.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</a>\n\n</div>\n\n## 📖 介绍\n\n通过添加各种想要抽取的内容，最后进行随机抽取。  \n\n## 🔧 开发环境\nNonebot2：2.0.0rc3  \npython：3.8.13  \n操作系统：Windows10（Linux兼容性问题不大）  \n编辑器：VS Code  \n\n## 💿 安装  \n\n### 1. nb-cli安装\n\n在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  \n```\nnb plugin install nonebot_plugin_random_draw\n```\n\n### 2. 本地安装\n\n将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_random_draw`文件夹里的内容拷贝至上一级目录即可。  \nclone命令参考（得先装`git`，懂的都懂）：\n```\ngit clone https://github.com/Ikaros-521/nonebot_plugin_random_draw.git\n``` \n也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_random_draw`至上一级目录。  \n目录结构： ```你的bot/src/plugins/nonebot_plugin_random_draw/__init__.py```  \n\n\n### 3. pip安装\n```\npip install nonebot_plugin_random_draw\n```  \n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_random_draw\')```  \n当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_random_draw```即可  \npyproject.toml配置例如：  \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_random_draw"]\n``` \n\n\n## 🔧 配置\n\n\n## 🎉 功能\n  \n\n## 👉 命令\n\n### /随抽帮助\n命令结构：```/随抽帮助```  \n例如：```/随抽帮助```  \n功能：返回所有命令的使用方式。  \nbot返回内容：  \n```\n功能说明：命令列表（命令前缀自行匹配）\n获取帮助：随抽帮助\n创建随抽组，一个群可以有多个组：随抽组创建 <组名>\n往指定的随抽组中添加待抽内容（可多个，用空格分隔）：随抽添加 <组号> <内容>\n删除指定随抽组中的待抽内容（可多个，用空格分隔）：随抽删除 <组号> <内容>\n删除指定组号的随抽组：随抽组删除 <组号>\n查看本群所有的随抽组内容（含组号和组名）：随抽组列表\n查看指定组号的所有待抽内容：随抽列表 <组号>\n在指定随抽组中随机抽取一个待抽内容：随抽 <组号>\n清空本群中所有的随抽组（慎用）：随抽组清空\n清空指定随抽组中所有的待抽内容（慎用）：随抽清空 <组号>\n```\n\n### 其他命令懒得写了，直接看图吧\n![](docs/result.png)\n\n## ⚙ 拓展\n \n\n## 📝 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.0.1\n\n- 插件初次发布  \n\n### 0.0.2\n\n- 增加批量添加和删除内容的功能\n\n</details>\n\n## 致谢\n- [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template)\n\n## 项目打包上传至pypi\n\n官网：https://pypi.org，注册账号，在系统用户根目录下创建`.pypirc`，配置  \n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://upload.pypi.org/legacy/ \nusername = 用户名 \npassword = 密码\n```\n\n### poetry\n\n```\n# 参考 https://www.freesion.com/article/58051228882/\n# poetry config pypi-token.pypi\n\n# 1、安装poetry\npip install poetry\n\n# 2、初始化配置文件（根据提示填写）\npoetry init\n\n# 3、微调配置文件pyproject.toml\n\n# 4、运行 poetry install, 可生成 “poetry.lock” 文件（可跳过）\npoetry install\n\n# 5、编译，生成dist\npoetry build\n\n# 6、发布(poetry config pypi-token.pypi 配置token)\npoetry publish\n\n```\n\n### twine\n\n```\n# 参考 https://www.cnblogs.com/danhuai/p/14915042.html\n#创建setup.py文件 填写相关信息\n\n# 1、可以先升级打包工具\npip install --upgrade setuptools wheel twine\n\n# 2、打包\npython setup.py sdist bdist_wheel\n\n# 3、可以先检查一下包\ntwine check dist/*\n\n# 4、上传包到pypi（需输入用户名、密码）\ntwine upload dist/*\n```\n',
-    'author': 'Ikaros',
-    'author_email': '327209194@qq.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Ikaros-521/nonebot_plugin_random_draw',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,73 +1,80 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_random_draw'] package_data = \ {'': ['*']} install_requires =
-\ ['nonebot-adapter-onebot>=2.1.3,<3.0.0', 'nonebot2>=2.0.0b5,<3.0.0']
-setup_kwargs = { 'name': 'nonebot-plugin-random-draw', 'version': '0.0.2',
-'description':
-'éè¿æ·»å åç§æ³è¦æ½åçåå®¹ï¼æåè¿è¡éæºæ½åã',
-'long_description': '
-                           \n [NoneBotPluginLogo]\n
-                                      \n
+Metadata-Version: 2.1 Name: nonebot-plugin-random-draw Version: 0.1.0 Summary:
+éè¿æ·»å åç§æ³è¦æ½åçåå®¹ï¼æåè¿è¡éæºæ½åã Home-
+page: https://github.com/Ikaros-521/nonebot_plugin_random_draw License: MIT
+Author: Ikaros Author-email: 327209194@qq.com Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2
+(>=2.0.0b5,<3.0.0) Project-URL: Documentation, https://github.com/Ikaros-521/
+nonebot_plugin_random_draw/blob/master/README.md Project-URL: Repository,
+https://github.com/Ikaros-521/nonebot_plugin_random_draw Description-Content-
+Type: text/markdown
+                             [NoneBotPluginLogo]
                               [NoneBotPluginText]
-                                      \n
-\n\n
-   \n\n# nonebot_plugin_random_draw\n\n_â¨ NoneBot éæºæ½åè®¾å®åå®¹
-    æä»¶ â¨_\n\n\n\n_[GitHub_stars]\n\n\n_[GitHub_issues]\n\n\n_[GitHub
-           forks]\n\n\n_[license]\n\n\n_[pypi]\n\n\n_[python]\n\n\n
-\n\n## ð
-ä»ç»\n\néè¿æ·»å åç§æ³è¦æ½åçåå®¹ï¼æåè¿è¡éæºæ½åã
-\n\n## ð§ å¼åç¯å¢\nNonebot2ï¼2.0.0rc3 \npythonï¼3.8.13
-\næä½ç³»ç»ï¼Windows10ï¼Linuxå¼å®¹æ§é®é¢ä¸å¤§ï¼ \nç¼è¾å¨ï¼VS
-Code \n\n## ð¿ å®è£ \n\n### 1. nb-
-cliå®è£\n\nå¨ä½ botå·¥ç¨çæä»¶å¤¹ä¸ï¼è¿è¡cmdï¼è¿è¡è·¯å¾è¦å¯¹åï¼ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
-\n```\nnb plugin install nonebot_plugin_random_draw\n```\n\n### 2.
-æ¬å°å®è£\n\nå°é¡¹ç®cloneå°ä½ çæºå¨äººæä»¶ä¸çå¯¹åºæä»¶ç®å½åï¼ä¸è¬ä¸ºæºå¨äººæä»¶å¤¹ä¸ç`src/
+# nonebot_plugin_random_draw _â¨ NoneBot éæºæ½åè®¾å®åå®¹ æä»¶ â¨_
+    [GitHub_stars] [GitHub_issues] [GitHub_forks] [license] [pypi] [python]
+## ð ä»ç»
+éè¿æ·»å åç§æ³è¦æ½åçåå®¹ï¼æåè¿è¡éæºæ½åã ## ð§
+å¼åç¯å¢ Nonebot2ï¼2.0.0rc3 pythonï¼3.8.13
+æä½ç³»ç»ï¼Windows10ï¼Linuxå¼å®¹æ§é®é¢ä¸å¤§ï¼ ç¼è¾å¨ï¼VS Code ##
+ð¿ å®è£ ### 1. nb-cliå®è£
+å¨ä½ botå·¥ç¨çæä»¶å¤¹ä¸ï¼è¿è¡cmdï¼è¿è¡è·¯å¾è¦å¯¹åï¼ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
+``` nb plugin install nonebot_plugin_random_draw ``` ### 2. æ¬å°å®è£
+å°é¡¹ç®cloneå°ä½ çæºå¨äººæä»¶ä¸çå¯¹åºæä»¶ç®å½åï¼ä¸è¬ä¸ºæºå¨äººæä»¶å¤¹ä¸ç`src/
 plugins`ï¼ï¼ç¶åæ`nonebot_plugin_random_draw`æä»¶å¤¹éçåå®¹æ·è´è³ä¸ä¸çº§ç®å½å³å¯ã
-\ncloneå½ä»¤åèï¼å¾åè£`git`ï¼æçé½æï¼ï¼\n```\ngit clone
-https://github.com/Ikaros-521/nonebot_plugin_random_draw.git\n```
-\nä¹å¯ä»¥ç´æ¥ä¸è½½åç¼©åå°æä»¶ç®å½è§£åï¼ç¶ååæ ·æå`nonebot_plugin_random_draw`è³ä¸ä¸çº§ç®å½ã
-\nç®å½ç»æï¼ ```ä½ çbot/src/plugins/nonebot_plugin_random_draw/
-__init__.py``` \n\n\n### 3. pipå®è£\n```\npip install
-nonebot_plugin_random_draw\n``` \næå¼ nonebot2 é¡¹ç®ç ```bot.py```
-æä»¶, å¨å¶ä¸­åå¥ \n```nonebot.load_plugin
-(\'nonebot_plugin_random_draw\')``` \nå½ç¶ï¼å¦ææ¯é»è®¤nb-
+cloneå½ä»¤åèï¼å¾åè£`git`ï¼æçé½æï¼ï¼ ``` git clone https://
+github.com/Ikaros-521/nonebot_plugin_random_draw.git ```
+ä¹å¯ä»¥ç´æ¥ä¸è½½åç¼©åå°æä»¶ç®å½è§£åï¼ç¶ååæ ·æå`nonebot_plugin_random_draw`è³ä¸ä¸çº§ç®å½ã
+ç®å½ç»æï¼ ```ä½ çbot/src/plugins/nonebot_plugin_random_draw/
+__init__.py``` ### 3. pipå®è£ ``` pip install nonebot_plugin_random_draw ```
+æå¼ nonebot2 é¡¹ç®ç ```bot.py``` æä»¶, å¨å¶ä¸­åå¥
+```nonebot.load_plugin('nonebot_plugin_random_draw')```
+å½ç¶ï¼å¦ææ¯é»è®¤nb-
 cliåå»ºçnonebot2çè¯ï¼å¨botè·¯å¾```pyproject.toml```ç```
 [tool.nonebot]```ç```plugins```ä¸­æ·»å ```nonebot_plugin_random_draw```å³å¯
-\npyproject.tomléç½®ä¾å¦ï¼ \n``` \n[tool.nonebot]\nplugin_dirs = ["src/
-plugins"]\nplugins = ["nonebot_plugin_random_draw"]\n``` \n\n\n## ð§
-éç½®\n\n\n## ð åè½\n \n\n## ð å½ä»¤\n\n### /
-éæ½å¸®å©\nå½ä»¤ç»æï¼```/éæ½å¸®å©``` \nä¾å¦ï¼```/éæ½å¸®å©```
-\nåè½ï¼è¿åææå½ä»¤çä½¿ç¨æ¹å¼ã \nbotè¿ååå®¹ï¼
-\n```\nåè½è¯´æï¼å½ä»¤åè¡¨ï¼å½ä»¤åç¼èªè¡å¹éï¼\nè·åå¸®å©ï¼éæ½å¸®å©\nåå»ºéæ½ç»ï¼ä¸ä¸ªç¾¤å¯ä»¥æå¤ä¸ªç»ï¼éæ½ç»åå»º
-<ç»å>\nå¾æå®çéæ½ç»ä¸­æ·»å å¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½æ·»å 
-<ç»å·>
-<åå®¹>\nå é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½å é¤
-<ç»å·> <åå®¹>\nå é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤
-<ç»å·>\næ¥çæ¬ç¾¤ææçéæ½ç»åå®¹ï¼å«ç»å·åç»åï¼ï¼éæ½ç»åè¡¨\næ¥çæå®ç»å·çææå¾æ½åå®¹ï¼éæ½åè¡¨
-<ç»å·>\nå¨æå®éæ½ç»ä¸­éæºæ½åä¸ä¸ªå¾æ½åå®¹ï¼éæ½
-<ç»å·>\næ¸ç©ºæ¬ç¾¤ä¸­ææçéæ½ç»ï¼æç¨ï¼ï¼éæ½ç»æ¸ç©º\næ¸ç©ºæå®éæ½ç»ä¸­ææçå¾æ½åå®¹ï¼æç¨ï¼ï¼éæ½æ¸ç©º
-<ç»å·>\n```\n\n### å¶ä»å½ä»¤æå¾åäºï¼ç´æ¥çå¾å§\n![](docs/
-result.png)\n\n## â æå±\n \n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
-æ¶èµ·\n\n### 0.0.1\n\n- æä»¶åæ¬¡åå¸ \n\n### 0.0.2\n\n-
-å¢å æ¹éæ·»å åå é¤åå®¹çåè½\n\n\n\n## è´è°¢\n- [nonebot-plugin-
-template](https://github.com/A-kirami/nonebot-plugin-template)\n\n##
-é¡¹ç®æåä¸ä¼ è³pypi\n\nå®ç½ï¼https://
+pyproject.tomléç½®ä¾å¦ï¼ ``` [tool.nonebot] plugin_dirs = ["src/plugins"]
+plugins = ["nonebot_plugin_random_draw"] ``` ## ð§ éç½® ## ð åè½ ##
+ð å½ä»¤ ### /éæ½å¸®å© å½ä»¤ç»æï¼```/éæ½å¸®å©``` ä¾å¦ï¼```/
+éæ½å¸®å©``` åè½ï¼è¿åææå½ä»¤çä½¿ç¨æ¹å¼ã
+botè¿ååå®¹ï¼ ```
+åè½è¯´æï¼å½ä»¤åè¡¨ï¼å½ä»¤åç¼èªè¡å¹éï¼
+è·åå¸®å©ï¼éæ½å¸®å©
+åå»ºéæ½ç»ï¼ä¸ä¸ªç¾¤å¯ä»¥æå¤ä¸ªç»ï¼éæ½ç»åå»º <ç»å>
+å¾æå®çéæ½ç»ä¸­æ·»å å¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½æ·»å 
+<ç»å·> <åå®¹>
+å é¤æå®éæ½ç»ä¸­çå¾æ½åå®¹ï¼å¯å¤ä¸ªï¼ç¨ç©ºæ ¼åéï¼ï¼éæ½å é¤
+<ç»å·> <åå®¹> å é¤æå®ç»å·çéæ½ç»ï¼éæ½ç»å é¤ <ç»å·>
+æ¥çæ¬ç¾¤ææçéæ½ç»åå®¹ï¼å«ç»å·åç»åï¼ï¼éæ½ç»åè¡¨
+æ¥çæå®ç»å·çææå¾æ½åå®¹ï¼éæ½åè¡¨ <ç»å·>
+å¨æå®éæ½ç»ä¸­éæºæ½åä¸ä¸ªå¾æ½åå®¹ï¼éæ½ <ç»å·>
+æ¸ç©ºæ¬ç¾¤ä¸­ææçéæ½ç»ï¼æç¨ï¼ï¼éæ½ç»æ¸ç©º
+æ¸ç©ºæå®éæ½ç»ä¸­ææçå¾æ½åå®¹ï¼æç¨ï¼ï¼éæ½æ¸ç©º
+<ç»å·> æ³¨æï¼ éæ½åå®¹å¿é¡»éåææ¬æè¿°ï¼ä¸è½åªæ¯å¾çã
+æ¹éæ·»å å¾æ½åå®¹ä¸æ¯æå¾çæ¹éï¼å¦æä½ ç¡¬è¿ä¹ç¨ï¼å°±é½æ¯éå¤çå¾çã
+éæ½å é¤åªéè¦ä¼ å¥ææ¬åå®¹å³å¯ï¼ä¸éè¦å¾çã
+æ¥çéæ½åè¡¨åªè¿åææ¬åå®¹ã
+å¾çç¨çæ¯txçå¾åºï¼æä»¥ä¸æ®µæ¶é´åä¼æã ``` ###
+å¶ä»å½ä»¤æå¾åäºï¼ç´æ¥çå¾å§ ![](docs/result.png) ![](docs/
+result2.png) ## â æå± ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
+æä»¶åæ¬¡åå¸ ### 0.0.2 - å¢å æ¹éæ·»å åå é¤åå®¹çåè½ ###
+0.1.0 - å¢å 
+å¾çåå®¹çå¼å®¹ï¼ä»åä¸ªæ·»å çæåµï¼å¿é¡»éåææ¬æè¿°ï¼
+## è´è°¢ - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-
+plugin-template) ## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
-\n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://
-upload.pypi.org/legacy/ \nusername = ç¨æ·å \npassword = å¯ç \n```\n\n###
-poetry\n\n```\n# åè https://www.freesion.com/article/58051228882/\n# poetry
-config pypi-token.pypi\n\n# 1ãå®è£poetry\npip install poetry\n\n#
-2ãåå§åéç½®æä»¶ï¼æ ¹æ®æç¤ºå¡«åï¼\npoetry init\n\n#
-3ãå¾®è°éç½®æä»¶pyproject.toml\n\n# 4ãè¿è¡ poetry install, å¯çæ
-âpoetry.lockâ æä»¶ï¼å¯è·³è¿ï¼\npoetry install\n\n#
-5ãç¼è¯ï¼çædist\npoetry build\n\n# 6ãåå¸(poetry config pypi-
-token.pypi éç½®token)\npoetry publish\n\n```\n\n### twine\n\n```\n# åè
-https://www.cnblogs.com/danhuai/p/14915042.html\n#åå»ºsetup.pyæä»¶
-å¡«åç¸å³ä¿¡æ¯\n\n# 1ãå¯ä»¥ååçº§æåå·¥å·\npip install --upgrade
-setuptools wheel twine\n\n# 2ãæå\npython setup.py sdist bdist_wheel\n\n#
-3ãå¯ä»¥åæ£æ¥ä¸ä¸å\ntwine check dist/*\n\n#
-4ãä¸ä¼ åå°pypiï¼éè¾å¥ç¨æ·åãå¯ç ï¼\ntwine upload dist/
-*\n```\n', 'author': 'Ikaros', 'author_email': '327209194@qq.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-Ikaros-521/nonebot_plugin_random_draw', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.8,<4.0', } setup(**setup_kwargs)
+``` [distutils] index-servers=pypi [pypi] repository = https://upload.pypi.org/
+legacy/ username = ç¨æ·å password = å¯ç  ``` ### poetry ``` # åè
+https://www.freesion.com/article/58051228882/ # poetry config pypi-token.pypi #
+1ãå®è£poetry pip install poetry #
+2ãåå§åéç½®æä»¶ï¼æ ¹æ®æç¤ºå¡«åï¼ poetry init #
+3ãå¾®è°éç½®æä»¶pyproject.toml # 4ãè¿è¡ poetry install, å¯çæ
+âpoetry.lockâ æä»¶ï¼å¯è·³è¿ï¼ poetry install #
+5ãç¼è¯ï¼çædist poetry build # 6ãåå¸(poetry config pypi-token.pypi
+éç½®token) poetry publish ``` ### twine ``` # åè https://www.cnblogs.com/
+danhuai/p/14915042.html #åå»ºsetup.pyæä»¶ å¡«åç¸å³ä¿¡æ¯ #
+1ãå¯ä»¥ååçº§æåå·¥å· pip install --upgrade setuptools wheel twine #
+2ãæå python setup.py sdist bdist_wheel # 3ãå¯ä»¥åæ£æ¥ä¸ä¸å
+twine check dist/* # 4ãä¸ä¼ åå°pypiï¼éè¾å¥ç¨æ·åãå¯ç ï¼
+twine upload dist/* ```
```

