# Comparing `tmp/thetagang-1.6.0.tar.gz` & `tmp/thetagang-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thetagang-1.6.0.tar", max compression
+gzip compressed data, was "thetagang-1.6.1.tar", max compression
```

## Comparing `thetagang-1.6.0.tar` & `thetagang-1.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    34523 2023-06-03 13:21:31.628847 thetagang-1.6.0/LICENSE
--rw-r--r--   0        0        0    14673 2023-06-03 13:21:31.628847 thetagang-1.6.0/README.md
--rw-r--r--   0        0        0     1634 2023-06-03 13:21:31.632847 thetagang-1.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/__init__.py
--rw-r--r--   0        0        0     8247 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/config.py
--rw-r--r--   0        0        0     1068 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/config_defaults.py
--rw-r--r--   0        0        0     1461 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/dict_merge.py
--rw-r--r--   0        0        0       59 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/entry.py
--rw-r--r--   0        0        0     1091 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/fmt.py
--rw-r--r--   0        0        0     1022 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/main.py
--rw-r--r--   0        0        0      376 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/options.py
--rw-r--r--   0        0        0    67559 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/portfolio_manager.py
--rw-r--r--   0        0        0     3951 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/test_util.py
--rwxr-xr-x   0        0        0     8433 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/thetagang.py
--rw-r--r--   0        0        0     5488 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/util.py
--rw-r--r--   0        0        0    15885 1970-01-01 00:00:00.000000 thetagang-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-07 22:18:40.144360 thetagang-1.6.1/LICENSE
+-rw-r--r--   0        0        0    14673 2023-06-07 22:18:40.144360 thetagang-1.6.1/README.md
+-rw-r--r--   0        0        0     1634 2023-06-07 22:18:40.144360 thetagang-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 22:18:40.148360 thetagang-1.6.1/thetagang/__init__.py
+-rw-r--r--   0        0        0     8247 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/config.py
+-rw-r--r--   0        0        0     1068 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/config_defaults.py
+-rw-r--r--   0        0        0     1461 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/dict_merge.py
+-rw-r--r--   0        0        0       59 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/entry.py
+-rw-r--r--   0        0        0     1091 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/fmt.py
+-rw-r--r--   0        0        0     1022 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/main.py
+-rw-r--r--   0        0        0      376 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/options.py
+-rw-r--r--   0        0        0    69028 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/portfolio_manager.py
+-rw-r--r--   0        0        0     3951 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/test_util.py
+-rwxr-xr-x   0        0        0     8433 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/thetagang.py
+-rw-r--r--   0        0        0     5488 2023-06-07 22:18:40.152360 thetagang-1.6.1/thetagang/util.py
+-rw-r--r--   0        0        0    15885 1970-01-01 00:00:00.000000 thetagang-1.6.1/PKG-INFO
```

### Comparing `thetagang-1.6.0/LICENSE` & `thetagang-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/README.md` & `thetagang-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/pyproject.toml` & `thetagang-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "ThetaGang is an IBKR bot for getting money"
 documentation = "https://github.com/brndnmtthws/thetagang/blob/master/README.md"
 homepage = "https://github.com/brndnmtthws/thetagang"
 license = "AGPL-3.0-only"
 name = "thetagang"
 readme = "README.md"
 repository = "https://github.com/brndnmtthws/thetagang.git"
-version = "1.6.0"
+version = "1.6.1"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 click-log = "^0.4.0"
 ib_insync = "^0.9.81"
 python = ">=3.9,<4.0"
 python-dateutil = "^2.8.1"
```

### Comparing `thetagang-1.6.0/thetagang/config.py` & `thetagang-1.6.1/thetagang/config.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/thetagang/config_defaults.py` & `thetagang-1.6.1/thetagang/config_defaults.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/thetagang/dict_merge.py` & `thetagang-1.6.1/thetagang/dict_merge.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/thetagang/fmt.py` & `thetagang-1.6.1/thetagang/fmt.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/thetagang/main.py` & `thetagang-1.6.1/thetagang/main.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/thetagang/portfolio_manager.py` & `thetagang-1.6.1/thetagang/portfolio_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import math
 import sys
 from functools import lru_cache
+from typing import Optional
 
 from ib_insync import Order, Ticker, util
 from ib_insync.contract import ComboLeg, Contract, Index, Option, Stock, TagValue
 from ib_insync.order import LimitOrder
 from rich import box
 from rich.console import Console, Group
 from rich.panel import Panel
@@ -33,15 +34,15 @@
 from .options import option_dte
 
 console = Console()
 
 # Typically the amount of time needed when waiting on data from the IBKR API.
 # Sometimes it can take a while to retrieve data, and it's lazy-loaded by the
 # API, so getting this number right is largely a matter of guesswork.
-API_RESPONSE_WAIT_TIME = 90
+API_RESPONSE_WAIT_TIME = 60
 
 
 # Turn off some of the more annoying logging output from ib_insync
 logging.getLogger("ib_insync.ib").setLevel(logging.ERROR)
 logging.getLogger("ib_insync.wrapper").setLevel(logging.CRITICAL)
 
 
@@ -76,20 +77,22 @@
         return self.get_options(portfolio_positions, "C")
 
     def get_puts(self, portfolio_positions):
         return self.get_options(portfolio_positions, "P")
 
     def get_options(self, portfolio_positions, right):
         ret = []
+        symbols = set(self.get_symbols())
         for symbol in portfolio_positions:
             ret = ret + list(
                 filter(
                     lambda p: (
                         isinstance(p.contract, Option)
                         and p.contract.right.startswith(right)
+                        and p.contract.symbol in symbols
                     ),
                     portfolio_positions[symbol],
                 )
             )
 
         return ret
 
@@ -309,14 +312,15 @@
         return False
 
     def call_is_itm(self, contract):
         # Special case for handling VIX
         if contract.symbol == "VIX":
             vix_contract = Index("VIX", "CBOE", "USD")
             self.ib.qualifyContracts(vix_contract)
+            self.ib.reqMktData(vix_contract)
             vix_ticker = self.get_ticker_for(vix_contract)
             return contract.strike <= vix_ticker.marketPrice()
 
         ticker = self.get_ticker_for_stock(contract.symbol, contract.primaryExchange)
 
         return contract.strike <= ticker.marketPrice()
 
@@ -1279,23 +1283,24 @@
         if not target_dte:
             target_dte = self.config["target"]["dte"]
         if not target_delta:
             target_delta = get_target_delta(self.config, main_contract.symbol, right)
 
         console.print(
             f"[green]Searching option chain for symbol={main_contract.symbol} "
-            f"right={right}, strike_limit={strike_limit}, minimum_price={dfmt(minimum_price,3)} preferred_minimum_price={dfmt(preferred_minimum_price,3)}"
+            f"right={right}, strike_limit={strike_limit}, minimum_price={dfmt(minimum_price,3)} "
+            f"preferred_minimum_price={dfmt(preferred_minimum_price,3)}"
             " this can take a while...[/green]",
         )
         with console.status(
             "[bold blue_violet]Hunting for juicy contracts... 😎"
         ) as status:
             self.ib.qualifyContracts(main_contract)
 
-            main_contract_ticker = self.get_ticker_for(main_contract)
+            main_contract_ticker = self.get_ticker_for(main_contract, midpoint=True)
             main_contract_price = midpoint_or_market_price(main_contract_ticker)
 
             chains = self.get_chains_for_contract(main_contract)
             chain = next(c for c in chains if c.exchange == main_contract.exchange)
 
             def valid_strike(strike):
                 if right.startswith("P") and strike_limit:
@@ -1316,15 +1321,14 @@
 
             chain_expirations = self.config["option_chains"]["expirations"]
             min_dte = (
                 option_dte(exclude_expirations_before)
                 if exclude_expirations_before
                 else 0
             )
-
             strikes = sorted(strike for strike in chain.strikes if valid_strike(strike))
             expirations = sorted(
                 exp
                 for exp in chain.expirations
                 if option_dte(exp) >= target_dte and option_dte(exp) >= min_dte
             )[:chain_expirations]
             rights = [right]
@@ -1502,165 +1506,190 @@
         def inner_handler():
             if not self.config["vix_call_hedge"]["enabled"]:
                 to_print.append(
                     "🛑 VIX call hedging not enabled, skipping",
                 )
                 return
 
+            def vix_calls_should_be_closed() -> (
+                tuple[bool, Optional[Ticker], Optional[float]]
+            ):
+                if "close_hedges_when_vix_exceeds" in self.config["vix_call_hedge"]:
+                    vix_contract = Index("VIX", "CBOE", "USD")
+                    self.ib.qualifyContracts(vix_contract)
+                    self.ib.reqMktData(vix_contract)
+                    vix_ticker = self.get_ticker_for(vix_contract)
+                    close_hedges_when_vix_exceeds = self.config["vix_call_hedge"][
+                        "close_hedges_when_vix_exceeds"
+                    ]
+                    if vix_ticker.marketPrice() > close_hedges_when_vix_exceeds:
+                        return (True, vix_ticker, close_hedges_when_vix_exceeds)
+                    return (False, vix_ticker, close_hedges_when_vix_exceeds)
+                return (False, None, None)
+
             with console.status(
                 "[bold blue_violet]Checking on our VIX call hedge..."
             ) as status:
                 net_vix_call_count = net_option_positions(
                     "VIX", portfolio_positions, "C"
                 )
                 if net_vix_call_count > 0:
                     status.update(
-                        f"[bold blue_violet]net_vix_call_count={net_vix_call_count}, checking if we need to close positions...",
+                        f"[bold blue_violet]net_vix_call_count={net_vix_call_count}, "
+                        "checking if we need to close positions...",
                     )
-                    if "close_hedges_when_vix_exceeds" in self.config["vix_call_hedge"]:
-                        vix_contract = Index("VIX", "CBOE", "USD")
-                        self.ib.qualifyContracts(vix_contract)
-                        vix_ticker = self.get_ticker_for(vix_contract)
-                        close_hedges_when_vix_exceeds = self.config["vix_call_hedge"][
-                            "close_hedges_when_vix_exceeds"
-                        ]
-                        if vix_ticker.marketPrice() > close_hedges_when_vix_exceeds:
+                    (
+                        close_vix_calls,
+                        vix_ticker,
+                        close_hedges_when_vix_exceeds,
+                    ) = vix_calls_should_be_closed()
+                    if close_vix_calls and vix_ticker and close_hedges_when_vix_exceeds:
+                        to_print.append(
+                            f"[deep_sky_blue1]VIX={vix_ticker.marketPrice()}, which exceeds "
+                            f"vix_call_hedge.close_hedges_when_vix_exceeds={close_hedges_when_vix_exceeds}"
+                        )
+                        status.update(
+                            f"[bold blue_violet]VIX={vix_ticker.marketPrice()}, which exceeds "
+                            f"vix_call_hedge.close_hedges_when_vix_exceeds={close_hedges_when_vix_exceeds}, "
+                            "checking if we need to close positions...",
+                        )
+                        for position in portfolio_positions["VIX"]:
+                            if (
+                                position.contract.right.startswith("C")
+                                and position.position < 0
+                            ):
+                                # only applies to long calls
+                                continue
                             to_print.append(
-                                f"[deep_sky_blue1]VIX={vix_ticker.marketPrice()}, which exceeds "
-                                f"vix_call_hedge.close_hedges_when_vix_exceeds={close_hedges_when_vix_exceeds}"
+                                f"[blue]Closing position {position.contract.localSymbol}"
                             )
                             status.update(
-                                f"[bold blue_violet]VIX={vix_ticker.marketPrice()}, which exceeds "
-                                f"vix_call_hedge.close_hedges_when_vix_exceeds={close_hedges_when_vix_exceeds}, "
-                                "checking if we need to close positions...",
+                                f"[bold blue_violet]Creating closing order for {position.contract.localSymbol}..."
+                            )
+                            position.contract.exchange = self.get_order_exchange()
+                            sell_ticker = self.get_ticker_for(
+                                position.contract, midpoint=True
+                            )
+                            price = round(get_lower_price(sell_ticker), 2)
+                            qty = abs(position.position)
+                            order = LimitOrder(
+                                "SELL",
+                                qty,
+                                price,
+                                algoStrategy=self.get_algo_strategy(),
+                                algoParams=self.get_algo_params(),
+                                tif="DAY",
+                                account=self.account_number,
                             )
-                            for position in portfolio_positions["VIX"]:
-                                if (
-                                    position.contract.right.startswith("C")
-                                    and position.position < 0
-                                ):
-                                    # only applies to long calls
-                                    continue
-                                to_print.append(
-                                    f"[blue]Closing position {position.contract.localSymbol}"
-                                )
-                                status.update(
-                                    f"[bold blue_violet]Creating closing order for {position.contract.localSymbol}..."
-                                )
-                                position.contract.exchange = self.get_order_exchange()
-                                sell_ticker = self.get_ticker_for(
-                                    position.contract, midpoint=True
-                                )
-                                price = round(get_lower_price(sell_ticker), 2)
-                                qty = abs(position.position)
-                                order = LimitOrder(
-                                    "SELL",
-                                    qty,
-                                    price,
-                                    algoStrategy=self.get_algo_strategy(),
-                                    algoParams=self.get_algo_params(),
-                                    tif="DAY",
-                                    account=self.account_number,
-                                )
 
-                                self.enqueue_order(sell_ticker.contract, order)
+                            self.enqueue_order(sell_ticker.contract, order)
 
                     to_print.append(
                         f"[cyan1]net_vix_call_count={net_vix_call_count}, no action is needed at this time",
                     )
                     return
                 else:
                     status.update(
                         f"[bold blue_violet]net_vix_call_count={net_vix_call_count}, checking if we should open new positions...",
                     )
 
-                try:
-                    vixmo_contract = Index("VIXMO", "CBOE", "USD")
-                    self.ib.qualifyContracts(vixmo_contract)
-                    self.ib.reqMktData(vixmo_contract)
-                    vixmo_ticker = self.get_ticker_for(vixmo_contract)
-
-                    weight = 0.0
-
-                    for allocation in self.config["vix_call_hedge"]["allocation"]:
-                        if (
-                            "lower_bound" in allocation
-                            and "upper_bound" in allocation
-                            and allocation["lower_bound"]
-                            <= vixmo_ticker.marketPrice()
-                            < allocation["upper_bound"]
-                        ):
-                            weight = allocation["weight"]
-                            break
-                        elif (
-                            "lower_bound" in allocation
-                            and allocation["lower_bound"] <= vixmo_ticker.marketPrice()
-                        ):
-                            weight = allocation["weight"]
-                            break
-                        elif (
-                            "upper_bound" in allocation
-                            and vixmo_ticker.marketPrice() < allocation["upper_bound"]
-                        ):
-                            weight = allocation["weight"]
-                            break
+                (
+                    close_vix_calls,
+                    vix_ticker,
+                    close_hedges_when_vix_exceeds,
+                ) = vix_calls_should_be_closed()
+                # we never want to write calls if we're simultaneously ready to close calls
+                if not close_vix_calls:
+                    try:
+                        vixmo_contract = Index("VIXMO", "CBOE", "USD")
+                        self.ib.qualifyContracts(vixmo_contract)
+                        self.ib.reqMktData(vixmo_contract)
+                        vixmo_ticker = self.get_ticker_for(vixmo_contract)
+
+                        weight = 0.0
+
+                        for allocation in self.config["vix_call_hedge"]["allocation"]:
+                            if (
+                                "lower_bound" in allocation
+                                and "upper_bound" in allocation
+                                and allocation["lower_bound"]
+                                <= vixmo_ticker.marketPrice()
+                                < allocation["upper_bound"]
+                            ):
+                                weight = allocation["weight"]
+                                break
+                            elif (
+                                "lower_bound" in allocation
+                                and allocation["lower_bound"]
+                                <= vixmo_ticker.marketPrice()
+                            ):
+                                weight = allocation["weight"]
+                                break
+                            elif (
+                                "upper_bound" in allocation
+                                and vixmo_ticker.marketPrice()
+                                < allocation["upper_bound"]
+                            ):
+                                weight = allocation["weight"]
+                                break
 
-                    to_print.append(
-                        f"VIXMO={vixmo_ticker.marketPrice()}, target call hedge weight={weight}",
-                    )
-
-                    allocation_amount = (
-                        float(account_summary["NetLiquidation"].value) * weight
-                    )
-                    delta = self.config["vix_call_hedge"]["delta"]
-                    if weight > 0:
                         to_print.append(
-                            f"[green]Current VIXMO spot price prescribes an allocation of up to "
-                            f"${allocation_amount:.2f} for purchasing VIX calls, at or above delta={delta} with a DTE >= 30",
+                            f"VIXMO={vixmo_ticker.marketPrice()}, target call hedge weight={weight}",
                         )
-                    else:
-                        to_print.append(
-                            "[cyan1]Based on current VIXMO value and rules, no action is needed",
+
+                        allocation_amount = (
+                            float(account_summary["NetLiquidation"].value) * weight
                         )
-                        return
+                        delta = self.config["vix_call_hedge"]["delta"]
+                        if weight > 0:
+                            to_print.append(
+                                f"[green]Current VIXMO spot price prescribes an allocation of up to "
+                                f"${allocation_amount:.2f} for purchasing VIX calls, at or above delta={delta} with a DTE >= 30",
+                            )
+                        else:
+                            to_print.append(
+                                "[cyan1]Based on current VIXMO value and rules, no action is needed",
+                            )
+                            return
 
-                    status.update(
-                        "[bold blue_violet]Scanning VIX option chain for eligible contracts...",
-                    )
-                    vix_contract = Index("VIX", "CBOE", "USD")
-                    self.ib.qualifyContracts(vix_contract)
+                        status.update(
+                            "[bold blue_violet]Scanning VIX option chain for eligible contracts...",
+                        )
+                        vix_contract = Index("VIX", "CBOE", "USD")
+                        self.ib.qualifyContracts(vix_contract)
+                        self.ib.reqMktData(vix_contract)
 
-                    status.stop()
-                    buy_ticker = self.find_eligible_contracts(
-                        vix_contract, "C", 0, target_delta=delta, target_dte=30
-                    )
-                    status.start()
-                    price = round(get_lower_price(buy_ticker), 2)
-                    qty = math.floor(
-                        allocation_amount
-                        / price
-                        / float(buy_ticker.contract.multiplier)
-                    )
-
-                    order = LimitOrder(
-                        "BUY",
-                        qty,
-                        price,
-                        algoStrategy=self.get_algo_strategy(),
-                        algoParams=self.get_algo_params(),
-                        tif="DAY",
-                        account=self.account_number,
-                    )
-
-                    self.enqueue_order(buy_ticker.contract, order)
-                except RuntimeError:
-                    console.print_exception()
-                    console.print(
-                        "[yellow]Error occurred when VIX call hedging. Continuing anyway...",
-                    )
+                        status.stop()
+                        buy_ticker = self.find_eligible_contracts(
+                            vix_contract, "C", 0, target_delta=delta, target_dte=30
+                        )
+                        status.start()
+                        price = round(get_lower_price(buy_ticker), 2)
+                        qty = math.floor(
+                            allocation_amount
+                            / price
+                            / float(buy_ticker.contract.multiplier)
+                        )
+
+                        order = LimitOrder(
+                            "BUY",
+                            qty,
+                            price,
+                            algoStrategy=self.get_algo_strategy(),
+                            algoParams=self.get_algo_params(),
+                            tif="DAY",
+                            account=self.account_number,
+                        )
+
+                        self.enqueue_order(buy_ticker.contract, order)
+                    except RuntimeError:
+                        console.print_exception()
+                        console.print(
+                            "[yellow]Error occurred when VIX call hedging. Continuing anyway...",
+                        )
 
         inner_handler()
 
         console.print(Panel(Group(*to_print), title="VIX call hedging"))
 
     def enqueue_order(self, contract: Contract, order: Order):
         self.orders.append((contract, order))
```

### Comparing `thetagang-1.6.0/thetagang/test_util.py` & `thetagang-1.6.1/thetagang/test_util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/thetagang/thetagang.py` & `thetagang-1.6.1/thetagang/thetagang.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/thetagang/util.py` & `thetagang-1.6.1/thetagang/util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.6.0/PKG-INFO` & `thetagang-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetagang
-Version: 1.6.0
+Version: 1.6.1
 Summary: ThetaGang is an IBKR bot for getting money
 Home-page: https://github.com/brndnmtthws/thetagang
 License: AGPL-3.0-only
 Author: Brenden Matthews
 Author-email: brenden@brndn.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

