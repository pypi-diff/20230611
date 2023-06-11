# Comparing `tmp/nonebot-plugin-twitter-0.1.4.tar.gz` & `tmp/nonebot-plugin-twitter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.1.4.tar", last modified: Sun Jun 11 07:20:53 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.1.5.tar", last modified: Sun Jun 11 07:23:35 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.1.4.tar` & `nonebot-plugin-twitter-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-11 07:20:42.638619 nonebot-plugin-twitter-0.1.4/LICENSE
--rw-r--r--   0        0        0     3053 2023-06-11 07:20:42.638619 nonebot-plugin-twitter-0.1.4/README.md
--rw-r--r--   0        0        0    14094 2023-06-11 07:20:42.638619 nonebot-plugin-twitter-0.1.4/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     4685 2023-06-11 07:20:42.638619 nonebot-plugin-twitter-0.1.4/nonebot_plugin_twitter/api.py
--rw-r--r--   0        0        0     1582 2023-06-11 07:20:42.638619 nonebot-plugin-twitter-0.1.4/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      654 2023-06-11 07:20:42.638619 nonebot-plugin-twitter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3053 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/README.md
+-rw-r--r--   0        0        0    14094 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     4685 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/api.py
+-rw-r--r--   0        0        0     1582 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      654 2023-06-11 07:23:27.833079 nonebot-plugin-twitter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.5/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.1.4/LICENSE` & `nonebot-plugin-twitter-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.4/README.md` & `nonebot-plugin-twitter-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.4/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.4/nonebot_plugin_twitter/api.py` & `nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                         if int(tweet_id) > int(since_id):
                             new_line.append(tweet_id)
                     else:
                         new_line.append(tweet_id)
                         
             if since_id == "0":
                 if new_line == []:
-                    new_line.append("0")
+                    new_line.append("1")
                 else:
                     new_line = [str(max(map(int,new_line)))]
             if new_line == []:
                 new_line = ["not found"]
         else:
             new_line = ["not found"]
     return new_line[-1]
```

### Comparing `nonebot-plugin-twitter-0.1.4/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.4/pyproject.toml` & `nonebot-plugin-twitter-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.1.4"
+version = "0.1.5"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.1.4/PKG-INFO` & `nonebot-plugin-twitter-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.1.4
+Version: 0.1.5
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
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.5 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
```

