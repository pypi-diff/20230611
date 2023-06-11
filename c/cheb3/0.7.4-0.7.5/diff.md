# Comparing `tmp/cheb3-0.7.4.tar.gz` & `tmp/cheb3-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheb3-0.7.4.tar", last modified: Thu Jun  8 04:03:37 2023, max compression
+gzip compressed data, was "cheb3-0.7.5.tar", last modified: Sun Jun 11 04:38:53 2023, max compression
```

## Comparing `cheb3-0.7.4.tar` & `cheb3-0.7.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:03:37.438230 cheb3-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-08 04:03:28.000000 cheb3-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-08 04:03:37.438230 cheb3-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-08 04:03:28.000000 cheb3-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:03:37.438230 cheb3-0.7.4/cheb3/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:03:37.438230 cheb3-0.7.4/cheb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 04:03:28.000000 cheb3-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 04:03:37.438230 cheb3-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:38:53.967335 cheb3-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-11 04:38:44.000000 cheb3-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-11 04:38:53.967335 cheb3-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-11 04:38:44.000000 cheb3-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:38:53.967335 cheb3-0.7.5/cheb3/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-11 04:38:44.000000 cheb3-0.7.5/cheb3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:38:53.967335 cheb3-0.7.5/cheb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 04:38:53.000000 cheb3-0.7.5/cheb3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-11 04:38:44.000000 cheb3-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:38:53.967335 cheb3-0.7.5/setup.cfg
```

### Comparing `cheb3-0.7.4/LICENSE` & `cheb3-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.4/PKG-INFO` & `cheb3-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.7.4
+Version: 0.7.5
 Summary: Web3 CTF tool based on web3.py
 Author-email: YanhuiJessica <y4nhv1@gmail.com>
 Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/YanhuiJessica/cheb3
 Project-URL: Bug Reports, https://github.com/YanhuiJessica/cheb3/issues
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cheb3 Version: 0.7.4 Summary: Web3 CTF tool based
+Metadata-Version: 2.1 Name: cheb3 Version: 0.7.5 Summary: Web3 CTF tool based
 on web3.py Author-email: YanhuiJessica
 gmail.com> Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/ Project-
 URL: Source, https://github.com/YanhuiJessica/cheb3 Project-URL: Bug Reports,
 https://github.com/YanhuiJessica/cheb3/issues Classifier: Development Status ::
 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `cheb3-0.7.4/README.md` & `cheb3-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.4/cheb3/account.py` & `cheb3-0.7.5/cheb3/account.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.4/cheb3/connection.py` & `cheb3-0.7.5/cheb3/connection.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.4/cheb3/contract.py` & `cheb3-0.7.5/cheb3/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from web3._utils.datatypes import PropertyCheckingFactory
 from web3._utils.abi import (
     filter_by_type,
     fallback_func_abi_exists,
     receive_func_abi_exists,
 )
 from web3._utils.function_identifiers import FallbackFn, ReceiveFn
+from web3.exceptions import ContractLogicError
 from web3.types import ABI, TxReceipt
 from eth_typing import ChecksumAddress
 import eth_account
 
 from cheb3.account import Account
 from cheb3.constants import GAS_BUFFER
 
@@ -214,20 +215,24 @@
 class ContractFunctionWrapper(ContractFunction):
     signer: eth_account.Account = None
 
     def send_transaction(self, **kwargs) -> TxReceipt:
         if not self.signer:
             raise AttributeError("The `signer` is missing.")
 
+        try:
+            estimate_gas = self.estimate_gas() + GAS_BUFFER
+        except ContractLogicError:
+            estimate_gas = 3000000
         tx = {
             "chainId": self.w3.eth.chain_id,
             "nonce": self.w3.eth.get_transaction_count(self.signer.address),
             "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
             "value": kwargs.get("value", 0),
-            "gas": kwargs.get("gas_limit", self.estimate_gas() + GAS_BUFFER),
+            "gas": kwargs.get("gas_limit", estimate_gas),
         }
         tx = self.signer.sign_transaction(self.build_transaction(tx)).rawTransaction
         tx_hash = self.w3.eth.send_raw_transaction(tx).hex()
         func_name = self.function_identifier if isinstance(self.function_identifier, str) else self.function_identifier.__name__
         logger.info(f"({self.address}).{func_name} transaction hash: {tx_hash}")
         receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         if not receipt.status:
```

### Comparing `cheb3-0.7.4/cheb3/utils.py` & `cheb3-0.7.5/cheb3/utils.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.4/cheb3.egg-info/PKG-INFO` & `cheb3-0.7.5/cheb3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.7.4
+Version: 0.7.5
 Summary: Web3 CTF tool based on web3.py
 Author-email: YanhuiJessica <y4nhv1@gmail.com>
 Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/YanhuiJessica/cheb3
 Project-URL: Bug Reports, https://github.com/YanhuiJessica/cheb3/issues
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cheb3 Version: 0.7.4 Summary: Web3 CTF tool based
+Metadata-Version: 2.1 Name: cheb3 Version: 0.7.5 Summary: Web3 CTF tool based
 on web3.py Author-email: YanhuiJessica
 gmail.com> Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/ Project-
 URL: Source, https://github.com/YanhuiJessica/cheb3 Project-URL: Bug Reports,
 https://github.com/YanhuiJessica/cheb3/issues Classifier: Development Status ::
 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `cheb3-0.7.4/pyproject.toml` & `cheb3-0.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cheb3"
-version = "0.7.4"
+version = "0.7.5"
 authors = [{name = "YanhuiJessica",email = "y4nhv1@gmail.com"}]
 description = "Web3 CTF tool based on web3.py"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "web3>=6.0.0",
   "py-solc-x",
```

