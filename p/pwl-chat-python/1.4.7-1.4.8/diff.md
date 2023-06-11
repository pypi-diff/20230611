# Comparing `tmp/pwl-chat-python-1.4.7.tar.gz` & `tmp/pwl-chat-python-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.7.tar", last modified: Sun Jun 11 09:29:16 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.8.tar", last modified: Sun Jun 11 13:51:50 2023, max compression
```

## Comparing `pwl-chat-python-1.4.7.tar` & `pwl-chat-python-1.4.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.983746 pwl-chat-python-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 09:29:16.983746 pwl-chat-python-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.979745 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:29:16.983746 pwl-chat-python-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.979745 pwl-chat-python-1.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.979745 pwl-chat-python-1.4.7/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/__api__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/chatroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/redpacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.979745 pwl-chat-python-1.4.7/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/chatroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/redpacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.983746 pwl-chat-python-1.4.7/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 13:51:50.000000 pwl-chat-python-1.4.8/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/__api__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/chatroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/redpacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/chatroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/redpacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/core/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:51:50.547101 pwl-chat-python-1.4.8/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-11 13:51:36.000000 pwl-chat-python-1.4.8/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.7/LICENSE` & `pwl-chat-python-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/PKG-INFO` & `pwl-chat-python-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.7
+Version: 1.4.8
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pwl-chat-python-1.4.7/README.md` & `pwl-chat-python-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.8/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.7
+Version: 1.4.8
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pwl-chat-python-1.4.7/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.8/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/setup.py` & `pwl-chat-python-1.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/api/__init__.py` & `pwl-chat-python-1.4.8/src/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/api/chatroom.py` & `pwl-chat-python-1.4.8/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/api/redpacket.py` & `pwl-chat-python-1.4.8/src/api/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/api/user.py` & `pwl-chat-python-1.4.8/src/api/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             print('此用户不存在: ' + username)
 
     def get_online_users(self) -> dict:
         resp = requests.get(f'{HOST}/chat-room/online-users', headers={'User-Agent': UA})
         return json.loads(resp.text)
 
     def get_yesterday_reward(self) -> None:
-        if self.reward == False:
+        if self.reward == True:
             print('你已经领取过昨日活跃度奖励了')
             return
         resp = requests.get(f'{HOST}/activity/yesterday-liveness-reward-api?apiKey={self.api_key}', headers={'User-Agent': UA})
         response = json.loads(resp.text)
         reward = response['sum']
         if reward == -1:
             print('你已经领取过昨日活跃度奖励了')
```

### Comparing `pwl-chat-python-1.4.7/src/core/__init__.py` & `pwl-chat-python-1.4.8/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/core/blacklist.py` & `pwl-chat-python-1.4.8/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/core/chatroom.py` & `pwl-chat-python-1.4.8/src/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/core/cli.py` & `pwl-chat-python-1.4.8/src/core/cli.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/core/config.py` & `pwl-chat-python-1.4.8/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/core/redpacket.py` & `pwl-chat-python-1.4.8/src/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/core/user.py` & `pwl-chat-python-1.4.8/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/core/websocket.py` & `pwl-chat-python-1.4.8/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/main.py` & `pwl-chat-python-1.4.8/src/main.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.7/src/utils/utils.py` & `pwl-chat-python-1.4.8/src/utils/utils.py`

 * *Files identical despite different names*

