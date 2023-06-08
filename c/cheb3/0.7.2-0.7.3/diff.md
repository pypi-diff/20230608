# Comparing `tmp/cheb3-0.7.2.tar.gz` & `tmp/cheb3-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheb3-0.7.2.tar", last modified: Tue Jun  6 13:41:08 2023, max compression
+gzip compressed data, was "cheb3-0.7.3.tar", last modified: Thu Jun  8 03:44:29 2023, max compression
```

## Comparing `cheb3-0.7.2.tar` & `cheb3-0.7.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:41:08.839815 cheb3-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-06 13:40:55.000000 cheb3-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-06 13:41:08.839815 cheb3-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-06 13:40:55.000000 cheb3-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:41:08.839815 cheb3-0.7.2/cheb3/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-06 13:40:55.000000 cheb3-0.7.2/cheb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-06 13:40:55.000000 cheb3-0.7.2/cheb3/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-06 13:40:55.000000 cheb3-0.7.2/cheb3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 13:40:55.000000 cheb3-0.7.2/cheb3/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-06-06 13:40:55.000000 cheb3-0.7.2/cheb3/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-06 13:40:55.000000 cheb3-0.7.2/cheb3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:41:08.839815 cheb3-0.7.2/cheb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-06 13:41:08.000000 cheb3-0.7.2/cheb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 13:41:08.000000 cheb3-0.7.2/cheb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:41:08.000000 cheb3-0.7.2/cheb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 13:41:08.000000 cheb3-0.7.2/cheb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 13:41:08.000000 cheb3-0.7.2/cheb3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-06 13:40:55.000000 cheb3-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:41:08.839815 cheb3-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:44:29.175829 cheb3-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-08 03:44:19.000000 cheb3-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-08 03:44:29.175829 cheb3-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-08 03:44:19.000000 cheb3-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:44:29.171829 cheb3-0.7.3/cheb3/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-08 03:44:19.000000 cheb3-0.7.3/cheb3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:44:29.175829 cheb3-0.7.3/cheb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 03:44:29.000000 cheb3-0.7.3/cheb3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 03:44:19.000000 cheb3-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 03:44:29.175829 cheb3-0.7.3/setup.cfg
```

### Comparing `cheb3-0.7.2/LICENSE` & `cheb3-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.2/PKG-INFO` & `cheb3-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.7.2
+Version: 0.7.3
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
-Metadata-Version: 2.1 Name: cheb3 Version: 0.7.2 Summary: Web3 CTF tool based
+Metadata-Version: 2.1 Name: cheb3 Version: 0.7.3 Summary: Web3 CTF tool based
 on web3.py Author-email: YanhuiJessica
 gmail.com> Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/ Project-
 URL: Source, https://github.com/YanhuiJessica/cheb3 Project-URL: Bug Reports,
 https://github.com/YanhuiJessica/cheb3/issues Classifier: Development Status ::
 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `cheb3-0.7.2/README.md` & `cheb3-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.2/cheb3/account.py` & `cheb3-0.7.3/cheb3/account.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.2/cheb3/connection.py` & `cheb3-0.7.3/cheb3/connection.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.2/cheb3/contract.py` & `cheb3-0.7.3/cheb3/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 )
 from web3._utils.function_identifiers import FallbackFn, ReceiveFn
 from web3.types import ABI, TxReceipt
 from eth_typing import ChecksumAddress
 import eth_account
 
 from cheb3.account import Account
+from cheb3.constants import GAS_BUFFER
 
 from loguru import logger
 
 
 class Contract:
     """Please use :func:`cheb3.Connection.contract` interface to
     create a contract instance associated with the connection.
@@ -218,15 +219,15 @@
             raise AttributeError("The `signer` is missing.")
 
         tx = {
             "chainId": self.w3.eth.chain_id,
             "nonce": self.w3.eth.get_transaction_count(self.signer.address),
             "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
             "value": kwargs.get("value", 0),
-            "gas": kwargs.get("gas_limit", self.estimate_gas()),
+            "gas": kwargs.get("gas_limit", self.estimate_gas() + GAS_BUFFER),
         }
         tx = self.signer.sign_transaction(self.build_transaction(tx)).rawTransaction
         tx_hash = self.w3.eth.send_raw_transaction(tx).hex()
         func_name = self.function_identifier if isinstance(self.function_identifier, str) else self.function_identifier.__name__
         logger.info(f"({self.address}).{func_name} transaction hash: {tx_hash}")
         receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         if not receipt.status:
```

### Comparing `cheb3-0.7.2/cheb3/utils.py` & `cheb3-0.7.3/cheb3/utils.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.2/cheb3.egg-info/PKG-INFO` & `cheb3-0.7.3/cheb3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.7.2
+Version: 0.7.3
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
-Metadata-Version: 2.1 Name: cheb3 Version: 0.7.2 Summary: Web3 CTF tool based
+Metadata-Version: 2.1 Name: cheb3 Version: 0.7.3 Summary: Web3 CTF tool based
 on web3.py Author-email: YanhuiJessica
 gmail.com> Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/ Project-
 URL: Source, https://github.com/YanhuiJessica/cheb3 Project-URL: Bug Reports,
 https://github.com/YanhuiJessica/cheb3/issues Classifier: Development Status ::
 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `cheb3-0.7.2/pyproject.toml` & `cheb3-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cheb3"
-version = "0.7.2"
+version = "0.7.3"
 authors = [{name = "YanhuiJessica",email = "y4nhv1@gmail.com"}]
 description = "Web3 CTF tool based on web3.py"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "web3>=6.0.0",
   "py-solc-x",
```

