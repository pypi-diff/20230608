# Comparing `tmp/cic-contracts-0.3.0.tar.gz` & `tmp/cic-contracts-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cic-contracts-0.3.0.tar", last modified: Thu Jun  8 07:18:45 2023, max compression
+gzip compressed data, was "dist/cic-contracts-0.3.1.tar", last modified: Thu Jun  8 07:22:41 2023, max compression
```

## Comparing `cic-contracts-0.3.0.tar` & `cic-contracts-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,59 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:18:45.359983 cic-contracts-0.3.0/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       53 2023-06-06 12:01:24.000000 cic-contracts-0.3.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      706 2023-06-08 07:18:45.359983 cic-contracts-0.3.0/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:18:45.356650 cic-contracts-0.3.0/cic_contracts/
--rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.0/cic_contracts/accounts_index.py
--rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.0/cic_contracts/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.0/cic_contracts/erc20.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.0/cic_contracts/registry.py
--rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.0/cic_contracts/writer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:18:45.356650 cic-contracts-0.3.0/cic_contracts.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      706 2023-06-08 07:18:45.000000 cic-contracts-0.3.0/cic_contracts.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      884 2023-06-08 07:18:45.000000 cic-contracts-0.3.0/cic_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 07:18:45.000000 cic-contracts-0.3.0/cic_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-08 07:18:45.000000 cic-contracts-0.3.0/cic_contracts.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       36 2023-06-08 07:18:45.000000 cic-contracts-0.3.0/cic_contracts.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:18:45.356650 cic-contracts-0.3.0/eth_capped/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.0/eth_capped/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.0/eth_capped/capped.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:18:45.356650 cic-contracts-0.3.0/eth_expire/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.0/eth_expire/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.0/eth_expire/expire.py
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.0/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      768 2023-06-08 07:18:45.359983 cic-contracts-0.3.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      494 2022-04-29 14:00:22.000000 cic-contracts-0.3.0/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:18:45.359983 cic-contracts-0.3.0/solidity/
--rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-06 17:11:24.000000 cic-contracts-0.3.0/solidity/BurnerTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.0/solidity/BurnerTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-06 17:11:24.000000 cic-contracts-0.3.0/solidity/CappedTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.0/solidity/CappedTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-06 17:11:24.000000 cic-contracts-0.3.0/solidity/ExpireTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-06 13:56:29.000000 cic-contracts-0.3.0/solidity/ExpireTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-06 17:11:24.000000 cic-contracts-0.3.0/solidity/MinterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.0/solidity/MinterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-06-08 07:04:30.000000 cic-contracts-0.3.0/solidity/SealTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      611 2023-06-08 07:04:28.000000 cic-contracts-0.3.0/solidity/SealTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 06:46:14.000000 cic-contracts-0.3.0/solidity/WriterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.0/solidity/WriterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.0/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:18:45.359983 cic-contracts-0.3.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.0/tests/test_burner.py
--rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-06 12:45:50.000000 cic-contracts-0.3.0/tests/test_capped.py
--rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-06 13:23:05.000000 cic-contracts-0.3.0/tests/test_expire.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.0/tests/test_minter.py
--rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.0/tests/test_seal.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.0/tests/test_writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.039982 cic-contracts-0.3.1/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.1/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       54 2023-06-08 07:22:32.000000 cic-contracts-0.3.1/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 07:22:41.039982 cic-contracts-0.3.1/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.1/README.md
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.033315 cic-contracts-0.3.1/cic_contracts/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.1/cic_contracts/accounts_index.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.1/cic_contracts/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.1/cic_contracts/erc20.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.1/cic_contracts/registry.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.1/cic_contracts/writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.033315 cic-contracts-0.3.1/cic_contracts.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 07:22:41.000000 cic-contracts-0.3.1/cic_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1065 2023-06-08 07:22:41.000000 cic-contracts-0.3.1/cic_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 07:22:41.000000 cic-contracts-0.3.1/cic_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-08 07:22:41.000000 cic-contracts-0.3.1/cic_contracts.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-08 07:22:41.000000 cic-contracts-0.3.1/cic_contracts.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.033315 cic-contracts-0.3.1/eth_burner/
+-rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.1/eth_burner/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.1/eth_burner/burn.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.033315 cic-contracts-0.3.1/eth_capped/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.1/eth_capped/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.1/eth_capped/capped.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.033315 cic-contracts-0.3.1/eth_expire/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.1/eth_expire/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.1/eth_expire/expire.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.036649 cic-contracts-0.3.1/eth_minter/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.1/eth_minter/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.1/eth_minter/minter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.036649 cic-contracts-0.3.1/eth_seal/
+-rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.1/eth_seal/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.1/eth_seal/seal.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.036649 cic-contracts-0.3.1/eth_writer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.1/eth_writer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.1/eth_writer/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.1/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      814 2023-06-08 07:22:41.039982 cic-contracts-0.3.1/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.1/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.036649 cic-contracts-0.3.1/solidity/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-06 17:11:24.000000 cic-contracts-0.3.1/solidity/BurnerTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.1/solidity/BurnerTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-06 17:11:24.000000 cic-contracts-0.3.1/solidity/CappedTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.1/solidity/CappedTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-06 17:11:24.000000 cic-contracts-0.3.1/solidity/ExpireTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-06 13:56:29.000000 cic-contracts-0.3.1/solidity/ExpireTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-06 17:11:24.000000 cic-contracts-0.3.1/solidity/MinterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.1/solidity/MinterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-06-08 07:04:30.000000 cic-contracts-0.3.1/solidity/SealTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      611 2023-06-08 07:04:28.000000 cic-contracts-0.3.1/solidity/SealTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 06:46:14.000000 cic-contracts-0.3.1/solidity/WriterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.1/solidity/WriterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.1/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:22:41.036649 cic-contracts-0.3.1/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.1/tests/test_burner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-06 12:45:50.000000 cic-contracts-0.3.1/tests/test_capped.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-06 13:23:05.000000 cic-contracts-0.3.1/tests/test_expire.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.1/tests/test_minter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.1/tests/test_seal.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.1/tests/test_writer.py
```

### Comparing `cic-contracts-0.3.0/LICENSE` & `cic-contracts-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/cic_contracts/accounts_index.py` & `cic-contracts-0.3.1/cic_contracts/accounts_index.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/cic_contracts/base.py` & `cic-contracts-0.3.1/cic_contracts/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/cic_contracts/erc20.py` & `cic-contracts-0.3.1/cic_contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/cic_contracts/registry.py` & `cic-contracts-0.3.1/cic_contracts/registry.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/cic_contracts/writer.py` & `cic-contracts-0.3.1/cic_contracts/writer.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/eth_capped/capped.py` & `cic-contracts-0.3.1/eth_capped/capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/eth_expire/expire.py` & `cic-contracts-0.3.1/eth_expire/expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/setup.cfg` & `cic-contracts-0.3.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cic-contracts
-version = 0.3.0
+version = 0.3.1
 description = CIC network smart contract interfaces
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://gitlab.com/cicnet/cic-contracts
 keywords = 
 	dlt
 	blockchain
@@ -21,17 +21,21 @@
 	Topic :: Internet
 license = GPL3
 licence_files = 
 	LICENSE
 
 [options]
 include_package_data = True
-python_requires = >= 3.7
+python_requires = >= 3.8
 packages = 
 	cic_contracts
 	eth_capped
 	eth_expire
+	eth_seal
+	eth_burner
+	eth_minter
+	eth_writer
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cic-contracts-0.3.0/solidity/BurnerTest.bin` & `cic-contracts-0.3.1/solidity/BurnerTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/BurnerTest.sol` & `cic-contracts-0.3.1/solidity/BurnerTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/CappedTest.bin` & `cic-contracts-0.3.1/solidity/CappedTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/CappedTest.sol` & `cic-contracts-0.3.1/solidity/CappedTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/ExpireTest.bin` & `cic-contracts-0.3.1/solidity/ExpireTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/ExpireTest.sol` & `cic-contracts-0.3.1/solidity/ExpireTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/MinterTest.bin` & `cic-contracts-0.3.1/solidity/MinterTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/MinterTest.sol` & `cic-contracts-0.3.1/solidity/MinterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/SealTest.bin` & `cic-contracts-0.3.1/solidity/SealTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/SealTest.sol` & `cic-contracts-0.3.1/solidity/SealTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/WriterTest.bin` & `cic-contracts-0.3.1/solidity/WriterTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/solidity/WriterTest.sol` & `cic-contracts-0.3.1/solidity/WriterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/tests/test_burner.py` & `cic-contracts-0.3.1/tests/test_burner.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/tests/test_capped.py` & `cic-contracts-0.3.1/tests/test_capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/tests/test_expire.py` & `cic-contracts-0.3.1/tests/test_expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/tests/test_minter.py` & `cic-contracts-0.3.1/tests/test_minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/tests/test_seal.py` & `cic-contracts-0.3.1/tests/test_seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.0/tests/test_writer.py` & `cic-contracts-0.3.1/tests/test_writer.py`

 * *Files identical despite different names*

