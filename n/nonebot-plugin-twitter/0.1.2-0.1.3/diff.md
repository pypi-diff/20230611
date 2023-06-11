# Comparing `tmp/nonebot-plugin-twitter-0.1.2.tar.gz` & `tmp/nonebot-plugin-twitter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.1.2.tar", last modified: Sun Jun 11 06:59:29 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.1.3.tar", last modified: Sun Jun 11 07:12:25 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.1.2.tar` & `nonebot-plugin-twitter-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/LICENSE
--rw-r--r--   0        0        0     3053 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/README.md
--rw-r--r--   0        0        0    14094 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     4563 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/api.py
--rw-r--r--   0        0        0     1582 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      654 2023-06-11 06:59:19.636522 nonebot-plugin-twitter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-11 07:12:17.661678 nonebot-plugin-twitter-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3053 2023-06-11 07:12:17.661678 nonebot-plugin-twitter-0.1.3/README.md
+-rw-r--r--   0        0        0    14094 2023-06-11 07:12:17.661678 nonebot-plugin-twitter-0.1.3/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     4583 2023-06-11 07:12:17.661678 nonebot-plugin-twitter-0.1.3/nonebot_plugin_twitter/api.py
+-rw-r--r--   0        0        0     1582 2023-06-11 07:12:17.661678 nonebot-plugin-twitter-0.1.3/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      654 2023-06-11 07:12:17.661678 nonebot-plugin-twitter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.3/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.1.2/LICENSE` & `nonebot-plugin-twitter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.2/README.md` & `nonebot-plugin-twitter-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.1.3/nonebot_plugin_twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/api.py` & `nonebot-plugin-twitter-0.1.3/nonebot_plugin_twitter/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         res = await client.get(url=f"{config_dev.twitter_url}/{user_name}")
         result ={}
         if res.status_code ==200:
             result["status"] = True
             result["user_name"] = user_name
             soup = BeautifulSoup(res.text,"html.parser")
             result["screen_name"] = soup.find_all('a', class_='profile-card-fullname')[0].next
-            result["bio"] = soup.find_all('p')[0].text
+            result["bio"] = match[0].text if (match := soup.find_all('p')) else ""
         else:
             result["status"] = False
-        
+
     return result
 
 async def get_user_newtimeline(user_name:str,since_id: str = "0") -> str:
     ''' 通过 user_name 获取推文id列表,
     有 since_id return 最近的新的推文id,
     无 since_id return 最新的推文id'''
     async with httpx.AsyncClient(proxies=config_dev.twitter_proxy) as client:
```

### Comparing `nonebot-plugin-twitter-0.1.2/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.1.3/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.2/pyproject.toml` & `nonebot-plugin-twitter-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.1.2"
+version = "0.1.3"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.1.2/PKG-INFO` & `nonebot-plugin-twitter-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.1.2
+Version: 0.1.3
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.3 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
```

