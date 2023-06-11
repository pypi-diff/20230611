# Comparing `tmp/nonebot-plugin-twitter-0.1.0.tar.gz` & `tmp/nonebot-plugin-twitter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.1.0.tar", last modified: Sun Jun 11 04:43:29 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.1.2.tar", last modified: Sun Jun 11 06:59:29 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.1.0.tar` & `nonebot-plugin-twitter-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/LICENSE
--rw-r--r--   0        0        0     3244 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/README.md
--rw-r--r--   0        0        0    14094 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     4549 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/api.py
--rw-r--r--   0        0        0     1582 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      624 2023-06-11 04:43:21.673112 nonebot-plugin-twitter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3053 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/README.md
+-rw-r--r--   0        0        0    14094 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     4563 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/api.py
+-rw-r--r--   0        0        0     1582 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      654 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.2/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.1.0/LICENSE` & `nonebot-plugin-twitter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.0/README.md` & `nonebot-plugin-twitter-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,22 +25,14 @@
 ## 📖 介绍
 
 订阅推送 twitter 推文
 
 ## 💿 安装
 
 <details>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-twitter
-
-</details>
-
-<details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
     pip install nonebot-plugin-twitter
```

#### html2text {}

```diff
@@ -1,14 +1,12 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
                                    [python]
-## ð ä»ç» è®¢éæ¨é twitter æ¨æ ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£
-å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-twitter
+## ð ä»ç» è®¢éæ¨é twitter æ¨æ ## ð¿ å®è£
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
 poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
 twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
 âï¸ éç½® å¨ nonebot2
```

### Comparing `nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/api.py` & `nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,30 @@
     '''
     async with httpx.AsyncClient(proxies=config_dev.twitter_proxy) as client:
         res = await client.get(url=f"{config_dev.twitter_url}/{user_name}")
         result ={}
         if res.status_code ==200:
             result["status"] = True
             result["user_name"] = user_name
-            soup = BeautifulSoup(res.text,"lxml")
+            soup = BeautifulSoup(res.text,"html.parser")
             result["screen_name"] = soup.find_all('a', class_='profile-card-fullname')[0].next
             result["bio"] = soup.find_all('p')[0].text
         else:
             result["status"] = False
         
     return result
 
 async def get_user_newtimeline(user_name:str,since_id: str = "0") -> str:
     ''' 通过 user_name 获取推文id列表,
     有 since_id return 最近的新的推文id,
     无 since_id return 最新的推文id'''
     async with httpx.AsyncClient(proxies=config_dev.twitter_proxy) as client:
         res = await client.get(url=f"{config_dev.twitter_url}/{user_name}")
         if res.status_code ==200:
-            soup = BeautifulSoup(res.text,"lxml")
+            soup = BeautifulSoup(res.text,"html.parser")
             timeline_list = soup.find_all('a', class_='tweet-link')
             new_line =[]
             for x in timeline_list:
                 if user_name in x.attrs["href"]:
                     tweet_id = x.attrs["href"].split("/").pop().replace("#m","")
                     if since_id != "0":
                         if int(tweet_id) > int(since_id):
```

### Comparing `nonebot-plugin-twitter-0.1.0/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.0/PKG-INFO` & `nonebot-plugin-twitter-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.1.0
+Version: 0.1.2
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
@@ -36,22 +36,14 @@
 ## 📖 介绍
 
 订阅推送 twitter 推文
 
 ## 💿 安装
 
 <details>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-twitter
-
-</details>
-
-<details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
     pip install nonebot-plugin-twitter
```

#### html2text {}

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.2 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
                                    [python]
-## ð ä»ç» è®¢éæ¨é twitter æ¨æ ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£
-å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-twitter
+## ð ä»ç» è®¢éæ¨é twitter æ¨æ ## ð¿ å®è£
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
 poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
 twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
 âï¸ éç½® å¨ nonebot2
```

