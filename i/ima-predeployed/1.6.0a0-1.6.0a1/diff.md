# Comparing `tmp/ima-predeployed-1.6.0a0.tar.gz` & `tmp/ima-predeployed-1.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ima-predeployed-1.6.0a0.tar", last modified: Wed Jun  7 18:05:11 2023, max compression
+gzip compressed data, was "ima-predeployed-1.6.0a1.tar", last modified: Thu Jun  8 15:43:42 2023, max compression
```

## Comparing `ima-predeployed-1.6.0a0.tar` & `ima-predeployed-1.6.0a1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:05:11.132145 ima-predeployed-1.6.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-07 18:05:11.132145 ima-predeployed-1.6.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 18:05:11.132145 ima-predeployed-1.6.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:05:11.112145 ima-predeployed-1.6.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:05:11.116145 ima-predeployed-1.6.0a0/src/ima_predeployed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:05:11.128145 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-06-07 18:04:58.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/CommunityLocker.json
--rw-r--r--   0 runner    (1001) docker     (123)   659611 2023-06-07 18:04:58.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/CommunityLocker.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    58650 2023-06-07 18:05:04.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC1155OnChain.json
--rw-r--r--   0 runner    (1001) docker     (123)   659610 2023-06-07 18:05:04.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC1155OnChain.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-06-07 18:05:03.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC20OnChain.json
--rw-r--r--   0 runner    (1001) docker     (123)   659608 2023-06-07 18:05:03.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC20OnChain.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    53201 2023-06-07 18:05:03.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC721OnChain.json
--rw-r--r--   0 runner    (1001) docker     (123)   659609 2023-06-07 18:05:03.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC721OnChain.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    39987 2023-06-07 18:05:02.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/EthErc20.json
--rw-r--r--   0 runner    (1001) docker     (123)   659604 2023-06-07 18:05:02.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/EthErc20.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-07 18:04:56.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/KeyStorage.json
--rw-r--r--   0 runner    (1001) docker     (123)   659606 2023-06-07 18:04:56.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/KeyStorage.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    91866 2023-06-07 18:04:57.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/MessageProxyForSchain.json
--rw-r--r--   0 runner    (1001) docker     (123)   659617 2023-06-07 18:04:57.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/MessageProxyForSchain.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-07 18:04:57.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManager.json
--rw-r--r--   0 runner    (1001) docker     (123)   659608 2023-06-07 18:04:57.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManager.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)   156723 2023-06-07 18:05:01.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC1155.json
--rw-r--r--   0 runner    (1001) docker     (123)   659615 2023-06-07 18:05:01.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC1155.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)   116677 2023-06-07 18:04:59.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)   659613 2023-06-07 18:04:59.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC20.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)   121106 2023-06-07 18:05:00.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC721.json
--rw-r--r--   0 runner    (1001) docker     (123)   659614 2023-06-07 18:05:00.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC721.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)   123774 2023-06-07 18:05:00.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.json
--rw-r--r--   0 runner    (1001) docker     (123)   659626 2023-06-07 18:05:00.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    47914 2023-06-07 18:05:02.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerEth.json
--rw-r--r--   0 runner    (1001) docker     (123)   659611 2023-06-07 18:05:02.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerEth.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-06-07 18:04:58.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerLinker.json
--rw-r--r--   0 runner    (1001) docker     (123)   659614 2023-06-07 18:04:58.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerLinker.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contract_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:05:11.132145 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/admin_upgradeability_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/community_locker.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/erc1155_on_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/erc20_on_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/erc721_on_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/eth_erc20.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/key_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/message_proxy_for_schain.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/proxy_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_erc20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_erc721.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_erc721_with_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_linker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/src/ima_predeployed/upgradeable_contract_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:05:11.116145 ima-predeployed-1.6.0a0/src/ima_predeployed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-07 18:05:11.000000 ima-predeployed-1.6.0a0/src/ima_predeployed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-07 18:05:11.000000 ima-predeployed-1.6.0a0/src/ima_predeployed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:05:11.000000 ima-predeployed-1.6.0a0/src/ima_predeployed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 18:05:11.000000 ima-predeployed-1.6.0a0/src/ima_predeployed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 18:05:11.000000 ima-predeployed-1.6.0a0/src/ima_predeployed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:05:11.132145 ima-predeployed-1.6.0a0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/test/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 17:57:47.000000 ima-predeployed-1.6.0a0/test/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:04:55.000000 ima-predeployed-1.6.0a0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.765028 ima-predeployed-1.6.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-08 15:43:42.765028 ima-predeployed-1.6.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-08 15:43:42.765028 ima-predeployed-1.6.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.741028 ima-predeployed-1.6.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.745028 ima-predeployed-1.6.0a1/src/ima_predeployed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.761028 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-06-08 15:43:30.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/CommunityLocker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659611 2023-06-08 15:43:30.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/CommunityLocker.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58650 2023-06-08 15:43:36.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC1155OnChain.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659610 2023-06-08 15:43:36.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC1155OnChain.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-06-08 15:43:34.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC20OnChain.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659608 2023-06-08 15:43:34.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC20OnChain.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53201 2023-06-08 15:43:35.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC721OnChain.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659609 2023-06-08 15:43:35.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC721OnChain.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39987 2023-06-08 15:43:34.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/EthErc20.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659604 2023-06-08 15:43:34.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/EthErc20.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-08 15:43:27.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/KeyStorage.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659606 2023-06-08 15:43:27.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/KeyStorage.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91866 2023-06-08 15:43:28.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/MessageProxyForSchain.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659617 2023-06-08 15:43:28.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/MessageProxyForSchain.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-08 15:43:29.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManager.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659608 2023-06-08 15:43:29.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManager.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)   156723 2023-06-08 15:43:32.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659615 2023-06-08 15:43:32.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC1155.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)   116677 2023-06-08 15:43:31.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659613 2023-06-08 15:43:31.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC20.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121106 2023-06-08 15:43:31.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659614 2023-06-08 15:43:31.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC721.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)   123774 2023-06-08 15:43:32.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659626 2023-06-08 15:43:32.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47914 2023-06-08 15:43:33.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerEth.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659611 2023-06-08 15:43:33.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerEth.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-06-08 15:43:29.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerLinker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659614 2023-06-08 15:43:29.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerLinker.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contract_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.761028 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/admin_upgradeability_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/community_locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/erc1155_on_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/erc20_on_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/erc721_on_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/eth_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/key_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/message_proxy_for_schain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/proxy_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_erc721.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_erc721_with_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed/upgradeable_contract_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.745028 ima-predeployed-1.6.0a1/src/ima_predeployed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-08 15:43:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-08 15:43:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:43:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 15:43:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 15:43:42.000000 ima-predeployed-1.6.0a1/src/ima_predeployed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.761028 ima-predeployed-1.6.0a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 15:35:42.000000 ima-predeployed-1.6.0a1/test/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 15:43:27.000000 ima-predeployed-1.6.0a1/version.txt
```

### Comparing `ima-predeployed-1.6.0a0/LICENSE` & `ima-predeployed-1.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/PKG-INFO` & `ima-predeployed-1.6.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ima-predeployed
-Version: 1.6.0a0
+Version: 1.6.0a1
 Summary: A tool to generate config for predeployed IMA
 Home-page: https://github.com/skalenetwork/IMA
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ima-predeployed-1.6.0a0/setup.cfg` & `ima-predeployed-1.6.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/addresses.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/addresses.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/CommunityLocker.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/CommunityLocker.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/CommunityLocker.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/CommunityLocker.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC1155OnChain.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC1155OnChain.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC1155OnChain.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC1155OnChain.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC20OnChain.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC20OnChain.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC20OnChain.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC20OnChain.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC721OnChain.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC721OnChain.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/ERC721OnChain.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/ERC721OnChain.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/EthErc20.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/EthErc20.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/EthErc20.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/EthErc20.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/KeyStorage.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/KeyStorage.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/KeyStorage.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/KeyStorage.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/MessageProxyForSchain.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/MessageProxyForSchain.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/MessageProxyForSchain.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/MessageProxyForSchain.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManager.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManager.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManager.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManager.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC1155.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC1155.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC1155.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC1155.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC20.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC20.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC20.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC20.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC721.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC721.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC721.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC721.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerEth.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerEth.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerEth.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerEth.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerLinker.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerLinker.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/artifacts/TokenManagerLinker.meta.json` & `ima-predeployed-1.6.0a1/src/ima_predeployed/artifacts/TokenManagerLinker.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contract_generator.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contract_generator.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/admin_upgradeability_proxy.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/admin_upgradeability_proxy.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/community_locker.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/community_locker.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/erc1155_on_chain.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/erc1155_on_chain.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/erc20_on_chain.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/erc20_on_chain.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/erc721_on_chain.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/erc721_on_chain.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/eth_erc20.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/eth_erc20.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/key_storage.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/key_storage.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/message_proxy_for_schain.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/message_proxy_for_schain.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_erc1155.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_erc1155.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_erc20.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_erc20.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_erc721.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_erc721.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_erc721_with_metadata.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_erc721_with_metadata.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_eth.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_eth.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/contracts/token_manager_linker.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/contracts/token_manager_linker.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/generator.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/generator.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed/upgradeable_contract_generator.py` & `ima-predeployed-1.6.0a1/src/ima_predeployed/upgradeable_contract_generator.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed.egg-info/PKG-INFO` & `ima-predeployed-1.6.0a1/src/ima_predeployed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ima-predeployed
-Version: 1.6.0a0
+Version: 1.6.0a1
 Summary: A tool to generate config for predeployed IMA
 Home-page: https://github.com/skalenetwork/IMA
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ima-predeployed-1.6.0a0/src/ima_predeployed.egg-info/SOURCES.txt` & `ima-predeployed-1.6.0a1/src/ima_predeployed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/test/test.py` & `ima-predeployed-1.6.0a1/test/test.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-1.6.0a0/test/test_generator.py` & `ima-predeployed-1.6.0a1/test/test_generator.py`

 * *Files identical despite different names*

