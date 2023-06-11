# Comparing `tmp/HTTP-PyServer-0.1.4.1.1.tar.gz` & `tmp/HTTP-PyServer-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.4.1.1.tar", last modified: Wed May 24 00:22:46 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.4.2.tar", last modified: Sun Jun 11 01:48:49 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.4.1.1.tar` & `HTTP-PyServer-0.1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 00:22:46.647447 HTTP-PyServer-0.1.4.1.1/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.1.1/LICENSE
--rw-rw-rw-   0        0        0     2095 2023-05-24 00:22:46.646451 HTTP-PyServer-0.1.4.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1530 2023-05-17 20:22:16.000000 HTTP-PyServer-0.1.4.1.1/README.md
--rw-rw-rw-   0        0        0      645 2023-05-24 00:22:19.000000 HTTP-PyServer-0.1.4.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 00:22:46.647447 HTTP-PyServer-0.1.4.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 00:22:46.606557 HTTP-PyServer-0.1.4.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 00:22:46.621518 HTTP-PyServer-0.1.4.1.1/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2095 2023-05-24 00:22:46.000000 HTTP-PyServer-0.1.4.1.1/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-05-24 00:22:46.000000 HTTP-PyServer-0.1.4.1.1/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 00:22:46.000000 HTTP-PyServer-0.1.4.1.1/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 00:22:46.000000 HTTP-PyServer-0.1.4.1.1/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 00:22:46.644456 HTTP-PyServer-0.1.4.1.1/src/server/
--rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.1.1/src/server/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.1.1/src/server/cache.py
--rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.1.1/src/server/render.py
--rw-rw-rw-   0        0        0     2800 2023-05-17 19:26:23.000000 HTTP-PyServer-0.1.4.1.1/src/server/request.py
--rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.1.1/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.1.1/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.1.1/src/server/response_messages.py
--rw-rw-rw-   0        0        0     8864 2023-05-17 20:18:32.000000 HTTP-PyServer-0.1.4.1.1/src/server/routes.py
--rw-rw-rw-   0        0        0     7645 2023-05-24 00:20:54.000000 HTTP-PyServer-0.1.4.1.1/src/server/server.py
--rw-rw-rw-   0        0        0     3608 2023-05-17 19:38:59.000000 HTTP-PyServer-0.1.4.1.1/src/server/sessions.py
--rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.1.1/src/server/template.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:48:49.161496 HTTP-PyServer-0.1.4.2/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     2106 2023-06-11 01:48:49.158055 HTTP-PyServer-0.1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.2/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-11 01:47:55.000000 HTTP-PyServer-0.1.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 01:48:49.161496 HTTP-PyServer-0.1.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 01:48:49.107680 HTTP-PyServer-0.1.4.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 01:48:49.125817 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2106 2023-06-11 01:48:49.000000 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-11 01:48:49.000000 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 01:48:49.000000 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 01:48:49.000000 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 01:48:49.156231 HTTP-PyServer-0.1.4.2/src/server/
+-rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.2/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.2/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.2/src/server/render.py
+-rw-rw-rw-   0        0        0     4527 2023-06-11 01:44:30.000000 HTTP-PyServer-0.1.4.2/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.2/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.2/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.2/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     8864 2023-05-17 20:18:32.000000 HTTP-PyServer-0.1.4.2/src/server/routes.py
+-rw-rw-rw-   0        0        0     7458 2023-06-11 01:44:49.000000 HTTP-PyServer-0.1.4.2/src/server/server.py
+-rw-rw-rw-   0        0        0     3608 2023-05-17 19:38:59.000000 HTTP-PyServer-0.1.4.2/src/server/sessions.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.2/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.4.1.1/LICENSE` & `HTTP-PyServer-0.1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.1.1/PKG-INFO` & `HTTP-PyServer-0.1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.1.1
+Version: 0.1.4.2
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -66,7 +66,8 @@
 - `re`
 - `time`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
 - `ssl`
+- `secrets`
```

### Comparing `HTTP-PyServer-0.1.4.1.1/README.md` & `HTTP-PyServer-0.1.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,7 +52,8 @@
 - `re`
 - `time`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
 - `ssl`
+- `secrets`
```

### Comparing `HTTP-PyServer-0.1.4.1.1/pyproject.toml` & `HTTP-PyServer-0.1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.4.1.1"
+version = "0.1.4.2"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.4.1.1/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.1.1
+Version: 0.1.4.2
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -66,7 +66,8 @@
 - `re`
 - `time`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
 - `ssl`
+- `secrets`
```

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/cache.py` & `HTTP-PyServer-0.1.4.2/src/server/cache.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/render.py` & `HTTP-PyServer-0.1.4.2/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/response.py` & `HTTP-PyServer-0.1.4.2/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/response_codes.py` & `HTTP-PyServer-0.1.4.2/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/response_messages.py` & `HTTP-PyServer-0.1.4.2/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/routes.py` & `HTTP-PyServer-0.1.4.2/src/server/routes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/server.py` & `HTTP-PyServer-0.1.4.2/src/server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,22 +134,21 @@
                         address: socket.AddressInfo) -> None:
         '''Handles a request from a client.'''
 
         while True:
             
             try:
 
-                raw_request = ''
+                raw_request = b''
 
                 while True:
 
-                    raw_request += connection.recv(4096).decode(encoding = 'utf-8',
-                                                                errors = 'ignore')
+                    raw_request += connection.recv(4096)
 
-                    if '\r\n\r\n' in raw_request or raw_request == '':
+                    if b'\r\n\r\n' in raw_request or raw_request == b'':
 
                         break
 
                 if not raw_request:
                         
                         if self._logger:
 
@@ -158,44 +157,43 @@
 
                         connection.close()
 
                         return None
 
                 try:
 
-                    parsed_request = request.Request.from_string(address = address,
-                                                                 request = raw_request)
+                    parsed_request = request.Request.from_bytestring(address = address,
+                                                                request = raw_request)
 
-                except Exception:
+                except Exception as e:
 
                     if self._logger:
 
                         self._logger.error(f'Invalid request from \
-{address[0]}:{address[1]}, closing connection.')
+{address[0]}:{address[1]}, closing connection. {e}')
 
                     connection.close()
 
                     return None
 
                 if content_length:=parsed_request.headers.get('Content-Length'):
 
-                    if (length_recieved:=len(raw_request.split('\r\n\r\n')[1])) < \
+                    if (length_recieved:=len(raw_request.split(b'\r\n\r\n')[1])) < \
                     (length_to_recieve:=int(content_length)):
 
                         raw_request += connection.recv(length_to_recieve - \
-                                                       length_recieved)\
-                            .decode(encoding = 'utf-8',
-                                    errors = 'ignore')
+                                                       length_recieved)
+
+                        parsed_request = request.Request.from_bytestring(
+                                        address = address,
+                                        request = raw_request)
 
-                        parsed_request = request.Request.from_string(address = address,
-                                                                request = raw_request)
-                        
                 if self._logger:
 
-                    self._logger.debug(f'Recieved request from \
+                    self._logger.debug(f'Recieved {parsed_request.method} request from \
 {address[0]}:{address[1]} for {parsed_request.path if parsed_request.path else "/"}')
 
                 connection.send(self._get_route(path = parsed_request.path,
                                                 request = parsed_request))
                 
                 if self._logger:
```

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/sessions.py` & `HTTP-PyServer-0.1.4.2/src/server/sessions.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.1.1/src/server/template.py` & `HTTP-PyServer-0.1.4.2/src/server/template.py`

 * *Files identical despite different names*

