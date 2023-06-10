# Comparing `tmp/carter_py-0.2.0-py3-none-any.whl.zip` & `tmp/carter_py-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8094 bytes, number of entries: 10
+Zip file size: 8152 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-15 11:17 carterpy/__init__.py
--rw-rw-rw-  2.0 fat     3196 b- defN 23-Apr-28 23:27 carterpy/async_carter.py
--rw-rw-rw-  2.0 fat     3110 b- defN 23-Apr-28 23:27 carterpy/carter.py
--rw-rw-rw-  2.0 fat     2767 b- defN 23-Apr-16 20:48 carterpy/classes.py
--rw-rw-rw-  2.0 fat      455 b- defN 23-Apr-12 20:13 carterpy/utils.py
--rw-rw-rw-  2.0 fat     8758 b- defN 23-Apr-28 23:32 carter_py-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 23:32 carter_py-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1075 b- defN 23-Apr-28 23:32 carter_py-0.2.0.dist-info/license.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-28 23:32 carter_py-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      779 b- defN 23-Apr-28 23:32 carter_py-0.2.0.dist-info/RECORD
-10 files, 20308 bytes uncompressed, 6770 bytes compressed:  66.7%
+-rw-rw-rw-  2.0 fat     3249 b- defN 23-Jun-10 19:44 carterpy/async_carter.py
+-rw-rw-rw-  2.0 fat     3161 b- defN 23-Jun-10 19:48 carterpy/carter.py
+-rw-rw-rw-  2.0 fat     2763 b- defN 23-Jun-10 19:49 carterpy/classes.py
+-rw-rw-rw-  2.0 fat      481 b- defN 23-Jun-10 19:50 carterpy/utils.py
+-rw-rw-rw-  2.0 fat     8818 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1075 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/license.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      779 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/RECORD
+10 files, 20494 bytes uncompressed, 6828 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: carterpy/classes.py
 Comment: 
 
 Filename: carterpy/utils.py
 Comment: 
 
-Filename: carter_py-0.2.0.dist-info/METADATA
+Filename: carter_py-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: carter_py-0.2.0.dist-info/WHEEL
+Filename: carter_py-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: carter_py-0.2.0.dist-info/license.txt
+Filename: carter_py-1.0.0.dist-info/license.txt
 Comment: 
 
-Filename: carter_py-0.2.0.dist-info/top_level.txt
+Filename: carter_py-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: carter_py-0.2.0.dist-info/RECORD
+Filename: carter_py-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## carterpy/async_carter.py

```diff
@@ -20,64 +20,66 @@
 
 class AsyncCarter:
     def __init__(self, api_key, speak=False):
         self.api_key = api_key
         self.history = []
         self.speak_default = speak
 
-    async def say(self, text, player_id, speak=None):
+    async def say(self, text, user_id, speak=None):
         text = convert_to_string("text", text)
-        player_id = convert_to_string("player_id", player_id)
+        user_id = convert_to_string("user_id", user_id)
         start = time.perf_counter()
         speak_now = speak if speak is not None else self.speak_default
         data = {
             "text": text,
-            "playerId": player_id,
+            "playerId": user_id,
             "key": self.api_key,
             "speak": speak_now
         }
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
         }
         response_data = await asyncRequest(URLS["say"], data, headersList)
         time_taken = int((time.perf_counter() - start) * 1000)
         interaction = Interaction("say", data, response_data, time_taken)
         if interaction.ok:
             self.history.insert(0, interaction)
         return interaction
 
-    async def opener(self, player_id, speak=None):
-        player_id = convert_to_string("player_id", player_id)
+    async def opener(self, user_id, speak=None):
+        user_id = convert_to_string("user_id", user_id)
         start = time.perf_counter()
         speak_now = speak if speak is not None else self.speak_default
         data = {
-            "playerId": player_id,
+            "playerId": user_id,
             "key": self.api_key,
-            "speak": speak_now
+            "speak": speak_now,
+            "personal": True
         }
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
         }
         response = await asyncRequest(URLS["opener"], data, headersList)
         time_taken = int((time.perf_counter() - start) * 1000)
         interaction = Interaction("opener", data, response, time_taken)
         if interaction.ok:
             self.history.insert(0, interaction)
         return interaction
 
-    async def personalise(self, text, speak=None):
+    async def personalise(self, text, user_id, speak=None):
         text = convert_to_string("text", text)
         start = time.perf_counter()
         speak_now = speak if speak is not None else self.speak_default
         data = {
             "text": text,
             "key": self.api_key,
-            "speak": speak_now
+            "speak": speak_now,
+            "user_id": user_id
         }
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
         }
         response = await asyncRequest(URLS["personalise"], data, headersList)
         time_taken = int((time.perf_counter() - start) * 1000)
```

## carterpy/carter.py

```diff
@@ -17,22 +17,22 @@
 
 class Carter:
     def __init__(self, api_key, speak=False):
         self.api_key = api_key
         self.history = []
         self.speak_default = speak
 
-    def say(self, text, player_id, speak=None):
+    def say(self, text, user_id, speak=None):
         text = convert_to_string("text", text)
-        player_id = convert_to_string("player_id", player_id)
+        user_id = convert_to_string("user_id", user_id)
         start = time.perf_counter()
         speak_now = speak if speak is not None else self.speak_default
         data = {
             "text": text,
-            "playerId": player_id,
+            "user_id": user_id,
             "key": self.api_key,
             "speak": speak_now
         }
 
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
@@ -41,43 +41,45 @@
         response_data = carterRequest(URLS["say"], data, headers=headersList)
         time_taken = int((time.perf_counter() - start) * 1000)
         interaction = Interaction("say", data, response_data, time_taken)
         if interaction.ok:
             self.history.insert(0, interaction)
         return interaction
 
-    def opener(self, player_id, speak=None):
-        player_id = convert_to_string("player_id", player_id)
+    def opener(self, user_id, speak=None):
+        user_id = convert_to_string("user_id", user_id)
         start = time.perf_counter()
         speak_now = speak if speak is not None else self.speak_default
         data = {
-            "playerId": player_id,
+            "user_id": user_id,
             "key": self.api_key,
-            "speak": speak_now
+            "speak": speak_now,
+            "personal": True
         }
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
         }
         response = carterRequest(
             URLS["opener"], headers=headersList, data=data)
         time_taken = int((time.perf_counter() - start) * 1000)
         interaction = Interaction("opener", data, response, time_taken)
         if interaction.ok:
             self.history.insert(0, interaction)
         return interaction
 
-    def personalise(self, text, speak=None):
+    def personalise(self, text, user_id, speak=None):
         text = convert_to_string("text", text)
         start = time.perf_counter()
         speak_now = speak if speak is not None else self.speak_default
         data = {
             "text": text,
             "key": self.api_key,
-            "speak": speak_now
+            "speak": speak_now,
+            "user_id": user_id
         }
         headersList = {
             "Accept": "*/*",
             "Content-Type": "application/json"
         }
         response = carterRequest(
             URLS["personalise"], headers=headersList, data=data)
```

## carterpy/classes.py

```diff
@@ -49,15 +49,15 @@
             self.status_code = None
             self.status_message = None
             self.output_text = None
             self.forced_behaviours = None
 
         # Payload data
         self.input_text = self.payload.get("text", self.type)
-        self.player_id = self.payload.get("player_id")
+        self.user_id = self.payload.get("user_id")
 
 
     def __str__(self):
         if self.ok:
             return f"<{self.type.capitalize()} interaction {self.id} - {self.input_text} -> {self.output_text}>"
         else:
             return f"<{self.type.capitalize()} interaction {self.id} - Failed with status code {self.status_code} and message {self.status_message}>"
```

## carterpy/utils.py

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 URLS = {
-    "say": "https://api.carterlabs.ai/chat",
-    "opener": "https://api.carterlabs.ai/opener",
-    "personalise": "https://api.carterlabs.ai/personalise",
+    "say": "https://unstable.carterlabs.ai/api/say",
+    "opener": "https://unstable.carterlabs.ai/api/opener",
+    "personalise": "https://unstable.carterlabs.ai/api/personalise",
 }
 
 def convert_to_string(variable_name, value):
     try:
         return str(value)
     except:
         raise TypeError(f"{variable_name} must be convertible to a string, received {type(value)}")
```

## Comparing `carter_py-0.2.0.dist-info/METADATA` & `carter_py-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carter-py
-Version: 0.2.0
+Version: 1.0.0
 Summary: A wrapper for the Carter API
 Home-page: https://github.com/LazyLyrics/carter-py
 Author: LazyLyrics
 Author-email: lazylyrics@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: Requests (==2.28.2)
 Requires-Dist: responses (==0.23.1)
 Requires-Dist: setuptools (==65.5.0)
 
 # carter-py: A Python Wrapper for the Carter API
 
-[GitHub](https://github.com/LazyLyrics/carter-py) | [PyPI](https://pypi.org/project/carter-py/) | [Change Log](https://github.com/LazyLyrics/carter-py/blob/main/CHANGELOG.md)
+[GitHub](https://github.com/LazyLyrics/carter-py) | [PyPI](https://pypi.org/project/carter-py/) | [Change Log](https://github.com/LazyLyrics/carter-py/blob/main/CHANGELOG.md)| [Docs](https://lazylyrics.gitbook.io/carter-py/)
 
 `carter-py` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
 
 Please note that this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). As carter-py is built around an API which is still in beta, breaking changes may be introduced indirectly in minor releases. Major releases will be reserved for breaking changes to the way in carter-py is used. IE. function names, parameter depreciations etc. Where a breaking change is made on the API side, carter-py will be updated to reflect this change.
 
 I will continue to build carter-py with the intention of maintaining backwards compatibility, but this is not guaranteed. Previous versions of carter-py are always likely to be outdated as the API progresses. Please consult the changelog for any breaking changes and try to use the latest version of carter-py.
 
@@ -164,15 +164,15 @@
 # Replace YOUR_API_KEY with your actual API key
 api_key = "YOUR_API_KEY"
 
 async def main():
     async_carter = AsyncCarter(api_key)
 
     # with carter object already created
-    interaction = await async_carter.opener("player123")
+    interaction = await async_carter.say("hi there!", "player123")
     personalise = await async_carter.personalise("Hello, world!")
     opener = await async_carter.opener("player123")
     print(interaction.output_text)
 
 asyncio.run(main())
 ```
```

## Comparing `carter_py-0.2.0.dist-info/license.txt` & `carter_py-1.0.0.dist-info/license.txt`

 * *Files identical despite different names*

## Comparing `carter_py-0.2.0.dist-info/RECORD` & `carter_py-1.0.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 carterpy/__init__.py,sha256=SWOh6maoMonoFWKkqj5S42uK47hk7OgGgWjymXeXuZ4,67
-carterpy/async_carter.py,sha256=9WR-ZiveRX7XFQC0HKg2nXpX8nKmmejhiG0l-gNwo40,3196
-carterpy/carter.py,sha256=-pltPb83auq24Fsm_bVI_CWiPqP3zYbPP8jUEM4QD0U,3110
-carterpy/classes.py,sha256=50KuVZWGwUX4xfZQ2WRauv4SJ73MO7DVmtCI6uVWhXI,2767
-carterpy/utils.py,sha256=0CplsSq1LFJfVsrjv09FtSgHvBxhiAP0Q0xeLUH5eok,455
-carter_py-0.2.0.dist-info/METADATA,sha256=hu1uvu81uFZULqoq0_3D3tdtAs2z4qc5nxPgqEiVSQM,8758
-carter_py-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-carter_py-0.2.0.dist-info/license.txt,sha256=ufmiTBS0Q6R8mZXaRjKpnIqT9NafpZYq9DoCZ_oGYBA,1075
-carter_py-0.2.0.dist-info/top_level.txt,sha256=l8aBC3U-dSDPJ4ZDLx8cpzscw9PFaB7vu3pA5WhXa4I,9
-carter_py-0.2.0.dist-info/RECORD,,
+carterpy/async_carter.py,sha256=dYBI0cTpz9iEybofgJ4eeE-qZ6dcB0U5aB5YhzEF9rs,3249
+carterpy/carter.py,sha256=RQE1kLH3J6dJHf4z7acoaSpV3MoekSehVFDoIMt_xlc,3161
+carterpy/classes.py,sha256=pICxet4VQ8tqEQE8ZukpTdi9tS193pXySAJHgU1Adp8,2763
+carterpy/utils.py,sha256=Ff6AzmCPIrvDHGF887ms1Zb6Jm69Sg3KjXzsMt8RNQ0,481
+carter_py-1.0.0.dist-info/METADATA,sha256=MPbWApEU_6H0UbxR1H_oesfiuVfhzSLzxvtId0-00vg,8818
+carter_py-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+carter_py-1.0.0.dist-info/license.txt,sha256=ufmiTBS0Q6R8mZXaRjKpnIqT9NafpZYq9DoCZ_oGYBA,1075
+carter_py-1.0.0.dist-info/top_level.txt,sha256=l8aBC3U-dSDPJ4ZDLx8cpzscw9PFaB7vu3pA5WhXa4I,9
+carter_py-1.0.0.dist-info/RECORD,,
```

