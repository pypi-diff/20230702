# Comparing `tmp/martin_binance-1.3.2.post2.tar.gz` & `tmp/martin_binance-1.3.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-1.3.2.post2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-1.3.2.post3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-1.3.2.post2.tar` & `martin_binance-1.3.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1079 2023-07-01 14:30:02.560426 martin_binance-1.3.2.post2/LICENSE
--rwxr-xr-x   0        0        0     4025 2023-07-01 14:30:02.560426 martin_binance-1.3.2.post2/README.md
--rw-r--r--   0        0        0     2015 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/__init__.py
--rw-r--r--   0        0        0     4642 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2946 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    14575 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6721 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6716 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6722 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4707 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/client.py
--rw-r--r--   0        0        0   186091 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    83511 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16282 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1282 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1427 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/pyproject.toml
--rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 martin_binance-1.3.2.post2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-02 16:21:19.194030 martin_binance-1.3.2.post3/LICENSE
+-rwxr-xr-x   0        0        0     4025 2023-07-02 16:21:19.194030 martin_binance-1.3.2.post3/README.md
+-rw-r--r--   0        0        0     2015 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/__init__.py
+-rw-r--r--   0        0        0     4642 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2946 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    14575 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6721 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6716 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6722 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4707 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/client.py
+-rw-r--r--   0        0        0   186162 2023-07-02 16:21:19.238031 martin_binance-1.3.2.post3/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2023-07-02 16:21:19.242031 martin_binance-1.3.2.post3/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2023-07-02 16:21:19.242031 martin_binance-1.3.2.post3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2023-07-02 16:21:19.242031 martin_binance-1.3.2.post3/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-07-02 16:21:19.242031 martin_binance-1.3.2.post3/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    83217 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16282 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1282 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1427 2023-07-02 16:21:19.246031 martin_binance-1.3.2.post3/pyproject.toml
+-rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 martin_binance-1.3.2.post3/PKG-INFO
```

### Comparing `martin_binance-1.3.2.post2/LICENSE` & `martin_binance-1.3.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/README.md` & `martin_binance-1.3.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/__init__.py` & `martin_binance-1.3.2.post3/martin_binance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.2-2"
+__version__ = "1.3.2-3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 STANDALONE = True
```

### Comparing `martin_binance-1.3.2.post2/martin_binance/backtest/OoTSP.py` & `martin_binance-1.3.2.post3/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/backtest/VCoSEL.py` & `martin_binance-1.3.2.post3/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/backtest/exchange_simulator.py` & `martin_binance-1.3.2.post3/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/cli_0_BTCUSDT.py.template` & `martin_binance-1.3.2.post3/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/cli_1_BTCUSDT.py.template` & `martin_binance-1.3.2.post3/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin_binance-1.3.2.post3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/client.py` & `martin_binance-1.3.2.post3/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/executor.py` & `martin_binance-1.3.2.post3/martin_binance/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.2-2"
+__version__ = "1.3.2-3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -1444,15 +1444,15 @@
                 self.cancel_order_id = self.tp_order_id
                 self.cancel_order(self.tp_order_id)
             return
         if self.tp_wait_id:
             # Wait tp order and cancel in on_cancel_order_success and restart
             self.tp_cancel = True
             return
-        ff, fs, _, _ = self.get_free_assets()
+        ff, fs, _, _ = self.get_free_assets(mode='available')
         # Save initial funds and cycle statistics to .db for external analytics
         if self.first_run:
             if MODE in ('T', 'TC'):
                 self.start_process()
             self.save_init_assets(ff, fs)
         if self.restart:
             # Check refunding before restart
@@ -1714,14 +1714,15 @@
             close.append(i.close)
         n = 1
         while n <= len(high) - 1:
             i = max(high[n] - low[n], abs(high[n] - close[n - 1]), abs(low[n] - close[n - 1]))
             if i:
                 tr_arr.append(i)
             n += 1
+        # noinspection PyTypeChecker
         return statistics.geometric_mean(tr_arr)
 
     def adx(self, adx_candle_size_in_minutes: int, adx_number_of_candles: int, adx_period: int) -> Dict[str, float]:
         """
         Average Directional Index
         Math from https://blog.quantinsti.com/adx-indicator-python/
         Test data
@@ -1837,29 +1838,29 @@
                          f"! ======================================")
 
     def get_free_assets(self, ff: Decimal = None, fs: Decimal = None, mode: str = 'total', backtest=False) -> ():
         """
         Get free asset for current trade pair
         :param fs:
         :param ff:
-        :param mode: 'total', 'free', 'reserved'
+        :param mode: 'total', 'available', 'reserved', 'free'
         :param backtest: bool
         :return: (ff, fs, ft, free_asset: str)
         """
         if ff is None or fs is None:
             funds = self.get_buffered_funds()
             _ff = funds.get(self.f_currency, 0)
             _fs = funds.get(self.s_currency, 0)
             ff = Decimal('0')
             fs = Decimal('0')
             if _ff and _fs:
                 if mode == 'total':
                     ff = f2d(_ff.total_for_currency)
                     fs = f2d(_fs.total_for_currency)
-                elif mode == 'free':
+                elif mode == 'available':
                     ff = f2d(_ff.available)
                     fs = f2d(_fs.available)
                 elif mode == 'reserved':
                     ff = f2d(_ff.reserved)
                     fs = f2d(_fs.reserved)
         #
         if mode == 'free':
```

### Comparing `martin_binance-1.3.2.post2/martin_binance/funds_rate.db.template` & `martin_binance-1.3.2.post3/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin_binance-1.3.2.post3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/margin_wrapper.py` & `martin_binance-1.3.2.post3/martin_binance/margin_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 margin.de <-> Python strategy <-> <margin_wrapper> <-> exchanges-wrapper <-> Exchanges API/WSS
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.2-2"
+__version__ = "1.3.2-3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import simplejson as json
 import logging
@@ -44,17 +44,19 @@
 from martin_binance.client import Trade
 from martin_binance.backtest.exchange_simulator import Account as backTestAccount
 
 ORDER_BOOK_PKL = "order_book.pkl"
 TICKER_PKL = "ticker.pkl"
 
 # For more channel options, please see https://grpc.io/grpc/core/group__grpc__arg__keys.html
-CHANNEL_OPTIONS = [('grpc.lb_policy_name', 'pick_first'),
-                   ('grpc.enable_retries', 0),
-                   ('grpc.keepalive_timeout_ms', 10000)]
+CHANNEL_OPTIONS = [
+    ('grpc.lb_policy_name', 'pick_first'),
+    ('grpc.enable_retries', 0),
+    ('grpc.keepalive_timeout_ms', 10000)
+]
 
 loop = asyncio.get_event_loop()
 KLINES_INIT = [Interval.ONE_MINUTE, Interval.FIFTY_MINUTES, Interval.ONE_HOUR]
 KLINES_LIM = 50  # Number of candles must be <= 1000
 CANCEL_ALL_ORDERS = True  # Ask about cancel all active orders before start strategy and ms.LOAD_LAST_STATE = 0
 TRADES_LIST_LIMIT = 100
 HEARTBEAT = 2  # Sec
@@ -493,17 +495,15 @@
         cls = StrategyBase
         cls.ticker = {}
         cls.funds = {}
         cls.order_book = {}
         cls.order_id = int(datetime.now().strftime("%S%M")) * 1000
         cls.wait_order_id = []  # List of placed orders for time-out detect
         cls.canceled_order_id = []  # List canceled orders  for time-out detect
-        cls.all_trades = []  # List of all (limit = ALL_TRADES_LIST_LIMIT) trades for a specific account and symbol
         cls.trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
-        cls.all_orders = []  # List of all open orders for symbol
         cls.orders = {}  # Set of orders associated with strategy
         cls.strategy.get_buffered_funds_last_time = cls.strategy.get_time()
         cls.rate_limiter = RATE_LIMITER
         cls.start_time_ms = int(time.time() * 1000)
         cls.backtest = {}
         cls.bulk_orders_cancel = {}
 
@@ -1037,30 +1037,28 @@
                                          color=ms.Style.GREEN)
 
             _orders = await cls.send_request(cls.stub.FetchOpenOrders, api_pb2.MarketRequest, symbol=cls.symbol)
             if _orders is None:
                 raise UserWarning("Can't fetch open orders")
             StrategyBase.rate_limiter = max(StrategyBase.rate_limiter, _orders.rate_limiter)
             orders = json_format.MessageToDict(_orders).get('items', [])
-            # print(f"buffered_orders.orders: {orders}")
             part_id = []
             for order in orders:
                 _id = int(order['orderId'])
                 exch_orders[_id] = Order(order)
                 if (order.get('status', None) == 'PARTIALLY_FILLED'
                         and order_trades_sum(_id) < Decimal(order['executedQty'])):
                     part_id.append(_id)
             # Add TP id
             if cls.strategy.tp_order_id:
                 save_orders_id.append(cls.strategy.tp_order_id)
             # Add grid id's
             save_orders_id.extend(list(cls.orders))
             # Missed fill event list
             diff_id = list(set(save_orders_id).difference(set(exch_orders)))
-            # print(f"buffered_orders.diff_id: {diff_id}")
             # Erroneously not deleted order
             diff_excess_id = list(set(exch_orders).
                                   difference(save_orders_id).
                                   intersection(cls.canceled_order_id))
             # print(f"buffered_orders.diff_excess_id: {diff_excess_id}")
 
             if diff_id or part_id:
@@ -1172,42 +1170,41 @@
 
 
 def on_order_update_handler(cls, ed):
     if (cls.symbol == ed['symbol']
             and (cls.strategy.order_exist(ed['order_id']) or cls.strategy.tp_order_id == ed['order_id'])
             and ed['order_status'] in ('FILLED', 'PARTIALLY_FILLED')):
         if ed['order_status'] == 'FILLED':
-            # Remove from all_orders and orders lists
+            # Remove from orders dict
             remove_from_orders_lists([ed['order_id']])
         if trade_not_exist(ed['order_id'], ed['trade_id']):
             trade = {"qty": ed['last_executed_quantity'],
                      "isBuyer": bool(ed['side'] == 'BUY'),
                      "id": ed['trade_id'],
                      "orderId": ed['order_id'],
                      "price": ed['last_executed_price'],
                      "time": ed['transaction_time']}
-            #  Append to all_trades and trades list
-            if len(cls.trades) > TRADES_LIST_LIMIT:
-                del cls.trades[0]
+            #  Append to trades list
             cls.trades.append(PrivateTrade(trade))
+            # noinspection PyStatementEffect
+            cls.trades[-TRADES_LIST_LIMIT:]
             cumulative_quantity = Decimal(ed['cumulative_filled_quantity'])
             saved_filled_quantity = order_trades_sum(ed['order_id'])
             if ed['order_status'] == 'FILLED' and saved_filled_quantity != cumulative_quantity:
                 cls.strategy.message_log(f"Order: {ed['order_id']} was missed partially filling event",
                                          log_level=LogLevel.INFO)
                 # Remove trades associated with order from list
                 remove_from_trades_lists(ed['order_id'])
                 # Update current trade
                 price = str(Decimal(ed['quote_asset_transacted']) / Decimal(ed['cumulative_filled_quantity']))
                 trade.update({"qty": ed['cumulative_filled_quantity'], "price": price})
                 # cls.strategy.message_log(f"on_order_update.trade: {trade}",
                 #                                  log_level=LogLevel.DEBUG, color=ms.Style.YELLOW)
                 # Append to list
                 cls.trades.append(PrivateTrade(trade))
-                cls.all_trades.append(PrivateTrade(trade))
             cls.strategy.on_order_update(OrderUpdate(ed))
 
 
 async def create_limit_order(_id: int, buy: bool, amount: str, price: str) -> None:
     cls = StrategyBase
     try:
         if ms.MODE in ('T', 'TC'):
@@ -1262,15 +1259,15 @@
                          "price": price,
                          "time": order.timestamp}
                 # cls.strategy.message_log(f"place_limit_order_callback.trade: {trade}", color=ms.Style.YELLOW)
                 if len(cls.trades) > TRADES_LIST_LIMIT:
                     del cls.trades[0]
                 cls.trades.append(PrivateTrade(trade))
             if executed_qty < orig_qty:
-                cls.orders[order.id] =  order
+                cls.orders[order.id] = order
             if ms.MODE == 'TC' and cls.strategy.start_collect:
                 cls.strategy.open_orders_snapshot()
             elif ms.MODE == 'S':
                 await on_funds_update()
             cls.strategy.on_place_order_success(_id, order)
 
 
@@ -1304,15 +1301,15 @@
             if check_status.get('status') == 'CANCELED':
                 # For stop timeout firing
                 cls.canceled_order_id.append(_id)
     except Exception as _ex:
         cls.strategy.message_log(f"Exception on cancel order call for {_id}:\n{_ex}")
     else:
         # print(f"cancel_order_call.result: {result}")
-        # Remove from all_orders and orders lists
+        # Remove from orders lists
         if result:
             remove_from_orders_lists([_id])
             cls.strategy.message_log(f"Cancel order {_id} success", color=ms.Style.GREEN)
             cls.strategy.on_cancel_order_success(_id, Order(result))
             cls.canceled_order_id.append(_id)
             if ms.MODE == 'TC' and cls.strategy.start_collect:
                 cls.strategy.open_orders_snapshot()
@@ -1332,15 +1329,15 @@
     except grpc.RpcError as ex:
         status_code = ex.code()
         cls.strategy.message_log(f"Exception on cancel all orders for {_id}: {status_code.name}, {ex.details()}")
     except Exception as _ex:
         cls.strategy.message_log(f"Exception on cancel all orders for {_id}:\n{_ex}")
     else:
         # print(f"cancel_all_order_call.result: {result}")
-        # Remove from all_orders and orders lists
+        # Remove from orders lists
         if result and result.get('status') == 'CANCELED':
             remove_from_orders_lists([_id])
             cls.strategy.message_log(f"Cancel order {_id} success", color=ms.Style.GREEN)
             cls.canceled_order_id.append(_id)
             cls.strategy.on_cancel_order_success(_id, Order(result), cancel_all=True)
 
 
@@ -1365,19 +1362,22 @@
         pass  # Task cancellation should not be logged as an error.
     except Exception as _ex:
         cls.strategy.message_log(f"Exception in fetch_order: {_ex}", log_level=LogLevel.ERROR)
         return {}
     else:
         cls.strategy.message_log(f"For order {_id} fetched status is {result.get('status')}",
                                  log_level=LogLevel.INFO)
-        if _filled_update_call and result and result.get('status') == 'CANCELED':
+        if _filled_update_call and result.get('status') == 'CANCELED':
             remove_from_orders_lists([_id])
             cls.canceled_order_id.append(_id)
             cls.strategy.message_log(f"Order {_id} has already been deleted", color=ms.Style.GREEN)
             cls.strategy.on_cancel_order_success(_id, Order(result))
+        elif not result:
+            remove_from_orders_lists([_id])
+            cls.strategy.message_log(f"Order {_id} status fixed", color=ms.Style.GREEN)
         return result
 
 
 async def transfer2master(symbol: str, amount: str):
     cls = StrategyBase
     try:
         res = await cls.send_request(cls.stub.TransferToMaster,
```

### Comparing `martin_binance-1.3.2.post2/martin_binance/ms_cfg.toml.template` & `martin_binance-1.3.2.post3/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/service/funds_rate_exporter.py` & `martin_binance-1.3.2.post3/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/service/grafana.json` & `martin_binance-1.3.2.post3/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/martin_binance/service/relaunch.py` & `martin_binance-1.3.2.post3/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/pyproject.toml` & `martin_binance-1.3.2.post3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2.post2/PKG-INFO` & `martin_binance-1.3.2.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.2.post2
+Version: 1.3.2.post3
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.2.post2 Summary: Free
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.2.post3 Summary: Free
 trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: exchanges-wrapper==1.3.2 Requires-Dist: margin-strategy-sdk==0.0.11
```

