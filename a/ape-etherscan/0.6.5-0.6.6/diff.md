# Comparing `tmp/ape-etherscan-0.6.5.tar.gz` & `tmp/ape-etherscan-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-etherscan-0.6.5.tar", last modified: Thu Jun  1 21:39:27 2023, max compression
+gzip compressed data, was "ape-etherscan-0.6.6.tar", last modified: Thu Jun  8 14:11:21 2023, max compression
```

## Comparing `ape-etherscan-0.6.5.tar` & `ape-etherscan-0.6.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/ape_etherscan/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/ape_etherscan/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.662877 ape-etherscan-0.6.5/ape_etherscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 21:39:27.000000 ape-etherscan-0.6.5/ape_etherscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:39:27.666877 ape-etherscan-0.6.5/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/mock_responses/get_account_transactions.json
--rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/mock_responses/get_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/mock_responses/get_proxy_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/mock_responses/get_vyper_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-01 21:38:14.000000 ape-etherscan-0.6.5/tests/test_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.869400 ape-etherscan-0.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.861400 ape-etherscan-0.6.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.861400 ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.865400 ape-etherscan-0.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-08 14:11:21.869400 ape-etherscan-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.865400 ape-etherscan-0.6.6/ape_etherscan/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/ape_etherscan/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.865400 ape-etherscan-0.6.6/ape_etherscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 14:11:21.000000 ape-etherscan-0.6.6/ape_etherscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 14:11:21.869400 ape-etherscan-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.865400 ape-etherscan-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:11:21.869400 ape-etherscan-0.6.6/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/mock_responses/get_account_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85181 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/mock_responses/get_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93453 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/mock_responses/get_proxy_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93483 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/mock_responses/get_vyper_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-08 14:09:59.000000 ape-etherscan-0.6.6/tests/test_etherscan.py
```

### Comparing `ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/bug.md` & `ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/feature.md` & `ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/ISSUE_TEMPLATE/work-item.md` & `ape-etherscan-0.6.6/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/release-drafter.yml` & `ape-etherscan-0.6.6/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/workflows/codeql.yml` & `ape-etherscan-0.6.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/workflows/commit.yaml` & `ape-etherscan-0.6.6/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/workflows/prtitle.yaml` & `ape-etherscan-0.6.6/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/workflows/publish.yaml` & `ape-etherscan-0.6.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/workflows/stale-prs.yml` & `ape-etherscan-0.6.6/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.github/workflows/test.yaml` & `ape-etherscan-0.6.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.gitignore` & `ape-etherscan-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/.pre-commit-config.yaml` & `ape-etherscan-0.6.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/CONTRIBUTING.md` & `ape-etherscan-0.6.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/LICENSE` & `ape-etherscan-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/PKG-INFO` & `ape-etherscan-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.5
+Version: 0.6.6
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-etherscan-0.6.5/README.md` & `ape-etherscan-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/ape_etherscan/__init__.py` & `ape-etherscan-0.6.6/ape_etherscan/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/ape_etherscan/client.py` & `ape-etherscan-0.6.6/ape_etherscan/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from io import StringIO
 from typing import Dict, Iterator, List, Optional
 
 from ape.logging import logger
 from ape.utils import USER_AGENT, ManagerAccessMixin
 from requests import Session
 
-from ape_etherscan.exceptions import UnhandledResultError, UnsupportedEcosystemError
+from ape_etherscan.exceptions import (
+    UnhandledResultError,
+    UnsupportedEcosystemError,
+    UnsupportedNetworkError,
+)
 from ape_etherscan.types import EtherscanResponse, SourceCodeResponse
 from ape_etherscan.utils import API_KEY_ENV_KEY_MAP
 
 
 def get_etherscan_uri(ecosystem_name: str, network_name: str):
     if ecosystem_name == "ethereum":
         return (
@@ -63,14 +67,18 @@
         )
     elif ecosystem_name == "bsc":
         return (
             f"https://{network_name}.bscscan.com"
             if network_name != "mainnet"
             else "https://bscscan.com"
         )
+    elif ecosystem_name == "gnosis":
+        if network_name == "mainnet":
+            return "https://gnosisscan.io"
+        raise UnsupportedNetworkError(ecosystem_name, network_name)
 
     raise UnsupportedEcosystemError(ecosystem_name)
 
 
 def get_etherscan_api_uri(ecosystem_name: str, network_name: str):
     if ecosystem_name == "ethereum":
         return (
@@ -124,14 +132,18 @@
         )
     elif ecosystem_name == "bsc":
         return (
             f"https://api-{network_name}.bscscan.com/api"
             if network_name != "mainnet"
             else "https://api.bscscan.com/api"
         )
+    elif ecosystem_name == "gnosis":
+        if network_name == "mainnet":
+            return "https://api.gnosisscan.io/api"
+        raise UnsupportedNetworkError(ecosystem_name, network_name)
 
     raise UnsupportedEcosystemError(ecosystem_name)
 
 
 class _APIClient(ManagerAccessMixin):
     DEFAULT_HEADERS = {"User-Agent": USER_AGENT}
     session = Session()
```

### Comparing `ape-etherscan-0.6.5/ape_etherscan/config.py` & `ape-etherscan-0.6.6/ape_etherscan/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,7 +12,8 @@
     fantom: EcosystemConfig = EcosystemConfig()
     optimism: EcosystemConfig = EcosystemConfig()
     base: EcosystemConfig = EcosystemConfig()
     polygon_zkevm: EcosystemConfig = EcosystemConfig()
     polygon: EcosystemConfig = EcosystemConfig()
     avalanche: EcosystemConfig = EcosystemConfig()
     bsc: EcosystemConfig = EcosystemConfig()
+    gnosis: EcosystemConfig = EcosystemConfig()
```

### Comparing `ape-etherscan-0.6.5/ape_etherscan/exceptions.py` & `ape-etherscan-0.6.6/ape_etherscan/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,23 @@
     Raised when there is no Etherscan buildout for ecosystem.
     """
 
     def __init__(self, ecosystem: str):
         super().__init__(f"Unsupported Ecosystem: {ecosystem}")
 
 
+class UnsupportedNetworkError(ApeEtherscanException):
+    """
+    Raised when there is no Etherscan buildout for ecosystem.
+    """
+
+    def __init__(self, ecosystem_name: str, network_name: str):
+        super().__init__(f"Unsupported Network for Ecosystem '{ecosystem_name}': {network_name}")
+
+
 class EtherscanResponseError(ApeEtherscanException):
     """
     Raised when the response is not correct.
     """
 
     def __init__(self, response: Union[Response, "EtherscanResponse"], message: str):
         if not isinstance(response, Response):
```

### Comparing `ape-etherscan-0.6.5/ape_etherscan/explorer.py` & `ape-etherscan-0.6.6/ape_etherscan/explorer.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/ape_etherscan/query.py` & `ape-etherscan-0.6.6/ape_etherscan/query.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/ape_etherscan/types.py` & `ape-etherscan-0.6.6/ape_etherscan/types.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/ape_etherscan/utils.py` & `ape-etherscan-0.6.6/ape_etherscan/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "fantom": "FTMSCAN_API_KEY",
     "optimism": "OPTIMISTIC_ETHERSCAN_API_KEY",
     "polygon-zkevm": "POLYGON_ZKEVM_ETHERSCAN_API_KEY",
     "base": "BASESCAN_API_KEY",
     "polygon": "POLYGONSCAN_API_KEY",
     "avalanche": "SNOWTRACE_API_KEY",
     "bsc": "BSCSCAN_API_KEY",
+    "gnosis": "GNOSISSCAN_API_KEY",
 }
 NETWORKS = {
     "ethereum": [
         "mainnet",
         "goerli",
         "sepolia",
     ],
@@ -43,8 +44,9 @@
         "mainnet",
         "fuji",
     ],
     "bsc": [
         "mainnet",
         "testnet",
     ],
+    "gnosis": ["mainnet"],
 }
```

### Comparing `ape-etherscan-0.6.5/ape_etherscan/verify.py` & `ape-etherscan-0.6.6/ape_etherscan/verify.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/ape_etherscan.egg-info/PKG-INFO` & `ape-etherscan-0.6.6/ape_etherscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.6.5
+Version: 0.6.6
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-etherscan-0.6.5/ape_etherscan.egg-info/SOURCES.txt` & `ape-etherscan-0.6.6/ape_etherscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/ape_etherscan.egg-info/requires.txt` & `ape-etherscan-0.6.6/ape_etherscan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/pyproject.toml` & `ape-etherscan-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/setup.py` & `ape-etherscan-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/tests/conftest.py` & `ape-etherscan-0.6.6/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,17 @@
                 "goerli": com_testnet_url("testnet-zkevm", "polygonscan"),
             },
             "avalanche": {"mainnet": url("snowtrace"), "fuji": testnet_url("testnet", "snowtrace")},
             "bsc": {
                 "mainnet": com_url("bscscan"),
                 "testnet": com_testnet_url("testnet", "bscscan"),
             },
+            "gnosis": {
+                "mainnet": url("gnosisscan"),
+            },
         }
 
     def set_network(self, ecosystem: str, network: str):
         self._expected_base_uri = self.expected_uri_map[ecosystem][network.replace("-fork", "")]
 
     def add_handler(
         self,
```

### Comparing `ape-etherscan-0.6.5/tests/mock_responses/get_account_transactions.json` & `ape-etherscan-0.6.6/tests/mock_responses/get_account_transactions.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/tests/mock_responses/get_contract_response.json` & `ape-etherscan-0.6.6/tests/mock_responses/get_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/tests/mock_responses/get_proxy_contract_response.json` & `ape-etherscan-0.6.6/tests/mock_responses/get_proxy_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/tests/mock_responses/get_vyper_contract_response.json` & `ape-etherscan-0.6.6/tests/mock_responses/get_vyper_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.6.5/tests/test_etherscan.py` & `ape-etherscan-0.6.6/tests/test_etherscan.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         ("base", "goerli", "goerli.basescan.org"),
         ("avalanche", "mainnet", "snowtrace.io"),
         ("avalanche", "fuji", "testnet.snowtrace.io"),
         ("bsc", "mainnet", "bscscan.com"),
         ("bsc", "mainnet-fork", "bscscan.com"),
         ("bsc", "testnet", "testnet.bscscan.com"),
         ("bsc", "testnet-fork", "testnet.bscscan.com"),
+        ("gnosis", "mainnet", "gnosisscan.io"),
+        ("gnosis", "mainnet-fork", "gnosisscan.io"),
     ],
 )
 
 
 @pytest.fixture
 def verification_tester_cls():
     class VerificationTester:
```

