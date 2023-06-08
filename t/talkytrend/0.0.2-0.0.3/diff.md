# Comparing `tmp/talkytrend-0.0.2.tar.gz` & `tmp/talkytrend-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-0.0.2.tar", max compression
+gzip compressed data, was "talkytrend-0.0.3.tar", max compression
```

## Comparing `talkytrend-0.0.2.tar` & `talkytrend-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-08 15:20:28.732463 talkytrend-0.0.2/LICENSE
--rw-r--r--   0        0        0     1336 2023-06-08 15:20:28.732463 talkytrend-0.0.2/README.md
--rw-r--r--   0        0        0     1686 2023-06-08 15:20:42.748369 talkytrend-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      102 2023-06-08 15:20:42.748369 talkytrend-0.0.2/talkytrend/__init__.py
--rw-r--r--   0        0        0      630 2023-06-08 15:20:28.732463 talkytrend-0.0.2/talkytrend/config.py
--rw-r--r--   0        0        0      264 2023-06-08 15:20:28.732463 talkytrend-0.0.2/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     1914 2023-06-08 15:20:28.732463 talkytrend-0.0.2/talkytrend/main.py
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 talkytrend-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 16:30:15.258978 talkytrend-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1336 2023-06-08 16:30:15.258978 talkytrend-0.0.3/README.md
+-rw-r--r--   0        0        0     1686 2023-06-08 16:30:29.603948 talkytrend-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-06-08 16:30:29.603948 talkytrend-0.0.3/talkytrend/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-08 16:30:15.258978 talkytrend-0.0.3/talkytrend/config.py
+-rw-r--r--   0        0        0      264 2023-06-08 16:30:15.258978 talkytrend-0.0.3/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     1818 2023-06-08 16:30:15.258978 talkytrend-0.0.3/talkytrend/main.py
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 talkytrend-0.0.3/PKG-INFO
```

### Comparing `talkytrend-0.0.2/LICENSE` & `talkytrend-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-0.0.2/README.md` & `talkytrend-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-0.0.2/pyproject.toml` & `talkytrend-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "0.0.2"
+version = "0.0.3"
 description = "A python package to retrieve key economic data such as Trend, Key economic data for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-0.0.2/talkytrend/config.py` & `talkytrend-0.0.3/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-0.0.2/talkytrend/main.py` & `talkytrend-0.0.3/talkytrend/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
  talky trend Main
 """
-__version__ = "0.0.0"
 
 import asyncio
 import logging 
 
 from tradingview_ta import TA_Handler, Interval
 
 from talkytrend import __version__
@@ -21,25 +20,25 @@
         if asset is None:
             asset = settings.asset
         self.enabled = settings.plugin_trend
         self.asset = asset
         self.exchange = exchange
         self.screener = screener
         self.interval = interval
-#         self.asset_signals = {asset: {'15m': None, '4h': None} for asset in self.assets}
+        self.asset_signals = {'15m': None, '4h': None} 
 
     async def fetch_analysis(self):
-        # Initialize the TA_Handler 
+        
+        # Initialize the TA_Handler
         handler = TA_Handler(
         symbol=self.asset,
         exchange=self.exchange,
         screener=self.screener,
         interval=self.interval)
 
-        # Fetch the technical analysis summary
         analysis = handler.get_analysis()
         print(analysis)
         return analysis.summary['RECOMMENDATION']
 
 #     async def check_signal(self, asset):
 #         for interval in ['15m', '4h']:
 #             current_signal = await self.fetch_analysis(asset, interval)
```

### Comparing `talkytrend-0.0.2/PKG-INFO` & `talkytrend-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package to retrieve key economic data such as Trend, Key economic data for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

