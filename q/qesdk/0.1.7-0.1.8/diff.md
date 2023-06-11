# Comparing `tmp/qesdk-0.1.7.tar.gz` & `tmp/qesdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qesdk-0.1.7.tar", last modified: Sun May 28 05:21:43 2023, max compression
+gzip compressed data, was "qesdk-0.1.8.tar", last modified: Sun Jun 11 13:23:30 2023, max compression
```

## Comparing `qesdk-0.1.7.tar` & `qesdk-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 05:21:43.977211 qesdk-0.1.7/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       38 2023-05-26 12:51:28.000000 qesdk-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6225 2023-05-28 05:21:43.977211 qesdk-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.7/README.md
--rw-rw-rw-   0        0        0      751 2023-05-28 05:21:07.000000 qesdk-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 05:21:43.977211 qesdk-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 05:21:43.963352 qesdk-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 05:21:43.972551 qesdk-0.1.7/src/qesdk/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.7/src/qesdk/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.7/src/qesdk/aio_api.py
--rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.7/src/qesdk/api.py
--rw-rw-rw-   0        0        0     7088 2023-05-28 05:20:54.000000 qesdk-0.1.7/src/qesdk/client.py
--rw-rw-rw-   0        0        0      237 2023-05-26 12:40:26.000000 qesdk-0.1.7/src/qesdk/config.py
--rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.7/src/qesdk/qedata.thrift
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.7/src/qesdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 05:21:43.975879 qesdk-0.1.7/src/qesdk.egg-info/
--rw-rw-rw-   0        0        0     6225 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 13:23:30.147007 qesdk-0.1.8/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       38 2023-05-26 12:51:28.000000 qesdk-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6225 2023-06-11 13:23:30.147007 qesdk-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.8/README.md
+-rw-rw-rw-   0        0        0      751 2023-06-11 13:17:44.000000 qesdk-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 13:23:30.147007 qesdk-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 13:23:30.130007 qesdk-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 13:23:30.141008 qesdk-0.1.8/src/qesdk/
+-rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.8/src/qesdk/__init__.py
+-rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.8/src/qesdk/aio_api.py
+-rw-rw-rw-   0        0        0    29394 2023-06-08 10:07:17.000000 qesdk-0.1.8/src/qesdk/api.py
+-rw-rw-rw-   0        0        0     7286 2023-06-11 13:17:29.000000 qesdk-0.1.8/src/qesdk/client.py
+-rw-rw-rw-   0        0        0      237 2023-05-26 12:40:26.000000 qesdk-0.1.8/src/qesdk/config.py
+-rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.8/src/qesdk/qedata.thrift
+-rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.8/src/qesdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:23:30.146008 qesdk-0.1.8/src/qesdk.egg-info/
+-rw-rw-rw-   0        0        0     6225 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/top_level.txt
```

### Comparing `qesdk-0.1.7/LICENSE` & `qesdk-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.7/PKG-INFO` & `qesdk-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qesdk-0.1.7/README.md` & `qesdk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.7/pyproject.toml` & `qesdk-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qesdk"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Scott Zhang", email="scott2011@qq.com" },
 ]
 description = "Quantease SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `qesdk-0.1.7/src/qesdk/aio_api.py` & `qesdk-0.1.8/src/qesdk/aio_api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.7/src/qesdk/api.py` & `qesdk-0.1.8/src/qesdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,14 +692,19 @@
     return qedataClient.instance()('get_instrument_broker_pnl', **locals())
 
 @assert_auth
 def update_public_ip(hostip):
     return qedataClient.instance()('update_public_ip', **locals())
 
 
+@assert_auth
+def get_risk_control_parameter():
+    return qedataClient.instance()('get_risk_control_parameter', **locals())
+
+
 __all__ = []
 
 def _collect_func():
     funcs = []
     for func in globals().keys():
         if func.startswith("get") or func.startswith("sm_get") or func.startswith("is_") or func.startswith("update_"):
             funcs.append(func)
```

### Comparing `qesdk-0.1.7/src/qesdk/client.py` & `qesdk-0.1.8/src/qesdk/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,36 +8,40 @@
 import thriftpy2
 import asyncio
 import zlib
 import pickle
 import msgpack
 import json
 import sys
+import time
+import threading
 from os import getenv, path
 
 from thriftpy2.rpc import make_aio_client
+from thriftpy2.transport import TFramedTransportFactory
+from thriftpy2.protocol import TBinaryProtocolFactory
 from .utils import get_mac_address
 import nest_asyncio
 nest_asyncio.apply()
 
 try:
     from .config import outside_server_config, second_server_config
     avail_servers = [outside_server_config, second_server_config]
     server_config = avail_servers[0]
     server_index = 0
 except ImportError:
-    server_config = {'host' : '192.168.123.199',
+    server_config = {'host' : '192.168.18.4',
                      'port' : 6001}  
     avail_servers = [server_config]
     server_index = 0                 
 
     
 
 
-__version__='0.1.7'
+__version__='0.1.8'
 
 thrift_path = path.join(sys.modules["ROOT_DIR"], "qedata.thrift")
 thrift_path = path.abspath(thrift_path)
 #print(thrift_path)
 qedata_thrift = thriftpy2.load(thrift_path, module_name="qedata_thrift")
 loop = asyncio.get_event_loop()
 def setTimeout(client, timeout):
@@ -79,125 +83,145 @@
             
     @classmethod
     def check_login(cls):
         smtoken = cls._syssmtoken
         #print('auth',token)
         return smtoken != ''
     
+    @classmethod
+    def start_heartbeat(cls):
+        t = threading.Thread(target=cls.heartbeat)
+        t.daemon = True
+        t.start()
     
-    async def echo(self, name):
-        global server_config
-        client = await make_aio_client(
-            qedata_thrift.TestService, server_config['host'], server_config['port'])#,timeout=30*1000)
-        #setTimeout(client, 30*1000)
-        result = await client.echo(name)
-        print(result,self._systoken)
-        client.close()
     
-    async def queryData(self, method, **kwargs):
+    @classmethod
+    async def heartbeat(cls):
+        while True:
+            try:
+                # 进行心跳操作，例如发送一个心跳消息给服务器
+                # 这里使用 echo 方法作为心跳
+                await cls.instance().echo('heartbeat')
+                print('heartbeat')
+            except Exception as e:
+                print(f'Heartbeat failed: {e}')
+            time.sleep(10)  # 每隔60秒执行一次心跳
+    
+    @classmethod
+    async def getClient(cls):
         global server_config, server_index, avail_servers
         try:
             client = await make_aio_client(
-                qedata_thrift.TestService, server_config['host'],  server_config['port'], timeout=self.request_timeout)
+                qedata_thrift.TestService, server_config['host'],  server_config['port'], timeout=cls.request_timeout)
         except Exception as e:
             if len(avail_servers) > 1:
                 server_index = (server_index + 1) % len(avail_servers)
                 server_config = avail_servers[server_index]
-                client = await make_aio_client(qedata_thrift.TestService, server_config['host'],  server_config['port'], timeout=self.request_timeout)
-            else:
-                return f'ERROR: {e}'
-        #print('qeryData')
-        try:
-            setTimeout(client, self.request_timeout)
-            req = qedata_thrift.St_Query_Req()
-            req.method_name = method
-            req.params = zlib.compress(msgpack.dumps(kwargs,use_bin_type=True))
-            if "sm_get" in method:
-                req.token = self._syssmtoken
-            else:    
-                req.token=self._systoken
-            #print('token',req.token)
-            result = await client.query(req)
-            
+                client = await make_aio_client(qedata_thrift.TestService, server_config['host'],  server_config['port'], timeout=cls.request_timeout,\
+                    )
+    #,trans_factory=TFramedTransportFactory())
+            else:
+                print(f'ERROR: {e}')
+                return None
+        return client
+
+    async def echo(self, name):
+        global server_config
+        client = await self.getClient()
+        if client:
+            #setTimeout(client, 30*1000)
+            result = await client.echo(name)
+            print(result,self._systoken)
             client.close()
-            if result.status:
-                msg = result.msg
-                #print(msg)
-                return(pickle.loads(zlib.decompress(msg)))
+    
+    async def queryData(self, method, **kwargs):
+        global server_config, server_index, avail_servers
+        try:
+            client = await self.getClient()
+            if client:
+                setTimeout(client, self.request_timeout)
+                req = qedata_thrift.St_Query_Req()
+                req.method_name = method
+                req.params = zlib.compress(msgpack.dumps(kwargs,use_bin_type=True))
+                if "sm_get" in method:
+                    req.token = self._syssmtoken
+                else:    
+                    req.token=self._systoken
+                #print('token',req.token)
+                result = await client.query(req)
+                
+                client.close()
+                if result.status:
+                    msg = result.msg
+                    #print(msg)
+                    return(pickle.loads(zlib.decompress(msg)))
+                else:
+                    return(result.msg)
             else:
-                return(result.msg)
+                return "Client load failed"
         except Exception as e:
             return f'ERROR: {e}'
             
     @classmethod
     async def login(cls, username, password):
-        global server_config, server_index,avail_servers
-        try:
-            client = await make_aio_client(
-                qedata_thrift.TestService, server_config['host'],  server_config['port'],timeout=cls.request_timeout)
-        except Exception as e:
-            if len(avail_servers) > 1:
-                server_index = (server_index + 1) % len(avail_servers)
-                server_config = avail_servers[server_index]
-                client = await make_aio_client(qedata_thrift.TestService, server_config['host'],  server_config['port'],timeout=cls.request_timeout)
-            else:
-                return f'ERROR: {e}'
+         
         try:                
-            setTimeout(client, cls.request_timeout)
-            result = await client.login(username, password, get_mac_address(), __version__)
-            #print(result)
-            client.close()
-            if result.status:
-                cls._syssmtoken = result.msg
-                print(result.msg, cls._syssmtoken)
-                print('LOGIN SUCCEED')
-                return True
+            client = await cls.getClient()
+            if client:
+                setTimeout(client, cls.request_timeout)
+                result = await client.login(username, password, get_mac_address(), __version__)
+                #print(result)
+                client.close()
+                if result.status:
+                    cls._syssmtoken = result.msg
+                    print(result.msg, cls._syssmtoken)
+                    print('LOGIN SUCCEED')
+                    return True
+                else:
+                    print(f'LOGIN FAILED : {result.msg}')
+                    return False
             else:
-                print(f'LOGIN FAILED : {result.msg}')
-                return False
+                return False        
         except Exception as e:
             return f'ERROR: {e}'    
     
     @classmethod
     async def auth(cls, username, authcode):
-        global server_config, server_index,avail_servers
         try:
-            client = await make_aio_client(
-                qedata_thrift.TestService, server_config['host'],  server_config['port'],timeout=cls.request_timeout)
-        except Exception as e:
-            if len(avail_servers) > 1:
-                server_index = (server_index + 1) % len(avail_servers)
-                server_config = avail_servers[server_index]
-                client = await make_aio_client(qedata_thrift.TestService, server_config['host'],  server_config['port'],timeout=cls.request_timeout)
+            client = await cls.getClient()
+            if client:
+                setTimeout(client, cls.request_timeout)
+                result = await client.auth(username, authcode, False, get_mac_address(), __version__)
+                client.close()
+                if result.status:
+                    cls._systoken = result.msg
+                    print('AUTH SUCCEED')
+                    return True
+                else:
+                    print(f'AUTH FAILED : {result.msg}')
+                    return False
             else:
-                return f'ERROR: {e}'
-        try:                
-            setTimeout(client, cls.request_timeout)
-            result = await client.auth(username, authcode, False, get_mac_address(), __version__)
-            #print(result)
-            client.close()
-            if result.status:
-                cls._systoken = result.msg
-                print('AUTH SUCCEED')
-                return True
-            else:
-                print(f'AUTH FAILED : {result.msg}')
-                return False
+                return False        
         except Exception as e:
             return f'ERROR: {e}'                
                 
 
-            
     
 def auth(username, authcode):
     return asyncio.run(qedataClient.auth(username, authcode))
 
 def login(username, password):
     return asyncio.run(qedataClient.login(username, password))
 
 def check_auth():
     return qedataClient.check_auth()
     
     
 def testClient():
-    #loop.run_until_complete(qedataClient.instance().auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.'))
-    asyncio.run(qedataClient.instance().echo('test'))
+    #ret = loop.run_until_complete(qedataClient.instance().auth('quantease','$1$$k7yjPQKv8AJuZERDA.eQX.'))
+    #print(ret)
+    ret = asyncio.run(qedataClient.instance().echo('hello world'))
+    print(ret)
+
+
+if __name__ == '__main__':
+    testClient()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qesdk-0.1.7/src/qesdk/qedata.thrift` & `qesdk-0.1.8/src/qesdk/qedata.thrift`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.7/src/qesdk/utils.py` & `qesdk-0.1.8/src/qesdk/utils.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.7/src/qesdk.egg-info/PKG-INFO` & `qesdk-0.1.8/src/qesdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

