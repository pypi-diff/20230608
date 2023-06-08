# Comparing `tmp/chaind-eth-0.3.3.tar.gz` & `tmp/chaind-eth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaind-eth-0.3.3.tar", last modified: Mon Nov 14 08:15:05 2022, max compression
+gzip compressed data, was "chaind-eth-0.4.0.tar", last modified: Thu Jun  8 15:20:43 2023, max compression
```

## Comparing `chaind-eth-0.3.3.tar` & `chaind-eth-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/
--rw-r--r--   0 lash      (1000) lash      (1000)       73 2022-11-14 07:40:20.000000 chaind-eth-0.3.3/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:39:21.000000 chaind-eth-0.3.3/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      119 2022-11-14 07:41:19.000000 chaind-eth-0.3.3/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      734 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     8677 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      870 2022-11-14 07:39:34.000000 chaind-eth-0.3.3/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:39:36.000000 chaind-eth-0.3.3/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind/eth/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1104 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/cache.py
--rw-r--r--   0 lash      (1000) lash      (1000)      524 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind/eth/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      586 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/cli/csv.py
--rw-r--r--   0 lash      (1000) lash      (1000)      745 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/cli/output.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind/eth/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind/eth/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       99 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/data/config/config.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind/eth/data/config/syncer/
--rw-r--r--   0 lash      (1000) lash      (1000)       62 2022-04-10 08:10:40.000000 chaind-eth-0.3.3/chaind/eth/data/config/syncer/config.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      210 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/dispatch.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind/eth/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     4756 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/runnable/queuer.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5868 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/runnable/send.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3221 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/runnable/syncer.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1103 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/settings.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind/eth/token/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/token/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1590 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/token/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1004 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/token/erc20.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1045 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/token/gas.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3076 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/chaind/eth/token/process.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/chaind_eth.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      734 2022-11-14 08:15:05.000000 chaind-eth-0.3.3/chaind_eth.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      795 2022-11-14 08:15:05.000000 chaind-eth-0.3.3/chaind_eth.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2022-11-14 08:15:05.000000 chaind-eth-0.3.3/chaind_eth.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      170 2022-11-14 08:15:05.000000 chaind-eth-0.3.3/chaind_eth.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      105 2022-11-14 08:15:05.000000 chaind-eth-0.3.3/chaind_eth.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2022-11-14 08:15:05.000000 chaind-eth-0.3.3/chaind_eth.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       17 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/erc20_requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       79 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1011 2022-11-14 08:15:05.599960 chaind-eth-0.3.3/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      969 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       81 2022-10-13 11:39:39.000000 chaind-eth-0.3.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.513317 chaind-eth-0.4.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)       73 2022-11-14 07:40:20.000000 chaind-eth-0.4.0/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:39:21.000000 chaind-eth-0.4.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      119 2022-11-14 07:41:19.000000 chaind-eth-0.4.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      666 2023-06-08 15:20:43.513317 chaind-eth-0.4.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     8659 2022-11-14 18:55:38.000000 chaind-eth-0.4.0/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      870 2022-11-14 07:39:34.000000 chaind-eth-0.4.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:39:36.000000 chaind-eth-0.4.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.509984 chaind-eth-0.4.0/chaind/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.509984 chaind-eth-0.4.0/chaind/eth/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1218 2023-06-08 15:20:11.000000 chaind-eth-0.4.0/chaind/eth/cache.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      591 2023-06-08 15:20:11.000000 chaind-eth-0.4.0/chaind/eth/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.509984 chaind-eth-0.4.0/chaind/eth/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      586 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/cli/csv.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      745 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/cli/output.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.509984 chaind-eth-0.4.0/chaind/eth/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.509984 chaind-eth-0.4.0/chaind/eth/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       99 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/data/config/config.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.509984 chaind-eth-0.4.0/chaind/eth/data/config/syncer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       62 2022-04-10 08:10:40.000000 chaind-eth-0.4.0/chaind/eth/data/config/syncer/config.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      210 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/dispatch.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.513317 chaind-eth-0.4.0/chaind/eth/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     4756 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/runnable/queuer.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5929 2023-06-08 15:20:11.000000 chaind-eth-0.4.0/chaind/eth/runnable/send.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3221 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/runnable/syncer.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1247 2023-06-08 15:20:11.000000 chaind-eth-0.4.0/chaind/eth/settings.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.513317 chaind-eth-0.4.0/chaind/eth/token/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/token/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1590 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/token/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1004 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/token/erc20.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1045 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/token/gas.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3076 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/chaind/eth/token/process.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.513317 chaind-eth-0.4.0/chaind_eth.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      666 2023-06-08 15:20:43.000000 chaind-eth-0.4.0/chaind_eth.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      812 2023-06-08 15:20:43.000000 chaind-eth-0.4.0/chaind_eth.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 15:20:43.000000 chaind-eth-0.4.0/chaind_eth.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      170 2023-06-08 15:20:43.000000 chaind-eth-0.4.0/chaind_eth.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      106 2023-06-08 15:20:43.000000 chaind-eth-0.4.0/chaind_eth.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-06-08 15:20:43.000000 chaind-eth-0.4.0/chaind_eth.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       17 2023-06-08 15:20:11.000000 chaind-eth-0.4.0/erc20_requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       80 2023-06-08 15:20:11.000000 chaind-eth-0.4.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      943 2023-06-08 15:20:43.513317 chaind-eth-0.4.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      969 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       81 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:20:43.513317 chaind-eth-0.4.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2207 2022-10-13 11:39:39.000000 chaind-eth-0.4.0/tests/test_tx.py
```

### Comparing `chaind-eth-0.3.3/LICENSE` & `chaind-eth-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/README.md` & `chaind-eth-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - [x] blockchain listener that updates state of transactions in queue
 - [x] CLI transaction listing tool, filterable by:
 	* [x] transaction range with lower and/or upper bound
 	* [x] only show transaction with errors
 	* [x] only show transaction that have not yet completed
 - [x] systemd unit / socket service
 - [x] sql storage backend
-- [ ] filesystem storage backend
+- [x] filesystem storage backend
 
 
 ## prerequisites
 
 For these examples you need:
 
 - linux (tested on 5.12.x, perhaps wsl/macos will work too, no guarantees, though)
@@ -37,19 +37,19 @@
 
 
 ## setting up the database backend
 
 Currently there is no more practical way of setting up the database backend than to pull the repository and run a database migration script :/
 
 ```
-git clone https://gitlab.com/chaintool/chaind
+git clone https://git.defalsify.org/chaind
 cd chaind
 python -m venv .venv
 . .venv/bin/activate
-pip install --extra-index-url https://pip.grassrootseconomics.net:8433 -r requirements.txt
+pip install --extra-index-url https://pip.grassrootseconomics.net -r requirements.txt
 # the following will set up your database in ~/.local/share/chaind/eth/chaind.sqlite
 PYTHONPATH=. CHAIND_DOMAIN=eth DATABASE_ENGINE=sqlite python scripts/migrate.py
 ```
 
 
 ## usage example
 
@@ -62,15 +62,15 @@
 ```
 
 ### create a chaind-eth sandbox
 
 ```
 python -m venv .venv
 . .venv/bin/activate
-pip install --extra-index-url https://pip.grassrootseconomics.net:8433 "chaind-eth>=0.0.3a5"
+pip install --extra-index-url https://pip.grassrootseconomics.net "chaind-eth>=0.0.3a5"
 ```
 
 ### start the services
 
 In terminal window B
 
 ```
@@ -190,15 +190,15 @@
 By default the signed transactions are output as hex to stdout, each on a separate line.
 
 If a valid `--socket` is given (i.e. the socket of the `chaind-eth-server`) the transactions will be send to the socket instead. The hash of the transaction will be output to standard output.
 
 
 ### Using token symbols
 
-If token symols are to be used in some or all values of column 3, then a valid `--token-index` executable address is required (in this case, a smart contract implementing the [`registry`](https://gitlab.com/grassrootseconomics/cic-contracts/-/blob/master/solidity/Registry.sol) contract interface).
+If token symols are to be used in some or all values of column 3, then a valid `--token-index` executable address is required (in this case, a smart contract implementing the [`registry`](https://gitlab.com/cicnet/eth-contract-registry/-/blob/master/solidity/Registry.sol) contract interface).
 
 
 ### Input validity checks
 
 The validity of the input data is verified _before_ actual execution takes place.
 
 These checks include:
```

### Comparing `chaind-eth-0.3.3/WAIVER` & `chaind-eth-0.4.0/WAIVER`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/WAIVER.asc` & `chaind-eth-0.4.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind/eth/cache.py` & `chaind-eth-0.4.0/chaind/eth/cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+# standard imports
+import logging
+
 # external imports
 from hexathon import strip_0x
 from chainqueue.cache import (
         CacheTx,
         NoopNormalizer,
         )
 from chainlib.eth.tx import unpack
 from chainlib.encode import TxHexNormalizer
 
+logg = logging.getLogger(__name__)
 
 class Normalizer(TxHexNormalizer, NoopNormalizer):
 
     def __init__(self):
         super(Normalizer, self).__init__()
         self.address = self.wallet_address
         self.hash = self.tx_hash
@@ -29,13 +33,14 @@
     def __init__(self, chain_spec):
         super(EthCacheTx, self).__init__(chain_spec)
 
 
     def deserialize(self, signed_tx):
         signed_tx_bytes = bytes.fromhex(strip_0x(signed_tx))
         tx = unpack(signed_tx_bytes, self.chain_spec)
+        logg.debug('have tx {}'.format(tx))
         self.hash = eth_normalizer.hash(tx['hash'])
         self.sender = eth_normalizer.address(tx['from'])
         self.recipient = eth_normalizer.address(tx['to'])
         self.nonce = eth_normalizer.value(tx['nonce'])
         self.value = eth_normalizer.value(tx['value'])
         self.src = signed_tx
```

### Comparing `chaind-eth-0.3.3/chaind/eth/chain.py` & `chaind-eth-0.4.0/chaind/eth/chain.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 from chainlib.eth.tx import (
         receipt,
         Tx,
         )
 
 class EthChainInterface(ChainInterface):
 
-    def __init__(self):
+    def __init__(self, dialect_filter=None):
         self._block_by_number = block_by_number
         self._block_from_src = Block.from_src
         self._tx_receipt = receipt
         self._src_normalize = Tx.src_normalize
         self._block_latest = block_latest
+        self._dialect_filter = dialect_filter
```

### Comparing `chaind-eth-0.3.3/chaind/eth/cli/csv.py` & `chaind-eth-0.4.0/chaind/eth/cli/csv.py`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind/eth/cli/output.py` & `chaind-eth-0.4.0/chaind/eth/cli/output.py`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind/eth/runnable/queuer.py` & `chaind-eth-0.4.0/chaind/eth/runnable/queuer.py`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind/eth/runnable/send.py` & `chaind-eth-0.4.0/chaind/eth/runnable/send.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,16 @@
             settings.get('CHAIN_SPEC'),
             settings.get('SENDER_ADDRESS'),
             settings.get('SIGNER'),
             settings.get('GAS_ORACLE'),
             settings.get('NONCE_ORACLE'),
             )
     
-    processor = Processor(token_resolver, config.get('_SOURCE'), use_checksum=not config.get('_UNSAFE'))
+    logg.debug('source {}'.format(config.get('_SOURCE')))
+    processor = Processor(token_resolver, config.get('_SOURCE')[0], use_checksum=not config.get('_UNSAFE'))
     processor.add_processor(CSVProcessor())
 
     sends = None
     try:
         sends = processor.load(conn)
     except TxSourceError as e:
         sys.stderr.write('processing error: {}. processors: {}\n'.format(str(e), str(processor)))
```

### Comparing `chaind-eth-0.3.3/chaind/eth/runnable/syncer.py` & `chaind-eth-0.4.0/chaind/eth/runnable/syncer.py`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind/eth/token/base.py` & `chaind-eth-0.4.0/chaind/eth/token/base.py`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind/eth/token/erc20.py` & `chaind-eth-0.4.0/chaind/eth/token/erc20.py`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind/eth/token/gas.py` & `chaind-eth-0.4.0/chaind/eth/token/gas.py`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind/eth/token/process.py` & `chaind-eth-0.4.0/chaind/eth/token/process.py`

 * *Files identical despite different names*

### Comparing `chaind-eth-0.3.3/chaind_eth.egg-info/SOURCES.txt` & `chaind-eth-0.4.0/chaind_eth.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 chaind/eth/token/gas.py
 chaind/eth/token/process.py
 chaind_eth.egg-info/PKG-INFO
 chaind_eth.egg-info/SOURCES.txt
 chaind_eth.egg-info/dependency_links.txt
 chaind_eth.egg-info/entry_points.txt
 chaind_eth.egg-info/requires.txt
-chaind_eth.egg-info/top_level.txt
+chaind_eth.egg-info/top_level.txt
+tests/test_tx.py
```

### Comparing `chaind-eth-0.3.3/setup.cfg` & `chaind-eth-0.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [metadata]
 name = chaind-eth
-version = 0.3.3
+version = 0.4.0
 description = Queue server for ethereum
 author = Louis Holbrook
 author_email = dev@holbrook.no
-url = https://git.defalsify.org/chaind-eth.git
+url = https://git.defalsify.org/chaind-eth
 keywords = 
 	dlt
 	blockchain
 	cryptocurrency
 	ethereum
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 	Topic :: Internet
-license = OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+license = AGPLv3+
 licence_files = 
 	LICENSE
 
 [options]
-python_requires = >= 3.7
+python_requires = >= 3.8
 include_package_data = True
 packages = 
 	chaind.eth
 	chaind.eth.runnable
 	chaind.eth.cli
 	chaind.eth.token
```

### Comparing `chaind-eth-0.3.3/setup.py` & `chaind-eth-0.4.0/setup.py`

 * *Files identical despite different names*

