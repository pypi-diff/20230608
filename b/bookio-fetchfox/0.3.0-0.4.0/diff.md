# Comparing `tmp/bookio_fetchfox-0.3.0.tar.gz` & `tmp/bookio_fetchfox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.3.0.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.4.0.tar", max compression
```

## Comparing `bookio_fetchfox-0.3.0.tar` & `bookio_fetchfox-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     3723 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      596 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1349 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1764 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      592 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2658 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      449 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1606 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/jpgstore.py
--rwxr-xr-x   0        0        0      675 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4147 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2555 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     6862 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      504 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     1996 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    10727 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1061 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0      452 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     8690 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      619 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0      453 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      154 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      178 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2263 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     1215 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      463 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1320 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      362 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1382 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1677 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/rest.py
--rw-r--r--   0        0        0     1148 2023-06-05 21:22:29.787876 bookio_fetchfox-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.3.0/setup.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3723 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2140 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      596 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1349 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1764 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      592 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      449 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1606 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      675 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4147 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2555 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     7721 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      504 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     1996 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    11423 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1061 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0      452 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0     9554 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      619 2023-06-08 19:24:11.326686 bookio_fetchfox-0.4.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      154 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      112 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0      296 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      188 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2263 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     1215 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      463 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1409 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      362 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1792 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1677 2023-06-08 19:24:11.330686 bookio_fetchfox-0.4.0/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2023-06-08 19:24:11.342686 bookio_fetchfox-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.4.0/setup.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.4.0/PKG-INFO
```

### Comparing `bookio_fetchfox-0.3.0/README.md` & `bookio_fetchfox-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/cardano/blockfrostio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.4.0/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.4.0/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 12% similar despite different names*

```diff
@@ -113,15 +113,16 @@
 
     def get_listings(self, collection_id: str, *args, **kwargs) -> Iterable[ListingDTO]:
         self.check_collection_id(collection_id)
 
         listings = randswapcom.get_listings(collection_id)
 
         for listing in listings:
-            asset_ids = [str(listing["assetId"])]
+            asset_id = str(listing["assetId"])
+            asset_ids = [asset_id]
             asset_names = [""]
 
             listed_at = datetime.fromtimestamp(
                 listing["timestamp"] // 1000,
             ).replace(
                 tzinfo=pytz.UTC,
             )
@@ -133,20 +134,22 @@
                 asset_names=asset_names,
                 listing_id=listing["timestamp"],
                 marketplace=RANDGALLERY_COM,
                 price=listing["price"],
                 currency=ALGO,
                 listed_at=listed_at,
                 listed_by=listing["sellerAddress"],
+                marketplace_url=f"https://www.randgallery.com/algo-collection/?address={asset_id}",
             )
 
         listings = algoxnftcom.get_listings(collection_id)
 
         for listing in listings:
-            asset_ids = [str(listing["asset_id"])]
+            asset_id = str(listing["assetId"])
+            asset_ids = [asset_id]
             asset_names = [""]
 
             listed_at = datetime.now(tz=pytz.utc)
 
             yield ListingDTO(
                 identifier=listing["buy_it_now_listing_id"],
                 collection_id=collection_id,
@@ -154,14 +157,15 @@
                 asset_names=asset_names,
                 listing_id=listing["buy_it_now_listing_id"],
                 marketplace=ALGOXNFT_COM,
                 price=listing["price"] // 10**6,
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=listing["seller"],
+                marketplace_url=f"https://algoxnft.com/asset/{asset_id}",
             )
 
     def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
         self.check_collection_id(collection_id)
 
         floor = None
 
@@ -185,29 +189,44 @@
 
         sales = nftexplorerapp.get_sales(
             collection_id,
             api_key=self.nftexplorerapp_api_key,
         )
 
         for sale in sales:
-            asset_ids = [str(sale["asset"])]
-            asset_names = [sale["assetName"]]
+            tx_hash = sale["txnId"]
+
+            asset_id = str(sale["asset"])
+            asset_name = sale["assetName"]
 
             confirmed_at = datetime.fromtimestamp(
                 sale["epochMs"] // 1000,
             ).replace(
                 tzinfo=pytz.UTC,
             )
 
+            marketplace = venues[sale.get("venue")]
+
+            if marketplace == RANDGALLERY_COM:
+                marketplace_url = f"https://www.randgallery.com/algo-collection/?address={asset_id}"
+            elif marketplace == ALGOXNFT_COM:
+                marketplace_url = f"https://algoxnft.com/asset/{asset_id}"
+            elif marketplace == SHUFL_APP:
+                marketplace_url = f"https://shufl.app/detail/{asset_id}"
+            else:
+                marketplace_url = None
+
             yield SaleDTO(
-                identifier=sale["txnId"],
+                identifier=tx_hash,
                 collection_id=collection_id,
-                asset_ids=asset_ids,
-                asset_names=asset_names,
-                tx_hash=sale["txnId"],
-                marketplace=venues[sale.get("venue")],
+                asset_ids=[asset_id],
+                asset_names=[asset_name],
+                tx_hash=tx_hash,
+                marketplace=marketplace,
                 price=sale["ualgos"] // 10**6,
                 currency=self.currency,
                 confirmed_at=confirmed_at,
                 sold_by=sale["sender"],
                 bought_by=sale["receiver"],
+                marketplace_url=marketplace_url,
+                explorer_url=f"https://algoexplorer.io/tx/{tx_hash}",
             )
```

### Comparing `bookio_fetchfox-0.3.0/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.4.0/fetchfox/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.4.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,21 @@
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
     HoldingDTO,
     ListingDTO,
     RankDTO,
     SaleDTO,
+    SaleType,
 )
 from fetchfox.helpers import formatters
 from . import utils
 
+WINTER_NFT_ADDRESS = "addr1qxnrv2quqxhvwxtxmygsmkufph4kjju6j5len7k2ljslpz8ql7k7gehlfvj6ektgu9ns8yx8epcp66337khxeq82rpgqe6lqyk"
+
 logger = logging.getLogger(__name__)
 
 
 class Cardano(Blockchain):
     def __init__(self, blockfrostio_project_id: str = None):
         super().__init__(CARDANO, ADA)
 
@@ -230,14 +233,15 @@
                 listing_id=listing["listing_id"],
                 marketplace=JPG_STORE,
                 price=int(listing["price_lovelace"]) // 10**6,
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=None,
                 tx_hash=listing["tx_hash"],
+                marketplace_url=f"https://www.jpg.store/asset/{asset_id}",
             )
 
     def get_floor(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Optional[ListingDTO]:
         self.check_collection_id(collection_id)
 
         floor = None
 
@@ -249,32 +253,41 @@
 
         return floor
 
     def get_sales(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Iterable[SaleDTO]:
         self.check_collection_id(collection_id)
 
         for sale in jpgstore.get_sales(collection_id):
+            tx_hash = sale["tx_hash"]
+
             asset_id = sale["asset_id"]
             policy_id, asset_name = utils.split_asset_id(asset_id)
 
             # required for multi-book policies (e.g. monsters, greek classics)
             if discriminator:
                 if discriminator not in asset_name.lower():
                     continue
 
             if sale["action"] == "ACCEPT_OFFER":
                 buyer = sale["seller_address"]
                 seller = sale["signer_address"]
+                sale_type = SaleType.OFFER
             elif sale["action"] == "ACCEPT_COLLECTION_OFFER":
                 buyer = sale["signer_address"]
                 seller = sale["seller_address"]
+                sale_type = SaleType.COLLECTION_OFFER
             else:
                 buyer = sale["signer_address"]
                 seller = sale["seller_address"]
 
+                if buyer == WINTER_NFT_ADDRESS:
+                    sale_type = SaleType.CREDIT_CARD
+                else:
+                    sale_type = SaleType.PURCHASE
+
             asset_ids = []
             asset_names = []
 
             if sale["listing_from_tx_history"]["bundled_assets"]:
                 for bundled_asset in sale["listing_from_tx_history"]["bundled_assets"]:
                     asset_ids.append(bundled_asset["asset_id"])
                     asset_names.append(bundled_asset["display_name"])
@@ -284,19 +297,22 @@
 
             if sale.get("confirmed_at"):
                 confirmed_at = datetime.fromisoformat(sale["confirmed_at"].replace("Z", "+00:00"))
             else:
                 confirmed_at = datetime.now(tz=pytz.utc)
 
             yield SaleDTO(
-                identifier=sale["tx_hash"],
+                identifier=tx_hash,
                 collection_id=policy_id,
                 asset_ids=asset_ids,
                 asset_names=asset_names,
-                tx_hash=sale["tx_hash"],
+                tx_hash=tx_hash,
                 marketplace=JPG_STORE,
                 price=int(sale["amount_lovelace"]) // 10**6,
                 currency=self.currency,
                 confirmed_at=confirmed_at,
+                type=sale_type,
                 sold_by=seller,
                 bought_by=buyer,
+                marketplace_url=f"https://www.jpg.store/asset/{asset_id}",
+                explorer_url=f"https://cardanoscan.io/transaction/{tx_hash}",
             )
```

### Comparing `bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.4.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.4.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Iterable, Optional
 
 import pytz
 
 from fetchfox.apis import bookio
 from fetchfox.apis.evm import moralisio, ensideascom, openseaio
 from fetchfox.blockchains.base import Blockchain
-from fetchfox.constants.blockchains import ETHEREUM
+from fetchfox.constants.blockchains import ETHEREUM, POLYGON
 from fetchfox.constants.marketplaces import OPENSEA_IO
 from fetchfox.dtos import AssetDTO, CampaignDTO, HoldingDTO, ListingDTO, SaleDTO
 from fetchfox.helpers import formatters
 from . import utils
 
 logger = logging.getLogger(__name__)
 
@@ -179,32 +179,39 @@
             asset_names = []
 
             for offer in parameters["offer"]:
                 if offer["token"].lower() != collection_id.lower():
                     continue
 
                 asset_ids.append(offer["identifierOrCriteria"])
+                asset_names.append("")
 
             if listing.get("eventTimestamp"):
                 listed_at = datetime.utcfromtimestamp(parameters["startTime"])
             else:
                 listed_at = datetime.now(tz=pytz.utc)
 
+            if self.name == POLYGON:
+                marketplace_url = f"https://opensea.io/assets/matic/{collection_id}/{asset_ids[0]}"
+            else:
+                marketplace_url = f"https://opensea.io/assets/ethereum/{collection_id}/{asset_ids[0]}"
+
             yield ListingDTO(
                 identifier=listing["order_hash"],
                 collection_id=collection_id,
                 asset_ids=asset_ids,
                 asset_names=asset_names,
                 listing_id=listing["order_hash"],
                 marketplace=OPENSEA_IO,
                 price=float(int(price["value"]) / 10 ** price["decimals"]),
                 currency=price["currency"].replace("WETH", "ETH"),
                 listed_at=listed_at,
                 listed_by=parameters["offerer"],
                 tx_hash=listing["order_hash"],
+                marketplace_url=marketplace_url,
             )
 
     def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
         self.check_collection_id(collection_id)
 
         floor = None
 
@@ -222,31 +229,41 @@
         sales = openseaio.get_sales(
             collection_id,
             api_key=self.openseaio_api_key,
             slug=slug,
         )
 
         for sale in sales:
-            asset = sale["asset"]
+            tx_hash = sale["transaction"]["transaction_hash"]
 
-            asset_ids = [asset["token_id"]]
-            asset_names = [asset["name"]]
+            asset = sale["asset"]
+            asset_id = asset["token_id"]
+            asset_name = asset["name"]
 
             if sale.get("event_timestamp"):
                 confirmed_at = datetime.fromisoformat(sale["event_timestamp"] + "+00:00")
             else:
                 confirmed_at = datetime.now(tz=pytz.utc)
 
+            if self.name == POLYGON:
+                marketplace_url = f"https://opensea.io/assets/matic/{collection_id}/{asset_id}"
+                explorer_url = f"https://polygonscan.com/tx/{tx_hash}"
+            else:
+                marketplace_url = f"https://opensea.io/assets/ethereum/{collection_id}/{asset_id}"
+                explorer_url = f"https://etherscan.io/tx/{tx_hash}"
+
             yield SaleDTO(
                 identifier=sale["id"],
                 collection_id=collection_id,
-                asset_ids=asset_ids,
-                asset_names=asset_names,
-                tx_hash=sale["transaction"]["transaction_hash"],
+                asset_ids=[asset_id],
+                asset_names=[asset_name],
+                tx_hash=tx_hash,
                 marketplace=OPENSEA_IO,
                 price=float(int(sale["total_price"]) / 10 ** sale["payment_token"]["decimals"]),
                 currency=sale["payment_token"]["symbol"].replace("WETH", "ETH"),
                 confirmed_at=confirmed_at,
                 sold_by=sale["transaction"]["from_account"]["address"],
                 bought_by=sale["transaction"]["to_account"]["address"],
                 sale_id=sale["id"],
+                marketplace_url=marketplace_url,
+                explorer_url=explorer_url,
             )
```

### Comparing `bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.4.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.4.0/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.4.0/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.4.0/fetchfox/dtos/listing.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,26 +14,28 @@
         listing_id: str,
         marketplace: str,
         price: float,
         currency: str,
         listed_at: datetime,
         listed_by: str = None,
         tx_hash: str = None,
+        marketplace_url: str = None,
     ):
         self.identifier: str = identifier
         self.collection_id: str = collection_id
         self.asset_ids: List[str] = asset_ids
         self.asset_names: List[str] = asset_names
         self.listing_id: str = listing_id
         self.marketplace: str = marketplace
         self.price: float = price
         self.currency: str = currency
         self.listed_at: datetime = listed_at
         self.listed_by: str = listed_by
         self.tx_hash: str = tx_hash
+        self.marketplace_url: str = marketplace_url
 
     @property
     def usd(self) -> float:
         return self.price * coingeckocom.usd(self.currency)
 
     @property
     def first(self) -> str:
```

### Comparing `bookio_fetchfox-0.3.0/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.4.0/fetchfox/dtos/sale.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 from datetime import datetime
+from enum import Enum
 from typing import List
 
 from fetchfox.apis import coingeckocom
 
 
+class SaleType(str, Enum):
+    OFFER = "OFFER"
+    COLLECTION_OFFER = "INSTANT"
+    PURCHASE = "PURCHASE"
+    CREDIT_CARD = "CREDIT_CARD"
+
+
 class SaleDTO:
     def __init__(
         self,
         identifier: str,
         collection_id: str,
         asset_ids: List[str],
         asset_names: List[str],
         tx_hash: str,
         marketplace: str,
         price: float,
         currency: str,
         confirmed_at: datetime,
+        type: SaleType = SaleType.PURCHASE,
         sale_id: str = None,
         sold_by: str = None,
         bought_by: str = None,
+        marketplace_url: str = None,
+        explorer_url: str = None,
     ):
         self.identifier: str = identifier
         self.collection_id: str = collection_id
         self.asset_ids: List[str] = asset_ids
         self.asset_names: List[str] = asset_names
         self.tx_hash: str = tx_hash
         self.marketplace: str = marketplace
         self.price: float = price
         self.currency: str = currency
         self.confirmed_at: datetime = confirmed_at
+        self.type: SaleType = type
         self.sale_id: str = sale_id
         self.sold_by: str = sold_by
         self.bought_by: str = bought_by
+        self.marketplace_url: str = marketplace_url
+        self.explorer_url: str = explorer_url
 
     @property
     def usd(self) -> float:
         return self.price * coingeckocom.usd(self.currency)
 
     @property
     def first(self) -> str:
```

### Comparing `bookio_fetchfox-0.3.0/fetchfox/rest.py` & `bookio_fetchfox-0.4.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.3.0/pyproject.toml` & `bookio_fetchfox-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.3.0"
+version = "0.4.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-0.3.0/setup.py` & `bookio_fetchfox-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-0.3.0/PKG-INFO` & `bookio_fetchfox-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.3.0
+Version: 0.4.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```

