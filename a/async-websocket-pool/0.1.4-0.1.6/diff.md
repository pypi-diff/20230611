# Comparing `tmp/async_websocket_pool-0.1.4.tar.gz` & `tmp/async_websocket_pool-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_websocket_pool-0.1.4.tar", max compression
+gzip compressed data, was "async_websocket_pool-0.1.6.tar", max compression
```

## Comparing `async_websocket_pool-0.1.4.tar` & `async_websocket_pool-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-05-23 21:56:44.111982 async_websocket_pool-0.1.4/LICENSE
--rw-r--r--   0        0        0     1549 2023-05-23 21:56:44.111982 async_websocket_pool-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-23 21:56:44.111982 async_websocket_pool-0.1.4/async_websocket_pool/__init__.py
--rw-r--r--   0        0        0     4516 2023-05-23 21:56:44.111982 async_websocket_pool-0.1.4/async_websocket_pool/websocket.py
--rw-r--r--   0        0        0      573 2023-05-23 21:56:44.111982 async_websocket_pool-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 async_websocket_pool-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-11 17:04:35.428789 async_websocket_pool-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1549 2023-06-11 17:04:35.428789 async_websocket_pool-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 17:04:35.428789 async_websocket_pool-0.1.6/async_websocket_pool/__init__.py
+-rw-r--r--   0        0        0     4483 2023-06-11 17:04:35.428789 async_websocket_pool-0.1.6/async_websocket_pool/websocket.py
+-rw-r--r--   0        0        0      573 2023-06-11 17:04:35.428789 async_websocket_pool-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 async_websocket_pool-0.1.6/PKG-INFO
```

### Comparing `async_websocket_pool-0.1.4/LICENSE` & `async_websocket_pool-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `async_websocket_pool-0.1.4/README.md` & `async_websocket_pool-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `async_websocket_pool-0.1.4/async_websocket_pool/websocket.py` & `async_websocket_pool-0.1.6/async_websocket_pool/websocket.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import asyncio
 import logging
-import sys
 from asyncio import Semaphore, Future
 from typing import Any, Optional, Callable, List
 
 import websockets
 from websockets import WebSocketClientProtocol
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
-logger.addHandler(logging.StreamHandler(sys.stdout))
-
 
 async def connect(
         url: str,
         on_message: Callable[[Any], None],
         on_connect: Optional[Callable[[WebSocketClientProtocol], None]],
         timeout: Optional[int | float] = None,
         max_concurrent_tasks: int = 10,
@@ -38,45 +33,47 @@
 
     :param url: The WebSocket URL to establish the connection.
     :param on_message: A callback function to handle incoming messages. This function should
                             accept a single argument which will be the received message.
     :param on_connect: A callback function that is executed every time successful connection is established.
     :param timeout: Optional; The maximum wait time for a message, in seconds. If set to None,
                     the function will wait indefinitely for a message.
+    :param max_concurrent_tasks: Optional; The maximum number of concurrent tasks to execute.
     :param kwargs: Optional; Additional keyword arguments for the websockets.connect function to
                    further customize the WebSocket connection.
     :return: None
 
     :raises: This function propagates all exceptions except for asyncio.TimeoutError and
              websockets.ConnectionClosed, which are handled internally.
     """
+
     async def handle_message(msg: Any):
         async with semaphore:
             await on_message(msg)
 
     semaphore: Semaphore = Semaphore(max_concurrent_tasks)
 
     async for websocket in websockets.connect(url, **kwargs):
         try:
-            logger.info(f'Connected to {url}')
+            logging.info(f'Connected to {url}')
 
             if on_connect:
                 await on_connect(websocket)
 
             while True:
                 try:
                     message: Any = await asyncio.wait_for(websocket.recv(), timeout=timeout)
                     asyncio.create_task(handle_message(message))
                 except asyncio.TimeoutError:
-                    logger.warning(f'Timeout detected for {url}')
+                    logging.warning(f'Timeout detected for {url}')
                     break
         except websockets.ConnectionClosed:
-            logger.warning(f'Disconnected from {url}')
+            logging.warning(f'Disconnected from {url}')
         except Exception as e:
-            logger.exception(e)
+            logging.exception(e)
 
 
 async def run_pool(funcs: List[Callable]) -> Future:
     """
     Concurrently executes a list of asynchronous functions utilizing the asyncio.gather method.
 
     This function serves as a utility for managing concurrent execution of tasks, effectively
```

### Comparing `async_websocket_pool-0.1.4/pyproject.toml` & `async_websocket_pool-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-websocket-pool"
-version = "0.1.4"
+version = "0.1.6"
 description = "async-websocket-pool is a Python library that enables efficient creation and management of a pool of asynchronous WebSocket clients."
 authors = ["mpol1t"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "async_websocket_pool"}]
 
 [tool.poetry.dependencies]
```

### Comparing `async_websocket_pool-0.1.4/PKG-INFO` & `async_websocket_pool-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-websocket-pool
-Version: 0.1.4
+Version: 0.1.6
 Summary: async-websocket-pool is a Python library that enables efficient creation and management of a pool of asynchronous WebSocket clients.
 License: MIT
 Author: mpol1t
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

