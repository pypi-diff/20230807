# Comparing `tmp/volstreet-1.1.0.tar.gz` & `tmp/volstreet-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.1.0.tar", last modified: Sun Aug  6 15:10:22 2023, max compression
+gzip compressed data, was "volstreet-1.2.0.tar", last modified: Mon Aug  7 09:13:26 2023, max compression
```

## Comparing `volstreet-1.1.0.tar` & `volstreet-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 15:10:22.571510 volstreet-1.1.0/
--rw-rw-rw-   0        0        0      497 2023-08-06 15:10:22.571510 volstreet-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.1.0/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-08-06 15:10:22.572323 volstreet-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 15:10:22.561394 volstreet-1.1.0/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.1.0/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.1.0/volstreet/__init__.py
--rw-rw-rw-   0        0        0    10080 2023-08-06 14:57:40.000000 volstreet-1.1.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2716 2023-08-03 18:56:13.000000 volstreet-1.1.0/volstreet/constants.py
--rw-rw-rw-   0        0        0    43826 2023-07-28 13:59:59.000000 volstreet-1.1.0/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   202207 2023-08-04 16:01:04.000000 volstreet-1.1.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.1.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      729 2023-08-02 13:31:19.000000 volstreet-1.1.0/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.1.0/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    14350 2023-08-04 10:10:12.000000 volstreet-1.1.0/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-08-06 15:10:22.570006 volstreet-1.1.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 09:13:26.811662 volstreet-1.2.0/
+-rw-rw-rw-   0        0        0      497 2023-08-07 09:13:26.811662 volstreet-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.2.0/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-08-07 09:13:26.812659 volstreet-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 09:13:26.806675 volstreet-1.2.0/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.2.0/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.2.0/volstreet/__init__.py
+-rw-rw-rw-   0        0        0    10080 2023-08-06 14:57:40.000000 volstreet-1.2.0/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2716 2023-08-03 18:56:13.000000 volstreet-1.2.0/volstreet/constants.py
+-rw-rw-rw-   0        0        0    43826 2023-07-28 13:59:59.000000 volstreet-1.2.0/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   203180 2023-08-07 09:12:22.000000 volstreet-1.2.0/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.2.0/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      729 2023-08-02 13:31:19.000000 volstreet-1.2.0/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.2.0/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    14632 2023-08-06 16:51:52.000000 volstreet-1.2.0/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:13:26.811662 volstreet-1.2.0/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.1.0/setup.cfg` & `volstreet-1.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 312e 300d 0a61  rsion = 1.1.0..a
+00000020: 7273 696f 6e20 3d20 312e 322e 300d 0a61  rsion = 1.2.0..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-1.1.0/volstreet/SmartWebSocketV2.py` & `volstreet-1.2.0/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.1.0/volstreet/blackscholes.py` & `volstreet-1.2.0/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.1.0/volstreet/constants.py` & `volstreet-1.2.0/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.1.0/volstreet/datamodule.py` & `volstreet-1.2.0/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.1.0/volstreet/dealingroom.py` & `volstreet-1.2.0/volstreet/dealingroom.py`

 * *Files 7% similar despite different names*

```diff
@@ -874,15 +874,15 @@
                 f"Order rejected for {index} {expiry} {qty_in_lots} Buy {buy_strike} Sell {sell_strike}"
             )
 
 
 class Index:
     """Initialize an index with the name of the index in uppercase"""
 
-    def __init__(self, name, webhook_url=None, websocket=None, spot_future_rate=0.06):
+    def __init__(self, name, spot_future_rate=0.06):
         if name not in symbol_df["SYMBOL"].values:
             closest_match, confidence = process.extractOne(
                 name, symbol_df["SYMBOL"].values
             )
             if confidence > 80:
                 raise Exception(
                     f"Index {name} not found. Did you mean {closest_match}?"
@@ -895,15 +895,14 @@
         self.ltp = None
         self.previous_close = None
         self.current_expiry = None
         self.next_expiry = None
         self.month_expiry = None
         self.fut_expiry = None
         self.order_log = defaultdict(list)
-        self.webhook_url = webhook_url
         self.spot_future_rate = spot_future_rate
         self.symbol, self.token = fetch_symbol_token(self.name)
         self.lot_size = fetch_lot_size(self.name)
         self.fetch_expirys(self.symbol)
         self.freeze_qty = self.fetch_freeze_limit()
         self.available_strikes = None
         self.available_straddle_strikes = None
@@ -923,26 +922,14 @@
         else:
             self.exchange_type = 1
 
         logger.info(
             f"Initialized {self.name} with lot size {self.lot_size}, base {self.base} and freeze qty {self.freeze_qty}"
         )
 
-        if websocket:
-            try:
-                websocket.subscribe(
-                    websocket.correlation_id,
-                    1,
-                    [{"exchangeType": self.exchange_type, "tokens": [self.token]}],
-                )
-                sleep(2)
-                print(f"{self.name}: Subscribed underlying to the websocket")
-            except Exception as e:
-                print(f"{self.name}: Websocket subscription failed. {e}")
-
     def __repr__(self):
         return (
             f"{self.__class__.__name__}(Name: {self.name}, Lot Size: {self.lot_size}, "
             f"Freeze Qty: {self.freeze_qty}, Current Expiry: {self.current_expiry}, Symbol: {self.symbol}, "
             f"Token: {self.token})"
         )
 
@@ -954,31 +941,23 @@
             df = pd.read_excel(response.content)
             df.columns = df.columns.str.strip()
             df["SYMBOL"] = df["SYMBOL"].str.strip()
             freeze_qty = df[df["SYMBOL"] == self.name]["VOL_FRZ_QTY"].values[0]
             freeze_qty_in_lots = freeze_qty / self.lot_size
             return int(freeze_qty_in_lots)
         except requests.exceptions.Timeout as e:
-            notifier(
-                f"Timeout error in fetching freeze limit for {self.name}: {e}",
-                self.webhook_url,
-            )
+            logger.error(f"Timeout error in fetching freeze limit for {self.name}: {e}")
             freeze_qty_in_lots = 20
             return int(freeze_qty_in_lots)
         except requests.exceptions.HTTPError as e:
-            notifier(
-                f"HTTP error in fetching freeze limit for {self.name}: {e}",
-                self.webhook_url,
-            )
+            logger.error(f"HTTP error in fetching freeze limit for {self.name}: {e}")
             freeze_qty_in_lots = 20
             return int(freeze_qty_in_lots)
         except Exception as e:
-            notifier(
-                f"Error in fetching freeze limit for {self.name}: {e}", self.webhook_url
-            )
+            logger.error(f"Error in fetching freeze limit for {self.name}: {e}")
             freeze_qty_in_lots = 20
             return freeze_qty_in_lots
 
     def fetch_expirys(self, symbol: str):
         expirymask = (
             (scrips.expiry != "")
             & (scrips.exch_seg == "NFO")
@@ -1166,26 +1145,28 @@
         buy_or_sell,
         quantity_in_lots,
         strike=None,
         call_strike=None,
         put_strike=None,
         return_avg_price=False,
         order_tag="",
+        notification_url=None,
     ):
         """
         Places a straddle or strangle order on the index.
         Params:
         strike: Strike price of the option (for straddle)
         expiry: Expiry of the option
         buy_or_sell: BUY or SELL
         quantity_in_lots: Quantity in lots
         call_strike: Strike price of the call (for strangle)
         put_strike: Strike price of the put (for strangle)
         return_avg_price: If True, returns the average price of the order
         order_tag: Tag to be added to the order
+        notification_url: URL to be notified when the order is placed
         """
 
         if strike is None:
             if call_strike is None and put_strike is None:
                 raise ValueError("Strike price not specified")
             strike_info = f"{call_strike}CE {put_strike}PE"
         elif call_strike is None and put_strike is None:
@@ -1242,15 +1223,15 @@
 
         if all(call_order_statuses == "complete") and all(
             put_order_statuses == "complete"
         ):
             notifier(
                 f"{order_prefix}Order(s) placed successfully for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s).",
-                self.webhook_url,
+                notification_url,
             )
             call_order_avg_price = (
                 lookup_and_return(
                     orderbook, "orderid", call_order_id_list, "averageprice"
                 )
                 .astype(float)
                 .mean()
@@ -1268,40 +1249,40 @@
                 return
         elif all(call_order_statuses == "rejected") and all(
             put_order_statuses == "rejected"
         ):
             notifier(
                 f"{order_prefix}All orders rejected for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s).",
-                self.webhook_url,
+                notification_url,
             )
             raise Exception("Orders rejected")
         elif any(call_order_statuses == "open") or any(put_order_statuses == "open"):
             notifier(
                 f"{order_prefix}Some orders pending for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s). You can modify the orders.",
-                self.webhook_url,
+                notification_url,
             )
             if return_avg_price:
                 return call_price, put_price
         elif any(call_order_statuses == "rejected") or any(
             put_order_statuses == "rejected"
         ):
             notifier(
                 f"{order_prefix}Some orders rejected for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s). You can place the rejected orders again.",
-                self.webhook_url,
+                notification_url,
             )
             if return_avg_price:
                 return call_price, put_price
         else:
             notifier(
                 f"{order_prefix}ERROR. Order statuses uncertain for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s).",
-                self.webhook_url,
+                notification_url,
             )
             raise Exception("Order statuses uncertain")
 
     def place_synthetic_fut(
         self,
         strike,
         expiry,
@@ -1320,15 +1301,21 @@
             prices,
             stop_loss_order,
             order_tag,
         )
 
     @time_the_function
     def find_equal_strike(
-        self, exit_time, websocket, wait_for_equality, target_disparity, expiry=None
+        self,
+        exit_time,
+        websocket,
+        wait_for_equality,
+        target_disparity,
+        expiry=None,
+        notification_url=None,
     ):
         expiry = expiry or self.current_expiry
         ltp = (
             self.fetch_ltp()
             if not websocket
             else websocket.price_dict.get(self.token, 0)["ltp"]
         )
@@ -1430,21 +1417,21 @@
                 if currenttime() - last_print_time > print_interval:
                     print(message)
                     last_print_time = currenttime()
                 if currenttime() - last_log_time > log_interval:
                     logger.info(message)
                     last_log_time = currenttime()
                 if currenttime() - last_notify_time > notify_interval:
-                    notifier(message, self.webhook_url)
+                    notifier(message, notification_url)
                     last_notify_time = currenttime()
 
                 if (currenttime() + timedelta(minutes=5)).time() > time(*exit_time):
                     notifier(
                         "Equal strike tracker exited due to time limit.",
-                        self.webhook_url,
+                        notification_url,
                     )
                     raise Exception("Equal strike tracker exited due to time limit.")
 
         idx = np.argmin(disparities)
         (
             strike_to_trade,
             call_symbol,
@@ -1471,42 +1458,48 @@
             put_token,
             call_ltp,
             put_ltp,
         )
 
     @log_errors
     def rollover_overnight_short_straddle(
-        self, quantity_in_lots, strike_offset=1, iv_threshold=0.95, take_avg_price=False
+        self,
+        quantity_in_lots,
+        strike_offset=1,
+        iv_threshold=0.95,
+        take_avg_price=False,
+        notification_url=None,
     ):
         """Rollover overnight short straddle to the next expiry.
         Args:
             quantity_in_lots (int): Quantity of the straddle in lots.
             strike_offset (float): Strike offset from the current strike.
             iv_threshold (float): IV threshold compared to vix.
             take_avg_price (bool): Take average price of the index over 5m timeframes.
+            notification_url (str): Webhook URL to send notifications.
         """
 
         def load_data():
             try:
                 with open(f"{obj.userId}_overnight_positions.json", "r") as f:
                     data = json.load(f)
                     return data
             except FileNotFoundError:
                 data = {}
                 notifier(
                     "No positions found for overnight straddle. Creating new file.",
-                    self.webhook_url,
+                    notification_url,
                 )
                 with open(f"{obj.userId}_overnight_positions.json", "w") as f:
                     json.dump(data, f)
                 return data
             except Exception as e:
                 notifier(
                     f"Error while reading overnight_positions.json: {e}",
-                    self.webhook_url,
+                    notification_url,
                 )
                 logger.error(
                     f"Error while reading positions.json",
                     exc_info=(type(e), e, e.__traceback__),
                 )
                 raise Exception("Error while reading positions.json")
 
@@ -1515,22 +1508,22 @@
                 json.dump(data, f)
 
         avg_ltp = None
         if take_avg_price:
             if currenttime().time() < time(15, 00):
                 notifier(
                     f"{self.name} Cannot take avg price before 3pm. Try running the strategy after 3pm",
-                    self.webhook_url,
+                    notification_url,
                 )
                 raise Exception(
                     "Cannot take avg price before 3pm. Try running the strategy after 3pm"
                 )
             notifier(
                 f"{self.name} Taking average price of the index over 5m timeframes.",
-                self.webhook_url,
+                notification_url,
             )
             price_list = [self.fetch_ltp()]
             while currenttime().time() < time(15, 28):
                 _ltp = self.fetch_ltp()
                 price_list.append(_ltp)
                 sleep(60)
             avg_ltp = np.mean(price_list)
@@ -1541,219 +1534,217 @@
         if self.name in ["FINNIFTY", "BANKNIFTY"]:
             beta = dm.get_summary_ratio(
                 self.name, "NIFTY"
             )  # beta of the index vs nifty since vix is of nifty
             beta = 1.3 if beta is None else beta
             vix = vix * beta
 
-        order_tag = "Overnight Short Straddle"
+        order_tag = "Overnight short straddle"
 
         weekend_in_expiry = check_for_weekend(self.current_expiry)
         ltp = avg_ltp if avg_ltp else self.fetch_ltp()
         sell_strike = findstrike(ltp * strike_offset, self.base)
-        call_ltp, put_ltp = fetch_straddle_price(
-            self.name, self.current_expiry, sell_strike
-        )
-        call_iv, put_iv, iv = straddle_iv(
-            call_ltp, put_ltp, ltp, sell_strike, timetoexpiry(self.current_expiry)
+        sell_straddle = Straddle(
+            strike=sell_strike, underlying=self.name, expiry=self.current_expiry
         )
+        call_iv, put_iv, iv = sell_straddle.ivs()
         iv = iv * 100
 
         # This if-clause checks how far the expiry is
         if weekend_in_expiry:  # far from expiry
             if iv < vix * iv_threshold:
                 notifier(
                     f"{self.name} IV is too low compared to VIX - IV: {iv}, Vix: {vix}.",
-                    self.webhook_url,
+                    notification_url,
                 )
                 return
             else:
                 notifier(
                     f"{self.name} IV is fine compared to VIX - IV: {iv}, Vix: {vix}.",
-                    self.webhook_url,
+                    notification_url,
                 )
         elif (
             timetoexpiry(self.current_expiry, effective_time=True, in_days=True) < 2
         ):  # only exit
             sell_strike = None
             notifier(
                 f"{self.name} Only exiting current position. IV: {iv}, Vix: {vix}.",
-                self.webhook_url,
+                notification_url,
             )
         else:
             notifier(
-                f"{self.name} Rolling over overnight straddle - IV: {iv}, Vix: {vix}.",
-                self.webhook_url,
+                f"{self.name} Deploying overnight straddle - IV: {iv}, Vix: {vix}.",
+                notification_url,
             )
 
         trade_data = load_data()
         buy_strike = trade_data.get(self.name, None)
+        buy_straddle = (
+            Straddle(
+                strike=buy_strike, underlying=self.name, expiry=self.current_expiry
+            )
+            if buy_strike
+            else None
+        )
 
         # Checking if the buy strike is valid
         if (
             not isinstance(buy_strike, int)
             and not isinstance(buy_strike, float)
             and buy_strike is not None
         ):
-            notifier(f"Invalid strike found for {self.name}.", self.webhook_url)
+            notifier(f"Invalid strike found for {self.name}.", notification_url)
             raise Exception(f"Invalid strike found for {self.name}.")
 
+        trade_info_dict = {
+            "Date": currenttime().strftime("%d-%m-%Y %H:%M:%S"),
+            "Underlying": self.name,
+            "Expiry": self.current_expiry,
+        }
+
+        call_buy_avg, put_buy_avg = np.nan, np.nan
+        call_sell_avg, put_sell_avg = np.nan, np.nan
+
         # Placing orders
         if buy_strike is None and sell_strike is None:
-            notifier(f"{self.name} No trade required.", self.webhook_url)
+            notifier(f"{self.name} No trade required.", notification_url)
         elif sell_strike is None:  # only exiting current position
             notifier(
                 f"{self.name} Exiting current position on strike {buy_strike}.",
-                self.webhook_url,
+                notification_url,
             )
-            call_buy_avg, put_buy_avg = self.place_combined_order(
-                self.current_expiry,
+            call_buy_avg, put_buy_avg = place_option_order_and_notify(
+                buy_straddle,
                 "BUY",
                 quantity_in_lots,
-                strike=buy_strike,
-                return_avg_price=True,
-                order_tag=order_tag,
-            )
-            self.log_combined_order(
-                buy_strike,
-                expiry=self.current_expiry,
-                buy_or_sell="BUY",
-                call_price=call_buy_avg,
-                put_price=put_buy_avg,
+                "LIMIT",
                 order_tag=order_tag,
+                webhook_url=notification_url,
+                return_avg_price=True,
             )
+
         elif buy_strike is None:  # only entering new position
             notifier(
                 f"{self.name} Entering new position on strike {sell_strike}.",
-                self.webhook_url,
+                notification_url,
             )
-            call_sell_avg, put_sell_avg = self.place_combined_order(
-                self.current_expiry,
+            call_sell_avg, put_sell_avg = place_option_order_and_notify(
+                sell_straddle,
                 "SELL",
                 quantity_in_lots,
-                strike=sell_strike,
-                return_avg_price=True,
-                order_tag=order_tag,
-            )
-            self.log_combined_order(
-                sell_strike,
-                expiry=self.current_expiry,
-                buy_or_sell="SELL",
-                call_price=call_sell_avg,
-                put_price=put_sell_avg,
+                "LIMIT",
                 order_tag=order_tag,
+                webhook_url=notification_url,
+                return_avg_price=True,
             )
+
         else:  # both entering and exiting positions
             if buy_strike == sell_strike:
                 notifier(
                     f"{self.name} No trade required as strike is same.",
-                    self.webhook_url,
+                    notification_url,
                 )
-                call_ltp, put_ltp = fetch_straddle_price(
-                    self.name, self.current_expiry, sell_strike
-                )
-                self.log_combined_order(
-                    buy_strike,
-                    expiry=self.current_expiry,
-                    buy_or_sell="BUY",
-                    call_price=call_ltp,
-                    put_price=put_ltp,
-                    order_tag=order_tag,
-                )
-                self.log_combined_order(
-                    sell_strike,
-                    expiry=self.current_expiry,
-                    buy_or_sell="SELL",
-                    call_price=call_ltp,
-                    put_price=put_ltp,
-                    order_tag=order_tag,
+                call_ltp, put_ltp = sell_straddle.fetch_ltp()
+                call_buy_avg, put_buy_avg, call_sell_avg, put_sell_avg = (
+                    call_ltp,
+                    put_ltp,
+                    call_ltp,
+                    put_ltp,
                 )
             else:
                 notifier(
                     f"{self.name} Buying {buy_strike} and selling {sell_strike}.",
-                    self.webhook_url,
+                    notification_url,
                 )
-                call_buy_avg, put_buy_avg = self.place_combined_order(
-                    self.current_expiry,
+                call_buy_avg, put_buy_avg = place_option_order_and_notify(
+                    buy_straddle,
                     "BUY",
                     quantity_in_lots,
-                    strike=buy_strike,
-                    return_avg_price=True,
+                    "LIMIT",
                     order_tag=order_tag,
+                    webhook_url=notification_url,
+                    return_avg_price=True,
                 )
-                call_sell_avg, put_sell_avg = self.place_combined_order(
-                    self.current_expiry,
+                call_sell_avg, put_sell_avg = place_option_order_and_notify(
+                    sell_straddle,
                     "SELL",
                     quantity_in_lots,
-                    strike=sell_strike,
-                    return_avg_price=True,
-                    order_tag=order_tag,
-                )
-                self.log_combined_order(
-                    buy_strike,
-                    expiry=self.current_expiry,
-                    buy_or_sell="BUY",
-                    call_price=call_buy_avg,
-                    put_price=put_buy_avg,
-                    order_tag=order_tag,
-                )
-                self.log_combined_order(
-                    sell_strike,
-                    expiry=self.current_expiry,
-                    buy_or_sell="SELL",
-                    call_price=call_sell_avg,
-                    put_price=put_sell_avg,
+                    "LIMIT",
                     order_tag=order_tag,
+                    webhook_url=notification_url,
+                    return_avg_price=True,
                 )
 
+        trade_info_dict.update(
+            {
+                "Buy Strike": buy_strike,
+                "Buy Call Price": call_buy_avg,
+                "Buy Put Price": put_buy_avg,
+                "Buy Total Price": call_buy_avg + put_buy_avg,
+                "Sell Strike": sell_strike,
+                "Sell Call Price": call_sell_avg,
+                "Sell Put Price": put_sell_avg,
+                "Sell Total Price": call_sell_avg + put_sell_avg,
+            }
+        )
+
         trade_data[self.name] = sell_strike
         save_data(trade_data)
 
+        self.strategy_log[order_tag].append(trade_info_dict)
+
     @log_errors
     def buy_weekly_hedge(
         self,
         quantity_in_lots,
         type_of_hedge="strangle",
         strike_offset=1,
         call_offset=1,
         put_offset=1,
+        notification_url=None,
     ):
+        order_tag = "Weekly hedge"
+
         ltp = self.fetch_ltp()
         if type_of_hedge == "strangle":
             call_strike = findstrike(ltp * call_offset, self.base)
             put_strike = findstrike(ltp * put_offset, self.base)
             strike = None
+            instrument = Strangle(call_strike, put_strike, self.name, self.next_expiry)
         elif type_of_hedge == "straddle":
             strike = findstrike(ltp * strike_offset, self.base)
             call_strike = None
             put_strike = None
+            instrument = Straddle(strike, self.name, self.next_expiry)
         else:
             raise Exception("Invalid type of hedge.")
 
-        call_buy_avg, put_buy_avg = self.place_combined_order(
-            self.next_expiry,
+        call_buy_avg, put_buy_avg = place_option_order_and_notify(
+            instrument,
             "BUY",
             quantity_in_lots,
-            strike=strike,
-            call_strike=call_strike,
-            put_strike=put_strike,
-            order_tag="Weekly Hedge",
+            "LIMIT",
+            order_tag=order_tag,
+            webhook_url=notification_url,
             return_avg_price=True,
         )
 
-        self.log_combined_order(
-            strike=strike,
-            call_strike=call_strike,
-            put_strike=put_strike,
-            expiry=self.next_expiry,
-            buy_or_sell="BUY",
-            call_price=call_buy_avg,
-            put_price=put_buy_avg,
-            order_tag="Weekly Hedge",
-        )
+        trade_info_dict = {
+            "Date": currenttime().strftime("%d-%m-%Y %H:%M:%S"),
+            "Underlying": self.name,
+            "Expiry": self.next_expiry,
+            "Buy Strike(s)": strike
+            if strike is not None
+            else (call_strike, put_strike),
+            "Buy Call Price": call_buy_avg,
+            "Buy Put Price": put_buy_avg,
+            "Buy Total Price": call_buy_avg + put_buy_avg,
+        }
+
+        self.strategy_log[order_tag].append(trade_info_dict)
 
     @log_errors
     def intraday_straddle(
         self,
         quantity_in_lots,
         exit_time=(15, 28),
         websocket=None,
@@ -1769,14 +1760,15 @@
         safeguard_movement=0.0035,
         safeguard_spike=1.2,
         smart_exit=False,
         take_profit=False,
         take_profit_points=np.inf,
         convert_to_butterfly=False,
         check_force_exit=False,
+        notification_url=None,
     ):
         """Params:
         quantity_in_lots: int
         exit_time: tuple
         websocket: websocket object
         wait_for_equality: bool
         move_sl: bool
@@ -1814,29 +1806,31 @@
             put_price,
         ) = self.find_equal_strike(
             exit_time=exit_time,
             websocket=websocket,
             wait_for_equality=wait_for_equality,
             target_disparity=target_disparity,
             expiry=expiry,
+            notification_url=notification_url,
         )
 
         notifier(
             f"{self.name}: Initiating intraday trade on {equal_strike} strike.",
-            self.webhook_url,
+            notification_url,
         )
 
         # Placing orders
         call_avg_price, put_avg_price = self.place_combined_order(
             expiry,
             "SELL",
             quantity_in_lots,
             strike=equal_strike,
             return_avg_price=True,
             order_tag=order_tag,
+            notification_url=notification_url,
         )
 
         underlying_price = self.fetch_ltp()
         entry_spot = underlying_price
 
         # Placing stoploss orders
         if stoploss == "fixed":
@@ -1890,19 +1884,19 @@
             orderbook, "orderid", put_stoploss_order_ids, "status"
         )
 
         if all(call_sl_statuses == "trigger pending") and all(
             put_sl_statuses == "trigger pending"
         ):
             notifier(
-                f"{self.name} stoploss orders placed successfully", self.webhook_url
+                f"{self.name} stoploss orders placed successfully", notification_url
             )
         else:
             notifier(
-                f"{self.name} stoploss orders not placed successfully", self.webhook_url
+                f"{self.name} stoploss orders not placed successfully", notification_url
             )
             raise Exception("Stoploss orders not placed successfully")
 
         self.log_combined_order(
             equal_strike,
             expiry=expiry,
             buy_or_sell="SELL",
@@ -1921,15 +1915,15 @@
             put_avg_price,
             entry_spot,
             equal_strike,
             timetoexpiry(expiry),
         )
         summary_iv = traded_avg_iv if traded_avg_iv is not None else 0
         summary_message += f"\nTraded IV: {summary_iv * 100:0.2f}"
-        notifier(summary_message, self.webhook_url)
+        notifier(summary_message, notification_url)
         sleep(1)
 
         def write_force_exit_status(user):
             with open(f"{user}_{self.name}_force_exit.json", "w") as file:
                 json.dump(False, file)
 
         def read_force_exit_status(user):
@@ -2031,15 +2025,15 @@
                 if take_profit and profit_in_pts > (
                     take_profit_points + per_share_charges
                 ):
                     notifier(
                         f"{self.name} take profit exit triggered\n"
                         f"Time: {currenttime().time()}\n"
                         f"Profit: {profit_in_pts}\n",
-                        self.webhook_url,
+                        notification_url,
                     )
                     take_profit_exit = True
 
                 # If no stop-loss is hit, and it is expiry day, then check for potential hedge purchase
                 if (
                     not (callsl or putsl)
                     and days_to_expiry < 1
@@ -2047,15 +2041,15 @@
                     and not ctb_notification_sent
                 ):
                     try:
                         ctb_hedge = process_ctb(ctb_threshold)
                         if ctb_hedge is not None:
                             notifier(
                                 f"{self.name} Convert to butterfly triggered\n",
-                                self.webhook_url,
+                                notification_url,
                             )
                             ctb_trg = True
                             ctb_message = f"Hedged with: {ctb_hedge}\n"
                             ctb_notification_sent = True
                     except Exception as _e:
                         print(f"Error in process_ctb: {_e}")
 
@@ -2096,15 +2090,15 @@
                     if average_delta < smart_exit_delta_threshold:
                         if not smart_exit_notification_sent:
                             notifier(
                                 f"{self.name} smart exit triggered\n"
                                 f"Time: {currenttime().time()}\n"
                                 f"Average delta: {average_delta}\n"
                                 f"Incremental gains: {incremental_gains}\n",
-                                self.webhook_url,
+                                notification_url,
                             )
                             smart_exit_notification_sent = True
                             smart_exit_trg = True
 
                 # Check for force exit
                 if check_force_exit:
                     force_exit = read_force_exit_status(obj.userId)
@@ -2141,15 +2135,15 @@
             """
 
             nonlocal orderbook, call_exit_price, put_exit_price, call_price, put_price, underlying_price
             nonlocal traded_call_iv, traded_put_iv, traded_avg_iv, call_iv, put_iv, avg_iv, entry_spot
 
             orderbook = fetch_orderbook_if_needed(data, refresh)
             triggered, complete = process_stop_loss_order_statuses(
-                orderbook, order_ids, context=f"SL: {side}", notify_url=self.webhook_url
+                orderbook, order_ids, context=f"SL: {side}", notify_url=notification_url
             )
 
             if not triggered and not complete:
                 return False, False
 
             # Checking if there has been an unjustified trigger of stoploss without much movement in the underlying
             # We will also use IV to check if the stoploss was justified or not
@@ -2165,15 +2159,15 @@
                     else traded_avg_iv
                 )
 
                 if present_iv is None or original_iv is None:
                     notifier(
                         f"{self.name} {side.capitalize()} stoploss triggered. "
                         f"Unable to calculate IV spike due to missing IV data.",
-                        self.webhook_url,
+                        notification_url,
                     )
                 else:
                     price_function = bs.call if side == "call" else bs.put
                     iv_spike = present_iv / original_iv
                     ideal_price = price_function(
                         underlying_price,
                         equal_strike,
@@ -2188,23 +2182,23 @@
                     ):
                         notifier(
                             f"{self.name} {side.capitalize()} stoploss triggered without much "
                             f"movement in the underlying or because of IV/Price spike.\n"
                             f"Movement: {movement_from_entry * 100:0.2f}\nPresent IV: {present_iv}\n"
                             f"IV spike: {iv_spike}\nIdeal Price: {ideal_price}\nPresent Price: {present_price}\n"
                             f"Price Spike: {price_spike}",
-                            self.webhook_url,
+                            notification_url,
                         )
                     else:
                         notifier(
                             f"{self.name} {side.capitalize()} stoploss triggered. "
                             f"Movement: {movement_from_entry * 100:0.2f}\nPresent IV: {present_iv}\n"
                             f"IV spike: {iv_spike}\nIdeal Price: {ideal_price}\nPresent Price: {present_price}\n"
                             f"Price Spike: {price_spike}",
-                            self.webhook_url,
+                            notification_url,
                         )
             if complete:
                 exit_price = (
                     lookup_and_return(orderbook, "orderid", order_ids, "averageprice")
                     .astype(float)
                     .mean()
                 )
@@ -2240,15 +2234,15 @@
                 if sl_type == "call"
                 else (underlying_price * (1 + trend_sl))
             )
             notifier(
                 f"{self.name} {sl_type} trend catcher starting. "
                 + f"Placed {qty} lots of {strike} {opt_type} at {option_ltp}. "
                 + f"Stoploss price: {sl_price}, Underlying Price: {underlying_price}",
-                self.webhook_url,
+                notification_url,
             )
             trend_sl_hit = False
             last_print_time = currenttime()
             print_interval = timedelta(seconds=10)
             while not check_exit_conditions(
                 currenttime().time(),
                 time(*exit_time),
@@ -2270,19 +2264,19 @@
                         + f"Stoploss price: {sl_price}, Underlying Price: {underlying_price} "
                         + f"Stoploss hit: {trend_sl_hit}"
                     )
 
             if trend_sl_hit:
                 notifier(
                     f"{self.name} {sl_type} trend catcher stoploss hit.",
-                    self.webhook_url,
+                    notification_url,
                 )
             else:
                 notifier(
-                    f"{self.name} {sl_type} trend catcher exiting.", self.webhook_url
+                    f"{self.name} {sl_type} trend catcher exiting.", notification_url
                 )
 
             for qty in trend_spliced_orders:
                 place_order(symbol, token, qty * self.lot_size, "BUY", "MARKET")
 
         def process_sl_hit(
             sl_type,
@@ -2327,15 +2321,15 @@
                         "BUY",
                         other_avg_price,
                         order_tag=stoploss_tag,
                         stop_loss_order=True,
                     )
                     other_stoploss_order_ids.append(sl_order_id)
 
-            # notifier(f'{self.name} {sl_type} stoploss triggered and completed.', self.webhook_url)
+            # notifier(f'{self.name} {sl_type} stoploss triggered and completed.', notification_url)
 
             refresh = True
             sleep(5)
             while not check_exit_conditions(
                 currenttime().time(),
                 time(*exit_time),
                 sl_dict[other_sl_type],
@@ -2385,24 +2379,29 @@
                 exit_spliced_orders(spliced_orders, "put")
             elif put_stop_loss_hit:
                 sl_type = "Put"
                 exit_spliced_orders(spliced_orders, "call")
             else:
                 sl_type = "None"
                 self.place_combined_order(
-                    expiry, "BUY", quantity_in_lots, strike=equal_strike
+                    expiry,
+                    "BUY",
+                    quantity_in_lots,
+                    strike=equal_strike,
+                    notification_url=notification_url,
                 )
                 if hedged:
                     # noinspection PyUnresolvedReferences
                     self.place_combined_order(
                         expiry,
                         "SELL",
                         quantity_in_lots,
                         call_strike=ctb_hedge.call_strike,
                         put_strike=ctb_hedge.put_strike,
+                        notification_url=notification_url,
                     )
 
             return sl_type
 
         # After placing the orders and stoploss orders setting up nonlocal variables
         in_trade = True
         error_faced = False
@@ -2438,15 +2437,15 @@
                 self.lot_size,
                 quantity_in_lots,
                 self.lot_size,
             )
             break_even_price = total_avg_price - per_share_charges
             notifier(
                 f"{self.name}: Charges per share {per_share_charges} | Break even price {break_even_price}",
-                self.webhook_url,
+                notification_url,
             )
 
         # Setting up stop loss dictionary and starting price thread
         sl_hit_dict = {"call": False, "put": False}
         price_updater = Thread(target=price_tracker)
 
         sleep(5)
@@ -2466,15 +2465,15 @@
                 sl_hit_dict["call"], call_sl_orders_complete = check_sl_orders(
                     call_stoploss_order_ids, "call", refresh=refresh_orderbook
                 )
                 sl_hit_dict["put"], put_sl_orders_complete = check_sl_orders(
                     put_stoploss_order_ids, "put", refresh=refresh_orderbook
                 )
             except Exception as e:
-                notifier(f"{self.name} Error: {e}", self.webhook_url)
+                notifier(f"{self.name} Error: {e}", notification_url)
                 error_faced = True
                 price_updater.join()
                 raise Exception(f"Error: {e}")
 
             if sl_hit_dict["call"]:
                 process_sl_hit(
                     "call",
@@ -2511,17 +2510,18 @@
             self.place_combined_order(
                 expiry,
                 "BUY",
                 quantity_in_lots,
                 call_strike=ctb_hedge.call_strike,
                 put_strike=ctb_hedge.put_strike,
                 order_tag=order_tag + " CTB",
+                notification_url=notification_url,
             )
             cancel_pending_orders(call_stoploss_order_ids + put_stoploss_order_ids)
-            notifier(f"{self.name}: Converted to butterfly", self.webhook_url)
+            notifier(f"{self.name}: Converted to butterfly", notification_url)
             while not check_exit_conditions(currenttime().time(), time(*exit_time)):
                 sleep(3)
 
         # After a complete exit is triggered
         sl_hit_call, sl_hit_put = sl_hit_dict["call"], sl_hit_dict["put"]
 
         # Fetching prices as a backup incase websocket has failed
@@ -2556,21 +2556,21 @@
         }
 
         try:
             self.order_log[order_tag][0].update(exit_dict)
         except Exception as e:
             notifier(
                 f"{self.name}: Error updating order list with exit details. {e}",
-                self.webhook_url,
+                notification_url,
             )
 
         notifier(
             f"{self.name}: Exited positions\n"
             + "".join([f"{key}: {value}\n" for key, value in exit_dict.items()]),
-            self.webhook_url,
+            notification_url,
         )
         in_trade = False
 
     @log_errors
     def intraday_strangle(
         self,
         quantity_in_lots,
@@ -2586,14 +2586,15 @@
         trend_strike_offset=0,
         trend_sl=0.003,
         disparity_threshold=np.inf,
         place_sl_orders=False,
         move_sl_to_cost=False,
         convert_to_butterfly=False,
         shared_data=None,
+        notification_url=None,
     ):
         """Intraday strangle strategy. Trades strangle with stop loss. All offsets are in percentage terms.
         Parameters
         ----------
         quantity_in_lots : int
             Quantity in lots
         call_strike_offset : float, optional
@@ -2624,14 +2625,16 @@
             Place stop loss orders or not, by default False
         move_sl_to_cost : bool, optional
             Move other stop loss to cost or not, by default False
         convert_to_butterfly : bool, optional
             Convert to butterfly or not, by default False
         shared_data : SharedData class, optional
             shared data about client level orderbook and positions, by default None
+        notification_url : str, optional
+            URL for sending notifications, by default None
         """
 
         @log_errors
         def position_monitor(info_dict):
             c_avg_price = info_dict["call_avg_price"]
             p_avg_price = info_dict["put_avg_price"]
             traded_strangle = info_dict["traded_strangle"]
@@ -2744,15 +2747,15 @@
                     and not ctb_notification_sent
                 ):
                     try:
                         ctb_hedge = process_ctb(ctb_threshold)
                         if ctb_hedge is not None:
                             notifier(
                                 f"{self.name} Convert to butterfly triggered\n",
-                                self.webhook_url,
+                                notification_url,
                             )
                             info_dict["exit_triggers"].update(
                                 {"convert_to_butterfly": True}
                             )
                             ctb_message = f"Hedged with: {ctb_hedge}\n"
                             info_dict["ctb_hedge"] = ctb_hedge
                             ctb_notification_sent = True
@@ -2779,15 +2782,15 @@
                 if currenttime() - last_print_time > print_interval:
                     print(message)
                     last_print_time = currenttime()
                 if currenttime() - last_log_time > log_interval:
                     logger.info(message)
                     last_log_time = currenttime()
                 if currenttime() - last_notify_time > notify_interval:
-                    notifier(message, self.webhook_url)
+                    notifier(message, notification_url)
                     last_notify_time = currenttime()
                 sleep(sleep_time)
 
         def get_range_of_strangles(c_strike, p_strike, exp, range_of_strikes=4):
             if range_of_strikes % 2 != 0:
                 range_of_strikes += 1
             c_strike_range = np.arange(
@@ -2822,27 +2825,27 @@
             # Placing the trend option order
             place_option_order_and_notify(
                 trend_option,
                 "SELL",
                 qty_in_lots,
                 "LIMIT",
                 "Intraday Strangle Trend Catcher",
-                self.webhook_url,
+                notification_url,
             )
 
             # Setting up the stop loss
             sl_multiplier = 1 - sl if sl_type == "call" else 1 + sl
             sl_price = spot_price * sl_multiplier
             trend_sl_hit = False
 
             notifier(
                 f"{self.name} strangle {sl_type} trend catcher starting. "
                 + f"Placed {qty_in_lots} lots of {strike} {opt_type} at {trend_option.fetch_ltp()}. "
                 + f"Stoploss price: {sl_price}, Underlying Price: {spot_price}",
-                self.webhook_url,
+                notification_url,
             )
 
             last_print_time = currenttime()
             print_interval = timedelta(seconds=10)
             while all(
                 [
                     currenttime().time() < time(*exit_time),
@@ -2866,30 +2869,30 @@
                         + f"Stoploss price: {sl_price}, Underlying price: {spot_price}\n"
                         + f"Underlying price avg: {spot_price_avg}, Stoploss hit: {trend_sl_hit}\n"
                     )
 
             if trend_sl_hit:
                 notifier(
                     f"{self.name} strangle {sl_type} trend catcher stoploss hit.",
-                    self.webhook_url,
+                    notification_url,
                 )
             else:
                 notifier(
                     f"{self.name} strangle {sl_type} trend catcher exiting.",
-                    self.webhook_url,
+                    notification_url,
                 )
 
             # Buying the trend option back
             place_option_order_and_notify(
                 trend_option,
                 "BUY",
                 qty_in_lots,
                 "LIMIT",
                 "Intraday Strangle Trend Catcher",
-                self.webhook_url,
+                notification_url,
             )
 
         def justify_stop_loss(info_dict, side):
             entry_spot = info_dict.get("spot_at_entry")
             current_spot = info_dict.get("underlying_ltp")
 
             # If the spot has moved in the direction of stop loss
@@ -2912,37 +2915,41 @@
             except OptionModelInputError:
                 estimated_movement = (
                     0.0015 if side == "call" else -0.0015
                 )  # Remove hard coded number
                 input_error_message = (
                     f"OptionModelInputError in justify_stop_loss for {self.name} {side} strangle. "
                     f"Setting estimated_movement to {estimated_movement}"
+                    f"Input flag: {side}, "
+                    f"Input stop loss price: {info_dict.get(f'{side}_stop_loss_price')}, "
+                    f"Input avg price: {info_dict.get(f'{side}_avg_price')}, "
+                    f"Input entry spot: {entry_spot}"
                 )
                 logger.error(input_error_message)
-                notifier(input_error_message, self.webhook_url)
+                notifier(input_error_message, notification_url)
 
             actual_movement = (current_spot - entry_spot) / entry_spot
             difference_in_sign = np.sign(estimated_movement) != np.sign(actual_movement)
             lack_of_movement = abs(actual_movement) < 0.8 * abs(estimated_movement)
             # Remove hard coded number.
             if difference_in_sign or lack_of_movement:
                 if not info_dict.get(f"{side}_sl_check_notification_sent"):
                     message = (
                         f"{self.name} strangle {side} stop loss appears to be unjustified. "
                         f"Estimated movement: {estimated_movement}, Actual movement: {actual_movement}"
                     )
-                    notifier(message, self.webhook_url)
+                    notifier(message, notification_url)
                     info_dict[f"{side}_sl_check_notification_sent"] = True
                 return False
             else:
                 message = (
                     f"{self.name} strangle {side} stop loss triggered. "
                     f"Estimated movement: {estimated_movement}, Actual movement: {actual_movement}"
                 )
-                notifier(message, self.webhook_url)
+                notifier(message, notification_url)
                 return True
 
         def check_for_stop_loss(info_dict, side, refresh_orderbook=False):
             """Check for stop loss."""
 
             stop_loss_order_ids = info_dict.get(f"{side}_stop_loss_order_ids")
 
@@ -2961,15 +2968,15 @@
                 )
                 if shared_data is None:
                     sleep(3)
                 orders_triggered, orders_complete = process_stop_loss_order_statuses(
                     orderbook,
                     stop_loss_order_ids,
                     context=side,
-                    notify_url=self.webhook_url,
+                    notify_url=notification_url,
                 )
                 if orders_triggered:
                     justify_stop_loss(info_dict, side)
                     info_dict[f"{side}_sl"] = True
                     if not orders_complete:
                         info_dict[f"{side}_stop_loss_order_ids"] = None
 
@@ -2991,15 +2998,15 @@
                 )
                 exit_price = place_option_order_and_notify(
                     option_to_buy,
                     "BUY",
                     quantity_in_lots,
                     "LIMIT",
                     order_tag,
-                    self.webhook_url,
+                    notification_url,
                 )
             else:
                 orderbook = fetch_book("orderbook")
                 exit_price = (
                     lookup_and_return(
                         orderbook,
                         "orderid",
@@ -3028,15 +3035,15 @@
                         f"{other_side}_stop_loss_order_ids"
                     ] = place_option_order_and_notify(
                         instrument=option_to_repair,
                         action="BUY",
                         qty_in_lots=quantity_in_lots,
                         prices=info_dict[f"{other_side}_stop_loss_price"],
                         order_tag=f"{other_side} SL Strangle",
-                        webhook_url=self.webhook_url,
+                        webhook_url=notification_url,
                         stop_loss_order=True,
                         target_status="trigger pending",
                         return_avg_price=False,
                     )
 
             # Starting the trend catcher
             if catch_trend:
@@ -3063,23 +3070,23 @@
                         other_sl_option = (
                             traded_strangle.call_option
                             if other_side == "call"
                             else traded_strangle.put_option
                         )
                         notifier(
                             f"{self.name} strangle {other_side} stop loss hit.",
-                            self.webhook_url,
+                            notification_url,
                         )
                         other_exit_price = place_option_order_and_notify(
                             other_sl_option,
                             "BUY",
                             quantity_in_lots,
                             "LIMIT",
                             order_tag,
-                            self.webhook_url,
+                            notification_url,
                         )
                     else:
                         orderbook = fetch_book("orderbook")
                         other_exit_price = (
                             lookup_and_return(
                                 orderbook,
                                 "orderid",
@@ -3118,29 +3125,35 @@
                 datetime.combine(datetime.now().date(), time(*exit_time))
                 - timedelta(minutes=5)
             ).time(),
         )
         if strangle is None:
             notifier(
                 f"{self.name} no strangle found within disparity threshold {disparity_threshold}",
-                self.webhook_url,
+                notification_url,
             )
             return
         call_ltp, put_ltp = strangle.fetch_ltp()
         call_avg_price, put_avg_price = place_option_order_and_notify(
             strangle,
             "SELL",
             quantity_in_lots,
             "LIMIT",
             order_tag,
-            self.webhook_url,
+            notification_url,
             return_avg_price=True,
         )
-        call_avg_price = call_ltp if np.isnan(call_avg_price) else call_avg_price
-        put_avg_price = put_ltp if np.isnan(put_avg_price) else put_avg_price
+        call_avg_price = (
+            call_ltp
+            if np.isnan(call_avg_price) or call_avg_price == 0
+            else call_avg_price
+        )
+        put_avg_price = (
+            put_ltp if np.isnan(put_avg_price) or put_avg_price == 0 else put_avg_price
+        )
         total_avg_price = call_avg_price + put_avg_price
 
         # Setting stop loss
         stop_loss_dict = {
             "fixed": {"BANKNIFTY": 1.7, "NIFTY": 1.5},
             "dynamic": {"BANKNIFTY": 1.7, "NIFTY": 1.5},
         }
@@ -3192,35 +3205,35 @@
         time_left_at_trade = timetoexpiry(expiry)
         summary_message += (
             f"\nTraded IVs: {traded_call_iv}, {traded_put_iv}, {traded_avg_iv}"
         )
         summary_message += (
             f"\nCall SL: {call_stop_loss_price}, Put SL: {put_stop_loss_price}"
         )
-        notifier(summary_message, self.webhook_url)
+        notifier(summary_message, notification_url)
 
         if place_sl_orders:
             call_stop_loss_order_ids = place_option_order_and_notify(
                 instrument=strangle.call_option,
                 action="BUY",
                 qty_in_lots=quantity_in_lots,
                 prices=call_stop_loss_price,
                 order_tag="Call SL Strangle",
-                webhook_url=self.webhook_url,
+                webhook_url=notification_url,
                 stop_loss_order=True,
                 target_status="trigger pending",
                 return_avg_price=False,
             )
             put_stop_loss_order_ids = place_option_order_and_notify(
                 instrument=strangle.put_option,
                 action="BUY",
                 qty_in_lots=quantity_in_lots,
                 prices=put_stop_loss_price,
                 order_tag="Put SL Strangle",
-                webhook_url=self.webhook_url,
+                webhook_url=notification_url,
                 stop_loss_order=True,
                 target_status="trigger pending",
                 return_avg_price=False,
             )
         else:
             call_stop_loss_order_ids = None
             put_stop_loss_order_ids = None
@@ -3285,23 +3298,23 @@
             hedge_strangle = shared_info_dict["ctb_hedge"]
             place_option_order_and_notify(
                 hedge_strangle,
                 "BUY",
                 quantity_in_lots,
                 "LIMIT",
                 order_tag,
-                self.webhook_url,
+                notification_url,
                 return_avg_price=False,
             )
             if place_sl_orders:
                 cancel_pending_orders(
                     shared_info_dict["call_stop_loss_order_ids"]
                     + shared_info_dict["put_stop_loss_order_ids"]
                 )
-            notifier(f"{self.name}: Converted to butterfly", self.webhook_url)
+            notifier(f"{self.name}: Converted to butterfly", notification_url)
             while currenttime().time() < time(*exit_time):
                 sleep(3)
 
         call_sl = shared_info_dict["call_sl"]
         put_sl = shared_info_dict["put_sl"]
 
         if not call_sl and not put_sl:  # Both stop losses not hit
@@ -3313,15 +3326,15 @@
             else:
                 call_exit_avg_price, put_exit_avg_price = place_option_order_and_notify(
                     strangle,
                     "BUY",
                     quantity_in_lots,
                     "LIMIT",
                     order_tag,
-                    self.webhook_url,
+                    notification_url,
                     return_avg_price=True,
                 )
             # noinspection PyTypeChecker
             if (
                 place_sl_orders
                 and not shared_info_dict["exit_triggers"]["convert_to_butterfly"]
             ):
@@ -3340,15 +3353,15 @@
                 exit_option = strangle.put_option if call_sl else strangle.call_option
                 non_sl_exit_price = place_option_order_and_notify(
                     exit_option,
                     "BUY",
                     quantity_in_lots,
                     "LIMIT",
                     order_tag,
-                    self.webhook_url,
+                    notification_url,
                 )
             if place_sl_orders:
                 cancel_pending_orders(
                     shared_info_dict[f"{exit_option_type}_stop_loss_order_ids"]
                 )
             shared_info_dict[f"{exit_option_type}_exit_price"] = non_sl_exit_price
 
@@ -3378,15 +3391,15 @@
             "Put exit price": shared_info_dict["put_exit_price"],
             "Total exit price": total_exit_price,
             "Points captured": total_avg_price - total_exit_price,
             "Call stop loss": shared_info_dict["call_sl"],
             "Put stop loss": shared_info_dict["put_sl"],
         }
 
-        notifier(exit_message, self.webhook_url)
+        notifier(exit_message, notification_url)
         shared_info_dict["trade_complete"] = True
         position_monitor_thread.join()
 
         trade_log.update(exit_dict)
         self.strategy_log[order_tag].append(trade_log)
 
         return shared_info_dict
@@ -3398,14 +3411,15 @@
         start_time=(9, 15, 58),
         exit_time=(15, 27),
         sleep_time=5,
         threshold_movement=None,
         seconds_to_avg=45,
         beta=0.8,
         max_entries=3,
+        notification_url=None,
     ):
         strategy_tag = "Intraday trend"
 
         while currenttime().time() < time(*start_time):
             sleep(1)
 
         open_price = self.fetch_ltp()
@@ -3425,26 +3439,26 @@
         n_prices = max(int(seconds_to_avg / sleep_time), 1)
         price_deque = deque(maxlen=n_prices)
 
         notifier(
             f"{self.name} trender starting with {threshold_movement:0.2f} threshold movement\n"
             f"Current Price: {open_price}\nUpper limit: {price_boundaries[0]:0.2f}\n"
             f"Lower limit: {price_boundaries[1]:0.2f}.",
-            self.webhook_url,
+            notification_url,
         )
 
         entries = 0
         last_print_time = currenttime()
         movement = 0
         entries_log = []
         while entries < max_entries and currenttime().time() < exit_time:
             # Scan for entry condition
             notifier(
                 f"{self.name} trender {entries+1} scanning for entry condition.",
-                self.webhook_url,
+                notification_url,
             )
             while (abs(movement) < threshold_movement) and (
                 currenttime().time() < scan_end_time
             ):
                 ltp = self.fetch_ltp()
                 price_deque.append(ltp)
                 avg_price = (
@@ -3456,15 +3470,15 @@
                     print(f"{self.name} trender: {movement:0.2f} movement.")
                     last_print_time = currenttime()
                 sleep(sleep_time)
 
             if currenttime().time() > scan_end_time:
                 notifier(
                     f"{self.name} trender {entries+1} exiting due to time.",
-                    self.webhook_url,
+                    notification_url,
                 )
                 return
 
             # Entry condition met taking position
             price = self.fetch_ltp()
             atm_strike = findstrike(price, self.base)
             position = "BUY" if movement > 0 else "SELL"
@@ -3472,36 +3486,36 @@
                 atm_strike, self.name, self.current_expiry
             )
             stop_loss_price = price * (0.997 if position == "BUY" else 1.003)
             stop_loss_hit = False
             notifier(
                 f"{self.name} {position} trender triggered with {movement:0.2f} movement. {self.name} at {price}. "
                 f"Stop loss at {stop_loss_price}.",
-                self.webhook_url,
+                notification_url,
             )
             call_entry_price, put_entry_price = place_option_order_and_notify(
                 atm_synthetic_fut,
                 position,
                 quantity_in_lots,
                 "LIMIT",
                 strategy_tag,
-                self.webhook_url,
+                notification_url,
                 return_avg_price=True,
             )
 
             if call_entry_price == 0 or put_entry_price == 0:
                 call_entry_price, put_entry_price = atm_synthetic_fut.fetch_ltp()
 
             entry_price = atm_strike + call_entry_price - put_entry_price
             spot_future_basis = entry_price - price
 
             notifier(
                 f"{self.name} trender {entries+1} entry price: {entry_price}, "
                 f"spot-future basis: {spot_future_basis}",
-                self.webhook_url,
+                notification_url,
             )
 
             trade_info = {
                 "Entry time": currenttime().strftime("%d-%m-%Y %H:%M:%S"),
                 "Position": position,
                 "Spot price": price,
                 "Entry price": entry_price,
@@ -3526,23 +3540,23 @@
                 sleep(sleep_time)
 
             # Exit condition met exiting position (stop loss or time)
             price = self.fetch_ltp()
             stop_loss_message = f"Trender stop loss hit. " if stop_loss_hit else ""
             notifier(
                 f"{stop_loss_message}{self.name} trender {entries+1} exiting. {self.name} at {price}.",
-                self.webhook_url,
+                notification_url,
             )
             call_exit_price, put_exit_price = place_option_order_and_notify(
                 atm_synthetic_fut,
                 "BUY" if position == "SELL" else "SELL",
                 quantity_in_lots,
                 "LIMIT",
                 strategy_tag,
-                self.webhook_url,
+                notification_url,
             )
 
             if call_exit_price == 0 or put_exit_price == 0:
                 call_exit_price, put_exit_price = atm_synthetic_fut.fetch_ltp()
 
             exit_price = atm_strike + call_exit_price - put_exit_price
             pnl = (
@@ -3551,15 +3565,15 @@
                 else (entry_price - exit_price)
             )
             spot_future_basis = exit_price - price
 
             notifier(
                 f"{self.name} trender {entries+1} exit price: {exit_price}, "
                 f"spot-future basis: {spot_future_basis}, pnl: {pnl}",
-                self.webhook_url,
+                notification_url,
             )
 
             trade_info.update(
                 {
                     "Exit time": currenttime().strftime("%d-%m-%Y %H:%M:%S"),
                     "Stop loss hit": stop_loss_hit,
                     "Spot exit price": price,
@@ -3576,43 +3590,51 @@
     def intraday_straddle_delta_hedged(
         self,
         quantity_in_lots,
         exit_time=(15, 30),
         websocket=None,
         wait_for_equality=False,
         delta_threshold=1,
+        notification_url=None,
         **kwargs,
     ):
         # Finding equal strike
         (
             equal_strike,
             call_symbol,
             put_symbol,
             call_token,
             put_token,
             call_price,
             put_price,
-        ) = self.find_equal_strike(exit_time, websocket, wait_for_equality, **kwargs)
+        ) = self.find_equal_strike(
+            exit_time,
+            websocket,
+            wait_for_equality,
+            notification_url=notification_url,
+            **kwargs,
+        )
         expiry = self.current_expiry
         print(
             f"Index: {self.name}, Strike: {equal_strike}, Call: {call_price}, Put: {put_price}"
         )
         notifier(
             f"{self.name}: Initiating intraday trade on {equal_strike} strike.",
-            self.webhook_url,
+            notification_url,
         )
 
         # Placing orders
         self.place_combined_order(
             expiry,
             "SELL",
             quantity_in_lots,
             strike=equal_strike,
             return_avg_price=True,
             order_tag="Intraday straddle with delta",
+            notification_url=notification_url,
         )
 
         positions = {
             f"{self.name} {equal_strike} {expiry} CE": {
                 "token": call_token,
                 "quantity": -1 * quantity_in_lots * self.lot_size,
                 "delta_quantity": 0,
@@ -3663,15 +3685,15 @@
 
             if abs(current_delta) > delta_threshold:
                 if current_delta > 0:  # We are long
                     lots_to_sell = round(abs(current_delta) / self.lot_size, 0)
                     notifier(
                         f"Delta greater than {delta_threshold}. Selling {lots_to_sell} "
                         + f"synthetic futures to reduce delta.\n",
-                        self.webhook_url,
+                        notification_url,
                     )
                     place_synthetic_fut_order(
                         self.name,
                         equal_strike,
                         expiry,
                         "SELL",
                         lots_to_sell,
@@ -3684,15 +3706,15 @@
                     )
 
                 else:  # We are short
                     lots_to_buy = round(abs(current_delta) / self.lot_size, 0)
                     notifier(
                         f"Delta less than -{delta_threshold}. Buying {lots_to_buy} "
                         + f"synthetic futures to reduce delta.\n",
-                        self.webhook_url,
+                        notification_url,
                     )
                     place_synthetic_fut_order(
                         self.name,
                         equal_strike,
                         expiry,
                         "BUY",
                         lots_to_buy,
@@ -3703,21 +3725,22 @@
                     positions[synthetic_fut_put]["delta_quantity"] -= (
                         lots_to_buy * self.lot_size
                     )
 
             sleep(2)
 
         # Closing the main positions along with the delta positions if any are open
-        notifier(f"Intraday straddle with delta: Closing positions.", self.webhook_url)
+        notifier(f"Intraday straddle with delta: Closing positions.", notification_url)
         self.place_combined_order(
             expiry,
             "BUY",
             quantity_in_lots,
             strike=equal_strike,
             order_tag="Intraday straddle with delta",
+            notification_url=notification_url,
         )
 
         # Squaring off the delta positions
         call_delta_quantity = positions[synthetic_fut_call]["delta_quantity"]
         put_delta_quantity = positions[synthetic_fut_put]["delta_quantity"]
 
         if call_delta_quantity != 0 and put_delta_quantity != 0:
@@ -3732,27 +3755,25 @@
 
             self.place_synthetic_fut(
                 equal_strike, expiry, action, quantity_to_square_up_in_lots
             )
             notifier(
                 f"Intraday Straddle with delta: Squared off delta positions. "
                 + f"{action} {quantity_to_square_up} synthetic futures.",
-                self.webhook_url,
+                notification_url,
             )
         elif call_delta_quantity == 0 and put_delta_quantity == 0:
-            notifier("No delta positions to square off.", self.webhook_url)
+            notifier("No delta positions to square off.", notification_url)
         else:
             raise AssertionError("Delta positions are not balanced.")
 
 
 class Stock(Index):
-    def __init__(
-        self, name, webhook_url=None, websocket=None, spot_future_difference=0.06
-    ):
-        super().__init__(name, webhook_url, websocket, spot_future_difference)
+    def __init__(self, name, spot_future_difference=0.06):
+        super().__init__(name, spot_future_difference)
 
 
 def convert_to_serializable(data):
     if isinstance(data, dict):
         return {k: convert_to_serializable(v) for k, v in data.items()}
     elif isinstance(data, list):
         return [convert_to_serializable(item) for item in data]
@@ -3761,14 +3782,17 @@
     elif hasattr(data, "item"):  # Check for numpy scalar types, e.g., numpy.int32
         return data.item()
     else:
         return data
 
 
 def append_data_to_json(new_data: defaultdict | dict | list, file_name: str) -> None:
+    if new_data is None:
+        return
+
     # Attempt to read the existing data from the JSON file
     try:
         with open(file_name, "r") as file:
             existing_data = json.load(file)
     except (FileNotFoundError, json.JSONDecodeError):
         # If the file doesn't exist or has invalid JSON content, create an empty list and write it to the file
         existing_data = []
@@ -4426,19 +4450,30 @@
     if expiry is None and strike is None and option_type is None:  # Cash segment
         if name in ["NIFTY", "BANKNIFTY"]:  # Index scrips
             filtered_scrips = scrips.loc[
                 (scrips.name == name)
                 & (scrips.exch_seg == "NSE")
                 & (scrips.instrumenttype != "AMXIDX")
             ]  # Temp fix for AMXIDX
-            # print(f'Length of filtered scrips: {len(filtered_scrips)}')
-            assert (
-                len(filtered_scrips) == 1
-            ), "More than one index scrip found for name."
-            symbol, token = filtered_scrips[["symbol", "token"]].values[0]
+
+            if len(filtered_scrips) != 1:
+                logger.error(
+                    f"Could not find symbol, token for {name} from scrips file."
+                )
+                if len(filtered_scrips) == 0:
+                    logger.error(f"No scrips found: {filtered_scrips}")
+                else:
+                    logger.error(f"Multiple scrips found: {filtered_scrips}")
+
+                symbol, token = (
+                    ("NIFTY", "26000") if name == "NIFTY" else ("BANKNIFTY", "26009")
+                )  # Temp fix for NIFTY & BANKNIFTY. To be removed later.
+
+            else:
+                symbol, token = filtered_scrips[["symbol", "token"]].values[0]
 
         elif name in ["FINNIFTY", "MIDCPNIFTY"]:  # Finnifty & Midcpnifty temp fix
             futures = scrips.loc[
                 (scrips.name == name) & (scrips.instrumenttype == "FUTIDX"),
                 ["expiry", "symbol", "token"],
             ]
             futures["expiry"] = pd.to_datetime(futures["expiry"], format="%d%b%Y")
```

### Comparing `volstreet-1.1.0/volstreet/discord_bot.py` & `volstreet-1.2.0/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.1.0/volstreet/exceptions.py` & `volstreet-1.2.0/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.1.0/volstreet/nsefunctions.py` & `volstreet-1.2.0/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.1.0/volstreet/strategies.py` & `volstreet-1.2.0/volstreet/strategies.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,24 +75,25 @@
     vs.login(
         user=user,
         pin=pin,
         apikey=apikey,
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
-    nifty = vs.Index("NIFTY", webhook_url=discord_webhook_url)
-    bnf = vs.Index("BANKNIFTY", webhook_url=discord_webhook_url)
-    fin = vs.Index("FINNIFTY", webhook_url=discord_webhook_url)
-    midcap = vs.Index("MIDCPNIFTY", webhook_url=discord_webhook_url)
+    nifty = vs.Index("NIFTY")
+    bnf = vs.Index("BANKNIFTY")
+    fin = vs.Index("FINNIFTY")
+    midcap = vs.Index("MIDCPNIFTY")
 
     indices = vs.get_strangle_indices_to_trade(
         nifty, bnf, fin, midcap, safe_indices=safe_indices
     )
 
     parameters["quantity_in_lots"] = parameters["quantity_in_lots"] // len(indices)
+    parameters["notification_url"] = discord_webhook_url
 
     # Setting the shared data
     if shared_data:
         shared_data = vs.SharedData()
         update_data_thread = threading.Thread(target=shared_data.update_data)
         parameters["shared_data"] = shared_data
     else:
@@ -164,29 +165,42 @@
     vs.login(
         user=user,
         pin=pin,
         apikey=apikey,
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
-    nifty = vs.Index("NIFTY", webhook_url=discord_webhook_url)
+    nifty = vs.Index("NIFTY")
 
     # Rolling over the short straddle
     nifty.rollover_overnight_short_straddle(
-        quantity_in_lots, strike_offset=1.003, take_avg_price=True
+        quantity_in_lots,
+        strike_offset=1.003,
+        take_avg_price=True,
+        notification_url=discord_webhook_url,
     )
 
     # Buying next week's hedge if it is expiry day
     if vs.timetoexpiry(nifty.current_expiry, in_days=True) < 1:
         nifty.buy_weekly_hedge(
-            quantity_in_lots, "strangle", call_offset=0.997, put_offset=0.98
+            quantity_in_lots,
+            "strangle",
+            call_offset=0.997,
+            put_offset=0.98,
+            notification_url=discord_webhook_url,
         )
 
     try:
-        vs.append_data_to_json(nifty.order_log, f"{user}_NIFTY_ON_straddle_log.json")
+        vs.append_data_to_json(
+            nifty.strategy_log["Overnight short straddle"],
+            f"{user}_NIFTY_overnight_short_straddle.json",
+        )
+        vs.append_data_to_json(
+            nifty.strategy_log["Weekly hedge"], f"{user}_NIFTY_weekly_hedge.json"
+        )
     except Exception as e:
         vs.notifier(f"Appending data failed: {e}", discord_webhook_url)
 
 
 def intraday_trend_on_indices(
     parameters,
     indices,
@@ -236,15 +250,17 @@
         user=user,
         pin=pin,
         apikey=apikey,
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
 
-    indices = [vs.Index(index, webhook_url=discord_webhook_url) for index in indices]
+    indices = [vs.Index(index) for index in indices]
+
+    parameters["notification_url"] = discord_webhook_url
 
     threads = []
     for index in indices:
         index_parameters = parameters.copy()
         index_parameters.update(special_parameters.get(index.name, {}))
         thread = threading.Thread(target=index.intraday_trend, kwargs=index_parameters)
         threads.append(thread)
```

### Comparing `volstreet-1.1.0/volstreet.egg-info/requires.txt` & `volstreet-1.2.0/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

