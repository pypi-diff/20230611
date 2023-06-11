# Comparing `tmp/sourceserver-0.9.1.tar.gz` & `tmp/sourceserver-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourceserver-0.9.1.tar", last modified: Sun Sep 19 16:24:28 2021, max compression
+gzip compressed data, was "sourceserver-0.9.2.tar", last modified: Tue Feb  8 05:07:04 2022, max compression
```

## Comparing `sourceserver-0.9.1.tar` & `sourceserver-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 16:24:28.751357 sourceserver-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-09-19 16:24:21.000000 sourceserver-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2021-09-19 16:24:28.751357 sourceserver-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2021-09-19 16:24:21.000000 sourceserver-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-19 16:24:28.751357 sourceserver-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-09-19 16:24:21.000000 sourceserver-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 16:24:28.751357 sourceserver-0.9.1/sourceserver/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 16:24:21.000000 sourceserver-0.9.1/sourceserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-09-19 16:24:21.000000 sourceserver-0.9.1/sourceserver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6407 2021-09-19 16:24:21.000000 sourceserver-0.9.1/sourceserver/masterserver.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-09-19 16:24:21.000000 sourceserver-0.9.1/sourceserver/peekablestream.py
--rw-r--r--   0 runner    (1001) docker     (121)    13902 2021-09-19 16:24:21.000000 sourceserver-0.9.1/sourceserver/sourceserver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 16:24:28.751357 sourceserver-0.9.1/sourceserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2021-09-19 16:24:28.000000 sourceserver-0.9.1/sourceserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-09-19 16:24:28.000000 sourceserver-0.9.1/sourceserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-19 16:24:28.000000 sourceserver-0.9.1/sourceserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-19 16:24:28.000000 sourceserver-0.9.1/sourceserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-08 05:07:04.444298 sourceserver-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)    35149 2022-02-08 05:06:52.000000 sourceserver-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     3005 2022-02-08 05:07:04.444298 sourceserver-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2567 2022-02-08 05:06:52.000000 sourceserver-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-02-08 05:07:04.444298 sourceserver-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      668 2022-02-08 05:06:52.000000 sourceserver-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-08 05:07:04.444298 sourceserver-0.9.2/sourceserver/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-08 05:06:52.000000 sourceserver-0.9.2/sourceserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      466 2022-02-08 05:06:52.000000 sourceserver-0.9.2/sourceserver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6407 2022-02-08 05:06:52.000000 sourceserver-0.9.2/sourceserver/masterserver.py
+-rw-r--r--   0 runner    (1001) docker     (116)      281 2022-02-08 05:06:52.000000 sourceserver-0.9.2/sourceserver/peekablestream.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14140 2022-02-08 05:06:52.000000 sourceserver-0.9.2/sourceserver/sourceserver.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-08 05:07:04.444298 sourceserver-0.9.2/sourceserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3005 2022-02-08 05:07:04.000000 sourceserver-0.9.2/sourceserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      311 2022-02-08 05:07:04.000000 sourceserver-0.9.2/sourceserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-08 05:07:04.000000 sourceserver-0.9.2/sourceserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2022-02-08 05:07:04.000000 sourceserver-0.9.2/sourceserver.egg-info/top_level.txt
```

### Comparing `sourceserver-0.9.1/LICENSE` & `sourceserver-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sourceserver-0.9.1/PKG-INFO` & `sourceserver-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sourceserver
-Version: 0.9.1
+Version: 0.9.2
 Summary: Query Source engine servers over UDP
 Home-page: https://github.com/Derpius/pythonsourceserver/
-Author: 100 Pixels Squared
-Author-email: 100pxsquared@gmail.com
+Author: Derpius
+Author-email: derpius.yt@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sourceserver-0.9.1/README.md` & `sourceserver-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `sourceserver-0.9.1/setup.py` & `sourceserver-0.9.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = []
 
 setup(
     name="sourceserver",
-    version="0.9.1",
-    author="100 Pixels Squared",
-    author_email="100pxsquared@gmail.com",
+    version="0.9.2",
+    author="Derpius",
+    author_email="derpius.yt@gmail.com",
     description="Query Source engine servers over UDP",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/Derpius/pythonsourceserver/",
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
```

### Comparing `sourceserver-0.9.1/sourceserver/masterserver.py` & `sourceserver-0.9.2/sourceserver/masterserver.py`

 * *Files identical despite different names*

### Comparing `sourceserver-0.9.1/sourceserver/sourceserver.py` & `sourceserver-0.9.2/sourceserver/sourceserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
 		# Set up connection
 		self.constr = connectionString
 		self._ip, self._port = connectionString.split(":")
 		self._port = int(self._port)
 
 		try: self._connect()
-		except SourceError:
-			self._log("Failed to connect to server")
+		except SourceError as e:
+			self._log("Failed to connect to server: " + e.message)
 			self.isClosed = True
 		else: self._log("Successfully established connection to server")
 
 	def _openSocket(self):
 		'''Open the socket to the server'''
 		self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 		self.socket.setblocking(0)
@@ -281,14 +281,16 @@
 		return rulesDict
 	
 	def _getInfo(self):
 		'''Gets the server's information'''
 		self._openSocket()
 
 		response = self._request(bytes.fromhex("FF FF FF FF 54 53 6F 75 72 63 65 20 45 6E 67 69 6E 65 20 51 75 65 72 79 00"))
+		if len(response) == 9 and response[4] == 0x41: # Info request requires challenge
+			response = self._request(bytes.fromhex("FF FF FF FF 54 53 6F 75 72 63 65 20 45 6E 67 69 6E 65 20 51 75 65 72 79 00") + response[5:])
 		if len(response) < 23 or response[4] != 0x49: raise SourceError(self, "Info response header invalid")
 
 		# Tokenise and return info
 		ret = self._tokeniseInfo(response[5:])
 		self._closeSocket()
 		return ret
```

### Comparing `sourceserver-0.9.1/sourceserver.egg-info/PKG-INFO` & `sourceserver-0.9.2/sourceserver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sourceserver
-Version: 0.9.1
+Version: 0.9.2
 Summary: Query Source engine servers over UDP
 Home-page: https://github.com/Derpius/pythonsourceserver/
-Author: 100 Pixels Squared
-Author-email: 100pxsquared@gmail.com
+Author: Derpius
+Author-email: derpius.yt@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

