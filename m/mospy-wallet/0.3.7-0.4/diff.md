# Comparing `tmp/mospy_wallet-0.3.7.tar.gz` & `tmp/mospy_wallet-0.4.tar.gz`

## Comparing `mospy_wallet-0.3.7.tar` & `mospy_wallet-0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/mkdocs.yml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/requirements.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/setup.cfg
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/.github/workflows/tests.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/CNAME
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/account.md
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/examples.md
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/index.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/transaction.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/clients/grpcclient.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/clients/httpclient.md
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/clients/index.md
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/docs/transaction/types.md
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/examples/builtin_staking.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/examples/delegate.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/examples/evmos_transfer.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/examples/ibc_transfer.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/examples/osmosis_trade.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/examples/set_withdraw_address.py
--rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/Account.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/Transaction.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/__init__.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/utils.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/_transactions/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/_transactions/_delegate.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/_transactions/_transfer.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/_transactions/_undelegate.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/_transactions/_withdraw_reward.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/clients/GRPCClient.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/clients/HTTPClient.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/clients/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/src/mospy/exceptions/clients.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/tests/test_account.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/tests/test_eth.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/tests/test_transaction.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/tests/clients/test_grpcclient.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/tests/clients/test_httpclient.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/.gitignore
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 mospy_wallet-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 mospy_wallet-0.4/mkdocs.yml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 mospy_wallet-0.4/requirements.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mospy_wallet-0.4/setup.cfg
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mospy_wallet-0.4/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/CNAME
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/account.md
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/examples.md
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/index.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/transaction.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/clients/grpcclient.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/clients/httpclient.md
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/clients/index.md
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 mospy_wallet-0.4/docs/transaction/types.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mospy_wallet-0.4/examples/builtin_staking.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mospy_wallet-0.4/examples/delegate.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 mospy_wallet-0.4/examples/evmos_transfer.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 mospy_wallet-0.4/examples/ibc_transfer.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mospy_wallet-0.4/examples/osmosis_trade.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mospy_wallet-0.4/examples/set_withdraw_address.py
+-rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/Account.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/Transaction.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/utils.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/_transactions/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/_transactions/_delegate.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/_transactions/_transfer.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/_transactions/_undelegate.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/_transactions/_withdraw_reward.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/clients/GRPCClient.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/clients/HTTPClient.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/clients/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mospy_wallet-0.4/src/mospy/exceptions/clients.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 mospy_wallet-0.4/tests/test_account.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 mospy_wallet-0.4/tests/test_eth.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 mospy_wallet-0.4/tests/test_transaction.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mospy_wallet-0.4/tests/clients/test_grpcclient.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 mospy_wallet-0.4/tests/clients/test_httpclient.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mospy_wallet-0.4/.gitignore
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 mospy_wallet-0.4/README.md
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 mospy_wallet-0.4/pyproject.toml
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 mospy_wallet-0.4/PKG-INFO
```

### Comparing `mospy_wallet-0.3.7/.github/workflows/tests.yaml` & `mospy_wallet-0.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/docs/examples.md` & `mospy_wallet-0.4/docs/examples.md`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/docs/index.md` & `mospy_wallet-0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/docs/transaction/types.md` & `mospy_wallet-0.4/docs/transaction/types.md`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/examples/builtin_staking.py` & `mospy_wallet-0.4/examples/builtin_staking.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/examples/delegate.py` & `mospy_wallet-0.4/examples/delegate.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/examples/evmos_transfer.py` & `mospy_wallet-0.4/examples/evmos_transfer.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/examples/ibc_transfer.py` & `mospy_wallet-0.4/examples/ibc_transfer.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/examples/osmosis_trade.py` & `mospy_wallet-0.4/examples/osmosis_trade.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/examples/set_withdraw_address.py` & `mospy_wallet-0.4/examples/set_withdraw_address.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/src/mospy/Account.py` & `mospy_wallet-0.4/src/mospy/Account.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/src/mospy/Transaction.py` & `mospy_wallet-0.4/src/mospy/Transaction.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/src/mospy/utils.py` & `mospy_wallet-0.4/src/mospy/utils.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/src/mospy/_transactions/_delegate.py` & `mospy_wallet-0.4/src/mospy/_transactions/_delegate.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/src/mospy/_transactions/_transfer.py` & `mospy_wallet-0.4/src/mospy/_transactions/_transfer.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/src/mospy/_transactions/_undelegate.py` & `mospy_wallet-0.4/src/mospy/_transactions/_undelegate.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/src/mospy/_transactions/_withdraw_reward.py` & `mospy_wallet-0.4/src/mospy/_transactions/_withdraw_reward.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/src/mospy/clients/GRPCClient.py` & `mospy_wallet-0.4/src/mospy/clients/GRPCClient.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,23 +33,27 @@
             "osmosis": "osmosis_protobuf",
             "evmos": "evmos_protobuf",
         }
         _protobuf_package = (_protobuf_packages[protobuf.lower()]
                              if protobuf.lower() in _protobuf_packages.keys()
                              else protobuf)
         try:
-            self.BroadcastTxRequest = importlib.import_module(
+            self._cosmos_tx_service_pb2 = importlib.import_module(
                 _protobuf_package +
-                ".cosmos.tx.v1beta1.service_pb2").BroadcastTxRequest
-            self.query_pb2 = importlib.import_module(
+                ".cosmos.tx.v1beta1.service_pb2")
+            self._cosmos_auth_query_pb2 = importlib.import_module(
                 _protobuf_package + ".cosmos.auth.v1beta1.query_pb2")
-            self.query_pb2_grpc = importlib.import_module(
+            self._cosmos_auth_query_pb2_grpc = importlib.import_module(
                 _protobuf_package + ".cosmos.auth.v1beta1.query_pb2_grpc")
-            self.service_pb2_grpc = importlib.import_module(
+            self._cosmos_tx_service_pb2_grpc = importlib.import_module(
                 _protobuf_package + ".cosmos.tx.v1beta1.service_pb2_grpc")
+
+            self._BroadcastTxRequest = self._cosmos_tx_service_pb2.BroadcastTxRequest
+            self._SimulateTxRequest = self._cosmos_tx_service_pb2.SimulateRequest
+
         except AttributeError:
             raise ImportError(
                 "It seems that you are importing conflicting protobuf files. Have sou set the protobuf attribute to specify your coin? Check out the documentation for more information."
             )
         except:
             raise ImportError(
                 f"Couldn't import from {_protobuf_package}. Is the package installed? "
@@ -74,16 +78,16 @@
 
         Args:
             account (Account): Account
         """
         con = self._connect()
         address = account.address
 
-        query_stub = self.query_pb2_grpc.QueryStub(con)
-        account_request = self.query_pb2.QueryAccountRequest(address=address)
+        query_stub = self._cosmos_auth_query_pb2_grpc.QueryStub(con)
+        account_request = self._cosmos_auth_query_pb2.QueryAccountRequest(address=address)
 
         req = query_stub.Account(account_request)
         data = dict(MessageToDict(req.account))
 
         sequence = 0 if not "sequence" in data else int(data["sequence"])
         account_number = int(data["accountNumber"])
 
@@ -108,20 +112,57 @@
             hash: Transaction hash
             code: Result code
             log: Log (None if transaction successful)
         """
         con = self._connect()
         tx_bytes = transaction.get_tx_bytes()
 
-        tx_request = self.BroadcastTxRequest(
+        tx_request = self._BroadcastTxRequest(
             tx_bytes=tx_bytes,
             mode=2  # BROADCAST_MODE_SYNC
         )
 
-        tx_stub = self.service_pb2_grpc.ServiceStub(con)
+        tx_stub = self._cosmos_tx_service_pb2_grpc.ServiceStub(con)
         tx_data = tx_stub.BroadcastTx(tx_request)
 
         hash = tx_data.tx_response.txhash
         code = tx_data.tx_response.code
         log = None if code == 0 else tx_data.tx_response.raw_log
 
         return {"hash": hash, "code": code, "log": log}
+
+    def estimate_gas(self,
+                              *,
+                              transaction: Transaction,
+                              update: bool = True,
+                              multiplier: float = 1.2
+                     ) ->int:
+        """
+        Simulate a transaction to get the estimated gas usage.
+
+        Note:
+            Takes only positional arguments
+
+        Args:
+            transaction (Transaction): The transaction object
+            update (bool): Update the transaction with the estimated gas amount
+            multiplier (float): Multiplier for the estimated gas when updating the transaction. Defaults to 1.2
+
+        Returns:
+            expedted_gas: Expected gas
+        """
+        con = self._connect()
+        tx_bytes = transaction.get_tx_bytes()
+
+        simulate_request = self._SimulateTxRequest(
+            tx_bytes=tx_bytes,
+        )
+
+        tx_stub = self._cosmos_tx_service_pb2_grpc.ServiceStub(con)
+        tx_data = tx_stub.Simulate(simulate_request)
+
+        gas_used = tx_data.gas_info.gas_used
+
+        if update:
+            transaction.set_gas(int(gas_used * multiplier))
+
+        return gas_used
```

### Comparing `mospy_wallet-0.3.7/src/mospy/clients/HTTPClient.py` & `mospy_wallet-0.4/src/mospy/clients/HTTPClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,25 +95,25 @@
 
         Note:
             Takes only positional arguments
 
         Args:
             transaction (Transaction): The transaction object
             update (bool): Update the transaction with the estimated gas amount
-            update (float): Multiplier for the estimated gas when updating the transaction. Defaults to 1.2
+            multiplier (float): Multiplier for the estimated gas when updating the transaction. Defaults to 1.2
             timeout (int): Timeout
 
         Returns:
             expedted_gas: Expected gas
         """
         path = "/cosmos/tx/v1beta1/simulate"
         tx_bytes = transaction.get_tx_bytes_as_string()
         payload = {"tx_bytes": tx_bytes}
 
         data = self._make_post_request(path, payload, timeout)
 
         gas_used = int(data["gas_info"]["gas_used"])
 
         if update:
-
             transaction.set_gas(int(gas_used * multiplier))
+
         return gas_used
```

### Comparing `mospy_wallet-0.3.7/tests/test_account.py` & `mospy_wallet-0.4/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/tests/test_eth.py` & `mospy_wallet-0.4/tests/test_eth.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/tests/test_transaction.py` & `mospy_wallet-0.4/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/tests/clients/test_grpcclient.py` & `mospy_wallet-0.4/tests/clients/test_grpcclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,7 +48,17 @@
         )
 
         tx_data = client.broadcast_transaction(transaction=tx)
 
         assert (
             tx_data["hash"] ==
             "54B845AEB1523803D4EAF2330AE5759A83458CB5F0211159D04CC257428503C4")
+
+
+        client.load_account_data(account=account)
+
+        gas_used = client.estimate_gas(
+            transaction=tx,
+            update=False,
+        )
+
+        assert gas_used > 0
```

### Comparing `mospy_wallet-0.3.7/tests/clients/test_httpclient.py` & `mospy_wallet-0.4/tests/clients/test_httpclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
         assert (
             tx_data["hash"] ==
             "54B845AEB1523803D4EAF2330AE5759A83458CB5F0211159D04CC257428503C4")
 
         client.load_account_data(account=account)
 
-        gas_wanted = client.estimate_gas(
+        gas_used = client.estimate_gas(
             transaction=tx,
             update=False,
         )
 
 
-        assert gas_wanted > 0
+        assert gas_used > 0
+
```

### Comparing `mospy_wallet-0.3.7/README.md` & `mospy_wallet-0.4/README.md`

 * *Files identical despite different names*

### Comparing `mospy_wallet-0.3.7/pyproject.toml` & `mospy_wallet-0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mospy-wallet"
-version = "0.3.7"
+version = "0.4"
 description = "This package is a fork of cosmospy and is a light framework for the cosmos ecosystem"
 authors = [
     { name = "ctrl-felix", email = "dev@ctrl-felix.de" },
 ]
 readme = "README.md"
 keywords = ["cosmospy", "mospy", "cosmos"]
 license = {text = "BSD 3-Clause License"}
@@ -21,15 +21,16 @@
     "grpcio~=1.51.3",
     "httpx==0.23.0",
     "cosmospy-protobuf==0.0.2",
     "ecdsa==0.17.0",
     "bech32==1.2.0",
     "mnemonic==0.20",
     "hdwallets==0.1.2",
-    "safe-pysha3==1.0.3"
+    "safe-pysha3==1.0.3;python_version>='3.9'",
+    "pysha3==1.0.2;python_version<'3.9'",
 ]
 dynamic = []
 
 [project.urls]
 "Homepage" = "https://github.com/ctrl-Felix/mospy/"
 "Bug Tracker" = "https://github.com/ctrl-Felix/mospy/issues"
```

### Comparing `mospy_wallet-0.3.7/PKG-INFO` & `mospy_wallet-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mospy-wallet
-Version: 0.3.7
+Version: 0.4
 Summary: This package is a fork of cosmospy and is a light framework for the cosmos ecosystem
 Project-URL: Homepage, https://github.com/ctrl-Felix/mospy/
 Project-URL: Bug Tracker, https://github.com/ctrl-Felix/mospy/issues
 Author-email: ctrl-felix <dev@ctrl-felix.de>
 License: BSD 3-Clause License
 Keywords: cosmos,cosmospy,mospy
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,16 @@
 Requires-Dist: cosmospy-protobuf==0.0.2
 Requires-Dist: ecdsa==0.17.0
 Requires-Dist: grpcio~=1.51.3
 Requires-Dist: hdwallets==0.1.2
 Requires-Dist: httpx==0.23.0
 Requires-Dist: mnemonic==0.20
 Requires-Dist: protobuf==4.22.1
-Requires-Dist: safe-pysha3==1.0.3
+Requires-Dist: pysha3==1.0.2; python_version < '3.9'
+Requires-Dist: safe-pysha3==1.0.3; python_version >= '3.9'
 Description-Content-Type: text/markdown
 
 # MosPy
 
 MosPy is a fork of the cosmospy library and aims to be a versatile transaction signing library for the whole cosmos ecosystem.
 It depends [cosmospy-protobuf](https://github.com/ctrl-Felix/cosmospy-protobuf) for the protos. Through this library you also can add your own transaction types and sign them through Mospy.
```

