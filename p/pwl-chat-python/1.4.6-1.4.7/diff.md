# Comparing `tmp/pwl-chat-python-1.4.6.tar.gz` & `tmp/pwl-chat-python-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.6.tar", last modified: Sat Jun 10 14:17:09 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.7.tar", last modified: Sun Jun 11 09:29:16 2023, max compression
```

## Comparing `pwl-chat-python-1.4.6.tar` & `pwl-chat-python-1.4.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.420221 pwl-chat-python-1.4.6/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.6/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     2246 2023-06-10 14:17:09.419762 pwl-chat-python-1.4.6/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1647 2023-06-10 14:02:37.000000 pwl-chat-python-1.4.6/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.401338 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     2246 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      570 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       41 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-06-10 14:17:09.000000 pwl-chat-python-1.4.6/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-06-10 14:17:09.420365 pwl-chat-python-1.4.6/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3539 2023-06-10 14:02:37.000000 pwl-chat-python-1.4.6/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.401934 pwl-chat-python-1.4.6/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.407830 pwl-chat-python-1.4.6/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.6/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1833 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     2036 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1351 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/api/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.6/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.417298 pwl-chat-python-1.4.6/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2951 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1699 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.6/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     2164 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     5084 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1666 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     5469 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1217 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.6/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1326 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1395 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-10 14:17:09.418944 pwl-chat-python-1.4.6/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)     1675 2023-06-10 14:02:28.000000 pwl-chat-python-1.4.6/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-06-10 14:02:37.000000 pwl-chat-python-1.4.6/src/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.983746 pwl-chat-python-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 09:29:16.983746 pwl-chat-python-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.979745 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 09:29:16.000000 pwl-chat-python-1.4.7/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:29:16.983746 pwl-chat-python-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.979745 pwl-chat-python-1.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.979745 pwl-chat-python-1.4.7/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/__api__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/chatroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/redpacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.979745 pwl-chat-python-1.4.7/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/chatroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/redpacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/core/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:29:16.983746 pwl-chat-python-1.4.7/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 09:29:05.000000 pwl-chat-python-1.4.7/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.6/LICENSE` & `pwl-chat-python-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/PKG-INFO` & `pwl-chat-python-1.4.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.6
+Version: 1.4.7
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.8
 Description-Content-Type: text/markdown
@@ -49,14 +50,15 @@
 ```
 
 ## 功能
 
 - 💬 聊天模式
   - 💬 聊天吹水
   - 🤖️ 自动复读
+  - 🤖️ 自动领取昨日奖励
   - 🧠 自言自语
     - 自定义语句池
     - 定时发送
   - 🧧 自动化抢红包（脚本哥）
     - 自定义抢红包延时
     - 心跳红包防止踩坑
     - 心跳红包风险预测
@@ -65,20 +67,31 @@
   - 命令/聊天模式切换
     - (聊天模式也可以执行命令)
   - 进入答题模式(前缀自动加上 鸽)
   - ⬆️ 社区快捷命令
     - 领取昨日活跃度奖励
     - 查看个人积分
     - 查看签到状态
+    - 转账
+    - 发送清风明月
     - 查看当前活跃度
     - 查看在线用户列表
     - 查询用户详细信息
     - 🈲️ 小黑屋功能
       - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
       - 将某人从小黑屋中放出
-    - 发红包
+    - 发红包🧧
+      - 拼手气红包
+      - 普通红包
+      - 专属红包
+      - 心跳红包
+      - 猜拳红包
+      - 设置抢红包等待时间
 
 ## 效果
 
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
+![image.png](https://file.fishpi.cn/2023/06/image-d4da9bf7.png)
+![redpacket](https://file.fishpi.cn/2023/06/image-d0ad7756.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
+
+
```

### Comparing `pwl-chat-python-1.4.6/README.md` & `pwl-chat-python-1.4.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 ```
 
 ## 功能
 
 - 💬 聊天模式
   - 💬 聊天吹水
   - 🤖️ 自动复读
+  - 🤖️ 自动领取昨日奖励
   - 🧠 自言自语
     - 自定义语句池
     - 定时发送
   - 🧧 自动化抢红包（脚本哥）
     - 自定义抢红包延时
     - 心跳红包防止踩坑
     - 心跳红包风险预测
@@ -47,20 +48,29 @@
   - 命令/聊天模式切换
     - (聊天模式也可以执行命令)
   - 进入答题模式(前缀自动加上 鸽)
   - ⬆️ 社区快捷命令
     - 领取昨日活跃度奖励
     - 查看个人积分
     - 查看签到状态
+    - 转账
+    - 发送清风明月
     - 查看当前活跃度
     - 查看在线用户列表
     - 查询用户详细信息
     - 🈲️ 小黑屋功能
       - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
       - 将某人从小黑屋中放出
-    - 发红包
+    - 发红包🧧
+      - 拼手气红包
+      - 普通红包
+      - 专属红包
+      - 心跳红包
+      - 猜拳红包
+      - 设置抢红包等待时间
 
 ## 效果
 
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
+![image.png](https://file.fishpi.cn/2023/06/image-d4da9bf7.png)
+![redpacket](https://file.fishpi.cn/2023/06/image-d0ad7756.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.6/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.7/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.6
+Version: 1.4.7
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.8
 Description-Content-Type: text/markdown
@@ -49,14 +50,15 @@
 ```
 
 ## 功能
 
 - 💬 聊天模式
   - 💬 聊天吹水
   - 🤖️ 自动复读
+  - 🤖️ 自动领取昨日奖励
   - 🧠 自言自语
     - 自定义语句池
     - 定时发送
   - 🧧 自动化抢红包（脚本哥）
     - 自定义抢红包延时
     - 心跳红包防止踩坑
     - 心跳红包风险预测
@@ -65,20 +67,31 @@
   - 命令/聊天模式切换
     - (聊天模式也可以执行命令)
   - 进入答题模式(前缀自动加上 鸽)
   - ⬆️ 社区快捷命令
     - 领取昨日活跃度奖励
     - 查看个人积分
     - 查看签到状态
+    - 转账
+    - 发送清风明月
     - 查看当前活跃度
     - 查看在线用户列表
     - 查询用户详细信息
     - 🈲️ 小黑屋功能
       - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
       - 将某人从小黑屋中放出
-    - 发红包
+    - 发红包🧧
+      - 拼手气红包
+      - 普通红包
+      - 专属红包
+      - 心跳红包
+      - 猜拳红包
+      - 设置抢红包等待时间
 
 ## 效果
 
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
+![image.png](https://file.fishpi.cn/2023/06/image-d4da9bf7.png)
+![redpacket](https://file.fishpi.cn/2023/06/image-d0ad7756.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
+
+
```

### Comparing `pwl-chat-python-1.4.6/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.7/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/setup.py` & `pwl-chat-python-1.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/src/api/__init__.py` & `pwl-chat-python-1.4.7/src/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,28 +32,23 @@
 
     def login(self, username: str, password: str, mfa_code='') -> bool:
         params = {
             'nameOrEmail': username,
             'userPassword': hashlib.md5(str(password).encode('utf-8')).hexdigest(),
             'mfaCode': mfa_code
         }
-        res = requests.post(HOST + "/api/getKey", json=params,
-                            headers={'User-Agent': UA})
+        res = requests.post(f"{HOST}/api/getKey", json=params, headers={'User-Agent': UA})
         rsp = json.loads(res.text)
         if rsp['code'] == 0:
             self.set_token(rsp['Key'])
             self.set_current_user(username)
             print(f'登陆成功! 更多功能与趣味游戏请访问网页端: {HOST}')
             return True
         elif rsp['code'] == -1 and rsp['msg'] == '两步验证失败，请填写正确的一次性密码':
             print("请输入两步验证码:")
             return False
         else:
             print(f"登陆失败: {rsp['msg']}")
             sys.exit(1)
 
-    def get_yesterday_reward(self) -> dict:
-        resp = requests.get(f'{HOST}/activity/yesterday-liveness-reward-api?apiKey={self.api_key}', headers={'User-Agent': UA})
-        return json.loads(resp.text)
-
 
 API = FishPi()
```

### Comparing `pwl-chat-python-1.4.6/src/api/chatroom.py` & `pwl-chat-python-1.4.7/src/api/chatroom.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,49 +8,44 @@
 
 
 class ChatRoom(Base):
 
     def more(self, page: int = 1) -> None | dict:
         if self.api_key == '':
             return None
-        resp = requests.get(HOST + f"/chat-room/more?page={page}",
+        resp = requests.get(f"{HOST}/chat-room/more?page={page}",
                             headers={'User-Agent': UA})
         return json.loads(resp.text)
 
     def send(self, message: str) -> dict | None:
         if self.api_key == '':
             return None
         params = {'apiKey': self.api_key, 'content': message,
                   'client': f'Python/客户端v{__version__}'}
-        ret = requests.post(HOST + "/chat-room/send",
-                            json=params, headers={'User-Agent': UA})
+        ret = requests.post(f'{HOST}/chat-room/send', json=params, headers={'User-Agent': UA})
         ret_json = json.loads(ret.text)
         if ('code' in ret_json and ret_json['code'] == -1):
             print(ret_json['msg'])
             
 
     def send_redpacket(self, redpacket :RedPacket=RedPacket('最后的发', 128, 5,RedPacketType.RANDOM)):
         content = f'[redpacket]{json.dumps(redpacket.__json__())}[/redpacket]'
-        print(content)
         self.send(content)        
 
     def open_redpacket(self, red_packet_id) -> dict:
         params = {
             'apiKey': self.api_key,
             'oId': red_packet_id
         }
-        resp = requests.post(HOST + "/chat-room/red-packet/open",
-                             json=params, headers={'User-Agent': UA})
+        resp = requests.post(f"{HOST}/chat-room/red-packet/open", json=params, headers={'User-Agent': UA})
         return json.loads(resp.text)
 
     def open_rock_paper_scissors_redpacket(self, red_packet_id, gesture: int = -1) -> dict:
         if gesture not in [0, 1, 2]:
             gesture = random.choice([0, 1, 2])
         params = {
             'apiKey': self.api_key,
             'oId': red_packet_id,
             'gesture': gesture
         }
-        print(gesture)
-        resp = requests.post(HOST + "/chat-room/red-packet/open",
-                             json=params, headers={'User-Agent': UA})
+        resp = requests.post(f"{HOST}/chat-room/red-packet/open", json=params, headers={'User-Agent': UA})
         return json.loads(resp.text)
```

### Comparing `pwl-chat-python-1.4.6/src/api/redpacket.py` & `pwl-chat-python-1.4.7/src/api/redpacket.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             'money': self.money,
             'count': self.count,
             'type': self.type.value
         }    
         
 class SpecifyRedPacket(RedPacket):
     def __init__(self, msg :str = '给!', money :int = 32, send_to :list = []):
-        super().__init__(msg, money, 1, RedPacketType.SPECIFY)
+        super().__init__(msg, money, len(send_to), RedPacketType.SPECIFY)
         self.recivers = send_to
 
     def __json__(self):
         json_data = super().__json__()
         json_data['recivers'] = self.recivers
         return json_data
```

### Comparing `pwl-chat-python-1.4.6/src/core/__init__.py` & `pwl-chat-python-1.4.7/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/src/core/blacklist.py` & `pwl-chat-python-1.4.7/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/src/core/chatroom.py` & `pwl-chat-python-1.4.7/src/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/src/core/cli.py` & `pwl-chat-python-1.4.7/src/core/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,36 +4,17 @@
 from .user import *
 from .websocket import chatroom_out,init_chatroom
 from src.api.redpacket import *
 from src.utils.utils import *
 
 
 
-def console_input(api: FishPi):
-    while True:
-        msg = input("")
-        if msg == '#help':
-            print(COMMAND_GUIDE)
-        elif len(api.api_key) == 0:
-            api.login(GLOBAL_CONFIG.auth_config.username,
-                      GLOBAL_CONFIG.auth_config.password, msg)                
-        elif msg == '#cli':
-            if api.ws == None:
-                print("已经进入交互模式了")
-            else:    
-                chatroom_out(api)
-                print("进入交互模式")
-        elif msg == '#chatroom':
-            if api.ws == None:
-               init_chatroom(api)
-            else:
-               chatroom_out(api)
-               init_chatroom(api)         
-        elif msg == "#rp":
-               api.chatroom.send_redpacket()       
+def __send_redpacket_handler(api :FishPi, msg :str):
+        if  msg == "#rp":
+               api.chatroom.send_redpacket()
         elif msg == "#rp-ave":
                api.chatroom.send_redpacket(RedPacket('人人有份!', 32, 5, RedPacketType.AVERAGE))
         elif msg == "#rp-hb":
                api.chatroom.send_redpacket(RedPacket('慎点!', 32, 5, RedPacketType.HEARTBEAT))
         elif msg == "#rp-rps":
                api.chatroom.send_redpacket(RPSRedPacket('剪刀石头布!', 32, 0))
         elif msg.startswith('#rp-to'):
@@ -49,45 +30,82 @@
             else:
                 print('非法红包指令')       
         elif msg.startswith('#rp-hb'):
             res = re.fullmatch(RP_HB_CODE_RE,msg)
             if res is not None:
                 api.chatroom.send_redpacket(RedPacket('人人有份!', res.group(2), res.group(1), RedPacketType.HEARTBEAT))
             else:
-                print('非法红包指令')  
+                print('非法红包指令')
         elif msg.startswith('#rp-rps'):
             res = re.fullmatch(RP_RPS_CODE_RE,msg)
             if res is not None:
                 api.chatroom.send_redpacket(RPSRedPacket('剪刀石头布!', res.group(2), res.group(1)))
             else:
                 print('非法红包指令')
+        elif msg.startswith('#rp-time'):
+            res = re.fullmatch(RP_TIME_CODE_RE,msg)
+            if res is not None:
+                time = res.group(1)
+                GLOBAL_CONFIG.redpacket_config.rate = int(time)
+                print(f'红包等待时间已设置成功 {time}s')
+            else:
+                print('非法红包指令')
         elif msg.startswith('#rp'):
             res = re.fullmatch(RP_CODE_RE,msg)
             if res is not None:
                 api.chatroom.send_redpacket(RedPacket('那就看运气吧!', res.group(2), res.group(1), RedPacketType.RANDOM))
             else:
-                print('非法红包指令')                                                             
+                print('非法红包指令')
+                    
+
+
+def cli_handler(api: FishPi):
+    while True:
+        msg = input("")
+        if msg == '#help':
+            print(COMMAND_GUIDE)
+        elif len(api.api_key) == 0:
+            api.login(GLOBAL_CONFIG.auth_config.username,
+                      GLOBAL_CONFIG.auth_config.password, msg)                
+        elif msg == '#cli':
+            if api.ws == None:
+                print("已经进入交互模式了")
+            else:    
+                chatroom_out(api)
+                print("进入交互模式")
+        elif msg == '#chatroom':
+            if api.ws == None:
+               init_chatroom(api)
+            else:
+               chatroom_out(api)
+               init_chatroom(api)
+        elif msg.startswith('#bm'):
+            api.user.send_breezemoon(msg[msg.find(' ')+1:len(msg)])
+        elif msg.startswith('#transfer'):
+            res = re.fullmatch(TRANSFER_RE, msg)
+            if res is not None:
+                api.user.transfer(res.group(2), res.group(1), res.group(3))
+            else:
+               print('非法转账命令')    
+        elif msg.startswith('#rp'):
+            __send_redpacket_handler(api, msg)                                   
         elif msg == '#answer':
             if GLOBAL_CONFIG.chat_config.answerMode:
                 GLOBAL_CONFIG.chat_config.answerMode = False
                 print('退出答题模式')
             else:
                 GLOBAL_CONFIG.chat_config.answerMode = True
                 print('进入答题模式')
         elif msg == '#checked':
             if api.user.checked_status()['checkedIn']:
                 print('今日你已签到！')
             else:
                 print('今日还未签到，摸鱼也要努力呀！')
         elif msg == '#reward':
-            reward = api.get_yesterday_reward()['sum']
-            if reward == -1:
-                print('你已经领取过昨日活跃度奖励了')
-            else:
-                print(f'领取昨日活跃度奖励 积分: {reward}')
+            api.user.get_yesterday_reward()
         elif msg == '#liveness':
             print('当前活跃度: ' +
                   str(api.user.get_liveness_info()['liveness']))
         elif msg == '#point':
             print('当前积分: ' + str(api.user.get_user_info(GLOBAL_CONFIG.auth_config.username)['userPoint']))
         elif msg == '#online-users':
             render_online_users(api)
```

### Comparing `pwl-chat-python-1.4.6/src/core/config.py` & `pwl-chat-python-1.4.7/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/src/core/redpacket.py` & `pwl-chat-python-1.4.7/src/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/src/core/user.py` & `pwl-chat-python-1.4.7/src/core/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     print('----------------------')
     print('| 聊天室在线人数: ' + str(data['onlineChatCnt']) + ' |')
     print('----------------------')
     for user in data['users']:
         print('用户: ' + user['userName'])
         print('----------------------')
 
+def auto_check_in(api: FishPi):
+    if len(api.api_key) == 0:
+        print('未登录')
+    else:
+        api.user.get_yesterday_reward()
 
 def login(api: FishPi):
     success = api.login(GLOBAL_CONFIG.auth_config.username,
                         GLOBAL_CONFIG.auth_config.password, GLOBAL_CONFIG.auth_config.mfa_code)
     if success:
         print(HELP)
     else:
```

### Comparing `pwl-chat-python-1.4.6/src/core/websocket.py` & `pwl-chat-python-1.4.7/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.6/src/main.py` & `pwl-chat-python-1.4.7/src/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 import click
-import rel
 from src.core import __init__
 from src.core.config import GLOBAL_CONFIG, AuthConfig
-from src.core.user import login
-from src.core.cli import console_input
+from src.core.user import login, auto_check_in
+from src.core.cli import cli_handler
 from src.core.websocket import init_chatroom
 from src.utils.version import __version__
 from src.api import API
 
 
 class CliConfig(object):
     def __init__(self, username: str = '', password: str = '', code: str = '', file_path: str = None):
@@ -20,16 +19,17 @@
 
 def run(config: CliConfig):
     __init__(API, config.file_path)
     if config.username is not None and config.password is not None:
         GLOBAL_CONFIG.auth_config = AuthConfig(
             config.username, config.password, config.code)
     login(API)
+    auto_check_in(API)
     init_chatroom(API)
-    console_input(API)
+    cli_handler(API)
 
 @click.command()
 @click.version_option(__version__)
 @click.option("--username", "-u", type=click.STRING, help="摸鱼派用户名")
 @click.option("--password", "-p", type=click.STRING, help="密码")
 @click.option("--code", "-c", type=click.STRING, help="两步验证码")
 @click.option("--file_path", "-f", type=click.STRING, help="配置文件路径")
```

### Comparing `pwl-chat-python-1.4.6/src/utils/utils.py` & `pwl-chat-python-1.4.7/src/utils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 UA = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36'
 
 HELP = '输入#help获得命令提示列表'
 
 COMMAND_GUIDE = '''
 [#cli] 进入命令交互模式
 [#chatroom] 进入聊天室模式
-[#rp] 拼手气红包 1128 1个128积分 (默认5个,128积分)
-[#rp-ave] 平均红包 1128 1个128积分 (默认5个,32积分)
-[#rp-hb] 心跳红包 5128 5个128积分 (默认5个,32积分)
-[#rp-rps] 猜拳红包 0128 128积分 (0=石头 1=剪刀 2=布)
-[#rp-to] 专属红包 32 Gakkiyomi (积分 用户)
+[#rp] 1128 1个128积分 (默认5个,128积分)拼手气红包
+[#rp-ave] 1128 1个128积分 (默认5个,32积分)平均红包
+[#rp-hb] 5128 5个128积分 (默认5个,32积分)心跳红包
+[#rp-rps] 0128 128积分 (0=石头 1=剪刀 2=布)猜拳红包
+[#rp-to] 32 Gakkiyomi,xiaoIce (积分 用户)专属红包
+[#rp-time] 3 设置抢红包等待时间
+[#bm] 发送清风明月
 [#answer] 进入|退出 答题模式
 [#checked] 查看当前是否签到
 [#reward] 领取昨日活跃奖励
+[#transfer] 32 Gakkiyomi 送给你 (积分 用户 留言)
 [#point] 查看当前个人积分
 [#online-users] 查看当前在线的用户列表
 [#user username] 输入 #user 用户名 可查看此用户详细信息 (#user Gakkiyomi)
 [#blacklist] 查看黑名单列表
 [#ban username] 将某人送入黑名单
 [#unban username] 将某人解除黑名单
 [#liveness] 查看当前活跃度(⚠️慎用，如果频繁请求此命令(最少间隔30s)，登录状态会被直接注销,需要重启脚本！)
@@ -30,8 +33,10 @@
 
 
 
 RP_CODE_RE = re.compile('#rp\s{1,1}(\d)(\d+)')
 RP_AVER_CODE_RE = re.compile('#rp-ave\s{1,1}(\d)(\d+)')
 RP_HB_CODE_RE = re.compile('#rp-hb\s{1,1}(\d)(\d+)')
 RP_RPS_CODE_RE = re.compile('#rp-rps\s{1,1}(\d)(\d+)')
-RP_SEND_TO_CODE_RE = re.compile('#rp-to (\d+) ([\w,]+)(?<!,)$')
+RP_SEND_TO_CODE_RE = re.compile('#rp-to (\d+) ([\w,]+)(?<!,)$')
+RP_TIME_CODE_RE = re.compile('#rp-time (\d+)')
+TRANSFER_RE = re.compile('#transfer (\d+) (\w+)( \S+)?')
```

