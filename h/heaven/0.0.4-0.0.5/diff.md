# Comparing `tmp/heaven-0.0.4.tar.gz` & `tmp/heaven-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.0.4.tar", max compression
+gzip compressed data, was "heaven-0.0.5.tar", max compression
```

## Comparing `heaven-0.0.4.tar` & `heaven-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.4/LICENSE
--rw-r--r--   0        0        0     1312 2023-06-10 13:10:30.152074 heaven-0.0.4/README.md
--rw-r--r--   0        0        0      216 2023-06-10 13:11:18.625084 heaven-0.0.4/heaven/__init__.py
--rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.4/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.4/heaven/context.py
--rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.4/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.4/heaven/form.py
--rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.4/heaven/mocks.py
--rw-r--r--   0        0        0     3427 2023-06-10 23:16:34.082772 heaven-0.0.4/heaven/request.py
--rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.4/heaven/response.py
--rw-r--r--   0        0        0    21607 2023-06-10 23:32:01.834217 heaven-0.0.4/heaven/router.py
--rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.4/heaven/server.py
--rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.4/heaven/tutorials.py
--rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.4/heaven/utils.py
--rw-r--r--   0        0        0      485 2023-06-10 23:37:54.237700 heaven-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 heaven-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1312 2023-06-10 13:10:30.152074 heaven-0.0.5/README.md
+-rw-r--r--   0        0        0      216 2023-06-11 00:42:20.272309 heaven-0.0.5/heaven/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.5/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.5/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.5/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.5/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.5/heaven/mocks.py
+-rw-r--r--   0        0        0     3427 2023-06-10 23:16:34.082772 heaven-0.0.5/heaven/request.py
+-rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.5/heaven/response.py
+-rw-r--r--   0        0        0    21987 2023-06-11 00:41:32.757365 heaven-0.0.5/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.5/heaven/server.py
+-rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.5/heaven/tutorials.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.5/heaven/utils.py
+-rw-r--r--   0        0        0      485 2023-06-11 00:42:49.100375 heaven-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 heaven-0.0.5/PKG-INFO
```

### Comparing `heaven-0.0.4/LICENSE` & `heaven-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/README.md` & `heaven-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/heaven/constants.py` & `heaven-0.0.5/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/heaven/form.py` & `heaven-0.0.5/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/heaven/mocks.py` & `heaven-0.0.5/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/heaven/request.py` & `heaven-0.0.5/heaven/request.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/heaven/response.py` & `heaven-0.0.5/heaven/response.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/heaven/router.py` & `heaven-0.0.5/heaven/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -456,34 +456,41 @@
 
             try: assert isinstance(second, Callable)
             except AssertionError: raise TypeError(error_message)
 
             if first.lower() == STARTUP: self.initializers.append(closure(second))
             else: self.deinitializers.append(closure(second))
 
-    def TEMPLATES(self, folder: str, escape=None, asynchronous=True):
+    def TEMPLATES(self, folder: str, escape=None, asynchronous=True, relative_to=None):
+        # TODO: add warning if root folder slash is used
+        if relative_to: relative_file_path_folder = path.realpath(path.dirname(relative_to))
+        else: relative_file_path_folder = getcwd()
+
+        file_system_loader = FileSystemLoader(path.join(relative_file_path_folder, folder))
         files_to_escape = escape or ['htm', 'html']
-        file_system_loader = FileSystemLoader(path.join(getcwd(), folder))
         environment = Environment(loader=file_system_loader, autoescape=select_autoescape(files_to_escape))
         environment.is_async = asynchronous
         self._templater = environment
 
-    def ASSETS(self, folder: str, route='/public/*', subdomain=DEFAULT):
+    def ASSETS(self, folder: str, route='/public/*', subdomain=DEFAULT, relative_to=None):
+        # TODO: add warning if root folder slash is used
+        if relative_to: assets_folder_path = path.realpath(path.dirname(relative_to))
+        else: assets_folder_path = path.realpath(getcwd())
+
         async def serve_assets(req: Request, res: Response, ctx: Context):
             static_asset = f"{req.params.get('*', '')}"
-            remove_symlinks_if_present = path.realpath(getcwd())
-            location = path.join(remove_symlinks_if_present, f'{folder}')
+            location = path.join(assets_folder_path, f'{folder}')
             target_resource_path = path.join(location, static_asset)
             try:
                 async with async_open_file(target_resource_path, 'rb') as opened_asset_file:
                     _set_content_type(req, res)
                     res.body = b''.join(await opened_asset_file.readlines())
             except Exception as exc:
                 print(exc)
-                res.status = HTTPStatus.INTERNAL_SERVER_ERROR
+                res.status = HTTPStatus.NOT_FOUND
         self.GET(route, serve_assets, subdomain)
 
     async def _register(self):
         i = len(self.initializers)
         while self.initializers:
             initializer, c = self.initializers.popleft(), len(self.initializers)
             index = i - c
```

### Comparing `heaven-0.0.4/heaven/tutorials.py` & `heaven-0.0.5/heaven/tutorials.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/heaven/utils.py` & `heaven-0.0.5/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.4/PKG-INFO` & `heaven-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

