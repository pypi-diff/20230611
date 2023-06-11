# Comparing `tmp/pymino-1.1.8.6.tar.gz` & `tmp/pymino-1.1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\sub\dist\.tmp-xekccvso\pymino-1.1.8.6.tar", last modified: Thu Jun  8 12:38:37 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\New folder (4)\dist\.tmp-jdfef514\pymino-1.1.8.7.tar", last modified: Sun Jun 11 14:03:44 2023, max compression
```

## Comparing `pymino-1.1.8.6.tar` & `pymino-1.1.8.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.371657 pymino-1.1.8.6/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.6/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-06-08 12:38:37.372154 pymino-1.1.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.293784 pymino-1.1.8.6/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-08 12:38:10.000000 pymino-1.1.8.6/pymino/__init__.py
--rw-rw-rw-   0        0        0     7879 2023-06-08 12:33:52.000000 pymino-1.1.8.6/pymino/async_bot.py
--rw-rw-rw-   0        0        0    27301 2023-06-08 12:33:51.000000 pymino-1.1.8.6/pymino/bot.py
--rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.8.6/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.338424 pymino-1.1.8.6/pymino/ext/
--rw-rw-rw-   0        0        0      474 2023-06-08 05:17:39.000000 pymino-1.1.8.6/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.8.6/pymino/ext/account.py
--rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.8.6/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    17955 2023-06-08 12:35:46.000000 pymino-1.1.8.6/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    23899 2023-06-08 07:29:50.000000 pymino-1.1.8.6/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7098 2023-06-08 07:26:50.000000 pymino-1.1.8.6/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   284982 2023-06-08 12:32:12.000000 pymino-1.1.8.6/pymino/ext/community.py
--rw-rw-rw-   0        0        0    41392 2023-06-08 07:22:51.000000 pymino-1.1.8.6/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.6/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.363225 pymino-1.1.8.6/pymino/ext/entities/
--rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.8.6/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.8.6/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.8.6/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.8.6/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.6/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15812 2023-06-08 11:41:30.000000 pymino-1.1.8.6/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.8.6/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4763 2023-05-29 00:33:12.000000 pymino-1.1.8.6/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.8.6/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.8.6/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.8.6/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.6/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.6/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.6/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6833 2023-06-08 07:28:43.000000 pymino-1.1.8.6/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.370665 pymino-1.1.8.6/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      118 2023-05-28 22:35:54.000000 pymino-1.1.8.6/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.8.6/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.6/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.6/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.8.6/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.311640 pymino-1.1.8.6/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1153 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-08 12:38:37.376120 pymino-1.1.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.662464 pymino-1.1.8.7/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.7/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-06-11 14:03:44.662464 pymino-1.1.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.590023 pymino-1.1.8.7/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-11 13:45:06.000000 pymino-1.1.8.7/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.8.7/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    28459 2023-06-11 13:40:20.000000 pymino-1.1.8.7/pymino/bot.py
+-rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.8.7/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.633671 pymino-1.1.8.7/pymino/ext/
+-rw-rw-rw-   0        0        0      474 2023-06-08 05:17:39.000000 pymino-1.1.8.7/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.8.7/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.8.7/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.8.7/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    23958 2023-06-11 13:57:44.000000 pymino-1.1.8.7/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.8.7/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   291593 2023-06-10 01:27:27.000000 pymino-1.1.8.7/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    41528 2023-06-11 13:55:44.000000 pymino-1.1.8.7/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.7/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.654999 pymino-1.1.8.7/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.8.7/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.8.7/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.8.7/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.8.7/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.7/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.8.7/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.8.7/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4763 2023-06-10 01:04:26.000000 pymino-1.1.8.7/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.8.7/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.8.7/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.8.7/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.7/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.7/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.7/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.8.7/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.661447 pymino-1.1.8.7/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      118 2023-05-28 22:35:54.000000 pymino-1.1.8.7/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.8.7/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.7/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.7/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.8.7/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.607383 pymino-1.1.8.7/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1153 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-11 14:03:44.664423 pymino-1.1.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.7/setup.py
```

### Comparing `pymino-1.1.8.6/LICENSE` & `pymino-1.1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/PKG-INFO` & `pymino-1.1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.6
+Version: 1.1.8.7
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.6 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.7 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.6/README.md` & `pymino-1.1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/__init__.py` & `pymino-1.1.8.7/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.8.6'
+__version__ = '1.1.8.7'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.8.6/pymino/async_bot.py` & `pymino-1.1.8.7/pymino/async_bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,93 @@
 import asyncio
 from typing import Optional, Union
 from time import time, perf_counter
 
 from .ext.entities import *
 from .ext.async_socket import AsyncWSClient
 from .ext.async_community import AsyncCommunity
-from .ext.utilities.generate import device_id
+from .ext.utilities.generate import device_id as generate_device_id
 from .ext.utilities.async_request_handler import AsyncRequestHandler
 
 
 class AsyncBot(AsyncWSClient):
     def __init__(
         self,
         command_prefix: Optional[str] = "!",
         community_id: Union[str, int] = None,
-        online_status: bool = True,
-        **kwargs
+        device_id: Optional[str] = None,
+        intents: bool = False,
+        online_status: bool = False,
+        proxy: Optional[str] = None
         ):
-
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
         self.loop:              asyncio.AbstractEventLoop = asyncio.get_event_loop()
         self._debug:            bool = check_debugger()
+        self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
         self.command_prefix:    Optional[str] = command_prefix
         self.community_id:      Union[str, int] = community_id
         self.online_status:     bool = online_status
-        self.device_id:         Optional[str] = kwargs.get("device_id") or device_id()
+        self.device_id:         Optional[str] = device_id or generate_device_id()
         self.request:           AsyncRequestHandler = AsyncRequestHandler(
                                 bot = self,
                                 loop = self.loop,
-                                proxy=kwargs.get("proxy")
+                                proxy=proxy
                                 )
         self.community:         AsyncCommunity = AsyncCommunity(
                                 bot = self,
                                 session=self.request,
                                 community_id=self.community_id
                                 )
         if self.community_id:   self.set_community_id(community_id)
 
         AsyncWSClient.__init__(self)
 
     @property
     def debug(self) -> bool:
         return self._debug
-    
 
     @debug.setter
     def debug(self, value: bool) -> None:
         self._debug = value
 
 
     @property
+    def intents(self) -> bool:
+        return self._intents
+    
+    @intents.setter
+    def intents(self, value: bool) -> None:
+        self._intents = value
+
+    @property
     def is_ready(self) -> bool:
         return self._is_ready
     
-
     @is_ready.setter
     def is_ready(self, value: bool) -> None:
         self._is_ready = value
 
 
     @property
     def userId(self) -> str:
         return self._userId
 
-
     @userId.setter
     def userId(self, value: str) -> None:
         self._userId = value
 
         
     @property
     def sid(self) -> str:
         return self._sid
 
-
     @sid.setter
     def sid(self, value: str) -> None:
         self._sid = value
 
 
     async def authenticate(self, email: str, password: str, device_id: str=None) -> dict:
         if device_id:
@@ -190,18 +193,17 @@
         self.userId: str = self.profile.userId
         self.community.userId: str = self.userId
         self.request.sid: str = self.sid
         self.request.userId: str = self.userId
         self.is_authenticated: bool = True
 
         if hasattr(self.request, "email") and self._cached:
-            print("Caching login credentials...")
             cache_login(email=self.request.email, device=self.device_id, sid=self.sid)
 
-        if all([not self.is_ready, not hasattr(self, "disable_socket") or not self.disable_socket]):
+        if not self.is_ready:
             self.is_ready = True
             await self.run_forever()
 
 
     async def fetch_account(self) -> dict:
         self.profile: UserProfile = UserProfile(
             await self.request.handler(
```

### Comparing `pymino-1.1.8.6/pymino/bot.py` & `pymino-1.1.8.7/pymino/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 from typing import Optional, Union
 from time import perf_counter, time
 
 from .ext.entities import *
 from .ext.socket import WSClient
 from .ext.account import Account
 from .ext.community import Community
-from .ext.utilities.generate import device_id
 from .ext.utilities.request_handler import RequestHandler
-
+from .ext.utilities.generate import device_id as generate_device_id
 
 class Bot(WSClient):
     """
     `Bot` - This is the main client.
 
     `**Parameters**``
     - `command_prefix` - The prefix to use for commands. `Defaults` to `!`.
     - `community_id` - The community id to use for the bot. `Defaults` to `None`.
+    - `device_id` - The device id to use for the bot. `Defaults` to `None`.
+    - `intents` - Avoids receiving events that you do not need. `Defaults` to `False`.
     - `online_status` - Whether to set the bot's online status to `online`. `Defaults` to `True`.
-    - `**kwargs` - Any other parameters to use for the bot.
-
-        - `device_id` - The device id to use for the bot.
-
-        - `proxy` - The proxy to use for the bot. `proxy` must be `str`.
-
-        - `disable_socket` - Whether to disable the socket.
+    - `proxy` - The proxy to use for the bot. `Defaults` to `None`.
 
     ----------------------------
     When should I use `Bot` instead of `Client`?
 
     - If you want to create a bot that responds to commands or events.
     - `Client` does not respond to commands or events.
 
@@ -209,45 +204,49 @@
         bot.run(email="email", password="password")
         ```
     """
     def __init__(
         self,
         command_prefix: Optional[str] = "!",
         community_id: Union[str, int] = None,
-        online_status: bool = True, 
-        **kwargs):
+        device_id: str = None,
+        intents: bool = False,
+        online_status: bool = False,
+        proxy: str = None
+        ):
 
-        for key, value in kwargs.items(): setattr(self, key, value)
         self._debug:            bool = check_debugger()
+        self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
         self.command_prefix:    Optional[str] = command_prefix
         self.community_id:      Union[str, int] = community_id
         self.online_status:     bool = online_status
-        self.device_id:         Optional[str] = kwargs.get("device_id") or device_id()
+        self.device_id:         Optional[str] = device_id or generate_device_id()
         self.request:           RequestHandler = RequestHandler(
                                 bot = self,
-                                proxy=kwargs.get("proxy")
+                                proxy=proxy
                                 )
         self.community:         Community = Community(
                                 bot = self,
                                 session=self.request,
                                 community_id=self.community_id
                                 )
         self.account:           Account = Account(
                                 session=self.request
                                 )
 
         if self.community_id:   self.set_community_id(community_id)
 
         WSClient.__init__(self)
 
+
     @property
     def debug(self) -> bool:
         """
         Whether or not debug mode is enabled.
 
         :return: True if debug mode is enabled, False otherwise.
         :rtype: bool
@@ -276,14 +275,48 @@
         **Note:** This setter only sets the debug mode state and cannot be used to retrieve the debug mode state. To retrieve
         the debug mode state, use the `self.debug` property.
         """
         self._debug = value
 
 
     @property
+    def intents(self) -> bool:
+        """
+        Whether or not intents are enabled.
+
+        :return: True if intents are enabled, False otherwise.
+        :rtype: bool
+
+        This property returns whether or not intents are enabled. Intents allow the bot to use additional features such as
+        `ctx.wait_for_message()`.
+
+        **Note:** This property only returns the intents state and cannot be used to set the intents state. To set the intents
+        state, use the `self._intents` attribute directly.
+        """
+        return self._intents
+    
+
+    @intents.setter
+    def intents(self, value: bool) -> None:
+        """
+        Sets the intents state.
+
+        :param value: True to enable intents, False to disable them.
+        :type value: bool
+        :return: None
+
+        This setter sets the intents state. Intents allow the bot to use additional features such as `ctx.wait_for_message()`.
+
+        **Note:** This setter only sets the intents state and cannot be used to retrieve the intents state. To retrieve the
+        intents state, use the `self.intents` property.
+        """
+        self._intents = value
+
+
+    @property
     def is_ready(self) -> bool:
         """
         Whether or not the bot is ready.
 
         :return: True if the bot is ready, False otherwise.
         :rtype: bool
 
@@ -568,15 +601,15 @@
         self.request.sid: str = self.sid
         self.request.userId: str = self.userId
         self.is_authenticated: bool = True
 
         if hasattr(self.request, "email") and self._cached:
             cache_login(email=self.request.email, device=self.device_id, sid=self.sid)
 
-        if all([not self.is_ready, not hasattr(self, "disable_socket") or not self.disable_socket]):
+        if not self.is_ready:
             self.is_ready = True
             self.connect()
 
         if self.debug:
             print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
 
         return response
```

### Comparing `pymino-1.1.8.6/pymino/client.py` & `pymino-1.1.8.7/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/account.py` & `pymino-1.1.8.7/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/async_community.py` & `pymino-1.1.8.7/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/async_context.py` & `pymino-1.1.8.7/pymino/ext/async_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     `Context` - This handles the event context.
 
     `**Parameters**``
     - `message` - The message which triggered the event.
     - `session` - The session we will use to send requests.
 
     """
-    def __init__(self, message: Message, loop: AbstractEventLoop, session):
+    def __init__(self, message: Message, loop: AbstractEventLoop, session, intents: bool):
+        self.intents:   bool = intents
         self.request    = session
         self.loop:      AbstractEventLoop = loop
         self.message:   Message = message
         self.userId:    str = session.userId
 
 
     @property
@@ -127,14 +128,17 @@
             await self.request.handler(
                 method = "DELETE",
                 url = f"/{self.communityId}/s/chat/thread/{self.message.chatId}/message/{delete_message.messageId}"
             ))
 
 
     async def wait_for_message(self, message: str, timeout: int = 10) -> Message:
+        if not self.intents:
+            raise IntentsNotEnabled
+
         start = time()
         cache = Cache("cache")
 
         while time() - start < timeout:
             cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
 
             if cached_message == message:
```

### Comparing `pymino-1.1.8.6/pymino/ext/async_event_handler.py` & `pymino-1.1.8.7/pymino/ext/async_event_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -698,28 +698,29 @@
         event: str,
         data: Union[Message, OnlineMembers, Notification, AsyncContext]
         ) -> Union[AsyncContext, None]:
         """
         `_handle_event` is a function that handles events.
         """
         with suppress(KeyError):
-            context = self.context(data, self.loop, self.request)
 
-            if event == "text_message":
-                if not self.command_exists(
-                    command_name=data.content[len(self.command_prefix):].split(" ")[0]
-                    ):
-                    self._add_cache(data.chatId, data.author.userId, data.content)
+            if event in self._events:
+                context = self.context(data, self.loop, self.request, self.intents)
 
-                return await self._handle_command(data=data, context=context)
+                if event == "text_message":
+                    if not self.command_exists(
+                        command_name=data.content[len(self.command_prefix):].split(" ")[0]
+                    ) and self.intents:
+                        self._add_cache(data.chatId, data.author.userId, data.content)
 
+                    return await self._handle_command(data=data, context=context)
 
-            if event in self._events:
-                if event in {
+                elif event in {
                     "user_online",
                     "member_set_you_host",
                     "member_set_you_cohost",
                     "member_remove_your_cohost",
                 }:
                     return await self._events[event](data)
+
                 else:
                     return await self._handle_all_events(event=event, data=data, context=context)
```

### Comparing `pymino-1.1.8.6/pymino/ext/async_socket.py` & `pymino-1.1.8.7/pymino/ext/async_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,36 +109,40 @@
 
         
     async def run_forever(self) -> None:
         if self.session:
             await self.session.close()
             del self.session
 
-
-        async with create_client_session() as session:
-            self.session = session
-            ws_data = f"{device_id()}|{int(time() * 1000)}"
-            self.ws = await session.ws_connect(
-                url=f"{await self.fetch_ws_url()}/?{urlencode({'signbody': ws_data})}",
-                headers={
-                    "NDCDEVICEID": device_id(),
-                    "NDCAUTH": f"sid={self.sid}",
-                    "NDC-MSG-SIG": generate_signature(ws_data)
-                }
-            )
-
-            if not self.tasks:
-                await asyncio.gather(
-                    self._ready(),
-                    self.start_worker_pool(),
-                    alive_loop(self),
-                    self.websocket_forever()
+        try:
+            async with create_client_session() as session:
+                self.session = session
+                ws_data = f"{device_id()}|{int(time() * 1000)}"
+                self.ws = await session.ws_connect(
+                    url=f"{await self.fetch_ws_url()}/?{urlencode({'signbody': ws_data})}",
+                    headers={
+                        "NDCDEVICEID": device_id(),
+                        "NDCAUTH": f"sid={self.sid}",
+                        "NDC-MSG-SIG": generate_signature(ws_data)
+                    }
                 )
-                
-            
+
+                if not self.tasks:
+                    await asyncio.gather(
+                        self._ready(),
+                        self.start_worker_pool(),
+                        alive_loop(self),
+                        self.websocket_forever()
+                    )
+        except Exception as e:
+            await self.logger(f"Error: {e}")
+            await asyncio.sleep(5)
+            await self.reconnect()
+   
+
     async def _handle_message(self, message: dict) -> None:
         _message: Message = Message(message)
 
         if self.userId == _message.userId:
             return None
 
         None if any([_message.ndcId is None, _message.ndcId == 0]) else self._communities.add(_message.ndcId)
@@ -188,15 +192,14 @@
 
 
     async def _activity_status(self) -> None:
         for comId in self._communities:
 
             if self.online_status:
                 try:
-                    await self.community.online_status(comId=comId)
                     await self.community.send_active(comId=comId,
                     timers=[{"start": int(time()), "end": int(time()) + 300}]
                     )
                 except Exception:
                     self.online_status = False
 
             await asyncio.sleep(randint(5, 10))
```

### Comparing `pymino-1.1.8.6/pymino/ext/community.py` & `pymino-1.1.8.7/pymino/ext/community.py`

 * *Files 1% similar despite different names*

```diff
@@ -6087,8 +6087,174 @@
                 ]
             }
 
         return UserProfile(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id or comId}/s/user-profile/{self.userId}",
             data = data
-        ))
+        ))
+    
+
+    @community
+    def change_username(self, username: str, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile username.
+
+        :param username: The new username for the user profile.
+        :type username: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile username.
+
+        `UserProfile`:
+
+        - `username` (str): The username of the user.
+
+        **Example usage:**
+
+        >>> profile = client.community.edit_profile_username("JohnDoe")
+        ... print(profile.username)
+        """
+        return self.edit_profile(username=username, comId=comId)
+    
+
+    @community
+    def change_icon(self, icon: str, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile icon.
+
+        :param icon: The new icon image file for the user profile.
+        :type icon: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile icon.
+
+        `UserProfile`:
+
+        - `icon` (str): The URL of the icon image.
+
+        **Example usage:**
+
+        >>> profile = client.community.edit_profile_icon("path/to/icon.jpg")
+        ... print(profile.icon)
+        """
+        return self.edit_profile(icon=icon, comId=comId)
+    
+
+    @community
+    def edit_profile_background(self, backgroundImage: str, backgroundColor: str = None, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile background.
+
+        :param backgroundImage: The new background image file for the user profile.
+        :type backgroundImage: str
+        :param backgroundColor: The new background color for the user profile.
+        :type backgroundColor: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile background.
+
+        `UserProfile`:
+
+        - `backgroundImage` (str): The URL of the background image.
+        - `backgroundColor` (str): The background color of the user profile.
+
+        **Example usage:**
+
+        >>> profile = client.community.edit_profile_background("path/to/background.jpg", "#FFFFFF")
+        ... print(profile.backgroundImage)
+        ... print(profile.backgroundColor)
+        """
+        return self.edit_profile(backgroundImage=backgroundImage, backgroundColor=backgroundColor, comId=comId)
+    
+
+    @community
+    def edit_profile_titles(self, titles: list, colors: list, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile custom titles.
+
+        :param titles: A list of custom titles to set.
+        :type titles: list
+        :param colors: A list of colors corresponding to the custom titles.
+        :type colors: list
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile custom titles.
+
+        `UserProfile`:
+
+        - `titles` (list): A list of custom titles.
+        - `colors` (list): A list of colors corresponding to the custom titles.
+
+        **Example usage:**
+
+        >>> titles = ["Title 1", "Title 2"]
+        ... colors = ["#FF0000", "#00FF00"]
+        ... profile = client.community.edit_profile_titles(titles, colors)
+        ... print(profile.titles)
+        ... print(profile.colors)
+        """
+        return self.edit_profile(titles=titles, colors=colors, comId=comId)
+    
+
+    @community
+    def edit_profile_default_bubble(self, defaultBubbleId: str, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile default bubble.
+
+        :param defaultBubbleId: The ID of the default bubble to set.
+        :type defaultBubbleId: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile default bubble.
+
+        `UserProfile`:
+
+        - `defaultBubbleId` (str): The ID of the default bubble.
+
+        **Example usage:**
+
+        >>> profile = client.community.edit_profile_default_bubble("bubble123")
+        ... print(profile.defaultBubbleId)
+        """
+        return self.edit_profile(defaultBubbleId=defaultBubbleId, comId=comId)
+    
+
+    @community
+    def chat_request_privilege(self, privilege: bool, comId: Union[str, int] = None) -> UserProfile:
+        """
+        Edits the user profile chat request privilege.
+
+        :param privilege: Whether or not to enable chat request privilege.
+        :type privilege: bool
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile chat request privilege.
+
+        `UserProfile`:
+
+        - `chatRequestPrivilege` (bool): Whether or not chat request privilege is enabled.
+
+        **Example usage:**
+
+        >>> profile = client.community.chat_request_privilege(True)
+        ... print(profile.chatRequestPrivilege)
+        """
+        return self.edit_profile(chatRequestPrivilege=1 if privilege else 2, comId=comId)
```

### Comparing `pymino-1.1.8.6/pymino/ext/context.py` & `pymino-1.1.8.7/pymino/ext/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     `Context` - This handles the event context.
 
     `**Parameters**``
     - `message` - The message which triggered the event.
     - `session` - The session we will use to send requests.
 
     """
-    def __init__(self, message: Message, session):
+    def __init__(self, message: Message, session, intents: bool):
+        self.intents:   bool = intents
         self.message:   Message = message
         self.userId:    str = session.userId
         self.request    = session
 
     @property
     def author(self) -> MessageAuthor:
         """The author of the message."""
@@ -83,15 +84,16 @@
             "mediaValue": kwargs.get("mediaValue"),
             "mediaUploadValue": kwargs.get("mediaUploadValue"),
             "stickerId": kwargs.get("stickerId"),
             "attachedObject": kwargs.get("attachedObject"),
             "uid": self.userId
             } 
 
-    def __message__(self, **kwargs) -> dict: return PrepareMessage(**kwargs).json()
+    def __message__(self, **kwargs) -> dict:
+        return PrepareMessage(**kwargs).json()
 
     def __send_message__(self, **kwargs) -> CMessage:
         return CMessage(self.request.handler(
             method = "POST",
             url = self.__message_endpoint__,
             data = self.__message__(**kwargs)
             ))
@@ -139,14 +141,17 @@
                 ctx.send(content="You took too long to verify yourself. You have been kicked from the chat.", delete_after=TIMEOUT)
                 return bot.community.kick(userId=ctx.author.userId, chatId=ctx.chatId, allowRejoin=True, comId=ctx.comId)
 
             else:
                 ctx.send(content="You have been verified!", delete_after=TIMEOUT)
         ```
         """
+        if not self.intents:
+            raise IntentsNotEnabled
+
         start = time()
         cache = Cache("cache")
         
         while time() - start < timeout:
             cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
 
             if cached_message == message:
@@ -791,22 +796,20 @@
             return func
         return decorator
 
 
     def _add_cache(self, chatId: str, userId: str, content: str):
         if self._wait_for.get(f"{chatId}_{userId}") is not None:
             self._wait_for.clear(f"{chatId}_{userId}")
-            print("Cleared cache.")
 
         self._wait_for.add(
             key=f"{chatId}_{userId}",
             value=content,
             expire=90
             )
-        print("Added cache.")
 
 
     def on_image_message(self):
         def decorator(func: Callable) -> Callable:
             self._events["image_message"] = func
             return func
         return decorator
@@ -1226,28 +1229,29 @@
         event: str,
         data: Union[Message, OnlineMembers, Notification, Context]
         ) -> Union[Context, None]:
         """
         `_handle_event` is a function that handles events.
         """
         with suppress(KeyError):
-            context = self.context(data, self.request)
 
-            if event == "text_message":
-                if not self.command_exists(
-                    command_name=data.content[len(self.command_prefix):].split(" ")[0]
-                    ):
-                    self._add_cache(data.chatId, data.author.userId, data.content)
+            if event in self._events:
+                context = self.context(data, self.request, self.intents)
 
-                return self._handle_command(data=data, context=context)
+                if event == "text_message":
+                    if all([self.intents, not self.command_exists(
+                        command_name=data.content[len(self.command_prefix):].split(" ")[0]
+                        )]):
+                            self._add_cache(data.chatId, data.author.userId, data.content)
 
+                    return self._handle_command(data=data, context=context)
 
-            if event in self._events:
-                if event in {
+                elif event in {
                     "user_online",
                     "member_set_you_host",
                     "member_set_you_cohost",
                     "member_remove_your_cohost",
                 }:
                     return self._events[event](data)
+
                 else:
                     return self._handle_all_events(event=event, data=data, context=context)
```

### Comparing `pymino-1.1.8.6/pymino/ext/dispatcher.py` & `pymino-1.1.8.7/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/api_response.py` & `pymino-1.1.8.7/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/chat_threads.py` & `pymino-1.1.8.7/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/comments.py` & `pymino-1.1.8.7/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/enums.py` & `pymino-1.1.8.7/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/exceptions.py` & `pymino-1.1.8.7/pymino/ext/entities/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,8 +492,14 @@
             "Server returned a null response. Possible crash content in the requested data."
             )
         
 class PingFailed(Exception):
     def __init__(self):
         super().__init__(
             "Ping failed. Please make sure you are logged in and try again."
+            )
+        
+class IntentsNotEnabled(Exception):
+    def __init__(self):
+        super().__init__(
+            "Intents are not enabled. Please enable them in your Bot instance and try again."
             )
```

### Comparing `pymino-1.1.8.6/pymino/ext/entities/general.py` & `pymino-1.1.8.7/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/handlers.py` & `pymino-1.1.8.7/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/link_info.py` & `pymino-1.1.8.7/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/messages.py` & `pymino-1.1.8.7/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/notification.py` & `pymino-1.1.8.7/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/userprofile.py` & `pymino-1.1.8.7/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/entities/wsevents.py` & `pymino-1.1.8.7/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/handle_queue.py` & `pymino-1.1.8.7/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/socket.py` & `pymino-1.1.8.7/pymino/ext/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 
 
 class WSClient(EventHandler):
     """
     `WSClient` is a class that handles the websocket.
     """
     def __init__(self):
-        self.ws:            WebSocketApp = None
-        self.online_status: bool = True        
+        self.ws:            WebSocketApp = None      
         self._communities:  set = set()
         self.event_types:   dict =  EventTypes().events
         self.notif_types:   dict =  NotifTypes().notifs
         self.dispatcher:    MessageDispatcher = MessageDispatcher()
         self.channel:       Optional[Channel] = None
         self.orjson:        bool = orjson_exists()
         
         self.dispatcher.register(10, self._handle_notification)
         self.dispatcher.register(201, self._handle_agora_channel)
         self.dispatcher.register(400, self._handle_user_online)
         self.dispatcher.register(1000, self._handle_message)
+
         EventHandler.__init__(self)
 
 
     def fetch_ws_url(self) -> str:
         return f"wss://ws{randint(1, 4)}.aminoapps.com"
 
 
@@ -181,15 +181,14 @@
 
     def _activity_status(self) -> None:
         """Sets the user's activity status to online."""
         for comId in self._communities:
 
             if self.online_status:
                 try:
-                    self.community.online_status(comId=comId)
                     self.community.send_active(comId=comId,
                     timers=[{"start": int(time()), "end": int(time()) + 300}]
                     )
                 except Exception:
                     self.online_status = False
 
             delay(randint(5, 10))
```

### Comparing `pymino-1.1.8.6/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.8.7/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/utilities/commands.py` & `pymino-1.1.8.7/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/utilities/generate.py` & `pymino-1.1.8.7/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino/ext/utilities/request_handler.py` & `pymino-1.1.8.7/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/pymino.egg-info/PKG-INFO` & `pymino-1.1.8.7/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.6
+Version: 1.1.8.7
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.6 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.7 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.6/pymino.egg-info/SOURCES.txt` & `pymino-1.1.8.7/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.6/setup.cfg` & `pymino-1.1.8.7/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e38 2e36 0d0a 6175  on = 1.1.8.6..au
+00000020: 6f6e 203d 2031 2e31 2e38 2e37 0d0a 6175  on = 1.1.8.7..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.8.6/setup.py` & `pymino-1.1.8.7/setup.py`

 * *Files identical despite different names*

