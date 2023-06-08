# Comparing `tmp/coinmetrics_api_client-2023.5.26.17.tar.gz` & `tmp/coinmetrics_api_client-2023.6.8.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinmetrics_api_client-2023.5.26.17.tar", max compression
+gzip compressed data, was "coinmetrics_api_client-2023.6.8.20.tar", max compression
```

## Comparing `coinmetrics_api_client-2023.5.26.17.tar` & `coinmetrics_api_client-2023.6.8.20.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1088 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/LICENSE
--rw-r--r--   0        0        0    20460 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/README.md
--rw-r--r--   0        0        0       29 2023-05-26 17:44:05.653887 coinmetrics_api_client-2023.5.26.17/coinmetrics/__init__.py
--rw-r--r--   0        0        0    20751 2023-05-26 17:43:04.970269 coinmetrics_api_client-2023.5.26.17/coinmetrics/_catalogs.py
--rw-r--r--   0        0        0     9947 2023-04-21 16:07:42.661803 coinmetrics_api_client-2023.5.26.17/coinmetrics/_data_collection.py
--rw-r--r--   0        0        0     2328 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/coinmetrics/_exceptions.py
--rw-r--r--   0        0        0     1286 2023-05-26 17:43:04.970269 coinmetrics_api_client-2023.5.26.17/coinmetrics/_models.py
--rw-r--r--   0        0        0      699 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/coinmetrics/_typing.py
--rw-r--r--   0        0        0     3951 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/coinmetrics/_utils.py
--rw-r--r--   0        0        0   233688 2023-05-26 17:43:04.970269 coinmetrics_api_client-2023.5.26.17/coinmetrics/api_client.py
--rw-r--r--   0        0        0        0 2023-05-26 17:52:06.838675 coinmetrics_api_client-2023.5.26.17/coinmetrics/build.py
--rw-r--r--   0        0        0      148 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/coinmetrics/constants.py
--rw-r--r--   0        0        0    20520 2023-03-15 18:54:39.226986 coinmetrics_api_client-2023.5.26.17/coinmetrics/data_exporter.py
--rw-r--r--   0        0        0     8669 2023-03-15 16:25:45.286233 coinmetrics_api_client-2023.5.26.17/coinmetrics/typer_cli.py
--rw-r--r--   0        0        0     1237 2023-05-26 17:44:05.657887 coinmetrics_api_client-2023.5.26.17/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 17:52:06.842675 coinmetrics_api_client-2023.5.26.17/test/__init__.py
--rw-r--r--   0        0        0     1640 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_asset_pair_candles.csv
--rw-r--r--   0        0        0      412 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_asset_pairs.csv
--rw-r--r--   0        0        0     2097 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_assets_markets.csv
--rw-r--r--   0        0        0      605 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_assets_metrics.csv
--rw-r--r--   0        0        0      436 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchange_assets.csv
--rw-r--r--   0        0        0     3595 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchanges_markets.csv
--rw-r--r--   0        0        0      822 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchanges_metrics.csv
--rw-r--r--   0        0        0      556 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_indexes.csv
--rw-r--r--   0        0        0      223 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_institutions.csv
--rw-r--r--   0        0        0      178 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_market_orderbooks.csv
--rw-r--r--   0        0        0      254 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_market_quotes.csv
--rw-r--r--   0        0        0      297 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_market_trades.csv
--rw-r--r--   0        0        0      579 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_markets.csv
--rw-r--r--   0        0        0     2557 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_metrics.csv
--rw-r--r--   0        0        0    28915 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/test_api_client.py
--rw-r--r--   0        0        0    10311 2023-04-10 18:58:58.715180 coinmetrics_api_client-2023.5.26.17/test/test_api_methods.py
--rw-r--r--   0        0        0     2910 2023-03-16 17:53:46.528810 coinmetrics_api_client-2023.5.26.17/test/test_as_list.py
--rw-r--r--   0        0        0     1788 2023-04-10 18:58:58.715180 coinmetrics_api_client-2023.5.26.17/test/test_blockchain_methods.py
--rw-r--r--   0        0        0     2273 2023-03-15 16:25:45.306233 coinmetrics_api_client-2023.5.26.17/test/test_custom_exceptions.py
--rw-r--r--   0        0        0    13462 2023-03-15 16:25:45.306233 coinmetrics_api_client-2023.5.26.17/test/test_data_exporter.py
--rw-r--r--   0        0        0     1015 2023-03-15 16:25:45.306233 coinmetrics_api_client-2023.5.26.17/test/test_debugging.py
--rw-r--r--   0        0        0     2142 2023-04-21 16:07:42.665803 coinmetrics_api_client-2023.5.26.17/test/test_models.py
--rw-r--r--   0        0        0     1193 2023-05-02 20:36:52.152834 coinmetrics_api_client-2023.5.26.17/test/test_rate_limits.py
--rw-r--r--   0        0        0    14167 2023-04-25 18:16:09.653330 coinmetrics_api_client-2023.5.26.17/test/test_to_dataframe.py
--rw-r--r--   0        0        0     5829 2023-05-02 20:36:52.152834 coinmetrics_api_client-2023.5.26.17/test/test_websocket_methods.py
--rw-r--r--   0        0        0    21649 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.5.26.17/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/LICENSE
+-rw-r--r--   0        0        0    20460 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/README.md
+-rw-r--r--   0        0        0       28 2023-06-08 20:26:54.999797 coinmetrics_api_client-2023.6.8.20/coinmetrics/__init__.py
+-rw-r--r--   0        0        0    20960 2023-06-08 16:41:39.966788 coinmetrics_api_client-2023.6.8.20/coinmetrics/_catalogs.py
+-rw-r--r--   0        0        0     9947 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/_data_collection.py
+-rw-r--r--   0        0        0     2328 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/_exceptions.py
+-rw-r--r--   0        0        0     1286 2023-06-07 14:08:45.748120 coinmetrics_api_client-2023.6.8.20/coinmetrics/_models.py
+-rw-r--r--   0        0        0      699 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/_typing.py
+-rw-r--r--   0        0        0     3951 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/_utils.py
+-rw-r--r--   0        0        0   233688 2023-06-07 14:08:45.748120 coinmetrics_api_client-2023.6.8.20/coinmetrics/api_client.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:34:37.623456 coinmetrics_api_client-2023.6.8.20/coinmetrics/build.py
+-rw-r--r--   0        0        0      148 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/constants.py
+-rw-r--r--   0        0        0    20520 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/data_exporter.py
+-rw-r--r--   0        0        0     8669 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/typer_cli.py
+-rw-r--r--   0        0        0     1236 2023-06-08 20:26:54.999797 coinmetrics_api_client-2023.6.8.20/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 20:34:37.627456 coinmetrics_api_client-2023.6.8.20/test/__init__.py
+-rw-r--r--   0        0        0     1640 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_asset_pair_candles.csv
+-rw-r--r--   0        0        0      412 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_asset_pairs.csv
+-rw-r--r--   0        0        0     2097 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_assets_markets.csv
+-rw-r--r--   0        0        0      605 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_assets_metrics.csv
+-rw-r--r--   0        0        0      436 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchange_assets.csv
+-rw-r--r--   0        0        0     3595 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchanges_markets.csv
+-rw-r--r--   0        0        0      822 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchanges_metrics.csv
+-rw-r--r--   0        0        0      556 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_indexes.csv
+-rw-r--r--   0        0        0      223 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_institutions.csv
+-rw-r--r--   0        0        0      178 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_market_orderbooks.csv
+-rw-r--r--   0        0        0      254 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_market_quotes.csv
+-rw-r--r--   0        0        0      297 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_market_trades.csv
+-rw-r--r--   0        0        0      579 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_markets.csv
+-rw-r--r--   0        0        0     2557 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_metrics.csv
+-rw-r--r--   0        0        0    28915 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_api_client.py
+-rw-r--r--   0        0        0    10311 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_api_methods.py
+-rw-r--r--   0        0        0     2910 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_as_list.py
+-rw-r--r--   0        0        0     1788 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_blockchain_methods.py
+-rw-r--r--   0        0        0     2273 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_custom_exceptions.py
+-rw-r--r--   0        0        0    13462 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_data_exporter.py
+-rw-r--r--   0        0        0     1015 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_debugging.py
+-rw-r--r--   0        0        0     2142 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_models.py
+-rw-r--r--   0        0        0     1193 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_rate_limits.py
+-rw-r--r--   0        0        0    14793 2023-06-08 16:41:39.966788 coinmetrics_api_client-2023.6.8.20/test/test_to_dataframe.py
+-rw-r--r--   0        0        0     5829 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_websocket_methods.py
+-rw-r--r--   0        0        0    21648 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.6.8.20/PKG-INFO
```

### Comparing `coinmetrics_api_client-2023.5.26.17/LICENSE` & `coinmetrics_api_client-2023.6.8.20/LICENSE`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/README.md` & `coinmetrics_api_client-2023.6.8.20/README.md`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/_catalogs.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/_catalogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -521,23 +521,37 @@
     """
     Transforms catalog data in list form into a dataframe
     :return: Catalog Data
     """
 
     def to_dataframe(self) -> DataFrameType:
         df_catalog_market_metrics = pd.DataFrame(self)
-        df_catalog_market_metrics = df_catalog_market_metrics.explode("metrics")
-        df_metrics = pd.json_normalize(df_catalog_market_metrics['metrics'])
-        df_catalog_market_metrics = df_catalog_market_metrics.join(df_metrics)
-        df_catalog_market_metrics = df_catalog_market_metrics.explode("frequencies")
-        df_frequencies = pd.json_normalize(df_catalog_market_metrics['frequencies'])
-        df_catalog_market_metrics = df_catalog_market_metrics.join(df_frequencies)
-        df_catalog_market_metrics = df_catalog_market_metrics.drop(["metrics", "frequencies"], axis=1)
-        df_catalog_market_metrics = df_catalog_market_metrics.reset_index(drop=True)
-
+        df_catalog_market_metrics = (
+            df_catalog_market_metrics.explode("metrics")
+            .assign(metric=lambda df: _expand_df(key="metric", iterable=df.metrics))
+            .assign(
+                frequencies=lambda df: _expand_df(
+                    key="frequencies", iterable=df.metrics
+                )
+            )
+            .explode("frequencies")
+            .assign(
+                frequency=lambda df: _expand_df(
+                    key="frequency", iterable=df.frequencies
+                )
+            )
+            .assign(
+                min_time=lambda df: _expand_df(key="min_time", iterable=df.frequencies)
+            )
+            .assign(
+                max_time=lambda df: _expand_df(key="max_time", iterable=df.frequencies)
+            )
+            .reset_index(drop=True)
+            .drop(["metrics", "frequencies"], axis=1)
+        )
         return convert_catalog_dtypes(df_catalog_market_metrics)
 
 
 class CatalogMarketCandlesData(List[Any]):
     """
     Transforms catalog data in list form into a dataframe
     :return: Catalog Data
```

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/_data_collection.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/_data_collection.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/_exceptions.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/_models.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/_typing.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/_typing.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/_utils.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/_utils.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/api_client.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/api_client.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/data_exporter.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/coinmetrics/typer_cli.py` & `coinmetrics_api_client-2023.6.8.20/coinmetrics/typer_cli.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/pyproject.toml` & `coinmetrics_api_client-2023.6.8.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinmetrics-api-client"
-version = "2023.5.26.17"
+version = "2023.6.8.20"
 description = "Python client for Coin Metrics API v4."
 authors = ["Coin Metrics <info@coinmetrics.io>", "Oleksandr Buchkovskyi <oleksandr@coinmetrics.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://coinmetrics.github.io/api-client-python/site/index.html"
 repository = "https://github.com/coinmetrics/api-client-python"
 packages = [{include = "coinmetrics"}]
```

### Comparing `coinmetrics_api_client-2023.5.26.17/test/data/catalog_asset_pair_candles.csv` & `coinmetrics_api_client-2023.6.8.20/test/data/catalog_asset_pair_candles.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/data/catalog_assets_markets.csv` & `coinmetrics_api_client-2023.6.8.20/test/data/catalog_assets_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/data/catalog_assets_metrics.csv` & `coinmetrics_api_client-2023.6.8.20/test/data/catalog_assets_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchanges_markets.csv` & `coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchanges_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchanges_metrics.csv` & `coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchanges_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/data/catalog_indexes.csv` & `coinmetrics_api_client-2023.6.8.20/test/data/catalog_indexes.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/data/catalog_markets.csv` & `coinmetrics_api_client-2023.6.8.20/test/data/catalog_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/data/catalog_metrics.csv` & `coinmetrics_api_client-2023.6.8.20/test/data/catalog_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_api_client.py` & `coinmetrics_api_client-2023.6.8.20/test/test_api_client.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_api_methods.py` & `coinmetrics_api_client-2023.6.8.20/test/test_api_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_as_list.py` & `coinmetrics_api_client-2023.6.8.20/test/test_as_list.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_blockchain_methods.py` & `coinmetrics_api_client-2023.6.8.20/test/test_blockchain_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_custom_exceptions.py` & `coinmetrics_api_client-2023.6.8.20/test/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_data_exporter.py` & `coinmetrics_api_client-2023.6.8.20/test/test_data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_debugging.py` & `coinmetrics_api_client-2023.6.8.20/test/test_debugging.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_models.py` & `coinmetrics_api_client-2023.6.8.20/test/test_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_rate_limits.py` & `coinmetrics_api_client-2023.6.8.20/test/test_rate_limits.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_to_dataframe.py` & `coinmetrics_api_client-2023.6.8.20/test/test_to_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,9 +378,24 @@
 def test_market_implied_vol_catalog_full() -> None:
     data = client.catalog_full_market_implied_volatility().to_dataframe()
     assert len(data) > 100
     expected_cols = ["market", "min_time", "max_time"]
     assert all([col in data.columns for col in expected_cols])
 
 
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_catalog_market_metrics_row_counts() -> None:
+    """
+    Tests that data is the same coming from both the as a list and to_dataframe
+    """
+    list_data = client.catalog_market_metrics(exchange="coinbase")
+    count_markets_and_frequencies = 0
+    for catalog_data in list_data:
+        for metric_data in catalog_data['metrics']:
+            count_markets_and_frequencies += len(metric_data['frequencies'])
+    as_data_frame = list_data.to_dataframe()
+    count_df_rows = len(as_data_frame)
+    assert count_df_rows == count_markets_and_frequencies
+
+
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `coinmetrics_api_client-2023.5.26.17/test/test_websocket_methods.py` & `coinmetrics_api_client-2023.6.8.20/test/test_websocket_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.26.17/PKG-INFO` & `coinmetrics_api_client-2023.6.8.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinmetrics-api-client
-Version: 2023.5.26.17
+Version: 2023.6.8.20
 Summary: Python client for Coin Metrics API v4.
 Home-page: https://coinmetrics.github.io/api-client-python/site/index.html
 License: MIT
 Keywords: coin metrics,coin,metrics,crypto,bitcoin,network-data,market-data,api,handy
 Author: Coin Metrics
 Author-email: info@coinmetrics.io
 Requires-Python: >=3.7.1,<4.0.0
```

