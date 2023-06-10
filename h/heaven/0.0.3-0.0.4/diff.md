# Comparing `tmp/heaven-0.0.3.tar.gz` & `tmp/heaven-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.0.3.tar", max compression
+gzip compressed data, was "heaven-0.0.4.tar", max compression
```

## Comparing `heaven-0.0.3.tar` & `heaven-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.3/LICENSE
--rw-r--r--   0        0        0     1312 2023-06-10 13:10:30.152074 heaven-0.0.3/README.md
--rw-r--r--   0        0        0      216 2023-06-10 13:11:18.625084 heaven-0.0.3/heaven/__init__.py
--rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.3/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.3/heaven/context.py
--rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.3/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.3/heaven/form.py
--rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.3/heaven/mocks.py
--rw-r--r--   0        0        0     3188 2023-06-10 13:10:30.157851 heaven-0.0.3/heaven/request.py
--rw-r--r--   0        0        0     3999 2023-06-10 13:10:30.158043 heaven-0.0.3/heaven/response.py
--rw-r--r--   0        0        0    20838 2023-06-10 13:10:30.158327 heaven-0.0.3/heaven/router.py
--rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.3/heaven/server.py
--rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.3/heaven/tutorials.py
--rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.3/heaven/utils.py
--rw-r--r--   0        0        0      485 2023-06-10 13:12:13.066504 heaven-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 heaven-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1312 2023-06-10 13:10:30.152074 heaven-0.0.4/README.md
+-rw-r--r--   0        0        0      216 2023-06-10 13:11:18.625084 heaven-0.0.4/heaven/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.4/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.4/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.4/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.4/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.4/heaven/mocks.py
+-rw-r--r--   0        0        0     3427 2023-06-10 23:16:34.082772 heaven-0.0.4/heaven/request.py
+-rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.4/heaven/response.py
+-rw-r--r--   0        0        0    21607 2023-06-10 23:32:01.834217 heaven-0.0.4/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.4/heaven/server.py
+-rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.4/heaven/tutorials.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.4/heaven/utils.py
+-rw-r--r--   0        0        0      485 2023-06-10 23:37:54.237700 heaven-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 heaven-0.0.4/PKG-INFO
```

### Comparing `heaven-0.0.3/LICENSE` & `heaven-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.0.3/README.md` & `heaven-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.0.3/heaven/constants.py` & `heaven-0.0.4/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.3/heaven/form.py` & `heaven-0.0.4/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.3/heaven/mocks.py` & `heaven-0.0.4/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.3/heaven/request.py` & `heaven-0.0.4/heaven/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         self._body = body
         self._cookies = None
         self._form = None
         self._receive = receive
         self._scope = scope
         self._subdomain, self._headers = metadata
         self._params = None
+        self._mounted_from_application = None
 
     def _parse_qs(self):
         qs = self._scope.get("query_string")
         qsd = {}
         if not qs:
             return qsd
         else:
@@ -81,14 +82,22 @@
         return self._headers
 
     @property
     def method(self):
         return self._scope.get("method")
 
     @property
+    def mounted(self):
+        return self._mounted_from_application
+
+    @mounted.setter
+    def mounted(self, value: 'Router'):
+        self._mounted_from_application
+
+    @property
     def params(self):
         if not self._params:
             self._params = self._parse_qs()
         return self._params
 
     @params.setter
     def params(self, pair):
```

### Comparing `heaven-0.0.3/heaven/response.py` & `heaven-0.0.4/heaven/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self._abort = False
         self._body = MESSAGE_NOT_FOUND.encode()
         self._deferred = []
         self._metadata = {}
         self._headers = []
         self._status = STATUS_NOT_FOUND
         self._template = None
+        self._mounted_from_application = None
 
     @MethodDispatch
     def abort(self, payload):
         self._abort = True
         self._body = payload
 
     @abort.register(str)
@@ -91,38 +92,47 @@
         value = _encode(key), _encode(val)
         self._headers.append(value)
     
     def file(self, name: str, folder='public'):
         """Serve file from assets/public folder with correct file type from known_file_types"""
         pass
 
+    @property
+    def metadata(self):
+        return self._metadata
+
+    @metadata.setter
+    def metadata(self, value):
+        if not isinstance(value, dict): raise ValueError
+        self._metadata = value
+
+    @property
+    def mounted(self):
+        return self._mounted_from_application
+
+    @mounted.setter
+    def mounted(self, value: 'App'):
+        self._mounted_from_application = value
+
     async def render(self, name: str, **contexts):
         """Serve html file walking up parent router/app tree until base parent if necessary"""
-        templater = self._app._templater
+        # TODO: add support to customize order in **contexts later when you think of the api and make an atomic commit
+        templater = self.mounted._templater or self._app._templater
         if not templater:
             self.headers = 'Content-Type', 'text/html'
             self.status = HTTPStatus.INTERNAL_SERVER_ERROR
             self.body = get_guardian_angel_html('You did not enable templating', NO_TEMPLATING)
             return
         template = templater.get_template(name)
         self.body = await template.render_async({'ctx': self._ctx, **contexts})
 
     def renders(self, name: str):
         """Synchronous version of render method above"""
         pass
 
-    @property
-    def metadata(self):
-        return self._metadata
-
-    @metadata.setter
-    def metadata(self, value):
-        if not isinstance(value, dict): raise ValueError
-        self._metadata = value
-
     def redirect(self, location, permanent=False):
         if permanent: self.status = HTTPStatus.PERMANENT_REDIRECT
         else: self.status = HTTPStatus.TEMPORARY_REDIRECT
         self.headers = 'Location', location
 
     @property
     def status(self):
```

### Comparing `heaven-0.0.3/heaven/router.py` & `heaven-0.0.4/heaven/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,23 @@
 
 
 Handler = Callable[[Request, Response], object]
 
 SEPARATOR = INDEX = "/"
 
 
+def _closure_mounted_application(handler: Handler, mounted: 'Router'):
+    async def delegate(req: Request, res: Response, ctx: Context):
+        req.mounted = mounted
+        res.mounted = mounted
+        if iscoroutinefunction(handler): await handler(req, res, ctx)
+        else: handler(req, res, ctx)
+    return delegate
+
+
 def _get_configuration(configurator=None):
     if not configurator: return {}
     if isinstance(configurator, dict): return configurator
     return configurator()
 
 
 def _isparamx(r: str):
@@ -64,14 +73,21 @@
 def _notify(width=80, event=STARTUP): #pragma: nocover
     drawline = lambda: print('=' * width)
     drawline()
     print(f'NOTE: The `LAST` {event} func above failed and prevented others from running')
     drawline()
 
 
+def _set_content_type(req: Request, res: Response):
+    ct = 'Content-Type'
+    if(req.url.endswith('.css')): res.headers = ct, 'text/css'
+    elif(req.url.endswith('.svg')): res.headers = ct, 'image/svg+xml'
+    elif(req.url.endswith('.js')): res.headers = ct, 'text/javascript'
+
+
 class Route(object):
     def __init__(self, route: str, handler: Callable, router: 'Router') -> None:
         self.heaven_instance = router
         self.parameterized = False
         self.route = route
         self.handler = handler
         self.children = {}
@@ -455,14 +471,15 @@
         async def serve_assets(req: Request, res: Response, ctx: Context):
             static_asset = f"{req.params.get('*', '')}"
             remove_symlinks_if_present = path.realpath(getcwd())
             location = path.join(remove_symlinks_if_present, f'{folder}')
             target_resource_path = path.join(location, static_asset)
             try:
                 async with async_open_file(target_resource_path, 'rb') as opened_asset_file:
+                    _set_content_type(req, res)
                     res.body = b''.join(await opened_asset_file.readlines())
             except Exception as exc:
                 print(exc)
                 res.status = HTTPStatus.INTERNAL_SERVER_ERROR
         self.GET(route, serve_assets, subdomain)
 
     async def _register(self):
@@ -515,15 +532,16 @@
         for subdomain in router.subdomains:
             engine: Routes = router.subdomains[subdomain]
             for method in engine.cache:
                 cache = engine.cache[method]
                 for route in cache:
                     handler = cache[route]
                     self.subdomain(subdomain)
-                    self.abettor(method, route, handler, subdomain=subdomain, router=router if isolated else self)
+                    closured_handler = _closure_mounted_application(handler, router)
+                    self.abettor(method, route, closured_handler, subdomain=subdomain, router=router if isolated else self)
             for after in engine.afters:
                 self.subdomains[subdomain].afters[after] = [*engine.afters[after], *self.subdomains[subdomain].afters.get(after, [])]
             for before in engine.befores:
                 self.subdomains[subdomain].befores[before] = [*engine.befores[before], *self.subdomains[subdomain].befores.get(before, [])]
 
 
 class Application(Router):...
```

### Comparing `heaven-0.0.3/heaven/tutorials.py` & `heaven-0.0.4/heaven/tutorials.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.3/heaven/utils.py` & `heaven-0.0.4/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.3/PKG-INFO` & `heaven-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

