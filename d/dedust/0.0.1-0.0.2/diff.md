# Comparing `tmp/dedust-0.0.1.tar.gz` & `tmp/dedust-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedust-0.0.1.tar", last modified: Sat Apr 22 20:24:04 2023, max compression
+gzip compressed data, was "dedust-0.0.2.tar", last modified: Sun Jun 11 09:27:07 2023, max compression
```

## Comparing `dedust-0.0.1.tar` & `dedust-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       12 2023-04-20 20:45:31.325307 dedust-0.0.1/.gitignore
--rw-r--r--   0        0        0    11350 2023-04-20 20:08:32.030831 dedust-0.0.1/LICENSE.md
--rw-r--r--   0        0        0     1231 2023-04-20 20:46:01.933941 dedust-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-20 20:25:11.314002 dedust-0.0.1/dedust/__init__.py
--rw-r--r--   0        0        0      275 2023-04-20 20:28:32.619931 dedust-0.0.1/dedust/api.py
--rw-r--r--   0        0        0     1481 2023-04-20 20:04:32.179143 dedust-0.0.1/dedust/functions.py
--rw-r--r--   0        0        0      839 2023-04-20 20:42:47.325983 dedust-0.0.1/dedust/tokens.py
--rw-r--r--   0        0        0      485 2023-04-20 20:44:59.656497 dedust-0.0.1/examples/full.py
--rw-r--r--   0        0        0      339 2023-04-20 20:50:35.001726 dedust-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1483 1970-01-01 00:00:00.000000 dedust-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-04-20 20:45:31.325307 dedust-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11350 2023-04-20 20:08:32.030831 dedust-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1273 2023-06-11 09:26:44.160168 dedust-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 20:25:11.314002 dedust-0.0.2/dedust/__init__.py
+-rw-r--r--   0        0        0      275 2023-04-20 20:28:32.619931 dedust-0.0.2/dedust/api.py
+-rw-r--r--   0        0        0     1553 2023-06-11 09:24:19.451717 dedust-0.0.2/dedust/functions.py
+-rw-r--r--   0        0        0      998 2023-06-11 09:24:41.554230 dedust-0.0.2/dedust/tokens.py
+-rw-r--r--   0        0        0      547 2023-06-11 09:25:31.716914 dedust-0.0.2/examples/full.py
+-rw-r--r--   0        0        0      339 2023-06-11 09:26:36.570138 dedust-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 dedust-0.0.2/PKG-INFO
```

### Comparing `dedust-0.0.1/LICENSE.md` & `dedust-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dedust-0.0.1/README.md` & `dedust-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: dedust
+Version: 0.0.2
+Summary: DeDust - DeDust v2 API for Python.
+Author: Vlad100
+Description-Content-Type: text/markdown
+Requires-Dist: aiohttp
+Requires-Dist: flask
+Requires-Dist: tox ; extra == "dev"
+Provides-Extra: dev
+
 # DeDust API for Python
 
 Library for connecting DeDust API to Python apps.
 
 ## Description
 
 You can get token prices, volumes and liquidity.
@@ -11,16 +22,15 @@
 ### Dependencies
 
 * aiohttp
 
 ### Installing
 
 ```
-git clone https://github.com/ClickoTON-Foundation/dedust.git
-pip install -e dedust
+pip install dedust
 ```
 
 ### Using
 
 Example of getting data about token.
 
 ```python
@@ -33,14 +43,15 @@
 async def main():
     api = API()
     token = Token(api, TOKEN)
     
     print(f'$SCALE price: {await token.get_price()} TON')
     print(f'Volume: {(await token.get_volume())[0]} TON')
     print(f'Liquidity: {(await token.get_liquidity())[0]} TON')
+    print(f'$LP token: {await token.get_lp_token_address()}')
 
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
@@ -48,21 +59,24 @@
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
 * 0.0.1
     * Initial Beta
+* 0.0.2
+    * LP token address getting
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details
 
 ## Donate
 
-If you liked the library, I will be glad to donate.
+If you like the bot, I will be glad to accept donations.
 
 * TON: EQCgphx8rTI0PukwmgpVqiPgqguTujhQscg2h7jgc4U0t347
 
 ## Acknowledgments
 
 * [dedust-docs](https://api.dedust.io)
+
```

### Comparing `dedust-0.0.1/dedust/functions.py` & `dedust-0.0.2/dedust/functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,7 +42,10 @@
 async def get_volume(pool: dict, jetton_index: int) -> tuple[int, float]:
     ton_index = int(not jetton_index)
     
     raw_volume = pool['stats']['volume']
     volume = tuple(map(int, raw_volume))
     
     return volume[ton_index] / 10 ** 9, volume[jetton_index] / 10 ** 9
+
+async def get_lp_token_address(pool: dict):
+    return pool['address']
```

### Comparing `dedust-0.0.1/dedust/tokens.py` & `dedust-0.0.2/dedust/tokens.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .functions import get_reserves, get_liquidity, get_price, get_volume
+from .functions import get_reserves, get_liquidity, get_price, get_volume, get_lp_token_address
 from .api import API
 
 class Token():
     def __init__(self, api: API, address: str):
         self.api = api
         self.address = address
     
@@ -23,7 +23,12 @@
         
         return await get_price(await self.get_liquidity())
     
     async def get_volume(self):
         await self.update()
         
         return await get_volume(self.pool, self.index)
+    
+    async def get_lp_token_address(self):
+        await self.update()
+        
+        return await get_lp_token_address(self.pool)
```

### Comparing `dedust-0.0.1/PKG-INFO` & `dedust-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: dedust
-Version: 0.0.1
-Summary: DeDust - DeDust v2 API for Python.
-Author: Vlad100
-Description-Content-Type: text/markdown
-Requires-Dist: aiohttp
-Requires-Dist: flask
-Requires-Dist: tox ; extra == "dev"
-Provides-Extra: dev
-
 # DeDust API for Python
 
 Library for connecting DeDust API to Python apps.
 
 ## Description
 
 You can get token prices, volumes and liquidity.
@@ -22,16 +11,15 @@
 ### Dependencies
 
 * aiohttp
 
 ### Installing
 
 ```
-git clone https://github.com/ClickoTON-Foundation/dedust.git
-pip install -e dedust
+pip install dedust
 ```
 
 ### Using
 
 Example of getting data about token.
 
 ```python
@@ -44,14 +32,15 @@
 async def main():
     api = API()
     token = Token(api, TOKEN)
     
     print(f'$SCALE price: {await token.get_price()} TON')
     print(f'Volume: {(await token.get_volume())[0]} TON')
     print(f'Liquidity: {(await token.get_liquidity())[0]} TON')
+    print(f'$LP token: {await token.get_lp_token_address()}')
 
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
@@ -59,22 +48,23 @@
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
 * 0.0.1
     * Initial Beta
+* 0.0.2
+    * LP token address getting
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details
 
 ## Donate
 
-If you liked the library, I will be glad to donate.
+If you like the bot, I will be glad to accept donations.
 
 * TON: EQCgphx8rTI0PukwmgpVqiPgqguTujhQscg2h7jgc4U0t347
 
 ## Acknowledgments
 
 * [dedust-docs](https://api.dedust.io)
-
```

