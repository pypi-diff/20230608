# Comparing `tmp/ezyquant-0.7.3.tar.gz` & `tmp/ezyquant-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-0.7.3.tar", last modified: Thu Jun  8 07:49:52 2023, max compression
+gzip compressed data, was "ezyquant-0.7.4.tar", last modified: Thu Jun  8 09:27:14 2023, max compression
```

## Comparing `ezyquant-0.7.3.tar` & `ezyquant-0.7.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.258824 ezyquant-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 07:48:46.000000 ezyquant-0.7.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-08 07:49:52.258824 ezyquant-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-08 07:48:46.000000 ezyquant-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.254824 ezyquant-0.7.3/ezyquant/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.258824 ezyquant-0.7.3/ezyquant/backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.258824 ezyquant-0.7.3/ezyquant/indicators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/pivot_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/rsi_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/ta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/zigzag.py
--rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.254824 ezyquant-0.7.3/ezyquant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 07:49:52.258824 ezyquant-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-08 07:48:46.000000 ezyquant-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.258824 ezyquant-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-06-08 07:48:46.000000 ezyquant-0.7.3/tests/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-06-08 07:48:46.000000 ezyquant-0.7.3/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-08 07:48:46.000000 ezyquant-0.7.3/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-08 07:48:46.000000 ezyquant-0.7.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:14.284501 ezyquant-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 09:26:12.000000 ezyquant-0.7.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-08 09:27:14.284501 ezyquant-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-08 09:26:12.000000 ezyquant-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:14.280501 ezyquant-0.7.4/ezyquant/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:14.280501 ezyquant-0.7.4/ezyquant/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/backtesting/_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/backtesting/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/backtesting/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/backtesting/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/backtesting/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:14.284501 ezyquant-0.7.4/ezyquant/indicators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/indicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/indicators/pivot_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/indicators/rsi_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21928 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/indicators/ta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/indicators/zigzag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 09:26:12.000000 ezyquant-0.7.4/ezyquant/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:14.280501 ezyquant-0.7.4/ezyquant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-08 09:27:14.000000 ezyquant-0.7.4/ezyquant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-08 09:27:14.000000 ezyquant-0.7.4/ezyquant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:27:14.000000 ezyquant-0.7.4/ezyquant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 09:27:14.000000 ezyquant-0.7.4/ezyquant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 09:27:14.000000 ezyquant-0.7.4/ezyquant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 09:27:14.284501 ezyquant-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-08 09:26:12.000000 ezyquant-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:14.284501 ezyquant-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-06-08 09:26:12.000000 ezyquant-0.7.4/tests/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-06-08 09:26:12.000000 ezyquant-0.7.4/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-08 09:26:12.000000 ezyquant-0.7.4/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-08 09:26:12.000000 ezyquant-0.7.4/tests/test_utils.py
```

### Comparing `ezyquant-0.7.3/LICENSE.txt` & `ezyquant-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/PKG-INFO` & `ezyquant-0.7.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.7.3
-Summary: Powerful backtest python library for Thai stocks
+Version: 0.7.4
+Summary: Powerful Python backtesting for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
 Project-URL: Documentation, https://pydoc.ezyquant.com/
@@ -14,8 +14,8 @@
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 
-Powerful backtest python library for Thai stocks
+Powerful Python backtesting for Thai stocks
```

### Comparing `ezyquant-0.7.3/README.md` & `ezyquant-0.7.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-<div align="center">
-  <img src="docs\source\_static\logo-text-right.svg">
-</div>
+[![Logo](docs/source/_static/logo-text-right.svg)](https://pydoc.ezyquant.com/)
 
------------------
+# EzyQuant: Powerful Python backtesting for Thai stocks
 
-# Ezyquant: Powerful backtest python library for Thai stocks
-
-[![PyPI](https://img.shields.io/pypi/v/ezyquant?label=PyPI)](https://pydoc.ezyquant.com/)
+[![PyPI](https://img.shields.io/pypi/v/ezyquant?label=PyPI)](https://pypi.org/project/ezyquant/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ezyquant?label=PyPI%20Downloads)](https://pepy.tech/project/ezyquant)
 [![License](https://img.shields.io/pypi/l/ezyquant.svg)](https://github.com/ezyquant/ezyquant/blob/main/LICENSE.txt)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## Features
```

### Comparing `ezyquant-0.7.3/ezyquant/backtesting/_backtesting.py` & `ezyquant-0.7.4/ezyquant/backtesting/_backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/backtesting/account.py` & `ezyquant-0.7.4/ezyquant/backtesting/account.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/backtesting/backtesting.py` & `ezyquant-0.7.4/ezyquant/backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/backtesting/context.py` & `ezyquant-0.7.4/ezyquant/backtesting/context.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/backtesting/position.py` & `ezyquant-0.7.4/ezyquant/backtesting/position.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/backtesting/trade.py` & `ezyquant-0.7.4/ezyquant/backtesting/trade.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/connect.py` & `ezyquant-0.7.4/ezyquant/connect.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/creator.py` & `ezyquant-0.7.4/ezyquant/creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/fields.py` & `ezyquant-0.7.4/ezyquant/fields.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/indicators/pivot_point.py` & `ezyquant-0.7.4/ezyquant/indicators/pivot_point.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/indicators/rsi_divergence.py` & `ezyquant-0.7.4/ezyquant/indicators/rsi_divergence.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         Series of 'high' prices.
     low : pd.Series
         Series of 'low' prices.
     close : pd.Series
         Series of 'close' prices.
     rsi_period : int, optional
         RSI period, by default 14
-    pivot_up_thresh : int
+    pivot_up_thresh : float
         Pivot up threshold, by default 0.05
-    pivot_down_thresh : int
+    pivot_down_thresh : float
         Pivot down threshold, by default -0.05
     """
     # Calculate RSI
     rsi_ = rsi(close, window=rsi_period)
 
     # Calculate pivot points using zigzag
     zz_ = zigzag.peak_valley_pivots_candlestick(
```

### Comparing `ezyquant-0.7.3/ezyquant/indicators/ta.py` & `ezyquant-0.7.4/ezyquant/indicators/ta.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     BollingerBands,
     DonchianChannel,
     KeltnerChannel,
 )
 
 from ..errors import InputError
 from .rsi_divergence import rsi_divergence
+from .zigzag import peak_valley_pivots_candlestick
 
 nan = float("nan")
 
 
 class TA:
     """Trend Indicators."""
 
@@ -313,14 +314,53 @@
         psar_down = _apply_t(ind, PSARIndicator.psar_down)
         psar_down_indicator = _apply_t(ind, PSARIndicator.psar_down_indicator)
         psar_up = _apply_t(ind, PSARIndicator.psar_up)
         psar_up_indicator = _apply_t(ind, PSARIndicator.psar_up_indicator)
 
         return psar, psar_down, psar_down_indicator, psar_up, psar_up_indicator
 
+    @staticmethod
+    def zigzag(
+        high: pd.DataFrame,
+        low: pd.DataFrame,
+        close: pd.DataFrame,
+        up_thresh: float = 0.05,
+        down_thresh: float = -0.05,
+    ) -> pd.DataFrame:
+        """Zig Zag.
+
+        Parameters
+        ----------
+        high: pd.DataFrame
+            dataset 'High' dataframe.
+        low: pd.DataFrame
+            dataset 'Low' dataframe.
+        close: pd.DataFrame
+            dataset 'Close' dataframe.
+        up_thresh: float = 0.05
+            up threshold value.
+        down_thresh: float = -0.05
+            down threshold value.
+
+        Returns
+        -------
+        pd.DataFrame
+            Zig Zag value. If the value is 1, it means high. If the value is -1, it means low.
+        """
+        out = close.apply(
+            lambda x: peak_valley_pivots_candlestick(
+                close=x,
+                high=high[x.name],
+                low=low[x.name],
+                up_thresh=up_thresh,
+                down_thresh=down_thresh,
+            )
+        )
+        return out
+
     """Momentum Indicators"""
 
     @staticmethod
     def rsi(
         close: pd.DataFrame, window: int = 14, fillna: bool = False
     ) -> pd.DataFrame:
         """Relative Strength Index (RSI)
@@ -376,15 +416,15 @@
             threshold for pivot up.
         pivot_down_thresh: float = -0.05
             threshold for pivot down.
 
         Returns
         -------
         pd.DataFrame
-            Relative Strength Index (RSI) Divergence
+            Relative Strength Index (RSI) Divergence. If bullish divergence, return 1. If bearish divergence, return -1.
         """
         out = close.apply(
             lambda x: rsi_divergence(
                 close=x,
                 high=high[x.name],
                 low=low[x.name],
                 rsi_period=rsi_period,
@@ -393,14 +433,15 @@
             )
         )
 
         # Return only signal
         out = np.sign(out)
         assert isinstance(out, pd.DataFrame)
         out = out.fillna(0)
+
         return out
 
     @staticmethod
     def sto(
         high: pd.DataFrame,
         low: pd.DataFrame,
         close: pd.DataFrame,
```

### Comparing `ezyquant-0.7.3/ezyquant/indicators/zigzag.py` & `ezyquant-0.7.4/ezyquant/indicators/zigzag.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/reader.py` & `ezyquant-0.7.4/ezyquant/reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/report.py` & `ezyquant-0.7.4/ezyquant/report.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/utils.py` & `ezyquant-0.7.4/ezyquant/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant/validators.py` & `ezyquant-0.7.4/ezyquant/validators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/ezyquant.egg-info/PKG-INFO` & `ezyquant-0.7.4/ezyquant.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.7.3
-Summary: Powerful backtest python library for Thai stocks
+Version: 0.7.4
+Summary: Powerful Python backtesting for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
 Project-URL: Documentation, https://pydoc.ezyquant.com/
@@ -14,8 +14,8 @@
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 
-Powerful backtest python library for Thai stocks
+Powerful Python backtesting for Thai stocks
```

### Comparing `ezyquant-0.7.3/ezyquant.egg-info/SOURCES.txt` & `ezyquant-0.7.4/ezyquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/setup.py` & `ezyquant-0.7.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 setup(
     name="ezyquant",
     packages=find_packages(include=["ezyquant", "ezyquant.*"]),
     version=verstr,
-    description="Powerful backtest python library for Thai stocks",
-    long_description="Powerful backtest python library for Thai stocks",
+    description="Powerful Python backtesting for Thai stocks",
+    long_description="Powerful Python backtesting for Thai stocks",
     author="Fintech (Thailand) Company Limited",
     author_email="admin@fintech.co.th",
     url="https://www.ezyquant.com/",
     maintainer="Fintech (Thailand) Company Limited",
     maintainer_email="admin@fintech.co.th",
     python_requires=">=3.8",
     install_requires=[
```

### Comparing `ezyquant-0.7.3/tests/test_creator.py` & `ezyquant-0.7.4/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/tests/test_reader.py` & `ezyquant-0.7.4/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/tests/test_test_utils.py` & `ezyquant-0.7.4/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.3/tests/test_utils.py` & `ezyquant-0.7.4/tests/test_utils.py`

 * *Files identical despite different names*

