# Comparing `tmp/nonebot_plugin_audiocraft-0.0.3.tar.gz` & `tmp/nonebot_plugin_audiocraft-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_audiocraft-0.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_audiocraft-0.0.4.tar", max compression
```

## Comparing `nonebot_plugin_audiocraft-0.0.3.tar` & `nonebot_plugin_audiocraft-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1837 2023-06-10 14:28:50.607447 nonebot_plugin_audiocraft-0.0.3/README.md
--rw-r--r--   0        0        0     6148 2023-06-10 13:04:05.827943 nonebot_plugin_audiocraft-0.0.3/nonebot_plugin_audiocraft/.DS_Store
--rw-r--r--   0        0        0     2576 2023-06-11 03:06:21.751454 nonebot_plugin_audiocraft-0.0.3/nonebot_plugin_audiocraft/__init__.py
--rw-r--r--   0        0        0      545 2023-06-11 03:06:35.889543 nonebot_plugin_audiocraft-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 nonebot_plugin_audiocraft-0.0.3/setup.py
--rw-r--r--   0        0        0     2535 1970-01-01 00:00:00.000000 nonebot_plugin_audiocraft-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1752 2023-06-11 04:58:20.222484 nonebot_plugin_audiocraft-0.0.4/README.md
+-rw-r--r--   0        0        0     6148 2023-06-10 13:04:05.827943 nonebot_plugin_audiocraft-0.0.4/nonebot_plugin_audiocraft/.DS_Store
+-rw-r--r--   0        0        0     2579 2023-06-11 04:58:30.170828 nonebot_plugin_audiocraft-0.0.4/nonebot_plugin_audiocraft/__init__.py
+-rw-r--r--   0        0        0      545 2023-06-11 04:58:44.244079 nonebot_plugin_audiocraft-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 nonebot_plugin_audiocraft-0.0.4/setup.py
+-rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 nonebot_plugin_audiocraft-0.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_audiocraft-0.0.3/README.md` & `nonebot_plugin_audiocraft-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 <div align="center">
 
 # nonebot-plugin-audiocraft
 </div>
 
 # 介绍
-- 本插件适配[Facebook开源的AI作曲模型](https://github.com/facebookresearch/audiocraft/blob/984b3755a1b37c85dcff24fb516b946ea75da4aa/audiocraft/modules/conditioners.py#L371)，在nonebot框架下调用已经部署好的模型后端服务器API进行AI作曲
+- 本插件适配[Facebook开源的AI作曲模型](https://github.com/facebookresearch/audiocraft/)，在nonebot框架下调用已经部署好的模型后端服务器API进行AI作曲
 - 本插件需要配合部署好的audiocraft进行使用
 
 # 安装
 
 * 手动安装
   ```
   git clone https://github.com/Alpaca4610/nonebot_plugin_audiocraft.git
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                           # nonebot-plugin-audiocraft
 # ä»ç» - æ¬æä»¶éé[Facebookå¼æºçAIä½æ²æ¨¡å](https://github.com/
-facebookresearch/audiocraft/blob/984b3755a1b37c85dcff24fb516b946ea75da4aa/
-audiocraft/modules/
-conditioners.py#L371)ï¼å¨nonebotæ¡æ¶ä¸è°ç¨å·²ç»é¨ç½²å¥½çæ¨¡ååç«¯æå¡å¨APIè¿è¡AIä½æ²
+facebookresearch/audiocraft/
+)ï¼å¨nonebotæ¡æ¶ä¸è°ç¨å·²ç»é¨ç½²å¥½çæ¨¡ååç«¯æå¡å¨APIè¿è¡AIä½æ²
 - æ¬æä»¶éè¦éåé¨ç½²å¥½çaudiocraftè¿è¡ä½¿ç¨ # å®è£ *
 æå¨å®è£ ``` git clone https://github.com/Alpaca4610/
 nonebot_plugin_audiocraft.git ```
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼ ```
 plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/nonebot-
 plugin-audiocraft"] ``` * ä½¿ç¨ pip ``` pip install nonebot-plugin-audiocraft
 ``` # åç«¯æå¡å¨é¨ç½² åè[å®æ¹ä»åº](https://github.com/
```

### Comparing `nonebot_plugin_audiocraft-0.0.3/nonebot_plugin_audiocraft/.DS_Store` & `nonebot_plugin_audiocraft-0.0.4/nonebot_plugin_audiocraft/.DS_Store`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_audiocraft-0.0.3/nonebot_plugin_audiocraft/__init__.py` & `nonebot_plugin_audiocraft-0.0.4/nonebot_plugin_audiocraft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     name="AI作曲",
     description="Nonebot框架下的AI作曲插件",
     usage=
     '''
     每次重启机器人后，使用 %%后端服务器地址 绑定audiocraft后端服务器。
     绑定后端服务器后，使用 AI作曲+乐曲的英文描述 即可触发AI作曲。
     ''',
-    config="",
+    config= None,
     extra={},
     type="application",
     homepage="https://github.com/Alpaca4610/nonebot-plugin-audiocraft",
     supported_adapters={"~onebot.v11"}
 )
 
 url = ""
```

### Comparing `nonebot_plugin_audiocraft-0.0.3/pyproject.toml` & `nonebot_plugin_audiocraft-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-audiocraft"
-version = "0.0.3"
+version = "0.0.4"
 description = "A nonebot plugin for facebook's audiocraft"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_audiocraft-0.0.3/setup.py` & `nonebot_plugin_audiocraft-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 install_requires = \
 ['gradio-client>=0.2.5,<0.3.0',
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-audiocraft',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': "A nonebot plugin for facebook's audiocraft",
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-audiocraft\n</div>\n\n# 介绍\n- 本插件适配[Facebook开源的AI作曲模型](https://github.com/facebookresearch/audiocraft/blob/984b3755a1b37c85dcff24fb516b946ea75da4aa/audiocraft/modules/conditioners.py#L371)，在nonebot框架下调用已经部署好的模型后端服务器API进行AI作曲\n- 本插件需要配合部署好的audiocraft进行使用\n\n# 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_audiocraft.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-audiocraft"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-audiocraft\n  ```\n# 后端服务器部署\n参考[官方仓库](https://github.com/facebookresearch/audiocraft#usage)部署好gradio后端，获得后端网址。（coblab上部署的可以开启gradio的外链分享）\n\n\n# 使用方法\n\n- 由于最近tx风控严重，go-cqhttp面临重启后可能掉账号的风险，所以插件使用给机器人发送消息配置后端服务器配置的方法。\n- 每次重启机器人后，使用 %%后端服务器地址 绑定audiocraft后端服务器。\n- 绑定后端服务器后，使用 AI作曲+乐曲的英文描述 即可触发AI作曲。\n- AI作曲的参数（如模型、时长）等通过代码进行修改，代码中有注释说明。\n\n# 效果\n\n![Alt](demo1.png)\n![Alt](demo2.png)\n',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-audiocraft\n</div>\n\n# 介绍\n- 本插件适配[Facebook开源的AI作曲模型](https://github.com/facebookresearch/audiocraft/)，在nonebot框架下调用已经部署好的模型后端服务器API进行AI作曲\n- 本插件需要配合部署好的audiocraft进行使用\n\n# 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_audiocraft.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-audiocraft"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-audiocraft\n  ```\n# 后端服务器部署\n参考[官方仓库](https://github.com/facebookresearch/audiocraft#usage)部署好gradio后端，获得后端网址。（coblab上部署的可以开启gradio的外链分享）\n\n\n# 使用方法\n\n- 由于最近tx风控严重，go-cqhttp面临重启后可能掉账号的风险，所以插件使用给机器人发送消息配置后端服务器配置的方法。\n- 每次重启机器人后，使用 %%后端服务器地址 绑定audiocraft后端服务器。\n- 绑定后端服务器后，使用 AI作曲+乐曲的英文描述 即可触发AI作曲。\n- AI作曲的参数（如模型、时长）等通过代码进行修改，代码中有注释说明。\n\n# 效果\n\n![Alt](demo1.png)\n![Alt](demo2.png)\n',
     'author': 'Alpaca',
     'author_email': 'alpaca@bupt.edu.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_audiocraft'] package_data = \ {'': ['*']} install_requires = \
 ['gradio-client>=0.2.5,<0.3.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
 'nonebot2>=2.0.0rc3,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-
-audiocraft', 'version': '0.0.3', 'description': "A nonebot plugin for
+audiocraft', 'version': '0.0.4', 'description': "A nonebot plugin for
 facebook's audiocraft", 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
                        \n\n# nonebot-plugin-audiocraft\n
 \n\n# ä»ç»\n- æ¬æä»¶éé[Facebookå¼æºçAIä½æ²æ¨¡å](https://
-github.com/facebookresearch/audiocraft/blob/
-984b3755a1b37c85dcff24fb516b946ea75da4aa/audiocraft/modules/
-conditioners.py#L371)ï¼å¨nonebotæ¡æ¶ä¸è°ç¨å·²ç»é¨ç½²å¥½çæ¨¡ååç«¯æå¡å¨APIè¿è¡AIä½æ²\n-
+github.com/facebookresearch/audiocraft/
+)ï¼å¨nonebotæ¡æ¶ä¸è°ç¨å·²ç»é¨ç½²å¥½çæ¨¡ååç«¯æå¡å¨APIè¿è¡AIä½æ²\n-
 æ¬æä»¶éè¦éåé¨ç½²å¥½çaudiocraftè¿è¡ä½¿ç¨\n\n# å®è£\n\n*
 æå¨å®è£\n ```\n git clone https://github.com/Alpaca4610/
 nonebot_plugin_audiocraft.git\n ```\n\n
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼\n\n
 ```\n plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/
 nonebot-plugin-audiocraft"]\n ```\n* ä½¿ç¨ pip\n ```\n pip install nonebot-
 plugin-audiocraft\n ```\n# åç«¯æå¡å¨é¨ç½²\nåè[å®æ¹ä»åº](https://
```

### Comparing `nonebot_plugin_audiocraft-0.0.3/PKG-INFO` & `nonebot_plugin_audiocraft-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-audiocraft
-Version: 0.0.3
+Version: 0.0.4
 Summary: A nonebot plugin for facebook's audiocraft
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 
 <div align="center">
 
 # nonebot-plugin-audiocraft
 </div>
 
 # 介绍
-- 本插件适配[Facebook开源的AI作曲模型](https://github.com/facebookresearch/audiocraft/blob/984b3755a1b37c85dcff24fb516b946ea75da4aa/audiocraft/modules/conditioners.py#L371)，在nonebot框架下调用已经部署好的模型后端服务器API进行AI作曲
+- 本插件适配[Facebook开源的AI作曲模型](https://github.com/facebookresearch/audiocraft/)，在nonebot框架下调用已经部署好的模型后端服务器API进行AI作曲
 - 本插件需要配合部署好的audiocraft进行使用
 
 # 安装
 
 * 手动安装
   ```
   git clone https://github.com/Alpaca4610/nonebot_plugin_audiocraft.git
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-audiocraft Version: 0.0.3 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-audiocraft Version: 0.0.4 Summary: A
 nonebot plugin for facebook's audiocraft License: MIT Author: Alpaca Author-
 email: alpaca@bupt.edu.cn Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: gradio-client
 (>=0.2.5,<0.3.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0) Description-Content-Type: text/
 markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                           # nonebot-plugin-audiocraft
 # ä»ç» - æ¬æä»¶éé[Facebookå¼æºçAIä½æ²æ¨¡å](https://github.com/
-facebookresearch/audiocraft/blob/984b3755a1b37c85dcff24fb516b946ea75da4aa/
-audiocraft/modules/
-conditioners.py#L371)ï¼å¨nonebotæ¡æ¶ä¸è°ç¨å·²ç»é¨ç½²å¥½çæ¨¡ååç«¯æå¡å¨APIè¿è¡AIä½æ²
+facebookresearch/audiocraft/
+)ï¼å¨nonebotæ¡æ¶ä¸è°ç¨å·²ç»é¨ç½²å¥½çæ¨¡ååç«¯æå¡å¨APIè¿è¡AIä½æ²
 - æ¬æä»¶éè¦éåé¨ç½²å¥½çaudiocraftè¿è¡ä½¿ç¨ # å®è£ *
 æå¨å®è£ ``` git clone https://github.com/Alpaca4610/
 nonebot_plugin_audiocraft.git ```
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼ ```
 plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/nonebot-
 plugin-audiocraft"] ``` * ä½¿ç¨ pip ``` pip install nonebot-plugin-audiocraft
 ``` # åç«¯æå¡å¨é¨ç½² åè[å®æ¹ä»åº](https://github.com/
```

