# Comparing `tmp/pymino-1.1.8.7.tar.gz` & `tmp/pymino-1.1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\New folder (4)\dist\.tmp-jdfef514\pymino-1.1.8.7.tar", last modified: Sun Jun 11 14:03:44 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\New folder (4)\dist\.tmp-1p8cyq0e\pymino-1.1.8.8.tar", last modified: Sun Jun 11 21:14:45 2023, max compression
```

## Comparing `pymino-1.1.8.7.tar` & `pymino-1.1.8.8.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.662464 pymino-1.1.8.7/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.7/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-06-11 14:03:44.662464 pymino-1.1.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.590023 pymino-1.1.8.7/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-11 13:45:06.000000 pymino-1.1.8.7/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.8.7/pymino/async_bot.py
--rw-rw-rw-   0        0        0    28459 2023-06-11 13:40:20.000000 pymino-1.1.8.7/pymino/bot.py
--rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.8.7/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.633671 pymino-1.1.8.7/pymino/ext/
--rw-rw-rw-   0        0        0      474 2023-06-08 05:17:39.000000 pymino-1.1.8.7/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.8.7/pymino/ext/account.py
--rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.8.7/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.8.7/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    23958 2023-06-11 13:57:44.000000 pymino-1.1.8.7/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.8.7/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   291593 2023-06-10 01:27:27.000000 pymino-1.1.8.7/pymino/ext/community.py
--rw-rw-rw-   0        0        0    41528 2023-06-11 13:55:44.000000 pymino-1.1.8.7/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.7/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.654999 pymino-1.1.8.7/pymino/ext/entities/
--rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.8.7/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.8.7/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.8.7/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.8.7/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.7/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.8.7/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.8.7/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4763 2023-06-10 01:04:26.000000 pymino-1.1.8.7/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.8.7/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.8.7/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.8.7/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.7/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.7/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.7/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.8.7/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.661447 pymino-1.1.8.7/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      118 2023-05-28 22:35:54.000000 pymino-1.1.8.7/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.8.7/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.7/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.7/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.8.7/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:03:44.607383 pymino-1.1.8.7/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1153 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 14:03:44.000000 pymino-1.1.8.7/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-11 14:03:44.664423 pymino-1.1.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:14:45.699823 pymino-1.1.8.8/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.8/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-06-11 21:14:45.700319 pymino-1.1.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 21:14:45.632397 pymino-1.1.8.8/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-11 21:14:12.000000 pymino-1.1.8.8/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.8.8/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30128 2023-06-11 20:06:18.000000 pymino-1.1.8.8/pymino/bot.py
+-rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.8.8/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:14:45.666591 pymino-1.1.8.8/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.8.8/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.8.8/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.8.8/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.8.8/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    23958 2023-06-11 13:57:44.000000 pymino-1.1.8.8/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.8.8/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   292004 2023-06-11 18:06:25.000000 pymino-1.1.8.8/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     2045 2023-06-11 20:01:07.000000 pymino-1.1.8.8/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    41963 2023-06-11 20:52:12.000000 pymino-1.1.8.8/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.8/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:14:45.686927 pymino-1.1.8.8/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.8.8/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.8.8/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.8.8/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.8.8/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.8/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.8.8/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.8.8/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4763 2023-06-10 01:04:26.000000 pymino-1.1.8.8/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.8.8/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.8.8/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.8.8/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.8/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.8/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.8/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.8.8/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:14:45.698831 pymino-1.1.8.8/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.8.8/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.8.8/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0     9402 2023-06-11 21:09:40.000000 pymino-1.1.8.8/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.8/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1937 2023-06-11 17:27:37.000000 pymino-1.1.8.8/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.8/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2927 2023-06-11 17:26:12.000000 pymino-1.1.8.8/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2153 2023-06-11 17:29:29.000000 pymino-1.1.8.8/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.8.8/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:14:45.646750 pymino-1.1.8.8/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-06-11 21:14:45.000000 pymino-1.1.8.8/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1323 2023-06-11 21:14:45.000000 pymino-1.1.8.8/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:14:45.000000 pymino-1.1.8.8/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-11 21:14:45.000000 pymino-1.1.8.8/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 21:14:45.000000 pymino-1.1.8.8/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-11 21:14:45.707262 pymino-1.1.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.8/setup.py
```

### Comparing `pymino-1.1.8.7/LICENSE` & `pymino-1.1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/PKG-INFO` & `pymino-1.1.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.7
+Version: 1.1.8.8
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
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.7 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.8 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.7/README.md` & `pymino-1.1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/__init__.py` & `pymino-1.1.8.8/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.8.7'
+__version__ = '1.1.8.8'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.8.7/pymino/async_bot.py` & `pymino-1.1.8.8/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/bot.py` & `pymino-1.1.8.8/pymino/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from threading import Thread
 from typing import Optional, Union
 from time import perf_counter, time
 
+from .ext.console import *
 from .ext.entities import *
 from .ext.socket import WSClient
 from .ext.account import Account
 from .ext.community import Community
 from .ext.utilities.request_handler import RequestHandler
 from .ext.utilities.generate import device_id as generate_device_id
 
@@ -205,20 +207,22 @@
         ```
     """
     def __init__(
         self,
         command_prefix: Optional[str] = "!",
         community_id: Union[str, int] = None,
         device_id: str = None,
+        console_enabled: bool = False,
         intents: bool = False,
         online_status: bool = False,
         proxy: str = None
         ):
 
         self._debug:            bool = check_debugger()
+        self._console_enabled:  bool = console_enabled
         self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
         self.command_prefix:    Optional[str] = command_prefix
@@ -273,14 +277,49 @@
         during development.
 
         **Note:** This setter only sets the debug mode state and cannot be used to retrieve the debug mode state. To retrieve
         the debug mode state, use the `self.debug` property.
         """
         self._debug = value
 
+    
+    @property
+    def console_enabled(self) -> bool:
+        """
+        Whether or not the CONSOLE is enabled.
+
+        :return: True if the CONSOLE is enabled, False otherwise.
+        :rtype: bool
+
+        This property returns whether or not the CONSOLE is enabled. The CONSOLE can be used to interact with the bot and access
+        additional features such as the console.
+
+        **Note:** This property only returns the CONSOLE state and cannot be used to set the CONSOLE state. To set the CONSOLE state, use
+        the `self._console_enabled` attribute directly.
+        """
+        return self._console_enabled
+    
+
+    @console_enabled.setter
+    def console_enabled(self, value: bool) -> None:
+        """
+        Sets the CONSOLE state.
+
+        :param value: True to enable the CONSOLE, False to disable it.
+        :type value: bool
+        :return: None
+
+        This setter sets the CONSOLE state. The CONSOLE can be used to interact with the bot and access additional features such as
+        the console.
+
+        **Note:** This setter only sets the CONSOLE state and cannot be used to retrieve the CONSOLE state. To retrieve the CONSOLE state,
+        use the `self.console_enabled` property.
+        """
+        self._console_enabled = value
+
 
     @property
     def intents(self) -> bool:
         """
         Whether or not intents are enabled.
 
         :return: True if intents are enabled, False otherwise.
@@ -608,16 +647,23 @@
         if not self.is_ready:
             self.is_ready = True
             self.connect()
 
         if self.debug:
             print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
 
+        Thread(target=self.__run_console__).start()
         return response
 
+    
+    def __run_console__(self) -> None:
+        if self.console_enabled:
+            self._debug = False
+            Console(self).fetch_menu()
+
 
     def fetch_account(self) -> dict:
         """
         Fetches the account information for the authenticated user.
 
         :return: A dictionary containing the user's account information.
         :rtype: dict
```

### Comparing `pymino-1.1.8.7/pymino/client.py` & `pymino-1.1.8.8/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/account.py` & `pymino-1.1.8.8/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/async_community.py` & `pymino-1.1.8.8/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/async_context.py` & `pymino-1.1.8.8/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/async_event_handler.py` & `pymino-1.1.8.8/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/async_socket.py` & `pymino-1.1.8.8/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/community.py` & `pymino-1.1.8.8/pymino/ext/community.py`

 * *Files 1% similar despite different names*

```diff
@@ -4047,14 +4047,23 @@
 
     @community
     def send_message(self, chatId: str, content: str, comId: Union[str, int] = None) -> CMessage:
         return CMessage(self.session.handler(
             method = "POST", url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/message",
             data = PrepareMessage(content=content).json()
             ))
+    
+
+    @community
+    def reply_message(self, chatId: str, messageId: str, content: str, comId: Union[str, int] = None) -> CMessage:
+        return CMessage(self.session.handler(
+            method = "POST", url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/message",
+            data = PrepareMessage(content=content, replyMessageId=messageId
+            ).json()))
+
 
     @community
     def send_image(self, chatId: str, image: BinaryIO = None, comId: Union[str, int] = None) -> CMessage:
         return CMessage(self.session.handler(
             method = "POST", url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/message",
             data = PrepareMessage(
                 mediaType = 100,
```

### Comparing `pymino-1.1.8.7/pymino/ext/context.py` & `pymino-1.1.8.8/pymino/ext/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -732,32 +732,37 @@
         if (not self.command_exists(command_name) or
                 self.command_prefix != data.content[:len(self.command_prefix)]):
 
             if (command_name == "help" and
                     data.content == f"{self.command_prefix}help"):
                 return context.reply(self._commands.__help__())
 
-            elif "text_message" in self._events:
-                return self._handle_all_events(event="text_message", data=data, context=context)
+            elif any(
+                event in self._events
+                for event in {"text_message", "_console_text_message"}
+            ):
+                for event in {"text_message", "_console_text_message"}:
+                    self._handle_all_events(event=event, data=data, context=context)
+                return None
 
             else:
                 return None
 
         if data.content[:len(self.command_prefix)] != self.command_prefix:
             return None
 
         message = data.content[len(self.command_prefix) + len(command_name) + 1:]
         command_name = dict(self._commands.__command_aliases__().copy()).get(command_name, command_name)
-        
+
         response = self._check_cooldown(command_name, data, context)
 
         if response  != 403:
             func = self._commands.fetch_command(command_name).func
             return func(*self._set_parameters(context=context, func=func, message=message))
-        
+
         return None
 
         
     def _check_cooldown(self, command_name: str, data: Message, context: Context) -> None:
         """`_check_cooldown` is a function that checks if a command is on cooldown."""
         if self._commands.fetch_command(command_name).cooldown > 0:
             if self._commands.fetch_cooldown(command_name, data.author.userId) > time():
@@ -791,14 +796,20 @@
 
 
     def on_text_message(self):
         def decorator(func: Callable) -> Callable:
             self._events["text_message"] = func
             return func
         return decorator
+    
+    def _console_on_text_message(self):
+        def decorator(func: Callable) -> Callable:
+            self._events["_console_text_message"] = func
+            return func
+        return decorator
 
 
     def _add_cache(self, chatId: str, userId: str, content: str):
         if self._wait_for.get(f"{chatId}_{userId}") is not None:
             self._wait_for.clear(f"{chatId}_{userId}")
 
         self._wait_for.add(
@@ -1230,26 +1241,27 @@
         data: Union[Message, OnlineMembers, Notification, Context]
         ) -> Union[Context, None]:
         """
         `_handle_event` is a function that handles events.
         """
         with suppress(KeyError):
 
-            if event in self._events:
+            if event == "text_message":
                 context = self.context(data, self.request, self.intents)
+                if all([self.intents, not self.command_exists(
+                    command_name=data.content[len(self.command_prefix):].split(" ")[0]
+                    )]):
+                        self._add_cache(data.chatId, data.author.userId, data.content)
 
-                if event == "text_message":
-                    if all([self.intents, not self.command_exists(
-                        command_name=data.content[len(self.command_prefix):].split(" ")[0]
-                        )]):
-                            self._add_cache(data.chatId, data.author.userId, data.content)
-
-                    return self._handle_command(data=data, context=context)
+                self._handle_command(data=data, context=context)
+            
+            if event in self._events:
+                context = self.context(data, self.request, self.intents)
 
-                elif event in {
+                if event in {
                     "user_online",
                     "member_set_you_host",
                     "member_set_you_cohost",
                     "member_remove_your_cohost",
                 }:
                     return self._events[event](data)
```

### Comparing `pymino-1.1.8.7/pymino/ext/dispatcher.py` & `pymino-1.1.8.8/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/api_response.py` & `pymino-1.1.8.8/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/chat_threads.py` & `pymino-1.1.8.8/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/comments.py` & `pymino-1.1.8.8/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/enums.py` & `pymino-1.1.8.8/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/exceptions.py` & `pymino-1.1.8.8/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/general.py` & `pymino-1.1.8.8/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/handlers.py` & `pymino-1.1.8.8/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/link_info.py` & `pymino-1.1.8.8/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/messages.py` & `pymino-1.1.8.8/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/notification.py` & `pymino-1.1.8.8/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/userprofile.py` & `pymino-1.1.8.8/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/entities/wsevents.py` & `pymino-1.1.8.8/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/handle_queue.py` & `pymino-1.1.8.8/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/socket.py` & `pymino-1.1.8.8/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.8.8/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/utilities/commands.py` & `pymino-1.1.8.8/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/utilities/generate.py` & `pymino-1.1.8.8/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino/ext/utilities/request_handler.py` & `pymino-1.1.8.8/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.7/pymino.egg-info/PKG-INFO` & `pymino-1.1.8.8/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.7
+Version: 1.1.8.8
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
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.7 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.8 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.7/pymino.egg-info/SOURCES.txt` & `pymino-1.1.8.8/pymino.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 pymino/ext/__init__.py
 pymino/ext/account.py
 pymino/ext/async_community.py
 pymino/ext/async_context.py
 pymino/ext/async_event_handler.py
 pymino/ext/async_socket.py
 pymino/ext/community.py
+pymino/ext/console.py
 pymino/ext/context.py
 pymino/ext/dispatcher.py
 pymino/ext/handle_queue.py
 pymino/ext/socket.py
 pymino/ext/entities/__init__.py
 pymino/ext/entities/api_response.py
 pymino/ext/entities/chat_threads.py
@@ -33,10 +34,14 @@
 pymino/ext/entities/link_info.py
 pymino/ext/entities/messages.py
 pymino/ext/entities/notification.py
 pymino/ext/entities/userprofile.py
 pymino/ext/entities/wsevents.py
 pymino/ext/utilities/__init__.py
 pymino/ext/utilities/async_request_handler.py
+pymino/ext/utilities/chat_console.py
 pymino/ext/utilities/commands.py
+pymino/ext/utilities/community_console.py
 pymino/ext/utilities/generate.py
+pymino/ext/utilities/menu.py
+pymino/ext/utilities/profile_console.py
 pymino/ext/utilities/request_handler.py
```

### Comparing `pymino-1.1.8.7/setup.cfg` & `pymino-1.1.8.8/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e38 2e37 0d0a 6175  on = 1.1.8.7..au
+00000020: 6f6e 203d 2031 2e31 2e38 2e38 0d0a 6175  on = 1.1.8.8..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.8.7/setup.py` & `pymino-1.1.8.8/setup.py`

 * *Files identical despite different names*

