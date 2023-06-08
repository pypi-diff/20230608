# Comparing `tmp/ape-optimism-0.6.0.tar.gz` & `tmp/ape-optimism-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-optimism-0.6.0.tar", last modified: Tue Jan 31 19:27:05 2023, max compression
+gzip compressed data, was "ape-optimism-0.6.1.tar", last modified: Thu Jun  8 19:30:18 2023, max compression
```

## Comparing `ape-optimism-0.6.0.tar` & `ape-optimism-0.6.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/ape_optimism/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/ape_optimism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/ape_optimism/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/ape_optimism/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:27:05.000000 ape-optimism-0.6.0/ape_optimism/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/ape_optimism.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-31 19:27:05.000000 ape-optimism-0.6.0/ape_optimism.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-31 19:27:05.000000 ape-optimism-0.6.0/ape_optimism.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:27:05.000000 ape-optimism-0.6.0/ape_optimism.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:27:05.000000 ape-optimism-0.6.0/ape_optimism.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-31 19:27:05.000000 ape-optimism-0.6.0/ape_optimism.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-31 19:27:05.000000 ape-optimism-0.6.0/ape_optimism.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:27:05.798896 ape-optimism-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-01-31 19:26:06.000000 ape-optimism-0.6.0/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.832200 ape-optimism-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.832200 ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/ape_optimism/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/ape_optimism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/ape_optimism/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/ape_optimism/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/ape_optimism.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/test_provider.py
```

### Comparing `ape-optimism-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.github/release-drafter.yml` & `ape-optimism-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.github/workflows/commitlint.yaml` & `ape-optimism-0.6.1/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.github/workflows/prtitle.yaml` & `ape-optimism-0.6.1/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.github/workflows/publish.yaml` & `ape-optimism-0.6.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.github/workflows/test.yaml` & `ape-optimism-0.6.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.gitignore` & `ape-optimism-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/.pre-commit-config.yaml` & `ape-optimism-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/CONTRIBUTING.md` & `ape-optimism-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/LICENSE` & `ape-optimism-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/PKG-INFO` & `ape-optimism-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-optimism
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-optimism: Ape Ecosystem Plugin for Optimism
 Home-page: https://github.com/ApeWorX/ape-optimism
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-optimism-0.6.0/README.md` & `ape-optimism-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/ape_optimism/__init__.py` & `ape-optimism-0.6.1/ape_optimism/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/ape_optimism/ecosystem.py` & `ape-optimism-0.6.1/ape_optimism/ecosystem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from typing import Optional, Type, Union, cast
+from typing import Dict, Optional, Type, Union, cast
 
 from ape.api import TransactionAPI
 from ape.api.config import PluginConfig
 from ape.api.networks import LOCAL_NETWORK_NAME
 from ape.exceptions import ApeException
 from ape.types import TransactionSignature
 from ape_ethereum.ecosystem import Ethereum, NetworkConfig
-from ape_ethereum.transactions import StaticFeeTransaction, TransactionType
-from eth_typing import HexStr
-from eth_utils import add_0x_prefix
+from ape_ethereum.transactions import (
+    AccessListTransaction,
+    DynamicFeeTransaction,
+    StaticFeeTransaction,
+    TransactionType,
+)
 
 NETWORKS = {
     # chain_id, network_id
     "mainnet": (10, 10),
     "goerli": (420, 420),
 }
 
@@ -29,15 +32,15 @@
     return NetworkConfig(
         required_confirmations=required_confirmations, block_time=block_time, **kwargs
     )
 
 
 def _create_local_config(default_provider: Optional[str] = None) -> NetworkConfig:
     return _create_network_config(
-        required_confirmations=0, block_time=0, default_provider=default_provider
+        required_confirmations=0, block_time=0, default_provider=default_provider, gas_limit="max"
     )
 
 
 class OptimismConfig(PluginConfig):
     mainnet: NetworkConfig = _create_network_config()
     mainnet_fork: NetworkConfig = _create_local_config()
     goerli: NetworkConfig = _create_network_config()
@@ -58,15 +61,15 @@
 
         **kwargs: Kwargs for the transaction class.
 
         Returns:
             :class:`~ape.api.transactions.TransactionAPI`
         """
 
-        transaction_type = _get_transaction_type(kwargs.get("type"))
+        transaction_type = self.get_transaction_type(kwargs.get("type"))
         kwargs["type"] = transaction_type.value
         txn_class = _get_transaction_cls(transaction_type)
 
         if "required_confirmations" not in kwargs or kwargs["required_confirmations"] is None:
             # Attempt to use default required-confirmations from `ape-config.yaml`.
             required_confirmations = 0
             active_provider = self.network_manager.active_provider
@@ -86,34 +89,27 @@
                 v=kwargs["v"],
                 r=bytes(kwargs["r"]),
                 s=bytes(kwargs["s"]),
             )
 
         return txn_class.parse_obj(kwargs)
 
-
-def _get_transaction_type(_type: Optional[Union[int, str, bytes]]) -> TransactionType:
-    if not _type:
-        return TransactionType.STATIC
-
-    if _type is None:
-        _type = TransactionType.STATIC.value
-    elif isinstance(_type, int):
-        _type = f"0{_type}"
-    elif isinstance(_type, bytes):
-        _type = _type.hex()
-
-    suffix = _type.replace("0x", "")
-    if len(suffix) == 1:
-        _type = f"{_type.rstrip(suffix)}0{suffix}"
-
-    return TransactionType(add_0x_prefix(HexStr(_type)))
+    def get_transaction_type(self, _type: Optional[Union[int, str, bytes]]) -> TransactionType:
+        if _type is None:
+            version = TransactionType.STATIC
+        elif not isinstance(_type, int):
+            version = TransactionType(self.conversion_manager.convert(_type, int))
+        else:
+            version = TransactionType(_type)
+        return version
 
 
 def _get_transaction_cls(transaction_type: TransactionType) -> Type[TransactionAPI]:
-    transaction_types = {
+    transaction_types: Dict[TransactionType, Type[TransactionAPI]] = {
         TransactionType.STATIC: StaticFeeTransaction,
+        TransactionType.DYNAMIC: DynamicFeeTransaction,
+        TransactionType.ACCESS_LIST: AccessListTransaction,
     }
     if transaction_type not in transaction_types:
         raise ApeOptimismError(f"Transaction type '{transaction_type}' not supported.")
 
     return transaction_types[transaction_type]
```

### Comparing `ape-optimism-0.6.0/ape_optimism.egg-info/PKG-INFO` & `ape-optimism-0.6.1/ape_optimism.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-optimism
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-optimism: Ape Ecosystem Plugin for Optimism
 Home-page: https://github.com/ApeWorX/ape-optimism
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-optimism-0.6.0/ape_optimism.egg-info/SOURCES.txt` & `ape-optimism-0.6.1/ape_optimism.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 ape_optimism.egg-info/SOURCES.txt
 ape_optimism.egg-info/dependency_links.txt
 ape_optimism.egg-info/not-zip-safe
 ape_optimism.egg-info/requires.txt
 ape_optimism.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_ecosystem.py
 tests/test_integration.py
 tests/test_provider.py
```

### Comparing `ape-optimism-0.6.0/ape_optimism.egg-info/requires.txt` & `ape-optimism-0.6.1/ape_optimism.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/pyproject.toml` & `ape-optimism-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/setup.py` & `ape-optimism-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.0/tests/test_integration.py` & `ape-optimism-0.6.1/tests/test_integration.py`

 * *Files identical despite different names*

