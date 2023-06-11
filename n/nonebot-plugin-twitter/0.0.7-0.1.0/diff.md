# Comparing `tmp/nonebot-plugin-twitter-0.0.7.tar.gz` & `tmp/nonebot-plugin-twitter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.0.7.tar", last modified: Tue Jun  6 06:04:27 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.1.0.tar", last modified: Sun Jun 11 04:43:29 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.0.7.tar` & `nonebot-plugin-twitter-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-06 06:04:17.925635 nonebot-plugin-twitter-0.0.7/LICENSE
--rw-r--r--   0        0        0     3405 2023-06-06 06:04:17.925635 nonebot-plugin-twitter-0.0.7/README.md
--rw-r--r--   0        0        0    17458 2023-06-06 06:04:17.929635 nonebot-plugin-twitter-0.0.7/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     1252 2023-06-06 06:04:17.929635 nonebot-plugin-twitter-0.0.7/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      646 2023-06-06 06:04:17.929635 nonebot-plugin-twitter-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3244 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/README.md
+-rw-r--r--   0        0        0    14094 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     4549 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/api.py
+-rw-r--r--   0        0        0     1582 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      624 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.0/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.0.7/LICENSE` & `nonebot-plugin-twitter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.0.7/README.md` & `nonebot-plugin-twitter-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -65,41 +65,44 @@
 
     plugins = ["nonebot_plugin_twitter"]
 
 </details>
 
 ## ⚙️ 配置
 
-申请 [twitter api](https://developer.twitter.com/zh-cn/docs/twitter-ads-api/getting-started) 权限
-
-创建一个 Project ，生成并记录 API Key 和 [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
-
-[![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0)
  
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bearer_token | 是 | 无 | Bearer Token |
+| twitter_website | 否 | 无 | 自定义website |
 | twitter_proxy | 否 | 无 | proxy |
-| twitter_debug | 否 | False | debug模式 |
+| twitter_qq | 否 | 2854196310 | 合并消息头像来源 |
 | command_priority | 否 | 10 | 命令优先级 |
 
-[![pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)](https://imgse.com/i/pCPq2Hs)
+配置格式示例
+```bash
+#twitter
+twitter_proxy="http://127.0.0.1:1090"
+twitter_qq=2854196306
+command_priority=10
+```
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18]” r18为可选参数，不开启和默认为不推送r18推文|
 | 取关推主 | 无 | 否 | 群聊/私聊 | 取关切割 |
 | 推主列表 | 无 | 否 | 群聊/私聊 | 展示列表 |
-| 推特推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
-| 推特推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
+| 推文推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
+| 推文推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
 ### 效果图
 [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV)
 [![pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT)
 ### 注意事项
 1.推主id：
 [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
 
 2.消息为合并转发发送，存在延迟和发送失败的可能
+
+3.新的0.1.0版本为破坏性更新：代理配置格式更改，关注列表需重新关注。
```

#### html2text {}

```diff
@@ -7,30 +7,28 @@
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-twitter
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
 poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
 twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
-âï¸ éç½® ç³è¯· [twitter api](https://developer.twitter.com/zh-cn/docs/
-twitter-ads-api/getting-started) æé åå»ºä¸ä¸ª Project ï¼çæå¹¶è®°å½
-API Key å [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
-[![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/
-i/pCPufJ0) å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
-| éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-bearer_token | æ¯ | æ  | Bearer Token | | twitter_proxy | å¦ | æ  | proxy |
-| twitter_debug | å¦ | False | debugæ¨¡å¼ | | command_priority | å¦ | 10 |
-å½ä»¤ä¼åçº§ | [![pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)]
-(https://imgse.com/i/pCPq2Hs) ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
-éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
-å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
+âï¸ éç½® å¨ nonebot2
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
+é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | twitter_website | å¦ |
+æ  | èªå®ä¹website | | twitter_proxy | å¦ | æ  | proxy | | twitter_qq |
+å¦ | 2854196310 | åå¹¶æ¶æ¯å¤´åæ¥æº | | command_priority | å¦ | 10 |
+å½ä»¤ä¼åçº§ | éç½®æ ¼å¼ç¤ºä¾ ```bash #twitter twitter_proxy="http://
+127.0.0.1:1090" twitter_qq=2854196306 command_priority=10 ``` ## ð ä½¿ç¨
+### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:
+----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
 å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
 r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
 æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
-ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
-å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
+ç§è | å±ç¤ºåè¡¨ | | æ¨ææ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
+å³é­æ¨é | | æ¨ææ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
 pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
 2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
 1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)]
 (https://imgse.com/i/pCPMu36)
 2.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
+3.æ°ç0.1.0çæ¬ä¸ºç ´åæ§æ´æ°ï¼ä»£çéç½®æ ¼å¼æ´æ¹ï¼å³æ³¨åè¡¨ééæ°å³æ³¨ã
```

### Comparing `nonebot-plugin-twitter-0.0.7/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 from pydantic import BaseModel,validator
 from typing import Optional
 from nonebot.log import logger
+from nonebot import get_driver
 import sys
 
 if sys.version_info < (3, 10):
     from importlib_metadata import version
 else:
     from importlib.metadata import version
 
 try:
     __version__ = version("nonebot_plugin_bilichat")
 except Exception:
     __version__ = None
 
 class Config(BaseModel):
-    bearer_token: Optional[str] = ""
-    twitter_proxy: Optional[str] = ""
+    twitter_website: Optional[str] = ""
+    twitter_proxy: Optional[str] = None
+    twitter_url: Optional[str] = ""
+    twitter_qq: int = 2854196310
     command_priority: int = 10
     plugin_enabled: bool = True
-    twitter_debug: bool = False
     
-    @validator("bearer_token")
-    def check_bearer_token(cls,v):
+    @validator("twitter_website")
+    def check_twitter_website(cls,v):
         if isinstance(v,str):
-            logger.info("bearer_token 读取成功")
+            logger.info("twitter_website 读取成功")
             return v
     @validator("twitter_proxy")
     def check_proxy(cls,v):
         if isinstance(v,str):
             logger.info("twitter_proxy 读取成功")
             return v
+    @validator("twitter_qq")
+    def check_twitter_qq(cls,v):
+        if isinstance(v,int):
+            logger.info("twitter_qq 读取成功")
+            return v
         
     @validator("command_priority")
     def check_command_priority(cls,v):
         if isinstance(v,int) and v >= 1:
             logger.info("command_priority 读取成功")
             return v
-    
-    @validator("twitter_debug")
-    def check_twitter_debug(cls,v):
-        if isinstance(v,bool):
-            logger.info("twitter_debug 开启成功")
-            return v
+        
+config_dev = Config.parse_obj(get_driver().config)
+
+website_list = [
+    "https://twitter.owacon.moe",
+    "https://nitter.unixfox.eu",
+    "https://nitter.1d4.us/",
+    "https://nitter.it/",
+    "https://bird.trom.tf/",
+    "https://nitter.moomoo.me/"
+]
```

### Comparing `nonebot-plugin-twitter-0.0.7/pyproject.toml` & `nonebot-plugin-twitter-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.0.7"
+version = "0.1.0"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
     "httpx>=0.23.0",
-    "tweepy>=4.14.0",
     "nonebot_plugin_apscheduler>=0.2.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot-plugin-twitter-0.0.7/PKG-INFO` & `nonebot-plugin-twitter-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.0.7
+Version: 0.1.0
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
@@ -76,42 +76,45 @@
 
     plugins = ["nonebot_plugin_twitter"]
 
 </details>
 
 ## ⚙️ 配置
 
-申请 [twitter api](https://developer.twitter.com/zh-cn/docs/twitter-ads-api/getting-started) 权限
-
-创建一个 Project ，生成并记录 API Key 和 [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
-
-[![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/i/pCPufJ0)
  
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bearer_token | 是 | 无 | Bearer Token |
+| twitter_website | 否 | 无 | 自定义website |
 | twitter_proxy | 否 | 无 | proxy |
-| twitter_debug | 否 | False | debug模式 |
+| twitter_qq | 否 | 2854196310 | 合并消息头像来源 |
 | command_priority | 否 | 10 | 命令优先级 |
 
-[![pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)](https://imgse.com/i/pCPq2Hs)
+配置格式示例
+```bash
+#twitter
+twitter_proxy="http://127.0.0.1:1090"
+twitter_qq=2854196306
+command_priority=10
+```
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18]” r18为可选参数，不开启和默认为不推送r18推文|
 | 取关推主 | 无 | 否 | 群聊/私聊 | 取关切割 |
 | 推主列表 | 无 | 否 | 群聊/私聊 | 展示列表 |
-| 推特推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
-| 推特推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
+| 推文推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
+| 推文推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
 ### 效果图
 [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV)
 [![pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT)
 ### 注意事项
 1.推主id：
 [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
 
 2.消息为合并转发发送，存在延迟和发送失败的可能
 
+3.新的0.1.0版本为破坏性更新：代理配置格式更改，关注列表需重新关注。
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.0.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.0 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
@@ -12,30 +12,28 @@
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-twitter
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
 poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
 twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
-âï¸ éç½® ç³è¯· [twitter api](https://developer.twitter.com/zh-cn/docs/
-twitter-ads-api/getting-started) æé åå»ºä¸ä¸ª Project ï¼çæå¹¶è®°å½
-API Key å [Bearer Token](https://developer.twitter.com/en/portal/dashboard)
-[![pCPufJ0.png](https://s1.ax1x.com/2023/06/05/pCPufJ0.png)](https://imgse.com/
-i/pCPufJ0) å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
-| éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-bearer_token | æ¯ | æ  | Bearer Token | | twitter_proxy | å¦ | æ  | proxy |
-| twitter_debug | å¦ | False | debugæ¨¡å¼ | | command_priority | å¦ | 10 |
-å½ä»¤ä¼åçº§ | [![pCPq2Hs.png](https://s1.ax1x.com/2023/06/06/pCPq2Hs.png)]
-(https://imgse.com/i/pCPq2Hs) ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
-éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
-å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
+âï¸ éç½® å¨ nonebot2
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
+é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | twitter_website | å¦ |
+æ  | èªå®ä¹website | | twitter_proxy | å¦ | æ  | proxy | | twitter_qq |
+å¦ | 2854196310 | åå¹¶æ¶æ¯å¤´åæ¥æº | | command_priority | å¦ | 10 |
+å½ä»¤ä¼åçº§ | éç½®æ ¼å¼ç¤ºä¾ ```bash #twitter twitter_proxy="http://
+127.0.0.1:1090" twitter_qq=2854196306 command_priority=10 ``` ## ð ä½¿ç¨
+### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:
+----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
 å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
 r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
 æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
-ç§è | å±ç¤ºåè¡¨ | | æ¨ç¹æ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
-å³é­æ¨é | | æ¨ç¹æ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
+ç§è | å±ç¤ºåè¡¨ | | æ¨ææ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
+å³é­æ¨é | | æ¨ææ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
 å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
 pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
 2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
 1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)]
 (https://imgse.com/i/pCPMu36)
 2.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
+3.æ°ç0.1.0çæ¬ä¸ºç ´åæ§æ´æ°ï¼ä»£çéç½®æ ¼å¼æ´æ¹ï¼å³æ³¨åè¡¨ééæ°å³æ³¨ã
```

