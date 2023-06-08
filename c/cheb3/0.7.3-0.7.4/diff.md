# Comparing `tmp/cheb3-0.7.3.tar.gz` & `tmp/cheb3-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheb3-0.7.3.tar", last modified: Thu Jun  8 03:44:29 2023, max compression
+gzip compressed data, was "cheb3-0.7.4.tar", last modified: Thu Jun  8 04:03:37 2023, max compression
```

## Comparing `cheb3-0.7.3.tar` & `cheb3-0.7.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:44:29.175829 cheb3-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-08 03:44:19.000000 cheb3-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-08 03:44:29.175829 cheb3-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-08 03:44:19.000000 cheb3-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:44:29.171829 cheb3-0.7.3/cheb3/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:44:29.175829 cheb3-0.7.3/cheb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 03:44:19.000000 cheb3-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 03:44:29.175829 cheb3-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:03:37.438230 cheb3-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-08 04:03:28.000000 cheb3-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-08 04:03:37.438230 cheb3-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-08 04:03:28.000000 cheb3-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:03:37.438230 cheb3-0.7.4/cheb3/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-08 04:03:28.000000 cheb3-0.7.4/cheb3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:03:37.438230 cheb3-0.7.4/cheb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 04:03:37.000000 cheb3-0.7.4/cheb3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 04:03:28.000000 cheb3-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 04:03:37.438230 cheb3-0.7.4/setup.cfg
```

### Comparing `cheb3-0.7.3/LICENSE` & `cheb3-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.3/PKG-INFO` & `cheb3-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.7.3
+Version: 0.7.4
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
-Metadata-Version: 2.1 Name: cheb3 Version: 0.7.3 Summary: Web3 CTF tool based
+Metadata-Version: 2.1 Name: cheb3 Version: 0.7.4 Summary: Web3 CTF tool based
 on web3.py Author-email: YanhuiJessica
 gmail.com> Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/ Project-
 URL: Source, https://github.com/YanhuiJessica/cheb3 Project-URL: Bug Reports,
 https://github.com/YanhuiJessica/cheb3/issues Classifier: Development Status ::
 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `cheb3-0.7.3/README.md` & `cheb3-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.3/cheb3/account.py` & `cheb3-0.7.4/cheb3/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from web3 import Web3
 from web3._utils.datatypes import PropertyCheckingFactory
 from web3.types import TxReceipt
 from eth_typing import HexStr
 import eth_account
 
+from cheb3.constants import GAS_BUFFER
+
 from loguru import logger
 
 
 class Account:
     """Please use :func:`cheb3.Connection.account` interface to
     create an account instance associated with the connection.
     """
@@ -25,28 +27,24 @@
         if self.w3 is None:
             raise AttributeError(
                 "The `Account` class has not been initialized. Please use the "
                 "`Connection.account` interface to create an account."
             )
 
         if private_key is None:
-            self.eth_acct = eth_account.Account.create(
-                "".join(random.choices(string.ascii_letters, k=3))
-            )
+            self.eth_acct = eth_account.Account.create("".join(random.choices(string.ascii_letters, k=3)))
         else:
             self.eth_acct = eth_account.Account.from_key(private_key)
 
         self.address = self.eth_acct.address
         self.private_key = self.eth_acct.key.hex()
 
     @classmethod
     def factory(cls, w3: Web3) -> "Account":
-        eth_acct = cast(
-            Account, PropertyCheckingFactory(cls.__name__, (cls,), {"w3": w3})
-        )
+        eth_acct = cast(Account, PropertyCheckingFactory(cls.__name__, (cls,), {"w3": w3}))
         return eth_acct
 
     def get_balance(self) -> int:
         """Returns the balance of the account instance."""
         return self.w3.eth.get_balance(self.eth_acct.address)
 
     def call(self, to: HexStr, data: HexStr = "0x") -> HexBytes:
@@ -65,17 +63,15 @@
             {
                 "to": to,
                 "from": self.address,
                 "data": data,
             }
         )
 
-    def send_transaction(
-        self, to: HexStr, value: int = 0, data: HexStr = "0x", **kwargs
-    ) -> TxReceipt:
+    def send_transaction(self, to: HexStr, value: int = 0, data: HexStr = "0x", **kwargs) -> TxReceipt:
         """Transfer ETH or interact with a smart contract.
 
         :param to: The address of the receiver.
         :type to: HexStr
         :param value: The amount to transfer, defaults to 0 (wei).
         :type value: int
         :param data: The transaction data, defaults to `0x`.
@@ -93,15 +89,15 @@
             "to": to,
             "chainId": self.w3.eth.chain_id,
             "nonce": self.w3.eth.get_transaction_count(self.address),
             "value": value,
             "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
             "data": data,
         }
-        tx["gas"] = kwargs.get("gas_limit", self.w3.eth.estimate_gas(tx))
+        tx["gas"] = kwargs.get("gas_limit", self.w3.eth.estimate_gas(tx) + GAS_BUFFER)
         tx = self.eth_acct.sign_transaction(tx).rawTransaction
         tx_hash = self.w3.eth.send_raw_transaction(tx).hex()
         logger.info(f"Transaction to {to}: {tx_hash}")
         receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         if not receipt.status:
             raise Exception(f"Transact to {to} failed.")
         return receipt
```

### Comparing `cheb3-0.7.3/cheb3/connection.py` & `cheb3-0.7.4/cheb3/connection.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.3/cheb3/contract.py` & `cheb3-0.7.4/cheb3/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             self.instance.constructor(*constructor_args).build_transaction(
                 {
                     "chainId": self.w3.eth.chain_id,
                     "nonce": self.w3.eth.get_transaction_count(self.signer.address),
                     "gas": kwargs.get(
                         "gas_limit",
                         self.instance.constructor(*constructor_args).estimate_gas({"from": self.signer.address}),
-                    ),
+                    ) + GAS_BUFFER,
                     "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
                     "value": kwargs.get("value", 0),
                 }
             )
         ).rawTransaction
         logger.debug(f"Deploying {type(self).__name__} ...")
         tx_hash = self.w3.eth.send_raw_transaction(tx).hex()
@@ -106,15 +106,15 @@
                 "from": self.signer.address,
                 "to": None,
                 "chainId": self.w3.eth.chain_id,
                 "nonce": self.w3.eth.get_transaction_count(self.signer.address),
                 "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
                 "data": proxy_bytecode,
             }
-            tx["gas"] = kwargs.get("gas_limit", self.w3.eth.estimate_gas(tx))
+            tx["gas"] = kwargs.get("gas_limit", self.w3.eth.estimate_gas(tx) + GAS_BUFFER)
             tx = self.signer.sign_transaction(tx).rawTransaction
             logger.debug("Deploying the proxy ...")
             tx_hash = self.w3.eth.send_raw_transaction(tx).hex()
             receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
             if not receipt.status:
                 raise Exception("Failed to deploy the proxy.")
             logger.info(f"The proxy is deployed at {receipt.contractAddress}")
```

### Comparing `cheb3-0.7.3/cheb3/utils.py` & `cheb3-0.7.4/cheb3/utils.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.3/cheb3.egg-info/PKG-INFO` & `cheb3-0.7.4/cheb3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.7.3
+Version: 0.7.4
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
-Metadata-Version: 2.1 Name: cheb3 Version: 0.7.3 Summary: Web3 CTF tool based
+Metadata-Version: 2.1 Name: cheb3 Version: 0.7.4 Summary: Web3 CTF tool based
 on web3.py Author-email: YanhuiJessica
 gmail.com> Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/ Project-
 URL: Source, https://github.com/YanhuiJessica/cheb3 Project-URL: Bug Reports,
 https://github.com/YanhuiJessica/cheb3/issues Classifier: Development Status ::
 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `cheb3-0.7.3/pyproject.toml` & `cheb3-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cheb3"
-version = "0.7.3"
+version = "0.7.4"
 authors = [{name = "YanhuiJessica",email = "y4nhv1@gmail.com"}]
 description = "Web3 CTF tool based on web3.py"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "web3>=6.0.0",
   "py-solc-x",
```

