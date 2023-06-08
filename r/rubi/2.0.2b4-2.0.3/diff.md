# Comparing `tmp/rubi-2.0.2b4.tar.gz` & `tmp/rubi-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.0.2b4.tar", max compression
+gzip compressed data, was "rubi-2.0.3.tar", max compression
```

## Comparing `rubi-2.0.2b4.tar` & `rubi-2.0.3.tar`

### file list

```diff
@@ -1,86 +1,52 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.2b4/LICENSE
--rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.2b4/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.2b4/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.2b4/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.2b4/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.2b4/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      645 2023-06-01 18:59:40.465341 rubi-2.0.2b4/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.2b4/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.2b4/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      664 2023-06-01 18:59:40.468200 rubi-2.0.2b4/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.2b4/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.2b4/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      518 2023-06-01 18:59:40.468648 rubi-2.0.2b4/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.2b4/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.2b4/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      631 2023-06-01 18:59:40.469759 rubi-2.0.2b4/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0      750 2023-06-01 22:57:17.303245 rubi-2.0.2b4/pyproject.toml
--rw-r--r--   0        0        0       96 2023-06-01 18:59:40.472105 rubi-2.0.2b4/rubi/__init__.py
--rw-r--r--   0        0        0      189 2023-02-14 17:43:51.820506 rubi-2.0.2b4/rubi/book/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4761 2023-02-14 17:43:51.821426 rubi-2.0.2b4/rubi/book/__pycache__/book.cpython-310.pyc
--rw-r--r--   0        0        0    27357 2023-06-01 18:59:40.472316 rubi-2.0.2b4/rubi/client.py
--rw-r--r--   0        0        0      154 2023-06-01 18:59:40.472446 rubi-2.0.2b4/rubi/contracts/__init__.py
--rw-r--r--   0        0        0      356 2023-06-01 19:30:35.704392 rubi-2.0.2b4/rubi/contracts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    36251 2023-02-14 17:43:51.831184 rubi-2.0.2b4/rubi/contracts/__pycache__/aid.cpython-310.pyc
--rw-r--r--   0        0        0     9599 2023-06-01 19:30:35.707087 rubi-2.0.2b4/rubi/contracts/__pycache__/base_contract.cpython-310.pyc
--rw-r--r--   0        0        0    14072 2023-06-01 22:56:32.965076 rubi-2.0.2b4/rubi/contracts/__pycache__/erc20.cpython-310.pyc
--rw-r--r--   0        0        0    20660 2023-06-01 19:30:35.709447 rubi-2.0.2b4/rubi/contracts/__pycache__/market.cpython-310.pyc
--rw-r--r--   0        0        0    12742 2023-06-01 19:30:35.710349 rubi-2.0.2b4/rubi/contracts/__pycache__/router.cpython-310.pyc
--rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.2b4/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11606 2023-06-01 18:59:40.472881 rubi-2.0.2b4/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0    16334 2023-06-01 22:56:14.494810 rubi-2.0.2b4/rubi/contracts/erc20.py
--rw-r--r--   0        0        0      265 2023-02-14 17:43:51.823336 rubi-2.0.2b4/rubi/contracts/helper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    13060 2023-02-14 17:43:51.825386 rubi-2.0.2b4/rubi/contracts/helper/__pycache__/erc20.cpython-310.pyc
--rw-r--r--   0        0        0     3544 2023-02-14 17:43:51.823886 rubi-2.0.2b4/rubi/contracts/helper/__pycache__/rolodex.cpython-310.pyc
--rw-r--r--   0        0        0    24182 2023-06-01 18:59:40.473250 rubi-2.0.2b4/rubi/contracts/market.py
--rw-r--r--   0        0        0    14668 2023-06-01 18:59:40.473453 rubi-2.0.2b4/rubi/contracts/router.py
--rw-r--r--   0        0        0       22 2023-06-01 18:59:40.473528 rubi-2.0.2b4/rubi/contracts/types/__init__.py
--rw-r--r--   0        0        0      190 2023-06-01 19:30:35.704851 rubi-2.0.2b4/rubi/contracts/types/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    16435 2023-06-01 19:30:35.706228 rubi-2.0.2b4/rubi/contracts/types/__pycache__/events.cpython-310.pyc
--rw-r--r--   0        0        0    16011 2023-06-01 18:59:40.473629 rubi-2.0.2b4/rubi/contracts/types/events.py
--rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.2b4/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.2b4/rubi/data/__init__.py
--rw-r--r--   0        0        0      209 2023-02-14 17:43:51.831555 rubi-2.0.2b4/rubi/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2675 2023-02-14 17:43:51.832049 rubi-2.0.2b4/rubi/data/__pycache__/data.cpython-310.pyc
--rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.2b4/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.2b4/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.2b4/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0      261 2023-02-14 17:43:55.749387 rubi-2.0.2b4/rubi/data/processing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    13304 2023-03-31 00:50:49.322124 rubi-2.0.2b4/rubi/data/processing/__pycache__/aid.cpython-310.pyc
--rw-r--r--   0        0        0     8742 2023-02-14 17:43:55.750234 rubi-2.0.2b4/rubi/data/processing/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.2b4/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.2b4/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0      216 2023-02-14 17:43:55.751294 rubi-2.0.2b4/rubi/data/processing/helper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2094 2023-02-14 17:43:55.751724 rubi-2.0.2b4/rubi/data/processing/helper/__pycache__/processing.cpython-310.pyc
--rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.2b4/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.2b4/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.2b4/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0      263 2023-02-14 17:43:55.741565 rubi-2.0.2b4/rubi/data/sources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    14673 2023-03-31 00:50:49.318062 rubi-2.0.2b4/rubi/data/sources/__pycache__/aid.cpython-310.pyc
--rw-r--r--   0        0        0    13205 2023-02-14 17:43:55.743562 rubi-2.0.2b4/rubi/data/sources/__pycache__/market.cpython-310.pyc
--rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.2b4/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.2b4/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.2b4/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0      277 2023-02-14 17:43:55.743957 rubi-2.0.2b4/rubi/data/sources/helper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9542 2023-02-27 20:45:05.206965 rubi-2.0.2b4/rubi/data/sources/helper/__pycache__/gas.cpython-310.pyc
--rw-r--r--   0        0        0    11532 2023-02-14 17:43:55.746162 rubi-2.0.2b4/rubi/data/sources/helper/__pycache__/price.cpython-310.pyc
--rw-r--r--   0        0        0     3974 2023-02-14 17:43:55.744606 rubi-2.0.2b4/rubi/data/sources/helper/__pycache__/rolodex.cpython-310.pyc
--rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.2b4/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.2b4/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.2b4/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.2b4/rubi/data/sources/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.2b4/rubi/network/__init__.py
--rw-r--r--   0        0        0      268 2023-06-01 19:30:35.354611 rubi-2.0.2b4/rubi/network/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      266 2023-06-01 17:38:18.909828 rubi-2.0.2b4/rubi/network/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7862 2023-06-01 22:56:32.749071 rubi-2.0.2b4/rubi/network/__pycache__/network.cpython-310.pyc
--rw-r--r--   0        0        0     7866 2023-06-01 17:38:18.911845 rubi-2.0.2b4/rubi/network/__pycache__/network.cpython-39.pyc
--rw-r--r--   0        0        0     7684 2023-06-01 22:56:21.811207 rubi-2.0.2b4/rubi/network/network.py
--rw-r--r--   0        0        0       66 2023-06-01 18:59:40.474481 rubi-2.0.2b4/rubi/types/__init__.py
--rw-r--r--   0        0        0      216 2023-06-01 19:30:35.710993 rubi-2.0.2b4/rubi/types/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    11065 2023-06-01 19:30:35.712007 rubi-2.0.2b4/rubi/types/__pycache__/order.cpython-310.pyc
--rw-r--r--   0        0        0     6040 2023-06-01 19:30:35.713289 rubi-2.0.2b4/rubi/types/__pycache__/orderbook.cpython-310.pyc
--rw-r--r--   0        0        0     2880 2023-06-01 19:30:35.712427 rubi-2.0.2b4/rubi/types/__pycache__/pair.cpython-310.pyc
--rw-r--r--   0        0        0    12515 2023-06-01 18:59:40.474581 rubi-2.0.2b4/rubi/types/order.py
--rw-r--r--   0        0        0     5719 2023-06-01 18:59:40.474684 rubi-2.0.2b4/rubi/types/orderbook.py
--rw-r--r--   0        0        0     2707 2023-06-01 18:59:40.474750 rubi-2.0.2b4/rubi/types/pair.py
--rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 rubi-2.0.2b4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.3/LICENSE
+-rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.3/README.md
+-rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.3/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.3/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.3/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.3/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      645 2023-06-01 18:59:40.465341 rubi-2.0.3/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.3/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.3/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      664 2023-06-01 18:59:40.468200 rubi-2.0.3/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.3/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.3/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      518 2023-06-01 18:59:40.468648 rubi-2.0.3/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.3/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.3/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      631 2023-06-01 18:59:40.469759 rubi-2.0.3/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0      748 2023-06-08 02:20:45.126846 rubi-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-06-01 18:59:40.472105 rubi-2.0.3/rubi/__init__.py
+-rw-r--r--   0        0        0    26809 2023-06-07 23:47:41.357240 rubi-2.0.3/rubi/client.py
+-rw-r--r--   0        0        0      154 2023-06-01 18:59:40.472446 rubi-2.0.3/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.3/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    11394 2023-06-07 23:47:41.357521 rubi-2.0.3/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0    16600 2023-06-07 23:47:41.358043 rubi-2.0.3/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24654 2023-06-07 23:47:41.358440 rubi-2.0.3/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14838 2023-06-07 23:47:41.358885 rubi-2.0.3/rubi/contracts/router.py
+-rw-r--r--   0        0        0       74 2023-06-07 23:47:41.359211 rubi-2.0.3/rubi/contracts/types/__init__.py
+-rw-r--r--   0        0        0    16011 2023-06-01 18:59:40.473629 rubi-2.0.3/rubi/contracts/types/events.py
+-rw-r--r--   0        0        0     2674 2023-06-07 23:47:41.359354 rubi-2.0.3/rubi/contracts/types/transaction_reciept.py
+-rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.3/rubi/data/README.md
+-rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.3/rubi/data/__init__.py
+-rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.3/rubi/data/data.py
+-rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.3/rubi/data/processing/README.md
+-rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.3/rubi/data/processing/__init__.py
+-rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.3/rubi/data/processing/aid.py
+-rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.3/rubi/data/processing/helper/__init__.py
+-rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.3/rubi/data/processing/helper/processing.py
+-rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.3/rubi/data/processing/user.py
+-rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.3/rubi/data/sources/__init__.py
+-rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.3/rubi/data/sources/aid.py
+-rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.3/rubi/data/sources/helper/README.md
+-rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.3/rubi/data/sources/helper/__init__.py
+-rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.3/rubi/data/sources/helper/gas.py
+-rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.3/rubi/data/sources/helper/price.py
+-rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.3/rubi/data/sources/helper/rolodex.py
+-rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.3/rubi/data/sources/market.py
+-rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.3/rubi/network/__init__.py
+-rw-r--r--   0        0        0     7589 2023-06-01 23:03:08.489079 rubi-2.0.3/rubi/network/network.py
+-rw-r--r--   0        0        0       66 2023-06-01 18:59:40.474481 rubi-2.0.3/rubi/types/__init__.py
+-rw-r--r--   0        0        0    12516 2023-06-07 23:47:41.359563 rubi-2.0.3/rubi/types/order.py
+-rw-r--r--   0        0        0     5719 2023-06-01 18:59:40.474684 rubi-2.0.3/rubi/types/orderbook.py
+-rw-r--r--   0        0        0     2707 2023-06-01 18:59:40.474750 rubi-2.0.3/rubi/types/pair.py
+-rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.3/PKG-INFO
```

### Comparing `rubi-2.0.2b4/LICENSE` & `rubi-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/README.md` & `rubi-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/ERC20.json` & `rubi-2.0.3/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/README.md` & `rubi-2.0.3/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/abitrum_goerli/abis/market.json` & `rubi-2.0.3/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/abitrum_goerli/abis/router.json` & `rubi-2.0.3/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/abitrum_goerli/network.yaml` & `rubi-2.0.3/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/optimism/abis/market.json` & `rubi-2.0.3/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/optimism/abis/router.json` & `rubi-2.0.3/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/optimism/network.yaml` & `rubi-2.0.3/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/optimism_goerli/abis/market.json` & `rubi-2.0.3/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/optimism_goerli/abis/router.json` & `rubi-2.0.3/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/optimism_goerli/network.yaml` & `rubi-2.0.3/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/polygon_mumbai/abis/market.json` & `rubi-2.0.3/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/polygon_mumbai/abis/router.json` & `rubi-2.0.3/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/network_config/polygon_mumbai/network.yaml` & `rubi-2.0.3/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/pyproject.toml` & `rubi-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.0.2b4"
+version = "2.0.3"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.0.2b4/rubi/client.py` & `rubi-2.0.3/rubi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from eth_typing import ChecksumAddress
 from web3.types import EventData
 
 from rubi.contracts import (
     RubiconMarket,
     RubiconRouter,
     ERC20,
+    TransactionReceipt
 )
 from rubi.network import (
     Network,
 )
 from rubi.types import (
     OrderSide,
     NewMarketOrder,
@@ -60,15 +61,14 @@
         self.wallet = self.network.w3.to_checksum_address(wallet) if wallet else wallet  # type: ChecksumAddress |  None
         self.key = key  # type: str |  None
 
         self.market = RubiconMarket.from_network(network=self.network, wallet=self.wallet, key=self.key)
         self.router = RubiconRouter.from_network(network=self.network, wallet=self.wallet, key=self.key)
 
         self._pairs: Dict[str, Pair] = {}
-        self._pair_orderbooks: Dict[str, OrderBook] = {}
 
         self.message_queue = message_queue  # type: Queue | None
 
     @classmethod
     def from_http_node_url(
         cls,
         http_node_url: str,
@@ -230,16 +230,14 @@
         self.update_pair_allowance(
             pair_name=pair_name,
             new_base_asset_allowance=Decimal("0"),
             new_quote_asset_allowance=Decimal("0")
         )
 
         del self._pairs[pair_name]
-        if self._pair_orderbooks.get(pair_name):
-            del self._pair_orderbooks[pair_name]
 
     ######################################################################
     # orderbook methods
     ######################################################################
 
     def get_orderbook(self, pair_name: str) -> OrderBook:
         """Retrieve the order book for a specific pair from the Rubicon Router.
@@ -303,16 +301,14 @@
         :type poll_time: int, optional
         """
         polling: bool = True
         while polling:
             try:
                 order_book = self.get_orderbook(pair_name=pair.name)
 
-                self._pair_orderbooks[pair.name] = order_book
-
                 self.message_queue.put(order_book)
             except PairDoesNotExistException:
                 log.warning("pair does not exist in client. shutting down orderbook poller")
                 polling = False
             except Exception as e:
                 log.error(e)
             sleep(poll_time)
@@ -387,21 +383,16 @@
             order_event = OrderEvent.from_event(pair=pair, event=raw_event, wallet=self.wallet)
 
             self.message_queue.put(order_event)
 
     ######################################################################
     # order methods
     ######################################################################
-    # TODO: would be cool if these methods could understand how much they are spending on gas (use TxReceipt)
-    #  also need a way to return the order id for limit orders
-    #  we could listen for the event and return the order id along with relevant gas spend information 
-    #  one thing we will need to be conscious of and figure out how to handle is the fact that gas is calculated in a
-    #  variety of ways depending upon the chain
 
-    def place_market_order(self, transaction: Transaction) -> str:
+    def place_market_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a market order transaction by executing the specified transaction object. The transaction
         object should contain a single order of type NewMarketOrder. The order is retrieved from the transaction and
         the corresponding market buy or sell method is called based on the order side.
 
         :param transaction: Transaction object containing the market order.
         :type transaction: Transaction
         :return: The transaction hash of the executed market order.
@@ -435,15 +426,15 @@
                     min_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price),
                     nonce=transaction.nonce,
                     gas=transaction.gas,
                     max_fee_per_gas=transaction.max_fee_per_gas,
                     max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
                 )
 
-    def place_limit_order(self, transaction: Transaction) -> str:
+    def place_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order transaction by executing the specified transaction object. The transaction object should
         contain a single order of type NewLimitOrder.
 
         :param transaction: Transaction object containing the limit order.
         :type transaction: Transaction
         :return: The transaction hash of the executed limit order.
         :rtype: str
@@ -476,15 +467,15 @@
                     buy_gem=pair.quote_asset.address,
                     nonce=transaction.nonce,
                     gas=transaction.gas,
                     max_fee_per_gas=transaction.max_fee_per_gas,
                     max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
                 )
 
-    def cancel_limit_order(self, transaction: Transaction) -> str:
+    def cancel_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order cancel transaction by executing the specified transaction object. The transaction object
         should contain a single order of type NewCancelOrder.
 
         :param transaction: Transaction object containing the cancel order.
         :type transaction: Transaction
         :return: The transaction hash of the executed cancel order.
         :rtype: str
@@ -499,15 +490,15 @@
             id=order.order_id,
             nonce=transaction.nonce,
             gas=transaction.gas,
             max_fee_per_gas=transaction.max_fee_per_gas,
             max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
         )
 
-    def batch_place_limit_orders(self, transaction: Transaction) -> str:
+    def batch_place_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Place multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit orders.
         :type transaction: Transaction
         :return: The transaction hash of the executed batch limit orders.
         :rtype: str
         """
@@ -539,15 +530,15 @@
             buy_gems=buy_gems,
             nonce=transaction.nonce,
             gas=transaction.gas,
             max_fee_per_gas=transaction.max_fee_per_gas,
             max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
         )
 
-    def batch_update_limit_orders(self, transaction: Transaction) -> str:
+    def batch_update_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Update multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order updates.
         :type transaction: Transaction
         :return: The transaction hash of the executed batch limit order updates.
         :rtype: str
         """
@@ -582,15 +573,15 @@
             buy_gems=buy_gems,
             nonce=transaction.nonce,
             gas=transaction.gas,
             max_fee_per_gas=transaction.max_fee_per_gas,
             max_priority_fee_per_gas=transaction.max_priority_fee_per_gas
         )
 
-    def batch_cancel_limit_orders(self, transaction: Transaction) -> str:
+    def batch_cancel_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Cancel multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order cancellations.
         :type transaction: Transaction
         :return: The transaction hash of the executed batch limit order cancellations.
         :rtype: str
         """
```

### Comparing `rubi-2.0.2b4/rubi/contracts/__pycache__/router.cpython-310.pyc` & `rubi-2.0.3/rubi/contracts/base_contract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,797 +1,713 @@
-00000000: 6f0d 0d0a 0000 0000 9cea 7864 4c39 0000  o.........xdL9..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
-00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 4700  ..d.d.l.m.Z...G.
-00000080: 6407 6408 8400 6408 650b 8303 5a0e 6409  d.d...d.e...Z.d.
-00000090: 5300 290a e900 0000 0029 03da 084f 7074  S.)......)...Opt
-000000a0: 696f 6e61 6cda 0554 7570 6c65 da04 4c69  ional..Tuple..Li
-000000b0: 7374 2901 da0f 4368 6563 6b73 756d 4164  st)...ChecksumAd
-000000c0: 6472 6573 7329 01da 0457 6562 3329 01da  dress)...Web3)..
-000000d0: 0843 6f6e 7472 6163 7429 01da 0c42 6173  .Contract)...Bas
-000000e0: 6543 6f6e 7472 6163 7429 01da 074e 6574  eContract)...Net
-000000f0: 776f 726b 6300 0000 0000 0000 0000 0000  workc...........
-00000100: 0000 0000 0013 0000 0000 0000 0073 2202  .............s".
-00000110: 0000 6500 5a01 6400 5a02 6401 5a03 0902  ..e.Z.d.Z.d.Z...
-00000120: 0902 6438 6403 6504 6404 6505 6405 6506  ..d8d.e.d.e.d.e.
-00000130: 6507 1900 6406 6506 6508 1900 6407 6402  e...d.e.e...d.d.
-00000140: 660a 8700 6601 6408 6409 840d 5a09 650a  f...f.d.d...Z.e.
-00000150: 0902 0902 6438 640a 650b 6405 6506 6507  ....d8d.e.d.e.e.
-00000160: 1900 6406 6506 6508 1900 6407 6400 6608  ..d.e.e...d.d.f.
-00000170: 640b 640c 8405 8301 5a0c 640d 6507 640e  d.d.....Z.d.e.d.
-00000180: 650d 6507 1900 640f 6507 6407 650e 650f  e.e...d.e.d.e.e.
-00000190: 650f 6602 1900 6608 6410 6411 8404 5a10  e.f...f.d.d...Z.
-000001a0: 6412 6507 6413 6507 640f 6507 6407 650f  d.e.d.e.d.e.d.e.
-000001b0: 6608 6414 6415 8404 5a11 6412 6507 6413  f.d.d...Z.d.e.d.
-000001c0: 6507 6407 650e 650d 650d 650f 1900 1900  e.d.e.e.e.e.....
-000001d0: 650d 650d 650f 1900 1900 6602 1900 6606  e.e.e.....f...f.
-000001e0: 6416 6417 8404 5a12 6418 6507 6419 6507  d.d...Z.d.e.d.e.
-000001f0: 6407 650e 650f 650f 6602 1900 6606 641a  d.e.e.e.f...f.d.
-00000200: 641b 8404 5a13 6412 6507 6413 6507 6407  d...Z.d.e.d.e.d.
-00000210: 650e 650f 650f 6507 650f 6507 6605 1900  e.e.e.e.e.e.f...
-00000220: 6606 641c 641d 8404 5a14 641e 650f 641f  f.d.d...Z.d.e.d.
-00000230: 650f 6420 650d 6507 1900 6407 650f 6608  e.d e.e...d.e.f.
-00000240: 6421 6422 8404 5a15 6423 650d 650f 1900  d!d"..Z.d#e.e...
-00000250: 6424 650d 650f 1900 6425 650d 650d 6507  d$e.e...d%e.e.e.
-00000260: 1900 1900 6407 650f 6608 6426 6427 8404  ....d.e.f.d&d'..
-00000270: 5a16 6428 6507 6429 650d 6507 1900 642a  Z.d(e.d)e.e...d*
-00000280: 6507 6407 650f 6608 642b 642c 8404 5a17  e.d.e.f.d+d,..Z.
-00000290: 0902 092d 0902 0902 6439 6425 650d 650d  ...-....d9d%e.e.
-000002a0: 6507 1900 1900 6423 650d 650f 1900 642e  e.....d#e.e...d.
-000002b0: 650d 650f 1900 642f 6507 6430 6506 650f  e.e...d/e.d0e.e.
-000002c0: 1900 6431 650f 6432 6506 650f 1900 6433  ..d1e.d2e.e...d3
-000002d0: 6506 650f 1900 6407 6508 6612 6434 6435  e.e...d.e.f.d4d5
-000002e0: 8405 5a18 0902 092d 0902 0902 6439 641e  ..Z....-....d9d.
-000002f0: 650f 641f 650f 6420 650d 6507 1900 642f  e.d.e.d e.e...d/
-00000300: 6507 6430 6506 650f 1900 6431 650f 6432  e.d0e.e...d1e.d2
-00000310: 6506 650f 1900 6433 6506 650f 1900 6407  e.e...d3e.e...d.
-00000320: 6508 6612 6436 6437 8405 5a19 8700 0400  e.f.d6d7..Z.....
-00000330: 5a1a 5300 293a da0d 5275 6269 636f 6e52  Z.S.):..RubiconR
-00000340: 6f75 7465 7261 2e02 0000 5468 6973 2063  outera....This c
-00000350: 6c61 7373 2072 6570 7265 7365 6e74 7320  lass represents 
-00000360: 7468 6520 5275 6269 636f 6e52 6f75 7465  the RubiconRoute
-00000370: 722e 736f 6c20 636f 6e74 7261 6374 2061  r.sol contract a
-00000380: 6e64 2062 7920 6465 6661 756c 7420 6861  nd by default ha
-00000390: 7320 7265 6164 2066 756e 6374 696f 6e61  s read functiona
-000003a0: 6c69 7479 2e0a 2020 2020 4966 2061 2077  lity..    If a w
-000003b0: 616c 6c65 7420 616e 6420 6b65 7920 6172  allet and key ar
-000003c0: 6520 7061 7373 6564 2069 6e20 696e 7374  e passed in inst
-000003d0: 616e 7469 6174 696f 6e20 7468 656e 2074  antiation then t
-000003e0: 6869 7320 636c 6173 7320 6361 6e20 616c  his class can al
-000003f0: 736f 2062 6520 7573 6564 2074 6f20 7772  so be used to wr
-00000400: 6974 6520 746f 2074 6865 2063 6f6e 7472  ite to the contr
-00000410: 6163 7420 696e 7374 616e 6365 2e0a 0a20  act instance... 
-00000420: 2020 203a 7061 7261 6d20 7733 3a20 5765     :param w3: We
-00000430: 6233 2069 6e73 7461 6e63 650a 2020 2020  b3 instance.    
-00000440: 3a74 7970 6520 7733 3a20 5765 6233 0a20  :type w3: Web3. 
-00000450: 2020 203a 7061 7261 6d20 636f 6e74 7261     :param contra
-00000460: 6374 3a20 436f 6e74 7261 6374 2069 6e73  ct: Contract ins
-00000470: 7461 6e63 650a 2020 2020 3a74 7970 6520  tance.    :type 
-00000480: 636f 6e74 7261 6374 3a20 436f 6e74 7261  contract: Contra
-00000490: 6374 0a20 2020 203a 7061 7261 6d20 7761  ct.    :param wa
-000004a0: 6c6c 6574 3a20 6120 7761 6c6c 6574 2061  llet: a wallet a
-000004b0: 6464 7265 7373 206f 6620 7468 6520 7369  ddress of the si
-000004c0: 676e 6572 2028 6f70 7469 6f6e 616c 2c20  gner (optional, 
-000004d0: 6465 6661 756c 7420 6973 204e 6f6e 6529  default is None)
-000004e0: 0a20 2020 203a 7479 7065 2077 616c 6c65  .    :type walle
-000004f0: 743a 204f 7074 696f 6e61 6c5b 4368 6563  t: Optional[Chec
-00000500: 6b73 756d 4164 6472 6573 735d 0a20 2020  ksumAddress].   
-00000510: 203a 7061 7261 6d20 6b65 793a 2074 6865   :param key: the
-00000520: 2070 7269 7661 7465 206b 6579 206f 6620   private key of 
-00000530: 7468 6520 7369 676e 6572 2028 6f70 7469  the signer (opti
-00000540: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
-00000550: 204e 6f6e 6529 0a20 2020 203a 7479 7065   None).    :type
-00000560: 206b 6579 3a20 4f70 7469 6f6e 616c 5b73   key: Optional[s
-00000570: 7472 5d0a 2020 2020 4eda 0277 33da 0863  tr].    N..w3..c
-00000580: 6f6e 7472 6163 74da 0677 616c 6c65 74da  ontract..wallet.
-00000590: 036b 6579 da06 7265 7475 726e 6305 0000  .key..returnc...
-000005a0: 0000 0000 0000 0000 0005 0000 0006 0000  ................
-000005b0: 0003 0000 0073 1800 0000 7400 8300 6a01  .....s....t...j.
-000005c0: 7c01 7c02 7c03 7c04 6401 8d04 0100 6402  |.|.|.|.d.....d.
-000005d0: 5300 2903 7a12 636f 6e73 7472 7563 746f  S.).z.constructo
-000005e0: 7220 6d65 7468 6f64 2904 720b 0000 0072  r method).r....r
-000005f0: 0c00 0000 720d 0000 0072 0e00 0000 4e29  ....r....r....N)
-00000600: 02da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
-00000610: 5f5f 2905 da04 7365 6c66 720b 0000 0072  __)...selfr....r
-00000620: 0c00 0000 720d 0000 0072 0e00 0000 a901  ....r....r......
-00000630: da09 5f5f 636c 6173 735f 5fa9 00fa 422f  ..__class__...B/
-00000640: 5573 6572 732f 6465 6e76 6572 2f44 6f63  Users/denver/Doc
-00000650: 756d 656e 7473 2f6f 7065 6e2f 7275 6269  uments/open/rubi
-00000660: 2d70 792f 7275 6269 2f72 7562 692f 636f  -py/rubi/rubi/co
-00000670: 6e74 7261 6374 732f 726f 7574 6572 2e70  ntracts/router.p
-00000680: 7972 1100 0000 1900 0000 730c 0000 0006  yr........s.....
-00000690: 0802 0102 0102 0102 010a fc7a 1652 7562  ...........z.Rub
-000006a0: 6963 6f6e 526f 7574 6572 2e5f 5f69 6e69  iconRouter.__ini
-000006b0: 745f 5fda 076e 6574 776f 726b 6304 0000  t__..networkc...
-000006c0: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-000006d0: 0043 0000 0073 2200 0000 7c00 6a00 7c01  .C...s"...|.j.|.
-000006e0: 6a01 7c01 6a02 6a03 6a04 7c01 6a02 6a03  j.|.j.j.j.|.j.j.
-000006f0: 6a05 7c02 7c03 6401 8d05 5300 2902 6114  j.|.|.d...S.).a.
-00000700: 0200 0043 7265 6174 6520 6120 5275 6269  ...Create a Rubi
-00000710: 636f 6e52 6f75 7465 7220 696e 7374 616e  conRouter instan
-00000720: 6365 2062 6173 6564 206f 6e20 6120 4e65  ce based on a Ne
-00000730: 7477 6f72 6b20 696e 7374 616e 6365 2e0a  twork instance..
-00000740: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000750: 6e65 7477 6f72 6b3a 2041 204e 6574 776f  network: A Netwo
-00000760: 726b 2069 6e73 7461 6e63 652e 0a20 2020  rk instance..   
-00000770: 2020 2020 203a 7479 7065 206e 6574 776f       :type netwo
-00000780: 726b 3a20 4e65 7477 6f72 6b0a 2020 2020  rk: Network.    
-00000790: 2020 2020 3a70 6172 616d 2077 616c 6c65      :param walle
-000007a0: 743a 204f 7074 696f 6e61 6c20 7761 6c6c  t: Optional wall
-000007b0: 6574 2061 6464 7265 7373 2074 6f20 7573  et address to us
-000007c0: 6520 666f 7220 696e 7465 7261 6374 696e  e for interactin
-000007d0: 6720 7769 7468 2074 6865 2063 6f6e 7472  g with the contr
-000007e0: 6163 7420 286f 7074 696f 6e61 6c2c 2064  act (optional, d
-000007f0: 6566 6175 6c74 2069 7320 4e6f 6e65 292e  efault is None).
-00000800: 200a 2020 2020 2020 2020 3a74 7970 6520   .        :type 
-00000810: 7761 6c6c 6574 3a20 4f70 7469 6f6e 616c  wallet: Optional
-00000820: 5b43 6865 636b 7375 6d41 6464 7265 7373  [ChecksumAddress
-00000830: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-00000840: 206b 6579 3a20 4f70 7469 6f6e 616c 2070   key: Optional p
-00000850: 7269 7661 7465 206b 6579 2066 6f72 2074  rivate key for t
-00000860: 6865 2077 616c 6c65 7420 286f 7074 696f  he wallet (optio
-00000870: 6e61 6c2c 2064 6566 6175 6c74 2069 7320  nal, default is 
-00000880: 4e6f 6e65 292e 0a20 2020 2020 2020 203a  None)..        :
-00000890: 7479 7065 206b 6579 3a20 4f70 7469 6f6e  type key: Option
-000008a0: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
-000008b0: 3a72 6574 7572 6e3a 2041 2052 7562 6963  :return: A Rubic
-000008c0: 6f6e 526f 7574 6572 2069 6e73 7461 6e63  onRouter instanc
-000008d0: 6520 6261 7365 6420 6f6e 2074 6865 204e  e based on the N
-000008e0: 6574 776f 726b 2069 6e73 7461 6e63 652e  etwork instance.
-000008f0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00000900: 2052 7562 6963 6f6e 526f 7574 6572 0a20   RubiconRouter. 
-00000910: 2020 2020 2020 2029 0572 0b00 0000 da07         ).r......
-00000920: 6164 6472 6573 73da 0c63 6f6e 7472 6163  address..contrac
-00000930: 745f 6162 6972 0d00 0000 720e 0000 0029  t_abir....r....)
-00000940: 06da 1466 726f 6d5f 6164 6472 6573 735f  ...from_address_
-00000950: 616e 645f 6162 6972 0b00 0000 da07 7275  and_abir......ru
-00000960: 6269 636f 6eda 0672 6f75 7465 7272 1800  bicon..routerr..
-00000970: 0000 da03 6162 6929 04da 0363 6c73 7217  ....abi)...clsr.
-00000980: 0000 0072 0d00 0000 720e 0000 0072 1500  ...r....r....r..
-00000990: 0000 7215 0000 0072 1600 0000 da0c 6672  ..r....r......fr
-000009a0: 6f6d 5f6e 6574 776f 726b 2800 0000 730e  om_network(...s.
-000009b0: 0000 0004 1204 0108 0108 0102 0102 0106  ................
-000009c0: fb7a 1a52 7562 6963 6f6e 526f 7574 6572  .z.RubiconRouter
-000009d0: 2e66 726f 6d5f 6e65 7477 6f72 6bda 0a62  .from_network..b
-000009e0: 6173 655f 746f 6b65 6eda 0674 6f6b 656e  ase_token..token
-000009f0: 73da 056d 616b 6572 6304 0000 0000 0000  s..makerc.......
-00000a00: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-00000a10: 00f3 1600 0000 7c00 6a00 6a01 a002 7c01  ......|.j.j...|.
-00000a20: 7c02 7c03 a103 a003 a100 5300 2901 6149  |.|.......S.).aI
-00000a30: 0200 0049 7465 7261 7465 7320 7468 726f  ...Iterates thro
-00000a40: 7567 6820 616c 6c20 7468 6520 6261 7365  ugh all the base
-00000a50: 5f74 6f6b 656e 2f74 6f6b 656e 735b 695d  _token/tokens[i]
-00000a60: 206f 6666 6572 7320 6f66 2074 6865 206d   offers of the m
-00000a70: 616b 6572 2061 6e64 2072 6574 7572 6e73  aker and returns
-00000a80: 2074 6865 2062 616c 616e 6365 206f 6620   the balance of 
-00000a90: 7468 6520 6261 7365 5f74 6f6b 656e 0a20  the base_token. 
-00000aa0: 2020 2020 2020 2069 6e20 7468 6520 626f         in the bo
-00000ab0: 6f6b 2061 6e64 2074 6865 2062 616c 616e  ok and the balan
-00000ac0: 6365 206f 6620 7468 6520 6261 7365 2074  ce of the base t
-00000ad0: 6f6b 656e 2e0a 0a20 2020 2020 2020 203a  oken...        :
-00000ae0: 7061 7261 6d20 6261 7365 5f74 6f6b 656e  param base_token
-00000af0: 3a20 5468 6520 6164 6472 6573 7320 6f66  : The address of
-00000b00: 2074 6865 2062 6173 6520 746f 6b65 6e2e   the base token.
-00000b10: 0a20 2020 2020 2020 203a 7479 7065 2062  .        :type b
-00000b20: 6173 655f 746f 6b65 6e3a 2043 6865 636b  ase_token: Check
-00000b30: 7375 6d41 6464 7265 7373 0a20 2020 2020  sumAddress.     
-00000b40: 2020 203a 7061 7261 6d20 746f 6b65 6e73     :param tokens
-00000b50: 3a20 4120 6c69 7374 206f 6620 616c 6c20  : A list of all 
-00000b60: 7468 6520 746f 6b65 6e73 2074 6f20 6361  the tokens to ca
-00000b70: 6c63 756c 6174 6520 7468 6520 6261 6c61  lculate the bala
-00000b80: 6e63 6520 6f66 0a20 2020 2020 2020 203a  nce of.        :
-00000b90: 7479 7065 2074 6f6b 656e 733a 204c 6973  type tokens: Lis
-00000ba0: 745b 4368 6563 6b73 756d 4164 6472 6573  t[ChecksumAddres
-00000bb0: 735d 0a20 2020 2020 2020 203a 7061 7261  s].        :para
-00000bc0: 6d20 6d61 6b65 723a 2054 6865 2061 6464  m maker: The add
-00000bd0: 7265 7373 206f 6620 7468 6520 6d61 6b65  ress of the make
-00000be0: 7220 746f 2066 6574 2074 6865 2062 616c  r to fet the bal
-00000bf0: 616e 6365 2066 6f72 0a20 2020 2020 2020  ance for.       
-00000c00: 203a 7479 7065 206d 616b 6572 3a20 4368   :type maker: Ch
-00000c10: 6563 6b73 756d 4164 6472 6573 730a 2020  ecksumAddress.  
-00000c20: 2020 2020 2020 3a72 6574 7572 6e3a 2062        :return: b
-00000c30: 616c 616e 6365 2069 6e20 626f 6f6b 2c20  alance in book, 
-00000c40: 746f 7461 6c20 746f 6b65 6e20 6261 6c61  total token bala
-00000c50: 6e63 650a 2020 2020 2020 2020 3a72 7479  nce.        :rty
-00000c60: 7065 3a20 5475 706c 655b 696e 742c 2069  pe: Tuple[int, i
-00000c70: 6e74 5d0a 2020 2020 2020 2020 2904 720c  nt].        ).r.
-00000c80: 0000 00da 0966 756e 6374 696f 6e73 5a0f  .....functionsZ.
-00000c90: 6765 744d 616b 6572 4261 6c61 6e63 65da  getMakerBalance.
-00000ca0: 0463 616c 6c29 0472 1200 0000 7220 0000  .call).r....r ..
-00000cb0: 0072 2100 0000 7222 0000 0072 1500 0000  .r!...r"...r....
-00000cc0: 7215 0000 0072 1600 0000 da11 6765 745f  r....r......get_
-00000cd0: 6d61 6b65 725f 6261 6c61 6e63 6548 0000  maker_balanceH..
-00000ce0: 00f3 0200 0000 1613 7a1f 5275 6269 636f  ........z.Rubico
-00000cf0: 6e52 6f75 7465 722e 6765 745f 6d61 6b65  nRouter.get_make
-00000d00: 725f 6261 6c61 6e63 65da 0561 7373 6574  r_balance..asset
-00000d10: da05 7175 6f74 6563 0400 0000 0000 0000  ..quotec........
-00000d20: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
-00000d30: 7223 0000 0029 0161 bd01 0000 5265 7472  r#...).a....Retr
-00000d40: 6965 7665 7320 7468 6520 6261 6c61 6e63  ieves the balanc
-00000d50: 6520 6f66 2061 2073 7065 6369 6669 6320  e of a specific 
-00000d60: 6d61 6b65 7220 666f 7220 6120 6769 7665  maker for a give
-00000d70: 6e20 6173 7365 742f 7175 6f74 6520 7061  n asset/quote pa
-00000d80: 6972 2e0a 0a20 2020 2020 2020 203a 7061  ir...        :pa
-00000d90: 7261 6d20 6173 7365 743a 2054 6865 2061  ram asset: The a
-00000da0: 6464 7265 7373 206f 6620 7468 6520 6173  ddress of the as
-00000db0: 7365 7420 746f 6b65 6e2e 0a20 2020 2020  set token..     
-00000dc0: 2020 203a 7479 7065 2061 7373 6574 3a20     :type asset: 
-00000dd0: 4368 6563 6b73 756d 4164 6472 6573 730a  ChecksumAddress.
-00000de0: 2020 2020 2020 2020 3a70 6172 616d 2071          :param q
-00000df0: 756f 7465 3a20 5468 6520 6164 6472 6573  uote: The addres
-00000e00: 7320 6f66 2074 6865 2071 756f 7465 2074  s of the quote t
-00000e10: 6f6b 656e 2e0a 2020 2020 2020 2020 3a74  oken..        :t
-00000e20: 7970 6520 7175 6f74 653a 2043 6865 636b  ype quote: Check
-00000e30: 7375 6d41 6464 7265 7373 0a20 2020 2020  sumAddress.     
-00000e40: 2020 203a 7061 7261 6d20 6d61 6b65 723a     :param maker:
-00000e50: 2054 6865 2061 6464 7265 7373 206f 6620   The address of 
-00000e60: 7468 6520 6d61 6b65 722e 0a20 2020 2020  the maker..     
-00000e70: 2020 203a 7479 7065 206d 616b 6572 3a20     :type maker: 
-00000e80: 4368 6563 6b73 756d 4164 6472 6573 730a  ChecksumAddress.
-00000e90: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000ea0: 2054 6865 2062 616c 616e 6365 206f 6620   The balance of 
-00000eb0: 7468 6520 6d61 6b65 7220 696e 2074 6865  the maker in the
-00000ec0: 2073 7065 6369 6669 6564 2061 7373 6574   specified asset
-00000ed0: 2f71 756f 7465 2070 6169 722e 0a20 2020  /quote pair..   
-00000ee0: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-00000ef0: 0a20 2020 2020 2020 2029 0472 0c00 0000  .        ).r....
-00000f00: 7224 0000 005a 1567 6574 4d61 6b65 7242  r$...Z.getMakerB
-00000f10: 616c 616e 6365 496e 5061 6972 7225 0000  alanceInPairr%..
-00000f20: 0029 0472 1200 0000 7228 0000 0072 2900  .).r....r(...r).
-00000f30: 0000 7222 0000 0072 1500 0000 7215 0000  ..r"...r....r...
-00000f40: 0072 1600 0000 da19 6765 745f 6d61 6b65  .r......get_make
-00000f50: 725f 6261 6c61 6e63 655f 696e 5f70 6169  r_balance_in_pai
-00000f60: 725e 0000 00f3 0200 0000 1612 7a27 5275  r^..........z'Ru
-00000f70: 6269 636f 6e52 6f75 7465 722e 6765 745f  biconRouter.get_
-00000f80: 6d61 6b65 725f 6261 6c61 6e63 655f 696e  maker_balance_in
-00000f90: 5f70 6169 7263 0300 0000 0000 0000 0000  _pairc..........
-00000fa0: 0000 0300 0000 0400 0000 4300 0000 f314  ..........C.....
-00000fb0: 0000 007c 006a 006a 01a0 027c 017c 02a1  ...|.j.j...|.|..
-00000fc0: 02a0 03a1 0053 0029 0161 7802 0000 5265  .....S.).ax...Re
-00000fd0: 7472 6965 7665 7320 7468 6520 6f72 6465  trieves the orde
-00000fe0: 7220 626f 6f6b 2066 6f72 2061 2073 7065  r book for a spe
-00000ff0: 6369 6669 6320 6173 7365 742f 7175 6f74  cific asset/quot
-00001000: 6520 7061 6972 2e0a 0a20 2020 2020 2020  e pair...       
-00001010: 203a 7061 7261 6d20 6173 7365 743a 2054   :param asset: T
-00001020: 6865 2061 6464 7265 7373 206f 6620 7468  he address of th
-00001030: 6520 6173 7365 7420 746f 6b65 6e2e 0a20  e asset token.. 
-00001040: 2020 2020 2020 203a 7479 7065 2061 7373         :type ass
-00001050: 6574 3a20 4368 6563 6b73 756d 4164 6472  et: ChecksumAddr
-00001060: 6573 730a 2020 2020 2020 2020 3a70 6172  ess.        :par
-00001070: 616d 2071 756f 7465 3a20 5468 6520 6164  am quote: The ad
-00001080: 6472 6573 7320 6f66 2074 6865 2071 756f  dress of the quo
-00001090: 7465 2074 6f6b 656e 2e0a 2020 2020 2020  te token..      
-000010a0: 2020 3a74 7970 6520 7175 6f74 653a 2043    :type quote: C
-000010b0: 6865 636b 7375 6d41 6464 7265 7373 0a20  hecksumAddress. 
-000010c0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-000010d0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
-000010e0: 6e67 2074 776f 206c 6973 7473 3a20 6173  ng two lists: as
-000010f0: 6b73 2061 6e64 2062 6964 732e 2045 6163  ks and bids. Eac
-00001100: 6820 6c69 7374 2063 6f6e 7461 696e 7320  h list contains 
-00001110: 6120 7375 626c 6973 7420 6f66 206c 656e  a sublist of len
-00001120: 6774 6820 332c 2072 6570 7265 7365 6e74  gth 3, represent
-00001130: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00001140: 7468 6520 6f72 6465 7220 626f 6f6b 2065  the order book e
-00001150: 6e74 7269 6573 2069 6e20 7468 6520 666f  ntries in the fo
-00001160: 6c6c 6f77 696e 6720 666f 726d 6174 2028  llowing format (
-00001170: 7061 795f 616d 742c 2062 7579 5f61 6d74  pay_amt, buy_amt
-00001180: 2c20 6964 292e 2054 6865 2061 736b 7320  , id). The asks 
-00001190: 6c69 7374 2072 6570 7265 7365 6e74 7320  list represents 
-000011a0: 7468 6520 6f72 6465 7273 0a20 2020 2020  the orders.     
-000011b0: 2020 2020 2020 2073 656c 6c69 6e67 2074         selling t
-000011c0: 6865 2061 7373 6574 2c20 7768 696c 6520  he asset, while 
-000011d0: 7468 6520 6269 6473 206c 6973 7420 7265  the bids list re
-000011e0: 7072 6573 656e 7473 2074 6865 206f 7264  presents the ord
-000011f0: 6572 7320 6275 7969 6e67 2074 6865 2061  ers buying the a
-00001200: 7373 6574 2e0a 2020 2020 2020 2020 3a72  sset..        :r
-00001210: 7479 7065 3a20 5475 706c 655b 4c69 7374  type: Tuple[List
-00001220: 5b4c 6973 745b 696e 745d 5d2c 204c 6973  [List[int]], Lis
-00001230: 745b 4c69 7374 5b69 6e74 5d5d 5d0a 2020  t[List[int]]].  
-00001240: 2020 2020 2020 2904 720c 0000 0072 2400        ).r....r$.
-00001250: 0000 5a0f 6765 7442 6f6f 6b46 726f 6d50  ..Z.getBookFromP
-00001260: 6169 7272 2500 0000 a903 7212 0000 0072  airr%.....r....r
-00001270: 2800 0000 7229 0000 0072 1500 0000 7215  (...r)...r....r.
-00001280: 0000 0072 1600 0000 da12 6765 745f 626f  ...r......get_bo
-00001290: 6f6b 5f66 726f 6d5f 7061 6972 7300 0000  ok_from_pairs...
-000012a0: 7302 0000 0014 117a 2052 7562 6963 6f6e  s......z Rubicon
-000012b0: 526f 7574 6572 2e67 6574 5f62 6f6f 6b5f  Router.get_book_
-000012c0: 6672 6f6d 5f70 6169 72da 0874 6f6b 656e  from_pair..token
-000012d0: 5f69 6eda 0974 6f6b 656e 5f6f 7574 6303  _in..token_outc.
-000012e0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000012f0: 0000 0043 0000 0072 2c00 0000 2901 61cf  ...C...r,...).a.
-00001300: 0100 0052 6574 7269 6576 6573 2074 6865  ...Retrieves the
-00001310: 2064 6570 7468 206f 6620 6f6e 6520 7369   depth of one si
-00001320: 6465 206f 6620 7468 6520 6f72 6465 7220  de of the order 
-00001330: 626f 6f6b 2066 6f72 2061 2073 7065 6369  book for a speci
-00001340: 6669 6320 746f 6b65 6e20 7061 6972 2061  fic token pair a
-00001350: 6c6f 6e67 2077 6974 6820 7468 6520 6964  long with the id
-00001360: 206f 6620 7468 6520 6265 7374 0a20 2020   of the best.   
-00001370: 2020 2020 206f 6666 6572 2e0a 0a20 2020       offer...   
-00001380: 2020 2020 203a 7061 7261 6d20 746f 6b65       :param toke
-00001390: 6e5f 696e 3a20 5468 6520 6164 6472 6573  n_in: The addres
-000013a0: 7320 6f66 2074 6865 2071 756f 7465 2e0a  s of the quote..
-000013b0: 2020 2020 2020 2020 3a74 7970 6520 746f          :type to
-000013c0: 6b65 6e5f 696e 3a20 4368 6563 6b73 756d  ken_in: Checksum
-000013d0: 4164 6472 6573 730a 2020 2020 2020 2020  Address.        
-000013e0: 3a70 6172 616d 2074 6f6b 656e 5f6f 7574  :param token_out
-000013f0: 3a20 5468 6520 6164 6472 6573 7320 6f66  : The address of
-00001400: 2074 6865 2061 7373 6574 2e0a 2020 2020   the asset..    
-00001410: 2020 2020 3a74 7970 6520 746f 6b65 6e5f      :type token_
-00001420: 6f75 743a 2043 6865 636b 7375 6d41 6464  out: ChecksumAdd
-00001430: 7265 7373 0a20 2020 2020 2020 203a 7265  ress.        :re
-00001440: 7475 726e 3a20 4120 7475 706c 6520 636f  turn: A tuple co
-00001450: 6e74 6169 6e69 6e67 2074 6865 2064 6570  ntaining the dep
-00001460: 7468 206f 6620 7468 6520 6f72 6465 7220  th of the order 
-00001470: 626f 6f6b 2061 6e64 2074 6865 2049 4420  book and the ID 
-00001480: 6f66 2074 6865 2062 6573 7420 6f66 6665  of the best offe
-00001490: 7220 666f 7220 746f 6b65 6e5f 6f75 742f  r for token_out/
-000014a0: 746f 6b65 6e5f 696e 2e0a 2020 2020 2020  token_in..      
-000014b0: 2020 3a72 7479 7065 3a20 5475 706c 655b    :rtype: Tuple[
-000014c0: 696e 742c 2069 6e74 5d0a 2020 2020 2020  int, int].      
-000014d0: 2020 2904 720c 0000 0072 2400 0000 5a0c    ).r....r$...Z.
-000014e0: 6765 7442 6f6f 6b44 6570 7468 7225 0000  getBookDepthr%..
-000014f0: 0029 0372 1200 0000 722f 0000 0072 3000  .).r....r/...r0.
-00001500: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001510: 00da 0e67 6574 5f62 6f6f 6b5f 6465 7074  ...get_book_dept
-00001520: 6887 0000 0073 0200 0000 140c 7a1c 5275  h....s......z.Ru
-00001530: 6269 636f 6e52 6f75 7465 722e 6765 745f  biconRouter.get_
-00001540: 626f 6f6b 5f64 6570 7468 6303 0000 0000  book_depthc.....
-00001550: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00001560: 0000 0072 2c00 0000 2901 61fa 0100 0052  ...r,...).a....R
-00001570: 6574 7269 6576 6573 2074 6865 2069 6e66  etrieves the inf
-00001580: 6f72 6d61 7469 6f6e 2061 6e64 2069 6420  ormation and id 
-00001590: 6f66 2074 6865 2062 6573 7420 6f66 6665  of the best offe
-000015a0: 7220 666f 7220 6120 7370 6563 6966 6963  r for a specific
-000015b0: 2061 7373 6574 2f71 756f 7465 2070 6169   asset/quote pai
-000015c0: 722e 0a0a 2020 2020 2020 2020 3a70 6172  r...        :par
-000015d0: 616d 2061 7373 6574 3a20 5468 6520 6164  am asset: The ad
-000015e0: 6472 6573 7320 6f66 2074 6865 2061 7373  dress of the ass
-000015f0: 6574 2074 6f6b 656e 2e0a 2020 2020 2020  et token..      
-00001600: 2020 3a74 7970 6520 6173 7365 743a 2043    :type asset: C
-00001610: 6865 636b 7375 6d41 6464 7265 7373 0a20  hecksumAddress. 
-00001620: 2020 2020 2020 203a 7061 7261 6d20 7175         :param qu
-00001630: 6f74 653a 2054 6865 2061 6464 7265 7373  ote: The address
-00001640: 206f 6620 7468 6520 7175 6f74 6520 746f   of the quote to
-00001650: 6b65 6e2e 0a20 2020 2020 2020 203a 7479  ken..        :ty
-00001660: 7065 2071 756f 7465 3a20 4368 6563 6b73  pe quote: Checks
-00001670: 756d 4164 6472 6573 730a 2020 2020 2020  umAddress.      
-00001680: 2020 3a72 6574 7572 6e3a 2041 2074 7570    :return: A tup
-00001690: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
-000016a0: 6520 4944 206f 6620 7468 6520 6265 7374  e ID of the best
-000016b0: 206f 6666 6572 2c20 7468 6520 7061 795f   offer, the pay_
-000016c0: 616d 742c 2074 6865 2061 6464 7265 7373  amt, the address
-000016d0: 206f 6620 7468 6520 7061 795f 6765 6d2c   of the pay_gem,
-000016e0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-000016f0: 2062 7579 5f61 6d74 2c20 616e 6420 7468   buy_amt, and th
-00001700: 6520 6164 6472 6573 7320 6f66 2074 6865  e address of the
-00001710: 2062 7579 5f67 656d 2e0a 2020 2020 2020   buy_gem..      
-00001720: 2020 3a72 7479 7065 3a20 5475 706c 655b    :rtype: Tuple[
-00001730: 696e 742c 2069 6e74 2c20 4368 6563 6b73  int, int, Checks
-00001740: 756d 4164 6472 6573 732c 2069 6e74 2c20  umAddress, int, 
-00001750: 4368 6563 6b73 756d 4164 6472 6573 735d  ChecksumAddress]
-00001760: 0a20 2020 2020 2020 2029 0472 0c00 0000  .        ).r....
-00001770: 7224 0000 005a 1367 6574 4265 7374 4f66  r$...Z.getBestOf
-00001780: 6665 7241 6e64 496e 666f 7225 0000 0072  ferAndInfor%...r
-00001790: 2d00 0000 7215 0000 0072 1500 0000 7216  -...r....r....r.
-000017a0: 0000 00da 1767 6574 5f62 6573 745f 6f66  .....get_best_of
-000017b0: 6665 725f 616e 645f 696e 666f 9600 0000  fer_and_info....
-000017c0: 7302 0000 0014 107a 2552 7562 6963 6f6e  s......z%Rubicon
-000017d0: 526f 7574 6572 2e67 6574 5f62 6573 745f  Router.get_best_
-000017e0: 6f66 6665 725f 616e 645f 696e 666f da07  offer_and_info..
-000017f0: 7061 795f 616d 74da 0b62 7579 5f61 6d74  pay_amt..buy_amt
-00001800: 5f6d 696e da05 726f 7574 6563 0400 0000  _min..routec....
-00001810: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00001820: 4300 0000 7223 0000 0029 0161 2602 0000  C...r#...).a&...
-00001830: 4573 7469 6d61 7465 7320 7468 6520 6578  Estimates the ex
-00001840: 7065 6374 6564 2061 6d6f 756e 7420 696e  pected amount in
-00001850: 636c 7564 696e 6720 6665 6573 2077 6865  cluding fees whe
-00001860: 6e20 7377 6170 7069 6e67 2074 6865 2073  n swapping the s
-00001870: 7065 6369 6669 6564 2070 6179 6d65 6e74  pecified payment
-00001880: 2061 6d6f 756e 7420 7573 696e 6720 7468   amount using th
-00001890: 6520 7370 6563 6966 6965 640a 2020 2020  e specified.    
-000018a0: 2020 2020 726f 7574 652e 2072 6576 6572      route. rever
-000018b0: 7473 2077 6974 6820 616e 2065 7863 6570  ts with an excep
-000018c0: 7469 6f6e 2069 6620 7468 6520 7377 6170  tion if the swap
-000018d0: 2063 616e 6e6f 7420 6163 6869 6576 6520   cannot achieve 
-000018e0: 7468 6520 6275 795f 616d 745f 6d69 6e0a  the buy_amt_min.
-000018f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001900: 7061 795f 616d 743a 2054 6865 2070 6179  pay_amt: The pay
-00001910: 6d65 6e74 2061 6d6f 756e 742e 0a20 2020  ment amount..   
-00001920: 2020 2020 203a 7479 7065 2070 6179 5f61       :type pay_a
-00001930: 6d74 3a20 696e 740a 2020 2020 2020 2020  mt: int.        
-00001940: 3a70 6172 616d 2062 7579 5f61 6d74 5f6d  :param buy_amt_m
-00001950: 696e 3a20 5468 6520 6d69 6e69 6d75 6d20  in: The minimum 
-00001960: 6275 7920 616d 6f75 6e74 2e0a 2020 2020  buy amount..    
-00001970: 2020 2020 3a74 7970 6520 6275 795f 616d      :type buy_am
-00001980: 745f 6d69 6e3a 2069 6e74 0a20 2020 2020  t_min: int.     
-00001990: 2020 203a 7061 7261 6d20 726f 7574 653a     :param route:
-000019a0: 2054 6865 2072 6f75 7465 206f 6620 6164   The route of ad
-000019b0: 6472 6573 7365 7320 7265 7072 6573 656e  dresses represen
-000019c0: 7469 6e67 2074 6865 2073 7761 7020 7061  ting the swap pa
-000019d0: 7468 2e0a 2020 2020 2020 2020 3a74 7970  th..        :typ
-000019e0: 6520 726f 7574 653a 204c 6973 745b 4368  e route: List[Ch
-000019f0: 6563 6b73 756d 4164 6472 6573 735d 0a20  ecksumAddress]. 
-00001a00: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00001a10: 5468 6520 6573 7469 6d61 7465 6420 7377  The estimated sw
-00001a20: 6170 2061 6d6f 756e 7420 696e 636c 7564  ap amount includ
-00001a30: 696e 6720 6665 6573 2e0a 2020 2020 2020  ing fees..      
-00001a40: 2020 3a72 7479 7065 3a20 696e 740a 2020    :rtype: int.  
-00001a50: 2020 2020 2020 2904 720c 0000 0072 2400        ).r....r$.
-00001a60: 0000 5a13 6765 7445 7870 6563 7465 6453  ..Z.getExpectedS
-00001a70: 7761 7046 696c 6c72 2500 0000 2904 7212  wapFillr%...).r.
-00001a80: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
-00001a90: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001aa0: 00da 1667 6574 5f65 7870 6563 7465 645f  ...get_expected_
-00001ab0: 7377 6170 5f66 696c 6ca9 0000 0073 0200  swap_fill....s..
-00001ac0: 0000 160e 7a24 5275 6269 636f 6e52 6f75  ....z$RubiconRou
-00001ad0: 7465 722e 6765 745f 6578 7065 6374 6564  ter.get_expected
-00001ae0: 5f73 7761 705f 6669 6c6c da08 7061 795f  _swap_fill..pay_
-00001af0: 616d 7473 da0c 6275 795f 616d 745f 6d69  amts..buy_amt_mi
-00001b00: 6e73 da06 726f 7574 6573 6304 0000 0000  ns..routesc.....
-00001b10: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
-00001b20: 0000 0072 2300 0000 2901 61aa 0200 0045  ...r#...).a....E
-00001b30: 7374 696d 6174 6573 2074 6865 2065 7870  stimates the exp
-00001b40: 6563 7465 6420 616d 6f75 6e74 2069 6e63  ected amount inc
-00001b50: 6c75 6469 6e67 2066 6565 7320 7768 656e  luding fees when
-00001b60: 2073 7761 7070 696e 6720 6d75 6c74 6970   swapping multip
-00001b70: 6c65 2073 7065 6369 6669 6564 2070 6179  le specified pay
-00001b80: 6d65 6e74 2061 6d6f 756e 7420 7573 696e  ment amount usin
-00001b90: 6720 6d75 6c74 6970 6c65 0a20 2020 2020  g multiple.     
-00001ba0: 2020 2073 7065 6369 6669 6564 2072 6f75     specified rou
-00001bb0: 7465 732e 2072 6576 6572 7473 2077 6974  tes. reverts wit
-00001bc0: 6820 616e 2065 7863 6570 7469 6f6e 2069  h an exception i
-00001bd0: 6620 7468 6520 6d75 6c74 6973 7761 7020  f the multiswap 
-00001be0: 6361 6e6e 6f74 2061 6368 6965 7665 2074  cannot achieve t
-00001bf0: 6865 2062 7579 5f61 6d74 5f6d 696e 7320  he buy_amt_mins 
-00001c00: 616c 6f6e 6720 6561 6368 2072 6f75 7465  along each route
-00001c10: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00001c20: 2070 6179 5f61 6d74 733a 2054 6865 206c   pay_amts: The l
-00001c30: 6973 7420 6f66 2070 6179 6d65 6e74 2061  ist of payment a
-00001c40: 6d6f 756e 7473 2066 6f72 2065 6163 6820  mounts for each 
-00001c50: 7377 6170 2e0a 2020 2020 2020 2020 3a74  swap..        :t
-00001c60: 7970 6520 7061 795f 616d 7473 3a20 4c69  ype pay_amts: Li
-00001c70: 7374 5b69 6e74 5d0a 2020 2020 2020 2020  st[int].        
-00001c80: 3a70 6172 616d 2062 7579 5f61 6d74 5f6d  :param buy_amt_m
-00001c90: 696e 733a 2054 6865 206c 6973 7420 6f66  ins: The list of
-00001ca0: 206d 696e 696d 756d 2062 7579 2061 6d6f   minimum buy amo
-00001cb0: 756e 7473 2066 6f72 2065 6163 6820 7377  unts for each sw
-00001cc0: 6170 2e0a 2020 2020 2020 2020 3a74 7970  ap..        :typ
-00001cd0: 6520 6275 795f 616d 745f 6d69 6e73 3a20  e buy_amt_mins: 
-00001ce0: 4c69 7374 5b69 6e74 5d0a 2020 2020 2020  List[int].      
-00001cf0: 2020 3a70 6172 616d 2072 6f75 7465 733a    :param routes:
-00001d00: 2054 6865 206c 6973 7420 6f66 2072 6f75   The list of rou
-00001d10: 7465 732c 2077 6865 7265 2065 6163 6820  tes, where each 
-00001d20: 726f 7574 6520 6973 2061 206c 6973 7420  route is a list 
-00001d30: 6f66 2061 6464 7265 7373 6573 2072 6570  of addresses rep
-00001d40: 7265 7365 6e74 696e 6720 7468 6520 7377  resenting the sw
-00001d50: 6170 2070 6174 682e 0a20 2020 2020 2020  ap path..       
-00001d60: 203a 7479 7065 2072 6f75 7465 733a 204c   :type routes: L
-00001d70: 6973 745b 4c69 7374 5b43 6865 636b 7375  ist[List[Checksu
-00001d80: 6d41 6464 7265 7373 5d5d 0a20 2020 2020  mAddress]].     
-00001d90: 2020 203a 7265 7475 726e 3a20 5468 6520     :return: The 
-00001da0: 6573 7469 6d61 7465 6420 6d75 6c74 692d  estimated multi-
-00001db0: 7377 6170 2061 6d6f 756e 742e 0a20 2020  swap amount..   
-00001dc0: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-00001dd0: 0a20 2020 2020 2020 2029 0472 0c00 0000  .        ).r....
-00001de0: 7224 0000 005a 1867 6574 4578 7065 6374  r$...Z.getExpect
-00001df0: 6564 4d75 6c74 6973 7761 7046 696c 6c72  edMultiswapFillr
-00001e00: 2500 0000 2904 7212 0000 0072 3700 0000  %...).r....r7...
-00001e10: 7238 0000 0072 3900 0000 7215 0000 0072  r8...r9...r....r
-00001e20: 1500 0000 7216 0000 00da 1b67 6574 5f65  ....r......get_e
-00001e30: 7870 6563 7465 645f 6d75 6c74 6973 7761  xpected_multiswa
-00001e40: 705f 6669 6c6c bb00 0000 7227 0000 007a  p_fill....r'...z
-00001e50: 2952 7562 6963 6f6e 526f 7574 6572 2e67  )RubiconRouter.g
-00001e60: 6574 5f65 7870 6563 7465 645f 6d75 6c74  et_expected_mult
-00001e70: 6973 7761 705f 6669 6c6c da04 7573 6572  iswap_fill..user
-00001e80: da12 7461 7267 6574 5f62 6174 685f 746f  ..target_bath_to
-00001e90: 6b65 6e73 da05 746f 6b65 6e63 0400 0000  kens..tokenc....
-00001ea0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00001eb0: 4300 0000 7223 0000 0029 0161 1202 0000  C...r#...).a....
-00001ec0: 4368 6563 6b73 2074 6865 2061 6c6c 2062  Checks the all b
-00001ed0: 6f6e 7573 2074 6f6b 656e 7320 7468 6174  onus tokens that
-00001ee0: 2063 616e 2062 6520 636c 6169 6d65 6420   can be claimed 
-00001ef0: 6279 2061 2075 7365 7220 6561 726e 6564  by a user earned
-00001f00: 2061 6372 6f73 7320 616c 6c20 7370 6563   across all spec
-00001f10: 6966 6965 6420 7275 6269 636f 6e20 706f  ified rubicon po
-00001f20: 6f6c 732e 0a0a 2020 2020 2020 2020 3a70  ols...        :p
-00001f30: 6172 616d 2075 7365 723a 2054 6865 2061  aram user: The a
-00001f40: 6464 7265 7373 206f 6620 7468 6520 7573  ddress of the us
-00001f50: 6572 2e0a 2020 2020 2020 2020 3a74 7970  er..        :typ
-00001f60: 6520 7573 6572 3a20 4368 6563 6b73 756d  e user: Checksum
-00001f70: 4164 6472 6573 730a 2020 2020 2020 2020  Address.        
-00001f80: 3a70 6172 616d 2074 6172 6765 745f 6261  :param target_ba
-00001f90: 7468 5f74 6f6b 656e 733a 2054 6865 206c  th_tokens: The l
-00001fa0: 6973 7420 6f66 2074 6172 6765 7420 6261  ist of target ba
-00001fb0: 7468 2074 6f6b 656e 7320 746f 2063 6c61  th tokens to cla
-00001fc0: 696d 2062 6f6e 7573 2066 726f 6d2e 0a20  im bonus from.. 
-00001fd0: 2020 2020 2020 203a 7479 7065 2074 6172         :type tar
-00001fe0: 6765 745f 6261 7468 5f74 6f6b 656e 733a  get_bath_tokens:
-00001ff0: 204c 6973 745b 4368 6563 6b73 756d 4164   List[ChecksumAd
-00002000: 6472 6573 735d 0a20 2020 2020 2020 203a  dress].        :
-00002010: 7061 7261 6d20 746f 6b65 6e3a 2054 6865  param token: The
-00002020: 2061 6464 7265 7373 206f 6620 7468 6520   address of the 
-00002030: 746f 6b65 6e20 666f 7220 7768 6963 6820  token for which 
-00002040: 7468 6520 626f 6e75 7320 6973 2063 6c61  the bonus is cla
-00002050: 696d 6564 2e0a 2020 2020 2020 2020 3a74  imed..        :t
-00002060: 7970 6520 746f 6b65 6e3a 2043 6865 636b  ype token: Check
-00002070: 7375 6d41 6464 7265 7373 0a20 2020 2020  sumAddress.     
-00002080: 2020 203a 7265 7475 726e 3a20 5468 6520     :return: The 
-00002090: 746f 7461 6c20 616d 6f75 6e74 2065 6172  total amount ear
-000020a0: 6e65 6420 6163 726f 7373 2061 6c6c 2070  ned across all p
-000020b0: 6f6f 6c73 2e0a 2020 2020 2020 2020 3a72  ools..        :r
-000020c0: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
-000020d0: 2020 2904 720c 0000 0072 2400 0000 5a1c    ).r....r$...Z.
-000020e0: 6368 6563 6b43 6c61 696d 416c 6c55 7365  checkClaimAllUse
-000020f0: 7242 6f6e 7573 546f 6b65 6e73 7225 0000  rBonusTokensr%..
-00002100: 0029 0472 1200 0000 723b 0000 0072 3c00  .).r....r;...r<.
-00002110: 0000 723d 0000 0072 1500 0000 7215 0000  ..r=...r....r...
-00002120: 0072 1600 0000 da21 6368 6563 6b5f 636c  .r.....!check_cl
-00002130: 6169 6d5f 616c 6c5f 7573 6572 5f62 6f6e  aim_all_user_bon
-00002140: 7573 5f74 6f6b 656e 73d2 0000 0072 2b00  us_tokens....r+.
-00002150: 0000 7a2f 5275 6269 636f 6e52 6f75 7465  ..z/RubiconRoute
-00002160: 722e 6368 6563 6b5f 636c 6169 6d5f 616c  r.check_claim_al
-00002170: 6c5f 7573 6572 5f62 6f6e 7573 5f74 6f6b  l_user_bonus_tok
-00002180: 656e 73e9 3057 0500 da0c 6275 795f 616d  ens.0W....buy_am
-00002190: 7473 5f6d 696e da02 746f da05 6e6f 6e63  ts_min..to..nonc
-000021a0: 65da 0367 6173 da0f 6d61 785f 6665 655f  e..gas..max_fee_
-000021b0: 7065 725f 6761 73da 186d 6178 5f70 7269  per_gas..max_pri
-000021c0: 6f72 6974 795f 6665 655f 7065 725f 6761  ority_fee_per_ga
-000021d0: 7363 0900 0000 0000 0000 0000 0000 0a00  sc..............
-000021e0: 0000 0700 0000 4300 0000 f328 0000 007c  ......C....(...|
-000021f0: 006a 006a 01a0 027c 017c 027c 037c 04a1  .j.j...|.|.|.|..
-00002200: 047d 097c 006a 037c 097c 067c 057c 077c  .}.|.j.|.|.|.|.|
-00002210: 0864 018d 0553 0029 0261 f105 0000 5065  .d...S.).a....Pe
-00002220: 7266 6f72 6d20 6120 6d75 6c74 6970 6c65  rform a multiple
-00002230: 2073 7761 7073 2066 6f72 2074 6865 2073   swaps for the s
-00002240: 7065 6369 6669 6564 2070 6179 6d65 6e74  pecified payment
-00002250: 2061 6d6f 756e 7473 2075 7369 6e67 2074   amounts using t
-00002260: 6865 2073 7065 6369 6669 6564 2072 6f75  he specified rou
-00002270: 7465 732e 2052 6576 6572 7473 2077 6974  tes. Reverts wit
-00002280: 6820 616e 0a20 2020 2020 2020 2065 7863  h an.        exc
-00002290: 6570 7469 6f6e 2069 6620 616e 7920 6f66  eption if any of
-000022a0: 2074 6865 2073 7761 7073 2063 616e 6e6f   the swaps canno
-000022b0: 7420 6163 6869 6576 6520 7468 6520 6275  t achieve the bu
-000022c0: 795f 616d 745f 6d69 6e20 616c 6f6e 6720  y_amt_min along 
-000022d0: 7468 6520 7370 6563 6966 6965 6420 726f  the specified ro
-000022e0: 7574 652e 0a0a 2020 2020 2020 2020 3a70  ute...        :p
-000022f0: 6172 616d 2072 6f75 7465 733a 2054 6865  aram routes: The
-00002300: 206c 6973 7420 6f66 2072 6f75 7465 732c   list of routes,
-00002310: 2077 6865 7265 2065 6163 6820 726f 7574   where each rout
-00002320: 6520 6973 2061 206c 6973 7420 6f66 2061  e is a list of a
-00002330: 6464 7265 7373 6573 2072 6570 7265 7365  ddresses represe
-00002340: 6e74 696e 6720 7468 6520 7377 6170 2070  nting the swap p
-00002350: 6174 682e 0a20 2020 2020 2020 203a 7479  ath..        :ty
-00002360: 7065 2072 6f75 7465 733a 204c 6973 745b  pe routes: List[
-00002370: 4c69 7374 5b43 6865 636b 7375 6d41 6464  List[ChecksumAdd
-00002380: 7265 7373 5d5d 0a20 2020 2020 2020 203a  ress]].        :
-00002390: 7061 7261 6d20 7061 795f 616d 7473 3a20  param pay_amts: 
-000023a0: 5468 6520 6c69 7374 206f 6620 7061 796d  The list of paym
-000023b0: 656e 7420 616d 6f75 6e74 7320 666f 7220  ent amounts for 
-000023c0: 6561 6368 2073 7761 702e 0a20 2020 2020  each swap..     
-000023d0: 2020 203a 7479 7065 2070 6179 5f61 6d74     :type pay_amt
-000023e0: 733a 204c 6973 745b 696e 745d 0a20 2020  s: List[int].   
-000023f0: 2020 2020 203a 7061 7261 6d20 6275 795f       :param buy_
-00002400: 616d 7473 5f6d 696e 3a20 5468 6520 6c69  amts_min: The li
-00002410: 7374 206f 6620 6d69 6e69 6d75 6d20 6275  st of minimum bu
-00002420: 7920 616d 6f75 6e74 7320 666f 7220 6561  y amounts for ea
-00002430: 6368 2073 7761 702e 0a20 2020 2020 2020  ch swap..       
-00002440: 203a 7479 7065 2062 7579 5f61 6d74 735f   :type buy_amts_
-00002450: 6d69 6e3a 204c 6973 745b 696e 745d 0a20  min: List[int]. 
-00002460: 2020 2020 2020 203a 7061 7261 6d20 746f         :param to
-00002470: 3a20 5468 6520 6164 6472 6573 7320 6f66  : The address of
-00002480: 2074 6865 2072 6563 6970 6965 6e74 2e0a   the recipient..
-00002490: 2020 2020 2020 2020 3a74 7970 6520 746f          :type to
-000024a0: 3a20 4368 6563 6b73 756d 4164 6472 6573  : ChecksumAddres
-000024b0: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
-000024c0: 206e 6f6e 6365 3a20 4e6f 6e63 6520 6f66   nonce: Nonce of
-000024d0: 2074 6865 2074 7261 6e73 6163 7469 6f6e   the transaction
-000024e0: 2e20 4465 6661 756c 7473 2074 6f20 6361  . Defaults to ca
-000024f0: 6c6c 696e 6720 7468 6520 6368 6169 6e20  lling the chain 
-00002500: 7374 6174 6520 746f 2067 6574 2074 6865  state to get the
-00002510: 206e 6f6e 6365 2e0a 2020 2020 2020 2020   nonce..        
-00002520: 2020 2020 286f 7074 696f 6e61 6c2c 2064      (optional, d
-00002530: 6566 6175 6c74 2069 7320 4e6f 6e65 292e  efault is None).
-00002540: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
-00002550: 6f6e 6365 3a20 4f70 7469 6f6e 616c 5b69  once: Optional[i
-00002560: 6e74 5d0a 2020 2020 2020 2020 3a70 6172  nt].        :par
-00002570: 616d 2067 6173 3a20 4761 7320 6c69 6d69  am gas: Gas limi
-00002580: 7420 6f66 2074 6865 2074 7261 6e73 6163  t of the transac
-00002590: 7469 6f6e 2e20 4465 6661 756c 7473 2074  tion. Defaults t
-000025a0: 6f20 6120 7665 7279 2068 6967 6820 6573  o a very high es
-000025b0: 7469 6d61 7465 206d 6164 6520 7768 656e  timate made when
-000025c0: 2077 7269 7469 6e67 2074 6865 2063 6c61   writing the cla
-000025d0: 7373 2e0a 2020 2020 2020 2020 3a74 7970  ss..        :typ
-000025e0: 6520 6761 733a 2069 6e74 0a20 2020 2020  e gas: int.     
-000025f0: 2020 203a 7061 7261 6d20 6d61 785f 6665     :param max_fe
-00002600: 655f 7065 725f 6761 733a 204d 6178 2066  e_per_gas: Max f
-00002610: 6565 2074 6861 7420 6361 6e20 6265 2070  ee that can be p
-00002620: 6169 6420 666f 7220 6761 732e 2044 6566  aid for gas. Def
-00002630: 6175 6c74 7320 746f 206d 6178 5f70 7269  aults to max_pri
-00002640: 6f72 6974 795f 6665 6520 2866 726f 6d20  ority_fee (from 
-00002650: 6368 6169 6e29 0a20 2020 2020 2020 2020  chain).         
-00002660: 2020 202b 2028 3220 2a20 6261 7365 2066     + (2 * base f
-00002670: 6565 2070 6572 2067 6173 206f 6620 6c61  ee per gas of la
-00002680: 7465 7374 2062 6c6f 636b 2920 286f 7074  test block) (opt
-00002690: 696f 6e61 6c2c 2064 6566 6175 6c74 2069  ional, default i
-000026a0: 7320 4e6f 6e65 292e 0a20 2020 2020 2020  s None)..       
-000026b0: 203a 7479 7065 206d 6178 5f66 6565 5f70   :type max_fee_p
-000026c0: 6572 5f67 6173 3a20 4f70 7469 6f6e 616c  er_gas: Optional
-000026d0: 5b69 6e74 5d0a 2020 2020 2020 2020 3a70  [int].        :p
-000026e0: 6172 616d 206d 6178 5f70 7269 6f72 6974  aram max_priorit
-000026f0: 795f 6665 655f 7065 725f 6761 733a 204d  y_fee_per_gas: M
-00002700: 6178 2070 7269 6f72 6974 7920 6665 6520  ax priority fee 
-00002710: 7468 6174 2063 616e 2062 6520 7061 6964  that can be paid
-00002720: 2066 6f72 2067 6173 2e20 4465 6661 756c   for gas. Defaul
-00002730: 7473 2074 6f20 6361 6c6c 696e 6720 7468  ts to calling th
-00002740: 6520 6368 6169 6e20 746f 0a20 2020 2020  e chain to.     
-00002750: 2020 2020 2020 2065 7374 696d 6174 6520         estimate 
-00002760: 7468 6520 6d61 785f 7072 696f 7269 7479  the max_priority
-00002770: 5f66 6565 5f70 6572 5f67 6173 2028 6f70  _fee_per_gas (op
-00002780: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00002790: 6973 204e 6f6e 6529 2e0a 2020 2020 2020  is None)..      
-000027a0: 2020 3a74 7970 6520 6d61 785f 7072 696f    :type max_prio
-000027b0: 7269 7479 5f66 6565 5f70 6572 5f67 6173  rity_fee_per_gas
-000027c0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0a  : Optional[int].
-000027d0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-000027e0: 2054 7261 6e73 6163 7469 6f6e 2068 6173   Transaction has
-000027f0: 682e 0a20 2020 2020 2020 203a 7274 7970  h..        :rtyp
-00002800: 653a 2073 7472 0a20 2020 2020 2020 20a9  e: str.        .
-00002810: 05da 1e69 6e73 7461 6e74 6961 7465 645f  ...instantiated_
-00002820: 636f 6e74 7261 6374 5f66 756e 6374 696f  contract_functio
-00002830: 6e72 4300 0000 7242 0000 0072 4400 0000  nrC...rB...rD...
-00002840: 7245 0000 0029 0472 0c00 0000 7224 0000  rE...).r....r$..
-00002850: 00da 096d 756c 7469 7377 6170 da1c 5f64  ...multiswap.._d
-00002860: 6566 6175 6c74 5f74 7261 6e73 6163 7469  efault_transacti
-00002870: 6f6e 5f68 616e 646c 6572 290a 7212 0000  on_handler).r...
-00002880: 0072 3900 0000 7237 0000 0072 4000 0000  .r9...r7...r@...
-00002890: 7241 0000 0072 4200 0000 7243 0000 0072  rA...rB...rC...r
-000028a0: 4400 0000 7245 0000 0072 4900 0000 7215  D...rE...rI...r.
-000028b0: 0000 0072 1500 0000 7216 0000 0072 4900  ...r....r....rI.
-000028c0: 0000 eb00 0000 f310 0000 0014 2504 0202  ............%...
-000028d0: 0102 0102 0102 0102 0106 fb7a 1752 7562  ...........z.Rub
-000028e0: 6963 6f6e 526f 7574 6572 2e6d 756c 7469  iconRouter.multi
-000028f0: 7377 6170 6309 0000 0000 0000 0000 0000  swapc...........
-00002900: 000a 0000 0007 0000 0043 0000 0072 4600  .........C...rF.
-00002910: 0000 2902 618f 0500 0050 6572 666f 726d  ..).a....Perform
-00002920: 2061 2073 7761 7020 6f70 6572 6174 696f   a swap operatio
-00002930: 6e20 7769 7468 2074 6865 2073 7065 6369  n with the speci
-00002940: 6669 6564 2070 6179 6d65 6e74 2061 6d6f  fied payment amo
-00002950: 756e 7420 7573 696e 6720 7468 6520 7370  unt using the sp
-00002960: 6563 6966 6965 6420 726f 7574 6520 616e  ecified route an
-00002970: 6420 7061 7969 6e67 206f 7574 2074 6f20  d paying out to 
-00002980: 7468 650a 2020 2020 2020 2020 7265 6369  the.        reci
-00002990: 7069 656e 742e 2052 6576 6572 7473 2069  pient. Reverts i
-000029a0: 6620 7468 6520 7377 6170 2064 6f65 7320  f the swap does 
-000029b0: 6e6f 7420 7265 7375 6c74 2069 6e20 7468  not result in th
-000029c0: 6520 6275 795f 6d69 6e5f 616d 6f75 6e74  e buy_min_amount
-000029d0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000029e0: 6d20 7061 795f 616d 743a 2054 6865 2070  m pay_amt: The p
-000029f0: 6179 6d65 6e74 2061 6d6f 756e 742e 0a20  ayment amount.. 
-00002a00: 2020 2020 2020 203a 7479 7065 2070 6179         :type pay
-00002a10: 5f61 6d74 3a20 696e 740a 2020 2020 2020  _amt: int.      
-00002a20: 2020 3a70 6172 616d 2062 7579 5f61 6d74    :param buy_amt
-00002a30: 5f6d 696e 3a20 5468 6520 6d69 6e69 6d75  _min: The minimu
-00002a40: 6d20 6275 7920 616d 6f75 6e74 2e0a 2020  m buy amount..  
-00002a50: 2020 2020 2020 3a74 7970 6520 6275 795f        :type buy_
-00002a60: 616d 745f 6d69 6e3a 2069 6e74 0a20 2020  amt_min: int.   
-00002a70: 2020 2020 203a 7061 7261 6d20 726f 7574       :param rout
-00002a80: 653a 2054 6865 2072 6f75 7465 2c20 7265  e: The route, re
-00002a90: 7072 6573 656e 7465 6420 6173 2061 206c  presented as a l
-00002aa0: 6973 7420 6f66 2061 6464 7265 7373 6573  ist of addresses
-00002ab0: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
-00002ac0: 6520 7377 6170 2070 6174 682e 0a20 2020  e swap path..   
-00002ad0: 2020 2020 203a 7479 7065 2072 6f75 7465       :type route
-00002ae0: 3a20 4c69 7374 5b43 6865 636b 7375 6d41  : List[ChecksumA
-00002af0: 6464 7265 7373 5d0a 2020 2020 2020 2020  ddress].        
-00002b00: 3a70 6172 616d 2074 6f3a 2054 6865 2061  :param to: The a
-00002b10: 6464 7265 7373 206f 6620 7468 6520 7265  ddress of the re
-00002b20: 6369 7069 656e 742e 0a20 2020 2020 2020  cipient..       
-00002b30: 203a 7479 7065 2074 6f3a 2043 6865 636b   :type to: Check
-00002b40: 7375 6d41 6464 7265 7373 0a20 2020 2020  sumAddress.     
-00002b50: 2020 203a 7061 7261 6d20 6e6f 6e63 653a     :param nonce:
-00002b60: 204e 6f6e 6365 206f 6620 7468 6520 7472   Nonce of the tr
-00002b70: 616e 7361 6374 696f 6e2e 2044 6566 6175  ansaction. Defau
-00002b80: 6c74 7320 746f 2063 616c 6c69 6e67 2074  lts to calling t
-00002b90: 6865 2063 6861 696e 2073 7461 7465 2074  he chain state t
-00002ba0: 6f20 6765 7420 7468 6520 6e6f 6e63 652e  o get the nonce.
-00002bb0: 0a20 2020 2020 2020 2020 2020 2028 6f70  .            (op
-00002bc0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00002bd0: 6973 204e 6f6e 6529 2e0a 2020 2020 2020  is None)..      
-00002be0: 2020 3a74 7970 6520 6e6f 6e63 653a 204f    :type nonce: O
-00002bf0: 7074 696f 6e61 6c5b 696e 745d 0a20 2020  ptional[int].   
-00002c00: 2020 2020 203a 7061 7261 6d20 6761 733a       :param gas:
-00002c10: 2047 6173 206c 696d 6974 206f 6620 7468   Gas limit of th
-00002c20: 6520 7472 616e 7361 6374 696f 6e2e 2044  e transaction. D
-00002c30: 6566 6175 6c74 7320 746f 2061 2076 6572  efaults to a ver
-00002c40: 7920 6869 6768 2065 7374 696d 6174 6520  y high estimate 
-00002c50: 6d61 6465 2077 6865 6e20 7772 6974 696e  made when writin
-00002c60: 6720 7468 6520 636c 6173 732e 0a20 2020  g the class..   
-00002c70: 2020 2020 203a 7479 7065 2067 6173 3a20       :type gas: 
-00002c80: 696e 740a 2020 2020 2020 2020 3a70 6172  int.        :par
-00002c90: 616d 206d 6178 5f66 6565 5f70 6572 5f67  am max_fee_per_g
-00002ca0: 6173 3a20 4d61 7820 6665 6520 7468 6174  as: Max fee that
-00002cb0: 2063 616e 2062 6520 7061 6964 2066 6f72   can be paid for
-00002cc0: 2067 6173 2e20 4465 6661 756c 7473 2074   gas. Defaults t
-00002cd0: 6f20 6d61 785f 7072 696f 7269 7479 5f66  o max_priority_f
-00002ce0: 6565 2028 6672 6f6d 2063 6861 696e 290a  ee (from chain).
-00002cf0: 2020 2020 2020 2020 2020 2020 2b20 2832              + (2
-00002d00: 202a 2062 6173 6520 6665 6520 7065 7220   * base fee per 
-00002d10: 6761 7320 6f66 206c 6174 6573 7420 626c  gas of latest bl
-00002d20: 6f63 6b29 2028 6f70 7469 6f6e 616c 2c20  ock) (optional, 
-00002d30: 6465 6661 756c 7420 6973 204e 6f6e 6529  default is None)
-00002d40: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00002d50: 6d61 785f 6665 655f 7065 725f 6761 733a  max_fee_per_gas:
-00002d60: 204f 7074 696f 6e61 6c5b 696e 745d 0a20   Optional[int]. 
-00002d70: 2020 2020 2020 203a 7061 7261 6d20 6d61         :param ma
-00002d80: 785f 7072 696f 7269 7479 5f66 6565 5f70  x_priority_fee_p
-00002d90: 6572 5f67 6173 3a20 4d61 7820 7072 696f  er_gas: Max prio
-00002da0: 7269 7479 2066 6565 2074 6861 7420 6361  rity fee that ca
-00002db0: 6e20 6265 2070 6169 6420 666f 7220 6761  n be paid for ga
-00002dc0: 732e 2044 6566 6175 6c74 7320 746f 2063  s. Defaults to c
-00002dd0: 616c 6c69 6e67 2074 6865 2063 6861 696e  alling the chain
-00002de0: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-00002df0: 6573 7469 6d61 7465 2074 6865 206d 6178  estimate the max
-00002e00: 5f70 7269 6f72 6974 795f 6665 655f 7065  _priority_fee_pe
-00002e10: 725f 6761 7320 286f 7074 696f 6e61 6c2c  r_gas (optional,
-00002e20: 2064 6566 6175 6c74 2069 7320 4e6f 6e65   default is None
-00002e30: 292e 0a20 2020 2020 2020 203a 7479 7065  )..        :type
-00002e40: 206d 6178 5f70 7269 6f72 6974 795f 6665   max_priority_fe
-00002e50: 655f 7065 725f 6761 733a 204f 7074 696f  e_per_gas: Optio
-00002e60: 6e61 6c5b 696e 745d 0a20 2020 2020 2020  nal[int].       
-00002e70: 203a 7265 7475 726e 3a20 5472 616e 7361   :return: Transa
-00002e80: 6374 696f 6e20 6861 7368 2e0a 2020 2020  ction hash..    
-00002e90: 2020 2020 3a72 7479 7065 3a20 7374 720a      :rtype: str.
-00002ea0: 2020 2020 2020 2020 7247 0000 0029 0472          rG...).r
-00002eb0: 0c00 0000 7224 0000 00da 0473 7761 7072  ....r$.....swapr
-00002ec0: 4a00 0000 290a 7212 0000 0072 3300 0000  J...).r....r3...
-00002ed0: 7234 0000 0072 3500 0000 7241 0000 0072  r4...r5...rA...r
-00002ee0: 4200 0000 7243 0000 0072 4400 0000 7245  B...rC...rD...rE
-00002ef0: 0000 0072 4c00 0000 7215 0000 0072 1500  ...rL...r....r..
-00002f00: 0000 7216 0000 0072 4c00 0000 1b01 0000  ..r....rL.......
-00002f10: 724b 0000 007a 1252 7562 6963 6f6e 526f  rK...z.RubiconRo
-00002f20: 7574 6572 2e73 7761 7029 024e 4e29 044e  uter.swap).NN).N
-00002f30: 723f 0000 004e 4e29 1bda 085f 5f6e 616d  r?...NN)...__nam
-00002f40: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00002f50: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00002f60: 5f64 6f63 5f5f 7206 0000 0072 0700 0000  _doc__r....r....
-00002f70: 7202 0000 0072 0500 0000 da03 7374 7272  r....r......strr
-00002f80: 1100 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
-00002f90: 6472 0900 0000 721f 0000 0072 0400 0000  dr....r....r....
-00002fa0: 7203 0000 00da 0369 6e74 7226 0000 0072  r......intr&...r
-00002fb0: 2a00 0000 722e 0000 0072 3100 0000 7232  *...r....r1...r2
-00002fc0: 0000 0072 3600 0000 723a 0000 0072 3e00  ...r6...r:...r>.
-00002fd0: 0000 7249 0000 0072 4c00 0000 da0d 5f5f  ..rI...rL.....__
-00002fe0: 636c 6173 7363 656c 6c5f 5f72 1500 0000  classcell__r....
-00002ff0: 7215 0000 0072 1300 0000 7216 0000 0072  r....r....r....r
-00003000: 0a00 0000 0b00 0000 73fa 0000 0008 0004  ........s.......
-00003010: 0102 1102 0104 fb02 0202 fe02 0302 fd06  ................
-00003020: 0402 fc06 0502 fb02 060e fa02 0f02 0402  ................
-00003030: 0104 fc02 0202 fe06 0302 fd06 0402 fc02  ................
-00003040: 050c fb02 1f02 0202 fe06 0302 fd02 0402  ................
-00003050: fc0a 050a fb02 1602 0202 fe02 0302 fd02  ................
-00003060: 0402 fc02 050a fb02 1502 0202 fe02 0302  ................
-00003070: fd1a 040a fc1e 1402 0f02 0202 fe02 0302  ................
-00003080: fd10 040a fc1e 1302 1206 0202 fe06 0302  ................
-00003090: fd0a 0402 fc02 050a fb02 1702 0202 fe06  ................
-000030a0: 0302 fd02 0402 fc02 050a fb02 1f02 0102  ................
-000030b0: 0102 0104 f70a 0202 fe06 0302 fd06 0402  ................
-000030c0: fc02 0502 fb06 0602 fa02 0702 f906 0802  ................
-000030d0: f806 0902 f702 0a0a f602 3602 0102 0102  ..........6.....
-000030e0: 0104 f702 0202 fe02 0302 fd06 0402 fc02  ................
-000030f0: 0502 fb06 0602 fa02 0702 f906 0802 f806  ................
-00003100: 0902 f702 0a12 f672 0a00 0000 4e29 0fda  .......r....N)..
-00003110: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-00003120: 0072 0400 0000 da0a 6574 685f 7479 7069  .r......eth_typi
-00003130: 6e67 7205 0000 00da 0477 6562 3372 0600  ngr......web3r..
-00003140: 0000 da0d 7765 6233 2e63 6f6e 7472 6163  ....web3.contrac
-00003150: 7472 0700 0000 5a1c 7275 6269 2e63 6f6e  tr....Z.rubi.con
-00003160: 7472 6163 7473 2e62 6173 655f 636f 6e74  tracts.base_cont
-00003170: 7261 6374 7208 0000 005a 0c72 7562 692e  ractr....Z.rubi.
-00003180: 6e65 7477 6f72 6b72 0900 0000 720a 0000  networkr....r...
-00003190: 0072 1500 0000 7215 0000 0072 1500 0000  .r....r....r....
-000031a0: 7216 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000031b0: 0000 0073 0e00 0000 1400 0c02 0c01 0c01  ...s............
-000031c0: 0c02 0c01 1403                           ......
+00000000: 696d 706f 7274 206c 6f67 6769 6e67 2061  import logging a
+00000010: 7320 6c6f 670a 6672 6f6d 2074 6872 6561  s log.from threa
+00000020: 6469 6e67 2069 6d70 6f72 7420 5468 7265  ding import Thre
+00000030: 6164 0a66 726f 6d20 7469 6d65 2069 6d70  ad.from time imp
+00000040: 6f72 7420 736c 6565 700a 6672 6f6d 2074  ort sleep.from t
+00000050: 7970 696e 6720 696d 706f 7274 204f 7074  yping import Opt
+00000060: 696f 6e61 6c2c 2043 616c 6c61 626c 652c  ional, Callable,
+00000070: 2054 7970 652c 2044 6963 742c 2041 6e79   Type, Dict, Any
+00000080: 0a0a 6672 6f6d 2065 7468 5f61 6363 6f75  ..from eth_accou
+00000090: 6e74 2e64 6174 6173 7472 7563 7475 7265  nt.datastructure
+000000a0: 7320 696d 706f 7274 2053 6967 6e65 6454  s import SignedT
+000000b0: 7261 6e73 6163 7469 6f6e 0a66 726f 6d20  ransaction.from 
+000000c0: 6574 685f 7479 7069 6e67 2069 6d70 6f72  eth_typing impor
+000000d0: 7420 4368 6563 6b73 756d 4164 6472 6573  t ChecksumAddres
+000000e0: 730a 6672 6f6d 2077 6562 3320 696d 706f  s.from web3 impo
+000000f0: 7274 2057 6562 330a 6672 6f6d 2077 6562  rt Web3.from web
+00000100: 332e 5f75 7469 6c73 2e66 696c 7465 7273  3._utils.filters
+00000110: 2069 6d70 6f72 7420 4c6f 6746 696c 7465   import LogFilte
+00000120: 7220 2023 206e 6f71 610a 6672 6f6d 2077  r  # noqa.from w
+00000130: 6562 332e 636f 6e74 7261 6374 2069 6d70  eb3.contract imp
+00000140: 6f72 7420 436f 6e74 7261 6374 0a66 726f  ort Contract.fro
+00000150: 6d20 7765 6233 2e63 6f6e 7472 6163 742e  m web3.contract.
+00000160: 636f 6e74 7261 6374 2069 6d70 6f72 7420  contract import 
+00000170: 436f 6e74 7261 6374 4675 6e63 7469 6f6e  ContractFunction
+00000180: 0a66 726f 6d20 7765 6233 2e74 7970 6573  .from web3.types
+00000190: 2069 6d70 6f72 7420 4142 492c 204e 6f6e   import ABI, Non
+000001a0: 6365 0a0a 6672 6f6d 2072 7562 692e 636f  ce..from rubi.co
+000001b0: 6e74 7261 6374 732e 7479 7065 7320 696d  ntracts.types im
+000001c0: 706f 7274 2042 6173 6545 7665 6e74 2c20  port BaseEvent, 
+000001d0: 5472 616e 7361 6374 696f 6e52 6563 6569  TransactionRecei
+000001e0: 7074 0a0a 0a63 6c61 7373 2042 6173 6543  pt...class BaseC
+000001f0: 6f6e 7472 6163 743a 0a20 2020 2022 2222  ontract:.    """
+00000200: 4261 7365 2063 6c61 7373 2072 6570 7265  Base class repre
+00000210: 7365 6e74 6174 696f 6e20 6f66 2061 2063  sentation of a c
+00000220: 6f6e 7472 6163 7420 7768 6963 6820 6465  ontract which de
+00000230: 6669 6e65 7320 7468 6520 7374 7275 6374  fines the struct
+00000240: 7572 6520 6f66 2061 2063 6f6e 7472 6163  ure of a contrac
+00000250: 7420 616e 6420 7072 6f76 6964 6573 2073  t and provides s
+00000260: 6576 6572 616c 2068 656c 7066 756c 0a20  everal helpful. 
+00000270: 2020 206d 6574 686f 6473 2074 6861 7420     methods that 
+00000280: 6361 6e20 6265 2075 7365 6420 6279 2073  can be used by s
+00000290: 7562 636c 6173 7320 636f 6e74 7261 6374  ubclass contract
+000002a0: 7320 7468 6174 2065 7874 656e 6420 7468  s that extend th
+000002b0: 6973 2063 6f6e 7472 6163 742e 0a0a 2020  is contract...  
+000002c0: 2020 3a70 6172 616d 2077 333a 2057 6562    :param w3: Web
+000002d0: 3320 696e 7374 616e 6365 0a20 2020 203a  3 instance.    :
+000002e0: 7479 7065 2077 333a 2057 6562 330a 2020  type w3: Web3.  
+000002f0: 2020 3a70 6172 616d 2063 6f6e 7472 6163    :param contrac
+00000300: 743a 2043 6f6e 7472 6163 7420 696e 7374  t: Contract inst
+00000310: 616e 6365 0a20 2020 203a 7479 7065 2063  ance.    :type c
+00000320: 6f6e 7472 6163 743a 2043 6f6e 7472 6163  ontract: Contrac
+00000330: 740a 2020 2020 3a70 6172 616d 2077 616c  t.    :param wal
+00000340: 6c65 743a 2061 2077 616c 6c65 7420 6164  let: a wallet ad
+00000350: 6472 6573 7320 6f66 2074 6865 2073 6967  dress of the sig
+00000360: 6e65 7220 286f 7074 696f 6e61 6c2c 2064  ner (optional, d
+00000370: 6566 6175 6c74 2069 7320 4e6f 6e65 290a  efault is None).
+00000380: 2020 2020 3a74 7970 6520 7761 6c6c 6574      :type wallet
+00000390: 3a20 4f70 7469 6f6e 616c 5b43 6865 636b  : Optional[Check
+000003a0: 7375 6d41 6464 7265 7373 5d0a 2020 2020  sumAddress].    
+000003b0: 3a70 6172 616d 206b 6579 3a20 7468 6520  :param key: the 
+000003c0: 7072 6976 6174 6520 6b65 7920 6f66 2074  private key of t
+000003d0: 6865 2073 6967 6e65 7220 286f 7074 696f  he signer (optio
+000003e0: 6e61 6c2c 2064 6566 6175 6c74 2069 7320  nal, default is 
+000003f0: 4e6f 6e65 290a 2020 2020 3a74 7970 6520  None).    :type 
+00000400: 6b65 793a 204f 7074 696f 6e61 6c5b 7374  key: Optional[st
+00000410: 725d 0a20 2020 2022 2222 0a0a 2020 2020  r].    """..    
+00000420: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00000430: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00000440: 2020 2020 7733 3a20 5765 6233 2c0a 2020      w3: Web3,.  
+00000450: 2020 2020 2020 636f 6e74 7261 6374 3a20        contract: 
+00000460: 436f 6e74 7261 6374 2c0a 2020 2020 2020  Contract,.      
+00000470: 2020 7761 6c6c 6574 3a20 4f70 7469 6f6e    wallet: Option
+00000480: 616c 5b43 6865 636b 7375 6d41 6464 7265  al[ChecksumAddre
+00000490: 7373 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ss] = None,.    
+000004a0: 2020 2020 6b65 793a 204f 7074 696f 6e61      key: Optiona
+000004b0: 6c5b 7374 725d 203d 204e 6f6e 650a 2020  l[str] = None.  
+000004c0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+000004d0: 636f 6e73 7472 7563 746f 7220 6d65 7468  constructor meth
+000004e0: 6f64 2222 220a 2020 2020 2020 2020 6966  od""".        if
+000004f0: 2028 7761 6c6c 6574 2069 7320 4e6f 6e65   (wallet is None
+00000500: 2920 213d 2028 6b65 7920 6973 204e 6f6e  ) != (key is Non
+00000510: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00000520: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00000530: 2262 6f74 6820 6120 7761 6c6c 6574 2061  "both a wallet a
+00000540: 6e64 2061 206b 6579 2061 7265 2072 6571  nd a key are req
+00000550: 7569 7265 6420 746f 2073 6967 6e20 7472  uired to sign tr
+00000560: 616e 7361 6374 696f 6e73 2e20 7072 6f76  ansactions. prov
+00000570: 6964 6520 626f 7468 206f 7220 6f6d 6974  ide both or omit
+00000580: 2062 6f74 6822 290a 0a20 2020 2020 2020   both")..       
+00000590: 2073 656c 662e 636f 6e74 7261 6374 203d   self.contract =
+000005a0: 2063 6f6e 7472 6163 740a 2020 2020 2020   contract.      
+000005b0: 2020 7365 6c66 2e61 6464 7265 7373 203d    self.address =
+000005c0: 2063 6f6e 7472 6163 742e 6164 6472 6573   contract.addres
+000005d0: 730a 2020 2020 2020 2020 7365 6c66 2e77  s.        self.w
+000005e0: 3320 3d20 7733 0a20 2020 2020 2020 2073  3 = w3.        s
+000005f0: 656c 662e 6368 6169 6e5f 6964 203d 2073  elf.chain_id = s
+00000600: 656c 662e 7733 2e65 7468 2e63 6861 696e  elf.w3.eth.chain
+00000610: 5f69 640a 0a20 2020 2020 2020 2023 2053  _id..        # S
+00000620: 6967 6e69 6e67 2070 6572 6d69 7373 696f  igning permissio
+00000630: 6e73 0a20 2020 2020 2020 2073 656c 662e  ns.        self.
+00000640: 7369 676e 696e 675f 7065 726d 6973 7369  signing_permissi
+00000650: 6f6e 7320 3d20 2877 616c 6c65 7420 6973  ons = (wallet is
+00000660: 206e 6f74 204e 6f6e 6520 616e 6420 6b65   not None and ke
+00000670: 7920 6973 206e 6f74 204e 6f6e 6529 0a0a  y is not None)..
+00000680: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00000690: 7369 676e 696e 675f 7065 726d 6973 7369  signing_permissi
+000006a0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+000006b0: 206c 6f67 2e69 6e66 6f28 6622 696e 7374   log.info(f"inst
+000006c0: 616e 7469 6174 6564 207b 7365 6c66 2e5f  antiated {self._
+000006d0: 5f63 6c61 7373 5f5f 7d20 7769 7468 2073  _class__} with s
+000006e0: 6967 6e69 6e67 2072 6967 6874 7322 290a  igning rights").
+000006f0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+00000700: 6f72 6365 2074 7970 696e 6720 6173 206d  orce typing as m
+00000710: 7920 6564 6974 6f72 7320 696e 7370 6563  y editors inspec
+00000720: 7469 6f6e 2069 7320 7468 726f 7769 6e67  tion is throwing
+00000730: 2061 2074 616e 7472 756d 0a20 2020 2020   a tantrum.     
+00000740: 2020 2020 2020 2073 656c 662e 7761 6c6c         self.wall
+00000750: 6574 203d 2077 616c 6c65 7420 2023 2074  et = wallet  # t
+00000760: 7970 653a 2043 6865 636b 7375 6d41 6464  ype: ChecksumAdd
+00000770: 7265 7373 0a20 2020 2020 2020 2020 2020  ress.           
+00000780: 2073 656c 662e 6b65 7920 3d20 6b65 7920   self.key = key 
+00000790: 2023 2074 7970 653a 2073 7472 0a0a 2020   # type: str..  
+000007a0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+000007b0: 2020 2064 6566 2066 726f 6d5f 6164 6472     def from_addr
+000007c0: 6573 735f 616e 645f 6162 6928 0a20 2020  ess_and_abi(.   
+000007d0: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
+000007e0: 2020 7733 3a20 5765 6233 2c0a 2020 2020    w3: Web3,.    
+000007f0: 2020 2020 6164 6472 6573 733a 2043 6865      address: Che
+00000800: 636b 7375 6d41 6464 7265 7373 2c0a 2020  cksumAddress,.  
+00000810: 2020 2020 2020 636f 6e74 7261 6374 5f61        contract_a
+00000820: 6269 3a20 4142 492c 0a20 2020 2020 2020  bi: ABI,.       
+00000830: 2077 616c 6c65 743a 204f 7074 696f 6e61   wallet: Optiona
+00000840: 6c5b 4368 6563 6b73 756d 4164 6472 6573  l[ChecksumAddres
+00000850: 735d 203d 204e 6f6e 652c 0a20 2020 2020  s] = None,.     
+00000860: 2020 206b 6579 3a20 4f70 7469 6f6e 616c     key: Optional
+00000870: 5b73 7472 5d20 3d20 4e6f 6e65 0a20 2020  [str] = None.   
+00000880: 2029 202d 3e20 2242 6173 6543 6f6e 7472   ) -> "BaseContr
+00000890: 6163 7422 3a0a 2020 2020 2020 2020 2222  act":.        ""
+000008a0: 2243 7265 6174 6520 6120 4261 7365 436f  "Create a BaseCo
+000008b0: 6e74 7261 6374 2069 6e73 7461 6e63 6520  ntract instance 
+000008c0: 6672 6f6d 2074 6865 2063 6f6e 7472 6163  from the contrac
+000008d0: 7420 6164 6472 6573 7320 616e 6420 4142  t address and AB
+000008e0: 492e 0a0a 2020 2020 2020 2020 3a70 6172  I...        :par
+000008f0: 616d 2077 333a 2054 6865 2057 6562 3320  am w3: The Web3 
+00000900: 696e 7374 616e 6365 2e0a 2020 2020 2020  instance..      
+00000910: 2020 3a74 7970 6520 7733 3a20 5765 6233    :type w3: Web3
+00000920: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000930: 6164 6472 6573 733a 2054 6865 2061 6464  address: The add
+00000940: 7265 7373 206f 6620 7468 6520 636f 6e74  ress of the cont
+00000950: 7261 6374 2e0a 2020 2020 2020 2020 3a74  ract..        :t
+00000960: 7970 6520 6164 6472 6573 733a 2043 6865  ype address: Che
+00000970: 636b 7375 6d41 6464 7265 7373 0a20 2020  cksumAddress.   
+00000980: 2020 2020 203a 7061 7261 6d20 636f 6e74       :param cont
+00000990: 7261 6374 5f61 6269 3a20 5468 6520 4142  ract_abi: The AB
+000009a0: 4920 6f66 2074 6865 2063 6f6e 7472 6163  I of the contrac
+000009b0: 742e 0a20 2020 2020 2020 203a 7479 7065  t..        :type
+000009c0: 2063 6f6e 7472 6163 745f 6162 693a 2041   contract_abi: A
+000009d0: 4249 0a20 2020 2020 2020 203a 7061 7261  BI.        :para
+000009e0: 6d20 7761 6c6c 6574 3a20 5468 6520 7761  m wallet: The wa
+000009f0: 6c6c 6574 2061 6464 7265 7373 2074 6f20  llet address to 
+00000a00: 7573 6520 666f 7220 696e 7465 7261 6374  use for interact
+00000a10: 696e 6720 7769 7468 2074 6865 2063 6f6e  ing with the con
+00000a20: 7472 6163 7420 286f 7074 696f 6e61 6c2c  tract (optional,
+00000a30: 2064 6566 6175 6c74 2069 7320 4e6f 6e65   default is None
+00000a40: 292e 0a20 2020 2020 2020 203a 7479 7065  )..        :type
+00000a50: 2077 616c 6c65 743a 204f 7074 696f 6e61   wallet: Optiona
+00000a60: 6c5b 4368 6563 6b73 756d 4164 6472 6573  l[ChecksumAddres
+00000a70: 735d 0a20 2020 2020 2020 203a 7061 7261  s].        :para
+00000a80: 6d20 6b65 793a 2054 6865 2070 7269 7661  m key: The priva
+00000a90: 7465 206b 6579 206f 6620 7468 6520 7761  te key of the wa
+00000aa0: 6c6c 6574 2028 6f70 7469 6f6e 616c 2c20  llet (optional, 
+00000ab0: 6465 6661 756c 7420 6973 204e 6f6e 6529  default is None)
+00000ac0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00000ad0: 6b65 793a 204f 7074 696f 6e61 6c5b 7374  key: Optional[st
+00000ae0: 725d 0a20 2020 2020 2020 203a 7265 7475  r].        :retu
+00000af0: 726e 3a20 416e 2069 6e73 7461 6e63 6520  rn: An instance 
+00000b00: 6f66 2042 6173 6543 6f6e 7472 6163 742e  of BaseContract.
+00000b10: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00000b20: 2042 6173 6543 6f6e 7472 6163 740a 2020   BaseContract.  
+00000b30: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00000b40: 2020 2063 6f6e 7472 6163 7420 3d20 7733     contract = w3
+00000b50: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
+00000b60: 6472 6573 733d 6164 6472 6573 732c 2061  dress=address, a
+00000b70: 6269 3d63 6f6e 7472 6163 745f 6162 6929  bi=contract_abi)
+00000b80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000b90: 2063 6c73 2877 333d 7733 2c20 636f 6e74   cls(w3=w3, cont
+00000ba0: 7261 6374 3d63 6f6e 7472 6163 742c 2077  ract=contract, w
+00000bb0: 616c 6c65 743d 7761 6c6c 6574 2c20 6b65  allet=wallet, ke
+00000bc0: 793d 6b65 7929 0a0a 2020 2020 2323 2323  y=key)..    ####
+00000bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000c00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000c10: 2323 0a20 2020 2023 2065 7665 6e74 206c  ##.    # event l
+00000c20: 6973 7465 6e65 7273 0a20 2020 2023 2323  isteners.    ###
+00000c30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000c40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000c50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000c60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000c70: 2323 230a 0a20 2020 2023 2054 4f44 4f3a  ###..    # TODO:
+00000c80: 2072 6576 6973 6974 2070 6f6c 6c20 7469   revisit poll ti
+00000c90: 6d65 2e20 5269 6768 7420 6e6f 7720 6974  me. Right now it
+00000ca0: 2069 7320 7365 7420 746f 2062 6c6f 636b   is set to block
+00000cb0: 2070 726f 6475 6374 696f 6e20 7469 6d65   production time
+00000cc0: 206f 6620 6f70 7469 6d69 736d 2061 6363   of optimism acc
+00000cd0: 6f72 6469 6e67 2074 6f3a 0a20 2020 2023  ording to:.    #
+00000ce0: 2020 6874 7470 733a 2f2f 636f 6d6d 756e    https://commun
+00000cf0: 6974 792e 6f70 7469 6d69 736d 2e69 6f2f  ity.optimism.io/
+00000d00: 646f 6373 2f70 726f 746f 636f 6c2f 322d  docs/protocol/2-
+00000d10: 726f 6c6c 7570 2d70 726f 746f 636f 6c2f  rollup-protocol/
+00000d20: 2362 6c6f 636b 2d73 746f 7261 6765 0a20  #block-storage. 
+00000d30: 2020 2023 2020 686f 7765 7665 7220 6172     #  however ar
+00000d40: 6269 7472 756d 2070 726f 6475 6365 7320  bitrum produces 
+00000d50: 626c 6f63 6b73 2066 6173 7465 7220 2865  blocks faster (e
+00000d60: 7665 7279 2030 2e32 3520 7365 6373 2920  very 0.25 secs) 
+00000d70: 6163 636f 7264 696e 6720 746f 3a0a 2020  according to:.  
+00000d80: 2020 2320 2068 7474 7073 3a2f 2f61 7262    #  https://arb
+00000d90: 6973 6361 6e2e 696f 2f63 6861 7274 2f62  iscan.io/chart/b
+00000da0: 6c6f 636b 7469 6d65 2073 6f20 7765 206d  locktime so we m
+00000db0: 6179 2062 6520 7072 7564 656e 7420 746f  ay be prudent to
+00000dc0: 2061 6363 6f75 6e74 2066 6f72 2064 6966   account for dif
+00000dd0: 6665 7265 6e74 2063 6861 696e 730a 2020  ferent chains.  
+00000de0: 2020 2320 2068 6f77 6576 6572 2074 6865    #  however the
+00000df0: 2062 6574 7465 7220 7761 7920 746f 2064   better way to d
+00000e00: 6f20 7468 6973 2069 7320 7072 6f62 6162  o this is probab
+00000e10: 6c79 2061 2077 6562 736f 636b 6574 2063  ly a websocket c
+00000e20: 6f6e 6e65 6374 696f 6e20 746f 2074 6865  onnection to the
+00000e30: 206e 6f64 650a 2020 2020 2320 544f 444f   node.    # TODO
+00000e40: 3a20 696e 7665 7374 6967 6174 6520 7573  : investigate us
+00000e50: 696e 6720 6120 6d6f 7265 2067 656e 6572  ing a more gener
+00000e60: 6963 2066 696c 7465 7220 736f 2074 6861  ic filter so tha
+00000e70: 7420 796f 7520 646f 6e27 7420 6e65 6564  t you don't need
+00000e80: 2074 6f20 706f 6c6c 2066 6f72 2065 6163   to poll for eac
+00000e90: 6820 6576 656e 7420 6173 2074 6869 7320  h event as this 
+00000ea0: 636f 756c 640a 2020 2020 2320 2073 7061  could.    #  spa
+00000eb0: 6d20 7468 6520 6e6f 6465 2074 6861 7420  m the node that 
+00000ec0: 6973 2062 6569 6e67 2063 6f6e 6e65 6374  is being connect
+00000ed0: 6564 2074 6f0a 2020 2020 6465 6620 7374  ed to.    def st
+00000ee0: 6172 745f 6576 656e 745f 706f 6c6c 6572  art_event_poller
+00000ef0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00000f00: 2020 2020 2020 2020 7061 6972 5f6e 616d          pair_nam
+00000f10: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00000f20: 6576 656e 745f 7479 7065 3a20 5479 7065  event_type: Type
+00000f30: 5b42 6173 6545 7665 6e74 5d2c 0a20 2020  [BaseEvent],.   
+00000f40: 2020 2020 2061 7267 756d 656e 745f 6669       argument_fi
+00000f50: 6c74 6572 733a 204f 7074 696f 6e61 6c5b  lters: Optional[
+00000f60: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
+00000f70: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00000f80: 6576 656e 745f 6861 6e64 6c65 723a 204f  event_handler: O
+00000f90: 7074 696f 6e61 6c5b 4361 6c6c 6162 6c65  ptional[Callable
+00000fa0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00000fb0: 2020 706f 6c6c 5f74 696d 653a 2069 6e74    poll_time: int
+00000fc0: 203d 2032 0a20 2020 2029 202d 3e20 4e6f   = 2.    ) -> No
+00000fd0: 6e65 3a0a 2020 2020 2020 2020 2222 2253  ne:.        """S
+00000fe0: 7461 7274 2061 2074 6872 6561 6420 7768  tart a thread wh
+00000ff0: 6963 6820 7275 6e73 2061 6e20 6576 656e  ich runs an even
+00001000: 7420 706f 6c6c 6572 2066 6f72 2061 2073  t poller for a s
+00001010: 7065 6369 6669 6320 6576 656e 7420 7479  pecific event ty
+00001020: 7065 2e0a 0a20 2020 2020 2020 203a 7061  pe...        :pa
+00001030: 7261 6d20 7061 6972 5f6e 616d 653a 2054  ram pair_name: T
+00001040: 6865 206e 616d 6520 6f66 2074 6865 2070  he name of the p
+00001050: 6169 7220 7765 2061 7265 206d 6f6e 6974  air we are monit
+00001060: 6f72 696e 6720 6576 656e 7473 206f 662e  oring events of.
+00001070: 0a20 2020 2020 2020 203a 7479 7065 2070  .        :type p
+00001080: 6169 725f 6e61 6d65 3a20 7374 720a 2020  air_name: str.  
+00001090: 2020 2020 2020 3a70 6172 616d 2065 7665        :param eve
+000010a0: 6e74 5f74 7970 653a 2054 6865 2074 7970  nt_type: The typ
+000010b0: 6520 6f66 2065 7665 6e74 2074 6f20 706f  e of event to po
+000010c0: 6c6c 2066 6f72 2e0a 2020 2020 2020 2020  ll for..        
+000010d0: 3a74 7970 6520 6576 656e 745f 7479 7065  :type event_type
+000010e0: 3a20 5479 7065 5b42 6173 6545 7665 6e74  : Type[BaseEvent
+000010f0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+00001100: 2061 7267 756d 656e 745f 6669 6c74 6572   argument_filter
+00001110: 733a 204f 7074 696f 6e61 6c20 6669 6c74  s: Optional filt
+00001120: 6572 7320 7468 6174 2074 6865 206e 6f64  ers that the nod
+00001130: 6520 7769 6c6c 2066 696c 7465 7220 6576  e will filter ev
+00001140: 656e 7473 206f 6e20 286f 7074 696f 6e61  ents on (optiona
+00001150: 6c2c 2064 6566 6175 6c74 2069 7320 4e6f  l, default is No
+00001160: 6e65 292e 0a20 2020 2020 2020 203a 7479  ne)..        :ty
+00001170: 7065 2061 7267 756d 656e 745f 6669 6c74  pe argument_filt
+00001180: 6572 733a 204f 7074 696f 6e61 6c5b 4469  ers: Optional[Di
+00001190: 6374 5b73 7472 2c20 416e 795d 5d0a 2020  ct[str, Any]].  
+000011a0: 2020 2020 2020 3a70 6172 616d 2065 7665        :param eve
+000011b0: 6e74 5f68 616e 646c 6572 3a20 4f70 7469  nt_handler: Opti
+000011c0: 6f6e 616c 2065 7665 6e74 2068 616e 646c  onal event handl
+000011d0: 6572 2066 756e 6374 696f 6e2e 2044 6566  er function. Def
+000011e0: 6175 6c74 7320 746f 2075 7369 6e67 2074  aults to using t
+000011f0: 6865 2065 7665 6e74 7320 6465 6661 756c  he events defaul
+00001200: 7420 6861 6e64 6c65 722e 0a20 2020 2020  t handler..     
+00001210: 2020 203a 7479 7065 2065 7665 6e74 5f68     :type event_h
+00001220: 616e 646c 6572 3a20 4f70 7469 6f6e 616c  andler: Optional
+00001230: 5b43 616c 6c61 626c 655d 0a20 2020 2020  [Callable].     
+00001240: 2020 203a 7061 7261 6d20 706f 6c6c 5f74     :param poll_t
+00001250: 696d 653a 2054 6865 2074 696d 6520 696e  ime: The time in
+00001260: 7465 7276 616c 2062 6574 7765 656e 2065  terval between e
+00001270: 6163 6820 706f 6c6c 2069 6e20 7365 636f  ach poll in seco
+00001280: 6e64 732e 2044 6566 6175 6c74 7320 746f  nds. Defaults to
+00001290: 2032 2073 6563 6f6e 6473 2e0a 2020 2020   2 seconds..    
+000012a0: 2020 2020 3a74 7970 6520 706f 6c6c 5f74      :type poll_t
+000012b0: 696d 653a 2069 6e74 0a20 2020 2020 2020  ime: int.       
+000012c0: 2022 2222 0a0a 2020 2020 2020 2020 6576   """..        ev
+000012d0: 656e 745f 6669 6c74 6572 203d 2065 7665  ent_filter = eve
+000012e0: 6e74 5f74 7970 652e 6372 6561 7465 5f65  nt_type.create_e
+000012f0: 7665 6e74 5f66 696c 7465 7228 636f 6e74  vent_filter(cont
+00001300: 7261 6374 3d73 656c 662e 636f 6e74 7261  ract=self.contra
+00001310: 6374 2c20 6172 6775 6d65 6e74 5f66 696c  ct, argument_fil
+00001320: 7465 7273 3d61 7267 756d 656e 745f 6669  ters=argument_fi
+00001330: 6c74 6572 7329 0a20 2020 2020 2020 2068  lters).        h
+00001340: 616e 646c 6572 203d 2065 7665 6e74 5f68  andler = event_h
+00001350: 616e 646c 6572 2069 6620 6576 656e 745f  andler if event_
+00001360: 6861 6e64 6c65 7220 6973 206e 6f74 204e  handler is not N
+00001370: 6f6e 6520 656c 7365 2065 7665 6e74 5f74  one else event_t
+00001380: 7970 652e 6465 6661 756c 745f 6861 6e64  ype.default_hand
+00001390: 6c65 720a 0a20 2020 2020 2020 2074 6872  ler..        thr
+000013a0: 6561 6420 3d20 5468 7265 6164 280a 2020  ead = Thread(.  
+000013b0: 2020 2020 2020 2020 2020 7461 7267 6574            target
+000013c0: 3d73 656c 662e 5f73 7461 7274 5f64 6566  =self._start_def
+000013d0: 6175 6c74 5f65 7665 6e74 5f70 6f6c 6c65  ault_event_polle
+000013e0: 722c 0a20 2020 2020 2020 2020 2020 2061  r,.            a
+000013f0: 7267 733d 2870 6169 725f 6e61 6d65 2c20  rgs=(pair_name, 
+00001400: 6576 656e 745f 7479 7065 2c20 6576 656e  event_type, even
+00001410: 745f 6669 6c74 6572 2c20 6861 6e64 6c65  t_filter, handle
+00001420: 722c 2070 6f6c 6c5f 7469 6d65 292c 0a20  r, poll_time),. 
+00001430: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
+00001440: 6e3d 5472 7565 0a20 2020 2020 2020 2029  n=True.        )
+00001450: 0a20 2020 2020 2020 2074 6872 6561 642e  .        thread.
+00001460: 7374 6172 7428 290a 0a20 2020 2040 7374  start()..    @st
+00001470: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00001480: 6566 205f 7374 6172 745f 6465 6661 756c  ef _start_defaul
+00001490: 745f 6576 656e 745f 706f 6c6c 6572 280a  t_event_poller(.
+000014a0: 2020 2020 2020 2020 7061 6972 5f6e 616d          pair_nam
+000014b0: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+000014c0: 6576 656e 745f 7479 7065 3a20 5479 7065  event_type: Type
+000014d0: 5b42 6173 6545 7665 6e74 5d2c 0a20 2020  [BaseEvent],.   
+000014e0: 2020 2020 2065 7665 6e74 5f66 696c 7465       event_filte
+000014f0: 723a 204c 6f67 4669 6c74 6572 2c0a 2020  r: LogFilter,.  
+00001500: 2020 2020 2020 6576 656e 745f 6861 6e64        event_hand
+00001510: 6c65 723a 2043 616c 6c61 626c 652c 0a20  ler: Callable,. 
+00001520: 2020 2020 2020 2070 6f6c 6c5f 7469 6d65         poll_time
+00001530: 3a20 696e 740a 2020 2020 2920 2d3e 204e  : int.    ) -> N
+00001540: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00001550: 5374 6172 7420 7468 6520 6465 6661 756c  Start the defaul
+00001560: 7420 6576 656e 7420 706f 6c6c 6572 206c  t event poller l
+00001570: 6f6f 702e 2054 6869 7320 7468 7265 6164  oop. This thread
+00001580: 2077 696c 6c20 7374 6f70 2069 6620 7468   will stop if th
+00001590: 6520 7061 6972 2069 7320 7265 6d6f 7665  e pair is remove
+000015a0: 6420 6672 6f6d 2074 6865 2063 6c69 656e  d from the clien
+000015b0: 742e 0a0a 2020 2020 2020 2020 3a70 6172  t...        :par
+000015c0: 616d 2070 6169 725f 6e61 6d65 3a20 5468  am pair_name: Th
+000015d0: 6520 6e61 6d65 206f 6620 7468 6520 6576  e name of the ev
+000015e0: 656e 7420 7061 6972 2e0a 2020 2020 2020  ent pair..      
+000015f0: 2020 3a74 7970 6520 7061 6972 5f6e 616d    :type pair_nam
+00001600: 653a 2073 7472 0a20 2020 2020 2020 203a  e: str.        :
+00001610: 7061 7261 6d20 6576 656e 745f 7479 7065  param event_type
+00001620: 3a20 5468 6520 7479 7065 206f 6620 7468  : The type of th
+00001630: 6520 6576 656e 742e 0a20 2020 2020 2020  e event..       
+00001640: 203a 7479 7065 2065 7665 6e74 5f74 7970   :type event_typ
+00001650: 653a 2054 7970 655b 4261 7365 4576 656e  e: Type[BaseEven
+00001660: 745d 0a20 2020 2020 2020 203a 7061 7261  t].        :para
+00001670: 6d20 6576 656e 745f 6669 6c74 6572 3a20  m event_filter: 
+00001680: 5468 6520 6576 656e 7420 6669 6c74 6572  The event filter
+00001690: 2074 6f20 7265 7472 6965 7665 206e 6577   to retrieve new
+000016a0: 2065 6e74 7269 6573 2e0a 2020 2020 2020   entries..      
+000016b0: 2020 3a74 7970 6520 6576 656e 745f 6669    :type event_fi
+000016c0: 6c74 6572 3a20 4c6f 6746 696c 7465 720a  lter: LogFilter.
+000016d0: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
+000016e0: 7665 6e74 5f68 616e 646c 6572 3a20 5468  vent_handler: Th
+000016f0: 6520 6576 656e 7420 6861 6e64 6c65 7220  e event handler 
+00001700: 6675 6e63 7469 6f6e 2e0a 2020 2020 2020  function..      
+00001710: 2020 3a74 7970 6520 6576 656e 745f 6861    :type event_ha
+00001720: 6e64 6c65 723a 2043 616c 6c61 626c 650a  ndler: Callable.
+00001730: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00001740: 6f6c 6c5f 7469 6d65 3a20 5468 6520 7469  oll_time: The ti
+00001750: 6d65 2069 6e74 6572 7661 6c20 6265 7477  me interval betw
+00001760: 6565 6e20 706f 6c6c 2069 7465 7261 7469  een poll iterati
+00001770: 6f6e 7320 696e 2073 6563 6f6e 6473 2e0a  ons in seconds..
+00001780: 2020 2020 2020 2020 3a74 7970 6520 706f          :type po
+00001790: 6c6c 5f74 696d 653a 2069 6e74 0a20 2020  ll_time: int.   
+000017a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000017b0: 2070 6f6c 6c69 6e67 203d 2054 7275 650a   polling = True.
+000017c0: 0a20 2020 2020 2020 2077 6869 6c65 2070  .        while p
+000017d0: 6f6c 6c69 6e67 3a0a 2020 2020 2020 2020  olling:.        
+000017e0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000017f0: 2020 2020 2020 2020 2066 6f72 2065 7665           for eve
+00001800: 6e74 5f64 6174 6120 696e 2065 7665 6e74  nt_data in event
+00001810: 5f66 696c 7465 722e 6765 745f 6e65 775f  _filter.get_new_
+00001820: 656e 7472 6965 7328 293a 0a20 2020 2020  entries():.     
+00001830: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00001840: 7665 6e74 5f68 616e 646c 6572 2870 6169  vent_handler(pai
+00001850: 725f 6e61 6d65 2c20 6576 656e 745f 7479  r_name, event_ty
+00001860: 7065 2c20 6576 656e 745f 6461 7461 290a  pe, event_data).
+00001870: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00001880: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00001890: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000018a0: 2020 206c 6f67 2e65 7272 6f72 2865 290a     log.error(e).
+000018b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018c0: 2023 2054 4f44 4f3a 2074 6869 7320 6973   # TODO: this is
+000018d0: 2061 2068 6163 6b20 746f 2064 6574 6563   a hack to detec
+000018e0: 7420 6966 2061 2050 6169 7244 6f65 734e  t if a PairDoesN
+000018f0: 6f74 4578 6973 7445 7863 6570 7469 6f6e  otExistException
+00001900: 2069 7320 7261 6973 6564 2061 6e64 2070   is raised and p
+00001910: 6f6c 6c69 6e67 2073 686f 756c 6420 7374  olling should st
+00001920: 6f70 2e0a 2020 2020 2020 2020 2020 2020  op..            
+00001930: 2020 2020 2320 2043 7572 7265 6e74 6c79      #  Currently
+00001940: 2061 6e20 6164 6469 7469 6f6e 616c 2065   an additional e
+00001950: 7863 6570 7420 5061 6972 446f 6573 4e6f  xcept PairDoesNo
+00001960: 7445 7869 7374 4578 6365 7074 696f 6e20  tExistException 
+00001970: 6173 2065 3a20 6361 6e6e 6f74 2062 6520  as e: cannot be 
+00001980: 6164 6465 6420 6173 2074 6869 7320 6361  added as this ca
+00001990: 7573 6573 2061 0a20 2020 2020 2020 2020  uses a.         
+000019a0: 2020 2020 2020 2023 2020 6369 7263 756c         #  circul
+000019b0: 6172 2069 6d70 6f72 742e 2054 6869 6e6b  ar import. Think
+000019c0: 2061 626f 7574 2072 6573 7472 7563 7475   about restructu
+000019d0: 7269 6e67 2074 6865 2064 6972 6563 746f  ring the directo
+000019e0: 7269 6573 2074 6f20 6176 6f69 6420 7468  ries to avoid th
+000019f0: 6973 2028 652e 6720 6f6e 6520 726f 6f74  is (e.g one root
+00001a00: 206c 6576 656c 2074 7970 6573 0a20 2020   level types.   
+00001a10: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+00001a20: 6469 7265 6374 6f72 7929 2e0a 2020 2020  directory)..    
+00001a30: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00001a40: 6164 6420 7061 6972 2074 6f20 7468 6520  add pair to the 
+00001a50: 636c 6965 6e74 2220 696e 2073 7472 2865  client" in str(e
+00001a60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00001a70: 2020 2020 2020 2070 6f6c 6c69 6e67 203d         polling =
+00001a80: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+00001a90: 2020 2020 736c 6565 7028 706f 6c6c 5f74      sleep(poll_t
+00001aa0: 696d 6529 0a0a 2020 2020 2323 2323 2323  ime)..    ######
+00001ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001af0: 0a20 2020 2023 2068 656c 7065 7220 6d65  .    # helper me
+00001b00: 7468 6f64 730a 2020 2020 2323 2323 2323  thods.    ######
+00001b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001b50: 0a0a 2020 2020 6465 6620 5f64 6566 6175  ..    def _defau
+00001b60: 6c74 5f74 7261 6e73 6163 7469 6f6e 5f68  lt_transaction_h
+00001b70: 616e 646c 6572 280a 2020 2020 2020 2020  andler(.        
+00001b80: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
+00001b90: 7374 616e 7469 6174 6564 5f63 6f6e 7472  stantiated_contr
+00001ba0: 6163 745f 6675 6e63 7469 6f6e 3a20 436f  act_function: Co
+00001bb0: 6e74 7261 6374 4675 6e63 7469 6f6e 2c0a  ntractFunction,.
+00001bc0: 2020 2020 2020 2020 6761 733a 2069 6e74          gas: int
+00001bd0: 2c0a 2020 2020 2020 2020 6e6f 6e63 653a  ,.        nonce:
+00001be0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00001bf0: 204e 6f6e 652c 0a20 2020 2020 2020 206d   None,.        m
+00001c00: 6178 5f66 6565 5f70 6572 5f67 6173 3a20  ax_fee_per_gas: 
+00001c10: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00001c20: 4e6f 6e65 2c0a 2020 2020 2020 2020 6d61  None,.        ma
+00001c30: 785f 7072 696f 7269 7479 5f66 6565 5f70  x_priority_fee_p
+00001c40: 6572 5f67 6173 3a20 4f70 7469 6f6e 616c  er_gas: Optional
+00001c50: 5b69 6e74 5d20 3d20 4e6f 6e65 0a20 2020  [int] = None.   
+00001c60: 2029 202d 3e20 5472 616e 7361 6374 696f   ) -> Transactio
+00001c70: 6e52 6563 6569 7074 3a0a 2020 2020 2020  nReceipt:.      
+00001c80: 2020 2222 2244 6566 6175 6c74 2074 7261    """Default tra
+00001c90: 6e73 6163 7469 6f6e 2068 616e 646c 6572  nsaction handler
+00001ca0: 2066 6f72 2065 7865 6375 7469 6e67 2074   for executing t
+00001cb0: 7261 6e73 6163 7469 6f6e 7320 6167 6169  ransactions agai
+00001cc0: 6e73 7420 7468 6973 2063 6f6e 7472 6163  nst this contrac
+00001cd0: 742e 2054 6869 7320 6675 6e63 7469 6f6e  t. This function
+00001ce0: 2077 696c 6c20 6275 696c 642c 2073 6967   will build, sig
+00001cf0: 6e0a 2020 2020 2020 2020 616e 6420 6578  n.        and ex
+00001d00: 6563 7574 6520 6120 7472 616e 7361 6374  ecute a transact
+00001d10: 696f 6e20 7769 7468 2072 6561 736f 6e61  ion with reasona
+00001d20: 626c 6520 6465 6661 756c 7473 2028 6d6f  ble defaults (mo
+00001d30: 7374 6c79 2066 726f 6d20 7468 6520 7765  stly from the we
+00001d40: 6233 7079 206c 6962 7261 7279 292e 0a0a  b3py library)...
+00001d50: 2020 2020 2020 2020 4e6f 7465 3a20 6966          Note: if
+00001d60: 2061 206e 6f6e 6365 2069 7320 6e6f 7420   a nonce is not 
+00001d70: 7061 7373 6564 2074 6865 6e20 7468 6973  passed then this
+00001d80: 2066 756e 6374 696f 6e20 7769 6c6c 2071   function will q
+00001d90: 7565 7279 2074 6f20 7468 6520 7761 6c6c  uery to the wall
+00001da0: 6574 2074 6f20 6765 7420 7468 6520 6e6f  et to get the no
+00001db0: 6e63 6520 616e 6420 616c 736f 2077 6169  nce and also wai
+00001dc0: 7420 666f 720a 2020 2020 2020 2020 7468  t for.        th
+00001dd0: 6520 7472 616e 7361 6374 696f 6e20 7265  e transaction re
+00001de0: 6365 6970 7420 6265 666f 7265 2072 6574  ceipt before ret
+00001df0: 7572 6e69 6e67 2e0a 0a20 2020 2020 2020  urning...       
+00001e00: 203a 7061 7261 6d20 696e 7374 616e 7469   :param instanti
+00001e10: 6174 6564 5f63 6f6e 7472 6163 745f 6675  ated_contract_fu
+00001e20: 6e63 7469 6f6e 3a20 5468 6520 696e 7374  nction: The inst
+00001e30: 616e 7469 6174 6564 2063 6f6e 7472 6163  antiated contrac
+00001e40: 7420 6675 6e63 7469 6f6e 2074 6f20 6361  t function to ca
+00001e50: 6c6c 2e0a 2020 2020 2020 2020 3a74 7970  ll..        :typ
+00001e60: 6520 696e 7374 616e 7469 6174 6564 5f63  e instantiated_c
+00001e70: 6f6e 7472 6163 745f 6675 6e63 7469 6f6e  ontract_function
+00001e80: 3a20 436f 6e74 7261 6374 4675 6e63 7469  : ContractFuncti
+00001e90: 6f6e 0a20 2020 2020 2020 203a 7061 7261  on.        :para
+00001ea0: 6d20 6761 733a 2054 6865 2067 6173 206c  m gas: The gas l
+00001eb0: 696d 6974 2066 6f72 2074 6865 2074 7261  imit for the tra
+00001ec0: 6e73 6163 7469 6f6e 2e0a 2020 2020 2020  nsaction..      
+00001ed0: 2020 3a74 7970 6520 6761 733a 2069 6e74    :type gas: int
+00001ee0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001ef0: 6e6f 6e63 653a 204f 7074 696f 6e61 6c20  nonce: Optional 
+00001f00: 6e6f 6e63 6520 7661 6c75 6520 666f 7220  nonce value for 
+00001f10: 7468 6520 7472 616e 7361 6374 696f 6e20  the transaction 
+00001f20: 286f 7074 696f 6e61 6c2c 2064 6566 6175  (optional, defau
+00001f30: 6c74 2069 7320 4e6f 6e65 292e 0a20 2020  lt is None)..   
+00001f40: 2020 2020 203a 7479 7065 206e 6f6e 6365       :type nonce
+00001f50: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0a  : Optional[int].
+00001f60: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
+00001f70: 6178 5f66 6565 5f70 6572 5f67 6173 3a20  ax_fee_per_gas: 
+00001f80: 4f70 7469 6f6e 616c 206d 6178 696d 756d  Optional maximum
+00001f90: 2066 6565 2070 6572 2067 6173 2066 6f72   fee per gas for
+00001fa0: 2074 6865 2074 7261 6e73 6163 7469 6f6e   the transaction
+00001fb0: 2028 6f70 7469 6f6e 616c 2c20 6465 6661   (optional, defa
+00001fc0: 756c 7420 6973 204e 6f6e 6529 2e0a 2020  ult is None)..  
+00001fd0: 2020 2020 2020 3a74 7970 6520 6d61 785f        :type max_
+00001fe0: 6665 655f 7065 725f 6761 733a 204f 7074  fee_per_gas: Opt
+00001ff0: 696f 6e61 6c5b 696e 745d 0a20 2020 2020  ional[int].     
+00002000: 2020 203a 7061 7261 6d20 6d61 785f 7072     :param max_pr
+00002010: 696f 7269 7479 5f66 6565 5f70 6572 5f67  iority_fee_per_g
+00002020: 6173 3a20 4f70 7469 6f6e 616c 206d 6178  as: Optional max
+00002030: 696d 756d 2070 7269 6f72 6974 7920 6665  imum priority fe
+00002040: 6520 7065 7220 6761 7320 666f 7220 7468  e per gas for th
+00002050: 6520 7472 616e 7361 6374 696f 6e2e 0a20  e transaction.. 
+00002060: 2020 2020 2020 2020 2020 2028 6f70 7469             (opti
+00002070: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
+00002080: 204e 6f6e 6529 2e0a 2020 2020 2020 2020   None)..        
+00002090: 3a74 7970 6520 6d61 785f 7072 696f 7269  :type max_priori
+000020a0: 7479 5f66 6565 5f70 6572 5f67 6173 3a20  ty_fee_per_gas: 
+000020b0: 4f70 7469 6f6e 616c 5b69 6e74 5d0a 2020  Optional[int].  
+000020c0: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
+000020d0: 6e20 6f62 6a65 6374 2072 6570 7265 7365  n object represe
+000020e0: 6e74 696e 6720 7468 6520 7472 616e 7361  nting the transa
+000020f0: 6374 696f 6e20 7265 6365 6970 740a 2020  ction receipt.  
+00002100: 2020 2020 2020 3a72 7479 7065 3a20 5472        :rtype: Tr
+00002110: 616e 7361 6374 696f 6e52 6563 6569 7074  ansactionReceipt
+00002120: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002130: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00002140: 2e73 6967 6e69 6e67 5f70 6572 6d69 7373  .signing_permiss
+00002150: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+00002160: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+00002170: 6e28 6622 6361 6e6e 6f74 2077 7269 7465  n(f"cannot write
+00002180: 2074 7261 6e73 6163 7469 6f6e 2077 6974   transaction wit
+00002190: 686f 7574 2073 6967 6e69 6e67 2072 6967  hout signing rig
+000021a0: 6874 732e 2022 0a20 2020 2020 2020 2020  hts. ".         
+000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021c0: 2020 2066 2272 652d 696e 7374 616e 7469     f"re-instanti
+000021d0: 6174 6520 7b73 656c 662e 5f5f 636c 6173  ate {self.__clas
+000021e0: 735f 5f7d 2077 6974 6820 6120 7761 6c6c  s__} with a wall
+000021f0: 6574 2061 6e64 2070 7269 7661 7465 206b  et and private k
+00002200: 6579 2229 0a0a 2020 2020 2020 2020 6261  ey")..        ba
+00002210: 7365 5f74 786e 203d 2073 656c 662e 5f74  se_txn = self._t
+00002220: 7261 6e73 6163 7469 6f6e 5f70 6172 616d  ransaction_param
+00002230: 7328 0a20 2020 2020 2020 2020 2020 2067  s(.            g
+00002240: 6173 3d67 6173 2c0a 2020 2020 2020 2020  as=gas,.        
+00002250: 2020 2020 6e6f 6e63 653d 6e6f 6e63 652c      nonce=nonce,
+00002260: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00002270: 5f66 6565 5f70 6572 5f67 6173 3d6d 6178  _fee_per_gas=max
+00002280: 5f66 6565 5f70 6572 5f67 6173 2c0a 2020  _fee_per_gas,.  
+00002290: 2020 2020 2020 2020 2020 6d61 785f 7072            max_pr
+000022a0: 696f 7269 7479 5f66 6565 5f70 6572 5f67  iority_fee_per_g
+000022b0: 6173 3d6d 6178 5f70 7269 6f72 6974 795f  as=max_priority_
+000022c0: 6665 655f 7065 725f 6761 730a 2020 2020  fee_per_gas.    
+000022d0: 2020 2020 290a 0a20 2020 2020 2020 2074      )..        t
+000022e0: 786e 203d 2069 6e73 7461 6e74 6961 7465  xn = instantiate
+000022f0: 645f 636f 6e74 7261 6374 5f66 756e 6374  d_contract_funct
+00002300: 696f 6e2e 6275 696c 645f 7472 616e 7361  ion.build_transa
+00002310: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
+00002320: 2020 2074 7261 6e73 6163 7469 6f6e 3d62     transaction=b
+00002330: 6173 655f 7478 6e0a 2020 2020 2020 2020  ase_txn.        
+00002340: 290a 0a20 2020 2020 2020 2073 6967 6e65  )..        signe
+00002350: 645f 7478 6e20 3d20 7365 6c66 2e77 332e  d_txn = self.w3.
+00002360: 6574 682e 6163 636f 756e 742e 7369 676e  eth.account.sign
+00002370: 5f74 7261 6e73 6163 7469 6f6e 280a 2020  _transaction(.  
+00002380: 2020 2020 2020 2020 2020 7472 616e 7361            transa
+00002390: 6374 696f 6e5f 6469 6374 3d74 786e 2c0a  ction_dict=txn,.
+000023a0: 2020 2020 2020 2020 2020 2020 7072 6976              priv
+000023b0: 6174 655f 6b65 793d 7365 6c66 2e6b 6579  ate_key=self.key
+000023c0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+000023d0: 2020 2020 7365 6c66 2e77 332e 6574 682e      self.w3.eth.
+000023e0: 7365 6e64 5f72 6177 5f74 7261 6e73 6163  send_raw_transac
+000023f0: 7469 6f6e 2873 6967 6e65 645f 7478 6e2e  tion(signed_txn.
+00002400: 7261 7754 7261 6e73 6163 7469 6f6e 290a  rawTransaction).
+00002410: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002420: 7365 6c66 2e5f 7761 6974 5f66 6f72 5f74  self._wait_for_t
+00002430: 7261 6e73 6163 7469 6f6e 5f72 6563 6569  ransaction_recei
+00002440: 7074 2874 7261 6e73 6163 7469 6f6e 3d73  pt(transaction=s
+00002450: 6967 6e65 645f 7478 6e29 0a0a 2020 2020  igned_txn)..    
+00002460: 6465 6620 5f74 7261 6e73 6163 7469 6f6e  def _transaction
+00002470: 5f70 6172 616d 7328 0a20 2020 2020 2020  _params(.       
+00002480: 2073 656c 662c 0a20 2020 2020 2020 206e   self,.        n
+00002490: 6f6e 6365 3a20 4f70 7469 6f6e 616c 5b4e  once: Optional[N
+000024a0: 6f6e 6365 5d2c 0a20 2020 2020 2020 2067  once],.        g
+000024b0: 6173 3a20 696e 742c 0a20 2020 2020 2020  as: int,.       
+000024c0: 206d 6178 5f66 6565 5f70 6572 5f67 6173   max_fee_per_gas
+000024d0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d2c  : Optional[int],
+000024e0: 0a20 2020 2020 2020 206d 6178 5f70 7269  .        max_pri
+000024f0: 6f72 6974 795f 6665 655f 7065 725f 6761  ority_fee_per_ga
+00002500: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
+00002510: 0a20 2020 2029 202d 3e20 4469 6374 3a0a  .    ) -> Dict:.
+00002520: 2020 2020 2020 2020 2222 2242 7569 6c64          """Build
+00002530: 2074 7261 6e73 6163 7469 6f6e 2070 6172   transaction par
+00002540: 616d 6574 6572 7320 4469 6374 2066 6f72  ameters Dict for
+00002550: 2061 2074 7261 6e73 6163 7469 6f6e 2e20   a transaction. 
+00002560: 4966 2061 206b 6579 2069 7320 6173 736f  If a key is asso
+00002570: 6369 6174 6564 2077 6974 6820 6120 4e6f  ciated with a No
+00002580: 6e65 2076 616c 7565 2061 6674 6572 2062  ne value after b
+00002590: 7569 6c64 696e 670a 2020 2020 2020 2020  uilding.        
+000025a0: 7468 6520 4469 6374 2074 6865 6e20 7468  the Dict then th
+000025b0: 6973 206b 6579 2077 696c 6c20 6265 2072  is key will be r
+000025c0: 656d 6f76 6564 2062 6566 6f72 6520 7265  emoved before re
+000025d0: 7475 726e 696e 6720 7468 6520 6469 6374  turning the dict
+000025e0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+000025f0: 6d20 6e6f 6e63 653a 204f 7074 696f 6e61  m nonce: Optiona
+00002600: 6c20 6e6f 6e63 6520 7661 6c75 6520 666f  l nonce value fo
+00002610: 7220 7468 6520 7472 616e 7361 6374 696f  r the transactio
+00002620: 6e20 286f 7074 696f 6e61 6c2c 2064 6566  n (optional, def
+00002630: 6175 6c74 2069 7320 4e6f 6e65 292e 0a20  ault is None).. 
+00002640: 2020 2020 2020 203a 7479 7065 206e 6f6e         :type non
+00002650: 6365 3a20 4f70 7469 6f6e 616c 5b4e 6f6e  ce: Optional[Non
+00002660: 6365 5d0a 2020 2020 2020 2020 3a70 6172  ce].        :par
+00002670: 616d 2067 6173 3a20 5468 6520 6761 7320  am gas: The gas 
+00002680: 6c69 6d69 7420 666f 7220 7468 6520 7472  limit for the tr
+00002690: 616e 7361 6374 696f 6e2e 0a20 2020 2020  ansaction..     
+000026a0: 2020 203a 7479 7065 2067 6173 3a20 696e     :type gas: in
+000026b0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+000026c0: 206d 6178 5f66 6565 5f70 6572 5f67 6173   max_fee_per_gas
+000026d0: 3a20 4f70 7469 6f6e 616c 206d 6178 696d  : Optional maxim
+000026e0: 756d 2066 6565 2070 6572 2067 6173 2066  um fee per gas f
+000026f0: 6f72 2074 6865 2074 7261 6e73 6163 7469  or the transacti
+00002700: 6f6e 2028 6f70 7469 6f6e 616c 2c20 6465  on (optional, de
+00002710: 6661 756c 7420 6973 204e 6f6e 6529 2e0a  fault is None)..
+00002720: 2020 2020 2020 2020 3a74 7970 6520 6d61          :type ma
+00002730: 785f 6665 655f 7065 725f 6761 733a 204f  x_fee_per_gas: O
+00002740: 7074 696f 6e61 6c5b 696e 745d 0a20 2020  ptional[int].   
+00002750: 2020 2020 203a 7061 7261 6d20 6d61 785f       :param max_
+00002760: 7072 696f 7269 7479 5f66 6565 5f70 6572  priority_fee_per
+00002770: 5f67 6173 3a20 4f70 7469 6f6e 616c 206d  _gas: Optional m
+00002780: 6178 696d 756d 2070 7269 6f72 6974 7920  aximum priority 
+00002790: 6665 6520 7065 7220 6761 7320 666f 7220  fee per gas for 
+000027a0: 7468 6520 7472 616e 7361 6374 696f 6e2e  the transaction.
+000027b0: 0a20 2020 2020 2020 2020 2020 2028 6f70  .            (op
+000027c0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+000027d0: 6973 204e 6f6e 6529 2e0a 2020 2020 2020  is None)..      
+000027e0: 2020 3a74 7970 6520 6d61 785f 7072 696f    :type max_prio
+000027f0: 7269 7479 5f66 6565 5f70 6572 5f67 6173  rity_fee_per_gas
+00002800: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0a  : Optional[int].
+00002810: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00002820: 2054 6865 2074 7261 6e73 6163 7469 6f6e   The transaction
+00002830: 2070 6172 616d 6574 6572 7320 6469 6374   parameters dict
+00002840: 696f 6e61 7279 2e0a 2020 2020 2020 2020  ionary..        
+00002850: 3a72 7479 7065 3a20 4469 6374 0a20 2020  :rtype: Dict.   
+00002860: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00002870: 2020 6966 206e 6f6e 6365 2069 7320 4e6f    if nonce is No
+00002880: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00002890: 6e6f 6e63 6520 3d20 7365 6c66 2e77 332e  nonce = self.w3.
+000028a0: 6574 682e 6765 745f 7472 616e 7361 6374  eth.get_transact
+000028b0: 696f 6e5f 636f 756e 7428 7365 6c66 2e77  ion_count(self.w
+000028c0: 616c 6c65 7429 0a0a 2020 2020 2020 2020  allet)..        
+000028d0: 7472 616e 7361 6374 696f 6e20 3d20 7b0a  transaction = {.
+000028e0: 2020 2020 2020 2020 2020 2020 2763 6861              'cha
+000028f0: 696e 4964 273a 2073 656c 662e 6368 6169  inId': self.chai
+00002900: 6e5f 6964 2c0a 2020 2020 2020 2020 2020  n_id,.          
+00002910: 2020 2767 6173 273a 2067 6173 2c0a 2020    'gas': gas,.  
+00002920: 2020 2020 2020 2020 2020 276d 6178 4665            'maxFe
+00002930: 6550 6572 4761 7327 3a20 6d61 785f 6665  ePerGas': max_fe
+00002940: 655f 7065 725f 6761 732c 0a20 2020 2020  e_per_gas,.     
+00002950: 2020 2020 2020 2027 6d61 7850 7269 6f72         'maxPrior
+00002960: 6974 7946 6565 5065 7247 6173 273a 206d  ityFeePerGas': m
+00002970: 6178 5f70 7269 6f72 6974 795f 6665 655f  ax_priority_fee_
+00002980: 7065 725f 6761 732c 0a20 2020 2020 2020  per_gas,.       
+00002990: 2020 2020 2027 6e6f 6e63 6527 3a20 6e6f       'nonce': no
+000029a0: 6e63 652c 0a20 2020 2020 2020 207d 0a0a  nce,.        }..
+000029b0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+000029c0: 6b65 793a 2076 616c 7565 2066 6f72 206b  key: value for k
+000029d0: 6579 2c20 7661 6c75 6520 696e 2074 7261  ey, value in tra
+000029e0: 6e73 6163 7469 6f6e 2e69 7465 6d73 2829  nsaction.items()
+000029f0: 2069 6620 7661 6c75 6520 6973 206e 6f74   if value is not
+00002a00: 204e 6f6e 657d 0a0a 2020 2020 6465 6620   None}..    def 
+00002a10: 5f77 6169 745f 666f 725f 7472 616e 7361  _wait_for_transa
+00002a20: 6374 696f 6e5f 7265 6365 6970 7428 7365  ction_receipt(se
+00002a30: 6c66 2c20 7472 616e 7361 6374 696f 6e3a  lf, transaction:
+00002a40: 2053 6967 6e65 6454 7261 6e73 6163 7469   SignedTransacti
+00002a50: 6f6e 2920 2d3e 2054 7261 6e73 6163 7469  on) -> Transacti
+00002a60: 6f6e 5265 6365 6970 743a 0a20 2020 2020  onReceipt:.     
+00002a70: 2020 2022 2222 5761 6974 2066 6f72 2074     """Wait for t
+00002a80: 6865 2074 7261 6e73 6163 7469 6f6e 2072  he transaction r
+00002a90: 6563 6569 7074 2061 6e64 2063 6865 636b  eceipt and check
+00002aa0: 2069 6620 7468 6520 7472 616e 7361 6374   if the transact
+00002ab0: 696f 6e20 7761 7320 7375 6363 6573 7366  ion was successf
+00002ac0: 756c 2e0a 0a20 2020 2020 2020 203a 7061  ul...        :pa
+00002ad0: 7261 6d20 7472 616e 7361 6374 696f 6e3a  ram transaction:
+00002ae0: 2054 6865 2073 6967 6e65 6420 7472 616e   The signed tran
+00002af0: 7361 6374 696f 6e20 6f62 6a65 6374 2e0a  saction object..
+00002b00: 2020 2020 2020 2020 3a74 7970 6520 7472          :type tr
+00002b10: 616e 7361 6374 696f 6e3a 2053 6967 6e65  ansaction: Signe
+00002b20: 6454 7261 6e73 6163 7469 6f6e 0a20 2020  dTransaction.   
+00002b30: 2020 2020 203a 7261 6973 6573 2045 7863       :raises Exc
+00002b40: 6570 7469 6f6e 3a20 4966 2074 6865 2074  eption: If the t
+00002b50: 7261 6e73 6163 7469 6f6e 2066 6169 6c73  ransaction fails
+00002b60: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00002b70: 2020 2020 2020 7265 7375 6c74 203d 2054        result = T
+00002b80: 7261 6e73 6163 7469 6f6e 5265 6365 6970  ransactionReceip
+00002b90: 742e 6672 6f6d 5f74 785f 7265 6365 6970  t.from_tx_receip
+00002ba0: 7428 0a20 2020 2020 2020 2020 2020 2074  t(.            t
+00002bb0: 785f 7265 6365 6970 743d 7365 6c66 2e77  x_receipt=self.w
+00002bc0: 332e 6574 682e 7761 6974 5f66 6f72 5f74  3.eth.wait_for_t
+00002bd0: 7261 6e73 6163 7469 6f6e 5f72 6563 6569  ransaction_recei
+00002be0: 7074 2874 7261 6e73 6163 7469 6f6e 2e68  pt(transaction.h
+00002bf0: 6173 6829 0a20 2020 2020 2020 2029 0a0a  ash).        )..
+00002c00: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
+00002c10: 742e 7374 6174 7573 203d 3d20 303a 0a20  t.status == 0:. 
+00002c20: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002c30: 2045 7863 6570 7469 6f6e 2866 2274 7261   Exception(f"tra
+00002c40: 6e73 6163 7469 6f6e 207b 7472 616e 7361  nsaction {transa
+00002c50: 6374 696f 6e2e 6861 7368 2e68 6578 2829  ction.hash.hex()
+00002c60: 7d20 6661 696c 6564 2229 0a0a 2020 2020  } failed")..    
+00002c70: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00002c80: 740a                                     t.
```

### Comparing `rubi-2.0.2b4/rubi/contracts/aid.py` & `rubi-2.0.3/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/contracts/erc20.py` & `rubi-2.0.3/rubi/contracts/erc20.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 import os
 from _decimal import Decimal
 from typing import Optional
-# from pkg_resources import resource_stream
-# import importlib.resources as resources
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 from web3.types import ABI
 
 from rubi.contracts.base_contract import BaseContract
+from rubi.contracts.types import TransactionReceipt
 from rubi.network import Network
 
 
 class ERC20(BaseContract):
     """this class represents a contract that implements the ERC20 standard. it is used to read the contract instance.
     if a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
 
@@ -174,15 +173,15 @@
         self,
         spender: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
         gas: int = 100000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Approves the spender to spend the amount of the erc20 token from the signer's wallet
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param amount: amount of the erc20 token to approve the spender to spend
         :type amount: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
@@ -192,16 +191,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
         approve = self.contract.functions.approve(spender, amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=approve,
             gas=gas,
             nonce=nonce,
@@ -214,15 +213,15 @@
         self,
         recipient: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
         gas: int = 100000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Transfers the amount of the erc20 token to the recipient
 
         :param recipient: address of the recipient
         :type recipient: ChecksumAddress
         :param amount: amount of the erc20 token to transfer
         :type amount: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce
@@ -231,16 +230,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
         transfer = self.contract.functions.transfer(recipient, amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=transfer,
             gas=gas,
             nonce=nonce,
@@ -254,15 +253,15 @@
         sender: ChecksumAddress,
         recipient: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
         gas: int = 100000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Transfers the amount of the erc20 token from the sender to the recipient
 
         :param sender: address of the sender
         :type sender: ChecksumAddress
         :param recipient: address of the recipient
         :type recipient: ChecksumAddress
         :param amount: amount of the erc20 token to transfer
@@ -274,16 +273,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
 
         transfer_from = self.contract.functions.transferFrom(sender, recipient, amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=transfer_from,
             gas=gas,
@@ -297,15 +296,15 @@
         self,
         spender: ChecksumAddress,
         added_value: int,
         nonce: Optional[int] = None,
         gas: int = 100000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Increases the allowance of the spender by the added_value
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param added_value: amount to increase the allowance by, in the integer representation of the erc20 token
         :type added_value: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
@@ -315,16 +314,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
         increase_allowance = self.contract.functions.increaseAllowance(spender, added_value)
 
         return self._default_transaction_handler(
             instantiated_contract_function=increase_allowance,
             gas=gas,
             nonce=nonce,
@@ -337,15 +336,15 @@
         self,
         spender: ChecksumAddress,
         subtracted_value: int,
         nonce: Optional[int] = None,
         gas: int = 100000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Decreases the allowance of the spender by the subtracted_value
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param subtracted_value: amount to decrease the allowance by, in the integer representation of the erc20 token
         :type subtracted_value: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
@@ -355,16 +354,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
         decrease_allowance = self.contract.functions.decreaseAllowance(spender, subtracted_value)
 
         return self._default_transaction_handler(
             instantiated_contract_function=decrease_allowance,
             gas=gas,
             nonce=nonce,
```

### Comparing `rubi-2.0.2b4/rubi/contracts/market.py` & `rubi-2.0.3/rubi/contracts/market.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, Tuple, List
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 
 from rubi.contracts.base_contract import BaseContract
+from rubi.contracts.types import TransactionReceipt
 from rubi.network import Network
 
 
 class RubiconMarket(BaseContract):
     """This class represents the RubiconMarket.sol contract and by default has read functionality.
     If a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
 
@@ -222,18 +223,18 @@
         buy_amt: int,
         buy_gem: ChecksumAddress,
         pos: int = 0,
         rounding: bool = True,
         owner: Optional[ChecksumAddress] = None,
         recipient: Optional[ChecksumAddress] = None,
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: int = 400000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Make a new offer to buy the buy_amt of the buy_gem token in exchange for the pay_amt of the pay_gem token
 
         :param pay_amt: the amount of the token being sold
         :type pay_amt: int
         :param pay_gem: the address of the token being sold
         :type pay_gem: ChecksumAddress
         :param buy_amt: the amount of the token being bought
@@ -258,16 +259,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
 
         if not self.signing_permissions:
             raise Exception(f"cannot write transaction without signing rights. "
                             f"re-instantiate {self.__class__} with a wallet and private key")
 
         owner = owner if owner is not None else self.wallet
@@ -287,15 +288,15 @@
     def cancel(
         self,
         id: int,
         nonce: Optional[int] = None,
         gas: int = 350000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Cancel an offer by offer id
 
         :param id: the id of the offer to cancel
         :type id: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
@@ -303,16 +304,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
 
         cancel = self.contract.functions.cancel(id)
 
         return self._default_transaction_handler(
             instantiated_contract_function=cancel,
             gas=gas,
@@ -328,15 +329,15 @@
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
         gas: int = 350000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Batch the placement of a set of offers in one transaction
 
         :param pay_amts: the amounts of the token being sold
         :type pay_amts: List[int]
         :param pay_gems: the addresses of the tokens being sold
         :type pay_gems: List[ChecksumAddress]
         :param buy_amts: the amounts of the token being bought
@@ -350,16 +351,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
         if not (len(pay_amts) == len(pay_gems) == len(buy_amts) == len(buy_gems)):
             raise Exception("mismatches lengths in pay_amts, pay_gems, buy_amts and buy_gems")
 
         batch_offer = self.contract.functions.batchOffer(pay_amts, pay_gems, buy_amts, buy_gems)
 
         return self._default_transaction_handler(
@@ -374,15 +375,15 @@
     def batch_cancel(
         self,
         ids: List[int],
         nonce: Optional[int] = None,
         gas: int = 350000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Cancel a set offer by offer id in a single transaction
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
         :type nonce: Optional[int]
@@ -390,16 +391,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
         cancels = self.contract.functions.cancel(ids)
 
         return self._default_transaction_handler(
             instantiated_contract_function=cancels,
             gas=gas,
             nonce=nonce,
@@ -416,15 +417,15 @@
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
         gas: int = 350000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Batch update a set of offers in a single transaction and return a list of new offer ids
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
         :param pay_amts: the amounts of the token being sold
         :type pay_amts: List[int]
         :param pay_gems: the addresses of the tokens being sold
@@ -440,16 +441,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
 
         batch_requote = self.contract.functions.batchRequote(ids, pay_amts, pay_gems, buy_amts, buy_gems)
 
         return self._default_transaction_handler(
             instantiated_contract_function=batch_requote,
             gas=gas,
@@ -465,15 +466,15 @@
         pay_amt: int,
         buy_gem: ChecksumAddress,
         min_fill_amount: int,
         nonce: Optional[int] = None,
         gas: int = 350000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Sell the pay_amt of the pay_gem token in exchange for buy_gem, on the condition that you receive at least the
         min_fill_amount of the buy_gem token
 
         :param pay_gem: the address of the tokens being sold
         :type pay_gem: ChecksumAddress
         :param pay_amt: the amount of the token being sold
         :type pay_amt: int
@@ -488,16 +489,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
         sell_all_amount = self.contract.functions.sellAllAmount(pay_gem, pay_amt, buy_gem, min_fill_amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=sell_all_amount,
             gas=gas,
             nonce=nonce,
@@ -512,15 +513,15 @@
         buy_amt: int,
         pay_gem: ChecksumAddress,
         max_fill_amount: int,
         nonce: Optional[int] = None,
         gas: int = 350000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Buy the buy_amt of the buy_gem token in exchange for pay_gem, on the condition that it does not exceed the
         max_fill_amount of the pay_gem token
 
         :param buy_gem: the address of the tokens being bought
         :type buy_gem: ChecksumAddress
         :param buy_amt: the amount of the token being bought
         :type buy_amt: int
@@ -535,16 +536,16 @@
         :type gas: int
         :param max_fee_per_gas: max fee that can be paid for gas, defaults to
             max_priority_fee (from chain) + (2 * base fee per gas of latest block) (optional, default is None)
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
-        :return: transaction hash
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
         buy_all_amount = self.contract.functions.sellAllAmount(buy_gem, buy_amt, pay_gem, max_fill_amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=buy_all_amount,
             gas=gas,
             nonce=nonce,
```

### Comparing `rubi-2.0.2b4/rubi/contracts/router.py` & `rubi-2.0.3/rubi/contracts/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, Tuple, List
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 
 from rubi.contracts.base_contract import BaseContract
+from rubi.contracts.types import TransactionReceipt
 from rubi.network import Network
 
 
 class RubiconRouter(BaseContract):
     """This class represents the RubiconRouter.sol contract and by default has read functionality.
     If a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
 
@@ -238,15 +239,15 @@
         pay_amts: List[int],
         buy_amts_min: List[int],
         to: ChecksumAddress,
         nonce: Optional[int] = None,
         gas: int = 350000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Perform a multiple swaps for the specified payment amounts using the specified routes. Reverts with an
         exception if any of the swaps cannot achieve the buy_amt_min along the specified route.
 
         :param routes: The list of routes, where each route is a list of addresses representing the swap path.
         :type routes: List[List[ChecksumAddress]]
         :param pay_amts: The list of payment amounts for each swap.
         :type pay_amts: List[int]
@@ -261,16 +262,16 @@
         :type gas: int
         :param max_fee_per_gas: Max fee that can be paid for gas. Defaults to max_priority_fee (from chain)
             + (2 * base fee per gas of latest block) (optional, default is None).
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: Max priority fee that can be paid for gas. Defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None).
         :type max_priority_fee_per_gas: Optional[int]
-        :return: Transaction hash.
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
 
         multiswap = self.contract.functions.multiswap(routes, pay_amts, buy_amts_min, to)
 
         return self._default_transaction_handler(
             instantiated_contract_function=multiswap,
             gas=gas,
@@ -286,15 +287,15 @@
         buy_amt_min: int,
         route: List[ChecksumAddress],
         to: ChecksumAddress,
         nonce: Optional[int] = None,
         gas: int = 350000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
-    ) -> str:
+    ) -> TransactionReceipt:
         """Perform a swap operation with the specified payment amount using the specified route and paying out to the
         recipient. Reverts if the swap does not result in the buy_min_amount.
 
         :param pay_amt: The payment amount.
         :type pay_amt: int
         :param buy_amt_min: The minimum buy amount.
         :type buy_amt_min: int
@@ -309,16 +310,16 @@
         :type gas: int
         :param max_fee_per_gas: Max fee that can be paid for gas. Defaults to max_priority_fee (from chain)
             + (2 * base fee per gas of latest block) (optional, default is None).
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: Max priority fee that can be paid for gas. Defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None).
         :type max_priority_fee_per_gas: Optional[int]
-        :return: Transaction hash.
-        :rtype: str
+        :return: An object representing the transaction receipt
+        :rtype: TransactionReceipt
         """
 
         swap = self.contract.functions.swap(pay_amt, buy_amt_min, route, to)
 
         return self._default_transaction_handler(
             instantiated_contract_function=swap,
             gas=gas,
```

### Comparing `rubi-2.0.2b4/rubi/contracts/types/events.py` & `rubi-2.0.3/rubi/contracts/types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/data.py` & `rubi-2.0.3/rubi/data/data.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/processing/README.md` & `rubi-2.0.3/rubi/data/processing/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/processing/aid.py` & `rubi-2.0.3/rubi/data/processing/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/processing/helper/processing.py` & `rubi-2.0.3/rubi/data/processing/helper/processing.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/processing/user.py` & `rubi-2.0.3/rubi/data/processing/user.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/sources/aid.py` & `rubi-2.0.3/rubi/data/sources/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/sources/helper/README.md` & `rubi-2.0.3/rubi/data/sources/helper/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/sources/helper/gas.py` & `rubi-2.0.3/rubi/data/sources/helper/gas.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/sources/helper/price.py` & `rubi-2.0.3/rubi/data/sources/helper/price.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/sources/helper/rolodex.py` & `rubi-2.0.3/rubi/data/sources/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/data/sources/market.py` & `rubi-2.0.3/rubi/data/sources/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/rubi/network/network.py` & `rubi-2.0.3/rubi/network/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import json
 import os
 from enum import Enum
 from typing import Optional
-# from pkg_resources import resource_exists, resource_stream
-# import importlib.resources as resources
-
 
 import yaml
 from eth_typing import ChecksumAddress
 from web3 import Web3
 
 
 class NetworkId(Enum):
@@ -112,24 +109,24 @@
         :type custom_token_addresses_file: Optional[str]
         :return: A Network instance based on the network configuration.
         :rtype: Network
         :raises Exception: If no network configuration file is found for the specified network name.
         """
         w3 = Web3(Web3.HTTPProvider(http_node_url))
 
-        name_name = NetworkId(w3.eth.chain_id).name.lower()
+        network_name = NetworkId(w3.eth.chain_id).name.lower()
 
         try:
-            path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/{name_name}"
+            path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/{network_name}"
 
             with open(f"{path}/network.yaml") as f:
                 network_data = yaml.safe_load(f)
                 return cls(path=path, w3=w3, custom_token_addresses_file=custom_token_addresses_file, **network_data)
         except FileNotFoundError:
-            raise Exception(f"no network config found for {name_name}, there should be a corresponding folder in "
+            raise Exception(f"no network config found for {network_name}, there should be a corresponding folder in "
                             f"the network_config directory")
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.0.2b4/rubi/types/__pycache__/pair.cpython-310.pyc` & `rubi-2.0.3/rubi/types/pair.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,170 @@
-00000000: 6f0d 0d0a 0000 0000 9cea 7864 930a 0000  o.........xd....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
-00000050: 8302 5a04 4700 6405 6406 8400 6406 6505  ..Z.G.d.d...d.e.
-00000060: 8303 5a06 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
-00000070: 01da 0744 6563 696d 616c 2901 da05 4552  ...Decimal)...ER
-00000080: 4332 3063 0000 0000 0000 0000 0000 0000  C20c............
-00000090: 0000 0000 0a00 0000 4000 0000 7352 0000  ........@...sR..
-000000a0: 0065 005a 0164 005a 0264 015a 0364 0265  .e.Z.d.Z.d.Z.d.e
-000000b0: 0464 0365 0564 0465 0564 0565 0664 0665  .d.e.d.e.d.e.d.e
-000000c0: 0666 0a64 0764 0884 045a 0764 0965 0664  .f.d.d...Z.d.e.d
-000000d0: 0a64 0b66 0464 0c64 0d84 045a 0864 0e65  .d.f.d.d...Z.d.e
-000000e0: 0664 0a64 0b66 0464 0f64 1084 045a 0964  .d.d.f.d.d...Z.d
-000000f0: 0b53 0029 11da 0450 6169 7261 9b02 0000  .S.)...Paira....
-00000100: 436c 6173 7320 7265 7072 6573 656e 7469  Class representi
-00000110: 6e67 2061 2074 7261 6469 6e67 2061 7373  ng a trading ass
-00000120: 6574 2070 6169 722c 2065 2e67 2e20 5745  et pair, e.g. WE
-00000130: 5448 2f55 5344 4320 776f 756c 6420 6861  TH/USDC would ha
-00000140: 7665 2057 4554 4820 6173 2074 6865 2062  ve WETH as the b
-00000150: 6173 6520 6173 7365 7420 616e 6420 5553  ase asset and US
-00000160: 4443 2061 7320 7468 6520 7175 6f74 650a  DC as the quote.
-00000170: 2020 2020 6173 7365 742e 0a0a 2020 2020      asset...    
-00000180: 3a70 6172 616d 206e 616d 653a 2054 6865  :param name: The
-00000190: 206e 616d 6520 6f66 2074 6865 2070 6169   name of the pai
-000001a0: 722c 2065 2e67 2e20 5745 5448 2f55 5344  r, e.g. WETH/USD
-000001b0: 432e 0a20 2020 203a 7479 7065 206e 616d  C..    :type nam
-000001c0: 653a 2073 7472 0a20 2020 203a 7061 7261  e: str.    :para
-000001d0: 6d20 6261 7365 5f61 7373 6574 3a20 4261  m base_asset: Ba
-000001e0: 7365 2061 7373 6574 206f 6620 7468 6520  se asset of the 
-000001f0: 7061 6972 2e0a 2020 2020 3a74 7970 6520  pair..    :type 
-00000200: 6261 7365 5f61 7373 6574 3a20 4552 4332  base_asset: ERC2
-00000210: 300a 2020 2020 3a70 6172 616d 2071 756f  0.    :param quo
-00000220: 7465 5f61 7373 6574 3a20 5175 6f74 6520  te_asset: Quote 
-00000230: 6173 7365 7420 6f66 2074 6865 2070 6169  asset of the pai
-00000240: 722e 0a20 2020 203a 7479 7065 2071 756f  r..    :type quo
-00000250: 7465 5f61 7373 6574 3a20 4552 4332 300a  te_asset: ERC20.
-00000260: 2020 2020 3a70 6172 616d 2063 7572 7265      :param curre
-00000270: 6e74 5f62 6173 655f 6173 7365 745f 616c  nt_base_asset_al
-00000280: 6c6f 7761 6e63 653a 2054 6865 2062 6173  lowance: The bas
-00000290: 6520 6173 7365 7420 7370 656e 6469 6e67  e asset spending
-000002a0: 2061 6c6c 6f77 616e 6365 206f 6620 7468   allowance of th
-000002b0: 6520 5275 6269 636f 6e4d 6172 6b65 7420  e RubiconMarket 
-000002c0: 636f 6e74 7261 6374 2e0a 2020 2020 3a74  contract..    :t
-000002d0: 7970 6520 6375 7272 656e 745f 6261 7365  ype current_base
-000002e0: 5f61 7373 6574 5f61 6c6c 6f77 616e 6365  _asset_allowance
-000002f0: 3a20 4465 6369 6d61 6c0a 2020 2020 3a70  : Decimal.    :p
-00000300: 6172 616d 2063 7572 7265 6e74 5f71 756f  aram current_quo
-00000310: 7465 5f61 7373 6574 5f61 6c6c 6f77 616e  te_asset_allowan
-00000320: 6365 3a20 5468 6520 7175 6f74 6520 6173  ce: The quote as
-00000330: 7365 7420 7370 656e 6469 6e67 2061 6c6c  set spending all
-00000340: 6f77 616e 6365 206f 6620 7468 6520 5275  owance of the Ru
-00000350: 6269 636f 6e4d 6172 6b65 7420 636f 6e74  biconMarket cont
-00000360: 7261 6374 2e0a 2020 2020 3a74 7970 6520  ract..    :type 
-00000370: 6375 7272 656e 745f 7175 6f74 655f 6173  current_quote_as
-00000380: 7365 745f 616c 6c6f 7761 6e63 653a 2044  set_allowance: D
-00000390: 6563 696d 616c 0a20 2020 20da 046e 616d  ecimal.    ..nam
-000003a0: 65da 0a62 6173 655f 6173 7365 74da 0b71  e..base_asset..q
-000003b0: 756f 7465 5f61 7373 6574 da1c 6375 7272  uote_asset..curr
-000003c0: 656e 745f 6261 7365 5f61 7373 6574 5f61  ent_base_asset_a
-000003d0: 6c6c 6f77 616e 6365 da1d 6375 7272 656e  llowance..curren
-000003e0: 745f 7175 6f74 655f 6173 7365 745f 616c  t_quote_asset_al
-000003f0: 6c6f 7761 6e63 6563 0600 0000 0000 0000  lowancec........
-00000400: 0000 0000 0600 0000 0400 0000 4300 0000  ............C...
-00000410: 736e 0000 007c 017c 005f 007c 027c 005f  sn...|.|._.|.|._
-00000420: 017c 037c 005f 027c 026a 036a 0464 0164  .|.|._.|.j.j.d.d
-00000430: 0167 027c 006a 026a 057c 006a 016a 0567  .g.|.j.j.|.j.j.g
-00000440: 0264 028d 02a0 06a1 007c 005f 077c 026a  .d.......|._.|.j
-00000450: 036a 0464 0164 0167 027c 006a 016a 057c  .j.d.d.g.|.j.j.|
-00000460: 006a 026a 0567 0264 028d 02a0 06a1 007c  .j.j.g.d.......|
-00000470: 005f 087c 047c 005f 097c 057c 005f 0a64  ._.|.|._.|.|._.d
-00000480: 0053 0029 034e da07 6164 6472 6573 7329  .S.).N..address)
-00000490: 02da 0961 6269 5f74 7970 6573 da06 7661  ...abi_types..va
-000004a0: 6c75 6573 290b 7205 0000 0072 0600 0000  lues).r....r....
-000004b0: 7207 0000 00da 0277 33da 0f73 6f6c 6964  r......w3..solid
-000004c0: 6974 795f 6b65 6363 616b 720a 0000 00da  ity_keccakr.....
-000004d0: 0368 6578 da0e 6269 645f 6964 656e 7469  .hex..bid_identi
-000004e0: 6669 6572 da0e 6173 6b5f 6964 656e 7469  fier..ask_identi
-000004f0: 6669 6572 7208 0000 0072 0900 0000 2906  fierr....r....).
-00000500: da04 7365 6c66 7205 0000 0072 0600 0000  ..selfr....r....
-00000510: 7207 0000 0072 0800 0000 7209 0000 00a9  r....r....r.....
-00000520: 0072 1300 0000 fa3c 2f55 7365 7273 2f64  .r.....</Users/d
-00000530: 656e 7665 722f 446f 6375 6d65 6e74 732f  enver/Documents/
-00000540: 6f70 656e 2f72 7562 692d 7079 2f72 7562  open/rubi-py/rub
-00000550: 692f 7275 6269 2f74 7970 6573 2f70 6169  i/rubi/types/pai
-00000560: 722e 7079 da08 5f5f 696e 6974 5f5f 1600  r.py..__init__..
-00000570: 0000 7322 0000 0006 0806 0206 0106 0206  ..s"............
-00000580: 010e 0104 fe04 0304 fd06 0406 010e 0104  ................
-00000590: fe04 0304 fd06 070a 017a 0d50 6169 722e  .........z.Pair.
-000005a0: 5f5f 696e 6974 5f5f da18 6e65 775f 6261  __init__..new_ba
-000005b0: 7365 5f61 7373 6574 5f61 6c6c 6f77 616e  se_asset_allowan
-000005c0: 6365 da06 7265 7475 726e 4e63 0200 0000  ce..returnNc....
-000005d0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-000005e0: 4300 0000 f30a 0000 007c 017c 005f 0064  C........|.|._.d
-000005f0: 0153 0029 027a bb55 7064 6174 6520 7468  .S.).z.Update th
-00000600: 6520 6375 7272 656e 7420 6261 7365 2061  e current base a
-00000610: 7373 6574 2061 6c6c 6f77 616e 6365 2e0a  sset allowance..
-00000620: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000630: 6e65 775f 6261 7365 5f61 7373 6574 5f61  new_base_asset_a
-00000640: 6c6c 6f77 616e 6365 3a20 4e65 7720 6261  llowance: New ba
-00000650: 7365 2061 7373 6574 2061 6c6c 6f77 616e  se asset allowan
-00000660: 6365 2e0a 2020 2020 2020 2020 3a74 7970  ce..        :typ
-00000670: 6520 6e65 775f 6261 7365 5f61 7373 6574  e new_base_asset
-00000680: 5f61 6c6c 6f77 616e 6365 3a20 4465 6369  _allowance: Deci
-00000690: 6d61 6c0a 2020 2020 2020 2020 3a72 6574  mal.        :ret
-000006a0: 7572 6e3a 204e 6f6e 650a 2020 2020 2020  urn: None.      
-000006b0: 2020 4e29 0172 0800 0000 2902 7212 0000    N).r....).r...
-000006c0: 0072 1600 0000 7213 0000 0072 1300 0000  .r....r....r....
-000006d0: 7214 0000 00da 1b75 7064 6174 655f 6261  r......update_ba
-000006e0: 7365 5f61 7373 6574 5f61 6c6c 6f77 616e  se_asset_allowan
-000006f0: 6365 3100 0000 f302 0000 000a 077a 2050  ce1..........z P
-00000700: 6169 722e 7570 6461 7465 5f62 6173 655f  air.update_base_
-00000710: 6173 7365 745f 616c 6c6f 7761 6e63 65da  asset_allowance.
-00000720: 196e 6577 5f71 756f 7465 5f61 7373 6574  .new_quote_asset
-00000730: 5f61 6c6c 6f77 616e 6365 6302 0000 0000  _allowancec.....
-00000740: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000750: 0000 0072 1800 0000 2902 7abf 5570 6461  ...r....).z.Upda
-00000760: 7465 2074 6865 2063 7572 7265 6e74 2071  te the current q
-00000770: 756f 7465 2061 7373 6574 2061 6c6c 6f77  uote asset allow
-00000780: 616e 6365 2e0a 0a20 2020 2020 2020 203a  ance...        :
-00000790: 7061 7261 6d20 6e65 775f 7175 6f74 655f  param new_quote_
-000007a0: 6173 7365 745f 616c 6c6f 7761 6e63 653a  asset_allowance:
-000007b0: 204e 6577 2071 756f 7465 2061 7373 6574   New quote asset
-000007c0: 2061 6c6c 6f77 616e 6365 2e0a 2020 2020   allowance..    
-000007d0: 2020 2020 3a74 7970 6520 6e65 775f 7175      :type new_qu
-000007e0: 6f74 655f 6173 7365 745f 616c 6c6f 7761  ote_asset_allowa
-000007f0: 6e63 653a 2044 6563 696d 616c 0a20 2020  nce: Decimal.   
-00000800: 2020 2020 203a 7265 7475 726e 3a20 4e6f       :return: No
-00000810: 6e65 0a20 2020 2020 2020 204e 2901 7209  ne.        N).r.
-00000820: 0000 0029 0272 1200 0000 721b 0000 0072  ...).r....r....r
-00000830: 1300 0000 7213 0000 0072 1400 0000 da1c  ....r....r......
-00000840: 7570 6461 7465 5f71 756f 7465 5f61 7373  update_quote_ass
-00000850: 6574 5f61 6c6c 6f77 616e 6365 3a00 0000  et_allowance:...
-00000860: 721a 0000 007a 2150 6169 722e 7570 6461  r....z!Pair.upda
-00000870: 7465 5f71 756f 7465 5f61 7373 6574 5f61  te_quote_asset_a
-00000880: 6c6c 6f77 616e 6365 290a da08 5f5f 6e61  llowance)...__na
-00000890: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000008a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-000008b0: 5f5f 646f 635f 5fda 0373 7472 7203 0000  __doc__..strr...
-000008c0: 0072 0200 0000 7215 0000 0072 1900 0000  .r....r....r....
-000008d0: 721c 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-000008e0: 1300 0000 7214 0000 0072 0400 0000 0600  ....r....r......
-000008f0: 0000 731e 0000 0008 0004 0102 0f02 0202  ..s.............
-00000900: fe02 0302 fd02 0402 fc02 0502 fb02 060a  ................
-00000910: fa12 1b16 0972 0400 0000 6300 0000 0000  .....r....c.....
-00000920: 0000 0000 0000 0000 0000 0004 0000 0000  ................
-00000930: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
-00000940: 6401 5a03 6402 6504 6602 8700 6601 6403  d.Z.d.e.f...f.d.
-00000950: 6404 840c 5a05 8700 0400 5a06 5300 2905  d...Z.....Z.S.).
-00000960: da19 5061 6972 446f 6573 4e6f 7445 7869  ..PairDoesNotExi
-00000970: 7374 4578 6365 7074 696f 6e7a 6b45 7863  stExceptionzkExc
-00000980: 6570 7469 6f6e 2072 6169 7365 6420 7768  eption raised wh
-00000990: 656e 2061 6e20 6173 7365 7420 7061 6972  en an asset pair
-000009a0: 2064 6f65 7320 6e6f 7420 6578 6973 742e   does not exist.
-000009b0: 0a0a 2020 2020 3a70 6172 616d 206d 7367  ..    :param msg
-000009c0: 3a20 4572 726f 7220 6d65 7373 6167 652e  : Error message.
-000009d0: 0a20 2020 203a 7479 7065 206d 7367 3a20  .    :type msg: 
-000009e0: 7374 720a 2020 2020 da03 6d73 6763 0200  str.    ..msgc..
-000009f0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000a00: 0000 0300 0000 7310 0000 0074 0083 00a0  ......s....t....
-00000a10: 017c 01a1 0101 0064 0053 0029 014e 2902  .|.....d.S.).N).
-00000a20: da05 7375 7065 7272 1500 0000 2902 7212  ..superr....).r.
-00000a30: 0000 0072 2300 0000 a901 da09 5f5f 636c  ...r#.......__cl
-00000a40: 6173 735f 5f72 1300 0000 7214 0000 0072  ass__r....r....r
-00000a50: 1500 0000 4b00 0000 7302 0000 0010 017a  ....K...s......z
-00000a60: 2250 6169 7244 6f65 734e 6f74 4578 6973  "PairDoesNotExis
-00000a70: 7445 7863 6570 7469 6f6e 2e5f 5f69 6e69  tException.__ini
-00000a80: 745f 5f29 0772 1d00 0000 721e 0000 0072  t__).r....r....r
-00000a90: 1f00 0000 7220 0000 0072 2100 0000 7215  ....r ...r!...r.
-00000aa0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000ab0: 5f5f 7213 0000 0072 1300 0000 7225 0000  __r....r....r%..
-00000ac0: 0072 1400 0000 7222 0000 0044 0000 0073  .r....r"...D...s
-00000ad0: 0600 0000 0800 0401 1a06 7222 0000 004e  ..........r"...N
-00000ae0: 2907 da08 5f64 6563 696d 616c 7202 0000  )..._decimalr...
-00000af0: 00da 0472 7562 6972 0300 0000 7204 0000  ...rubir....r...
-00000b00: 00da 0945 7863 6570 7469 6f6e 7222 0000  ...Exceptionr"..
-00000b10: 0072 1300 0000 7213 0000 0072 1300 0000  .r....r....r....
-00000b20: 7214 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000b30: 0000 0073 0800 0000 0c00 0c02 0e03 143e  ...s...........>
+00000000: 6672 6f6d 205f 6465 6369 6d61 6c20 696d  from _decimal im
+00000010: 706f 7274 2044 6563 696d 616c 0a0a 6672  port Decimal..fr
+00000020: 6f6d 2072 7562 6920 696d 706f 7274 2045  om rubi import E
+00000030: 5243 3230 0a0a 0a63 6c61 7373 2050 6169  RC20...class Pai
+00000040: 723a 0a20 2020 2022 2222 436c 6173 7320  r:.    """Class 
+00000050: 7265 7072 6573 656e 7469 6e67 2061 2074  representing a t
+00000060: 7261 6469 6e67 2061 7373 6574 2070 6169  rading asset pai
+00000070: 722c 2065 2e67 2e20 5745 5448 2f55 5344  r, e.g. WETH/USD
+00000080: 4320 776f 756c 6420 6861 7665 2057 4554  C would have WET
+00000090: 4820 6173 2074 6865 2062 6173 6520 6173  H as the base as
+000000a0: 7365 7420 616e 6420 5553 4443 2061 7320  set and USDC as 
+000000b0: 7468 6520 7175 6f74 650a 2020 2020 6173  the quote.    as
+000000c0: 7365 742e 0a0a 2020 2020 3a70 6172 616d  set...    :param
+000000d0: 206e 616d 653a 2054 6865 206e 616d 6520   name: The name 
+000000e0: 6f66 2074 6865 2070 6169 722c 2065 2e67  of the pair, e.g
+000000f0: 2e20 5745 5448 2f55 5344 432e 0a20 2020  . WETH/USDC..   
+00000100: 203a 7479 7065 206e 616d 653a 2073 7472   :type name: str
+00000110: 0a20 2020 203a 7061 7261 6d20 6261 7365  .    :param base
+00000120: 5f61 7373 6574 3a20 4261 7365 2061 7373  _asset: Base ass
+00000130: 6574 206f 6620 7468 6520 7061 6972 2e0a  et of the pair..
+00000140: 2020 2020 3a74 7970 6520 6261 7365 5f61      :type base_a
+00000150: 7373 6574 3a20 4552 4332 300a 2020 2020  sset: ERC20.    
+00000160: 3a70 6172 616d 2071 756f 7465 5f61 7373  :param quote_ass
+00000170: 6574 3a20 5175 6f74 6520 6173 7365 7420  et: Quote asset 
+00000180: 6f66 2074 6865 2070 6169 722e 0a20 2020  of the pair..   
+00000190: 203a 7479 7065 2071 756f 7465 5f61 7373   :type quote_ass
+000001a0: 6574 3a20 4552 4332 300a 2020 2020 3a70  et: ERC20.    :p
+000001b0: 6172 616d 2063 7572 7265 6e74 5f62 6173  aram current_bas
+000001c0: 655f 6173 7365 745f 616c 6c6f 7761 6e63  e_asset_allowanc
+000001d0: 653a 2054 6865 2062 6173 6520 6173 7365  e: The base asse
+000001e0: 7420 7370 656e 6469 6e67 2061 6c6c 6f77  t spending allow
+000001f0: 616e 6365 206f 6620 7468 6520 5275 6269  ance of the Rubi
+00000200: 636f 6e4d 6172 6b65 7420 636f 6e74 7261  conMarket contra
+00000210: 6374 2e0a 2020 2020 3a74 7970 6520 6375  ct..    :type cu
+00000220: 7272 656e 745f 6261 7365 5f61 7373 6574  rrent_base_asset
+00000230: 5f61 6c6c 6f77 616e 6365 3a20 4465 6369  _allowance: Deci
+00000240: 6d61 6c0a 2020 2020 3a70 6172 616d 2063  mal.    :param c
+00000250: 7572 7265 6e74 5f71 756f 7465 5f61 7373  urrent_quote_ass
+00000260: 6574 5f61 6c6c 6f77 616e 6365 3a20 5468  et_allowance: Th
+00000270: 6520 7175 6f74 6520 6173 7365 7420 7370  e quote asset sp
+00000280: 656e 6469 6e67 2061 6c6c 6f77 616e 6365  ending allowance
+00000290: 206f 6620 7468 6520 5275 6269 636f 6e4d   of the RubiconM
+000002a0: 6172 6b65 7420 636f 6e74 7261 6374 2e0a  arket contract..
+000002b0: 2020 2020 3a74 7970 6520 6375 7272 656e      :type curren
+000002c0: 745f 7175 6f74 655f 6173 7365 745f 616c  t_quote_asset_al
+000002d0: 6c6f 7761 6e63 653a 2044 6563 696d 616c  lowance: Decimal
+000002e0: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
+000002f0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00000300: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00000310: 2020 6e61 6d65 3a20 7374 722c 0a20 2020    name: str,.   
+00000320: 2020 2020 2062 6173 655f 6173 7365 743a       base_asset:
+00000330: 2045 5243 3230 2c0a 2020 2020 2020 2020   ERC20,.        
+00000340: 7175 6f74 655f 6173 7365 743a 2045 5243  quote_asset: ERC
+00000350: 3230 2c0a 2020 2020 2020 2020 6375 7272  20,.        curr
+00000360: 656e 745f 6261 7365 5f61 7373 6574 5f61  ent_base_asset_a
+00000370: 6c6c 6f77 616e 6365 3a20 4465 6369 6d61  llowance: Decima
+00000380: 6c2c 0a20 2020 2020 2020 2063 7572 7265  l,.        curre
+00000390: 6e74 5f71 756f 7465 5f61 7373 6574 5f61  nt_quote_asset_a
+000003a0: 6c6c 6f77 616e 6365 3a20 4465 6369 6d61  llowance: Decima
+000003b0: 6c0a 2020 2020 293a 0a20 2020 2020 2020  l.    ):.       
+000003c0: 2073 656c 662e 6e61 6d65 203d 206e 616d   self.name = nam
+000003d0: 650a 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+000003e0: 6261 7365 5f61 7373 6574 3a20 4552 4332  base_asset: ERC2
+000003f0: 3020 3d20 6261 7365 5f61 7373 6574 0a20  0 = base_asset. 
+00000400: 2020 2020 2020 2073 656c 662e 7175 6f74         self.quot
+00000410: 655f 6173 7365 743a 2045 5243 3230 203d  e_asset: ERC20 =
+00000420: 2071 756f 7465 5f61 7373 6574 0a0a 2020   quote_asset..  
+00000430: 2020 2020 2020 7365 6c66 2e62 6964 5f69        self.bid_i
+00000440: 6465 6e74 6966 6965 723a 2073 7472 203d  dentifier: str =
+00000450: 2062 6173 655f 6173 7365 742e 7733 2e73   base_asset.w3.s
+00000460: 6f6c 6964 6974 795f 6b65 6363 616b 280a  olidity_keccak(.
+00000470: 2020 2020 2020 2020 2020 2020 6162 695f              abi_
+00000480: 7479 7065 733d 5b22 6164 6472 6573 7322  types=["address"
+00000490: 2c20 2261 6464 7265 7373 225d 2c0a 2020  , "address"],.  
+000004a0: 2020 2020 2020 2020 2020 7661 6c75 6573            values
+000004b0: 3d5b 7365 6c66 2e71 756f 7465 5f61 7373  =[self.quote_ass
+000004c0: 6574 2e61 6464 7265 7373 2c20 7365 6c66  et.address, self
+000004d0: 2e62 6173 655f 6173 7365 742e 6164 6472  .base_asset.addr
+000004e0: 6573 735d 0a20 2020 2020 2020 2029 2e68  ess].        ).h
+000004f0: 6578 2829 0a20 2020 2020 2020 2073 656c  ex().        sel
+00000500: 662e 6173 6b5f 6964 656e 7469 6669 6572  f.ask_identifier
+00000510: 3a20 7374 7220 3d20 6261 7365 5f61 7373  : str = base_ass
+00000520: 6574 2e77 332e 736f 6c69 6469 7479 5f6b  et.w3.solidity_k
+00000530: 6563 6361 6b28 0a20 2020 2020 2020 2020  eccak(.         
+00000540: 2020 2061 6269 5f74 7970 6573 3d5b 2261     abi_types=["a
+00000550: 6464 7265 7373 222c 2022 6164 6472 6573  ddress", "addres
+00000560: 7322 5d2c 0a20 2020 2020 2020 2020 2020  s"],.           
+00000570: 2076 616c 7565 733d 5b73 656c 662e 6261   values=[self.ba
+00000580: 7365 5f61 7373 6574 2e61 6464 7265 7373  se_asset.address
+00000590: 2c20 7365 6c66 2e71 756f 7465 5f61 7373  , self.quote_ass
+000005a0: 6574 2e61 6464 7265 7373 5d0a 2020 2020  et.address].    
+000005b0: 2020 2020 292e 6865 7828 290a 0a20 2020      ).hex()..   
+000005c0: 2020 2020 2023 2054 4f44 4f3a 2074 6869       # TODO: thi
+000005d0: 6e6b 2061 626f 7574 2073 7472 7563 7475  nk about structu
+000005e0: 7265 206f 6620 616c 6c6f 7761 6e63 6573  re of allowances
+000005f0: 206f 6e20 7468 6973 2063 6c61 7373 2e20   on this class. 
+00000600: 4375 7272 656e 746c 7920 7468 6973 206f  Currently this o
+00000610: 6e6c 7920 6361 7465 7273 2066 6f72 2074  nly caters for t
+00000620: 6865 2052 7562 6963 6f6e 4d61 726b 6574  he RubiconMarket
+00000630: 0a20 2020 2020 2020 2023 2020 636f 6e74  .        #  cont
+00000640: 7261 6374 2e0a 2020 2020 2020 2020 7365  ract..        se
+00000650: 6c66 2e63 7572 7265 6e74 5f62 6173 655f  lf.current_base_
+00000660: 6173 7365 745f 616c 6c6f 7761 6e63 6520  asset_allowance 
+00000670: 3d20 6375 7272 656e 745f 6261 7365 5f61  = current_base_a
+00000680: 7373 6574 5f61 6c6c 6f77 616e 6365 0a20  sset_allowance. 
+00000690: 2020 2020 2020 2073 656c 662e 6375 7272         self.curr
+000006a0: 656e 745f 7175 6f74 655f 6173 7365 745f  ent_quote_asset_
+000006b0: 616c 6c6f 7761 6e63 6520 3d20 6375 7272  allowance = curr
+000006c0: 656e 745f 7175 6f74 655f 6173 7365 745f  ent_quote_asset_
+000006d0: 616c 6c6f 7761 6e63 650a 0a20 2020 2064  allowance..    d
+000006e0: 6566 2075 7064 6174 655f 6261 7365 5f61  ef update_base_a
+000006f0: 7373 6574 5f61 6c6c 6f77 616e 6365 2873  sset_allowance(s
+00000700: 656c 662c 206e 6577 5f62 6173 655f 6173  elf, new_base_as
+00000710: 7365 745f 616c 6c6f 7761 6e63 653a 2044  set_allowance: D
+00000720: 6563 696d 616c 2920 2d3e 204e 6f6e 653a  ecimal) -> None:
+00000730: 0a20 2020 2020 2020 2022 2222 5570 6461  .        """Upda
+00000740: 7465 2074 6865 2063 7572 7265 6e74 2062  te the current b
+00000750: 6173 6520 6173 7365 7420 616c 6c6f 7761  ase asset allowa
+00000760: 6e63 652e 0a0a 2020 2020 2020 2020 3a70  nce...        :p
+00000770: 6172 616d 206e 6577 5f62 6173 655f 6173  aram new_base_as
+00000780: 7365 745f 616c 6c6f 7761 6e63 653a 204e  set_allowance: N
+00000790: 6577 2062 6173 6520 6173 7365 7420 616c  ew base asset al
+000007a0: 6c6f 7761 6e63 652e 0a20 2020 2020 2020  lowance..       
+000007b0: 203a 7479 7065 206e 6577 5f62 6173 655f   :type new_base_
+000007c0: 6173 7365 745f 616c 6c6f 7761 6e63 653a  asset_allowance:
+000007d0: 2044 6563 696d 616c 0a20 2020 2020 2020   Decimal.       
+000007e0: 203a 7265 7475 726e 3a20 4e6f 6e65 0a20   :return: None. 
+000007f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00000800: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
+00000810: 6261 7365 5f61 7373 6574 5f61 6c6c 6f77  base_asset_allow
+00000820: 616e 6365 203d 206e 6577 5f62 6173 655f  ance = new_base_
+00000830: 6173 7365 745f 616c 6c6f 7761 6e63 650a  asset_allowance.
+00000840: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
+00000850: 7175 6f74 655f 6173 7365 745f 616c 6c6f  quote_asset_allo
+00000860: 7761 6e63 6528 7365 6c66 2c20 6e65 775f  wance(self, new_
+00000870: 7175 6f74 655f 6173 7365 745f 616c 6c6f  quote_asset_allo
+00000880: 7761 6e63 653a 2044 6563 696d 616c 2920  wance: Decimal) 
+00000890: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000008a0: 2022 2222 5570 6461 7465 2074 6865 2063   """Update the c
+000008b0: 7572 7265 6e74 2071 756f 7465 2061 7373  urrent quote ass
+000008c0: 6574 2061 6c6c 6f77 616e 6365 2e0a 0a20  et allowance... 
+000008d0: 2020 2020 2020 203a 7061 7261 6d20 6e65         :param ne
+000008e0: 775f 7175 6f74 655f 6173 7365 745f 616c  w_quote_asset_al
+000008f0: 6c6f 7761 6e63 653a 204e 6577 2071 756f  lowance: New quo
+00000900: 7465 2061 7373 6574 2061 6c6c 6f77 616e  te asset allowan
+00000910: 6365 2e0a 2020 2020 2020 2020 3a74 7970  ce..        :typ
+00000920: 6520 6e65 775f 7175 6f74 655f 6173 7365  e new_quote_asse
+00000930: 745f 616c 6c6f 7761 6e63 653a 2044 6563  t_allowance: Dec
+00000940: 696d 616c 0a20 2020 2020 2020 203a 7265  imal.        :re
+00000950: 7475 726e 3a20 4e6f 6e65 0a20 2020 2020  turn: None.     
+00000960: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+00000970: 656c 662e 6375 7272 656e 745f 7175 6f74  elf.current_quot
+00000980: 655f 6173 7365 745f 616c 6c6f 7761 6e63  e_asset_allowanc
+00000990: 6520 3d20 6e65 775f 7175 6f74 655f 6173  e = new_quote_as
+000009a0: 7365 745f 616c 6c6f 7761 6e63 650a 0a0a  set_allowance...
+000009b0: 636c 6173 7320 5061 6972 446f 6573 4e6f  class PairDoesNo
+000009c0: 7445 7869 7374 4578 6365 7074 696f 6e28  tExistException(
+000009d0: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
+000009e0: 2222 2245 7863 6570 7469 6f6e 2072 6169  """Exception rai
+000009f0: 7365 6420 7768 656e 2061 6e20 6173 7365  sed when an asse
+00000a00: 7420 7061 6972 2064 6f65 7320 6e6f 7420  t pair does not 
+00000a10: 6578 6973 742e 0a0a 2020 2020 3a70 6172  exist...    :par
+00000a20: 616d 206d 7367 3a20 4572 726f 7220 6d65  am msg: Error me
+00000a30: 7373 6167 652e 0a20 2020 203a 7479 7065  ssage..    :type
+00000a40: 206d 7367 3a20 7374 720a 2020 2020 2222   msg: str.    ""
+00000a50: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00000a60: 745f 5f28 7365 6c66 2c20 6d73 673a 2073  t__(self, msg: s
+00000a70: 7472 293a 0a20 2020 2020 2020 2073 7570  tr):.        sup
+00000a80: 6572 2829 2e5f 5f69 6e69 745f 5f28 6d73  er().__init__(ms
+00000a90: 6729 0a                                  g).
```

### Comparing `rubi-2.0.2b4/rubi/types/order.py` & `rubi-2.0.3/rubi/types/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     :type max_priority_fee_per_gas: int
     """
 
     def __init__(
         self,
         orders: List[BaseNewOrder],
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: int = 3500000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ):
         """constructor method"""
         if len(orders) < 1:
             raise Exception("Transaction cannot be instantiated with an empty order list")
```

### Comparing `rubi-2.0.2b4/rubi/types/orderbook.py` & `rubi-2.0.3/rubi/types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.2b4/PKG-INFO` & `rubi-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.0.2b4
+Version: 2.0.3
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

