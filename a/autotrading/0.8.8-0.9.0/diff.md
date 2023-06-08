# Comparing `tmp/autotrading-0.8.8.tar.gz` & `tmp/autotrading-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrading-0.8.8.tar", last modified: Wed May 31 03:04:04 2023, max compression
+gzip compressed data, was "autotrading-0.9.0.tar", last modified: Wed Jun  7 08:29:23 2023, max compression
```

## Comparing `autotrading-0.8.8.tar` & `autotrading-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 03:04:04.378548 autotrading-0.8.8/
--rw-rw-rw-   0        0        0      311 2023-05-31 03:04:04.378548 autotrading-0.8.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 03:04:04.373230 autotrading-0.8.8/autotrader/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 autotrading-0.8.8/autotrader/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0     2692 2023-05-30 11:40:44.000000 autotrading-0.8.8/autotrader/__init__.py
--rw-rw-rw-   0        0        0   136609 2023-05-31 03:03:29.000000 autotrading-0.8.8/autotrader/autotradingfunctions.py
--rw-rw-rw-   0        0        0     7212 2023-05-31 03:03:29.000000 autotrading-0.8.8/autotrader/blackscholes.py
--rw-rw-rw-   0        0        0    21000 2023-05-30 10:12:37.000000 autotrading-0.8.8/autotrader/datamodule.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 autotrading-0.8.8/autotrader/discord_bot.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 autotrading-0.8.8/autotrader/nsefunctions.py
--rw-rw-rw-   0        0        0    14140 2023-05-30 10:07:04.000000 autotrading-0.8.8/autotrader/strategies.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:04:04.377265 autotrading-0.8.8/autotrading.egg-info/
--rw-rw-rw-   0        0        0      311 2023-05-31 03:04:04.000000 autotrading-0.8.8/autotrading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-05-31 03:04:04.000000 autotrading-0.8.8/autotrading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 03:04:04.000000 autotrading-0.8.8/autotrading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      752 2023-05-31 03:04:04.000000 autotrading-0.8.8/autotrading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 03:04:04.000000 autotrading-0.8.8/autotrading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 autotrading-0.8.8/pyproject.toml
--rw-rw-rw-   0        0        0     1201 2023-05-31 03:04:04.379571 autotrading-0.8.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 08:29:23.272335 autotrading-0.9.0/
+-rw-rw-rw-   0        0        0      311 2023-06-07 08:29:23.272335 autotrading-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2023-06-06 16:33:28.000000 autotrading-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 08:29:23.265067 autotrading-0.9.0/autotrader/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 autotrading-0.9.0/autotrader/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0     2697 2023-06-06 15:41:26.000000 autotrading-0.9.0/autotrader/__init__.py
+-rw-rw-rw-   0        0        0   157720 2023-06-07 08:25:50.000000 autotrading-0.9.0/autotrader/autotradingfunctions.py
+-rw-rw-rw-   0        0        0     8133 2023-06-07 07:39:33.000000 autotrading-0.9.0/autotrader/blackscholes.py
+-rw-rw-rw-   0        0        0    24244 2023-06-06 15:50:32.000000 autotrading-0.9.0/autotrader/datamodule.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 autotrading-0.9.0/autotrader/discord_bot.py
+-rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 autotrading-0.9.0/autotrader/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 autotrading-0.9.0/autotrader/nsefunctions.py
+-rw-rw-rw-   0        0        0    16085 2023-06-07 08:25:50.000000 autotrading-0.9.0/autotrader/strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:29:23.271337 autotrading-0.9.0/autotrading.egg-info/
+-rw-rw-rw-   0        0        0      311 2023-06-07 08:29:23.000000 autotrading-0.9.0/autotrading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-06-07 08:29:23.000000 autotrading-0.9.0/autotrading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:29:23.000000 autotrading-0.9.0/autotrading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      787 2023-06-07 08:29:23.000000 autotrading-0.9.0/autotrading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 08:29:23.000000 autotrading-0.9.0/autotrading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 autotrading-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1240 2023-06-07 08:29:23.273331 autotrading-0.9.0/setup.cfg
```

### Comparing `autotrading-0.8.8/autotrader/SmartWebSocketV2.py` & `autotrading-0.9.0/autotrader/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `autotrading-0.8.8/autotrader/__init__.py` & `autotrading-0.9.0/autotrader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         response = requests.get(freeze_qty_url, timeout=10)  # Set the timeout value
         response.raise_for_status()  # Raise an exception if the response contains an HTTP error status
         df = pd.read_excel(response.content)
         df.columns = df.columns.str.strip()
         df["SYMBOL"] = df["SYMBOL"].str.strip()
     except Exception as e:
         print(f"Error in fetching qtyfreeze.xls: {e}")
-        df = pd.read_csv("autotrader/qtyfreeze.csv")
+        df = pd.read_csv("autotrader/info/qtyfreeze.csv")
         df.columns = df.columns.str.strip()
         df["SYMBOL"] = df["SYMBOL"].str.strip()
     return df
 
 
 def create_logger(name):
     logger = logging.getLogger(name)
```

### Comparing `autotrading-0.8.8/autotrader/autotradingfunctions.py` & `autotrading-0.9.0/autotrader/autotradingfunctions.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests
 import json
 from smartapi import SmartConnect
 from smartapi.smartExceptions import DataException
 import pyotp
 from threading import Thread
 from autotrader.SmartWebSocketV2 import SmartWebSocketV2
-from autotrader import scrips, holidays, symbol_df, logger, blackscholes as bs
+from autotrader import scrips, holidays, symbol_df, logger, blackscholes as bs, datamodule as dm
 from collections import defaultdict
 import yfinance as yf
 from fuzzywuzzy import process
 import re
 import logging
 import functools
 import itertools
@@ -55,15 +55,15 @@
         self.price_dict = {}
         self.symbol_option_chains = {}
         self.last_update_time = None
         self.iv_log = defaultdict(lambda: defaultdict(dict))
         self.webhook_url = webhook_url
         self.index_option_chains_subscribed = []
         self.correlation_id = correlation_id
-        self.finnifty_index = Index("FINNIFTY", spot_future_rate=0.01)
+        self.finnifty_index = Index("FINNIFTY")
 
     def start_websocket(self):
         def on_open(wsapp):
             self.subscribe_tokens()
 
         # Assign the callbacks.
         self.on_open = on_open
@@ -183,14 +183,15 @@
     def update_option_chain(
         self,
         sleep_time=5,
         exit_time=(15, 30),
         process_iv_log=True,
         market_depth=True,
         calculate_iv=True,
+        stop_iv_calculation_hours=3,
         n_values=100,
         iv_threshold=1.1,
     ):
         while currenttime().time() < time(*exit_time):
             parsed_dict = self.parse_price_dict()
             indices = self.index_option_chains_subscribed
             for index in indices:
@@ -203,28 +204,30 @@
                         expiry,
                         parsed_dict,
                         market_depth,
                         process_iv_log,
                         calculate_iv,
                         n_values,
                         iv_threshold,
+                        stop_iv_calculation_hours,
                     )
 
             sleep(sleep_time)
 
     def build_option_chain(
         self,
         index: str,
         expiry: str,
         parsed_dict: dict,
         market_depth,
         process_iv_log,
         calculate_iv,
         n_values,
         iv_threshold,
+        stop_iv_calculation_hours=3,
     ):
         instrument_info = parsed_dict[index]
         spot = instrument_info["ltp"]
 
         for symbol, info in parsed_dict.items():
             if symbol.startswith(index) and "CE" in symbol and expiry in symbol:
                 strike = float(parse_symbol(symbol)[2])
@@ -239,15 +242,15 @@
                 self.symbol_option_chains[index][expiry][strike][
                     "put_price"
                 ] = put_price
                 self.symbol_option_chains[index].underlying_price = spot
 
                 if calculate_iv:
                     time_to_expiry = timetoexpiry(expiry)
-                    if time_to_expiry < 3 / (
+                    if time_to_expiry < stop_iv_calculation_hours / (
                         24 * 365
                     ):  # If time to expiry is less than 3 hours stop calculating iv
                         continue
                     call_iv, put_iv, avg_iv = straddle_iv(
                         call_price, put_price, spot, strike, time_to_expiry
                     )
                     self.symbol_option_chains[index][expiry][strike][
@@ -327,25 +330,25 @@
             index, expiry, strike, n_values
         )
 
         running_avg_call_iv = sum(call_ivs) / len(call_ivs) if call_ivs else None
         running_avg_put_iv = sum(put_ivs) / len(put_ivs) if put_ivs else None
         running_avg_total_iv = sum(total_ivs) / len(total_ivs) if total_ivs else None
 
-        self.check_and_notify(
+        self.check_and_notify_iv_spike(
             call_iv,
             running_avg_call_iv,
             "Call",
             index,
             spot,
             strike,
             expiry,
             iv_threshold,
         )
-        self.check_and_notify(
+        self.check_and_notify_iv_spike(
             put_iv, running_avg_put_iv, "Put", index, spot, strike, expiry, iv_threshold
         )
 
         self.symbol_option_chains[index][expiry][strike].update(
             {
                 "running_avg_call_iv": running_avg_call_iv,
                 "running_avg_put_iv": running_avg_put_iv,
@@ -358,15 +361,15 @@
         put_ivs = self.iv_log[index][expiry][strike]["put_ivs"][-n_values:]
         total_ivs = self.iv_log[index][expiry][strike]["total_ivs"][-n_values:]
         call_ivs = [*filter(lambda x: x is not None, call_ivs)]
         put_ivs = [*filter(lambda x: x is not None, put_ivs)]
         total_ivs = [*filter(lambda x: x is not None, total_ivs)]
         return call_ivs, put_ivs, total_ivs
 
-    def check_and_notify(
+    def check_and_notify_iv_spike(
         self, iv, running_avg_iv, iv_type, idx, idx_price, K, exp, iv_hurdle
     ):
         not_in_the_money_by_100 = False
 
         if iv_type == "Call":
             not_in_the_money_by_100 = idx_price <= K - 100
         elif iv_type == "Put":
@@ -478,24 +481,24 @@
 
     def fetch_ltp(self):
         return fetchltp("NFO", self.symbol, self.token)
 
     def fetch_symbol_token(self):
         return self.symbol, self.token
 
-    def place_order(self, transaction_type, quantity_in_lots, price="LIMIT"):
+    def place_order(self, transaction_type, quantity_in_lots, price="LIMIT", order_tag=""):
         if price.upper() == "LIMIT":
             price = self.fetch_ltp()
             modifier = 1.05 if transaction_type.upper() == "BUY" else 0.95
             price = price * modifier
         spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
         order_ids = []
         for qty in spliced_orders:
-            order_id = placeorder(
-                self.symbol, self.token, qty * self.lot_size, transaction_type, price
+            order_id = place_order(
+                self.symbol, self.token, qty * self.lot_size, transaction_type, price, order_tag=order_tag
             )
             order_ids.append(order_id)
         self.order_id_log.append(order_ids)
         return order_ids
 
 
 class Strangle:
@@ -505,14 +508,17 @@
         self.call_strike = self.call_option.strike
         self.put_strike = self.put_option.strike
         self.underlying = underlying
         self.underlying_exchange = "NFO" if self.underlying == "FINNIFTY" else "NSE"
         self.expiry = expiry
         self.call_symbol, self.call_token = self.call_option.fetch_symbol_token()
         self.put_symbol, self.put_token = self.put_option.fetch_symbol_token()
+        self.freeze_qty_in_shares = self.call_option.freeze_qty_in_shares
+        self.freeze_qty_in_lots = self.call_option.freeze_qty_in_lots
+        self.lot_size = self.call_option.lot_size
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}(callstrike={self.call_option.strike}, putstrike={self.put_option.strike}, "
             f"underlying={self.underlying}, expiry={self.expiry})"
         )
 
@@ -524,15 +530,15 @@
             "NFO", self.put_symbol, self.put_token
         )
 
     def underlying_ltp(self):
         symbol, token = fetch_symbol_token(self.underlying)
         return fetchltp(self.underlying_exchange, symbol, token)
 
-    def iv(self):
+    def ivs(self):
         return strangle_iv(
             *self.fetch_ltp(),
             self.underlying_ltp(),
             self.call_strike,
             self.put_strike,
             timeleft=timetoexpiry(self.expiry),
         )
@@ -542,26 +548,43 @@
             "NFO", self.call_symbol, self.call_token
         ), fetchltp("NFO", self.put_symbol, self.put_token)
         return call_ltp + put_ltp
 
     def fetch_symbol_token(self):
         return self.call_symbol, self.call_token, self.put_symbol, self.put_token
 
-    def place_order(self, transaction_type, quantity_in_lots, prices="LIMIT"):
+    def place_order(self, transaction_type, quantity_in_lots, prices="LIMIT", order_tag=""):
         if isinstance(prices, (tuple, list, np.ndarray)):
             call_price, put_price = prices
-        else:
+        elif prices.upper() == "LIMIT":
+            call_price, put_price = self.fetch_ltp()
+            modifier = 1.05 if transaction_type.upper() == "BUY" else 0.95
+            call_price, put_price = call_price * modifier, put_price * modifier
+        elif prices.upper() == "MARKET":
             call_price = put_price = prices
+        else:
+            raise ValueError("Prices must be either 'LIMIT' or 'MARKET' or a tuple of prices")
 
-        call_order_ids = self.call_option.place_order(
-            transaction_type, quantity_in_lots, call_price
-        )
-        put_order_ids = self.put_option.place_order(
-            transaction_type, quantity_in_lots, put_price
-        )
+        spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
+        call_order_ids = []
+        put_order_ids = []
+        for qty in spliced_orders:
+            call_order_id = place_order(
+                self.call_symbol,
+                self.call_token,
+                qty * self.lot_size,
+                transaction_type,
+                call_price,
+                order_tag=order_tag
+            )
+            put_order_id = place_order(
+                self.put_symbol, self.put_token, qty * self.lot_size, transaction_type, put_price, order_tag=order_tag
+            )
+            call_order_ids.append(call_order_id)
+            put_order_ids.append(put_order_id)
         return call_order_ids, put_order_ids
 
 
 class Straddle(Strangle):
     def __init__(self, strike, underlying, expiry):
         super().__init__(strike, strike, underlying, expiry)
 
@@ -750,27 +773,27 @@
             ]
             cancel_pending_orders(open_order_ids)
 
             # Reversing the trade which got executed
             for i, status in enumerate(statuses):
                 if status == "complete":
                     if i == 0:
-                        placeorder(
-                            call_buy_token, call_buy_symbol, qty, "SELL", "MARKET"
+                        place_order(
+                            call_buy_symbol, call_buy_token, qty, "SELL", "MARKET"
                         )
                     elif i == 1:
-                        placeorder(
-                            put_sell_token, put_sell_symbol, qty, "BUY", "MARKET"
+                        place_order(
+                            put_sell_symbol, put_sell_token, qty, "BUY", "MARKET"
                         )
                     elif i == 2:
-                        placeorder(
-                            call_sell_token, call_sell_symbol, qty, "BUY", "MARKET"
+                        place_order(
+                            call_sell_symbol, call_sell_token, qty, "BUY", "MARKET"
                         )
                     elif i == 3:
-                        placeorder(put_buy_token, put_buy_symbol, qty, "SELL", "MARKET")
+                        place_order(put_buy_symbol, put_buy_token, qty, "SELL", "MARKET")
             logger.info(
                 f"Order cancelled and reversed for {index} {expiry} {qty} Buy {buy_strike} Sell {sell_strike}"
             )
             self.unsuccessful_trades += 1
         elif all(statuses == "complete"):
             self.successful_trades += 1
             logger.info(
@@ -862,22 +885,22 @@
             freeze_qty_in_lots = freeze_qty / self.lot_size
             return int(freeze_qty_in_lots)
         except requests.exceptions.Timeout as e:
             notifier(
                 f"Timeout error in fetching freeze limit for {self.name}: {e}",
                 self.webhook_url,
             )
-            freeze_qty_in_lots = 30
+            freeze_qty_in_lots = 20
             return int(freeze_qty_in_lots)
         except requests.exceptions.HTTPError as e:
             notifier(
                 f"HTTP error in fetching freeze limit for {self.name}: {e}",
                 self.webhook_url,
             )
-            freeze_qty_in_lots = 30
+            freeze_qty_in_lots = 20
             return int(freeze_qty_in_lots)
         except Exception as e:
             notifier(
                 f"Error in fetching freeze limit for {self.name}: {e}", self.webhook_url
             )
             freeze_qty_in_lots = 20
             return freeze_qty_in_lots
@@ -954,15 +977,15 @@
         }
         expiry = expiry_dict[expiry]
         price = self.fetch_ltp()
         atm_strike = findstrike(price, self.base)
         atm_straddle = Straddle(atm_strike, self.name, expiry)
         call_price, put_price = atm_straddle.fetch_ltp()
         total_price = call_price + put_price
-        call_iv, put_iv, avg_iv = atm_straddle.iv()
+        call_iv, put_iv, avg_iv = atm_straddle.ivs()
         return {
             "underlying_price": price,
             "strike": atm_strike,
             "call_price": call_price,
             "put_price": put_price,
             "total_price": total_price,
             "call_iv": call_iv,
@@ -983,15 +1006,15 @@
         call_strike = price * (1 + strike_offset)
         put_strike = price * (1 - strike_offset)
         call_strike = findstrike(call_strike, self.base)
         put_strike = findstrike(put_strike, self.base)
         otm_strangle = Strangle(call_strike, put_strike, self.name, expiry)
         call_price, put_price = otm_strangle.fetch_ltp()
         total_price = call_price + put_price
-        call_iv, put_iv, avg_iv = otm_strangle.iv()
+        call_iv, put_iv, avg_iv = otm_strangle.ivs()
         return {
             "underlying_price": price,
             "call_strike": call_strike,
             "put_strike": put_strike,
             "call_price": call_price,
             "put_price": put_price,
             "total_price": total_price,
@@ -1008,20 +1031,39 @@
             self.available_straddle_strikes = available_strikes
         return available_strikes
 
     def get_constituents(self, cutoff_pct=101):
         tickers, weights = get_index_constituents(self.name, cutoff_pct)
         return tickers, weights
 
-    def log_order(self, strike, expiry, buy_or_sell, call_price, put_price, order_tag):
+    def log_combined_order(
+            self, strike=None,
+            call_strike=None,
+            put_strike=None,
+            expiry=None,
+            buy_or_sell=None,
+            call_price=None,
+            put_price=None,
+            order_tag=None):
+
+        if strike is None and (call_strike is None or put_strike is None):
+            raise Exception("Strike and call/put strike both not provided")
+
+        if strike is not None and (call_strike is not None or put_strike is not None):
+            raise Exception("Strike and call/put strike both provided")
+
+        if strike is not None:
+            call_strike = strike
+            put_strike = strike
+
         dict_format = {
             "Date": currenttime().strftime("%d-%m-%Y %H:%M:%S"),
             "Index": self.name,
-            "Put Strike": strike,
-            "Call Strike": strike,
+            "Call Strike": call_strike,
+            "Put Strike": put_strike,
             "Expiry": expiry,
             "Action Type": buy_or_sell,
             "Call Price": call_price,
             "Put Price": put_price,
             "Total Price": call_price + put_price,
             "Tag": order_tag,
         }
@@ -1082,36 +1124,36 @@
         call_symbol, call_token = fetch_symbol_token(
             self.name, expiry, call_strike, "CE"
         )
         put_symbol, put_token = fetch_symbol_token(self.name, expiry, put_strike, "PE")
         call_price = fetchltp("NFO", call_symbol, call_token)
         put_price = fetchltp("NFO", put_symbol, put_token)
 
-        limit_price_extender = 1.1 if buy_or_sell == "BUY" else 0.9
+        limit_price_extender = 1.05 if buy_or_sell == "BUY" else 0.95
 
         spliced_orders = self.splice_orders(quantity_in_lots)
 
         call_order_id_list = []
         put_order_id_list = []
         for quantity in spliced_orders:
-            call_order_id = placeorder(
+            call_order_id = place_order(
                 call_symbol,
                 call_token,
                 quantity * self.lot_size,
                 buy_or_sell,
                 call_price * limit_price_extender,
-                ordertag=order_tag,
+                order_tag=order_tag,
             )
-            put_order_id = placeorder(
+            put_order_id = place_order(
                 put_symbol,
                 put_token,
                 quantity * self.lot_size,
                 buy_or_sell,
                 put_price * limit_price_extender,
-                ordertag=order_tag,
+                order_tag=order_tag,
             )
             call_order_id_list.append(call_order_id)
             put_order_id_list.append(put_order_id)
             sleep(0.3)
 
         orderbook = fetch_book("orderbook")
 
@@ -1216,18 +1258,18 @@
         put_action = "SELL" if buy_or_sell == "BUY" else "BUY"
 
         order_ids_call = []
         order_ids_put = []
         for quantity in spliced_orders:
             quantity_in_shares = quantity * self.lot_size
 
-            order_id_call = placeorder(
+            order_id_call = place_order(
                 call_symbol, call_token, quantity_in_shares, call_action, call_price
             )
-            order_id_put = placeorder(
+            order_id_put = place_order(
                 put_symbol, put_token, quantity_in_shares, put_action, put_price
             )
             if check_status:
                 order_ids_call.append(order_id_call)
                 order_ids_put.append(order_id_put)
 
         if check_status:
@@ -1428,56 +1470,62 @@
             strike_offset (float): Strike offset from the current strike.
             iv_threshold (float): IV threshold compared to vix.
             take_avg_price (bool): Take average price of the index over 5m timeframes.
         """
 
         def load_data():
             try:
-                with open("positions.json", "r") as f:
+                with open(f"{obj.userId}_overnight_positions.json", "r") as f:
                     data = json.load(f)
                     return data
             except FileNotFoundError:
-                data = {"NIFTY": None, "BANKNIFTY": None}
+                data = {}
                 notifier(
-                    "No positions found for OSS. Creating new file.", self.webhook_url
+                    "No positions found for overnight straddle. Creating new file.", self.webhook_url
                 )
-                with open("positions.json", "w") as f:
+                with open(f"{obj.userId}_overnight_positions.json", "w") as f:
                     json.dump(data, f)
                 return data
             except Exception as e:
-                notifier(f"Error while reading positions.json: {e}", self.webhook_url)
+                notifier(f"Error while reading overnight_positions.json: {e}", self.webhook_url)
+                logger.error(f"Error while reading positions.json", exc_info=(type(e), e, e.__traceback__))
                 raise Exception("Error while reading positions.json")
 
         def save_data(data):
-            with open("positions.json", "w") as f:
+            with open(f"{obj.userId}_overnight_positions.json", "w") as f:
                 json.dump(data, f)
 
         avg_ltp = None
         if take_avg_price:
             if currenttime().time() < time(15, 00):
                 notifier(
-                    "Cannot take avg price before 3pm. Try running the strategy after 3pm",
+                    f"{self.name} Cannot take avg price before 3pm. Try running the strategy after 3pm",
                     self.webhook_url,
                 )
                 raise Exception(
                     "Cannot take avg price before 3pm. Try running the strategy after 3pm"
                 )
             notifier(
-                "Taking average price of the index over 5m timeframes.",
+                f"{self.name} Taking average price of the index over 5m timeframes.",
                 self.webhook_url,
             )
-            price_list = []
+            price_list = [self.fetch_ltp()]
             while currenttime().time() < time(15, 28):
-                nifty_ltp = self.fetch_ltp()
-                price_list.append(nifty_ltp)
+                _ltp = self.fetch_ltp()
+                price_list.append(_ltp)
                 sleep(60)
             avg_ltp = np.mean(price_list)
 
+        # Assigning vix
         vix = yf.Ticker("^INDIAVIX")
         vix = vix.fast_info["last_price"]
+        if self.name in ["FINNIFTY", "BANKNIFTY"]:
+            beta = dm.get_summary_ratio(self.name, 'NIFTY')  # beta of the index vs nifty since vix is of nifty
+            beta = 1.3 if beta is None else beta
+            vix = vix * beta
 
         order_tag = "Overnight Short Straddle"
 
         weekend_in_expiry = check_for_weekend(self.current_expiry)
         ltp = avg_ltp if avg_ltp else self.fetch_ltp()
         sell_strike = findstrike(ltp * strike_offset, self.base)
         call_ltp, put_ltp = fetch_straddle_price(
@@ -1485,112 +1533,93 @@
         )
         call_iv, put_iv, iv = straddle_iv(
             call_ltp, put_ltp, ltp, sell_strike, timetoexpiry(self.current_expiry)
         )
         iv = iv * 100
 
         # This if-clause checks how far the expiry is
-        if (
-            timetoexpiry(self.current_expiry, effective_time=True, in_days=True) > 4
-        ) or weekend_in_expiry:  # far from expiry
+        if weekend_in_expiry:  # far from expiry
 
             if iv < vix * iv_threshold:
                 notifier(
-                    f"IV is too low compared to VIX - IV: {iv}, Vix: {vix}.",
+                    f"{self.name} IV is too low compared to VIX - IV: {iv}, Vix: {vix}.",
                     self.webhook_url,
                 )
                 return
             else:
                 notifier(
-                    f"IV is fine compared to VIX - IV: {iv}, Vix: {vix}.", self.webhook_url
+                    f"{self.name} IV is fine compared to VIX - IV: {iv}, Vix: {vix}.", self.webhook_url
                 )
         elif (
             timetoexpiry(self.current_expiry, effective_time=True, in_days=True) < 2
         ):  # only exit
             sell_strike = None
+            notifier(f"{self.name} Only exiting current position. IV: {iv}, Vix: {vix}.", self.webhook_url)
         else:
             notifier(
-                f"Rolling over overnight straddle - IV: {iv}, Vix: {vix}.", self.webhook_url
+                f"{self.name} Rolling over overnight straddle - IV: {iv}, Vix: {vix}.", self.webhook_url
             )
 
         trade_data = load_data()
-        buy_strike = trade_data[self.name]
+        buy_strike = trade_data.get(self.name, None)
 
+        # Checking if the buy strike is valid
         if (
             not isinstance(buy_strike, int)
             and not isinstance(buy_strike, float)
             and buy_strike is not None
         ):
             notifier(f"Invalid strike found for {self.name}.", self.webhook_url)
             raise Exception(f"Invalid strike found for {self.name}.")
 
         # Placing orders
         if buy_strike is None and sell_strike is None:
-            notifier("No trade required.", self.webhook_url)
+            notifier(f"{self.name} No trade required.", self.webhook_url)
             return
         elif sell_strike is None:  # only exiting current position
             notifier(
-                f"Exiting current position on strike {buy_strike}.", self.webhook_url
+                f"{self.name} Exiting current position on strike {buy_strike}.", self.webhook_url
             )
             call_buy_avg, put_buy_avg = self.place_combined_order(
                 self.current_expiry,
                 "BUY",
                 quantity_in_lots,
                 strike=buy_strike,
                 return_avg_price=True,
                 order_tag=order_tag,
             )
-            self.log_order(
-                buy_strike,
-                self.current_expiry,
-                "BUY",
-                call_buy_avg,
-                put_buy_avg,
-                order_tag,
-            )
+            self.log_combined_order(buy_strike, expiry=self.current_expiry, buy_or_sell="BUY", call_price=call_buy_avg,
+                                    put_price=put_buy_avg, order_tag=order_tag)
         elif buy_strike is None:  # only entering new position
             notifier(
-                f"Entering new position on strike {sell_strike}.", self.webhook_url
+                f"{self.name} Entering new position on strike {sell_strike}.", self.webhook_url
             )
             call_sell_avg, put_sell_avg = self.place_combined_order(
                 self.current_expiry,
                 "SELL",
                 quantity_in_lots,
                 strike=sell_strike,
                 return_avg_price=True,
                 order_tag=order_tag,
             )
-            self.log_order(
-                sell_strike,
-                self.current_expiry,
-                "SELL",
-                call_sell_avg,
-                put_sell_avg,
-                order_tag,
-            )
+            self.log_combined_order(sell_strike, expiry=self.current_expiry, buy_or_sell="SELL",
+                                    call_price=call_sell_avg, put_price=put_sell_avg, order_tag=order_tag)
         else:  # both entering and exiting positions
             if buy_strike == sell_strike:
-                notifier("No trade required as strike is same.", self.webhook_url)
+                notifier(f"{self.name} No trade required as strike is same.", self.webhook_url)
                 call_ltp, put_ltp = fetch_straddle_price(
                     self.name, self.current_expiry, sell_strike
                 )
-                self.log_order(
-                    buy_strike, self.current_expiry, "BUY", call_ltp, put_ltp, order_tag
-                )
-                self.log_order(
-                    sell_strike,
-                    self.current_expiry,
-                    "SELL",
-                    call_ltp,
-                    put_ltp,
-                    order_tag,
-                )
+                self.log_combined_order(buy_strike, expiry=self.current_expiry, buy_or_sell="BUY", call_price=call_ltp,
+                                        put_price=put_ltp, order_tag=order_tag)
+                self.log_combined_order(sell_strike, expiry=self.current_expiry, buy_or_sell="SELL",
+                                        call_price=call_ltp, put_price=put_ltp, order_tag=order_tag)
             else:
                 notifier(
-                    f"Buying {buy_strike} and selling {sell_strike}.", self.webhook_url
+                    f"{self.name} Buying {buy_strike} and selling {sell_strike}.", self.webhook_url
                 )
                 call_buy_avg, put_buy_avg = self.place_combined_order(
                     self.current_expiry,
                     "BUY",
                     quantity_in_lots,
                     strike=buy_strike,
                     return_avg_price=True,
@@ -1600,30 +1629,18 @@
                     self.current_expiry,
                     "SELL",
                     quantity_in_lots,
                     strike=sell_strike,
                     return_avg_price=True,
                     order_tag=order_tag,
                 )
-                self.log_order(
-                    buy_strike,
-                    self.current_expiry,
-                    "BUY",
-                    call_buy_avg,
-                    put_buy_avg,
-                    order_tag,
-                )
-                self.log_order(
-                    sell_strike,
-                    self.current_expiry,
-                    "SELL",
-                    call_sell_avg,
-                    put_sell_avg,
-                    order_tag,
-                )
+                self.log_combined_order(buy_strike, expiry=self.current_expiry, buy_or_sell="BUY",
+                                        call_price=call_buy_avg, put_price=put_buy_avg, order_tag=order_tag)
+                self.log_combined_order(sell_strike, expiry=self.current_expiry, buy_or_sell="SELL",
+                                        call_price=call_sell_avg, put_price=put_sell_avg, order_tag=order_tag)
 
         trade_data[self.name] = sell_strike
         save_data(trade_data)
 
     def buy_weekly_hedge(
         self,
         quantity_in_lots,
@@ -1651,22 +1668,17 @@
             strike=strike,
             call_strike=call_strike,
             put_strike=put_strike,
             order_tag="Weekly Hedge",
             return_avg_price=True,
         )
 
-        self.log_order(
-            strike if strike is not None else call_strike,
-            self.next_expiry,
-            "BUY",
-            call_buy_avg,
-            put_buy_avg,
-            "Weekly Hedge",
-        )
+        self.log_combined_order(strike=strike, call_strike=call_strike, put_strike=put_strike, expiry=self.next_expiry,
+                                buy_or_sell="BUY", call_price=call_buy_avg, put_price=put_buy_avg,
+                                order_tag="Weekly Hedge")
 
     @log_errors
     def intraday_straddle(
         self,
         quantity_in_lots,
         exit_time=(15, 28),
         websocket=None,
@@ -1769,29 +1781,31 @@
         else:
             sl = stoploss
 
         call_stoploss_order_ids = []
         put_stoploss_order_ids = []
         stoploss_tag = f"{self.name} {strategy_id} stoploss"
         for quantity in spliced_orders:
-            call_sl_order_id = placeSLorder(
+            call_sl_order_id = place_order(
                 call_symbol,
                 call_token,
                 quantity * self.lot_size,
                 "BUY",
                 call_avg_price * sl,
-                stoploss_tag,
+                order_tag=stoploss_tag,
+                stop_loss_order=True
             )
-            put_sl_order_id = placeSLorder(
+            put_sl_order_id = place_order(
                 put_symbol,
                 put_token,
                 quantity * self.lot_size,
                 "BUY",
                 put_avg_price * sl,
-                stoploss_tag,
+                order_tag=stoploss_tag,
+                stop_loss_order=True
             )
             call_stoploss_order_ids.append(call_sl_order_id)
             put_stoploss_order_ids.append(put_sl_order_id)
             sleep(0.3)
 
         orderbook = fetch_book("orderbook")
         call_sl_statuses = lookup_and_return(
@@ -1809,17 +1823,16 @@
             )
         else:
             notifier(
                 f"{self.name} stoploss orders not placed successfully", self.webhook_url
             )
             raise Exception("Stoploss orders not placed successfully")
 
-        self.log_order(
-            equal_strike, expiry, "SELL", call_avg_price, put_avg_price, order_tag
-        )
+        self.log_combined_order(equal_strike, expiry=expiry, buy_or_sell="SELL", call_price=call_avg_price,
+                                put_price=put_avg_price, order_tag=order_tag)
         summary_message = "\n".join(
             f"{k}: {v}" for k, v in self.order_log[order_tag][0].items()
         )
 
         # Recording initial iv information
 
         traded_call_iv, traded_put_iv, traded_avg_iv = straddle_iv(
@@ -1987,15 +2000,15 @@
                     tracked_iv = put_iv if callsl and put_iv is not None else avg_iv
                     if tracked_iv is not None:
                         incremental_gains, average_delta = simulate_option_movement(
                             underlying_price,
                             equal_strike,
                             timetoexpiry(expiry),
                             option_type,
-                            simulated_move=0.2,
+                            simulated_move=0.002,
                             r=0.06,
                             vol=tracked_iv,
                             price=option_price,
                         )
                     else:
                         incremental_gains, average_delta = 100, 1
 
@@ -2031,15 +2044,16 @@
                     print(
                         f"Index: {self.name}\nTime: {currenttime().time()}\nStrike: {equal_strike}\n"
                         + f"Underlying Price: {underlying_price}\nCall SL: {callsl}\nPut SL: {putsl}\n"
                         + f"Call Price: {call_price}\nPut Price: {put_price}\n"
                         + stoploss_message
                         + f"Total price: {call_price + put_price:0.2f}\nMTM Price: {mtm_price:0.2f}\n"
                         + f"Profit in points: {profit_in_pts:0.2f}\n"
-                        + f"Profit Value: {profit_in_rs:0.2f}\nIV: {print_iv * 100:0.2f}\nSmart Exit: {smart_exit_trg}\n"
+                        + f"Profit Value: {profit_in_rs:0.2f}\n"
+                        + f"IV: {print_iv * 100:0.2f}\nSmart Exit: {smart_exit_trg}\n"
                         + ctb_message
                     )
                     last_print_time = currenttime()
 
         def process_order_statuses(
             order_book, order_ids, stop_loss=False, notify_url=None, context=""
         ):
@@ -2218,15 +2232,15 @@
             strike = findstrike(underlying_price, self.base)
             opt_type = "PE" if sl_type == "call" else "CE"
             symbol, token = fetch_symbol_token(self.name, expiry, strike, opt_type)
             option_ltp = fetchltp("NFO", symbol, token)
             qty = max(int(quantity_in_lots * qty_ratio), 1)
             trend_spliced_orders = self.splice_orders(qty)
             for spliced_qty in trend_spliced_orders:
-                placeorder(
+                place_order(
                     symbol, token, spliced_qty * self.lot_size, "SELL", option_ltp * 0.9
                 )
             sl_price = (
                 (underlying_price * (1 - trend_sl))
                 if sl_type == "call"
                 else (underlying_price * (1 + trend_sl))
             )
@@ -2268,15 +2282,15 @@
                 )
             else:
                 notifier(
                     f"{self.name} {sl_type} trend catcher exiting.", self.webhook_url
                 )
 
             for qty in trend_spliced_orders:
-                placeorder(symbol, token, qty * self.lot_size, "BUY", "MARKET")
+                place_order(symbol, token, qty * self.lot_size, "BUY", "MARKET")
 
         def process_sl_hit(
             sl_type,
             sl_dict,
             sl_orders_complete,
             symbol,
             token,
@@ -2291,36 +2305,38 @@
                 # print(f'{self.name} both stoploss orders completed. Not processing {sl_type}.')
                 return
 
             other_sl_type = "call" if sl_type == "put" else "put"
 
             if not sl_orders_complete:
                 for qty in spliced_orders:
-                    placeorder(symbol, token, qty * self.lot_size, "BUY", "MARKET")
+                    place_order(symbol, token, qty * self.lot_size, "BUY", "MARKET")
 
             if catch_trend:
                 trend_thread = Thread(
                     target=trend_catcher,
                     args=(sl_type, trend_qty_ratio, trend_catcher_sl),
                 )
                 trend_thread.start()
 
             if move_sl:
                 for o_id in other_stoploss_order_ids:
                     obj.cancelOrder(o_id, "STOPLOSS")
 
                 other_stoploss_order_ids.clear()
                 for qty in spliced_orders:
-                    sl_order_id = placeSLorder(
+                    sl_order_id = place_order(
                         other_symbol,
                         other_token,
                         qty * self.lot_size,
                         "BUY",
                         other_avg_price,
-                        stoploss_tag,
+                        order_tag=stoploss_tag,
+                        stop_loss_order=True
+
                     )
                     other_stoploss_order_ids.append(sl_order_id)
 
             # notifier(f'{self.name} {sl_type} stoploss triggered and completed.', self.webhook_url)
 
             refresh = True
             sleep(5)
@@ -2334,15 +2350,15 @@
             ):
                 sl_dict[other_sl_type], other_sl_orders_complete = check_sl_orders(
                     other_stoploss_order_ids, other_sl_type, refresh=refresh
                 )
                 if sl_dict[other_sl_type]:
                     if not other_sl_orders_complete:
                         for qty in spliced_orders:
-                            placeorder(
+                            place_order(
                                 other_symbol,
                                 other_token,
                                 qty * self.lot_size,
                                 "BUY",
                                 "MARKET",
                             )
                     break
@@ -2353,15 +2369,15 @@
         def process_exit(call_stop_loss_hit, put_stop_loss_hit, hedged=False):
             def exit_spliced_orders(orders, side):
                 symbol = call_symbol if side == "call" else put_symbol
                 token = call_token if side == "call" else put_token
                 price = call_price if side == "call" else put_price
 
                 for qty in orders:
-                    placeorder(
+                    place_order(
                         symbol,
                         token,
                         qty * self.lot_size,
                         "BUY",
                         price * 1.1,
                         "Exit order",
                     )
@@ -2417,25 +2433,26 @@
         # IV information
         call_iv = 0
         put_iv = 0
         avg_iv = 0
 
         # Basic price information being set in outer scope as well
         total_avg_price = call_avg_price + put_avg_price
-        per_share_charges = charges(
-            (call_avg_price + put_avg_price),
-            self.lot_size,
-            quantity_in_lots,
-            self.lot_size,
-        )
-        break_even_price = total_avg_price - per_share_charges
-        notifier(
-            f"{self.name}: Charges per share {per_share_charges} | Break even price {break_even_price}",
-            self.webhook_url,
-        )
+        if take_profit:
+            per_share_charges = charges(
+                (call_avg_price + put_avg_price),
+                self.lot_size,
+                quantity_in_lots,
+                self.lot_size,
+            )
+            break_even_price = total_avg_price - per_share_charges
+            notifier(
+                f"{self.name}: Charges per share {per_share_charges} | Break even price {break_even_price}",
+                self.webhook_url,
+            )
 
         # Setting up stop loss dictionary and starting price thread
         sl_hit_dict = {"call": False, "put": False}
         price_updater = Thread(target=price_tracker)
 
         sleep(5)
         refresh_orderbook = True
@@ -2554,14 +2571,356 @@
         notifier(
             f"{self.name}: Exited positions\n"
             + "".join([f"{key}: {value}\n" for key, value in exit_dict.items()]),
             self.webhook_url,
         )
         in_trade = False
 
+    @log_errors
+    def intraday_strangle(
+        self,
+        quantity_in_lots,
+        call_strike_offset=0,
+        put_strike_offset=0,
+        stop_loss=1.6,
+        exit_time=(15, 29),
+        sleep_time=60,
+        catch_trend=False,
+        trend_qty_ratio=1,
+        trend_strike_offset=0,
+        trend_sl=0.003
+    ):
+        """Intraday strangle strategy. Trades strangle with  stop loss. All offsets are in percentage terms.
+        Parameters
+        ----------
+        quantity_in_lots : int
+            Quantity in lots
+        call_strike_offset : float, optional
+            Call strike offset in percentage terms, by default 0
+        put_strike_offset : float, optional
+            Put strike offset in percentage terms, by default 0
+        stop_loss : float, optional
+            Stop loss percentage, by default 1.6
+        exit_time : tuple, optional
+            Exit time, by default (15, 29)
+        sleep_time : int, optional
+            Sleep time in seconds for updating prices, by default 60
+        catch_trend : bool, optional
+            Catch trend or not, by default False
+        trend_qty_ratio : int, optional
+            Ratio of trend quantity to strangle quantity, by default 1
+        trend_strike_offset : float, optional
+            Strike offset for trend order in percentage terms, by default 0
+        trend_sl : float, optional
+            Stop loss for trend order, by default 0.003
+        """
+
+        order_tag = "Intraday Strangle"
+        underlying_ltp = self.fetch_ltp()
+        call_strike = underlying_ltp * (1 + call_strike_offset)
+        put_strike = underlying_ltp * (1 - put_strike_offset)
+        call_strike = findstrike(call_strike, self.base)
+        put_strike = findstrike(put_strike, self.base)
+        expiry = self.current_expiry
+
+        strangle = Strangle(call_strike=call_strike, put_strike=put_strike, underlying=self.name, expiry=expiry)
+
+        call_order_ids, put_order_ids = strangle.place_order(
+            "SELL", quantity_in_lots, prices="LIMIT", order_tag=order_tag
+        )
+
+        orderbook = fetch_book('orderbook')
+        order_statuses = lookup_and_return(orderbook, 'orderid', call_order_ids+put_order_ids, 'status')
+        check_and_notify_order_statuses(
+            order_statuses,
+            self.webhook_url,
+            order_tag=order_tag,
+            Underlying=self.name,
+            Action="SELL",
+            Strikes=[call_strike, put_strike],
+            Expiry=expiry,
+            Quantity=quantity_in_lots
+        )
+
+        call_avg_price = lookup_and_return(orderbook, 'orderid', call_order_ids, 'averageprice').astype(float).mean()
+        put_avg_price = lookup_and_return(orderbook, 'orderid', put_order_ids, 'averageprice').astype(float).mean()
+        total_avg_price = call_avg_price + put_avg_price
+
+        call_stop_loss_price = call_avg_price * stop_loss
+        put_stop_loss_price = put_avg_price * stop_loss
+
+        self.log_combined_order(
+            call_strike=call_strike,
+            put_strike=put_strike,
+            expiry=expiry,
+            buy_or_sell="SELL",
+            call_price=call_avg_price,
+            put_price=put_avg_price,
+            order_tag=order_tag
+        )
+
+        summary_message = "\n".join(
+            f"{k}: {v}" for k, v in self.order_log[order_tag][0].items()
+        )
+
+        traded_call_iv, traded_put_iv, traded_avg_iv = strangle_iv(
+            callprice=call_avg_price,
+            putprice=put_avg_price,
+            callstrike=call_strike,
+            putstrike=put_strike,
+            spot=underlying_ltp,
+            timeleft=timetoexpiry(expiry)
+        )
+
+        summary_message += f"\nTraded IVs: {traded_call_iv}, {traded_put_iv}, {traded_avg_iv}"
+        summary_message += f"\nCall SL: {call_stop_loss_price}, Put SL: {put_stop_loss_price}"
+        notifier(summary_message, self.webhook_url)
+
+        def position_monitor():
+
+            nonlocal strangle, call_avg_price, put_avg_price, call_stop_loss_price, put_stop_loss_price, exit_price_dict
+            nonlocal call_sl, put_sl, underlying_ltp, call_ltp, put_ltp, profit_in_pts
+            nonlocal in_trade
+
+            last_print_time = currenttime()
+            last_log_time = currenttime()
+            last_notify_time = currenttime()
+            print_interval = timedelta(seconds=5)
+            log_interval = timedelta(minutes=5)
+            notify_interval = timedelta(minutes=60)
+            while in_trade:
+                underlying_ltp = self.fetch_ltp()
+                call_ltp, put_ltp = strangle.fetch_ltp()
+                call_iv, put_iv, avg_iv = strangle_iv(
+                    callprice=call_ltp,
+                    putprice=put_ltp,
+                    callstrike=call_strike,
+                    putstrike=put_strike,
+                    spot=underlying_ltp,
+                    timeleft=timetoexpiry(expiry)
+                )
+                call_sl = call_ltp > call_stop_loss_price
+                put_sl = put_ltp > put_stop_loss_price
+
+                # DELETE THIS LATER ONLY FOR TESTING
+                call_stop_loss_price = call_stop_loss_price - 0.2
+
+                # Calculate mtm price
+                call_exit_price = exit_price_dict.get('call', call_ltp)
+                put_exit_price = exit_price_dict.get('put', put_ltp)
+                mtm_price = call_exit_price + put_exit_price
+
+                # Calculate profit
+                profit_in_pts = (call_avg_price + put_avg_price) - mtm_price
+                profit_in_rs = profit_in_pts * self.lot_size * quantity_in_lots
+
+                message = (
+                    f"\nUnderlying: {self.name}\n"
+                    f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
+                    f"Underlying LTP: {underlying_ltp}\n"
+                    f"Call Strike: {call_strike}\n"
+                    f"Put Strike: {put_strike}\n"
+                    f"Call Price: {call_ltp}\n"
+                    f"Put Price: {put_ltp}\n"
+                    f"MTM Price: {mtm_price}\n"
+                    f"IVs: {call_iv}, {put_iv}, {avg_iv}\n"
+                    f"Call SL: {call_sl}\n"
+                    f"Put SL: {put_sl}\n"
+                    f"Profit Pts: {profit_in_pts:.2f}\n"
+                    f"Profit: {profit_in_rs:.2f}\n"
+                )
+                if currenttime() - last_print_time > print_interval:
+                    print(message)
+                    last_print_time = currenttime()
+                if currenttime() - last_log_time > log_interval:
+                    logger.info(message)
+                    last_log_time = currenttime()
+                if currenttime() - last_notify_time > notify_interval:
+                    notifier(message, self.webhook_url)
+                    last_notify_time = currenttime()
+                sleep(sleep_time)
+
+        def trend_catcher(sl_type, qty_ratio, stoploss, strike_offset):
+            nonlocal underlying_ltp, in_trade
+
+            offset = 1-strike_offset if sl_type == "call" else 1+strike_offset
+            trend = "Up" if sl_type == "call" else "Down"
+
+            # Setting up the trend option
+            strike = underlying_ltp * offset
+            strike = findstrike(strike, self.base)
+            opt_type = "PE" if sl_type == "call" else "CE"
+            qty_in_lots = max(int(quantity_in_lots * qty_ratio), 1)
+            trend_option = Option(strike, opt_type, self.name, expiry)
+
+            # Placing the trend option order
+            place_option_order_and_notify(
+                trend_option, "SELL", qty_in_lots, "Intraday Strangle Trend Catcher", self.webhook_url
+            )
+
+            # Setting up the stop loss
+            sl_multiplier = 1 - stoploss if sl_type == "call" else 1 + stoploss
+            sl_price = underlying_ltp * sl_multiplier
+            trend_sl_hit = False
+
+            last_print_time = currenttime()
+            print_interval = timedelta(seconds=10)
+            while all([currenttime().time() < time(*exit_time), in_trade]):
+                trend_sl_hit = underlying_ltp < sl_price if sl_type == "call" else underlying_ltp > sl_price
+                if trend_sl_hit:
+                    break
+                sleep(1)
+                if currenttime() - last_print_time > print_interval:
+                    last_print_time = currenttime()
+                    print(
+                        f"{self.name} {sl_type} trend catcher running.\n"
+                        + f"Stoploss price: {sl_price}, Underlying Price: {underlying_ltp}\n"
+                        + f"Stoploss hit: {trend_sl_hit}.\n"
+                    )
+
+            if trend_sl_hit:
+                notifier(
+                    f"{self.name} strangle {trend} trend catcher stoploss hit.", self.webhook_url
+                )
+            else:
+                notifier(
+                    f"{self.name} strangle {trend} trend catcher exiting.", self.webhook_url
+                )
+
+            # Buying the trend option back
+            place_option_order_and_notify(
+                trend_option, "BUY", qty_in_lots, "Intraday Strangle Trend Catcher", self.webhook_url
+            )
+
+        def process_stop_loss(sl_type):
+
+            nonlocal strangle, call_sl, put_sl, exit_price_dict
+
+            if call_sl and put_sl:  # Check to avoid double processing
+                return
+
+            # Buying the stop loss option back
+            notifier(f'{self.name} strangle {sl_type} stop loss hit.', self.webhook_url)
+            option_to_buy = strangle.call_option if sl_type == "call" else strangle.put_option
+            exit_price = place_option_order_and_notify(
+                option_to_buy, "BUY", quantity_in_lots, order_tag, self.webhook_url
+            )
+            exit_price_dict[sl_type] = exit_price
+
+            # Starting the trend catcher
+            if catch_trend:
+                trend_thread = Thread(
+                    target=trend_catcher,
+                    args=(sl_type, trend_qty_ratio, trend_sl, trend_strike_offset)
+                )
+                trend_thread.start()
+
+            # Wait for exit or other stop loss to hit
+            while all([currenttime().time() < time(*exit_time)]):
+                sleep(1)
+                if call_sl and put_sl:
+                    other_sl_option = strangle.put_option if sl_type == "call" else strangle.call_option
+                    other_sl_type = "put" if sl_type == "call" else "call"
+                    notifier(f'{self.name} strangle {other_sl_type} stop loss hit.', self.webhook_url)
+                    other_exit_price = place_option_order_and_notify(
+                        other_sl_option, "BUY", quantity_in_lots, order_tag, self.webhook_url
+                    )
+                    exit_price_dict[other_sl_type] = other_exit_price
+                    break
+
+        in_trade = True
+        call_sl = False
+        put_sl = False
+        profit_in_pts = 0
+        call_ltp, put_ltp = strangle.fetch_ltp()
+        exit_price_dict = {}
+
+        position_monitor_thread = Thread(target=position_monitor)
+        position_monitor_thread.start()
+
+        # Wait for exit time or both stop losses to hit (Main Loop)
+        while all([currenttime().time() < time(*exit_time)]):
+            sleep(2)
+            if call_sl or put_sl:
+                if call_sl:
+                    process_stop_loss("call")
+                if put_sl:
+                    process_stop_loss("put")
+                break
+
+        # Out of the while loop, so exit time reached or both stop losses hit
+
+        if not call_sl and not put_sl:
+            call_order_ids, put_order_ids = strangle.place_order("BUY", quantity_in_lots, "LIMIT", order_tag)
+            order_book = fetch_book('orderbook')
+            order_statuses_ = lookup_and_return(order_book, 'orderid', call_order_ids + put_order_ids, 'status')
+            check_and_notify_order_statuses(
+                order_statuses_,
+                self.webhook_url,
+                order_tag='Strangle Exit',
+                Underlying=self.name,
+                Action='BUY',
+                Strike=strangle.call_option.strike,
+                Expiry=strangle.call_option.expiry,
+                Qty=quantity_in_lots,
+            )
+
+            exit_price_dict['call'] = lookup_and_return(
+                order_book, 'orderid', call_order_ids, 'averageprice'
+            ).astype(float).mean()
+            exit_price_dict['put'] = lookup_and_return(
+                order_book, 'orderid', put_order_ids, 'averageprice'
+            ).astype(float).mean()
+
+        elif (call_sl or put_sl) and not (call_sl and put_sl):  # Only one stop loss hit
+            exit_option = strangle.put_option if call_sl else strangle.call_option
+            non_sl_exit_price = place_option_order_and_notify(
+                exit_option, "BUY", quantity_in_lots, order_tag, self.webhook_url
+            )
+            exit_option = "put" if call_sl else "call"
+            exit_price_dict[exit_option] = non_sl_exit_price
+
+        else:  # Both stop losses hit
+            pass
+
+        # Calculate profit
+        total_exit_price = sum(exit_price_dict.values())
+        exit_message = (
+            f"{self.name} strangle exited.\n"
+            f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
+            f"Underlying LTP: {underlying_ltp}\n"
+            f"Call Price: {call_ltp}\n"
+            f"Put Price: {put_ltp}\n"
+            f"Call SL: {call_sl}\n"
+            f"Put SL: {put_sl}\n"
+            f"Call Exit Price: {exit_price_dict['call']}\n"
+            f"Put Exit Price: {exit_price_dict['put']}\n"
+            f"Total Exit Price: {total_exit_price}\n"
+            f"Total Entry Price: {total_avg_price}\n"
+            f"Profit Pts: {total_avg_price - total_exit_price}\n"
+        )
+        exit_dict = {
+            "Call exit price": exit_price_dict["call"],
+            "Put exit price": exit_price_dict["put"],
+            "Total exit price": total_exit_price,
+            "Points captured": total_avg_price - total_exit_price,
+            "Call SL": call_sl,
+            "Put SL": put_sl,
+        }
+        try:
+            self.order_log[order_tag][0].update(exit_dict)
+        except Exception as e:
+            notifier(
+                f"{self.name}: Error updating order list with exit details. {e}",
+                self.webhook_url,
+            )
+        notifier(exit_message, self.webhook_url)
+        in_trade = False
+        position_monitor_thread.join()
+
     def intraday_straddle_delta_hedged(
         self,
         quantity_in_lots,
         exit_time=(15, 30),
         websocket=None,
         wait_for_equality=False,
         delta_threshold=1,
@@ -2909,14 +3268,68 @@
             data=json.dumps(data),
             headers={"Content-Type": "application/json"},
         )
         print(message)
     return
 
 
+def check_and_notify_order_statuses(statuses, webhook_url=None, **kwargs):
+
+    order_prefix = f"{kwargs['order_tag']}: " if "order_tag" in kwargs else ""
+    order_message = [f"{k}-{v}" for k, v in kwargs.items() if k != "order_tag"]
+    order_message = ", ".join(order_message)
+
+    if all(statuses == "complete"):
+        notifier(
+            f"{order_prefix}Order(s) placed successfully for {order_message}",
+            webhook_url
+        )
+    elif all(statuses == "rejected"):
+        notifier(
+            f"{order_prefix}All orders rejected for {order_message}",
+            webhook_url
+        )
+        raise Exception("Orders rejected")
+    elif any(statuses == "open"):
+        notifier(
+            f"{order_prefix}Some orders pending for {order_message}. You can modify the orders.",
+            webhook_url
+        )
+    elif any(statuses == "rejected"):
+        notifier(
+            f"{order_prefix}Some orders rejected for {order_message}.\nYou can place the rejected orders again.",
+            webhook_url
+        )
+    else:
+        notifier(
+            f"{order_prefix}ERROR. Order statuses uncertain for {order_message}",
+            webhook_url
+        )
+        raise Exception("Order statuses uncertain")
+
+
+def place_option_order_and_notify(option, action, qty_in_lots, order_tag, webhook_url=None):
+    order_ids = option.place_order(action, qty_in_lots, "LIMIT", order_tag)
+    order_book = fetch_book('orderbook')
+    order_statuses_ = lookup_and_return(order_book, 'orderid', order_ids, 'status')
+    check_and_notify_order_statuses(
+        order_statuses_,
+        webhook_url,
+        order_tag=order_tag,
+        Underlying=option.underlying,
+        Action=action,
+        Strike=option.strike,
+        OptionType=option.option_type,
+        Expiry=option.expiry,
+        Qty=qty_in_lots
+    )
+    avg_price = lookup_and_return(order_book, 'orderid', order_ids, 'averageprice').astype(float).mean()
+    return avg_price
+
+
 # Market Hours
 def markethours():
     if time(9, 10) < currenttime().time() < time(15, 30):
         return True
     else:
         return False
 
@@ -2929,49 +3342,77 @@
 
 
 def simulate_option_movement(
     spot,
     strike,
     time_to_expiry,
     flag,
-    simulated_move=0.2,
+    direction="away",
+    simulated_move=0.002,
     r=0.06,
     vol=None,
     price=None,
     print_results=False,
 ):
+    """
+    :param spot:
+    :param strike:
+    :param time_to_expiry:
+    :param flag: option type for which price is to be simulated
+    :param direction: the direction of the move, "away" or "towards"
+    :param simulated_move:
+    :param r:
+    :param vol:
+    :param price:
+    :param print_results:
+    :return:
+    """
+
     if price is None and vol is None:
         raise ValueError("Either price or vol must be specified.")
     flag = flag.lower()[0]
     price_func = bs.put if flag == 'p' else bs.call
-    simulated_move = simulated_move / 100
-    simulated_spot = (
-        (spot * (1 + simulated_move)) if flag == "p" else (spot * (1 - simulated_move))
-    )
+
+    if direction == "away":
+        if flag == "c":
+            simulated_move = -simulated_move
+        else:
+            simulated_move = simulated_move
+    elif direction == "towards" or direction == "toward":
+        if flag == "c":
+            simulated_move = simulated_move
+        else:
+            simulated_move = -simulated_move
+    else:
+        raise ValueError("Invalid direction.")
+
+    simulated_spot = spot * (1 + simulated_move)
     if vol is None:
         try:
             vol = bs.implied_volatility(price, spot, strike, time_to_expiry, r, flag)
         except ValueError:
             return None
     if price is None:
         price = price_func(spot, strike, time_to_expiry, r, vol)
     current_delta = bs.delta(spot, strike, time_to_expiry, r, vol, flag)
-    new_delta = bs.delta(simulated_spot, strike, time_to_expiry, r, vol, flag)
+
+    new_vol = bs.iv_curve_adjustor(simulated_move, time_to_expiry, vol, spot, strike)
+    new_delta = bs.delta(simulated_spot, strike, time_to_expiry, r, new_vol, flag)
     delta_change = new_delta - current_delta
     average_delta = abs((new_delta + current_delta) / 2)
-    new_price = price_func(simulated_spot, strike, time_to_expiry, r, vol)
+    new_price = price_func(simulated_spot, strike, time_to_expiry, r, new_vol)
     price_gain = price - new_price
 
     if print_results:
         print(
             f"Current Delta: {current_delta:.2f}\nNew Delta: {new_delta:.2f}\n"
             f"Delta Change: {delta_change:.2f}\nAverage Delta: {average_delta:.2f}\n"
             f"New Price: {new_price:.2f}\nPrice Change: {price_gain:.2f}\n"
             f"Volatility: {vol:.2f}\nSimulated Spot: {simulated_spot:.2f}\n"
-            f"Simulated Move: {simulated_move * 100:.2f}%\n"
+            f"Simulated Move: {simulated_move}%\n"
         )
 
     return [price_gain, average_delta]
 
 
 def spot_price_from_future(future_price, interest_rate, time_to_future):
     """
@@ -3039,15 +3480,15 @@
         symbol_token_pairs = [
             (token_df.loc[token_df["token"] == token, "symbol"].values[0], token)
             for token in tokens
         ]
         return symbol_token_pairs
 
     if expiry is None and strike is None and option_type is None:
-        if name in ["BANKNIFTY", "NIFTY"]:
+        if name in ["BANKNIFTY", "NIFTY", "NIFTY FIN SERVICE"]:
             symbol, token = scrips.loc[
                 (scrips.name == name) & (scrips.exch_seg == "NSE"), ["symbol", "token"]
             ].values[0]
         elif name == "FINNIFTY":
             futures = scrips.loc[
                 (scrips.name == name) & (scrips.instrumenttype == "FUTIDX"),
                 ["expiry", "symbol", "token"],
@@ -3336,28 +3777,73 @@
     vix = vix.fast_info["last_price"]
     return vix
 
 
 def get_index_constituents(index_symbol, cutoff_pct=101):
     # Fetch and filter constituents
     constituents = (
-        pd.read_csv(f"autotrader/{index_symbol}_constituents.csv")
+        pd.read_csv(f"autotrader/info/{index_symbol}_constituents.csv")
         .sort_values("Index weight", ascending=False)
         .assign(cum_weight=lambda df: df["Index weight"].cumsum())
         .loc[lambda df: df.cum_weight < cutoff_pct]
     )
 
     constituent_tickers, constituent_weights = (
         constituents.Ticker.to_list(),
         constituents["Index weight"].to_list(),
     )
 
     return constituent_tickers, constituent_weights
 
 
+def convert_option_chains_to_df(option_chains, return_all=False, for_surface=False):
+
+    def add_columns_for_surface(data_frame):
+
+        data_frame = data_frame.copy()
+        data_frame['atm_strike'] = data_frame.apply(
+            lambda row: findstrike(row.spot, 50) if row.symbol == 'NIFTY' else findstrike(row.spot, 100),
+            axis=1)
+        data_frame['strike_iv'] = np.where(data_frame.strike > data_frame.atm_strike, data_frame.call_iv,
+                                           np.where(data_frame.strike < data_frame.atm_strike,
+                                                    data_frame.put_iv, data_frame.avg_iv))
+        data_frame['atm_iv'] = data_frame.apply(
+            lambda row: data_frame[(data_frame.strike == row.atm_strike)
+                                   & (data_frame.expiry == row.expiry)].strike_iv.values[0], axis=1)
+        data_frame.sort_values(['symbol', 'expiry', 'strike'], inplace=True)
+        data_frame['distance'] = (data_frame['strike'] / data_frame['spot'] - 1)
+        data_frame['iv_multiple'] = data_frame['strike_iv'] / data_frame['atm_iv']
+        data_frame['distance_squared'] = data_frame['distance'] ** 2
+
+        return data_frame
+
+    symbol_dfs = []
+    for symbol in option_chains:
+        spot_price = option_chains[symbol].underlying_price
+        expiry_dfs = []
+        for expiry in option_chains[symbol]:
+            df = pd.DataFrame(option_chains[symbol][expiry]).T
+            df.index = df.index.set_names('strike')
+            df = df.reset_index()
+            df['spot'] = spot_price
+            df['expiry'] = expiry
+            df['symbol'] = symbol
+            df['time_to_expiry'] = timetoexpiry(expiry)
+            expiry_dfs.append(df)
+        symbol_oc = pd.concat(expiry_dfs)
+        if for_surface:
+            symbol_oc = add_columns_for_surface(symbol_oc)
+        symbol_dfs.append(symbol_oc)
+
+    if return_all:
+        return pd.concat(symbol_dfs)
+    else:
+        return symbol_dfs
+
+
 def charges(buy_premium, contract_size, num_contracts, freeze_quantity=None):
     if freeze_quantity:
         number_of_orders = np.ceil(num_contracts / freeze_quantity)
     else:
         number_of_orders = 1
 
     buy_brokerage = 40 * number_of_orders
@@ -3389,103 +3875,59 @@
     charges_per_share = total_charges / (num_contracts * contract_size)
 
     return round(charges_per_share, 1)
 
 
 # ORDER FUNCTIONS BELOW #
 
+def place_order(symbol, token, qty, action, price, order_tag="", stop_loss_order=False):
 
-def placeorder(symbol, token, qty, buyorsell, orderprice, ordertag=""):
-    """Provide symbol, token, qty (shares), buyorsell, orderprice, ordertag (optional)"""
-
-    if orderprice == "MARKET":
-        params = {
-            "variety": "NORMAL",
-            "tradingsymbol": symbol,
-            "symboltoken": token,
-            "transactiontype": buyorsell,
-            "exchange": "NFO",
-            "ordertype": "MARKET",
-            "producttype": "CARRYFORWARD",
-            "duration": "DAY",
-            "price": 0,
-            "squareoff": "0",
-            "stoploss": "0",
-            "quantity": int(qty),
-            "ordertag": ordertag,
-        }
-
-    else:
-        if buyorsell == "BUY" and orderprice < 1:
-            orderprice = 1
-        elif buyorsell == "SELL" and orderprice < 1:
-            orderprice = 0.05
-
-        params = {
-            "variety": "NORMAL",
-            "tradingsymbol": symbol,
-            "symboltoken": token,
-            "transactiontype": buyorsell,
-            "exchange": "NFO",
-            "ordertype": "LIMIT",
-            "producttype": "CARRYFORWARD",
-            "duration": "DAY",
-            "price": round(orderprice, 1),
-            "squareoff": "0",
-            "stoploss": "0",
-            "quantity": int(qty),
-            "ordertag": ordertag,
-        }
-
-    for attempt in range(1, 4):
-        try:
-            order_id = obj.placeOrder(params)
-            return order_id
-        except KeyboardInterrupt:
-            raise KeyboardInterrupt
-        except Exception as e:
-            if attempt == 3:
-                raise e
-            print(f"Error {attempt} in placing order for {symbol}: {e}")
-            sleep(2)
-            continue
-
-
-def placeSLorder(symbol, token, qty, buyorsell, triggerprice, ordertag=""):
-    executionprice = triggerprice * 1.1
+    action = action.upper()
+    if isinstance(price, str):
+        price = price.upper()
 
     params = {
-        "variety": "STOPLOSS",
         "tradingsymbol": symbol,
         "symboltoken": token,
-        "transactiontype": buyorsell,
+        "transactiontype": action,
         "exchange": "NFO",
-        "ordertype": "STOPLOSS_LIMIT",
         "producttype": "CARRYFORWARD",
         "duration": "DAY",
-        "triggerprice": round(triggerprice, 1),
-        "price": round(executionprice, 1),
-        "squareoff": "0",
-        "stoploss": "0",
         "quantity": int(qty),
-        "ordertag": ordertag,
+        "ordertag": order_tag,
     }
 
+    if stop_loss_order:
+        execution_price = price * 1.1
+        params.update({
+            "variety": "STOPLOSS",
+            "ordertype": "STOPLOSS_LIMIT",
+            "triggerprice": round(price, 1),
+            "price": round(execution_price, 1),
+        })
+    else:
+        order_type, execution_price = ("MARKET", 0) if price == "MARKET" else ("LIMIT", price)
+        if order_type == "LIMIT":
+            if execution_price < 10 and qty < 4000:
+                execution_price = np.ceil(price) if action == "BUY" else max(np.floor(price), 0.05)
+
+        params.update({
+            "variety": "NORMAL",
+            "ordertype": order_type,
+            "price": round(execution_price, 1)
+        })
+
     for attempt in range(1, 4):
         try:
-            order_id = obj.placeOrder(params)
-            return order_id
-        except KeyboardInterrupt:
-            raise KeyboardInterrupt
+            return obj.placeOrder(params)
         except Exception as e:
             if attempt == 3:
                 raise e
-            print(f"Error {attempt} in placing SL order for {symbol}: {e}")
+            print(f"Error {attempt} in placing {'stop-loss ' if stop_loss_order else ''}order for {symbol}: {e}")
             sleep(2)
-            continue
 
 
 def place_synthetic_fut_order(
     name,
     strike,
     expiry,
     buy_or_sell,
@@ -3502,18 +3944,18 @@
         call_price = "MARKET"
         put_price = "MARKET"
     else:
         call_price, put_price = prices
 
     call_action = "BUY" if buy_or_sell == "BUY" else "SELL"
     put_action = "SELL" if buy_or_sell == "BUY" else "BUY"
-    order_id_call = placeorder(
+    order_id_call = place_order(
         call_symbol, call_token, quantity_in_shares, call_action, call_price
     )
-    order_id_put = placeorder(
+    order_id_put = place_order(
         put_symbol, put_token, quantity_in_shares, put_action, put_price
     )
     return order_id_call, order_id_put
 
 
 def cancel_pending_orders(order_ids, variety="STOPLOSS"):
     if isinstance(order_ids, (list, np.ndarray)):
```

### Comparing `autotrading-0.8.8/autotrader/blackscholes.py` & `autotrading-0.9.0/autotrader/blackscholes.py`

 * *Files 8% similar despite different names*

```diff
@@ -165,55 +165,84 @@
             "theta": thetas,
             "vega": vegas,
             "implied_volatility": ivs,
         }
     )
 
 
-def iv_curve_adjustor(movement, iv=1, spot=100, strike=100):
+def iv_curve_adjustor(movement, time_to_expiry, iv=1, spot=100, strike=100, _print_details=False):
 
     """
-    This function returns a function that adjusts the implied volatility to account for the curve effect. The function
-    is currently calibrated for 2 days to expiry and it simulates a movement from atm. It tries to arrive at an IV
-    for the atm after the movement.
+    This function returns the adjusted implied volatility accounting for the curve effect.
     :param movement: movement of the underlying in percentage with sign
+    :param time_to_expiry: time to expiry in years
     :param iv: implied volatility of the strike
     :param spot: spot price
     :param strike: strike price
+    :param _print_details: print details of the adjustment
     :return: adjusted implied volatility for the strike after the movement
     """
 
-    coefs = [1065.29, 11.3532, 0.973536]
-    current_diff = (spot/strike - 1)
+    def iv_transformer_coeffs(tte):
+        adjuster = 3 if tte < (0.8 / 365) else 1
+        dfs2 = 1 / ((tte ** 1.2) * adjuster)
+        dfs2 = min(dfs2, 20000)
+
+        dfs = 1 / ((tte ** 0.45) * 5)
+        dfs = min(dfs, 5)
+        dfs = -6 + dfs
+        return dfs2, dfs, .97
+
+    coefs = iv_transformer_coeffs(time_to_expiry)
+    current_diff = (strike/spot - 1)
     current_iv_multiple = coefs[0] * current_diff ** 2 + coefs[1] * current_diff + coefs[2]
     atm_iv = iv / current_iv_multiple
-    print(f'atm_iv: {atm_iv}, iv: {iv}, current_iv_multiple: {current_iv_multiple}')
-    displacement_from_atm = movement + current_diff
-    print(f'displacement from atm: {displacement_from_atm}, movement: {movement}')
-    premium_to_atm_iv = coefs[0] * displacement_from_atm ** 2 + coefs[1] * displacement_from_atm + coefs[2]
-    return atm_iv * premium_to_atm_iv
-
 
-def target_movement(flag, current_price, target_price, current_spot, strike, timeleft, time_delta=None):
+    new_spot = spot * (1 + movement)
+    total_displacement = (strike / new_spot - 1)
+    premium_to_atm_iv = coefs[0] * total_displacement ** 2 + coefs[1] * total_displacement + coefs[2]
+    new_iv = atm_iv * premium_to_atm_iv
+
+    if _print_details:
+        print(
+            f'New iv: {new_iv} for strike {strike} spot {new_spot} '
+            f'iv {iv} atm_iv {atm_iv} movement {movement} '
+            f'time_to_expiry {time_to_expiry}'
+        )
+
+    return new_iv
+
+
+def target_movement(
+        flag, current_price, target_price, current_spot, strike, timeleft, time_delta=None, _print_details=False
+):
     """
     :param flag: 'c' or 'p'
     :param current_price: current price of the option
     :param target_price: target price of the option
     :param current_spot: current spot price
     :param strike: strike price
     :param timeleft: time left to expiry in years
     :param time_delta: in minutes
+    :param _print_details: print details of the adjustment
     :return:
     """
     flag = flag.lower()[0]
     price_func = call if flag == 'c' else put
     vol = implied_volatility(current_price, current_spot, strike, timeleft, 0.06, flag)
-    print(vol)
+    delta_ = delta(current_spot, strike, timeleft, 0.06, vol, flag)
+    estimated_movement_points = (target_price - current_price) / delta_
+    estimated_movement = estimated_movement_points / current_spot
     timeleft = timeleft - (time_delta / 525600) if time_delta else timeleft
-    f = lambda s1: price_func(s1, strike, timeleft, 0.06, vol) - target_price
+    modified_vol = iv_curve_adjustor(estimated_movement, timeleft, iv=vol, spot=current_spot, strike=strike)
+
+    if _print_details:
+        print(f'estimated movement: {estimated_movement}, vol: {vol}, modified vol: {modified_vol}')
+
+    f = lambda s1: price_func(s1, strike, timeleft, 0.06, modified_vol) - target_price
 
     if target_price > current_price:
         if flag == 'c':
             a = current_spot
             b = 2 * current_spot
         else:
             a = 0.05
```

### Comparing `autotrading-0.8.8/autotrader/datamodule.py` & `autotrading-0.9.0/autotrader/datamodule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import autotrader.autotradingfunctions as atf
+from autotrader.exceptions import ApiKeyNotFound
 from eod import EodHistoricalData
 import pandas as pd
 from dateutil.relativedelta import relativedelta, MO, TU, WE, TH, FR
 import numpy as np
 
 
 class DataClient:
     def __init__(self, api_key):
+        if api_key is None:
+            raise ApiKeyNotFound("EOD API Key not found")
         self.api_key = api_key
         self.client = EodHistoricalData(api_key=api_key)
 
     def get_data(self, symbol, from_date="2011-01-01", return_columns=None):
         symbol_dict = {
             "NIFTY": "NSEI.INDX",
             "BANKNIFTY": "NSEBANK.INDX",
@@ -63,20 +66,22 @@
     else:
         dates = date_filter.split("to")
         if len(dates) > 1:
             df = df.loc[dates[0]: dates[1]]
         else:
             df = df.loc[dates[0]]
 
-    if frequency is None or frequency == "D" or frequency == "B":
+    frequency = frequency.upper() if frequency is not None else None
+
+    if frequency is None or frequency.startswith("D") or frequency == "B":
         custom_frequency = "B"
         multiplier = 24
         df = df.resample("B").ffill()
 
-    else:
+    elif frequency.startswith("W") or frequency.startswith("M"):
         custom_frequency = frequency
         if frequency.startswith("W"):
             multiplier = 9.09
             df = df.resample(frequency).ffill()
         elif frequency.startswith("M"):
             multiplier = 4.4
             if len(frequency) == 1:
@@ -94,21 +99,27 @@
                 df = df.resample("M").ffill()
                 df.index = df.index.date + relativedelta(
                     weekday=weekday_module_dict[frequency.upper()](-1)
                 )
                 df.index = pd.Series(pd.to_datetime(df.index), name="date")
         else:
             raise ValueError("Frequency not supported")
+    else:
+        raise ValueError("Frequency not supported")
 
     df.loc[:, "change"] = df.close.pct_change() * 100
     df.loc[:, "open_change"] = ((df.open / df.close.shift(1)) - 1) * 100
     df.loc[:, "abs_change"] = abs(df.change)
     df.loc[:, "abs_open_change"] = abs(df.open_change)
     df.loc[:, "realized_vol"] = df.abs_change * multiplier
 
+    if frequency in ["D-MON", "D-TUE", "D-WED", "D-THU", "D-FRI"]:
+        day_of_week = frequency.split("-")[1]
+        df = df[df.index.day_name().str.upper().str.contains(day_of_week)]
+
     if _print:
         print(
             "Vol for period: {:0.2f}%, IV: {:0.2f}%".format(
                 df.abs_change.mean(), df.abs_change.mean() * multiplier
             )
         )
     else:
@@ -157,15 +168,25 @@
         recent_vol = get_recent_vol(
             symbol_monthly_data, periods=periods, ignore_last=ignore_last
         )
         df_dict[symbol] = recent_vol
     return df_dict
 
 
-def ratio_analysis(x_df, y_df, periods_to_avg, return_summary=False):
+def ratio_analysis(
+        x_df: pd.DataFrame,
+        y_df: pd.DataFrame,
+        periods_to_avg: int = None,
+        return_summary=True,
+        add_rolling: bool | int = False
+):
+
+    if periods_to_avg is None:
+        periods_to_avg = len(x_df)
+
     x_close = x_df.iloc[-periods_to_avg:].close
     x_array = x_df.iloc[-periods_to_avg:].abs_change
     x_avg = x_array.mean()
 
     y_close = y_df.iloc[-periods_to_avg:].close
     y_array = y_df.iloc[-periods_to_avg:].abs_change
     y_avg = y_array.mean()
@@ -186,17 +207,38 @@
         }
     )
     # print(f'\n{periods_to_avg} Period Average = {avg_ratio}\n\n')
     if return_summary:
         ratio_summary.loc["Summary"] = ratio_summary.mean()
         ratio_summary.loc["Summary", "Ratio"] = avg_ratio
 
+    if add_rolling:
+        rolling_x_avg = x_array.rolling(add_rolling, min_periods=1).mean()
+        rolling_y_avg = y_array.rolling(add_rolling, min_periods=1).mean()
+        rolling_ratio = rolling_x_avg / rolling_y_avg
+        ratio_summary[f"Rolling {add_rolling} Ratio"] = rolling_ratio
+
     return ratio_summary
 
 
+def get_summary_ratio(target_symbol, benchmark_symbol, frequency='D', periods_to_avg=50):
+
+    try:
+        dc = DataClient(__import__('os').getenv('EOD_API_KEY'))
+    except ApiKeyNotFound:
+        return None
+
+    benchmark = dc.get_data(benchmark_symbol)
+    target = dc.get_data(target_symbol)
+    benchmark = analyser(benchmark, frequency=frequency)
+    target = analyser(target, frequency=frequency)
+    ratio = ratio_analysis(target, benchmark, periods_to_avg=periods_to_avg)
+    return ratio.loc['Summary', 'Ratio']
+
+
 @retain_name
 def generate_streak(df, query):
     df = df.copy(deep=True)
 
     # Create a boolean series with the query
     _bool = df.query(f"{query}")
     df["result"] = df.index.isin(_bool.index)
@@ -227,54 +269,87 @@
                 days = ["mon", "tue", "wed", "thu", "fri"]
                 return [f"{frequency}-{day}" for day in days]
             else:
                 return [frequency]
         else:
             return [frequency]
 
-    def _calculate_streak_summary(dataframe, frequency):
+    def _calculate_streak_summary(df, frequency, query):
+
+        # Calculate the streak summary
+
+        if df.index[-1].replace(hour=15, minute=30) > atf.currenttime():
+            df = df.iloc[:-1]
+        check_date = df.index[-1]
+        total_instances = len(df)
+        df = generate_streak(df, query)
+        total_streaks = len(df)
+        number_of_positive_events = total_instances - total_streaks
+        event_occurrence_pct = number_of_positive_events / total_instances
+
         df = (
-            dataframe.reset_index()
+            df.reset_index()
             .groupby("streak_id")
             .agg({"date": ["min", "max"], "streak_count": "max"})
             .reset_index()
         )
         df.columns = ["streak_id", "start_date", "end_date", "streak_count"]
 
         # Check if there is an ongoing streak
         current_streak = (
-            df.iloc[-1].streak_count
-            if pd.Timestamp.today().date() <= df.iloc[-1].end_date.date()
-            else False
+            df.iloc[-1].streak_count if df.iloc[-1].end_date == check_date else None
         )
 
+        # Calculating the percentile of the current streak
+        if current_streak:
+            current_streak_percentile = (
+                    df.streak_count.sort_values().values.searchsorted(current_streak) / len(df)
+            )
+        else:
+            current_streak_percentile = 0
+
         return {
             "freq": frequency,  # Use the given freq value instead of df.iloc[-1].name
+            "total_instances": total_instances,
+            "total_streaks": total_streaks,
+            "event_occurrence": event_occurrence_pct,
             "longest_streak": df.streak_count.max(),
             "longest_streak_start": df.start_date[df.streak_count.idxmax()],
             "longest_streak_end": df.end_date[df.streak_count.idxmax()],
             "current_streak": current_streak,
+            "current_streak_percentile": current_streak_percentile,
             "dataframe": df,
         }
 
-    def print_streak_summary(streak_summary):
+    def print_streak_summary(summary):
         print(
-            f"{streak_summary['freq']} - longest streak: {streak_summary['longest_streak']} "
-            f"from {streak_summary['longest_streak_start']:%d %b %Y} to {streak_summary['longest_streak_end']:%d %b %Y}"
+            f"Query: {dataframe.name} {query}\n"
+            f"Frequency: {summary['freq']}\n"
+            f"Total Instances: {summary['total_instances']}\n"
+            f"Total Streaks: {summary['total_streaks']}\n"
+            f"Event Occurrence: {summary['event_occurrence']}\n"
+            f"Longest Streak: {summary['longest_streak']}\n"
+            f"Longest Streak Start: {summary['longest_streak_start']}\n"
+            f"Longest Streak End: {summary['longest_streak_end']}\n"
+            f"Current Streak: {summary['current_streak']}\n"
+            f"Current Streak Percentile: {summary['current_streak_percentile']}\n"
         )
-        if streak_summary["current_streak"]:
-            print(f"Current streak: {streak_summary['current_streak']}\n")
 
     freqs = generate_frequency(freq)
-
     streaks = []
     for freq in freqs:
-        df = analyser(instrument, frequency=freq)
-        df = generate_streak(df, query)
-        streak_summary = _calculate_streak_summary(df, freq)
+        dataframe = analyser(instrument, frequency=freq)
+        if query == "abs_change":
+            recommended_threshold = dataframe.abs_change.mean() * 0.70  # 0.70 should cover 50% of the data
+            # (mildly adjusted for abnormal distribution)
+            recommended_threshold = round(recommended_threshold, 2)
+            recommended_sign = ">" if dataframe.iloc[-2].abs_change > recommended_threshold else "<"
+            query = f"abs_change {recommended_sign} {recommended_threshold}"
+            print(f"Recommended query: {query}\n")
+        streak_summary = _calculate_streak_summary(dataframe, freq, query)
         streaks.append(streak_summary)
         print_streak_summary(streak_summary)
     # Convert the list of dictionaries to a list of DataFrames
     streaks_df = [pd.DataFrame([streak]) for streak in streaks]
 
     # Concatenate the list of DataFrames
     return (
@@ -383,15 +458,15 @@
     index_monthly_data = analyser(index_data, frequency="M-THU")
     index_monthly_data = index_monthly_data[["close", "abs_change"]]
     index_monthly_data.columns = ["index_close", "index_abs_change"]
 
     if simulate_backtest:
         if index_symbol == "BANKNIFTY":
             index_ivs = pd.read_csv(
-                "BANKNIFTY_IV_DATA.csv",
+                "data/banknifty_ivs.csv",
                 parse_dates=True,
                 index_col="date",
                 dayfirst=True,
             )
             index_ivs.index = pd.to_datetime(index_ivs.index)
             index_ivs = index_ivs.resample("D").ffill()
             index_monthly_data = index_monthly_data.merge(
```

### Comparing `autotrading-0.8.8/autotrader/discord_bot.py` & `autotrading-0.9.0/autotrader/discord_bot.py`

 * *Files identical despite different names*

### Comparing `autotrading-0.8.8/autotrader/nsefunctions.py` & `autotrading-0.9.0/autotrader/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `autotrading-0.8.8/autotrader/strategies.py` & `autotrading-0.9.0/autotrader/strategies.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         pin=pin,
         apikey=apikey,
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
     nifty = atf.Index("NIFTY", webhook_url=discord_webhook_url)
     bnf = atf.Index("BANKNIFTY", webhook_url=discord_webhook_url)
-    fin = atf.Index("FINNIFTY", webhook_url=discord_webhook_url, spot_future_rate=0.01)
+    fin = atf.Index("FINNIFTY", webhook_url=discord_webhook_url, spot_future_rate=0.05)
 
     indices = atf.indices_to_trade(
         nifty, bnf, fin, multi_before_weekend=multi_before_weekend
     )
     quantity_multiplier = 2 if len(indices) == 1 else 1
     parameters["quantity_in_lots"] = (
         parameters["quantity_in_lots"] * quantity_multiplier
@@ -108,14 +108,77 @@
     # Call the data appender function on the traded indices
     for index in indices:
         atf.append_data_to_json(
             index.order_log, f"{user}_{index.name}_straddle_log.json"
         )
 
 
+def intraday_strangles_on_indices(
+    parameters,
+    client=None,
+    user=None,
+    pin=None,
+    apikey=None,
+    authkey=None,
+    webhook_url=None,
+    start_time=(9, 16),
+    multi_before_weekend=True,
+):
+    user, pin, apikey, authkey, discord_webhook_url = get_user_data(
+        client, user, pin, apikey, authkey, webhook_url
+    )
+
+    # If today is a holiday, the script will exit
+    if atf.currenttime().date() in atf.holidays:
+        atf.notifier("Today is a holiday. Exiting.", discord_webhook_url)
+        exit()
+
+    atf.login(
+        user=user,
+        pin=pin,
+        apikey=apikey,
+        authkey=authkey,
+        webhook_url=discord_webhook_url,
+    )
+    nifty = atf.Index("NIFTY", webhook_url=discord_webhook_url)
+    bnf = atf.Index("BANKNIFTY", webhook_url=discord_webhook_url)
+    fin = atf.Index("FINNIFTY", webhook_url=discord_webhook_url, spot_future_rate=0.05)
+
+    indices = atf.indices_to_trade(
+        nifty, bnf, fin, multi_before_weekend=multi_before_weekend
+    )
+    quantity_multiplier = 2 if len(indices) == 1 else 1
+    parameters["quantity_in_lots"] = (
+        parameters["quantity_in_lots"] * quantity_multiplier
+    )
+
+    strangle_threads = []
+    for index in indices:
+        atf.notifier(f"Trading {index.name} strangle.", discord_webhook_url)
+        thread = threading.Thread(target=index.intraday_strangle, kwargs=parameters)
+        strangle_threads.append(thread)
+
+    # Wait for the market to open
+    while atf.currenttime().time() < time(*start_time):
+        pass
+
+    # Start the straddle threads
+    for thread in strangle_threads:
+        thread.start()
+
+    for thread in strangle_threads:
+        thread.join()
+
+    # Call the data appender function on the traded indices
+    for index in indices:
+        atf.append_data_to_json(
+            index.order_log, f"{user}_{index.name}_strangle_log.json"
+        )
+
+
 def overnight_straddle_nifty(
     quantity_in_lots,
     client=None,
     user=None,
     pin=None,
     apikey=None,
     authkey=None,
```

### Comparing `autotrading-0.8.8/autotrading.egg-info/requires.txt` & `autotrading-0.9.0/autotrading.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,27 @@
 nest-asyncio==1.5.6
 numpy==1.24.2
 packaging==23.0
 pandas==1.5.3
 parso==0.8.3
 pickleshare==0.7.5
 platformdirs==2.6.2
+plotly==5.14.1
 prompt-toolkit==3.0.36
 psutil==5.9.4
 pure-eval==0.2.2
 Pygments==2.14.0
 pyotp==2.8.0
 python-dateutil==2.8.2
 python-Levenshtein==0.21.0
 pytz==2022.7.1
 pywin32==305
 pyzmq==25.0.0
 requests==2.28.2
+scikit-learn==1.2.2
 scipy==1.10.1
 six==1.16.0
 smartapi-python==1.3.0
 spyder-kernels>=2.2.1
 stack-data==0.6.2
 tornado==6.2
 traitlets==5.8.1
```

### Comparing `autotrading-0.8.8/setup.cfg` & `autotrading-0.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7574 6f74 7261 6469 6e67 0d0a   = autotrading..
-00000020: 7665 7273 696f 6e20 3d20 302e 382e 380d  version = 0.8.8.
+00000020: 7665 7273 696f 6e20 3d20 302e 392e 300d  version = 0.9.0.
 00000030: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
 00000040: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
 00000050: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
 00000060: 203a 3a20 330d 0a09 5072 6f67 7261 6d6d   :: 3...Programm
 00000070: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
 00000080: 5079 7468 6f6e 203a 3a20 332e 360d 0a09  Python :: 3.6...
 00000090: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
@@ -38,39 +38,41 @@
 00000250: 796e 6369 6f3d 3d31 2e35 2e36 0d0a 096e  yncio==1.5.6...n
 00000260: 756d 7079 3d3d 312e 3234 2e32 0d0a 0970  umpy==1.24.2...p
 00000270: 6163 6b61 6769 6e67 3d3d 3233 2e30 0d0a  ackaging==23.0..
 00000280: 0970 616e 6461 733d 3d31 2e35 2e33 0d0a  .pandas==1.5.3..
 00000290: 0970 6172 736f 3d3d 302e 382e 330d 0a09  .parso==0.8.3...
 000002a0: 7069 636b 6c65 7368 6172 653d 3d30 2e37  pickleshare==0.7
 000002b0: 2e35 0d0a 0970 6c61 7466 6f72 6d64 6972  .5...platformdir
-000002c0: 733d 3d32 2e36 2e32 0d0a 0970 726f 6d70  s==2.6.2...promp
-000002d0: 742d 746f 6f6c 6b69 743d 3d33 2e30 2e33  t-toolkit==3.0.3
-000002e0: 360d 0a09 7073 7574 696c 3d3d 352e 392e  6...psutil==5.9.
-000002f0: 340d 0a09 7075 7265 2d65 7661 6c3d 3d30  4...pure-eval==0
-00000300: 2e32 2e32 0d0a 0950 7967 6d65 6e74 733d  .2.2...Pygments=
-00000310: 3d32 2e31 342e 300d 0a09 7079 6f74 703d  =2.14.0...pyotp=
-00000320: 3d32 2e38 2e30 0d0a 0970 7974 686f 6e2d  =2.8.0...python-
-00000330: 6461 7465 7574 696c 3d3d 322e 382e 320d  dateutil==2.8.2.
-00000340: 0a09 7079 7468 6f6e 2d4c 6576 656e 7368  ..python-Levensh
-00000350: 7465 696e 3d3d 302e 3231 2e30 0d0a 0970  tein==0.21.0...p
-00000360: 7974 7a3d 3d32 3032 322e 372e 310d 0a09  ytz==2022.7.1...
-00000370: 7079 7769 6e33 323d 3d33 3035 0d0a 0970  pywin32==305...p
-00000380: 797a 6d71 3d3d 3235 2e30 2e30 0d0a 0972  yzmq==25.0.0...r
-00000390: 6571 7565 7374 733d 3d32 2e32 382e 320d  equests==2.28.2.
-000003a0: 0a09 7363 6970 793d 3d31 2e31 302e 310d  ..scipy==1.10.1.
-000003b0: 0a09 7369 783d 3d31 2e31 362e 300d 0a09  ..six==1.16.0...
-000003c0: 736d 6172 7461 7069 2d70 7974 686f 6e3d  smartapi-python=
-000003d0: 3d31 2e33 2e30 0d0a 0973 7079 6465 722d  =1.3.0...spyder-
-000003e0: 6b65 726e 656c 733e 3d32 2e32 2e31 0d0a  kernels>=2.2.1..
-000003f0: 0973 7461 636b 2d64 6174 613d 3d30 2e36  .stack-data==0.6
-00000400: 2e32 0d0a 0974 6f72 6e61 646f 3d3d 362e  .2...tornado==6.
-00000410: 320d 0a09 7472 6169 746c 6574 733d 3d35  2...traitlets==5
-00000420: 2e38 2e31 0d0a 0975 726c 6c69 6233 3d3d  .8.1...urllib3==
-00000430: 312e 3236 2e31 340d 0a09 7763 7769 6474  1.26.14...wcwidt
-00000440: 683d 3d30 2e32 2e36 0d0a 0977 6562 736f  h==0.2.6...webso
-00000450: 636b 6574 2d63 6c69 656e 743d 3d31 2e35  cket-client==1.5
-00000460: 2e31 0d0a 0978 6c72 643d 3d32 2e30 2e31  .1...xlrd==2.0.1
-00000470: 0d0a 0979 6669 6e61 6e63 653d 3d30 2e32  ...yfinance==0.2
-00000480: 2e31 340d 0a0d 0a5b 6567 675f 696e 666f  .14....[egg_info
-00000490: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000004a0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000004b0: 0a                                       .
+000002c0: 733d 3d32 2e36 2e32 0d0a 0970 6c6f 746c  s==2.6.2...plotl
+000002d0: 793d 3d35 2e31 342e 310d 0a09 7072 6f6d  y==5.14.1...prom
+000002e0: 7074 2d74 6f6f 6c6b 6974 3d3d 332e 302e  pt-toolkit==3.0.
+000002f0: 3336 0d0a 0970 7375 7469 6c3d 3d35 2e39  36...psutil==5.9
+00000300: 2e34 0d0a 0970 7572 652d 6576 616c 3d3d  .4...pure-eval==
+00000310: 302e 322e 320d 0a09 5079 676d 656e 7473  0.2.2...Pygments
+00000320: 3d3d 322e 3134 2e30 0d0a 0970 796f 7470  ==2.14.0...pyotp
+00000330: 3d3d 322e 382e 300d 0a09 7079 7468 6f6e  ==2.8.0...python
+00000340: 2d64 6174 6575 7469 6c3d 3d32 2e38 2e32  -dateutil==2.8.2
+00000350: 0d0a 0970 7974 686f 6e2d 4c65 7665 6e73  ...python-Levens
+00000360: 6874 6569 6e3d 3d30 2e32 312e 300d 0a09  htein==0.21.0...
+00000370: 7079 747a 3d3d 3230 3232 2e37 2e31 0d0a  pytz==2022.7.1..
+00000380: 0970 7977 696e 3332 3d3d 3330 350d 0a09  .pywin32==305...
+00000390: 7079 7a6d 713d 3d32 352e 302e 300d 0a09  pyzmq==25.0.0...
+000003a0: 7265 7175 6573 7473 3d3d 322e 3238 2e32  requests==2.28.2
+000003b0: 0d0a 0973 6369 6b69 742d 6c65 6172 6e3d  ...scikit-learn=
+000003c0: 3d31 2e32 2e32 0d0a 0973 6369 7079 3d3d  =1.2.2...scipy==
+000003d0: 312e 3130 2e31 0d0a 0973 6978 3d3d 312e  1.10.1...six==1.
+000003e0: 3136 2e30 0d0a 0973 6d61 7274 6170 692d  16.0...smartapi-
+000003f0: 7079 7468 6f6e 3d3d 312e 332e 300d 0a09  python==1.3.0...
+00000400: 7370 7964 6572 2d6b 6572 6e65 6c73 3e3d  spyder-kernels>=
+00000410: 322e 322e 310d 0a09 7374 6163 6b2d 6461  2.2.1...stack-da
+00000420: 7461 3d3d 302e 362e 320d 0a09 746f 726e  ta==0.6.2...torn
+00000430: 6164 6f3d 3d36 2e32 0d0a 0974 7261 6974  ado==6.2...trait
+00000440: 6c65 7473 3d3d 352e 382e 310d 0a09 7572  lets==5.8.1...ur
+00000450: 6c6c 6962 333d 3d31 2e32 362e 3134 0d0a  llib3==1.26.14..
+00000460: 0977 6377 6964 7468 3d3d 302e 322e 360d  .wcwidth==0.2.6.
+00000470: 0a09 7765 6273 6f63 6b65 742d 636c 6965  ..websocket-clie
+00000480: 6e74 3d3d 312e 352e 310d 0a09 786c 7264  nt==1.5.1...xlrd
+00000490: 3d3d 322e 302e 310d 0a09 7966 696e 616e  ==2.0.1...yfinan
+000004a0: 6365 3d3d 302e 322e 3134 0d0a 0d0a 5b65  ce==0.2.14....[e
+000004b0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000004c0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000004d0: 203d 2030 0d0a 0d0a                       = 0....
```

