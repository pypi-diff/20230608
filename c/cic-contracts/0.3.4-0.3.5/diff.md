# Comparing `tmp/cic-contracts-0.3.4.tar.gz` & `tmp/cic-contracts-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cic-contracts-0.3.4.tar", last modified: Thu Jun  8 13:40:12 2023, max compression
+gzip compressed data, was "dist/cic-contracts-0.3.5.tar", last modified: Thu Jun  8 15:06:18 2023, max compression
```

## Comparing `cic-contracts-0.3.4.tar` & `cic-contracts-0.3.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.4/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-06-08 08:11:27.000000 cic-contracts-0.3.4/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.4/README.md
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.876638 cic-contracts-0.3.4/cic_contracts/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-06-08 12:53:10.000000 cic-contracts-0.3.4/cic_contracts/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.4/cic_contracts/accounts_index.py
--rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.4/cic_contracts/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.4/cic_contracts/erc20.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.4/cic_contracts/registry.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.876638 cic-contracts-0.3.4/cic_contracts/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)      303 2023-06-08 12:53:05.000000 cic-contracts-0.3.4/cic_contracts/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      617 2023-02-24 10:28:52.000000 cic-contracts-0.3.4/cic_contracts/unittest/owned.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.876638 cic-contracts-0.3.4/cic_contracts/unittest/solidity/
--rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-06 17:11:24.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/BurnerTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/BurnerTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-06 17:11:24.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/CappedTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/CappedTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-06 17:11:24.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/ExpireTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-06 13:56:29.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/ExpireTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-06 17:11:24.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/MinterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/MinterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-06-08 07:04:30.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/SealTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      611 2023-06-08 07:04:28.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/SealTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 06:46:14.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/WriterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.4/cic_contracts/unittest/solidity/WriterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.4/cic_contracts/writer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.876638 cic-contracts-0.3.4/cic_contracts.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 13:40:12.000000 cic-contracts-0.3.4/cic_contracts.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1986 2023-06-08 13:40:12.000000 cic-contracts-0.3.4/cic_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 13:40:12.000000 cic-contracts-0.3.4/cic_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-08 13:40:12.000000 cic-contracts-0.3.4/cic_contracts.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-08 13:40:12.000000 cic-contracts-0.3.4/cic_contracts.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.876638 cic-contracts-0.3.4/eth_burner/
--rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.4/eth_burner/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.4/eth_burner/burn.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.876638 cic-contracts-0.3.4/eth_burner/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 16:41:44.000000 cic-contracts-0.3.4/eth_burner/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1509 2023-06-08 12:58:24.000000 cic-contracts-0.3.4/eth_burner/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      613 2023-06-08 13:23:00.000000 cic-contracts-0.3.4/eth_burner/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.876638 cic-contracts-0.3.4/eth_capped/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.4/eth_capped/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.4/eth_capped/capped.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.876638 cic-contracts-0.3.4/eth_capped/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 12:09:11.000000 cic-contracts-0.3.4/eth_capped/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2091 2023-06-08 13:25:50.000000 cic-contracts-0.3.4/eth_capped/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1069 2023-06-08 13:32:19.000000 cic-contracts-0.3.4/eth_capped/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/eth_expire/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.4/eth_expire/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.4/eth_expire/expire.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/eth_expire/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 13:21:21.000000 cic-contracts-0.3.4/eth_expire/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2214 2023-06-08 12:58:26.000000 cic-contracts-0.3.4/eth_expire/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      975 2023-06-06 13:44:33.000000 cic-contracts-0.3.4/eth_expire/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/eth_minter/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.4/eth_minter/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.4/eth_minter/minter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/eth_minter/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 14:19:49.000000 cic-contracts-0.3.4/eth_minter/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1555 2023-06-08 12:57:48.000000 cic-contracts-0.3.4/eth_minter/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      618 2023-06-06 14:26:59.000000 cic-contracts-0.3.4/eth_minter/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/eth_seal/
--rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.4/eth_seal/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.4/eth_seal/seal.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/eth_seal/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-06-08 07:02:18.000000 cic-contracts-0.3.4/eth_seal/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2006 2023-06-08 12:57:46.000000 cic-contracts-0.3.4/eth_seal/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      502 2023-06-08 07:00:50.000000 cic-contracts-0.3.4/eth_seal/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/eth_writer/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.4/eth_writer/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.4/eth_writer/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/eth_writer/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 17:01:25.000000 cic-contracts-0.3.4/eth_writer/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1908 2023-06-08 12:59:05.000000 cic-contracts-0.3.4/eth_writer/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-06-06 17:11:14.000000 cic-contracts-0.3.4/eth_writer/unittest/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.4/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      962 2023-06-08 13:40:12.883305 cic-contracts-0.3.4/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.4/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.4/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 13:40:12.879972 cic-contracts-0.3.4/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.4/tests/test_burner.py
--rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-08 13:23:46.000000 cic-contracts-0.3.4/tests/test_capped.py
--rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-06 13:23:05.000000 cic-contracts-0.3.4/tests/test_expire.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.4/tests/test_minter.py
--rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.4/tests/test_seal.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.4/tests/test_writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-06-08 08:11:27.000000 cic-contracts-0.3.5/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.5/README.md
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.353323 cic-contracts-0.3.5/cic_contracts/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-06-08 12:53:10.000000 cic-contracts-0.3.5/cic_contracts/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/accounts_index.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/erc20.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/registry.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/cic_contracts/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)      303 2023-06-08 12:53:05.000000 cic-contracts-0.3.5/cic_contracts/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      617 2023-02-24 10:28:52.000000 cic-contracts-0.3.5/cic_contracts/unittest/owned.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/cic_contracts/unittest/solidity/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-08 15:04:59.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/BurnerTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/BurnerTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-08 15:04:59.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/CappedTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/CappedTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-08 15:05:00.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/ExpireTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-08 14:58:25.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/ExpireTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-08 15:05:00.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/MinterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/MinterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-06-08 15:05:00.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/SealTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      611 2023-06-08 07:04:28.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/SealTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 15:05:00.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/WriterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/WriterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/cic_contracts.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1986 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/eth_burner/
+-rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.5/eth_burner/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.5/eth_burner/burn.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/eth_burner/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 16:41:44.000000 cic-contracts-0.3.5/eth_burner/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1509 2023-06-08 12:58:24.000000 cic-contracts-0.3.5/eth_burner/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      613 2023-06-08 13:23:00.000000 cic-contracts-0.3.5/eth_burner/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_capped/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.5/eth_capped/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.5/eth_capped/capped.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_capped/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 12:09:11.000000 cic-contracts-0.3.5/eth_capped/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2091 2023-06-08 13:25:50.000000 cic-contracts-0.3.5/eth_capped/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1069 2023-06-08 13:32:19.000000 cic-contracts-0.3.5/eth_capped/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_expire/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.5/eth_expire/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.5/eth_expire/expire.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_expire/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 13:21:21.000000 cic-contracts-0.3.5/eth_expire/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2226 2023-06-08 14:46:09.000000 cic-contracts-0.3.5/eth_expire/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1005 2023-06-08 14:54:26.000000 cic-contracts-0.3.5/eth_expire/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_minter/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.5/eth_minter/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.5/eth_minter/minter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_minter/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 14:19:49.000000 cic-contracts-0.3.5/eth_minter/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1555 2023-06-08 12:57:48.000000 cic-contracts-0.3.5/eth_minter/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      618 2023-06-06 14:26:59.000000 cic-contracts-0.3.5/eth_minter/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_seal/
+-rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.5/eth_seal/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.5/eth_seal/seal.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_seal/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-06-08 07:02:18.000000 cic-contracts-0.3.5/eth_seal/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2006 2023-06-08 12:57:46.000000 cic-contracts-0.3.5/eth_seal/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      502 2023-06-08 07:00:50.000000 cic-contracts-0.3.5/eth_seal/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_writer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.5/eth_writer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.5/eth_writer/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/eth_writer/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 17:01:25.000000 cic-contracts-0.3.5/eth_writer/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1908 2023-06-08 12:59:05.000000 cic-contracts-0.3.5/eth_writer/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-06-06 17:11:14.000000 cic-contracts-0.3.5/eth_writer/unittest/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.5/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      962 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.5/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.5/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.5/tests/test_burner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-08 13:23:46.000000 cic-contracts-0.3.5/tests/test_capped.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-08 14:56:41.000000 cic-contracts-0.3.5/tests/test_expire.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.5/tests/test_minter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.5/tests/test_seal.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.5/tests/test_writer.py
```

### Comparing `cic-contracts-0.3.4/LICENSE` & `cic-contracts-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/PKG-INFO` & `cic-contracts-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cic-contracts
-Version: 0.3.4
+Version: 0.3.5
 Summary: CIC network smart contract interfaces
 Home-page: https://gitlab.com/cicnet/cic-contracts
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cic-contracts-0.3.4/README.md` & `cic-contracts-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/accounts_index.py` & `cic-contracts-0.3.5/cic_contracts/accounts_index.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/base.py` & `cic-contracts-0.3.5/cic_contracts/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/erc20.py` & `cic-contracts-0.3.5/cic_contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/registry.py` & `cic-contracts-0.3.5/cic_contracts/registry.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/owned.py` & `cic-contracts-0.3.5/cic_contracts/unittest/owned.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/BurnerTest.bin` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/BurnerTest.bin`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-608060405234801561001057600080fd5b5060405161070438038061070483398181016040528101906100329190610081565b8060008190555080600281905550506100ae565b600080fd5b6000819050919050565b61005e8161004b565b811461006957600080fd5b50565b60008151905061007b81610055565b92915050565b60006020828403121561009757610096610046565b5b60006100a58482850161006c565b91505092915050565b610647806100bd6000396000f3fe608060405234801561001057600080fd5b506004361061007f576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461008457806342966c68146100b457806344d17187146100e457806344df8e7014610100578063a2309ff81461011e578063d89135cd1461013c575b600080fd5b61009e60048036038101906100999190610353565b61015a565b6040516100ab919061039b565b60405180910390f35b6100ce60048036038101906100c991906103ec565b61020a565b6040516100db919061039b565b60405180910390f35b6100fe60048036038101906100f991906104dc565b61021f565b005b61010861022f565b604051610115919061055f565b60405180910390f35b610126610241565b604051610133919061055f565b60405180910390f35b610144610247565b604051610151919061055f565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101ae5760019050610205565b63bc4babdd7c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036102005760019050610205565b600090505b919050565b60006102158261024d565b5060019050919050565b6102288361020a565b5050505050565b600061023c60005461024d565b905090565b60005481565b60015481565b6000808260025461025e91906105a9565b101561026957600080fd5b816001600082825461027b91906105dd565b92505081905550816002600082825461029491906105a9565b925050819055503373ffffffffffffffffffffffffffffffffffffffff167fcc16f5dbb4873280815c1ee09dbd06736cffcc184412cf7a71a0fdb75d397ca5836040516102e1919061055f565b60405180910390a2819050919050565b600080fd5b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610330816102fb565b811461033b57600080fd5b50565b60008135905061034d81610327565b92915050565b600060208284031215610369576103686102f1565b5b60006103778482850161033e565b91505092915050565b60008115159050919050565b61039581610380565b82525050565b60006020820190506103b0600083018461038c565b92915050565b6000819050919050565b6103c9816103b6565b81146103d457600080fd5b50565b6000813590506103e6816103c0565b92915050565b600060208284031215610402576104016102f1565b5b6000610410848285016103d7565b91505092915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b600061044482610419565b9050919050565b61045481610439565b811461045f57600080fd5b50565b6000813590506104718161044b565b92915050565b600080fd5b600080fd5b600080fd5b60008083601f84011261049c5761049b610477565b5b8235905067ffffffffffffffff8111156104b9576104b861047c565b5b6020830191508360018202830111156104d5576104d4610481565b5b9250929050565b600080600080606085870312156104f6576104f56102f1565b5b600061050487828801610462565b9450506020610515878288016103d7565b935050604085013567ffffffffffffffff811115610536576105356102f6565b5b61054287828801610486565b925092505092959194509250565b610559816103b6565b82525050565b60006020820190506105746000830184610550565b92915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b60006105b4826103b6565b91506105bf836103b6565b92508282039050818111156105d7576105d661057a565b5b92915050565b60006105e8826103b6565b91506105f3836103b6565b925082820190508082111561060b5761060a61057a565b5b9291505056fea2646970667358221220cf04ca2f9a9ef1aee6a7109799862035ae01e772554ee9c71f0ca5243159197164736f6c63430008130033
+608060405234801561001057600080fd5b5060405161070438038061070483398181016040528101906100329190610081565b8060008190555080600281905550506100ae565b600080fd5b6000819050919050565b61005e8161004b565b811461006957600080fd5b50565b60008151905061007b81610055565b92915050565b60006020828403121561009757610096610046565b5b60006100a58482850161006c565b91505092915050565b610647806100bd6000396000f3fe608060405234801561001057600080fd5b506004361061007f576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461008457806342966c68146100b457806344d17187146100e457806344df8e7014610100578063a2309ff81461011e578063d89135cd1461013c575b600080fd5b61009e60048036038101906100999190610353565b61015a565b6040516100ab919061039b565b60405180910390f35b6100ce60048036038101906100c991906103ec565b61020a565b6040516100db919061039b565b60405180910390f35b6100fe60048036038101906100f991906104dc565b61021f565b005b61010861022f565b604051610115919061055f565b60405180910390f35b610126610241565b604051610133919061055f565b60405180910390f35b610144610247565b604051610151919061055f565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101ae5760019050610205565b63bc4babdd7c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036102005760019050610205565b600090505b919050565b60006102158261024d565b5060019050919050565b6102288361020a565b5050505050565b600061023c60005461024d565b905090565b60005481565b60015481565b6000808260025461025e91906105a9565b101561026957600080fd5b816001600082825461027b91906105dd565b92505081905550816002600082825461029491906105a9565b925050819055503373ffffffffffffffffffffffffffffffffffffffff167fcc16f5dbb4873280815c1ee09dbd06736cffcc184412cf7a71a0fdb75d397ca5836040516102e1919061055f565b60405180910390a2819050919050565b600080fd5b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610330816102fb565b811461033b57600080fd5b50565b60008135905061034d81610327565b92915050565b600060208284031215610369576103686102f1565b5b60006103778482850161033e565b91505092915050565b60008115159050919050565b61039581610380565b82525050565b60006020820190506103b0600083018461038c565b92915050565b6000819050919050565b6103c9816103b6565b81146103d457600080fd5b50565b6000813590506103e6816103c0565b92915050565b600060208284031215610402576104016102f1565b5b6000610410848285016103d7565b91505092915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b600061044482610419565b9050919050565b61045481610439565b811461045f57600080fd5b50565b6000813590506104718161044b565b92915050565b600080fd5b600080fd5b600080fd5b60008083601f84011261049c5761049b610477565b5b8235905067ffffffffffffffff8111156104b9576104b861047c565b5b6020830191508360018202830111156104d5576104d4610481565b5b9250929050565b600080600080606085870312156104f6576104f56102f1565b5b600061050487828801610462565b9450506020610515878288016103d7565b935050604085013567ffffffffffffffff811115610536576105356102f6565b5b61054287828801610486565b925092505092959194509250565b610559816103b6565b82525050565b60006020820190506105746000830184610550565b92915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b60006105b4826103b6565b91506105bf836103b6565b92508282039050818111156105d7576105d661057a565b5b92915050565b60006105e8826103b6565b91506105f3836103b6565b925082820190508082111561060b5761060a61057a565b5b9291505056fea26469706673582212208cc8e912e94a09c49f6772a6a0bfcea389d65478dcee0b3e12fa669028b5567e64736f6c63430008130033
```

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/BurnerTest.sol` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/BurnerTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/CappedTest.bin` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/CappedTest.bin`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-608060405234801561001057600080fd5b506040516104003803806104008339818101604052810190610032919061007a565b80600081905550506100a7565b600080fd5b6000819050919050565b61005781610044565b811461006257600080fd5b50565b6000815190506100748161004e565b92915050565b6000602082840312156100905761008f61003f565b5b600061009e84828501610065565b91505092915050565b61034a806100b66000396000f3fe608060405234801561001057600080fd5b506004361061005e576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a7146100635780636f8b44b014610093578063d5abeb01146100af575b600080fd5b61007d60048036038101906100789190610224565b6100cd565b60405161008a919061026c565b60405180910390f35b6100ad60048036038101906100a891906102bd565b61017d565b005b6100b76101c1565b6040516100c491906102f9565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101215760019050610178565b63869f75947c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101735760019050610178565b600090505b919050565b6000547f9722adea12ab7ef86fc45b88f0e0b567639e8dddaae60261e08c03d747fbbfe6826040516101af91906102f9565b60405180910390a28060008190555050565b60005481565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610201816101cc565b811461020c57600080fd5b50565b60008135905061021e816101f8565b92915050565b60006020828403121561023a576102396101c7565b5b60006102488482850161020f565b91505092915050565b60008115159050919050565b61026681610251565b82525050565b6000602082019050610281600083018461025d565b92915050565b6000819050919050565b61029a81610287565b81146102a557600080fd5b50565b6000813590506102b781610291565b92915050565b6000602082840312156102d3576102d26101c7565b5b60006102e1848285016102a8565b91505092915050565b6102f381610287565b82525050565b600060208201905061030e60008301846102ea565b9291505056fea2646970667358221220f6bc26e7c6827142ccee8c0cadc8cb76d33712a68eacd67b69e4f8108aa2b59064736f6c63430008130033
+608060405234801561001057600080fd5b506040516104003803806104008339818101604052810190610032919061007a565b80600081905550506100a7565b600080fd5b6000819050919050565b61005781610044565b811461006257600080fd5b50565b6000815190506100748161004e565b92915050565b6000602082840312156100905761008f61003f565b5b600061009e84828501610065565b91505092915050565b61034a806100b66000396000f3fe608060405234801561001057600080fd5b506004361061005e576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a7146100635780636f8b44b014610093578063d5abeb01146100af575b600080fd5b61007d60048036038101906100789190610224565b6100cd565b60405161008a919061026c565b60405180910390f35b6100ad60048036038101906100a891906102bd565b61017d565b005b6100b76101c1565b6040516100c491906102f9565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101215760019050610178565b63869f75947c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101735760019050610178565b600090505b919050565b6000547f9722adea12ab7ef86fc45b88f0e0b567639e8dddaae60261e08c03d747fbbfe6826040516101af91906102f9565b60405180910390a28060008190555050565b60005481565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610201816101cc565b811461020c57600080fd5b50565b60008135905061021e816101f8565b92915050565b60006020828403121561023a576102396101c7565b5b60006102488482850161020f565b91505092915050565b60008115159050919050565b61026681610251565b82525050565b6000602082019050610281600083018461025d565b92915050565b6000819050919050565b61029a81610287565b81146102a557600080fd5b50565b6000813590506102b781610291565b92915050565b6000602082840312156102d3576102d26101c7565b5b60006102e1848285016102a8565b91505092915050565b6102f381610287565b82525050565b600060208201905061030e60008301846102ea565b9291505056fea26469706673582212202fae6928974c7d7b0aa39737c7a191972db33126d9966e893091aac145fd34c864736f6c63430008130033
```

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/CappedTest.sol` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/CappedTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/ExpireTest.bin` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/MinterTest.bin`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-608060405234801561001057600080fd5b506040516105143803806105148339818101604052810190610032919061007a565b80600081905550506100a7565b600080fd5b6000819050919050565b61005781610044565b811461006257600080fd5b50565b6000815190506100748161004e565b92915050565b6000602082840312156100905761008f61003f565b5b600061009e84828501610065565b91505092915050565b61045e806100b66000396000f3fe608060405234801561001057600080fd5b5060043610610069576000357c01000000000000000000000000000000000000000000000000000000009004806301cceb381461006e57806301ffc9a71461008a5780635f408c04146100ba578063b1cb0db3146100d8575b600080fd5b610088600480360381019061008391906102df565b6100f6565b005b6100a4600480360381019061009f9190610364565b610162565b6040516100b191906103ac565b60405180910390f35b6100c2610212565b6040516100cf91906103e3565b60405180910390f35b6100e061029e565b6040516100ed919061040d565b60405180910390f35b600160009054906101000a900460ff161561011057600080fd5b600054811161011e57600080fd5b6000547ff5bd6cb27a0006b5ea8618058a0d84719695cb6d984f4840bc1a54ca12ae4b7c82604051610150919061040d565b60405180910390a28060008190555050565b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101b6576001905061020d565b63841a0e947c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191603610208576001905061020d565b600090505b919050565b6000600160009054906101000a900460ff1615610232576001905061029b565b600054421015610245576000905061029b565b60018060006101000a81548160ff0219169083151502179055507ff80dbaea4785589e52984ca36a31de106adc77759539a5c7d92883bf49692fe94260405161028e919061040d565b60405180910390a1600190505b90565b60005481565b600080fd5b6000819050919050565b6102bc816102a9565b81146102c757600080fd5b50565b6000813590506102d9816102b3565b92915050565b6000602082840312156102f5576102f46102a4565b5b6000610303848285016102ca565b91505092915050565b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b6103418161030c565b811461034c57600080fd5b50565b60008135905061035e81610338565b92915050565b60006020828403121561037a576103796102a4565b5b60006103888482850161034f565b91505092915050565b60008115159050919050565b6103a681610391565b82525050565b60006020820190506103c1600083018461039d565b92915050565b600060ff82169050919050565b6103dd816103c7565b82525050565b60006020820190506103f860008301846103d4565b92915050565b610407816102a9565b82525050565b600060208201905061042260008301846103fe565b9291505056fea264697066735822122008d6e0c184036b44d56435108c0e081869b445ea32edbcd7035807691a26a11264736f6c63430008130033
+608060405234801561001057600080fd5b50610653806100206000396000f3fe608060405234801561001057600080fd5b5060043610610074576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a714610079578063449a52f8146100a95780638832e6e3146100d957806394d008ef146100f5578063e3d670d714610111575b600080fd5b610093600480360381019061008e9190610353565b610141565b6040516100a0919061039b565b60405180910390f35b6100c360048036038101906100be919061044a565b6101f1565b6040516100d0919061039b565b60405180910390f35b6100f360048036038101906100ee91906104ef565b6102b7565b005b61010f600480360381019061010a91906104ef565b6102c8565b005b61012b60048036038101906101269190610563565b6102d9565b604051610138919061059f565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361019557600190506101ec565b635878bcf47c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101e757600190506101ec565b600090505b919050565b6000816000808573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff168152602001908152602001600020600082825461024191906105e9565b925050819055508273ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff167fab8530f87dc9b59234c4623bf917212bb2536d647574c8e7e5da92c2ede0c9f8846040516102a5919061059f565b60405180910390a36001905092915050565b6102c184846101f1565b5050505050565b6102d284846101f1565b5050505050565b60006020528060005260406000206000915090505481565b600080fd5b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610330816102fb565b811461033b57600080fd5b50565b60008135905061034d81610327565b92915050565b600060208284031215610369576103686102f1565b5b60006103778482850161033e565b91505092915050565b60008115159050919050565b61039581610380565b82525050565b60006020820190506103b0600083018461038c565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006103e1826103b6565b9050919050565b6103f1816103d6565b81146103fc57600080fd5b50565b60008135905061040e816103e8565b92915050565b6000819050919050565b61042781610414565b811461043257600080fd5b50565b6000813590506104448161041e565b92915050565b60008060408385031215610461576104606102f1565b5b600061046f858286016103ff565b925050602061048085828601610435565b9150509250929050565b600080fd5b600080fd5b600080fd5b60008083601f8401126104af576104ae61048a565b5b8235905067ffffffffffffffff8111156104cc576104cb61048f565b5b6020830191508360018202830111156104e8576104e7610494565b5b9250929050565b60008060008060608587031215610509576105086102f1565b5b6000610517878288016103ff565b945050602061052887828801610435565b935050604085013567ffffffffffffffff811115610549576105486102f6565b5b61055587828801610499565b925092505092959194509250565b600060208284031215610579576105786102f1565b5b6000610587848285016103ff565b91505092915050565b61059981610414565b82525050565b60006020820190506105b46000830184610590565b92915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b60006105f482610414565b91506105ff83610414565b9250828201905080821115610617576106166105ba565b5b9291505056fea2646970667358221220c34bf6d363f42169041e40ea19aaa4d82e75186dffd29b11557323de4adfbad564736f6c63430008130033
```

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/ExpireTest.sol` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/ExpireTest.sol`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	event Expired(uint256 _timestamp);
 	event ExpiryChange(uint256 indexed _oldTimestamp, uint256 _newTimestamp);
 
 	constructor(uint256 _timestamp) {
 		expires = _timestamp;
 	}
 
-	function setExpiry(uint256 _timestamp) public {
+	function setExpire(uint256 _timestamp) public {
 		require(!expired);
 		require(_timestamp > expires);
 		emit ExpiryChange(expires, _timestamp);
 		expires = _timestamp;
 	}
 
 	function applyExpiry() public returns(uint8) {
```

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/MinterTest.bin` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/WriterTest.bin`

 * *Files 20% similar despite different names*

```diff
@@ -1 +1 @@
-608060405234801561001057600080fd5b50610653806100206000396000f3fe608060405234801561001057600080fd5b5060043610610074576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a714610079578063449a52f8146100a95780638832e6e3146100d957806394d008ef146100f5578063e3d670d714610111575b600080fd5b610093600480360381019061008e9190610353565b610141565b6040516100a0919061039b565b60405180910390f35b6100c360048036038101906100be919061044a565b6101f1565b6040516100d0919061039b565b60405180910390f35b6100f360048036038101906100ee91906104ef565b6102b7565b005b61010f600480360381019061010a91906104ef565b6102c8565b005b61012b60048036038101906101269190610563565b6102d9565b604051610138919061059f565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361019557600190506101ec565b635878bcf47c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101e757600190506101ec565b600090505b919050565b6000816000808573ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff168152602001908152602001600020600082825461024191906105e9565b925050819055508273ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff167fab8530f87dc9b59234c4623bf917212bb2536d647574c8e7e5da92c2ede0c9f8846040516102a5919061059f565b60405180910390a36001905092915050565b6102c184846101f1565b5050505050565b6102d284846101f1565b5050505050565b60006020528060005260406000206000915090505481565b600080fd5b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610330816102fb565b811461033b57600080fd5b50565b60008135905061034d81610327565b92915050565b600060208284031215610369576103686102f1565b5b60006103778482850161033e565b91505092915050565b60008115159050919050565b61039581610380565b82525050565b60006020820190506103b0600083018461038c565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006103e1826103b6565b9050919050565b6103f1816103d6565b81146103fc57600080fd5b50565b60008135905061040e816103e8565b92915050565b6000819050919050565b61042781610414565b811461043257600080fd5b50565b6000813590506104448161041e565b92915050565b60008060408385031215610461576104606102f1565b5b600061046f858286016103ff565b925050602061048085828601610435565b9150509250929050565b600080fd5b600080fd5b600080fd5b60008083601f8401126104af576104ae61048a565b5b8235905067ffffffffffffffff8111156104cc576104cb61048f565b5b6020830191508360018202830111156104e8576104e7610494565b5b9250929050565b60008060008060608587031215610509576105086102f1565b5b6000610517878288016103ff565b945050602061052887828801610435565b935050604085013567ffffffffffffffff811115610549576105486102f6565b5b61055587828801610499565b925092505092959194509250565b600060208284031215610579576105786102f1565b5b6000610587848285016103ff565b91505092915050565b61059981610414565b82525050565b60006020820190506105b46000830184610590565b92915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b60006105f482610414565b91506105ff83610414565b9250828201905080821115610617576106166105ba565b5b9291505056fea2646970667358221220a5a810b6de36b1154b4b2d37d08d4e8a5fe442c870cd58cdba0d86a13da3dda964736f6c63430008130033
+608060405234801561001057600080fd5b506104da806100206000396000f3fe608060405234801561001057600080fd5b5060043610610069576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461006e5780632b29ba231461009e5780635ae06f7e146100ce578063da2824a8146100fe575b600080fd5b6100886004803603810190610083919061038c565b61012e565b60405161009591906103d4565b60405180910390f35b6100b860048036038101906100b3919061044d565b6101de565b6040516100c591906103d4565b60405180910390f35b6100e860048036038101906100e3919061044d565b6101fe565b6040516100f591906103d4565b60405180910390f35b6101186004803603810190610113919061044d565b610296565b60405161012591906103d4565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361018257600190506101d9565b63abe1f1f57c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101d457600190506101d9565b600090505b919050565b60006020528060005260406000206000915054906101000a900460ff1681565b6000806000808473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548160ff0219169083151502179055507f9002f14780245e47491e7a2caae4712e7cea2e298e4e76c6916845145b90a51c826040516102859190610489565b60405180910390a160019050919050565b600060016000808473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548160ff0219169083151502179055507f6ff3aa2ea7b53070f6d9d07a445d338d89e8edef44250ffa8be19f53910d4a2e8260405161031e9190610489565b60405180910390a160019050919050565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b61036981610334565b811461037457600080fd5b50565b60008135905061038681610360565b92915050565b6000602082840312156103a2576103a161032f565b5b60006103b084828501610377565b91505092915050565b60008115159050919050565b6103ce816103b9565b82525050565b60006020820190506103e960008301846103c5565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b600061041a826103ef565b9050919050565b61042a8161040f565b811461043557600080fd5b50565b60008135905061044781610421565b92915050565b6000602082840312156104635761046261032f565b5b600061047184828501610438565b91505092915050565b6104838161040f565b82525050565b600060208201905061049e600083018461047a565b9291505056fea264697066735822122020b67ff87e5eb051bb72e8e0a6d713bfca71e048393fa9cf2024224ab72bf93164736f6c63430008130033
```

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/MinterTest.sol` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/MinterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/SealTest.bin` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/SealTest.bin`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-6080604052600760015534801561001557600080fd5b50610355806100256000396000f3fe608060405234801561001057600080fd5b5060043610610069576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461006e57806318cbbcfc1461009e57806331a5995d146100bc57806386fe212d146100da575b600080fd5b6100886004803603810190610083919061022f565b6100f6565b6040516100959190610277565b60405180910390f35b6100a66101a6565b6040516100b391906102ab565b60405180910390f35b6100c46101ac565b6040516100d191906102ab565b60405180910390f35b6100f460048036038101906100ef91906102f2565b6101b2565b005b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361014a57600190506101a1565b630d7491f87c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361019c57600190506101a1565b600090505b919050565b60015481565b60005481565b60015481106101c057600080fd5b80600080828254179250508190555050565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b61020c816101d7565b811461021757600080fd5b50565b60008135905061022981610203565b92915050565b600060208284031215610245576102446101d2565b5b60006102538482850161021a565b91505092915050565b60008115159050919050565b6102718161025c565b82525050565b600060208201905061028c6000830184610268565b92915050565b6000819050919050565b6102a581610292565b82525050565b60006020820190506102c0600083018461029c565b92915050565b6102cf81610292565b81146102da57600080fd5b50565b6000813590506102ec816102c6565b92915050565b600060208284031215610308576103076101d2565b5b6000610316848285016102dd565b9150509291505056fea26469706673582212208356fec8f4fc7719bf58ea1be5e22cf56cadb8367918f5b4e0a90cad23396bb064736f6c63430008130033
+6080604052600760015534801561001557600080fd5b50610355806100256000396000f3fe608060405234801561001057600080fd5b5060043610610069576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461006e57806318cbbcfc1461009e57806331a5995d146100bc57806386fe212d146100da575b600080fd5b6100886004803603810190610083919061022f565b6100f6565b6040516100959190610277565b60405180910390f35b6100a66101a6565b6040516100b391906102ab565b60405180910390f35b6100c46101ac565b6040516100d191906102ab565b60405180910390f35b6100f460048036038101906100ef91906102f2565b6101b2565b005b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361014a57600190506101a1565b630d7491f87c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361019c57600190506101a1565b600090505b919050565b60015481565b60005481565b60015481106101c057600080fd5b80600080828254179250508190555050565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b61020c816101d7565b811461021757600080fd5b50565b60008135905061022981610203565b92915050565b600060208284031215610245576102446101d2565b5b60006102538482850161021a565b91505092915050565b60008115159050919050565b6102718161025c565b82525050565b600060208201905061028c6000830184610268565b92915050565b6000819050919050565b6102a581610292565b82525050565b60006020820190506102c0600083018461029c565b92915050565b6102cf81610292565b81146102da57600080fd5b50565b6000813590506102ec816102c6565b92915050565b600060208284031215610308576103076101d2565b5b6000610316848285016102dd565b9150509291505056fea2646970667358221220b3e52e50248018ee0796b0edf7d8a7660203424ceeafb7d1dd857819fab5037d64736f6c63430008130033
```

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/SealTest.sol` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/SealTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/WriterTest.bin` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/ExpireTest.bin`

 * *Files 22% similar despite different names*

```diff
@@ -1 +1 @@
-608060405234801561001057600080fd5b506104da806100206000396000f3fe608060405234801561001057600080fd5b5060043610610069576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461006e5780632b29ba231461009e5780635ae06f7e146100ce578063da2824a8146100fe575b600080fd5b6100886004803603810190610083919061038c565b61012e565b60405161009591906103d4565b60405180910390f35b6100b860048036038101906100b3919061044d565b6101de565b6040516100c591906103d4565b60405180910390f35b6100e860048036038101906100e3919061044d565b6101fe565b6040516100f591906103d4565b60405180910390f35b6101186004803603810190610113919061044d565b610296565b60405161012591906103d4565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361018257600190506101d9565b63abe1f1f57c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916036101d457600190506101d9565b600090505b919050565b60006020528060005260406000206000915054906101000a900460ff1681565b6000806000808473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548160ff0219169083151502179055507f9002f14780245e47491e7a2caae4712e7cea2e298e4e76c6916845145b90a51c826040516102859190610489565b60405180910390a160019050919050565b600060016000808473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548160ff0219169083151502179055507f6ff3aa2ea7b53070f6d9d07a445d338d89e8edef44250ffa8be19f53910d4a2e8260405161031e9190610489565b60405180910390a160019050919050565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b61036981610334565b811461037457600080fd5b50565b60008135905061038681610360565b92915050565b6000602082840312156103a2576103a161032f565b5b60006103b084828501610377565b91505092915050565b60008115159050919050565b6103ce816103b9565b82525050565b60006020820190506103e960008301846103c5565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b600061041a826103ef565b9050919050565b61042a8161040f565b811461043557600080fd5b50565b60008135905061044781610421565b92915050565b6000602082840312156104635761046261032f565b5b600061047184828501610438565b91505092915050565b6104838161040f565b82525050565b600060208201905061049e600083018461047a565b9291505056fea26469706673582212206bef2d3402160122da272241da7b2729136d4bc1e4399f01ddd8c8a7d3b93cdd64736f6c63430008130033
+608060405234801561001057600080fd5b506040516105143803806105148339818101604052810190610032919061007a565b80600081905550506100a7565b600080fd5b6000819050919050565b61005781610044565b811461006257600080fd5b50565b6000815190506100748161004e565b92915050565b6000602082840312156100905761008f61003f565b5b600061009e84828501610065565b91505092915050565b61045e806100b66000396000f3fe608060405234801561001057600080fd5b5060043610610069576000357c01000000000000000000000000000000000000000000000000000000009004806301ffc9a71461006e57806332c270521461009e5780635f408c04146100ba578063b1cb0db3146100d8575b600080fd5b61008860048036038101906100839190610301565b6100f6565b6040516100959190610349565b60405180910390f35b6100b860048036038101906100b3919061039a565b6101a6565b005b6100c2610212565b6040516100cf91906103e3565b60405180910390f35b6100e061029e565b6040516100ed919061040d565b60405180910390f35b60006301ffc9a77c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361014a57600190506101a1565b63841a0e947c010000000000000000000000000000000000000000000000000000000002827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff19160361019c57600190506101a1565b600090505b919050565b600160009054906101000a900460ff16156101c057600080fd5b60005481116101ce57600080fd5b6000547ff5bd6cb27a0006b5ea8618058a0d84719695cb6d984f4840bc1a54ca12ae4b7c82604051610200919061040d565b60405180910390a28060008190555050565b6000600160009054906101000a900460ff1615610232576001905061029b565b600054421015610245576000905061029b565b60018060006101000a81548160ff0219169083151502179055507ff80dbaea4785589e52984ca36a31de106adc77759539a5c7d92883bf49692fe94260405161028e919061040d565b60405180910390a1600190505b90565b60005481565b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b6102de816102a9565b81146102e957600080fd5b50565b6000813590506102fb816102d5565b92915050565b600060208284031215610317576103166102a4565b5b6000610325848285016102ec565b91505092915050565b60008115159050919050565b6103438161032e565b82525050565b600060208201905061035e600083018461033a565b92915050565b6000819050919050565b61037781610364565b811461038257600080fd5b50565b6000813590506103948161036e565b92915050565b6000602082840312156103b0576103af6102a4565b5b60006103be84828501610385565b91505092915050565b600060ff82169050919050565b6103dd816103c7565b82525050565b60006020820190506103f860008301846103d4565b92915050565b61040781610364565b82525050565b600060208201905061042260008301846103fe565b9291505056fea2646970667358221220b63ea2baf0ead38ab1ac33ec6425843f8242d5428057e132d8a123fc1846f25564736f6c63430008130033
```

### Comparing `cic-contracts-0.3.4/cic_contracts/unittest/solidity/WriterTest.sol` & `cic-contracts-0.3.5/cic_contracts/unittest/solidity/WriterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts/writer.py` & `cic-contracts-0.3.5/cic_contracts/writer.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/cic_contracts.egg-info/PKG-INFO` & `cic-contracts-0.3.5/cic_contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cic-contracts
-Version: 0.3.4
+Version: 0.3.5
 Summary: CIC network smart contract interfaces
 Home-page: https://gitlab.com/cicnet/cic-contracts
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cic-contracts-0.3.4/cic_contracts.egg-info/SOURCES.txt` & `cic-contracts-0.3.5/cic_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_burner/burn.py` & `cic-contracts-0.3.5/eth_burner/burn.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_burner/unittest/base.py` & `cic-contracts-0.3.5/eth_burner/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_burner/unittest/interface.py` & `cic-contracts-0.3.5/eth_burner/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_capped/capped.py` & `cic-contracts-0.3.5/eth_capped/capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_capped/unittest/base.py` & `cic-contracts-0.3.5/eth_capped/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_capped/unittest/interface.py` & `cic-contracts-0.3.5/eth_capped/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_expire/expire.py` & `cic-contracts-0.3.5/eth_expire/expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_expire/unittest/base.py` & `cic-contracts-0.3.5/eth_expire/unittest/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,34 +30,34 @@
 
         code = bytecode('expire')
 
         txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         tx = txf.template(self.accounts[0], None, use_nonce=True)
 
         date_expire = datetime.datetime.utcnow() + datetime.timedelta(seconds=10000)
-        self.expire = int(date_expire.timestamp())
+        self.expire_value = int(date_expire.timestamp())
         enc = ABIContractEncoder()
-        enc.uint256(self.expire)
+        enc.uint256(self.expire_value)
         args = enc.get()
 
         tx = txf.set_code(tx, code + args)
         (tx_hash_hex, o) = txf.build(tx)
         self.conn.do(o)
         o = receipt(tx_hash_hex)
         r = self.conn.do(o)
         self.assertEqual(r['status'], 1)
         self.address = r['contract_address']
         logg.debug('published expire test contract with hash {}'.format(r))
 
 
-    def set_expiry(self, contract_address, sender_address, v, tx_format=TxFormat.JSONRPC):
+    def set_expire(self, contract_address, sender_address, v, tx_format=TxFormat.JSONRPC):
         nonce_oracle = RPCNonceOracle(self.accounts[0], self.conn)
         txf = TxFactory(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
         enc = ABIContractEncoder()
-        enc.method('setExpiry')
+        enc.method('setExpire')
         enc.typ(ABIContractType.UINT256)
         enc.uint256(v)
         data = enc.get()
         tx = txf.template(sender_address, contract_address, use_nonce=True)
         tx = txf.set_code(tx, data)
         tx = txf.finalize(tx, tx_format)
         return tx
```

### Comparing `cic-contracts-0.3.4/eth_expire/unittest/interface.py` & `cic-contracts-0.3.5/eth_expire/unittest/interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 class TestEthExpireInterface:
 
     def __init__(self):
         self.set_method = None
 
 
     def test_expire(self):
-        if self.expire == 0:
+        if self.expire_value == 0:
             return
         c = EthExpire(self.chain_spec)
         o = c.expires(self.address, sender_address=self.accounts[0])
         r = self.rpc.do(o)
-        self.assertEqual(self.expire, int(r, 16))
+        self.assertEqual(self.expire_value, int(r, 16))
 
 
     def test_expire_change(self):
         if self.set_method == None:
             return
 
-        self.expire += 43200
-        (tx_hash_hex, o) = self.set_method(self.address, self.accounts[0], self.expire)
+        self.expire_value += 43200
+        (tx_hash_hex, o) = self.set_method(self.address, self.accounts[0], self.expire_value)
         self.rpc.do(o)
         o = receipt(tx_hash_hex)
         r = self.conn.do(o)
         self.assertEqual(r['status'], 1)
 
         c = EthExpire(self.chain_spec)
         o = c.expires(self.address, sender_address=self.accounts[0])
         r = self.rpc.do(o)
-        self.assertEqual(self.expire, int(r, 16))
+        self.assertEqual(self.expire_value, int(r, 16))
```

### Comparing `cic-contracts-0.3.4/eth_minter/minter.py` & `cic-contracts-0.3.5/eth_minter/minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_minter/unittest/base.py` & `cic-contracts-0.3.5/eth_minter/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_minter/unittest/interface.py` & `cic-contracts-0.3.5/eth_minter/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_seal/seal.py` & `cic-contracts-0.3.5/eth_seal/seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_seal/unittest/base.py` & `cic-contracts-0.3.5/eth_seal/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_writer/interface.py` & `cic-contracts-0.3.5/eth_writer/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_writer/unittest/base.py` & `cic-contracts-0.3.5/eth_writer/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/eth_writer/unittest/interface.py` & `cic-contracts-0.3.5/eth_writer/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/setup.cfg` & `cic-contracts-0.3.5/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cic-contracts
-version = 0.3.4
+version = 0.3.5
 description = CIC network smart contract interfaces
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://gitlab.com/cicnet/cic-contracts
 keywords = 
 	dlt
 	blockchain
```

### Comparing `cic-contracts-0.3.4/setup.py` & `cic-contracts-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/tests/test_burner.py` & `cic-contracts-0.3.5/tests/test_burner.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/tests/test_capped.py` & `cic-contracts-0.3.5/tests/test_capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/tests/test_expire.py` & `cic-contracts-0.3.5/tests/test_expire.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 
 
 class TestExpireBase(TestEthExpire, TestEthExpireInterface, TestERC165):
 
     def setUp(self):
         super(TestExpireBase, self).setUp()
         self.add_interface_check('841a0e94')
-        self.set_method = self.set_expiry
+        self.set_method = self.set_expire
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cic-contracts-0.3.4/tests/test_minter.py` & `cic-contracts-0.3.5/tests/test_minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/tests/test_seal.py` & `cic-contracts-0.3.5/tests/test_seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.4/tests/test_writer.py` & `cic-contracts-0.3.5/tests/test_writer.py`

 * *Files identical despite different names*

