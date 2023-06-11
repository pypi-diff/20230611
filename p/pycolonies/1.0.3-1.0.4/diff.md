# Comparing `tmp/pycolonies-1.0.3-py3-none-any.whl.zip` & `tmp/pycolonies-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9681 bytes, number of entries: 7
+Zip file size: 9709 bytes, number of entries: 7
 -rw-r--r--  2.0 unx     1116 b- defN 23-Mar-07 18:41 crypto.py
--rw-r--r--  2.0 unx    10787 b- defN 23-Jun-11 11:28 pycolonies.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jun-11 11:32 pycolonies-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    18159 b- defN 23-Jun-11 11:32 pycolonies-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 11:32 pycolonies-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-11 11:32 pycolonies-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      539 b- defN 23-Jun-11 11:32 pycolonies-1.0.3.dist-info/RECORD
-7 files, 31776 bytes uncompressed, 8735 bytes compressed:  72.5%
+-rw-r--r--  2.0 unx    10986 b- defN 23-Jun-11 19:51 pycolonies.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18159 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      539 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/RECORD
+7 files, 31975 bytes uncompressed, 8763 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: crypto.py
 Comment: 
 
 Filename: pycolonies.py
 Comment: 
 
-Filename: pycolonies-1.0.3.dist-info/LICENSE
+Filename: pycolonies-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: pycolonies-1.0.3.dist-info/METADATA
+Filename: pycolonies-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pycolonies-1.0.3.dist-info/WHEEL
+Filename: pycolonies-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pycolonies-1.0.3.dist-info/top_level.txt
+Filename: pycolonies-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pycolonies-1.0.3.dist-info/RECORD
+Filename: pycolonies-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycolonies.py

```diff
@@ -9,15 +9,15 @@
 
 class ColoniesConnectionError(Exception):
     pass
 
 class ColoniesError(Exception):
     pass
     
-def func_spec(func, args, colonyid, executortype, priority, maxexectime, maxretries, maxwaittime, code=None):
+def func_spec(func, args, colonyid, executortype, priority=1, maxexectime=-1, maxretries=-1, maxwaittime=-1, code=None):
     if isinstance(func, str):
         func_spec = {
             "nodename": func,
             "funcname": func, 
             "args": args,
             "priority": priority,
             "maxwaittime": maxwaittime,
@@ -89,33 +89,35 @@
     FAILED = 3
     
     def __init__(self, host, port, tls=False):
         if tls:
             self.url = "https://" + host + ":" + str(port) + "/api"
             self.host = host
             self.port = port
+            self.tls = False
         else:
             self.url = "http://" + host + ":" + str(port) + "/api"
             self.host = host
             self.port = port
+            self.tls = True 
     
     def __rpc(self, msg, prvkey):
         payload = str(base64.b64encode(json.dumps(msg).encode('utf-8')), "utf-8")
         crypto = Crypto()
         signature = crypto.sign(payload, prvkey)
 
         rpc = {
             "payloadtype" : msg["msgtype"],
             "payload" : payload,
             "signature" : signature
         }
 
         rpc_json = json.dumps(rpc) 
         try:
-            reply = requests.post(url = self.url, data=rpc_json, verify=False)
+            reply = requests.post(url = self.url, data=rpc_json, verify=True)
             reply_msg_json = json.loads(reply.content)
             base64_payload = reply_msg_json["payload"]
             payload_bytes = base64.b64decode(base64_payload)
             payload = json.loads(payload_bytes)
         except requests.exceptions.ConnectionError as err:
             raise ColoniesConnectionError(err)
         except Exception as err:
@@ -144,15 +146,18 @@
             "signature": ""
         }
 
         rpcmsg["payload"] = str(base64.b64encode(json.dumps(msg).encode('utf-8')), "utf-8")
         crypto = Crypto()
         rpcmsg["signature"] = crypto.sign(rpcmsg["payload"], prvkey) 
 
-        ws = create_connection("ws://" + self.host + ":" + str(self.port) + "/pubsub")
+        if self.tls:
+            ws = create_connection("ws://" + self.host + ":" + str(self.port) + "/pubsub")
+        else:
+            ws = create_connection("wss://" + self.host + ":" + str(self.port) + "/pubsub")
         ws.send(json.dumps(rpcmsg))
         ws.recv()
         ws.close()
 
         return self.get_process(process["processid"], prvkey)
 
     def add_colony(self, colony, prvkey):
```

## Comparing `pycolonies-1.0.3.dist-info/LICENSE` & `pycolonies-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycolonies-1.0.3.dist-info/METADATA` & `pycolonies-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolonies
-Version: 1.0.3
+Version: 1.0.4
 Summary: Colonies Python SDK
 Home-page: https://github.com/colonyos/pycolonies
 Author: Johan Kristiansson
 Author-email: johan.kristiansson@ri.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

