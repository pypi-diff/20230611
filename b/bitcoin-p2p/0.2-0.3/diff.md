# Comparing `tmp/bitcoin_p2p-0.2.tar.gz` & `tmp/bitcoin_p2p-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_p2p-0.2.tar", last modified: Sun Jun 11 05:47:39 2023, max compression
+gzip compressed data, was "bitcoin_p2p-0.3.tar", last modified: Sun Jun 11 06:32:06 2023, max compression
```

## Comparing `bitcoin_p2p-0.2.tar` & `bitcoin_p2p-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 05:47:39.451133 bitcoin_p2p-0.2/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_p2p-0.2/LICENSE
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4540 2023-06-11 05:47:39.451133 bitcoin_p2p-0.2/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4046 2023-06-10 19:59:43.000000 bitcoin_p2p-0.2/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 05:47:39.451133 bitcoin_p2p-0.2/bitcoin_p2p/
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 05:47:39.451133 bitcoin_p2p-0.2/bitcoin_p2p/bitcoin_p2p.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4540 2023-06-11 05:47:39.000000 bitcoin_p2p-0.2/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      260 2023-06-11 05:47:39.000000 bitcoin_p2p-0.2/bitcoin_p2p/bitcoin_p2p.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-11 05:47:39.000000 bitcoin_p2p-0.2/bitcoin_p2p/bitcoin_p2p.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       48 2023-06-11 05:47:39.000000 bitcoin_p2p-0.2/bitcoin_p2p/bitcoin_p2p.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-11 05:47:39.000000 bitcoin_p2p-0.2/bitcoin_p2p/bitcoin_p2p.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-06-11 05:47:39.451133 bitcoin_p2p-0.2/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1175 2023-06-11 05:46:22.000000 bitcoin_p2p-0.2/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 06:32:06.250905 bitcoin_p2p-0.3/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_p2p-0.3/LICENSE
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4625 2023-06-11 06:32:06.250905 bitcoin_p2p-0.3/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4131 2023-06-11 06:30:57.000000 bitcoin_p2p-0.3/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 06:32:06.250905 bitcoin_p2p-0.3/bitcoin_p2p/
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 06:32:06.250905 bitcoin_p2p-0.3/bitcoin_p2p/bitcoin_p2p.egg-info/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4625 2023-06-11 06:32:06.000000 bitcoin_p2p-0.3/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      260 2023-06-11 06:32:06.000000 bitcoin_p2p-0.3/bitcoin_p2p/bitcoin_p2p.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-11 06:32:06.000000 bitcoin_p2p-0.3/bitcoin_p2p/bitcoin_p2p.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       48 2023-06-11 06:32:06.000000 bitcoin_p2p-0.3/bitcoin_p2p/bitcoin_p2p.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-11 06:32:06.000000 bitcoin_p2p-0.3/bitcoin_p2p/bitcoin_p2p.egg-info/top_level.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-06-11 06:32:06.250905 bitcoin_p2p-0.3/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1175 2023-06-11 06:31:35.000000 bitcoin_p2p-0.3/setup.py
```

### Comparing `bitcoin_p2p-0.2/LICENSE` & `bitcoin_p2p-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_p2p-0.2/PKG-INFO` & `bitcoin_p2p-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin_p2p
-Version: 0.2
+Version: 0.3
 Summary: Bitcoin p2p communication tools in python
 Home-page: https://github.com/andreasgriffin/bitcoin-p2p
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Listen to the bitcoin p2p transaction data
 
 `bitcoin-p2p` can listen (no verification) to the p2p traffic of a bitcoin node and display the transactions like:
 ```python
-import socket
+import socket, asyncio
 import bdkpython as bdk
 from bitcoin_p2p import tools, p2p
 # see https://github.com/andreasgriffin/bitcoin-p2p
 
 global_dict = {}
 
 def callback_min_feerate(feerate):
@@ -34,15 +34,16 @@
     # transaction = tools.filter_txs(transaction)
     #if not transaction:
     #    return
     
     print(tools.transaction_table(transaction))
     
     
-p2p.listen(p2p.get_bitcoin_peer(), call_back_tx=call_back_tx, callback_min_feerate=callback_min_feerate)
+
+await p2p.listen(p2p.get_bitcoin_peer(), call_back_tx=call_back_tx, callback_min_feerate=callback_min_feerate )
 ```
 with the output:
 ```
 Received sendheaders command
 Received sendcmpct
 Received sendcmpct
 Received ping
@@ -78,15 +79,23 @@
 
 
 
 # Install package
 
 
 
+### From pypi
+
+```shell
+pip install bitcoin_p2p
+```
+
+
 
+###  From git
 
 ```shell
 python setup.py sdist bdist_wheel
 pip install dist/bitcoin_p2p-0.1-py3-none-any.whl  --force-reinstall
 ```
```

### Comparing `bitcoin_p2p-0.2/README.md` & `bitcoin_p2p-0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Listen to the bitcoin p2p transaction data
 
 `bitcoin-p2p` can listen (no verification) to the p2p traffic of a bitcoin node and display the transactions like:
 ```python
-import socket
+import socket, asyncio
 import bdkpython as bdk
 from bitcoin_p2p import tools, p2p
 # see https://github.com/andreasgriffin/bitcoin-p2p
 
 global_dict = {}
 
 def callback_min_feerate(feerate):
@@ -19,15 +19,16 @@
     # transaction = tools.filter_txs(transaction)
     #if not transaction:
     #    return
     
     print(tools.transaction_table(transaction))
     
     
-p2p.listen(p2p.get_bitcoin_peer(), call_back_tx=call_back_tx, callback_min_feerate=callback_min_feerate)
+
+await p2p.listen(p2p.get_bitcoin_peer(), call_back_tx=call_back_tx, callback_min_feerate=callback_min_feerate )
 ```
 with the output:
 ```
 Received sendheaders command
 Received sendcmpct
 Received sendcmpct
 Received ping
@@ -63,15 +64,23 @@
 
 
 
 # Install package
 
 
 
+### From pypi
+
+```shell
+pip install bitcoin_p2p
+```
+
+
 
+###  From git
 
 ```shell
 python setup.py sdist bdist_wheel
 pip install dist/bitcoin_p2p-0.1-py3-none-any.whl  --force-reinstall
 ```
```

### Comparing `bitcoin_p2p-0.2/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO` & `bitcoin_p2p-0.3/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin-p2p
-Version: 0.2
+Version: 0.3
 Summary: Bitcoin p2p communication tools in python
 Home-page: https://github.com/andreasgriffin/bitcoin-p2p
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Listen to the bitcoin p2p transaction data
 
 `bitcoin-p2p` can listen (no verification) to the p2p traffic of a bitcoin node and display the transactions like:
 ```python
-import socket
+import socket, asyncio
 import bdkpython as bdk
 from bitcoin_p2p import tools, p2p
 # see https://github.com/andreasgriffin/bitcoin-p2p
 
 global_dict = {}
 
 def callback_min_feerate(feerate):
@@ -34,15 +34,16 @@
     # transaction = tools.filter_txs(transaction)
     #if not transaction:
     #    return
     
     print(tools.transaction_table(transaction))
     
     
-p2p.listen(p2p.get_bitcoin_peer(), call_back_tx=call_back_tx, callback_min_feerate=callback_min_feerate)
+
+await p2p.listen(p2p.get_bitcoin_peer(), call_back_tx=call_back_tx, callback_min_feerate=callback_min_feerate )
 ```
 with the output:
 ```
 Received sendheaders command
 Received sendcmpct
 Received sendcmpct
 Received ping
@@ -78,15 +79,23 @@
 
 
 
 # Install package
 
 
 
+### From pypi
+
+```shell
+pip install bitcoin_p2p
+```
+
+
 
+###  From git
 
 ```shell
 python setup.py sdist bdist_wheel
 pip install dist/bitcoin_p2p-0.1-py3-none-any.whl  --force-reinstall
 ```
```

### Comparing `bitcoin_p2p-0.2/setup.py` & `bitcoin_p2p-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="bitcoin_p2p",
-    version="0.2",
+    version="0.3",
     author="Andreas Griffin",
     author_email="andreasgriffin@proton.me",
     description="Bitcoin p2p communication tools in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andreasgriffin/bitcoin-p2p",
     packages=find_namespace_packages("bitcoin_p2p", include=["bitcoin_p2p.*"]),
```

