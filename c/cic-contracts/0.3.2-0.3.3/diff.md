# Comparing `tmp/cic-contracts-0.3.2.tar.gz` & `tmp/cic-contracts-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cic-contracts-0.3.2.tar", last modified: Thu Jun  8 07:34:25 2023, max compression
+gzip compressed data, was "cic-contracts-0.3.3.tar", last modified: Thu Jun  8 13:01:06 2023, max compression
```

## Comparing `cic-contracts-0.3.2.tar` & `cic-contracts-0.3.3.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       54 2023-06-08 07:22:32.000000 cic-contracts-0.3.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.2/README.md
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.546644 cic-contracts-0.3.2/cic_contracts/
--rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.2/cic_contracts/accounts_index.py
--rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.2/cic_contracts/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.2/cic_contracts/erc20.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.2/cic_contracts/registry.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.546644 cic-contracts-0.3.2/cic_contracts/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)      617 2023-02-24 10:28:52.000000 cic-contracts-0.3.2/cic_contracts/unittest/owned.py
--rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.2/cic_contracts/writer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.546644 cic-contracts-0.3.2/cic_contracts.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 07:34:25.000000 cic-contracts-0.3.2/cic_contracts.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1649 2023-06-08 07:34:25.000000 cic-contracts-0.3.2/cic_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 07:34:25.000000 cic-contracts-0.3.2/cic_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-08 07:34:25.000000 cic-contracts-0.3.2/cic_contracts.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-08 07:34:25.000000 cic-contracts-0.3.2/cic_contracts.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.546644 cic-contracts-0.3.2/eth_burner/
--rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.2/eth_burner/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.2/eth_burner/burn.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.546644 cic-contracts-0.3.2/eth_burner/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 16:41:44.000000 cic-contracts-0.3.2/eth_burner/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1658 2023-06-06 16:45:29.000000 cic-contracts-0.3.2/eth_burner/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      612 2023-06-06 16:43:41.000000 cic-contracts-0.3.2/eth_burner/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.546644 cic-contracts-0.3.2/eth_capped/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.2/eth_capped/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.2/eth_capped/capped.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_capped/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 12:09:11.000000 cic-contracts-0.3.2/eth_capped/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2175 2023-06-08 06:58:37.000000 cic-contracts-0.3.2/eth_capped/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1063 2023-06-06 13:45:58.000000 cic-contracts-0.3.2/eth_capped/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_expire/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.2/eth_expire/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.2/eth_expire/expire.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_expire/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 13:21:21.000000 cic-contracts-0.3.2/eth_expire/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2241 2023-06-06 14:03:08.000000 cic-contracts-0.3.2/eth_expire/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      975 2023-06-06 13:44:33.000000 cic-contracts-0.3.2/eth_expire/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_minter/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.2/eth_minter/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.2/eth_minter/minter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_minter/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 14:19:49.000000 cic-contracts-0.3.2/eth_minter/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1582 2023-06-06 14:24:30.000000 cic-contracts-0.3.2/eth_minter/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      618 2023-06-06 14:26:59.000000 cic-contracts-0.3.2/eth_minter/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_seal/
--rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.2/eth_seal/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.2/eth_seal/seal.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_seal/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-06-08 07:02:18.000000 cic-contracts-0.3.2/eth_seal/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2033 2023-06-08 07:03:31.000000 cic-contracts-0.3.2/eth_seal/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      502 2023-06-08 07:00:50.000000 cic-contracts-0.3.2/eth_seal/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_writer/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.2/eth_writer/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.2/eth_writer/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/eth_writer/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 17:01:25.000000 cic-contracts-0.3.2/eth_writer/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1935 2023-06-06 17:10:58.000000 cic-contracts-0.3.2/eth_writer/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-06-06 17:11:14.000000 cic-contracts-0.3.2/eth_writer/unittest/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      962 2023-06-08 07:34:25.553311 cic-contracts-0.3.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.2/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/solidity/
--rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-06 17:11:24.000000 cic-contracts-0.3.2/solidity/BurnerTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.2/solidity/BurnerTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-06 17:11:24.000000 cic-contracts-0.3.2/solidity/CappedTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.2/solidity/CappedTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-06 17:11:24.000000 cic-contracts-0.3.2/solidity/ExpireTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-06 13:56:29.000000 cic-contracts-0.3.2/solidity/ExpireTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-06 17:11:24.000000 cic-contracts-0.3.2/solidity/MinterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.2/solidity/MinterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-06-08 07:04:30.000000 cic-contracts-0.3.2/solidity/SealTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      611 2023-06-08 07:04:28.000000 cic-contracts-0.3.2/solidity/SealTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 06:46:14.000000 cic-contracts-0.3.2/solidity/WriterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.2/solidity/WriterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 07:34:25.549978 cic-contracts-0.3.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.2/tests/test_burner.py
--rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-06 12:45:50.000000 cic-contracts-0.3.2/tests/test_capped.py
--rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-06 13:23:05.000000 cic-contracts-0.3.2/tests/test_expire.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.2/tests/test_minter.py
--rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.2/tests/test_seal.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.2/tests/test_writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.3/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-06-08 08:11:27.000000 cic-contracts-0.3.3/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.3/README.md
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.809986 cic-contracts-0.3.3/cic_contracts/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-06-08 12:53:10.000000 cic-contracts-0.3.3/cic_contracts/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.3/cic_contracts/accounts_index.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.3/cic_contracts/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.3/cic_contracts/erc20.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.3/cic_contracts/registry.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.809986 cic-contracts-0.3.3/cic_contracts/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)      303 2023-06-08 12:53:05.000000 cic-contracts-0.3.3/cic_contracts/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      617 2023-02-24 10:28:52.000000 cic-contracts-0.3.3/cic_contracts/unittest/owned.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/cic_contracts/unittest/solidity/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-06 17:11:24.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/BurnerTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/BurnerTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-06 17:11:24.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/CappedTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/CappedTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-06 17:11:24.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/ExpireTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-06 13:56:29.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/ExpireTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-06 17:11:24.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/MinterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/MinterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-06-08 07:04:30.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/SealTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      611 2023-06-08 07:04:28.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/SealTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 06:46:14.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/WriterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.3/cic_contracts/unittest/solidity/WriterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.3/cic_contracts/writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.809986 cic-contracts-0.3.3/cic_contracts.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 13:01:06.000000 cic-contracts-0.3.3/cic_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1986 2023-06-08 13:01:06.000000 cic-contracts-0.3.3/cic_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 13:01:06.000000 cic-contracts-0.3.3/cic_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-08 13:01:06.000000 cic-contracts-0.3.3/cic_contracts.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-08 13:01:06.000000 cic-contracts-0.3.3/cic_contracts.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_burner/
+-rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.3/eth_burner/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.3/eth_burner/burn.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_burner/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 16:41:44.000000 cic-contracts-0.3.3/eth_burner/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1509 2023-06-08 12:58:24.000000 cic-contracts-0.3.3/eth_burner/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      612 2023-06-06 16:43:41.000000 cic-contracts-0.3.3/eth_burner/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_capped/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.3/eth_capped/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.3/eth_capped/capped.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_capped/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 12:09:11.000000 cic-contracts-0.3.3/eth_capped/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2026 2023-06-08 12:53:30.000000 cic-contracts-0.3.3/eth_capped/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1063 2023-06-06 13:45:58.000000 cic-contracts-0.3.3/eth_capped/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_expire/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.3/eth_expire/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.3/eth_expire/expire.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_expire/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 13:21:21.000000 cic-contracts-0.3.3/eth_expire/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2214 2023-06-08 12:58:26.000000 cic-contracts-0.3.3/eth_expire/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      975 2023-06-06 13:44:33.000000 cic-contracts-0.3.3/eth_expire/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_minter/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.3/eth_minter/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.3/eth_minter/minter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_minter/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 14:19:49.000000 cic-contracts-0.3.3/eth_minter/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1555 2023-06-08 12:57:48.000000 cic-contracts-0.3.3/eth_minter/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      618 2023-06-06 14:26:59.000000 cic-contracts-0.3.3/eth_minter/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_seal/
+-rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.3/eth_seal/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.3/eth_seal/seal.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_seal/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-06-08 07:02:18.000000 cic-contracts-0.3.3/eth_seal/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2006 2023-06-08 12:57:46.000000 cic-contracts-0.3.3/eth_seal/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      502 2023-06-08 07:00:50.000000 cic-contracts-0.3.3/eth_seal/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_writer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.3/eth_writer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.3/eth_writer/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/eth_writer/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 17:01:25.000000 cic-contracts-0.3.3/eth_writer/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1908 2023-06-08 12:59:05.000000 cic-contracts-0.3.3/eth_writer/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-06-06 17:11:14.000000 cic-contracts-0.3.3/eth_writer/unittest/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.3/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      962 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.3/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:01:06.813319 cic-contracts-0.3.3/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.3/tests/test_burner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-06 12:45:50.000000 cic-contracts-0.3.3/tests/test_capped.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-06 13:23:05.000000 cic-contracts-0.3.3/tests/test_expire.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.3/tests/test_minter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.3/tests/test_seal.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.3/tests/test_writer.py
```

### Comparing `cic-contracts-0.3.2/LICENSE` & `cic-contracts-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/PKG-INFO` & `cic-contracts-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cic-contracts
-Version: 0.3.2
+Version: 0.3.3
 Summary: CIC network smart contract interfaces
 Home-page: https://gitlab.com/cicnet/cic-contracts
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cic-contracts-0.3.2/README.md` & `cic-contracts-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/cic_contracts/accounts_index.py` & `cic-contracts-0.3.3/cic_contracts/accounts_index.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/cic_contracts/base.py` & `cic-contracts-0.3.3/cic_contracts/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/cic_contracts/erc20.py` & `cic-contracts-0.3.3/cic_contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/cic_contracts/registry.py` & `cic-contracts-0.3.3/cic_contracts/registry.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/cic_contracts/unittest/owned.py` & `cic-contracts-0.3.3/cic_contracts/unittest/owned.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/cic_contracts/writer.py` & `cic-contracts-0.3.3/cic_contracts/writer.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/cic_contracts.egg-info/PKG-INFO` & `cic-contracts-0.3.3/cic_contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cic-contracts
-Version: 0.3.2
+Version: 0.3.3
 Summary: CIC network smart contract interfaces
 Home-page: https://gitlab.com/cicnet/cic-contracts
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cic-contracts-0.3.2/cic_contracts.egg-info/SOURCES.txt` & `cic-contracts-0.3.3/cic_contracts.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 test_requirements.txt
+cic_contracts/__init__.py
 cic_contracts/accounts_index.py
 cic_contracts/base.py
 cic_contracts/erc20.py
 cic_contracts/registry.py
 cic_contracts/writer.py
 cic_contracts.egg-info/PKG-INFO
 cic_contracts.egg-info/SOURCES.txt
 cic_contracts.egg-info/dependency_links.txt
 cic_contracts.egg-info/requires.txt
 cic_contracts.egg-info/top_level.txt
+cic_contracts/unittest/__init__.py
 cic_contracts/unittest/owned.py
+cic_contracts/unittest/solidity/BurnerTest.bin
+cic_contracts/unittest/solidity/BurnerTest.sol
+cic_contracts/unittest/solidity/CappedTest.bin
+cic_contracts/unittest/solidity/CappedTest.sol
+cic_contracts/unittest/solidity/ExpireTest.bin
+cic_contracts/unittest/solidity/ExpireTest.sol
+cic_contracts/unittest/solidity/MinterTest.bin
+cic_contracts/unittest/solidity/MinterTest.sol
+cic_contracts/unittest/solidity/SealTest.bin
+cic_contracts/unittest/solidity/SealTest.sol
+cic_contracts/unittest/solidity/WriterTest.bin
+cic_contracts/unittest/solidity/WriterTest.sol
 eth_burner/__init__.py
 eth_burner/burn.py
 eth_burner/unittest/__init__.py
 eth_burner/unittest/base.py
 eth_burner/unittest/interface.py
 eth_capped/__init__.py
 eth_capped/capped.py
@@ -42,25 +56,13 @@
 eth_seal/unittest/base.py
 eth_seal/unittest/interface.py
 eth_writer/__init__.py
 eth_writer/interface.py
 eth_writer/unittest/__init__.py
 eth_writer/unittest/base.py
 eth_writer/unittest/interface.py
-solidity/BurnerTest.bin
-solidity/BurnerTest.sol
-solidity/CappedTest.bin
-solidity/CappedTest.sol
-solidity/ExpireTest.bin
-solidity/ExpireTest.sol
-solidity/MinterTest.bin
-solidity/MinterTest.sol
-solidity/SealTest.bin
-solidity/SealTest.sol
-solidity/WriterTest.bin
-solidity/WriterTest.sol
 tests/test_burner.py
 tests/test_capped.py
 tests/test_expire.py
 tests/test_minter.py
 tests/test_seal.py
 tests/test_writer.py
```

### Comparing `cic-contracts-0.3.2/eth_burner/burn.py` & `cic-contracts-0.3.3/eth_burner/burn.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_burner/unittest/base.py` & `cic-contracts-0.3.3/eth_capped/unittest/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 # standard imports
 import os
 import logging
-import datetime
 
 # external imports
 from chainlib.eth.unittest.ethtester import EthTesterCase
 from chainlib.connection import RPCConnection
 from chainlib.eth.nonce import RPCNonceOracle
 from chainlib.eth.tx import receipt
 from chainlib.eth.tx import TxFactory
 from chainlib.eth.tx import TxFormat
 from chainlib.eth.contract import ABIContractEncoder
 from chainlib.eth.contract import ABIContractType
-
-# local imports
-from eth_burner import EthBurner
-
-script_dir = os.path.dirname(os.path.realpath(__file__))
-contract_dir = os.path.join(script_dir, '..', '..', 'solidity')
+from cic_contracts.unittest import bytecode
 
 logg = logging.getLogger(__name__)
 
 
-class TestEthBurner(EthTesterCase):
+class TestEthCapped(EthTesterCase):
 
     def setUp(self):
-        super(TestEthBurner, self).setUp()
+        super(TestEthCapped, self).setUp()
+
+        self.set_method = None
 
         self.conn = RPCConnection.connect(self.chain_spec, 'default')
         nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
 
-        f = open(os.path.join(contract_dir, 'BurnerTest.bin'))
-        code = f.read()
-        f.close()
+        code = bytecode('capped')
 
         txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         tx = txf.template(self.accounts[0], None, use_nonce=True)
 
-        self.initial_supply = 1024
+        self.max_supply_value = 1024
         enc = ABIContractEncoder()
-        enc = ABIContractEncoder()
-        enc.uint256(self.initial_supply)
+        enc.uint256(self.max_supply_value)
         args = enc.get()
 
         tx = txf.set_code(tx, code + args)
         (tx_hash_hex, o) = txf.build(tx)
         self.conn.do(o)
         o = receipt(tx_hash_hex)
         r = self.conn.do(o)
         self.assertEqual(r['status'], 1)
         self.address = r['contract_address']
-        logg.debug('published burner test contract with hash {}'.format(r))
+        logg.debug('published capped test contract with hash {}'.format(r))
+
+
+    def set_max_supply(self, contract_address, sender_address, v, tx_format=TxFormat.JSONRPC):
+        nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
+        txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
+        enc = ABIContractEncoder()
+        enc.method('setMaxSupply')
+        enc.typ(ABIContractType.UINT256)
+        enc.uint256(v)
+        data = enc.get()
+        tx = txf.template(sender_address, contract_address, use_nonce=True)
+        tx = txf.set_code(tx, data)
+        tx = txf.finalize(tx, tx_format)
+        return tx
```

### Comparing `cic-contracts-0.3.2/eth_burner/unittest/interface.py` & `cic-contracts-0.3.3/eth_burner/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_capped/capped.py` & `cic-contracts-0.3.3/eth_capped/capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_capped/unittest/base.py` & `cic-contracts-0.3.3/eth_seal/unittest/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,58 +7,53 @@
 from chainlib.connection import RPCConnection
 from chainlib.eth.nonce import RPCNonceOracle
 from chainlib.eth.tx import receipt
 from chainlib.eth.tx import TxFactory
 from chainlib.eth.tx import TxFormat
 from chainlib.eth.contract import ABIContractEncoder
 from chainlib.eth.contract import ABIContractType
+from cic_contracts.unittest import bytecode
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 contract_dir = os.path.join(script_dir, '..', '..', 'solidity')
 
 logg = logging.getLogger(__name__)
 
 
-class TestEthCapped(EthTesterCase):
+class TestEthSeal(EthTesterCase):
 
     def setUp(self):
-        super(TestEthCapped, self).setUp()
+        super(TestEthSeal, self).setUp()
 
         self.set_method = None
 
         self.conn = RPCConnection.connect(self.chain_spec, 'default')
         nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
 
-        f = open(os.path.join(contract_dir, 'CappedTest.bin'))
-        code = f.read()
-        f.close()
+        code = bytecode('seal')
 
         txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         tx = txf.template(self.accounts[0], None, use_nonce=True)
 
-        self.max_supply_value = 1024
-        enc = ABIContractEncoder()
-        enc.uint256(self.max_supply_value)
-        args = enc.get()
-
-        tx = txf.set_code(tx, code + args)
+        self.max_seal_state = 7
+        tx = txf.set_code(tx, code)
         (tx_hash_hex, o) = txf.build(tx)
         self.conn.do(o)
         o = receipt(tx_hash_hex)
         r = self.conn.do(o)
         self.assertEqual(r['status'], 1)
         self.address = r['contract_address']
-        logg.debug('published capped test contract with hash {}'.format(r))
+        logg.debug('published seal test contract with hash {}'.format(r))
 
 
-    def set_max_supply(self, contract_address, sender_address, v, tx_format=TxFormat.JSONRPC):
+    def seal(self, contract_address, sender_address, v, tx_format=TxFormat.JSONRPC):
         nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
         txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         enc = ABIContractEncoder()
-        enc.method('setMaxSupply')
+        enc.method('seal')
         enc.typ(ABIContractType.UINT256)
         enc.uint256(v)
         data = enc.get()
         tx = txf.template(sender_address, contract_address, use_nonce=True)
         tx = txf.set_code(tx, data)
         tx = txf.finalize(tx, tx_format)
         return tx
```

### Comparing `cic-contracts-0.3.2/eth_capped/unittest/interface.py` & `cic-contracts-0.3.3/eth_capped/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_expire/expire.py` & `cic-contracts-0.3.3/eth_expire/expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_expire/unittest/base.py` & `cic-contracts-0.3.3/eth_expire/unittest/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from chainlib.connection import RPCConnection
 from chainlib.eth.nonce import RPCNonceOracle
 from chainlib.eth.tx import receipt
 from chainlib.eth.tx import TxFactory
 from chainlib.eth.tx import TxFormat
 from chainlib.eth.contract import ABIContractEncoder
 from chainlib.eth.contract import ABIContractType
+from cic_contracts.unittest import bytecode
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 contract_dir = os.path.join(script_dir, '..', '..', 'solidity')
 
 logg = logging.getLogger(__name__)
 
 
@@ -23,17 +24,15 @@
 
     def setUp(self):
         super(TestEthExpire, self).setUp()
 
         self.conn = RPCConnection.connect(self.chain_spec, 'default')
         nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
 
-        f = open(os.path.join(contract_dir, 'ExpireTest.bin'))
-        code = f.read()
-        f.close()
+        code = bytecode('expire')
 
         txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         tx = txf.template(self.accounts[0], None, use_nonce=True)
 
         date_expire = datetime.datetime.utcnow() + datetime.timedelta(seconds=10000)
         self.expire = int(date_expire.timestamp())
         enc = ABIContractEncoder()
```

### Comparing `cic-contracts-0.3.2/eth_expire/unittest/interface.py` & `cic-contracts-0.3.3/eth_expire/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_minter/minter.py` & `cic-contracts-0.3.3/eth_minter/minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_minter/unittest/base.py` & `cic-contracts-0.3.3/eth_minter/unittest/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from chainlib.connection import RPCConnection
 from chainlib.eth.nonce import RPCNonceOracle
 from chainlib.eth.tx import receipt
 from chainlib.eth.tx import TxFactory
 from chainlib.eth.tx import TxFormat
 from chainlib.eth.contract import ABIContractEncoder
 from chainlib.eth.contract import ABIContractType
+from cic_contracts.unittest import bytecode
 
 # local imports
 from eth_minter import EthMinter
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 contract_dir = os.path.join(script_dir, '..', '..', 'solidity')
 
@@ -26,17 +27,15 @@
 
     def setUp(self):
         super(TestEthMinter, self).setUp()
 
         self.conn = RPCConnection.connect(self.chain_spec, 'default')
         nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
 
-        f = open(os.path.join(contract_dir, 'MinterTest.bin'))
-        code = f.read()
-        f.close()
+        code = bytecode('minter')
 
         txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         tx = txf.template(self.accounts[0], None, use_nonce=True)
 
         self.initial_supply = 1024
         enc = ABIContractEncoder()
         args = enc.get()
```

### Comparing `cic-contracts-0.3.2/eth_minter/unittest/interface.py` & `cic-contracts-0.3.3/eth_minter/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_seal/seal.py` & `cic-contracts-0.3.3/eth_seal/seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_seal/unittest/base.py` & `cic-contracts-0.3.3/eth_writer/unittest/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,54 +7,51 @@
 from chainlib.connection import RPCConnection
 from chainlib.eth.nonce import RPCNonceOracle
 from chainlib.eth.tx import receipt
 from chainlib.eth.tx import TxFactory
 from chainlib.eth.tx import TxFormat
 from chainlib.eth.contract import ABIContractEncoder
 from chainlib.eth.contract import ABIContractType
+from cic_contracts.unittest import bytecode
+
+# local imports
+from eth_writer import EthWriter
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 contract_dir = os.path.join(script_dir, '..', '..', 'solidity')
 
 logg = logging.getLogger(__name__)
 
 
-class TestEthSeal(EthTesterCase):
+class TestEthWriter(EthTesterCase):
 
     def setUp(self):
-        super(TestEthSeal, self).setUp()
+        super(TestEthWriter, self).setUp()
 
         self.set_method = None
 
         self.conn = RPCConnection.connect(self.chain_spec, 'default')
         nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
 
-        f = open(os.path.join(contract_dir, 'SealTest.bin'))
-        code = f.read()
-        f.close()
+        code = bytecode('writer')
 
         txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         tx = txf.template(self.accounts[0], None, use_nonce=True)
-
-        self.max_seal_state = 7
         tx = txf.set_code(tx, code)
         (tx_hash_hex, o) = txf.build(tx)
         self.conn.do(o)
         o = receipt(tx_hash_hex)
         r = self.conn.do(o)
         self.assertEqual(r['status'], 1)
         self.address = r['contract_address']
-        logg.debug('published seal test contract with hash {}'.format(r))
-
+        self.contracts['writer'] = self.address
+        self.roles['publisher'] = self.accounts[0]
+        self.roles['writer'] = self.accounts[1]
+        logg.debug('published writer test contract with hash {}'.format(r))
+
+        c = EthWriter(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
+        (tx_hash, o) = c.add_writer(self.address, self.accounts[0], self.accounts[0])
+        self.rpc.do(o)
+        o = receipt(tx_hash)
+        r = self.rpc.do(o)
+        self.assertEqual(r['status'], 1)
 
-    def seal(self, contract_address, sender_address, v, tx_format=TxFormat.JSONRPC):
-        nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
-        txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
-        enc = ABIContractEncoder()
-        enc.method('seal')
-        enc.typ(ABIContractType.UINT256)
-        enc.uint256(v)
-        data = enc.get()
-        tx = txf.template(sender_address, contract_address, use_nonce=True)
-        tx = txf.set_code(tx, data)
-        tx = txf.finalize(tx, tx_format)
-        return tx
```

### Comparing `cic-contracts-0.3.2/eth_writer/interface.py` & `cic-contracts-0.3.3/eth_writer/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/eth_writer/unittest/interface.py` & `cic-contracts-0.3.3/eth_writer/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/setup.cfg` & `cic-contracts-0.3.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cic-contracts
-version = 0.3.2
+version = 0.3.3
 description = CIC network smart contract interfaces
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://gitlab.com/cicnet/cic-contracts
 keywords = 
 	dlt
 	blockchain
```

### Comparing `cic-contracts-0.3.2/setup.py` & `cic-contracts-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/BurnerTest.bin` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/BurnerTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/BurnerTest.sol` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/BurnerTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/CappedTest.bin` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/CappedTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/CappedTest.sol` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/CappedTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/ExpireTest.bin` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/ExpireTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/ExpireTest.sol` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/ExpireTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/MinterTest.bin` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/MinterTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/MinterTest.sol` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/MinterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/SealTest.bin` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/SealTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/SealTest.sol` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/SealTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/WriterTest.bin` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/WriterTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/solidity/WriterTest.sol` & `cic-contracts-0.3.3/cic_contracts/unittest/solidity/WriterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/tests/test_burner.py` & `cic-contracts-0.3.3/tests/test_burner.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/tests/test_capped.py` & `cic-contracts-0.3.3/tests/test_capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/tests/test_expire.py` & `cic-contracts-0.3.3/tests/test_expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/tests/test_minter.py` & `cic-contracts-0.3.3/tests/test_minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/tests/test_seal.py` & `cic-contracts-0.3.3/tests/test_seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.2/tests/test_writer.py` & `cic-contracts-0.3.3/tests/test_writer.py`

 * *Files identical despite different names*

