# Comparing `tmp/pymino-1.1.8.9.tar.gz` & `tmp/pymino-1.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\New folder (4)\dist\.tmp-zl99s890\pymino-1.1.8.9.tar", last modified: Sun Jun 11 21:22:54 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\New folder (4)\dist\.tmp-mhkyc_ku\pymino-1.1.9.1.tar", last modified: Sun Jun 11 21:33:16 2023, max compression
```

## Comparing `pymino-1.1.8.9.tar` & `pymino-1.1.9.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 21:22:54.721812 pymino-1.1.8.9/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.9/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-06-11 21:22:54.721812 pymino-1.1.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 21:22:54.659317 pymino-1.1.8.9/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-11 21:22:08.000000 pymino-1.1.8.9/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.8.9/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30128 2023-06-11 20:06:18.000000 pymino-1.1.8.9/pymino/bot.py
--rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.8.9/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:22:54.690565 pymino-1.1.8.9/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.8.9/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.8.9/pymino/ext/account.py
--rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.8.9/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.8.9/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    23958 2023-06-11 13:57:44.000000 pymino-1.1.8.9/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.8.9/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   292004 2023-06-11 18:06:25.000000 pymino-1.1.8.9/pymino/ext/community.py
--rw-rw-rw-   0        0        0     2045 2023-06-11 20:01:07.000000 pymino-1.1.8.9/pymino/ext/console.py
--rw-rw-rw-   0        0        0    41963 2023-06-11 20:52:12.000000 pymino-1.1.8.9/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.9/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:22:54.708916 pymino-1.1.8.9/pymino/ext/entities/
--rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.8.9/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.8.9/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.8.9/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.8.9/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.9/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.8.9/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.8.9/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.8.9/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.8.9/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.8.9/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.8.9/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.9/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.9/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.9/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.8.9/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:22:54.720325 pymino-1.1.8.9/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.8.9/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.8.9/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0     9402 2023-06-11 21:09:40.000000 pymino-1.1.8.9/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.9/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1937 2023-06-11 17:27:37.000000 pymino-1.1.8.9/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.9/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2927 2023-06-11 17:26:12.000000 pymino-1.1.8.9/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2153 2023-06-11 17:29:29.000000 pymino-1.1.8.9/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.8.9/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:22:54.673700 pymino-1.1.8.9/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-06-11 21:22:54.000000 pymino-1.1.8.9/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1323 2023-06-11 21:22:54.000000 pymino-1.1.8.9/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 21:22:54.000000 pymino-1.1.8.9/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-11 21:22:54.000000 pymino-1.1.8.9/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 21:22:54.000000 pymino-1.1.8.9/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-11 21:22:54.723796 pymino-1.1.8.9/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:33:16.239827 pymino-1.1.9.1/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.1/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-06-11 21:33:16.240323 pymino-1.1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 21:33:16.170386 pymino-1.1.9.1/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-11 21:32:23.000000 pymino-1.1.9.1/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.1/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30128 2023-06-11 20:06:18.000000 pymino-1.1.9.1/pymino/bot.py
+-rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.9.1/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:33:16.204115 pymino-1.1.9.1/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.1/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.1/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.9.1/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.1/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    23958 2023-06-11 13:57:44.000000 pymino-1.1.9.1/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.1/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   292004 2023-06-11 18:06:25.000000 pymino-1.1.9.1/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     2044 2023-06-11 21:28:54.000000 pymino-1.1.9.1/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    41963 2023-06-11 20:52:12.000000 pymino-1.1.9.1/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.1/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:33:16.225938 pymino-1.1.9.1/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.9.1/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.9.1/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.9.1/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.1/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.1/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.9.1/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.1/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.1/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.1/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.9.1/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.1/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.1/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.1/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.1/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.1/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:33:16.238834 pymino-1.1.9.1/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.1/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.1/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0     9376 2023-06-11 21:32:02.000000 pymino-1.1.9.1/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.1/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1932 2023-06-11 21:28:04.000000 pymino-1.1.9.1/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.1/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2923 2023-06-11 21:28:12.000000 pymino-1.1.9.1/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     1984 2023-06-11 21:31:52.000000 pymino-1.1.9.1/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.1/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-11 21:33:16.184274 pymino-1.1.9.1/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-06-11 21:33:16.000000 pymino-1.1.9.1/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1323 2023-06-11 21:33:16.000000 pymino-1.1.9.1/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:33:16.000000 pymino-1.1.9.1/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-11 21:33:16.000000 pymino-1.1.9.1/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 21:33:16.000000 pymino-1.1.9.1/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-11 21:33:16.247267 pymino-1.1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.1/setup.py
```

### Comparing `pymino-1.1.8.9/LICENSE` & `pymino-1.1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/PKG-INFO` & `pymino-1.1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.9
+Version: 1.1.9.1
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
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.9 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.1 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.9/README.md` & `pymino-1.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/__init__.py` & `pymino-1.1.9.1/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.8.9'
+__version__ = '1.1.9.1'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.8.9/pymino/async_bot.py` & `pymino-1.1.9.1/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/bot.py` & `pymino-1.1.9.1/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/client.py` & `pymino-1.1.9.1/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/account.py` & `pymino-1.1.9.1/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/async_community.py` & `pymino-1.1.9.1/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/async_context.py` & `pymino-1.1.9.1/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/async_event_handler.py` & `pymino-1.1.9.1/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/async_socket.py` & `pymino-1.1.9.1/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/community.py` & `pymino-1.1.9.1/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/console.py` & `pymino-1.1.9.1/pymino/ext/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,14 @@
         """
         Accepts user input prefixed with a fixed number of spaces for consistent look and feel.
 
         :param text: The prompt to be displayed to the user.
         :type text: str
         :return: User input as a string.
         """
-        return input(" " * 20 + text)
+        return input(" " * 0 + text)
 
     def fetch_menu(self):
         """
         Displays the main menu of the application to the user and processes their input.
         """
         self.menu.display()
```

### Comparing `pymino-1.1.8.9/pymino/ext/context.py` & `pymino-1.1.9.1/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/dispatcher.py` & `pymino-1.1.9.1/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/api_response.py` & `pymino-1.1.9.1/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/chat_threads.py` & `pymino-1.1.9.1/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/comments.py` & `pymino-1.1.9.1/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/enums.py` & `pymino-1.1.9.1/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/exceptions.py` & `pymino-1.1.9.1/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/general.py` & `pymino-1.1.9.1/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/handlers.py` & `pymino-1.1.9.1/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/link_info.py` & `pymino-1.1.9.1/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/messages.py` & `pymino-1.1.9.1/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/notification.py` & `pymino-1.1.9.1/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/userprofile.py` & `pymino-1.1.9.1/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/entities/wsevents.py` & `pymino-1.1.9.1/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/handle_queue.py` & `pymino-1.1.9.1/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/socket.py` & `pymino-1.1.9.1/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.9.1/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/utilities/chat_console.py` & `pymino-1.1.9.1/pymino/ext/utilities/chat_console.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,64 +20,64 @@
     - Type 'clear' to clear the chat.
 """
 
     def join_public_chat(self):
         """
         Handles joining of a public chat.
         """
-        self.console.print("Join Public Chat", 20)
+        self.console.print("Join Public Chat", 0)
         self.console.print("""
     1. Join by Chat ID
     2. Join by Link
     3. Find Public Chats To Join
     4. Back
-    """, 20)
+    """, 0)
         choice = self.console.input(">>> ")
         self.console.print()
 
         try:
             if choice == "1":
                 chat_id = self.console.input("Enter chat ID: ")
             elif choice == "2":
                 chat_link = self.console.input("Enter chat link: ")
                 chat_id = self.console.bot.community.fetch_object_id(chat_link)
             elif choice == "3":
                 self.console.clear()
-                self.console.print("Find Public Chats To Join", 20)
+                self.console.print("Find Public Chats To Join", 0)
 
                 public_chats = self.console.bot.community.fetch_public_chats(size=25)
                 for index, (chat_id, chat_title) in enumerate(zip(public_chats.chatId, public_chats.title)):
-                    self.console.print(f"{index+1}. {chat_title}({chat_id})", 20)
+                    self.console.print(f"{index+1}. {chat_title}({chat_id})", 0)
 
                 self.console.print()
                 choice = self.console.input(">>> ")
                 self.console.print()
 
                 try:
                     choice = int(choice)
                     if not (1 <= choice <= len(public_chats.chatId)):
                         raise ValueError
                     chat_id = public_chats.chatId[choice-1]
                 except ValueError:
-                    self.console.print("Invalid option. Please try again.", 20)
+                    self.console.print("Invalid option. Please try again.", 0)
                     return self.join_public_chat()
 
             elif choice == "4":
                 return self.console.menu.display()
 
             else:
-                self.console.print("Invalid option. Please try again.", 20)
+                self.console.print("Invalid option. Please try again.", 0)
                 return self.join_public_chat()
 
             self.console.bot.community.join_chat(chatId=chat_id)
-            self.console.print("Joined chat successfully.", 20)
+            self.console.print("Joined chat successfully.", 0)
             self.console.sleep(2)
 
         except Exception as e:
-            self.console.print(f"Error: {e}", 20)
+            self.console.print(f"Error: {e}", 0)
             self.console.sleep(2)
 
         return self.console.menu.display()
 
     def my_chats(self):
         """
         Lists the user's chats and allows them to interact with selected chat.
@@ -89,24 +89,24 @@
         else:
             return self.console.menu.display()
 
     def print_chats(self):
         """
         Prints the user's chats.
         """
-        self.console.print("My Chats", 20)
+        self.console.print("My Chats", 0)
         chats = self.console.bot.community.fetch_chats()
         for index, (chat_id, chat_title) in enumerate(zip(chats.chatId, chats.title)):
             if chat_title is None:
                 chat_users = self.console.bot.community.fetch_chat_members(chat_id).members.nickname[:3]
                 chat_title = ", ".join(chat_users) + "[Private Chat]"
             else:
                 chat_title = f"{chat_title}[Public Chat]"
-            self.console.print(f"{index+1}. {chat_title}({chat_id})", 20)
-        self.console.print("\nType 'back' to go back to the menu.\n", 20)
+            self.console.print(f"{index+1}. {chat_title}({chat_id})", 0)
+        self.console.print("\nType 'back' to go back to the menu.\n", 0)
 
     def select_chat(self):
         """
         Allows the user to select a chat.
 
         :return: Tuple containing chat ID and chat title, or (None, None) if back was selected.
         :rtype: Tuple[str, str]
@@ -119,38 +119,38 @@
             choice = int(choice)
             chats = self.console.bot.community.fetch_chats()
             if not (1 <= choice <= len(chats.chatId)):
                 raise ValueError
             chat_id, chat_title = chats.chatId[choice-1], chats.title[choice-1]
             return chat_id, chat_title
         except ValueError:
-            self.console.print("Invalid option. Please try again.", 20)
+            self.console.print("Invalid option. Please try again.", 0)
             return self.select_chat()
 
     def interact_with_chat(self, chat_id: str, chat_title: str):
         """
         Allows the user to interact with the selected chat.
 
         :param chat_id: ID of the chat.
         :type chat_id: str
         :param chat_title: Title of the chat.
         :type chat_title: str
         :return: None
         """
         self.replies = {}
         self.console.clear()
-        self.console.print(f"Chat: {chat_title}", 20)
+        self.console.print(f"Chat: {chat_title}", 0)
 
         self.initiate_message_listener(chat_id)
-        self.console.print(self.help_message, 20)
+        self.console.print(self.help_message, 0)
 
         while self.handle_chat_interaction(chat_id, chat_title):
             self.console.sleep(2)
 
-        self.console.print("\nReturning to Main Menu.\n", 20)
+        self.console.print("\nReturning to Main Menu.\n", 0)
         self.console.sleep(2)
         return self.console.menu.display()
 
     def initiate_message_listener(self, chat_id: str):
         """
         Initiates a message listener for the specified chat.
 
@@ -162,17 +162,17 @@
 
         @self.console.bot._console_on_text_message()
         def on_message(ctx):
             nonlocal counter
             if ctx.chatId == chat_id:
                 self.console.print()
                 self.replies[counter] = ctx.message.messageId
-                self.console.print(f"[{counter}] {ctx.author.nickname}: {ctx.message.content}", 20)
+                self.console.print(f"[{counter}] {ctx.author.nickname}: {ctx.message.content}", 0)
                 counter += 1
-                sys.stdout.write(" "*20 + ">>> ")
+                sys.stdout.write(" "*0 + ">>> ")
                 sys.stdout.flush()
 
     def handle_chat_interaction(self, chat_id: str, chat_title: str = None) -> bool:
         """
         Handles user input for interacting with the chat.
 
         :param chat_id: ID of the chat.
@@ -186,23 +186,23 @@
                 self.handle_leave(None)
                 return False
             elif message == "reply":
                 return self.handle_reply(chat_id)
             elif message == "leave":
                 return self.handle_leave(chat_id)
             elif message == "help":
-                self.console.print(self.help_message, 20)
+                self.console.print(self.help_message, 0)
                 return True
             elif message == "clear":
                 self.console.clear()
-                self.console.print(f"Chat: {chat_title}", 20)
+                self.console.print(f"Chat: {chat_title}", 0)
                 return True
             else:
                 self.console.bot.community.send_message(chatId=chat_id, content=message)
-                self.console.print(f"You: {message}", 20)
+                self.console.print(f"You: {message}", 0)
                 return True
         except (EOFError):
             self.console.print("\n")
             sys.stdout.write(">>> ")
             sys.stdout.flush()
             return True
 
@@ -211,32 +211,32 @@
         Handles replying to a message in the chat.
 
         :param chat_id: ID of the chat.
         :type chat_id: str
         :return: True if the interaction should continue, False otherwise.
         :rtype: bool
         """
-        self.console.print("Enter the message ID of the message you want to reply to.", 20)
+        self.console.print("Enter the message ID of the message you want to reply to.", 0)
         message_id = self.console.input(">>> ")
         if message_id in {"exit", "quit", ""}:
             return True
         try:
             message_id = int(message_id)
         except ValueError:
-            self.console.print("Invalid message ID. Please try again.", 20)
+            self.console.print("Invalid message ID. Please try again.", 0)
             return True
         if message_id not in self.replies:
-            self.console.print("Invalid message ID. Please try again.", 20)
+            self.console.print("Invalid message ID. Please try again.", 0)
             return True
-        self.console.print("Enter your reply.", 20)
+        self.console.print("Enter your reply.", 0)
         reply = self.console.input(">>> ")
         if reply in {"exit", "quit", ""}:
             return True
         self.console.bot.community.reply_message(chatId=chat_id, content=reply, messageId=self.replies[message_id])
-        self.console.print(f"You: {reply}", 20)
+        self.console.print(f"You: {reply}", 0)
         return True
 
     def handle_leave(self, chat_id: str) -> bool:
         """
         Handles leaving the chat.
 
         :param chat_id: ID of the chat.
@@ -245,10 +245,10 @@
         :rtype: bool
         """
         if chat_id:
             self.console.bot.community.leave_chat(chat_id)
             
         self.replies.clear()
         del self.console.bot._events["_console_text_message"]
-        self.console.print("Left chat successfully.", 20)
+        self.console.print("Left chat successfully.", 0)
         self.console.sleep(2)
         return False
```

### Comparing `pymino-1.1.8.9/pymino/ext/utilities/commands.py` & `pymino-1.1.9.1/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/utilities/community_console.py` & `pymino-1.1.9.1/pymino/ext/utilities/community_console.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,39 +14,39 @@
         """
         Prints a list of communities the user has joined.
 
         :param communities: A list of communities.
         :type communities: list of Community objects
         """
         if not communities.comId:
-            self.console.print("You are not in any communities.", 20)
+            self.console.print("You are not in any communities.", 0)
             sleep(2)
             return self.console.menu.display()
 
         for index, (community_id, community_name) in enumerate(zip(communities.comId, communities.name), start=1):
             try:
-                self.console.print(f"{index}. {community_name}({community_id})", 20)
+                self.console.print(f"{index}. {community_name}({community_id})", 0)
             except Exception:
-                self.console.print("Error occurred while fetching communities.", 20)
+                self.console.print("Error occurred while fetching communities.", 0)
                 sleep(2)
 
     def select_community(self):
         """
         Prompts the user to select a community and sets the bot's community accordingly.
         """
         communities = self.console.bot.community.joined_communities()
-        self.console.print("\nSelect a community:\n", 20)
+        self.console.print("\nSelect a community:\n", 0)
         self.print_communities(communities)
         print()
         choice = self.console.input(">>> ")
         print()
 
         try:
             choice = int(choice)
             if not (1 <= choice <= len(communities.comId)):
                 raise ValueError
         except ValueError:
-            self.console.print("Invalid option. Please try again.", 20)
+            self.console.print("Invalid option. Please try again.", 0)
             return self.select_community()
 
         self.console.bot.set_community_id(communities.comId[choice-1])
         return self.console.menu.display()
```

### Comparing `pymino-1.1.8.9/pymino/ext/utilities/generate.py` & `pymino-1.1.9.1/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino/ext/utilities/menu.py` & `pymino-1.1.9.1/pymino/ext/utilities/menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,35 +23,35 @@
         self.menu_logo += self.author
 
     def display(self):
         """
         Displays the main menu options to the user and processes their input.
         """
         self.console.clear()
-        self.console.print(self.menu_logo, 20)
-        self.console.print(self.welcome_screen(), 20)
+        self.console.print(self.menu_logo, 0)
+        self.console.print(self.welcome_screen(), 0)
         self.console.print("""
     1. Select Community
     2. Edit Profile
     3. Join Public Chat
     4. My Chats
-    """, 20)
+    """, 0)
         choice = self.console.input(">>> ")
         print()
         menu = {
             "1": self.console.community_console.select_community,
             "2": self.console.profile_console.edit_profile,
             "3": self.console.chat_console.join_public_chat,
             "4": self.console.chat_console.my_chats
         }
         if choice in menu:
             self.console.clear()
             menu[choice]()
         else:
-            self.console.print("Invalid option. Please try again.", 20)
+            self.console.print("Invalid option. Please try again.", 0)
             self.display()
 
     def welcome_screen(self):
         """
         Returns a string containing the welcome message for the user.
 
         :return: A string containing the welcome message for the user.
```

### Comparing `pymino-1.1.8.9/pymino/ext/utilities/profile_console.py` & `pymino-1.1.9.1/pymino/ext/utilities/profile_console.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,22 @@
         """
         self.console = console
 
     def edit_profile(self):
         """
         Handles editing of user profile.
         """
-        self.console.print("Edit Profile", 20)
+        self.console.print("Edit Profile", 0)
         self.console.print("""
     1. Change Username
     2. Change Bio
     3. Change Profile Picture
     4. Change Background Picture
-    5. Change Amino ID
-    6. Back
-    """, 20)
+    5. Back
+    """, 0)
         choice = self.console.input(">>> ")
 
         try:
             if choice == "6":
                 return self.console.menu.display()
 
             field_name = None
@@ -36,25 +35,22 @@
             elif choice == "2":
                 field_name = "content"
                 new_value = self.console.input("Enter new bio: ")
             elif choice == "3":
                 field_name = "icon"
                 new_value = self.console.input("Enter new profile picture URL: ")
             elif choice == "4":
-                field_name = "background"
+                field_name = "backgroundImage"
                 new_value = self.console.input("Enter new background picture URL: ")
-            elif choice == "5":
-                field_name = "aminoId"
-                new_value = self.console.input("Enter new Amino ID: ")
             else:
-                self.console.print("Invalid option. Please try again.", 20)
+                self.console.print("Invalid option. Please try again.", 0)
                 return self.edit_profile()
 
             self.console.bot.community.edit_profile(**{field_name: new_value})
-            self.console.print(f"{field_name.capitalize()} changed successfully to {new_value}.", 20)
+            self.console.print(f"{field_name.capitalize()} changed successfully to {new_value}.", 0)
             self.console.sleep(2)
 
         except Exception as e:
-            self.console.print(f"Error: {e}", 20)
+            self.console.print(f"Error: {e}", 0)
             self.console.sleep(2)
 
         return self.console.menu.display()
```

### Comparing `pymino-1.1.8.9/pymino/ext/utilities/request_handler.py` & `pymino-1.1.9.1/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/pymino.egg-info/PKG-INFO` & `pymino-1.1.9.1/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.9
+Version: 1.1.9.1
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
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.9 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.1 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.9/pymino.egg-info/SOURCES.txt` & `pymino-1.1.9.1/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.9/setup.cfg` & `pymino-1.1.9.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e38 2e39 0d0a 6175  on = 1.1.8.9..au
+00000020: 6f6e 203d 2031 2e31 2e39 2e31 0d0a 6175  on = 1.1.9.1..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.8.9/setup.py` & `pymino-1.1.9.1/setup.py`

 * *Files identical despite different names*

