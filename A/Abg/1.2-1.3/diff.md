# Comparing `tmp/Abg-1.2.tar.gz` & `tmp/Abg-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-1.2.tar", last modified: Mon Jun  5 15:18:56 2023, max compression
+gzip compressed data, was "Abg-1.3.tar", last modified: Sun Jun 11 04:04:46 2023, max compression
```

## Comparing `Abg-1.2.tar` & `Abg-1.3.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.309213 Abg-1.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/
--rw-r--r--   0 root         (0) root         (0)      210 2023-06-05 15:18:31.000000 Abg-1.2/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/chat_status/
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-05 15:18:31.000000 Abg-1.2/Abg/chat_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5273 2023-06-05 15:18:31.000000 Abg-1.2/Abg/chat_status/chat_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/conversation/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-05 15:18:31.000000 Abg-1.2/Abg/conversation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5532 2023-06-05 15:18:31.000000 Abg-1.2/Abg/conversation/conversation.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-06-05 15:18:31.000000 Abg-1.2/Abg/conversation/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      844 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3181 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/lock.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-06-05 15:18:31.000000 Abg-1.2/Abg/helpers/pyro_progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      280 2023-06-05 15:18:31.000000 Abg-1.2/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6245 2023-06-05 15:18:31.000000 Abg-1.2/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4268 2023-06-05 15:18:31.000000 Abg-1.2/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-06-05 15:18:31.000000 Abg-1.2/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11748 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.309213 Abg-1.2/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-06-05 15:18:31.000000 Abg-1.2/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 15:18:56.305213 Abg-1.2/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5827 2023-06-05 15:18:56.000000 Abg-1.2/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      798 2023-06-05 15:18:56.000000 Abg-1.2/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 15:18:56.000000 Abg-1.2/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-05 15:18:56.000000 Abg-1.2/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5827 2023-06-05 15:18:56.309213 Abg-1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3268 2023-06-05 15:18:31.000000 Abg-1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 15:18:56.309213 Abg-1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-05 15:18:31.000000 Abg-1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.720066 Abg-1.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-11 04:03:36.000000 Abg-1.3/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/chat_status/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-11 04:03:36.000000 Abg-1.3/Abg/chat_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2023-06-11 04:03:36.000000 Abg-1.3/Abg/chat_status/chat_status.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-06-11 04:03:36.000000 Abg-1.3/Abg/chat_status/custom_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/conversation/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-11 04:03:36.000000 Abg-1.3/Abg/conversation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-06-11 04:03:36.000000 Abg-1.3/Abg/conversation/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      824 2023-06-11 04:03:36.000000 Abg-1.3/Abg/conversation/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      844 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/lock.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/pyro_progress.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-06-11 04:03:36.000000 Abg-1.3/Abg/helpers/ratelimit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-11 04:03:36.000000 Abg-1.3/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6245 2023-06-11 04:03:36.000000 Abg-1.3/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2023-06-11 04:03:36.000000 Abg-1.3/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-06-11 04:03:36.000000 Abg-1.3/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11748 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.720066 Abg-1.3/Abg/patch/listen/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11641 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/listen/listen.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/listen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.720066 Abg-1.3/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-06-11 04:03:36.000000 Abg-1.3/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 04:04:46.716066 Abg-1.3/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6936 2023-06-11 04:04:46.000000 Abg-1.3/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      939 2023-06-11 04:04:46.000000 Abg-1.3/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 04:04:46.000000 Abg-1.3/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-11 04:04:46.000000 Abg-1.3/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     6936 2023-06-11 04:04:46.720066 Abg-1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-06-11 04:03:36.000000 Abg-1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 04:04:46.720066 Abg-1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-11 04:03:36.000000 Abg-1.3/setup.py
```

### Comparing `Abg-1.2/Abg/chat_status/chat_status.py` & `Abg-1.3/Abg/chat_status/chat_status.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/conversation/conversation.py` & `Abg-1.3/Abg/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/conversation/errors.py` & `Abg-1.3/Abg/conversation/errors.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/helpers/__init__.py` & `Abg-1.3/Abg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/helpers/helpers.py` & `Abg-1.3/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/helpers/http_helper.py` & `Abg-1.3/Abg/helpers/http_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from asyncio import gather
-import httpx
+# import httpx
 from aiohttp import ClientSession
 
 # Aiohttp Async Client
 aiohttpsession = ClientSession()
 
+"""
 # HTTPx Async Client
 http = httpx.AsyncClient(
     http2=True,
     verify=False,
     timeout=httpx.Timeout(40),
 )
+"""
 
 async def get(url: str, *args, **kwargs):
     async with aiohttpsession.get(url, *args, **kwargs) as resp:
         try:
             data = await resp.json()
         except Exception:
             data = await resp.text()
```

### Comparing `Abg-1.2/Abg/helpers/human_read.py` & `Abg-1.3/Abg/helpers/human_read.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/helpers/parser.py` & `Abg-1.3/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/helpers/pyro_progress.py` & `Abg-1.3/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/inline/inline_keyboard.py` & `Abg-1.3/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/inline/inline_pagination_keyboard.py` & `Abg-1.3/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/inline/reply_keyboard.py` & `Abg-1.3/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/patch/bound/message.py` & `Abg-1.3/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/patch/methods/edit_message_text.py` & `Abg-1.3/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/patch/methods/send_as_file.py` & `Abg-1.3/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg/patch/methods/send_message.py` & `Abg-1.3/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-1.2/Abg.egg-info/PKG-INFO` & `Abg-1.3/Abg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,79 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.2
+Version: 1.3
 Summary: pyrogram helpers / add-on for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abg
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/wiki
 Description: # ᴀʙɢ-ᴘʏʀᴏ :->
-        
-        > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
         > 
-        • Conversation in pyrogram
+        ### • Conversation in pyrogram
         
         ```python
-          from Abg.conversation import Askclient
-          from pyrogram import Client, filters
-          
-          app = Client("my_account")
-          read = Askclient(app)
+        from pyrogram import filters, Client
+        from pyrogram.types import Message
+        from Abg import patch  # type : ignore
+        
+        app = Client("my_account")
+        
+        @app.on_message(filters.command(["myinto"]))
+        async def my_info(self: Client, ctx: Message):
+            if not ctx.from_user:
+                return
+            name = await ctx.chat.ask("Type Your Name")
+            age = await ctx.chat.ask("Tyoe your age")
+            add = await ctx.chat.ask("Type your address")
+            await app.send_msg(
+                ctx.chat.id,
+                f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+            )
         
-          @app.on_message(filters.command("start"))
-          async def start(c: app, m: Message):
-            answer = await read.ask(m, text)
-            if answer.text:
-             print(answer.text)
-            await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
+          app.run()
+        ```
+        >
+        ### • User Rights 
         
+        ```python 
+        from Abg.chat_status import adminsOnly
+        from pyrogram import filters
+        from pyrogram.enums import ChatType
+        from pyrogram.types import Message
+        from pyrogram import Client
+        
+        app = Client("my_account")
+        
+        @app.on_message(filters.command("del"))
+        @adminsOnly("can_delete_messages")
+        async def del_msg(c: Client, m: Message):
+            if m.chat.type != ChatType.SUPERGROUP:
+                return
+        
+            if m.reply_to_message:
+                await m.delete()
+                await c.delete_messages(
+                    chat_id=m.chat.id,
+                    message_ids=m.reply_to_message.id,
+                )
+            else:
+                await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
+            return
+          
           app.run()
         ```
+        
+        
         >
-        • Keyboards
+        ### • Keyboards
         
         ```python
         from Abg.inline import InlineKeyboard, InlineButton
         
         
         keyboard = InlineKeyboard(row_width=3)
         keyboard.add(
```

#### html2text {}

```diff
@@ -1,26 +1,36 @@
-Metadata-Version: 2.1 Name: Abg Version: 1.2 Summary: pyrogram helpers / add-on
+Metadata-Version: 2.1 Name: Abg Version: 1.3 Summary: pyrogram helpers / add-on
 for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org License: MIT Download-URL: https://github.com/
 Abishnoi69/Abg/releases/latest Project-URL: Tracker, https://github.com/
 Abishnoi69/Abg/issues Project-URL: Community, https://t.me/Abg Project-URL:
 Source, https://github.com/Abishnoi69/Abg Project-URL: Documentation, https://
-github.com/Abishnoi69/Abg/wiki Description: # á´ÊÉ¢-á´ÊÊá´ :-> >
-sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´
-[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] > â¢ Conversation in pyrogram ```python
-from Abg.conversation import Askclient from pyrogram import Client, filters app
-= Client("my_account") read = Askclient(app) @app.on_message(filters.command
-("start")) async def start(c: app, m: Message): answer = await read.ask(m,
-text) if answer.text: print(answer.text) await answer.reply("Éª É¢á´á´
-á´É´sá´¡á´Ê..") app.run() ``` > â¢ Keyboards ```python from Abg.inline
-import InlineKeyboard, InlineButton keyboard = InlineKeyboard(row_width=3)
-keyboard.add( InlineButton('1', 'inline_keyboard:1'), InlineButton('2',
-'inline_keyboard:2'), InlineButton('3', 'inline_keyboard:3'), InlineButton('4',
-'inline_keyboard:4'), InlineButton('5', 'inline_keyboard:5'), InlineButton('6',
-'inline_keyboard:6'), InlineButton('7', 'inline_keyboard:7') ) ``` #### Result
+github.com/Abishnoi69/Abg/wiki Description: # á´ÊÉ¢-á´ÊÊá´ :-> > ### â¢
+Conversation in pyrogram ```python from pyrogram import filters, Client from
+pyrogram.types import Message from Abg import patch # type : ignore app =
+Client("my_account") @app.on_message(filters.command(["myinto"])) async def
+my_info(self: Client, ctx: Message): if not ctx.from_user: return name = await
+ctx.chat.ask("Type Your Name") age = await ctx.chat.ask("Tyoe your age") add =
+await ctx.chat.ask("Type your address") await app.send_msg( ctx.chat.id, f"Your
+name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}", )
+app.run() ``` > ### â¢ User Rights ```python from Abg.chat_status import
+adminsOnly from pyrogram import filters from pyrogram.enums import ChatType
+from pyrogram.types import Message from pyrogram import Client app = Client
+("my_account") @app.on_message(filters.command("del")) @adminsOnly
+("can_delete_messages") async def del_msg(c: Client, m: Message): if
+m.chat.type != ChatType.SUPERGROUP: return if m.reply_to_message: await
+m.delete() await c.delete_messages( chat_id=m.chat.id,
+message_ids=m.reply_to_message.id, ) else: await m.reply_text(text="á´¡Êá´á´
+á´á´ Êá´á´ á´¡á´É´É´á´ á´á´Êá´á´á´?") return app.run() ``` > ###
+â¢ Keyboards ```python from Abg.inline import InlineKeyboard, InlineButton
+keyboard = InlineKeyboard(row_width=3) keyboard.add( InlineButton('1',
+'inline_keyboard:1'), InlineButton('2', 'inline_keyboard:2'), InlineButton('3',
+'inline_keyboard:3'), InlineButton('4', 'inline_keyboard:4'), InlineButton('5',
+'inline_keyboard:5'), InlineButton('6', 'inline_keyboard:6'), InlineButton('7',
+'inline_keyboard:7') ) ``` #### Result
 [add_inline_button]
 ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install Abg ```
 **** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ :-> ****
 [https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
 903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ :-> ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
```

### Comparing `Abg-1.2/PKG-INFO` & `Abg-1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,79 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.2
+Version: 1.3
 Summary: pyrogram helpers / add-on for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abg
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/wiki
 Description: # ᴀʙɢ-ᴘʏʀᴏ :->
-        
-        > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
         > 
-        • Conversation in pyrogram
+        ### • Conversation in pyrogram
         
         ```python
-          from Abg.conversation import Askclient
-          from pyrogram import Client, filters
-          
-          app = Client("my_account")
-          read = Askclient(app)
+        from pyrogram import filters, Client
+        from pyrogram.types import Message
+        from Abg import patch  # type : ignore
+        
+        app = Client("my_account")
+        
+        @app.on_message(filters.command(["myinto"]))
+        async def my_info(self: Client, ctx: Message):
+            if not ctx.from_user:
+                return
+            name = await ctx.chat.ask("Type Your Name")
+            age = await ctx.chat.ask("Tyoe your age")
+            add = await ctx.chat.ask("Type your address")
+            await app.send_msg(
+                ctx.chat.id,
+                f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+            )
         
-          @app.on_message(filters.command("start"))
-          async def start(c: app, m: Message):
-            answer = await read.ask(m, text)
-            if answer.text:
-             print(answer.text)
-            await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
+          app.run()
+        ```
+        >
+        ### • User Rights 
         
+        ```python 
+        from Abg.chat_status import adminsOnly
+        from pyrogram import filters
+        from pyrogram.enums import ChatType
+        from pyrogram.types import Message
+        from pyrogram import Client
+        
+        app = Client("my_account")
+        
+        @app.on_message(filters.command("del"))
+        @adminsOnly("can_delete_messages")
+        async def del_msg(c: Client, m: Message):
+            if m.chat.type != ChatType.SUPERGROUP:
+                return
+        
+            if m.reply_to_message:
+                await m.delete()
+                await c.delete_messages(
+                    chat_id=m.chat.id,
+                    message_ids=m.reply_to_message.id,
+                )
+            else:
+                await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
+            return
+          
           app.run()
         ```
+        
+        
         >
-        • Keyboards
+        ### • Keyboards
         
         ```python
         from Abg.inline import InlineKeyboard, InlineButton
         
         
         keyboard = InlineKeyboard(row_width=3)
         keyboard.add(
```

#### html2text {}

```diff
@@ -1,26 +1,36 @@
-Metadata-Version: 2.1 Name: Abg Version: 1.2 Summary: pyrogram helpers / add-on
+Metadata-Version: 2.1 Name: Abg Version: 1.3 Summary: pyrogram helpers / add-on
 for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org License: MIT Download-URL: https://github.com/
 Abishnoi69/Abg/releases/latest Project-URL: Tracker, https://github.com/
 Abishnoi69/Abg/issues Project-URL: Community, https://t.me/Abg Project-URL:
 Source, https://github.com/Abishnoi69/Abg Project-URL: Documentation, https://
-github.com/Abishnoi69/Abg/wiki Description: # á´ÊÉ¢-á´ÊÊá´ :-> >
-sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´
-[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] > â¢ Conversation in pyrogram ```python
-from Abg.conversation import Askclient from pyrogram import Client, filters app
-= Client("my_account") read = Askclient(app) @app.on_message(filters.command
-("start")) async def start(c: app, m: Message): answer = await read.ask(m,
-text) if answer.text: print(answer.text) await answer.reply("Éª É¢á´á´
-á´É´sá´¡á´Ê..") app.run() ``` > â¢ Keyboards ```python from Abg.inline
-import InlineKeyboard, InlineButton keyboard = InlineKeyboard(row_width=3)
-keyboard.add( InlineButton('1', 'inline_keyboard:1'), InlineButton('2',
-'inline_keyboard:2'), InlineButton('3', 'inline_keyboard:3'), InlineButton('4',
-'inline_keyboard:4'), InlineButton('5', 'inline_keyboard:5'), InlineButton('6',
-'inline_keyboard:6'), InlineButton('7', 'inline_keyboard:7') ) ``` #### Result
+github.com/Abishnoi69/Abg/wiki Description: # á´ÊÉ¢-á´ÊÊá´ :-> > ### â¢
+Conversation in pyrogram ```python from pyrogram import filters, Client from
+pyrogram.types import Message from Abg import patch # type : ignore app =
+Client("my_account") @app.on_message(filters.command(["myinto"])) async def
+my_info(self: Client, ctx: Message): if not ctx.from_user: return name = await
+ctx.chat.ask("Type Your Name") age = await ctx.chat.ask("Tyoe your age") add =
+await ctx.chat.ask("Type your address") await app.send_msg( ctx.chat.id, f"Your
+name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}", )
+app.run() ``` > ### â¢ User Rights ```python from Abg.chat_status import
+adminsOnly from pyrogram import filters from pyrogram.enums import ChatType
+from pyrogram.types import Message from pyrogram import Client app = Client
+("my_account") @app.on_message(filters.command("del")) @adminsOnly
+("can_delete_messages") async def del_msg(c: Client, m: Message): if
+m.chat.type != ChatType.SUPERGROUP: return if m.reply_to_message: await
+m.delete() await c.delete_messages( chat_id=m.chat.id,
+message_ids=m.reply_to_message.id, ) else: await m.reply_text(text="á´¡Êá´á´
+á´á´ Êá´á´ á´¡á´É´É´á´ á´á´Êá´á´á´?") return app.run() ``` > ###
+â¢ Keyboards ```python from Abg.inline import InlineKeyboard, InlineButton
+keyboard = InlineKeyboard(row_width=3) keyboard.add( InlineButton('1',
+'inline_keyboard:1'), InlineButton('2', 'inline_keyboard:2'), InlineButton('3',
+'inline_keyboard:3'), InlineButton('4', 'inline_keyboard:4'), InlineButton('5',
+'inline_keyboard:5'), InlineButton('6', 'inline_keyboard:6'), InlineButton('7',
+'inline_keyboard:7') ) ``` #### Result
 [add_inline_button]
 ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install Abg ```
 **** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ :-> ****
 [https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
 903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ :-> ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
```

### Comparing `Abg-1.2/setup.py` & `Abg-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="1.2",
+    version="1.3",
     description="pyrogram helpers / add-on for pyrogram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi1M",
     author_email="Abishnoi69@Abg.org",
```

