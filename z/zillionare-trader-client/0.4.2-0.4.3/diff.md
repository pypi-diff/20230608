# Comparing `tmp/zillionare_trader_client-0.4.2.tar.gz` & `tmp/zillionare_trader_client-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare_trader_client-0.4.2.tar", max compression
+gzip compressed data, was "zillionare_trader_client-0.4.3.tar", max compression
```

## Comparing `zillionare_trader_client-0.4.2.tar` & `zillionare_trader_client-0.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.2/LICENSE
--rw-r--r--   0        0        0     1752 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.2/README.md
--rw-r--r--   0        0        0     2513 2023-05-09 11:52:53.635475 zillionare_trader_client-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6831 2023-05-05 12:28:42.792689 zillionare_trader_client-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-04 02:55:06.817294 zillionare_trader_client-0.4.2/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.2/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0    56389 2023-05-05 09:15:16.952210 zillionare_trader_client-0.4.2/tests/data/calendar.json
--rw-r--r--   0        0        0      881 2023-05-05 09:05:10.906134 zillionare_trader_client-0.4.2/tests/data/defaults.yaml
--rw-r--r--   0        0        0      931 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.2/tests/data/hljh_1d.csv
--rw-r--r--   0        0        0   214231 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/hljh_1m.csv
--rw-r--r--   0        0        0      303 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/hljh_limits.csv
--rw-r--r--   0        0        0      902 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/limits.csv
--rw-r--r--   0        0        0     1078 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/limits.pkl
--rw-r--r--   0        0        0      438 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/readme.md
--rw-r--r--   0        0        0      896 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/tyst_1d.csv
--rw-r--r--   0        0        0   207056 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/tyst_1m.csv
--rw-r--r--   0        0        0      315 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/tyst_limits.csv
--rw-r--r--   0        0        0     1339 2023-05-05 09:31:56.254023 zillionare_trader_client-0.4.2/tests/helper.py
--rw-r--r--   0        0        0     4117 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/performance.py
--rw-r--r--   0        0        0    10473 2023-05-09 11:06:48.224979 zillionare_trader_client-0.4.2/tests/test_traderclient.py
--rw-r--r--   0        0        0     1620 2023-05-05 12:07:44.696724 zillionare_trader_client-0.4.2/tests/test_transport.py
--rw-r--r--   0        0        0      183 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/cli.py
--rw-r--r--   0        0        0    28929 2023-05-09 11:52:11.899518 zillionare_trader_client-0.4.2/traderclient/client.py
--rw-r--r--   0        0        0      487 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/datatypes.py
--rw-r--r--   0        0        0     6983 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/demo.py
--rw-r--r--   0        0        0      350 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/errors.py
--rw-r--r--   0        0        0     3750 2023-05-06 06:54:02.837816 zillionare_trader_client-0.4.2/traderclient/transport.py
--rw-r--r--   0        0        0     1572 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/utils.py
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 zillionare_trader_client-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1752 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.3/README.md
+-rw-r--r--   0        0        0     2513 2023-06-08 07:34:22.543668 zillionare_trader_client-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6831 2023-05-05 12:28:42.792689 zillionare_trader_client-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-04 02:55:06.817294 zillionare_trader_client-0.4.3/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.3/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0    56389 2023-05-05 09:15:16.952210 zillionare_trader_client-0.4.3/tests/data/calendar.json
+-rw-r--r--   0        0        0      881 2023-05-05 09:05:10.906134 zillionare_trader_client-0.4.3/tests/data/defaults.yaml
+-rw-r--r--   0        0        0      931 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.3/tests/data/hljh_1d.csv
+-rw-r--r--   0        0        0   214231 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/data/hljh_1m.csv
+-rw-r--r--   0        0        0      303 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/data/hljh_limits.csv
+-rw-r--r--   0        0        0      902 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/data/limits.csv
+-rw-r--r--   0        0        0     1078 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/data/limits.pkl
+-rw-r--r--   0        0        0      438 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/data/readme.md
+-rw-r--r--   0        0        0      896 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/data/tyst_1d.csv
+-rw-r--r--   0        0        0   207056 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/data/tyst_1m.csv
+-rw-r--r--   0        0        0      315 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/data/tyst_limits.csv
+-rw-r--r--   0        0        0     1339 2023-05-05 09:31:56.254023 zillionare_trader_client-0.4.3/tests/helper.py
+-rw-r--r--   0        0        0     4117 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.3/tests/performance.py
+-rw-r--r--   0        0        0    10511 2023-06-08 08:37:36.912651 zillionare_trader_client-0.4.3/tests/test_traderclient.py
+-rw-r--r--   0        0        0     1620 2023-05-05 12:07:44.696724 zillionare_trader_client-0.4.3/tests/test_transport.py
+-rw-r--r--   0        0        0      183 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.3/traderclient/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.3/traderclient/cli.py
+-rw-r--r--   0        0        0    28882 2023-06-08 08:39:48.911158 zillionare_trader_client-0.4.3/traderclient/client.py
+-rw-r--r--   0        0        0      487 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.3/traderclient/datatypes.py
+-rw-r--r--   0        0        0     6983 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.3/traderclient/demo.py
+-rw-r--r--   0        0        0      350 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.3/traderclient/errors.py
+-rw-r--r--   0        0        0     3750 2023-05-06 06:54:02.837816 zillionare_trader_client-0.4.3/traderclient/transport.py
+-rw-r--r--   0        0        0     1572 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.3/traderclient/utils.py
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 zillionare_trader_client-0.4.3/PKG-INFO
```

### Comparing `zillionare_trader_client-0.4.2/LICENSE` & `zillionare_trader_client-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/README.md` & `zillionare_trader_client-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/pyproject.toml` & `zillionare_trader_client-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "zillionare-trader-client"
-version = "0.4.2"
+version = "0.4.3"
 homepage = "https://github.com/zillionare/trader-client"
 description = "Zillionare Trader Client"
 authors = ["Aaron Yang <code@jieyu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `zillionare_trader_client-0.4.2/tests/__init__.py` & `zillionare_trader_client-0.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/bars_1d.pkl` & `zillionare_trader_client-0.4.3/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/bars_1m.pkl` & `zillionare_trader_client-0.4.3/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/calendar.json` & `zillionare_trader_client-0.4.3/tests/data/calendar.json`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/defaults.yaml` & `zillionare_trader_client-0.4.3/tests/data/defaults.yaml`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/hljh_1d.csv` & `zillionare_trader_client-0.4.3/tests/data/hljh_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/hljh_1m.csv` & `zillionare_trader_client-0.4.3/tests/data/hljh_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/limits.csv` & `zillionare_trader_client-0.4.3/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/limits.pkl` & `zillionare_trader_client-0.4.3/tests/data/limits.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/tyst_1d.csv` & `zillionare_trader_client-0.4.3/tests/data/tyst_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/data/tyst_1m.csv` & `zillionare_trader_client-0.4.3/tests/data/tyst_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/helper.py` & `zillionare_trader_client-0.4.3/tests/helper.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/performance.py` & `zillionare_trader_client-0.4.3/tests/performance.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/tests/test_traderclient.py` & `zillionare_trader_client-0.4.3/tests/test_traderclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,28 +109,28 @@
         self.assertAlmostEqual(balance["market_value"], 4750, 2)
         self.assertAlmostEqual(balance["assets"], 1000039.528, 2)
         self.assertAlmostEqual(balance["pnl"], 39.5289, 2)
         self.assertAlmostEqual(balance["ppnl"], 39.5289 / 1_000_000, 2)
 
     def test_positions(self):
         # this will test available_shares too
-        positions = self.client.get_positions()
+        positions = self.client.positions(datetime.date(2022, 3, 1))
         self.assertEqual(0, positions.size)
 
         self.client.buy(
             "002537.XSHE", 10, 500, order_time=datetime.datetime(2022, 3, 1, 10, 4)
         )
 
-        positions = self.client.get_positions()
+        positions = self.client.positions(datetime.date(2022, 3, 1))
         self.assertListEqual(positions["security"].tolist(), ["002537.XSHE"])
         self.assertListEqual(positions["shares"].tolist(), [500])
         self.assertListEqual(positions["sellable"].tolist(), [0])
         np.testing.assert_array_almost_equal(positions["price"], [9.42], decimal=2)
 
-        positions = self.client.get_positions(datetime.date(2022, 3, 7))
+        positions = self.client.positions(datetime.date(2022, 3, 7))
         self.assertListEqual(positions["security"].tolist(), ["002537.XSHE"])
         self.assertListEqual(positions["shares"].tolist(), [500])
         self.assertListEqual(positions["sellable"].tolist(), [500])
         np.testing.assert_array_almost_equal(positions["price"], [9.42], decimal=2)
 
         # last_trade day is still 2022, 3, 1, so the available_shares is 0
         r = self.client.available_shares("002537.XSHE", datetime.date(2022, 3, 1))
```

### Comparing `zillionare_trader_client-0.4.2/tests/test_transport.py` & `zillionare_trader_client-0.4.3/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/traderclient/client.py` & `zillionare_trader_client-0.4.3/traderclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,14 @@
             if start is None or end is None:
                 raise ValueError("start and end must be specified in backtest mode")
 
             self._start_backtest(acct, token, self._principal, commission, start, end)
 
         self._is_dirty = False
         self._cash = None
-        self._positions = None
 
     def _cmd_url(self, cmd: str) -> str:
         return f"{self._url}/{cmd}"
 
     def _start_backtest(
         self,
         acct: str,
@@ -175,30 +174,34 @@
         if self._is_backtest:
             return self._principal
 
         url = self._cmd_url("info")
         r = get(url, headers=self.headers)
         return r.get("principal")
 
-    def get_positions(self, dt: Optional[datetime.date] = None) -> np.ndarray:
+    def positions(self, dt: Optional[datetime.date] = None) -> np.ndarray:
         """取该子账户当前持仓信息
 
         Warning:
             在回测模式下，持仓信息不包含alias字段
 
         Args:
             dt: 指定日期，默认为None，表示取当前日期（最新）的持仓信息，trade server暂不支持此参数
         Returns:
             np.ndarray: dtype为[position_dtype](https://zillionare.github.io/backtesting/0.3.2/api/trade/#backtest.trade.datatypes.position_dtype)的numpy structured array
         """
-        url = self._cmd_url("positions")
-
-        r = get(url, params={"date": dt}, headers=self.headers)
+        if self._is_backtest and dt is None:
+            raise ValueError("`dt` is required under backtest mode")
 
-        return r
+        url = self._cmd_url("positions")
+        return get(
+            url,
+            params={"date": dt.isoformat() if dt is not None else None},
+            headers=self.headers,
+        )
 
     def available_shares(
         self, security: str, dt: Optional[datetime.date] = None
     ) -> float:
         """返回某支股票在`dt`日的可售数量
 
         Args:
@@ -207,19 +210,17 @@
 
         Returns:
             float: 指定股票在`dt`日可卖数量，无可卖即为0
         """
         if self._is_backtest and dt is None:
             raise ValueError("`dt` is required under backtest!")
 
-        if self._is_dirty or self._positions is None:
-            self._positions = self.get_positions(dt)
-            # 此时持仓虽然同步了，但其它数据，比如cash并未同步，所以不能更改_is_dirty状态
+        positions = self.positions(dt)
 
-        found = self._positions[self._positions["security"] == security]
+        found = positions[positions["security"] == security]
         if found.size == 1:
             return found["sellable"][0].item()
         elif found.size == 0:
             return 0
         else:
             logger.warning("found more than one position entry in response: %s", found)
             raise ValueError(f"found more than one position entry in response: {found}")
@@ -430,14 +431,15 @@
             if order_time is None:
                 raise ValueError("order_time is required in backtest mode")
 
             _order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
             parameters["order_time"] = _order_time
 
         self._is_dirty = True
+
         r = post_json(url, params=parameters, headers=self.headers)
 
         for key in ("time", "created_at", "recv_at"):
             if key in r:
                 r[key] = arrow.get(r[key]).naive
 
         return r
@@ -539,14 +541,15 @@
             if order_time is None:
                 raise ValueError("order_time is required in backtest mode")
 
             _order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
             parameters["order_time"] = _order_time
 
         self._is_dirty = True
+
         r = post_json(url, params=parameters, headers=self.headers)
         for key in ("time", "created_at", "recv_at"):
             if key in r:
                 r[key] = arrow.get(r[key]).naive
 
         return r
 
@@ -661,14 +664,15 @@
         if percent <= 0 or percent > 1:
             raise ValueError("percent should between [0, 1]")
 
         url = self._cmd_url("sell_all")
         parameters = {"percent": percent, "timeout": timeout}
 
         self._is_dirty = True
+
         return post_json(url, params=parameters, headers=self.headers)
 
     def metrics(
         self,
         start: Optional[datetime.date] = None,
         end: Optional[datetime.date] = None,
         baseline: Optional[str] = None,
```

### Comparing `zillionare_trader_client-0.4.2/traderclient/demo.py` & `zillionare_trader_client-0.4.3/traderclient/demo.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/traderclient/transport.py` & `zillionare_trader_client-0.4.3/traderclient/transport.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/traderclient/utils.py` & `zillionare_trader_client-0.4.3/traderclient/utils.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.2/PKG-INFO` & `zillionare_trader_client-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-trader-client
-Version: 0.4.2
+Version: 0.4.3
 Summary: Zillionare Trader Client
 Home-page: https://github.com/zillionare/trader-client
 License: MIT
 Author: Aaron Yang
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
 Classifier: Development Status :: 2 - Pre-Alpha
```

