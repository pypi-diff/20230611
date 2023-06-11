# Comparing `tmp/aiocqhttp-1.4.3.tar.gz` & `tmp/aiocqhttp-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocqhttp-1.4.3.tar", last modified: Thu Apr 28 03:39:40 2022, max compression
+gzip compressed data, was "aiocqhttp-1.4.4.tar", last modified: Sun Jun 11 05:20:07 2023, max compression
```

## Comparing `aiocqhttp-1.4.3.tar` & `aiocqhttp-1.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 03:39:40.895188 aiocqhttp-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-04-28 03:39:40.895188 aiocqhttp-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 03:39:40.895188 aiocqhttp-1.4.3/aiocqhttp/
--rw-r--r--   0 runner    (1001) docker     (121)    21889 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    34175 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/api.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7013 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/api_impl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/default.py
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    19063 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/message.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/aiocqhttp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 03:39:40.895188 aiocqhttp-1.4.3/aiocqhttp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-04-28 03:39:40.000000 aiocqhttp-1.4.3/aiocqhttp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-04-28 03:39:40.000000 aiocqhttp-1.4.3/aiocqhttp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 03:39:40.000000 aiocqhttp-1.4.3/aiocqhttp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-28 03:39:40.000000 aiocqhttp-1.4.3/aiocqhttp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-28 03:39:40.000000 aiocqhttp-1.4.3/aiocqhttp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-28 03:39:40.895188 aiocqhttp-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-04-28 03:39:33.000000 aiocqhttp-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:20:07.941564 aiocqhttp-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-11 05:20:07.941564 aiocqhttp-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:20:07.937564 aiocqhttp-1.4.4/aiocqhttp/
+-rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34175 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/api_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/aiocqhttp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 05:20:07.941564 aiocqhttp-1.4.4/aiocqhttp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-11 05:20:07.000000 aiocqhttp-1.4.4/aiocqhttp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-11 05:20:07.000000 aiocqhttp-1.4.4/aiocqhttp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 05:20:07.000000 aiocqhttp-1.4.4/aiocqhttp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-11 05:20:07.000000 aiocqhttp-1.4.4/aiocqhttp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 05:20:07.000000 aiocqhttp-1.4.4/aiocqhttp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 05:20:07.941564 aiocqhttp-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-11 05:19:51.000000 aiocqhttp-1.4.4/setup.py
```

### Comparing `aiocqhttp-1.4.3/LICENSE` & `aiocqhttp-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/PKG-INFO` & `aiocqhttp-1.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocqhttp
-Version: 1.4.3
+Version: 1.4.4
 Summary: A Python SDK with async I/O for OneBot (CQHTTP).
 Home-page: https://github.com/nonebot/aiocqhttp
 Author: Richard Chien
 Author-email: richardchienthebest@gmail.com
 Maintainer: NoneBot Team
 License: MIT License
 Description: # aiocqhttp
```

### Comparing `aiocqhttp-1.4.3/README.md` & `aiocqhttp-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp/__init__.py` & `aiocqhttp-1.4.4/aiocqhttp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,16 +222,14 @@
         self._server_app.run(host=host, port=port, *args, **kwargs)
 
     def run_task(self,
                  host: str = '127.0.0.1',
                  port: int = 8080,
                  *args,
                  **kwargs) -> Coroutine[None, None, None]:
-        if 'use_reloader' not in kwargs:
-            kwargs['use_reloader'] = False
         return self._server_app.run_task(host=host, port=port, *args, **kwargs)
 
     async def call_action(self, action: str, **params) -> Any:
         """
         通过内部维护的 `api.AsyncApi` 具体实现类调用 OneBot API，``action``
         为要调用的 API 动作名，``**params`` 为 API 所需参数。
         """
```

### Comparing `aiocqhttp-1.4.3/aiocqhttp/api.py` & `aiocqhttp-1.4.4/aiocqhttp/api.py`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp/api.pyi` & `aiocqhttp-1.4.4/aiocqhttp/api.pyi`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp/api_impl.py` & `aiocqhttp-1.4.4/aiocqhttp/api_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             raise ApiNotAvailable
 
         headers = {}
         if self._access_token:
             headers['Authorization'] = 'Bearer ' + self._access_token
 
         try:
-            async with httpx.AsyncClient() as client:
+            async with httpx.AsyncClient(timeout=self._timeout_sec) as client:
                 resp = await client.post(self._api_root + action,
                                          json=params,
                                          headers=headers)
             if 200 <= resp.status_code < 300:
                 return _handle_api_result(json.loads(resp.text))
             raise HttpFailed(resp.status_code)
         except httpx.InvalidURL:
@@ -213,14 +213,14 @@
 
 
 class LazyApi(Api):
     """
     延迟获取 `aiocqhttp.api.Api` 对象。
     """
 
-    def __init__(self, api_getter: Callable[[], Union[Api]]):
+    def __init__(self, api_getter: Callable[[], Api]):
         self._api_getter = api_getter
 
     def call_action(self, action: str, **params) -> Union[Awaitable[Any], Any]:
         """获取 `Api` 对象，并调用 OneBot API。"""
         api = self._api_getter()
         return api.call_action(action, **params)
```

### Comparing `aiocqhttp-1.4.3/aiocqhttp/bus.py` & `aiocqhttp-1.4.4/aiocqhttp/bus.py`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp/default.py` & `aiocqhttp-1.4.4/aiocqhttp/default.py`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp/event.py` & `aiocqhttp-1.4.4/aiocqhttp/event.py`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp/exceptions.py` & `aiocqhttp-1.4.4/aiocqhttp/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp/message.py` & `aiocqhttp-1.4.4/aiocqhttp/message.py`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp/utils.py` & `aiocqhttp-1.4.4/aiocqhttp/utils.py`

 * *Files identical despite different names*

### Comparing `aiocqhttp-1.4.3/aiocqhttp.egg-info/PKG-INFO` & `aiocqhttp-1.4.4/aiocqhttp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocqhttp
-Version: 1.4.3
+Version: 1.4.4
 Summary: A Python SDK with async I/O for OneBot (CQHTTP).
 Home-page: https://github.com/nonebot/aiocqhttp
 Author: Richard Chien
 Author-email: richardchienthebest@gmail.com
 Maintainer: NoneBot Team
 License: MIT License
 Description: # aiocqhttp
```

### Comparing `aiocqhttp-1.4.3/setup.py` & `aiocqhttp-1.4.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='aiocqhttp',
-    version='1.4.3',
+    version='1.4.4',
     url='https://github.com/nonebot/aiocqhttp',
     license='MIT License',
     author='Richard Chien',
     author_email='richardchienthebest@gmail.com',
     maintainer='NoneBot Team',
     description='A Python SDK with async I/O for OneBot (CQHTTP).',
     long_description=long_description,
```

