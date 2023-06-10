# Comparing `tmp/bantam-2.2.3.tar.gz` & `tmp/bantam-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.2.3.tar", last modified: Sat Jun 10 17:04:08 2023, max compression
+gzip compressed data, was "bantam-2.2.4.tar", last modified: Sat Jun 10 23:18:30 2023, max compression
```

## Comparing `bantam-2.2.3.tar` & `bantam-2.2.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-10 17:04:08.646937 bantam-2.2.3/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.3/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.3/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-10 17:04:08.646937 bantam-2.2.3/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-10 17:03:19.000000 bantam-2.2.3/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.3/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    10547 2023-06-04 23:41:07.000000 bantam-2.2.3/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.3/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.3/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20981 2023-06-10 16:40:12.000000 bantam-2.2.3/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.3/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.2.3/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    45360 2023-06-10 16:04:45.000000 bantam-2.2.3/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.3/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.3/src/bantam/js_async.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.3/src/bantam/pythonclient.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4785 2023-06-10 04:24:24.000000 bantam-2.2.3/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4634 2023-06-10 04:24:36.000000 bantam-2.2.3/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4942 2023-06-10 04:23:32.000000 bantam-2.2.3/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.3/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.3/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.3/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3254 2023-06-10 16:56:43.000000 bantam-2.2.3/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.2.3/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.892676 bantam-2.2.4/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-10 23:18:30.892676 bantam-2.2.4/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.4/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.4/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-10 23:18:30.892676 bantam-2.2.4/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-10 23:18:04.000000 bantam-2.2.4/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.888676 bantam-2.2.4/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.888676 bantam-2.2.4/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.4/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10548 2023-06-10 22:52:38.000000 bantam-2.2.4/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.892676 bantam-2.2.4/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.4/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.4/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20981 2023-06-10 22:33:04.000000 bantam-2.2.4/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.4/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.2.4/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    46266 2023-06-10 23:09:54.000000 bantam-2.2.4/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.4/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.4/src/bantam/js_async.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.4/src/bantam/pythonclient.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.888676 bantam-2.2.4/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-10 23:18:30.000000 bantam-2.2.4/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 23:18:30.892676 bantam-2.2.4/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4785 2023-06-10 04:24:24.000000 bantam-2.2.4/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4634 2023-06-10 04:24:36.000000 bantam-2.2.4/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6009 2023-06-10 23:07:07.000000 bantam-2.2.4/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.4/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.4/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.4/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3254 2023-06-10 16:56:43.000000 bantam-2.2.4/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.2.4/test/test_js_async.py
```

### Comparing `bantam-2.2.3/PKG-INFO` & `bantam-2.2.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.3
+Version: 2.2.4
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.3
+Download-URL: https://github.com/bantam/dist/2.2.4
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.3/setup.py` & `bantam-2.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.2.3"
+VERSION = "2.2.4"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.2.3/src/bantam/__init__.py` & `bantam-2.2.4/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/src/bantam/api.py` & `bantam-2.2.4/src/bantam/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         return self._real_func.__doc__
 
     @property
     def method(self):
         return self._method
 
     @property
-    def on_disonnect(self):
+    def on_disconnect(self):
         return self._on_disconnect
 
     @property
     def is_instance_method(self) -> bool:
         return self._is_instance_method
 
     @property
```

### Comparing `bantam-2.2.3/src/bantam/autogen/main.py` & `bantam-2.2.4/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/src/bantam/client.py` & `bantam-2.2.4/src/bantam/client.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/src/bantam/conversions.py` & `bantam-2.2.4/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/src/bantam/decorators.py` & `bantam-2.2.4/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/src/bantam/http.py` & `bantam-2.2.4/src/bantam/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,20 +599,14 @@
                     postprocess = postprocess or app.postprocessor
                     postprocess(response) if postprocess else response
                 except Exception as e:
                     text = traceback.format_exc()
                     return Response(status=400, text=f"Error in post-processing of response: {e}\n{text}")
                 return response
             except (CancelledError, ConnectionResetError, ClientConnectionError):
-                if api.is_instance_method:
-                    self_id = request.query['self']
-                    instance = cls.ObjectRepo.instances.get(self_id)
-                    api.on_disonnect(instance)
-                else:
-                    api.on_diconnect()
                 raise
             except BaseException as e:
                 text = traceback.format_exc()
                 return Response(status=500, reason=f"Server error: {e}",
                                 body=f"Server error: {e}\n{text}", content_type="test/plain")
 
         invoke.clazz = WebApplication._instance_methods_class_map.get(api) if is_instance_method else None
@@ -691,18 +685,29 @@
                 content_type = "text-streamed; charset=x-user-defined"
                 response = StreamResponse(status=200, reason='OK', headers={'Content-Type': content_type})
                 await response.prepare(request)
                 try:
                     # iterate to get the one (and hopefully only) yielded element:
                     # noinspection PyTypeChecker
                     async for res in result:
-                        serialized = _serialize_return_value(res, encoding)
-                        if not isinstance(res, bytes):
-                            serialized += b'\0'
-                        await response.write(serialized)
+                        try:
+                            serialized = _serialize_return_value(res, encoding)
+                            if not isinstance(res, bytes):
+                                serialized += b'\0'
+                            await response.write(serialized)
+                        except (CancelledError, ConnectionResetError, ClientConnectionError):
+                            if api.on_disconnect is not None:
+                                if inspect.iscoroutinefunction(api.on_disconnect):
+                                    await api.on_disconnect(res)
+                                else:
+                                    api.on_disconnect(res)
+                            raise
+
+                except (CancelledError, ConnectionResetError, ClientConnectionError):
+                    raise
                 except Exception as e:
                     print(str(e))
                     raise asyncio.CancelledError(f"Error in server-side logic: {e}") from e
                 await response.write_eof()
                 return response
             else:
                 #################
@@ -852,19 +857,29 @@
                 response = StreamResponse(status=200, reason='OK', headers={'Content-Type': content_type})
                 await response.prepare(request)
                 try:
                     # iterate to get the one (and hopefully only) yielded element:
                     # noinspection PyTypeChecker
                     count = 0
                     async for res in awaitable:
-                        serialized = _serialize_return_value(res, encoding)
-                        if not isinstance(res, bytes):
-                            serialized += b'\0'
-                        await response.write(serialized)
-                        count += 1
+                        try:
+                            serialized = _serialize_return_value(res, encoding)
+                            if not isinstance(res, bytes):
+                                serialized += b'\0'
+                            await response.write(serialized)
+                            count += 1
+                        except (CancelledError, ConnectionResetError, ClientConnectionError):
+                            if api.on_disconnect is not None:
+                                args = (instance, res, ) if api.is_instance_method else (res, )
+                                if inspect.iscoroutinefunction(api.on_disconnect):
+                                    await api.on_disconnect(*args)
+                                else:
+                                    api.on_disconnect(*args)
+                            raise
+
                 except (CancelledError, ConnectionResetError, ClientConnectionError):
                     raise
                 except Exception as e:
                     print(str(e))
                     await async_q.put(None)
                     raise RuntimeError(f"Exception in server-side logic: {e}") from e
                 await response.write_eof()
```

### Comparing `bantam-2.2.3/src/bantam/js.py` & `bantam-2.2.4/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/src/bantam/js_async.py` & `bantam-2.2.4/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/src/bantam/pythonclient.py` & `bantam-2.2.4/src/bantam/pythonclient.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/src/bantam.egg-info/PKG-INFO` & `bantam-2.2.4/src/bantam.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.3
+Version: 2.2.4
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.3
+Download-URL: https://github.com/bantam/dist/2.2.4
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.3/src/bantam.egg-info/SOURCES.txt` & `bantam-2.2.4/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/test/test_client_get.py` & `bantam-2.2.4/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/test/test_client_post.py` & `bantam-2.2.4/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/test/test_client_post_inherited_apis.py` & `bantam-2.2.4/test/test_client_post_inherited_apis.py`

 * *Files 9% similar despite different names*

```diff
@@ -115,7 +115,30 @@
             assert item == str(29)
             count += 1
         assert count == 200
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
+
+
+@pytest.mark.asyncio
+async def test_client_instance_method_streamed_str_disconnected(tmpdir):
+    from class_rest_inherit_apis import RestAPIExampleAsyncPostInheritedInterface
+    app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
+    task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_inherit_apis']))
+    try:
+        await asyncio.sleep(1)
+        Client = RestAPIExampleAsyncPostInheritedInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
+        instance = await Client.explicit_constructor(29)
+        count = 0
+        async for item in instance.my_value_repeated_string_disconnected(200):
+            assert item == str(29)*65537
+            count += 1
+            if count == 121:
+                break  # disconnects client
+        await asyncio.sleep(1)  # give server time to process disconnect
+        assert RestAPIExampleAsyncPostInheritedInterface.disconnected
+    finally:
+        task.cancel()
+        with suppress(CancelledError):
+            await task
```

### Comparing `bantam-2.2.3/test/test_conversions.py` & `bantam-2.2.4/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/test/test_decorators.py` & `bantam-2.2.4/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/test/test_js.py` & `bantam-2.2.4/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.3/test/test_js_async.py` & `bantam-2.2.4/test/test_js_async.py`

 * *Files identical despite different names*

