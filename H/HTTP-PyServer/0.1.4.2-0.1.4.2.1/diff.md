# Comparing `tmp/HTTP-PyServer-0.1.4.2.tar.gz` & `tmp/HTTP-PyServer-0.1.4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.4.2.tar", last modified: Sun Jun 11 01:48:49 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.4.2.1.tar", last modified: Sun Jun 11 02:13:36 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.4.2.tar` & `HTTP-PyServer-0.1.4.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 01:48:49.161496 HTTP-PyServer-0.1.4.2/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.2/LICENSE
--rw-rw-rw-   0        0        0     2106 2023-06-11 01:48:49.158055 HTTP-PyServer-0.1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.2/README.md
--rw-rw-rw-   0        0        0      643 2023-06-11 01:47:55.000000 HTTP-PyServer-0.1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 01:48:49.161496 HTTP-PyServer-0.1.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 01:48:49.107680 HTTP-PyServer-0.1.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 01:48:49.125817 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2106 2023-06-11 01:48:49.000000 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-11 01:48:49.000000 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 01:48:49.000000 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 01:48:49.000000 HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 01:48:49.156231 HTTP-PyServer-0.1.4.2/src/server/
--rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.2/src/server/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.2/src/server/cache.py
--rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.2/src/server/render.py
--rw-rw-rw-   0        0        0     4527 2023-06-11 01:44:30.000000 HTTP-PyServer-0.1.4.2/src/server/request.py
--rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.2/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.2/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.2/src/server/response_messages.py
--rw-rw-rw-   0        0        0     8864 2023-05-17 20:18:32.000000 HTTP-PyServer-0.1.4.2/src/server/routes.py
--rw-rw-rw-   0        0        0     7458 2023-06-11 01:44:49.000000 HTTP-PyServer-0.1.4.2/src/server/server.py
--rw-rw-rw-   0        0        0     3608 2023-05-17 19:38:59.000000 HTTP-PyServer-0.1.4.2/src/server/sessions.py
--rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.2/src/server/template.py
+drwxrwxrwx   0        0        0        0 2023-06-11 02:13:36.298981 HTTP-PyServer-0.1.4.2.1/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2108 2023-06-11 02:13:36.296988 HTTP-PyServer-0.1.4.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.2.1/README.md
+-rw-rw-rw-   0        0        0      645 2023-06-11 02:13:12.000000 HTTP-PyServer-0.1.4.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 02:13:36.299979 HTTP-PyServer-0.1.4.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 02:13:36.225150 HTTP-PyServer-0.1.4.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 02:13:36.255585 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2108 2023-06-11 02:13:36.000000 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-11 02:13:36.000000 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 02:13:36.000000 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 02:13:36.000000 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 02:13:36.293993 HTTP-PyServer-0.1.4.2.1/src/server/
+-rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.2.1/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.2.1/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.2.1/src/server/render.py
+-rw-rw-rw-   0        0        0     4565 2023-06-11 02:11:17.000000 HTTP-PyServer-0.1.4.2.1/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.2.1/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.2.1/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.2.1/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     8864 2023-05-17 20:18:32.000000 HTTP-PyServer-0.1.4.2.1/src/server/routes.py
+-rw-rw-rw-   0        0        0     7449 2023-06-11 02:12:16.000000 HTTP-PyServer-0.1.4.2.1/src/server/server.py
+-rw-rw-rw-   0        0        0     3608 2023-05-17 19:38:59.000000 HTTP-PyServer-0.1.4.2.1/src/server/sessions.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.2.1/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.4.2/LICENSE` & `HTTP-PyServer-0.1.4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/PKG-INFO` & `HTTP-PyServer-0.1.4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.2
+Version: 0.1.4.2.1
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.4.2/README.md` & `HTTP-PyServer-0.1.4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/pyproject.toml` & `HTTP-PyServer-0.1.4.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.4.2"
+version = "0.1.4.2.1"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.4.2/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.2
+Version: 0.1.4.2.1
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.4.2/src/server/cache.py` & `HTTP-PyServer-0.1.4.2.1/src/server/cache.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/src/server/render.py` & `HTTP-PyServer-0.1.4.2.1/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/src/server/request.py` & `HTTP-PyServer-0.1.4.2.1/src/server/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,21 +94,23 @@
 
         try:
 
             cookies = {}
 
             for cookie in self.headers.get('Cookie').split(';'):
 
-                key, value = urllib.parse.parse_qs(cookie.strip()).items()
+                key, value = list(urllib.parse.parse_qs(cookie.strip()).items())[0]
 
                 cookies[key] = value[0]
 
             return cookies
         
-        except Exception:
+        except Exception as e:
+
+            print(e)
 
             return {}
 
     def json(self):
         '''Returns the request body as a JSON object.'''
 
         return json.loads(self.body.decode(encoding = 'utf-8',
```

### Comparing `HTTP-PyServer-0.1.4.2/src/server/response.py` & `HTTP-PyServer-0.1.4.2.1/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/src/server/response_codes.py` & `HTTP-PyServer-0.1.4.2.1/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/src/server/response_messages.py` & `HTTP-PyServer-0.1.4.2.1/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/src/server/routes.py` & `HTTP-PyServer-0.1.4.2.1/src/server/routes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/src/server/server.py` & `HTTP-PyServer-0.1.4.2.1/src/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,20 +160,20 @@
                         return None
 
                 try:
 
                     parsed_request = request.Request.from_bytestring(address = address,
                                                                 request = raw_request)
 
-                except Exception as e:
+                except Exception:
 
                     if self._logger:
 
                         self._logger.error(f'Invalid request from \
-{address[0]}:{address[1]}, closing connection. {e}')
+{address[0]}:{address[1]}, closing connection.')
 
                     connection.close()
 
                     return None
 
                 if content_length:=parsed_request.headers.get('Content-Length'):
```

### Comparing `HTTP-PyServer-0.1.4.2/src/server/sessions.py` & `HTTP-PyServer-0.1.4.2.1/src/server/sessions.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2/src/server/template.py` & `HTTP-PyServer-0.1.4.2.1/src/server/template.py`

 * *Files identical despite different names*

