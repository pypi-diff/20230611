# Comparing `tmp/rocketchat_async-1.1.0.tar.gz` & `tmp/rocketchat_async-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketchat_async-1.1.0.tar", max compression
+gzip compressed data, was "rocketchat_async-1.2.0.tar", max compression
```

## Comparing `rocketchat_async-1.1.0.tar` & `rocketchat_async-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2022-12-29 18:27:14.756067 rocketchat_async-1.1.0/LICENSE
--rw-r--r--   0        0        0     3047 2023-03-23 17:19:26.957668 rocketchat_async-1.1.0/README.md
--rw-r--r--   0        0        0      610 2023-03-23 17:24:06.824263 rocketchat_async-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-12-29 15:03:17.541726 rocketchat_async-1.1.0/rocketchat_async/.gitignore
--rw-r--r--   0        0        0       45 2022-12-29 19:30:01.886734 rocketchat_async-1.1.0/rocketchat_async/__init__.py
--rw-r--r--   0        0        0     1013 2022-12-30 15:35:26.313806 rocketchat_async-1.1.0/rocketchat_async/constants.py
--rw-r--r--   0        0        0     3939 2023-03-23 17:03:10.776225 rocketchat_async-1.1.0/rocketchat_async/core.py
--rw-r--r--   0        0        0     2695 2023-03-04 15:32:14.342998 rocketchat_async-1.1.0/rocketchat_async/dispatcher.py
--rw-r--r--   0        0        0     7256 2023-03-09 20:47:07.291723 rocketchat_async-1.1.0/rocketchat_async/methods.py
--rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 rocketchat_async-1.1.0/setup.py
--rw-r--r--   0        0        0     3913 1970-01-01 00:00:00.000000 rocketchat_async-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2022-12-29 18:27:14.756067 rocketchat_async-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3178 2023-06-11 19:23:37.324110 rocketchat_async-1.2.0/README.md
+-rw-r--r--   0        0        0      610 2023-06-11 19:27:24.742301 rocketchat_async-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-12-29 15:03:17.541726 rocketchat_async-1.2.0/rocketchat_async/.gitignore
+-rw-r--r--   0        0        0       45 2022-12-29 19:30:01.886734 rocketchat_async-1.2.0/rocketchat_async/__init__.py
+-rw-r--r--   0        0        0     1013 2022-12-30 15:35:26.313806 rocketchat_async-1.2.0/rocketchat_async/constants.py
+-rw-r--r--   0        0        0     4771 2023-06-11 19:24:27.876593 rocketchat_async-1.2.0/rocketchat_async/core.py
+-rw-r--r--   0        0        0     2695 2023-06-11 19:23:10.391854 rocketchat_async-1.2.0/rocketchat_async/dispatcher.py
+-rw-r--r--   0        0        0     7948 2023-06-11 19:24:58.628888 rocketchat_async-1.2.0/rocketchat_async/methods.py
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 rocketchat_async-1.2.0/setup.py
+-rw-r--r--   0        0        0     4044 1970-01-01 00:00:00.000000 rocketchat_async-1.2.0/PKG-INFO
```

### Comparing `rocketchat_async-1.1.0/LICENSE` & `rocketchat_async-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketchat_async-1.1.0/README.md` & `rocketchat_async-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 
 async def main(address, username, password):
     while True:
         try:
             rc = RocketChat()
             await rc.start(address, username, password)
+            # Alternatively, use rc.resume for token-based authentication:
+            # await rc.resume(address, username, token)
 
             # A possible workflow consists of two steps:
             #
             # 1. Set up the desired callbacks...
             for channel_id, channel_type in await rc.get_channels():
                 await rc.subscribe_to_channel_messages(channel_id,
                                                        handle_message)
```

### Comparing `rocketchat_async-1.1.0/pyproject.toml` & `rocketchat_async-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rocketchat-async"
-version = "1.1.0"
+version = "1.2.0"
 description = "asyncio-based Python wrapper for the Rocket.Chat Realtime API."
 authors = ["Hynek Urban <hynek.urban@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rocketchat_async"}]
 homepage = "https://github.com/hynek-urban/rocketchat-async"
 documentation = "https://github.com/hynek-urban/rocketchat-async"
```

### Comparing `rocketchat_async-1.1.0/rocketchat_async/constants.py` & `rocketchat_async-1.2.0/rocketchat_async/constants.py`

 * *Files identical despite different names*

### Comparing `rocketchat_async-1.1.0/rocketchat_async/core.py` & `rocketchat_async-1.2.0/rocketchat_async/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import websockets
 
 from rocketchat_async.dispatcher import Dispatcher
-from rocketchat_async.methods import Connect, Login, GetChannels, SendMessage,\
+from rocketchat_async.methods import Connect, Login, Resume, GetChannels, SendMessage,\
         SendReaction, SendTypingEvent, SubscribeToChannelMessages,\
         SubscribeToChannelChanges, Unsubscribe
 
 
 class RocketChat:
     """Represents a connection to RocketChat, exposing the API."""
 
@@ -34,14 +34,31 @@
             raise self.ConnectCallFailed(e)
 
         # Connect and login.
         await self._connect()
         self.user_id = await self._login(username, password)
         self.username = username
 
+    async def resume(self, address, username, token):
+        ws_connected = asyncio.get_event_loop().create_future()
+        ws_connection = self._start(address, ws_connected)
+        self._ws_connection_task = asyncio.create_task(ws_connection)
+        try:
+            await ws_connected
+        except (OSError, websockets.InvalidMessage) as e:
+            # Exceptions that can arise during temporary network glitches or
+            # outages on the remote side.
+            # See also https://github.com/aaugustin/websockets/issues/593
+            raise self.ConnectCallFailed(e)
+
+        # Connect and login.
+        await self._connect()
+        self.user_id = await self._resume(token)
+        self.username = username
+
     async def run_forever(self):
         try:
             await self.dispatch_task
         except websockets.ConnectionClosed as e:
             raise self.ConnectionClosed(e)
 
     async def _start(self, address, connected_fut):
@@ -58,14 +75,17 @@
 
     async def _connect(self):
         await Connect.call(self._dispatcher)
 
     async def _login(self, username, password):
         return await Login.call(self._dispatcher, username, password)
 
+    async def _resume(self, token):
+        return await Resume.call(self._dispatcher, token)
+
     # --> Public API methods start here. <--
 
     async def get_channels(self):
         """Get a list of channels user is currently member of."""
         return await GetChannels.call(self._dispatcher)
 
     async def send_message(self, text, channel_id, thread_id=None):
```

### Comparing `rocketchat_async-1.1.0/rocketchat_async/dispatcher.py` & `rocketchat_async-1.2.0/rocketchat_async/dispatcher.py`

 * *Files identical despite different names*

### Comparing `rocketchat_async-1.1.0/rocketchat_async/methods.py` & `rocketchat_async-1.2.0/rocketchat_async/methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,42 @@
     }
 
     @classmethod
     async def call(cls, dispatcher):
         await dispatcher.call_method(cls.REQUEST_MSG)
 
 
+class Resume(RealtimeRequest):
+    """Log in to the service with a token."""
+
+    @staticmethod
+    def _get_request_msg(msg_id, token):
+        return {
+            "msg": "method",
+            "method": "login",
+            "id": msg_id,
+            "params": [
+                {
+                    "resume": token,
+                }
+            ]
+        }
+
+    @staticmethod
+    def _parse(response):
+        return response['result']['id']
+
+    @classmethod
+    async def call(cls, dispatcher, token):
+        msg_id = cls._get_new_id()
+        msg = cls._get_request_msg(msg_id, token)
+        response = await dispatcher.call_method(msg, msg_id)
+        return cls._parse(response)
+
+
 class Login(RealtimeRequest):
     """Log in to the service."""
 
     @staticmethod
     def _get_request_msg(msg_id, username, password):
         pwd_digest = hashlib.sha256(password.encode()).hexdigest()
         return {
```

### Comparing `rocketchat_async-1.1.0/setup.py` & `rocketchat_async-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'rocketchat-async',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': 'asyncio-based Python wrapper for the Rocket.Chat Realtime API.',
-    'long_description': '# rocketchat-async\n\nasyncio-based Python wrapper for the Rocket.Chat Realtime API.\n\n## When should you use this library?\n\nUse this library if you:\n\n- want to integrate with Rocket.Chat from Python\n- are using [asyncio](https://docs.python.org/3/library/asyncio.html) to drive your code\n- want to use Rocket.Chat\'s efficient websockets-based Realtime API\n\n## Installation\n\n`pip install rocketchat-async`\n\n## Example usage\n\n```python\nimport asyncio\nimport random\nfrom rocketchat_async import RocketChat\n\n\ndef handle_message(channel_id, sender_id, msg_id, thread_id, msg, qualifier):\n    """Simply print the message that arrived."""\n    print(msg)\n\n\nasync def main(address, username, password):\n    while True:\n        try:\n            rc = RocketChat()\n            await rc.start(address, username, password)\n\n            # A possible workflow consists of two steps:\n            #\n            # 1. Set up the desired callbacks...\n            for channel_id, channel_type in await rc.get_channels():\n                await rc.subscribe_to_channel_messages(channel_id,\n                                                       handle_message)\n            # 2. ...and then simply wait for the registered events.\n            await rc.run_forever()\n        except (RocketChat.ConnectionClosed,\n                RocketChat.ConnectCallFailed) as e:\n            print(f\'Connection failed: {e}. Waiting a few seconds...\')\n            await asyncio.sleep(random.uniform(4, 8))\n            print(\'Reconnecting...\')\n\n\n# Side note: Don\'t forget to use the wss:// scheme when TLS is used.\nasyncio.run(main(\'ws://localhost:3000/websocket\', \'username\', \'password\'))\n```\n\n## API Overview\n\nBrief overview of the currently implemented methods.\n\nAs of now, Rocket.Chat\'s API is only covered partially (based on my original\nneeds). I am open to both feature requests as well as pull requests.\n\n### Methods\n\n#### `RocketChat.get_channels()`\n\nGet a list of channels the logged-in user is currently member of.\n\n#### `RocketChat.send_message(text, channel_id, thread_id=None)`\n\nSend a text message to a channel.\n\n#### `RocketChat.send_reaction(orig_msg_id, emoji)`\n\nSend a reaction to a specific message.\n\n#### `RocketChat.send_typing_event(channel_id, is_typing)`\n\nSend the "typing" event to a channel.\n\n#### `RocketChat.subscribe_to_channel_messages(channel_id, callback)`\n\nSubscribe to all messages in the given channel. Returns the subscription ID.\n\nThe provided callback should accept six arguments: `channel_id`,\n`sender_id`, `msg_id`, `thread_id`, `msg_text` and\n`msg_qualifier`. The qualifier can help to determine if e.g. the\nmessage is a system message about the user being removed from\nthe channel.\n\n#### `RocketChat.subscribe_to_channel_changes(callback)`\n\nSubscribe to all changes in channels. Returns the subscription ID.\n\nThe provided callback should accept two arguments: `channel_id`\nand `channel_qualifier`. The qualifier helps to determine e.g.\nif it\'s a direct message or a normal room.\n\n#### `RocketChat.unsubscribe(subscription_id)`\n\nCancel a subscription.\n',
+    'long_description': '# rocketchat-async\n\nasyncio-based Python wrapper for the Rocket.Chat Realtime API.\n\n## When should you use this library?\n\nUse this library if you:\n\n- want to integrate with Rocket.Chat from Python\n- are using [asyncio](https://docs.python.org/3/library/asyncio.html) to drive your code\n- want to use Rocket.Chat\'s efficient websockets-based Realtime API\n\n## Installation\n\n`pip install rocketchat-async`\n\n## Example usage\n\n```python\nimport asyncio\nimport random\nfrom rocketchat_async import RocketChat\n\n\ndef handle_message(channel_id, sender_id, msg_id, thread_id, msg, qualifier):\n    """Simply print the message that arrived."""\n    print(msg)\n\n\nasync def main(address, username, password):\n    while True:\n        try:\n            rc = RocketChat()\n            await rc.start(address, username, password)\n            # Alternatively, use rc.resume for token-based authentication:\n            # await rc.resume(address, username, token)\n\n            # A possible workflow consists of two steps:\n            #\n            # 1. Set up the desired callbacks...\n            for channel_id, channel_type in await rc.get_channels():\n                await rc.subscribe_to_channel_messages(channel_id,\n                                                       handle_message)\n            # 2. ...and then simply wait for the registered events.\n            await rc.run_forever()\n        except (RocketChat.ConnectionClosed,\n                RocketChat.ConnectCallFailed) as e:\n            print(f\'Connection failed: {e}. Waiting a few seconds...\')\n            await asyncio.sleep(random.uniform(4, 8))\n            print(\'Reconnecting...\')\n\n\n# Side note: Don\'t forget to use the wss:// scheme when TLS is used.\nasyncio.run(main(\'ws://localhost:3000/websocket\', \'username\', \'password\'))\n```\n\n## API Overview\n\nBrief overview of the currently implemented methods.\n\nAs of now, Rocket.Chat\'s API is only covered partially (based on my original\nneeds). I am open to both feature requests as well as pull requests.\n\n### Methods\n\n#### `RocketChat.get_channels()`\n\nGet a list of channels the logged-in user is currently member of.\n\n#### `RocketChat.send_message(text, channel_id, thread_id=None)`\n\nSend a text message to a channel.\n\n#### `RocketChat.send_reaction(orig_msg_id, emoji)`\n\nSend a reaction to a specific message.\n\n#### `RocketChat.send_typing_event(channel_id, is_typing)`\n\nSend the "typing" event to a channel.\n\n#### `RocketChat.subscribe_to_channel_messages(channel_id, callback)`\n\nSubscribe to all messages in the given channel. Returns the subscription ID.\n\nThe provided callback should accept six arguments: `channel_id`,\n`sender_id`, `msg_id`, `thread_id`, `msg_text` and\n`msg_qualifier`. The qualifier can help to determine if e.g. the\nmessage is a system message about the user being removed from\nthe channel.\n\n#### `RocketChat.subscribe_to_channel_changes(callback)`\n\nSubscribe to all changes in channels. Returns the subscription ID.\n\nThe provided callback should accept two arguments: `channel_id`\nand `channel_qualifier`. The qualifier helps to determine e.g.\nif it\'s a direct message or a normal room.\n\n#### `RocketChat.unsubscribe(subscription_id)`\n\nCancel a subscription.\n',
     'author': 'Hynek Urban',
     'author_email': 'hynek.urban@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hynek-urban/rocketchat-async',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `rocketchat_async-1.1.0/PKG-INFO` & `rocketchat_async-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketchat-async
-Version: 1.1.0
+Version: 1.2.0
 Summary: asyncio-based Python wrapper for the Rocket.Chat Realtime API.
 Home-page: https://github.com/hynek-urban/rocketchat-async
 License: MIT
 Author: Hynek Urban
 Author-email: hynek.urban@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -49,14 +49,16 @@
 
 
 async def main(address, username, password):
     while True:
         try:
             rc = RocketChat()
             await rc.start(address, username, password)
+            # Alternatively, use rc.resume for token-based authentication:
+            # await rc.resume(address, username, token)
 
             # A possible workflow consists of two steps:
             #
             # 1. Set up the desired callbacks...
             for channel_id, channel_type in await rc.get_channels():
                 await rc.subscribe_to_channel_messages(channel_id,
                                                        handle_message)
```

