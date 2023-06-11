# Comparing `tmp/bantam-2.2.4.tar.gz` & `tmp/bantam-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.2.4.tar", last modified: Sat Jun 10 23:18:30 2023, max compression
+gzip compressed data, was "bantam-2.3.4.tar", last modified: Sun Jun 11 03:32:32 2023, max compression
```

## Comparing `bantam-2.2.4.tar` & `bantam-2.3.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.892676 bantam-2.2.4/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-10 23:18:30.892676 bantam-2.2.4/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.4/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.4/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-10 23:18:30.892676 bantam-2.2.4/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-10 23:18:04.000000 bantam-2.2.4/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.888676 bantam-2.2.4/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.888676 bantam-2.2.4/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.4/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    10548 2023-06-10 22:52:38.000000 bantam-2.2.4/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.892676 bantam-2.2.4/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.4/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.4/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20981 2023-06-10 22:33:04.000000 bantam-2.2.4/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.4/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.2.4/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    46266 2023-06-10 23:09:54.000000 bantam-2.2.4/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.4/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.4/src/bantam/js_async.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.4/src/bantam/pythonclient.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.888676 bantam-2.2.4/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.892676 bantam-2.2.4/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4785 2023-06-10 04:24:24.000000 bantam-2.2.4/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4634 2023-06-10 04:24:36.000000 bantam-2.2.4/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6009 2023-06-10 23:07:07.000000 bantam-2.2.4/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.4/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.4/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.4/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3254 2023-06-10 16:56:43.000000 bantam-2.2.4/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.2.4/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-11 03:32:32.431252 bantam-2.3.4/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.3.4/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       55 2023-06-11 01:27:30.000000 bantam-2.3.4/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-11 03:32:32.431252 bantam-2.3.4/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-11 03:23:54.000000 bantam-2.3.4/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4613 2023-06-11 03:31:41.000000 bantam-2.3.4/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10548 2023-06-10 22:52:38.000000 bantam-2.3.4/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.3.4/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.3.4/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20981 2023-06-10 22:33:04.000000 bantam-2.3.4/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.3.4/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.3.4/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    49446 2023-06-11 03:23:34.000000 bantam-2.3.4/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.3.4/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.3.4/src/bantam/js_async.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.3.4/src/bantam/pythonclient.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       55 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-11 03:32:32.000000 bantam-2.3.4/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-11 03:32:32.431252 bantam-2.3.4/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4785 2023-06-10 04:24:24.000000 bantam-2.3.4/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4634 2023-06-10 04:24:36.000000 bantam-2.3.4/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.3.4/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.3.4/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.3.4/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.3.4/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.3.4/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.3.4/test/test_js_async.py
```

### Comparing `bantam-2.2.4/PKG-INFO` & `bantam-2.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.4
+Version: 2.3.4
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.4
+Download-URL: https://github.com/bantam/dist/2.3.4
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.4/setup.py` & `bantam-2.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.2.4"
+VERSION = "2.3.4"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.2.4/src/bantam/__init__.py` & `bantam-2.3.4/src/bantam/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 to display various salutiations.
 
 To explain this code, the *@web_api* decorator declares a method that is mapped to a route. The route is determined
 by the class name, in this case *Greetings*, and the method name. Thus, the "welcome" method above, as a member of
 *Greetings* class, is mapped to the route '/Greetings/welcome".  There are some rules about methods declared as
 *@web_api*:
 
-#. They can be @staticmethods, @classmethods or even instance methods (explained below), but @classmethod or
+#. They can be @classmethods or even instance methods (explained below), but @classmethod or
    instance methods are prefered
 #. They must provide all type hints for parameters and return value.  The types must
    be of only specific kinds as explained below
 #. Be judicious on GET vs POST, particuraly being mindfl of the amount of data to be passed in parameters as
    wll as returned.  Large data transfers should use POST
 
 The query parameters provided in the full URL are mapped to the parameters in the Python method.  For example,
@@ -78,14 +78,23 @@
 payload of the request (not query parameters) as a simple JSON dictionary.
 
 .. caution::
 
     Although the code prevents name collisions, the underlying (automated) routes do not, and a route must be unique.
     Thus, each pair of class/method declared as a @web_api must be unique, even across differing modules.
 
+.. caution::
+
+    Batnam invokes all requests in a single thread within the server (and undoes any per-thread model of
+    the underlying http/web package used to conduct the HTTP transactions).  The user needs to be keenly
+    aware of the rules of asyncio. Specifically: (1) do not invoke blocking calls (await calls that yield processing
+    back but take a long time to complete are OK, of course) and (2) understand that if stateful, the state
+    of the server objects can change in the middle of execution if an await is invoked and processing is
+    yielded to another async request from another client call.
+
 """
 
 
 class HTTPException(Exception):
 
     def __init__(self, code: int, msg: str):
         super().__init__(msg)
```

### Comparing `bantam-2.2.4/src/bantam/api.py` & `bantam-2.3.4/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/src/bantam/autogen/main.py` & `bantam-2.3.4/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/src/bantam/client.py` & `bantam-2.3.4/src/bantam/client.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/src/bantam/conversions.py` & `bantam-2.3.4/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/src/bantam/decorators.py` & `bantam-2.3.4/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/src/bantam/http.py` & `bantam-2.3.4/src/bantam/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     List,
     Mapping,
     Optional,
     Union,
     Type,
 )
 
+from asynciomultiplexer import asynciomultiplexer
+
 from . import HTTPException
 from .conversions import from_str, to_str, normalize_from_json
 from .decorators import (
     PreProcessor,
     PostProcessor,
     web_api,
     WebApi,
@@ -79,14 +81,44 @@
     """
     _context: Dict[Awaitable, Request] = {}
     _class_instance_methods: Dict[Type, List[API]] = {}
     _instance_methods_class_map: Dict[API, Type] = {}
     _instance_methods: List[API] = []
     _all_methods: List[API] = []
 
+    class MainThread:
+        """
+        This is used to "undo" the threading in aiohttp.  It seems silly to combine threading and asyncio
+        by handling each request in its own response.  It is somewhat understandable to attempt to
+        de-conflict state perhaps(?), but overall is just silly IMHO.  This thread puts all invocations
+        of routes into one thread handle a main asyncio loop.  User needs to beware of stateful-ness in that
+        one asyncio task can change the state while another is in the middle of being awaited (but threading
+        really doesn't solve this anyway).
+        """
+        MAX_SIMULTANEOUS_REQUESTS = 1000
+
+        request_q = asynciomultiplexer.AsyncAdaptorQueue(MAX_SIMULTANEOUS_REQUESTS)
+
+        @classmethod
+        async def start(cls, coro: Awaitable, resp_q: asynciomultiplexer.AsyncAdaptorQueue):
+            await cls.request_q.put((coro, resp_q))
+
+        @classmethod
+        async def main(cls):
+            async def task(coro: Awaitable, resp_q: asynciomultiplexer.AsyncAdaptorQueue):
+                try:
+                    resp = await coro
+                except Exception as e:
+                    resp = e
+                await resp_q.put(resp)
+
+            while True:
+                request = await cls.request_q.get(polling_interval=0.01)
+                asyncio.create_task(task(*request))
+
     class ObjectRepo:
         DEFAULT_OBJECT_EXPIRATION: int = 60*60*2   # in seconds = 1 hour
 
         instances: Dict[str, Any] = {}
         by_instance: Dict[Any, str] = {}
         expiry: Dict[str, Task] = {}
 
@@ -117,14 +149,15 @@
                  *,
                  static_path: Optional[PathLike] = None,
                  js_bundle_name: Optional[str] = None,
                  handler_args: Optional[Mapping[str, Any]] = None,
                  client_max_size: int = MAX_CLIENTS,
                  using_async: bool = True,
                  debug: Any = ..., ) -> None:  # mypy doesn't support ellipsis
+        self._main_task: Optional[asyncio.Task] = None
         if static_path is not None and not Path(static_path).exists():
             raise ValueError(f"Provided static path, {static_path} does not exist")
         self._static_path = static_path
         self._js_bundle_name = js_bundle_name
         self._using_async = using_async
         self._web_app = Application(handler_args=handler_args,
                                     client_max_size=client_max_size, debug=debug)
@@ -339,14 +372,15 @@
         :param reuse_address: tells the kernel to reuse a local socket in TIME_WAIT state, without waiting for its
            natural timeout to expire. If not specified will automatically be set to True on UNIX.
         :param reuse_port: tells the kernel to allow this endpoint to be bound to the same port as other existing
             endpoints are bound to, so long as they all set this flag when being created. This option is not supported
             on Windows.
         """
         # noinspection PyProtectedMember
+        self._main_task = asyncio.create_task(self.MainThread.main())
         from aiohttp.web import _run_app as web_run_app
         for module in modules:
             self.preprocess_module(module)
             if module not in sys.modules:
                 mod = importlib.import_module(module)
             else:
                 mod = sys.modules.get(module)
@@ -397,15 +431,18 @@
                           ssl_context=ssl_context, backlog=backlog, handle_signals=handle_signals,
                           reuse_address=reuse_address, reuse_port=reuse_port)
 
     async def shutdown(self) -> None:
         """
         Shutdown this server
         """
+        if self._main_task is not None:
+            self._main_task.cancel()
         if self._started:
+
             await self._web_app.shutdown()
             self._started = False
 
     # noinspection PyProtectedMember
     @classmethod
     def get_context(cls):
         i = 1
@@ -571,47 +608,63 @@
         name = api.qualname.replace('__init__', 'create').replace('._expire', '.expire')
         name_parts = name.split('.')[-2:]
         route = '/' + '/'.join(name_parts)
         if '__isabstractmethod__' in func.__dict__:
             return func
 
         async def invoke(app: WebApplication, request: Request):
-            nonlocal preprocess, postprocess
-            try:
-                preprocess = preprocess or app.preprocessor
-                try:
-                    addl_args = (preprocess(request) or {}) if preprocess else {}
-                except Exception as e:
-                    text = traceback.format_exc()
-                    return Response(status=400, text=f"Error in preprocessing request: {e}\n{text}")
-                if method == RestMethod.GET:
-                    # noinspection PyProtectedMember
-                    response = await cls._invoke_get_api_wrapper(
-                        api, content_type=content_type, request=request, **addl_args
-                    )
-                elif method == RestMethod.POST:
-                    # noinspection PyProtectedMember
-                    response = await cls._invoke_post_api_wrapper(
-                        api, content_type=content_type, request=request, **addl_args
-                    )
-                else:
-                    raise ValueError(f"Unknown method {method} in @web-api")
+
+            async def invoke_proper():
+                nonlocal preprocess, postprocess
+                print(f">>>>>>>>>>>>>> INVOKING {api.name}")
                 try:
-                    postprocess = postprocess or app.postprocessor
-                    postprocess(response) if postprocess else response
-                except Exception as e:
+                    preprocess = preprocess or app.preprocessor
+                    try:
+                        addl_args = (preprocess(request) or {}) if preprocess else {}
+                    except Exception as e:
+                        text = traceback.format_exc()
+                        resp = Response(status=400, text=f"Error in preprocessing request: {e}\n{text}")
+                        await resp.prepare(request)
+                        return resp
+                    if method == RestMethod.GET:
+                        # noinspection PyProtectedMember
+                        response = await cls._invoke_get_api_wrapper(
+                            api, content_type=content_type, request=request, **addl_args
+                        )
+                    elif method == RestMethod.POST:
+                        # noinspection PyProtectedMember
+                        response = await cls._invoke_post_api_wrapper(
+                            api, content_type=content_type, request=request, **addl_args
+                        )
+                    else:
+                        raise ValueError(f"Unknown method {method} in @web-api")
+                    try:
+                        postprocess = postprocess or app.postprocessor
+                        postprocess(response) if postprocess else response
+                    except Exception as e:
+                        text = traceback.format_exc()
+                        resp = Response(status=400, text=f"Error in post-processing of response: {e}\n{text}")
+                        await resp.prepare(request)
+                        return resp
+                    return response
+                except (CancelledError, ConnectionResetError, ClientConnectionError):
+                    raise
+                except BaseException as e:
                     text = traceback.format_exc()
-                    return Response(status=400, text=f"Error in post-processing of response: {e}\n{text}")
-                return response
-            except (CancelledError, ConnectionResetError, ClientConnectionError):
+                    resp = Response(status=500, reason=f"Server error: {e}",
+                                    body=f"Server error: {e}\n{text}", content_type="test/plain")
+                    await resp.prepare(request)
+                    return resp
+            resp_q = asynciomultiplexer.AsyncAdaptorQueue(1)
+            await cls.MainThread.start(invoke_proper(), resp_q)
+            resp = await resp_q.get()
+            print(f">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> {api.name} RESP WRITE DONE {resp}")
+            if isinstance(resp, Exception):
                 raise
-            except BaseException as e:
-                text = traceback.format_exc()
-                return Response(status=500, reason=f"Server error: {e}",
-                                body=f"Server error: {e}\n{text}", content_type="test/plain")
+            return resp
 
         invoke.clazz = WebApplication._instance_methods_class_map.get(api) if is_instance_method else None
         if method == RestMethod.GET:
             # noinspection PyProtectedMember
             WebApplication.register_route_get(route, invoke, api, api._real_func.__module__)
         elif method == RestMethod.POST:
             # noinspection PyProtectedMember
@@ -640,18 +693,20 @@
             items = content_type.split(';')
             for item in items:
                 item = item.lower()
                 if item.startswith('charset='):
                     encoding = item.replace('charset=', '')
             # report first param that doesn't match the Python signature:
             for k in [p for p in request.query if p not in api.arg_annotations and p != 'self']:
-                return Response(
+                resp = Response(
                     status=400,
                     text=f"No such parameter or missing type hint for param {k} in method {api.qualname}"
                 )
+                await resp.prepare(request)
+                return resp
 
             # convert incoming str values to proper type:
             kwargs = {k: _convert_request_param(v, api.arg_annotations[k]) if k != 'self' else v
                       for k, v in request.query.items()}
             if addl_args:
                 kwargs.update(addl_args)
             if api.is_instance_method:
@@ -728,24 +783,28 @@
                         result = json.dumps({'uuid': uuid})
                     cls.ObjectRepo.instances[uuid] = instance
                     cls.ObjectRepo.by_instance[instance] = uuid
                     cls.ObjectRepo.expiry[uuid] = asyncio.create_task(cls.ObjectRepo.expire_obj(
                         uuid, cls.ObjectRepo.DEFAULT_OBJECT_EXPIRATION))
                 else:
                     result = _serialize_return_value(result, encoding)
-                return Response(status=200, body=result if result is not None else b"Success",
+                resp = Response(status=200, body=result if result is not None else b"Success",
                                 content_type=content_type)
+                await resp.prepare(request)
+                return resp
         except TypeError as e:
-            return Response(status=400, text=f"Improperly formatted query: {str(e)}\n{traceback.format_exc()}")
+            resp = Response(status=400, text=f"Improperly formatted query: {str(e)}\n{traceback.format_exc()}")
+            await resp.prepare(request)
+            return resp
         except HTTPException as e:
-            return Response(status=e.status_code, text=f"{e}: \n{traceback.format_exc()}")
-        except (asyncio.CancelledError, asyncio.TimeoutError):
             raise
         except Exception as e:
-            return Response(status=500, text=f"Exception: {e}: \n{traceback.format_exc()}")
+            resp = Response(status=500, text=f"Exception: {e}: \n{traceback.format_exc()}")
+            await resp.prepare(request)
+            return resp
         finally:
             # noinspection PyUnresolvedReferences,PyProtectedMember
             del cls._context[sys._getframe(0)]
 
     @classmethod
     async def _invoke_post_api_wrapper(cls, api: API, content_type: str, request: Request,
                                        **addl_args: Any) -> Union[Response, StreamResponse]:
@@ -753,14 +812,15 @@
         Invoke the underlying POST web API from given request. Called as part of setup in cls._func_wrapper
 
         :param api:  API wrapping async function to be called
         :param content_type: http header content-type
         :param request: request to be processed
         :return: http response object
         """
+
         async def line_by_line_response(req: Request):
             reader = req.content
             chunk = True
             while not reader.is_eof() and chunk:
                 chunk = await reader.readline()
                 yield chunk
             last = await reader.readline()
@@ -801,18 +861,20 @@
                 kwargs.update({k: _convert_request_param(v, api.synchronous_arg_annotations[k]) if k != 'self' else v
                                for k, v in request.query.items() if k in api.synchronous_arg_annotations})
             else:
                 # treat payload as json string:
                 bytes_response = await request.read()
                 json_dict = json.loads(bytes_response.decode('utf-8'))
                 for k in [p for p in json_dict if p not in api.arg_annotations and p != 'self']:
-                    return Response(
+                    resp = Response(
                         status=400,
                         text=f"No such parameter or missing type hint for param {k} in method {api.qualname}"
                     )
+                    await resp.prepare(request)
+                    return resp
 
                 # convert incoming str values to proper type:
                 kwargs.update(dict(json_dict))
             # call the underlying function:
             if addl_args:
                 kwargs.update(addl_args)
             for k, v in kwargs.items():
@@ -877,16 +939,20 @@
                             raise
 
                 except (CancelledError, ConnectionResetError, ClientConnectionError):
                     raise
                 except Exception as e:
                     print(str(e))
                     await async_q.put(None)
-                    raise RuntimeError(f"Exception in server-side logic: {e}") from e
+                    resp = Response(status=500, body=f"Exception in server-side logic: {e}",
+                                    content_type='text/plain')
+                    await resp.prepare(request)
+                    return resp
                 await response.write_eof()
+                return response
             else:
                 #################
                 #  regular response
                 #################
                 if api.is_constructor:
                     instance = await awaitable
                     if api.clazz and hasattr(api.clazz, '__aenter__'):
@@ -899,30 +965,40 @@
                     else:
                         uuid = kwargs.get(api.uuid_param, str(uuid_pkg.uuid4()))
                         result = json.dumps({'uuid': uuid})
                     cls.ObjectRepo.instances[uuid] = instance
                     cls.ObjectRepo.by_instance[instance] = uuid
                     cls.ObjectRepo.expiry[uuid] = asyncio.create_task(cls.ObjectRepo.expire_obj(
                         uuid, cls.ObjectRepo.DEFAULT_OBJECT_EXPIRATION))
-                    return Response(status=200, body=result if result is not None else b"Success",
+                    resp = Response(status=200, body=result if result is not None else b"Success",
                                     content_type=content_type)
+                    await resp.prepare(request)
+                    return resp
                 else:
                     result = _serialize_return_value(await awaitable, encoding)
-                return Response(status=200, body=result if result is not None else b"Success",
+                resp = Response(status=200, body=result if result is not None else b"Success",
                                 content_type=content_type)
+                await resp.prepare(request)
+                return resp
 
         except TypeError as e:
-            return Response(status=400, text=f"Improperly formatted query: {str(e)}")
+            resp = Response(status=400, text=f"Improperly formatted query: {str(e)}")
+            await resp.prepare(request)
+            return resp
         except HTTPException as e:
-            return Response(status=e.status_code, text=str(e))
+            resp = Response(status=e.status_code, text=str(e))
+            await resp.prepare(request)
+            return resp
         except (CancelledError, ConnectionResetError, ClientConnectionError):
             raise
         except Exception as e:
             text = f"Exception: {e}\n {traceback.format_exc()}"
-            return Response(status=500, text=text)
+            resp = Response(status=500, text=text)
+            await resp.prepare(request)
+            return resp
         finally:
             # noinspection PyUnresolvedReferences,PyProtectedMember
             del cls._context[sys._getframe(0)]
 
 
 def _convert_request_param(value: str, typ: Type) -> Any:
     """
```

### Comparing `bantam-2.2.4/src/bantam/js.py` & `bantam-2.3.4/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/src/bantam/js_async.py` & `bantam-2.3.4/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/src/bantam/pythonclient.py` & `bantam-2.3.4/src/bantam/pythonclient.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/src/bantam.egg-info/PKG-INFO` & `bantam-2.3.4/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.4
+Version: 2.3.4
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.4
+Download-URL: https://github.com/bantam/dist/2.3.4
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.4/src/bantam.egg-info/SOURCES.txt` & `bantam-2.3.4/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/test/test_client_get.py` & `bantam-2.3.4/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/test/test_client_post.py` & `bantam-2.3.4/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/test/test_client_post_inherited_apis.py` & `bantam-2.3.4/test/test_client_post_inherited_apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,10 +135,11 @@
             assert item == str(29)*65537
             count += 1
             if count == 121:
                 break  # disconnects client
         await asyncio.sleep(1)  # give server time to process disconnect
         assert RestAPIExampleAsyncPostInheritedInterface.disconnected
     finally:
+        await app.shutdown()
         task.cancel()
         with suppress(CancelledError):
             await task
```

### Comparing `bantam-2.2.4/test/test_conversions.py` & `bantam-2.3.4/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/test/test_decorators.py` & `bantam-2.3.4/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.4/test/test_js.py` & `bantam-2.3.4/test/test_js.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,44 +5,40 @@
 import webbrowser
 from contextlib import suppress
 from pathlib import Path
 from typing import AsyncGenerator, Optional, Dict, Any
 
 import pytest
 from aiohttp.web_request import Request
-from aiohttp.web_response import Response
+from aiohttp.web_response import Response, StreamResponse
 
-from bantam.decorators import web_api
-from bantam.api import AsyncLineIterator, RestMethod
 from bantam.http import WebApplication
 
 
-
 class TestJavascriptGenerator:
 
     @pytest.mark.asyncio
     async def test_generate_basic(self):
         def assert_preprocessor(request: Request) -> Dict[str, Any]:
             assert isinstance(request, Request), "Failed to get valid response on pre-processing"
             return {}
 
         def assert_postprocessor(response: Response) -> None:
-            assert isinstance(response, Response), "Failed to get valid response for post-processing"
+            assert isinstance(response, (Response, StreamResponse)), "Failed to get valid response for post-processing"
 
         from class_js_test import RestAPIExample
         RestAPIExample.result_queue = asyncio.Queue()
         root = Path(__file__).parent
         static_path = root.joinpath('static')
         app = WebApplication(static_path=static_path, js_bundle_name='generated', using_async=False)
         app.set_preprocessor(assert_preprocessor)
         app.set_postprocessor(assert_postprocessor)
 
         async def launch_browser():
             await asyncio.sleep(2.0)
-            browser = None
             default = False
             try:
                 browser = webbrowser.get("chrome")
             except:
                 with suppress(Exception):
                     browser = webbrowser.get("google-chrome")
                 if not browser:
@@ -53,28 +49,27 @@
                 with suppress(Exception):
                     browser = webbrowser.get("firefox")
                     flags = ["-new-instance"]
             if not browser:
                 os.write(sys.stderr.fileno(),
                          b"UNABLE TO GET BROWSER SUPPORT HEADLESS CONFIGURATION. DEFAULTING TO NON_HEADLESSS")
                 browser = webbrowser.get()
-            # cmdline = [browser.name] + flags + \
             browser.open("http://localhost:8080/static/index.html")
-            # process = subprocess.Popen(cmdline)
-            result = await RestAPIExample.result_queue.get()
-            if result != 'PASSED':
-                await asyncio.sleep(2.0)
-            await app.shutdown()
-            return result
 
+        app_task = asyncio.create_task(app.start(modules=['class_js_test']))
+        browser_task = asyncio.create_task(launch_browser())
         try:
-            completed, _ = await asyncio.wait([app.start(modules=['class_js_test']), launch_browser()],
-                                              timeout=100, return_when=asyncio.FIRST_COMPLETED)
-            results = [c.result() for c in completed if c is not None]
+            result = await asyncio.wait_for(RestAPIExample.result_queue.get(), timeout=120)
+            if result != 'PASSED':
+                await asyncio.sleep(2.0)
         except Exception as e:
+            await asyncio.sleep(2.0)
             assert False, f"Exception processing javascript results: {e}"
+        finally:
+            await app.shutdown()
+            browser_task.cancel()
 
-        if any([isinstance(r, Exception) for r in results]):
+        if isinstance(result, Exception):
             assert False, "At least one javascript test failed. See browser window for details"
-        assert results[0] == "PASSED", \
+        assert result == "PASSED", \
             "FAILED JAVASCRIPT TESTS FOUND: \n" + \
-            "\n".join([f"{test}: {msg}" for test, msg in json.loads(results[0]).items()])
+            "\n".join([f"{test}: {msg}" for test, msg in json.loads(result).items()])
```

### Comparing `bantam-2.2.4/test/test_js_async.py` & `bantam-2.3.4/test/test_js_async.py`

 * *Files identical despite different names*

