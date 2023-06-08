# Comparing `tmp/ezyquant-0.7.2.tar.gz` & `tmp/ezyquant-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-0.7.2.tar", last modified: Wed Jun  7 12:05:23 2023, max compression
+gzip compressed data, was "ezyquant-0.7.3.tar", last modified: Thu Jun  8 07:49:52 2023, max compression
```

## Comparing `ezyquant-0.7.2.tar` & `ezyquant-0.7.3.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 12:04:19.000000 ezyquant-0.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 12:05:23.944775 ezyquant-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-07 12:04:19.000000 ezyquant-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/ezyquant/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/ezyquant/backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    23370 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/ezyquant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-07 12:05:23.948775 ezyquant-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-07 12:04:19.000000 ezyquant-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.258824 ezyquant-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 07:48:46.000000 ezyquant-0.7.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-08 07:49:52.258824 ezyquant-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-08 07:48:46.000000 ezyquant-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.254824 ezyquant-0.7.3/ezyquant/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.258824 ezyquant-0.7.3/ezyquant/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/backtesting/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.258824 ezyquant-0.7.3/ezyquant/indicators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/pivot_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/rsi_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/ta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/indicators/zigzag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 07:48:46.000000 ezyquant-0.7.3/ezyquant/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.254824 ezyquant-0.7.3/ezyquant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 07:49:52.000000 ezyquant-0.7.3/ezyquant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 07:49:52.258824 ezyquant-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-08 07:48:46.000000 ezyquant-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:49:52.258824 ezyquant-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-06-08 07:48:46.000000 ezyquant-0.7.3/tests/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-06-08 07:48:46.000000 ezyquant-0.7.3/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-08 07:48:46.000000 ezyquant-0.7.3/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-08 07:48:46.000000 ezyquant-0.7.3/tests/test_utils.py
```

### Comparing `ezyquant-0.7.2/LICENSE.txt` & `ezyquant-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/PKG-INFO` & `ezyquant-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.7.2
+Version: 0.7.3
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-0.7.2/README.md` & `ezyquant-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/backtesting/_backtesting.py` & `ezyquant-0.7.3/ezyquant/backtesting/_backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/backtesting/account.py` & `ezyquant-0.7.3/ezyquant/backtesting/account.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/backtesting/backtesting.py` & `ezyquant-0.7.3/ezyquant/backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/backtesting/context.py` & `ezyquant-0.7.3/ezyquant/backtesting/context.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/backtesting/position.py` & `ezyquant-0.7.3/ezyquant/backtesting/position.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/backtesting/trade.py` & `ezyquant-0.7.3/ezyquant/backtesting/trade.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/connect.py` & `ezyquant-0.7.3/ezyquant/connect.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/creator.py` & `ezyquant-0.7.3/ezyquant/creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
 from . import fields as fld
 from . import utils
 from .errors import InputError
-from .indicators import TA
+from .indicators.ta import TA
 from .reader import _SETDataReaderCached
 
 nan = float("nan")
 
 MethodType = Optional[Literal["backfill", "bfill", "ffill", "pad"]]
```

### Comparing `ezyquant-0.7.2/ezyquant/fields.py` & `ezyquant-0.7.3/ezyquant/fields.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/indicators.py` & `ezyquant-0.7.3/ezyquant/indicators/ta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import operator
 from typing import Callable, Tuple
 
 import numpy as np
 import pandas as pd
-import zigzag
-from ta.momentum import ROCIndicator, RSIIndicator, StochasticOscillator, rsi
+from ta.momentum import ROCIndicator, RSIIndicator, StochasticOscillator
 from ta.trend import MACD, ADXIndicator, CCIIndicator, IchimokuIndicator, PSARIndicator
 from ta.utils import _ema, _sma
 from ta.volatility import (
     AverageTrueRange,
     BollingerBands,
     DonchianChannel,
     KeltnerChannel,
 )
 
-from .errors import InputError
+from ..errors import InputError
+from .rsi_divergence import rsi_divergence
 
 nan = float("nan")
 
 
 class TA:
     """Trend Indicators."""
 
@@ -350,23 +349,29 @@
 
         rsi = _apply_t(ind, RSIIndicator.rsi)
 
         return rsi
 
     @staticmethod
     def rsi_divergence(
+        high: pd.DataFrame,
+        low: pd.DataFrame,
         close: pd.DataFrame,
         rsi_period: int = 14,
         pivot_up_thresh: float = 0.05,
         pivot_down_thresh: float = -0.05,
     ) -> pd.DataFrame:
         """Relative Strength Index (RSI) Divergence.
 
         Parameters
         ----------
+        high: pd.DataFrame
+            dataset 'High' dataframe.
+        low: pd.DataFrame
+            dataset 'Low' dataframe.
         close: pd.DataFrame
             dataset 'Close' dataframe.
         rsi_period: int = 14
             n period for RSI.
         pivot_up_thresh: float = 0.05
             threshold for pivot up.
         pivot_down_thresh: float = -0.05
@@ -376,14 +381,16 @@
         -------
         pd.DataFrame
             Relative Strength Index (RSI) Divergence
         """
         out = close.apply(
             lambda x: rsi_divergence(
                 close=x,
+                high=high[x.name],
+                low=low[x.name],
                 rsi_period=rsi_period,
                 pivot_up_thresh=pivot_up_thresh,
                 pivot_down_thresh=pivot_down_thresh,
             )
         )
 
         # Return only signal
@@ -708,114 +715,7 @@
 
 def _apply_t(series: pd.Series, func: Callable) -> pd.DataFrame:
     df = series.apply(func).T
     if df.empty:
         raise InputError(f"{func.__name__} returned an empty dataframe")
     assert isinstance(df, pd.DataFrame)
     return df
-
-
-"""
-Pivot
-"""
-
-
-def pivot_points_high(high: pd.Series, left_bars: int, right_bars: int) -> pd.Series:
-    """Pivot Points High.
-
-    High is the highest high in a window between left_bars and
-    right_bars. If multiple bars have the same high, the most right bar
-    is used.
-    """
-    max_ = high.rolling(window=left_bars + 1).max()
-    max_right = high.rolling(window=right_bars).max().shift(-right_bars)
-
-    return high.where((max_ == high) & (max_ > max_right))
-
-
-def pivot_points_low(low: pd.Series, left_bars: int, right_bars: int) -> pd.Series:
-    """Pivot Points Low.
-
-    Low is the lowest low in a window between left_bars and right_bars.
-    If multiple bars have the same low, the most right bar is used.
-    """
-    min_ = low.rolling(window=left_bars + 1).min()
-    min_right = low.rolling(window=right_bars).min().shift(-right_bars)
-
-    return low.where((min_ == low) & (min_ < min_right))
-
-
-"""
-RSI Divergence
-"""
-
-
-def rsi_divergence(
-    close: pd.Series,
-    rsi_period: int = 14,
-    pivot_up_thresh: float = 0.05,
-    pivot_down_thresh: float = -0.05,
-) -> pd.Series:
-    """Return Positive RSI of the bullish divergence points and Negative RSI of
-    the bearish divergence points.
-
-    Parameters
-    ----------
-    high : pd.Series
-        Series of 'high' prices.
-    low : pd.Series
-        Series of 'low' prices.
-    close : pd.Series
-        Series of 'close' prices.
-    rsi_period : int, optional
-        RSI period, by default 14
-    pivot_up_thresh : int
-        Pivot up threshold, by default 0.05
-    pivot_down_thresh : int
-        Pivot down threshold, by default -0.05
-    """
-    # Calculate RSI
-    rsi_ = rsi(close, window=rsi_period)
-
-    # Calculate pivot points using zigzag
-    zz_ = zigzag.peak_valley_pivots(  # type: ignore
-        close.to_numpy(),
-        up_thresh=pivot_up_thresh,
-        down_thresh=pivot_down_thresh,
-    )
-    close_pl = close[zz_ < 0]
-    close_ph = close[zz_ > 0]
-
-    # Calculate Divergence
-    bullish = _divergence(close_pl, rsi_, bullish=True)
-    bearish = _divergence(close_ph, rsi_, bullish=False)
-
-    return bullish.fillna(-bearish)
-
-
-def _divergence(
-    price_pivot: pd.Series, indicator: pd.Series, bullish: bool = True
-) -> pd.Series:
-    """Divergence.
-
-    Parameters
-    ----------
-    price_pivot : pd.Series
-        Price pivot points. low for bullish divergence and high for bearish divergence.
-    indicator : pd.Series
-        indicator series.
-    bullish : bool, optional
-        bullish or bearish divergence, by default True
-
-    Returns
-    -------
-    pd.Series
-        Divergence series. Not NaN when divergence occurs.
-    """
-    indicator_pivot = indicator[price_pivot.index]
-
-    op = operator.lt if bullish else operator.gt
-
-    return indicator.where(
-        op(price_pivot, price_pivot.shift(1))
-        & op(indicator_pivot.shift(1), indicator_pivot)
-    )
```

### Comparing `ezyquant-0.7.2/ezyquant/reader.py` & `ezyquant-0.7.3/ezyquant/reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/report.py` & `ezyquant-0.7.3/ezyquant/report.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/utils.py` & `ezyquant-0.7.3/ezyquant/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant/validators.py` & `ezyquant-0.7.3/ezyquant/validators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/ezyquant.egg-info/PKG-INFO` & `ezyquant-0.7.3/ezyquant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.7.2
+Version: 0.7.3
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-0.7.2/ezyquant.egg-info/SOURCES.txt` & `ezyquant-0.7.3/ezyquant.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.py
 ezyquant/__init__.py
 ezyquant/_version.py
 ezyquant/connect.py
 ezyquant/creator.py
 ezyquant/errors.py
 ezyquant/fields.py
-ezyquant/indicators.py
 ezyquant/reader.py
 ezyquant/report.py
 ezyquant/utils.py
 ezyquant/validators.py
 ezyquant.egg-info/PKG-INFO
 ezyquant.egg-info/SOURCES.txt
 ezyquant.egg-info/dependency_links.txt
@@ -21,12 +20,16 @@
 ezyquant/backtesting/__init__.py
 ezyquant/backtesting/_backtesting.py
 ezyquant/backtesting/account.py
 ezyquant/backtesting/backtesting.py
 ezyquant/backtesting/context.py
 ezyquant/backtesting/position.py
 ezyquant/backtesting/trade.py
+ezyquant/indicators/__init__.py
+ezyquant/indicators/pivot_point.py
+ezyquant/indicators/rsi_divergence.py
+ezyquant/indicators/ta.py
+ezyquant/indicators/zigzag.py
 tests/test_creator.py
-tests/test_indicators.py
 tests/test_reader.py
 tests/test_test_utils.py
 tests/test_utils.py
```

### Comparing `ezyquant-0.7.2/setup.py` & `ezyquant-0.7.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         "pandas>=1.5",
         "sqlalchemy>=2.0",
         "psycopg2-binary>=2.9",
         "ta>=0.10",
         "XlsxWriter>=3.0",
         "typing_extensions>=4.4",
         "quantstats>=0.0",
-        "zigzag==0.2.2",
     ],
     license="The MIT License (MIT)",
     classifiers=[
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ezyquant-0.7.2/tests/test_creator.py` & `ezyquant-0.7.3/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/tests/test_reader.py` & `ezyquant-0.7.3/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/tests/test_test_utils.py` & `ezyquant-0.7.3/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.2/tests/test_utils.py` & `ezyquant-0.7.3/tests/test_utils.py`

 * *Files identical despite different names*

