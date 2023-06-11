# Comparing `tmp/dexie_rewards-1.8.1b1.tar.gz` & `tmp/dexie_rewards-1.8.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-1.8.1b1.tar", max compression
+gzip compressed data, was "dexie_rewards-1.8.1b2.tar", max compression
```

## Comparing `dexie_rewards-1.8.1b1.tar` & `dexie_rewards-1.8.1b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-1.8.1b1/LICENSE
--rw-r--r--   0        0        0     5641 2023-05-26 14:42:14.551472 dexie_rewards-1.8.1b1/README.md
--rw-r--r--   0        0        0      800 2023-06-10 08:57:34.470245 dexie_rewards-1.8.1b1/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-1.8.1b1/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1125 2023-06-10 08:56:40.442539 dexie_rewards-1.8.1b1/src/dexie_rewards/config.py
--rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-1.8.1b1/src/dexie_rewards/decorators/with_db_connection.py
--rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.443038 dexie_rewards-1.8.1b1/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-1.8.1b1/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     4557 2023-06-10 08:56:40.443604 dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     5122 2023-06-10 08:56:40.444110 dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.341294 dexie_rewards-1.8.1b1/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-1.8.1b1/src/dexie_rewards/services/dexie_db.py
--rw-r--r--   0        0        0     1759 2023-05-26 14:42:14.553106 dexie_rewards-1.8.1b1/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0      801 2023-05-16 00:41:08.479451 dexie_rewards-1.8.1b1/src/dexie_rewards/types/offer_reward.py
--rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-1.8.1b1/src/dexie_rewards/types/utils.py
--rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.444913 dexie_rewards-1.8.1b1/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0     6472 1970-01-01 00:00:00.000000 dexie_rewards-1.8.1b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 14:18:44.184005 dexie_rewards-1.8.1b2/LICENSE
+-rw-r--r--   0        0        0     5716 2023-06-11 05:14:21.000000 dexie_rewards-1.8.1b2/README.md
+-rw-r--r--   0        0        0      800 2023-06-11 05:36:33.383744 dexie_rewards-1.8.1b2/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-10 08:56:40.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:18:23.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-08 10:51:08.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     4557 2023-06-10 08:56:40.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-08 10:18:31.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     5043 2023-06-11 05:27:12.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1792 2023-06-11 05:27:12.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0      801 2023-05-16 00:41:08.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-09 11:06:14.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0     6547 1970-01-01 00:00:00.000000 dexie_rewards-1.8.1b2/PKG-INFO
```

### Comparing `dexie_rewards-1.8.1b1/LICENSE` & `dexie_rewards-1.8.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/README.md` & `dexie_rewards-1.8.1b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 ```
 ❯ dexie rewards claim
 
   --fingerprint  -f         Set the fingerprint to specify which wallet to use
   --verify-only  -vo        Only verify the claim, don't actually claim
   --yes          -y         Skip claim confirmation
   --verbose      -v         Display verbose output
+  --target       -t         Specify a target address to claim rewards to 
   --help                    Show help and exit
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, follow these steps to help identify and resolve them:
 
@@ -115,8 +116,8 @@
 
 ## Alternatives
 
 Advanced market makers may develop their own tools for claiming liquidity rewards. Refer to the [dexie API documentation](https://dexie.space/api) for information on how to claim rewards for offers using the API.
 
 ## Contributions
 
-Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
+Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
```

### Comparing `dexie_rewards-1.8.1b1/pyproject.toml` & `dexie_rewards-1.8.1b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "1.8.1-b1"
+version = "1.8.1-b2"
 description = "dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/config.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/config.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/decorators/with_db_connection.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/decorators/with_db_connection.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/claim.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/list.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/list.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,15 @@
 
 async def create_claims(
     offers_rewards: List[OfferReward], target_puzzle_hash: Optional[bytes32]
 ) -> List[Any]:
     timestamp = int(time.time())
     claims = []
     for offer_reward in offers_rewards:
-        (
-            public_key,
-            signature,
-            signing_mode,
-        ) = await sign_claim(
+        (public_key, signature, signing_mode,) = await sign_claim(
             offer_reward.offer_id,
             timestamp,
             offer_reward.maker_puzzle_hash,
             target_puzzle_hash,
         )
 
         # return offer hash, signature, pk, and puzzle hash
@@ -98,15 +94,14 @@
 async def sign_claim(
     offer_id: str,
     timestamp: int,
     maker_puzzle_hash: bytes32,
     target_puzzle_hash: Optional[bytes32],
 ) -> Tuple[str, str, str]:
     message = (
-        # TODO: removed in 2.0.0
         f"Claim dexie liquidity rewards for offer {offer_id} ({timestamp})"
         if target_puzzle_hash is None
         else f"Claim dexie liquidity rewards for offer {offer_id} to {target_puzzle_hash} ({timestamp})"
     )
     return await wallet_rpc_client.sign_message_by_puzzle_hash(
         maker_puzzle_hash, message
     )
```

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/services/dexie_api.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/services/dexie_db.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/services/dexie_db.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 async def get_synced(wallet_rpc_client: WalletRpcClient) -> bool:
     return await wallet_rpc_client.get_synced()
 
 
 @with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
 async def get_all_offers(wallet_rpc_client: WalletRpcClient) -> List[TradeRecord]:
     return await wallet_rpc_client.get_all_offers(
-        include_completed=True, exclude_taken_offers=True, file_contents=True, start=0, end=1000
+        include_completed=True,
+        exclude_taken_offers=True,
+        file_contents=True,
+        start=0,
+        end=1000,
     )
 
 
 @with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
 async def sign_message_by_puzzle_hash(
     wallet_rpc_client: WalletRpcClient, puzzle_hash: bytes32, message: str
 ) -> Tuple[str, str, str]:
```

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/types/offer_reward.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/types/offer_reward.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/src/dexie_rewards/utils.py` & `dexie_rewards-1.8.1b2/src/dexie_rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b1/PKG-INFO` & `dexie_rewards-1.8.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 1.8.1b1
+Version: 1.8.1b2
 Summary: dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -108,14 +108,15 @@
 ```
 ❯ dexie rewards claim
 
   --fingerprint  -f         Set the fingerprint to specify which wallet to use
   --verify-only  -vo        Only verify the claim, don't actually claim
   --yes          -y         Skip claim confirmation
   --verbose      -v         Display verbose output
+  --target       -t         Specify a target address to claim rewards to 
   --help                    Show help and exit
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, follow these steps to help identify and resolve them:
 
@@ -136,7 +137,8 @@
 ## Alternatives
 
 Advanced market makers may develop their own tools for claiming liquidity rewards. Refer to the [dexie API documentation](https://dexie.space/api) for information on how to claim rewards for offers using the API.
 
 ## Contributions
 
 Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
+
```

