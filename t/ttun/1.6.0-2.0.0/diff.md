# Comparing `tmp/ttun-1.6.0.tar.gz` & `tmp/ttun-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttun-1.6.0.tar", last modified: Mon Dec 19 13:33:16 2022, max compression
+gzip compressed data, was "ttun-2.0.0.tar", last modified: Sun Jun 11 11:35:05 2023, max compression
```

## Comparing `ttun-1.6.0.tar` & `ttun-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:33:16.984442 ttun-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2022-12-19 13:32:45.000000 ttun-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-19 13:32:45.000000 ttun-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-19 13:33:16.984442 ttun-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-19 13:32:45.000000 ttun-1.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-19 13:32:45.000000 ttun-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2022-12-19 13:33:16.984442 ttun-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:33:16.980442 ttun-1.6.0/ttun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 13:32:45.000000 ttun-1.6.0/ttun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2022-12-19 13:32:45.000000 ttun-1.6.0/ttun/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2022-12-19 13:32:45.000000 ttun-1.6.0/ttun/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2022-12-19 13:32:45.000000 ttun-1.6.0/ttun/inspect_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-19 13:32:45.000000 ttun-1.6.0/ttun/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2022-12-19 13:32:45.000000 ttun-1.6.0/ttun/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:33:16.984442 ttun-1.6.0/ttun/staticfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:33:16.984442 ttun-1.6.0/ttun/staticfiles/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   352540 2022-12-19 13:33:09.000000 ttun-1.6.0/ttun/staticfiles/assets/index.120f66e1.js
--rw-r--r--   0 runner    (1001) docker     (123)   324123 2022-12-19 13:33:09.000000 ttun-1.6.0/ttun/staticfiles/assets/index.cc7cded7.css
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-19 13:33:09.000000 ttun-1.6.0/ttun/staticfiles/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      368 2022-12-19 13:32:45.000000 ttun-1.6.0/ttun/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 13:33:16.984442 ttun-1.6.0/ttun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-19 13:33:16.000000 ttun-1.6.0/ttun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2022-12-19 13:33:16.000000 ttun-1.6.0/ttun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 13:33:16.000000 ttun-1.6.0/ttun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-19 13:33:16.000000 ttun-1.6.0/ttun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-19 13:33:16.000000 ttun-1.6.0/ttun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-19 13:33:16.000000 ttun-1.6.0/ttun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.063001 ttun-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-11 11:34:22.000000 ttun-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-11 11:34:22.000000 ttun-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-11 11:35:05.063001 ttun-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-11 11:34:22.000000 ttun-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-11 11:34:22.000000 ttun-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-11 11:35:05.063001 ttun-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.059002 ttun-2.0.0/ttun/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/inspect_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.059002 ttun-2.0.0/ttun/staticfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.063001 ttun-2.0.0/ttun/staticfiles/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   352540 2023-06-11 11:34:56.000000 ttun-2.0.0/ttun/staticfiles/assets/index.120f66e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   324123 2023-06-11 11:34:56.000000 ttun-2.0.0/ttun/staticfiles/assets/index.cc7cded7.css
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 11:34:56.000000 ttun-2.0.0/ttun/staticfiles/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-11 11:34:22.000000 ttun-2.0.0/ttun/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:35:05.059002 ttun-2.0.0/ttun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 11:35:05.000000 ttun-2.0.0/ttun.egg-info/top_level.txt
```

### Comparing `ttun-1.6.0/LICENSE` & `ttun-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ttun-1.6.0/PKG-INFO` & `ttun-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ttun
-Version: 1.6.0
-Summary: Expose a localport via your selfhosted TTUN Server
+Version: 2.0.0
+Summary: Expose a local port via your selfhosted TTUN Server
 Author: Tom van der Lee
 License: BSD-3-Clause
 License-File: LICENSE
 
 ===========
 TTUN Client
 ===========
```

### Comparing `ttun-1.6.0/README.rst` & `ttun-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `ttun-1.6.0/ttun/__main__.py` & `ttun-2.0.0/ttun/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from argparse import ArgumentParser
 from asyncio import FIRST_EXCEPTION
 from asyncio.exceptions import CancelledError
 from asyncio.exceptions import TimeoutError
 from typing import Dict
 from typing import Tuple
 
+from websockets.exceptions import ConnectionClosedError
+
 from ttun.client import Client
 from ttun.inspect_server import Server
 from ttun.settings import SERVER_HOSTNAME
 from ttun.settings import SERVER_USING_SSL
 
 inspect_queue = asyncio.Queue()
 
@@ -67,14 +69,15 @@
         subdomain=args.subdomain,
         server=args.server,
         to=args.to,
         https=args.https,
         headers=args.header,
     )
 
+
     try:
         loop = asyncio.get_running_loop()
     except RuntimeError:
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
 
     loop.run_until_complete(client.connect())
@@ -92,15 +95,16 @@
         on_started=print_info,
     )
 
     tasks = {loop.create_task(client.handle_messages()), loop.create_task(server.run())}
 
     try:
         loop.run_until_complete(asyncio.wait(tasks, return_when=FIRST_EXCEPTION))
-    except (CancelledError, TimeoutError):
+    except (CancelledError, TimeoutError) as e:
+        print(e)
         for task in tasks:
             task.cancel()
         loop.close()
     except KeyboardInterrupt:
         pass
```

### Comparing `ttun-1.6.0/ttun/client.py` & `ttun-2.0.0/ttun/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import asyncio
 import json
+import logging
+from asyncio import create_task
+from asyncio import get_running_loop
 from base64 import b64decode
 from base64 import b64encode
 from datetime import datetime
+from pprint import pformat
 from time import perf_counter
 from typing import Awaitable
 from typing import Callable
 from typing import Coroutine
 from typing import List
 from typing import Optional
 from typing import Tuple
@@ -16,45 +20,50 @@
 from aiohttp import ClientConnectionError
 from aiohttp import ClientError
 from aiohttp import ClientSession
 from aiohttp import DummyCookieJar
 from websockets import WebSocketClientProtocol
 from websockets.exceptions import ConnectionClosed
 
+from ttun import __version__
 from ttun.pubsub import PubSub
 from ttun.types import Config
+from ttun.types import Message
+from ttun.types import MessageType
 from ttun.types import RequestData
 from ttun.types import ResponseData
 
 
 class Client:
     def __init__(
         self,
         port: int,
         server: str,
         subdomain: str = None,
         to: str = "127.0.0.1",
         https: bool = False,
         headers: List[Tuple[str, str]] = None,
     ):
+        self.version = __version__
         self.server = server
         self.subdomain = subdomain
 
         self.config: Optional[Config] = None
         self.connection: WebSocketClientProtocol = None
 
         self.proxy_origin = f'{"https" if https else "http"}://{to}:{port}'
 
         self.headers = [] if headers is None else headers
 
     async def send(self, data: dict):
         await self.connection.send(json.dumps(data))
 
     async def receive(self) -> dict:
-        return json.loads(await self.connection.recv())
+        data = json.loads(await self.connection.recv())
+        return data
 
     @staticmethod
     def loop(sleep: int = None):
         async def wrapper(callback: Callable[[], Coroutine]):
             while True:
                 try:
                     await callback()
@@ -66,38 +75,61 @@
                     break
 
         return wrapper
 
     async def connect(self) -> WebSocketClientProtocol:
         self.connection = await websockets.connect(f"{self.server}/tunnel/")
 
-        await self.send({"subdomain": self.subdomain})
+        await self.send({"subdomain": self.subdomain, "version": self.version})
 
         self.config = await self.receive()
 
         if self.connection.open:
             return self.connection
 
     def session(self):
         return ClientSession(base_url=self.proxy_origin, cookie_jar=DummyCookieJar())
 
     async def handle_messages(self):
+        loop = get_running_loop()
         async with self.session() as session:
             while True:
                 try:
-                    request: RequestData = await self.receive()
+                    message: Message = await self.receive()
+
+                    try:
+                        if MessageType(message["type"]) != MessageType.request:
+                            continue
+                    except ValueError:
+                        continue
+
+                    request: RequestData = message["payload"]
 
                     request["headers"] = [
                         *request["headers"],
                         *self.headers,
                     ]
-                    await self.proxy_request(
-                        session=session,
-                        request=request,
-                        on_response=lambda response: self.send(response),
+
+                    async def response_handler(
+                        response: ResponseData, identifier=message["identifier"]
+                    ):
+                        await self.send(
+                            Message(
+                                type=MessageType.response.value,
+                                identifier=identifier,
+                                payload=response,
+                            )
+                        )
+
+                    loop.create_task(
+                        self.proxy_request(
+                            session=session,
+                            request=request,
+                            on_response=response_handler,
+                        )
                     )
                 except ConnectionClosed:
                     break
 
     async def resend(self, data: RequestData):
         async with self.session() as session:
             await self.proxy_request(session, data)
```

### Comparing `ttun-1.6.0/ttun/inspect_server.py` & `ttun-2.0.0/ttun/inspect_server.py`

 * *Files identical despite different names*

### Comparing `ttun-1.6.0/ttun/pubsub.py` & `ttun-2.0.0/ttun/pubsub.py`

 * *Files identical despite different names*

### Comparing `ttun-1.6.0/ttun/settings.py` & `ttun-2.0.0/ttun/settings.py`

 * *Files identical despite different names*

### Comparing `ttun-1.6.0/ttun/staticfiles/assets/index.120f66e1.js` & `ttun-2.0.0/ttun/staticfiles/assets/index.120f66e1.js`

 * *Files identical despite different names*

### Comparing `ttun-1.6.0/ttun/staticfiles/assets/index.cc7cded7.css` & `ttun-2.0.0/ttun/staticfiles/assets/index.cc7cded7.css`

 * *Files identical despite different names*

### Comparing `ttun-1.6.0/ttun.egg-info/PKG-INFO` & `ttun-2.0.0/ttun.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ttun
-Version: 1.6.0
-Summary: Expose a localport via your selfhosted TTUN Server
+Version: 2.0.0
+Summary: Expose a local port via your selfhosted TTUN Server
 Author: Tom van der Lee
 License: BSD-3-Clause
 License-File: LICENSE
 
 ===========
 TTUN Client
 ===========
```

