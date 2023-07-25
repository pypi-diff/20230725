# Comparing `tmp/volstreet-1.0.5.tar.gz` & `tmp/volstreet-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.0.5.tar", last modified: Sun Jul 23 12:50:36 2023, max compression
+gzip compressed data, was "volstreet-1.0.7.tar", last modified: Tue Jul 25 18:05:05 2023, max compression
```

## Comparing `volstreet-1.0.5.tar` & `volstreet-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 12:50:36.402143 volstreet-1.0.5/
--rw-rw-rw-   0        0        0      497 2023-07-23 12:50:36.402143 volstreet-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.5/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-07-23 12:50:36.403140 volstreet-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-23 12:50:36.395166 volstreet-1.0.5/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.5/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.5/volstreet/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.5/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.5/volstreet/constants.py
--rw-rw-rw-   0        0        0    42857 2023-07-23 12:48:19.000000 volstreet-1.0.5/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   192083 2023-07-21 17:03:46.000000 volstreet-1.0.5/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.5/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.5/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.5/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    13257 2023-07-17 06:22:53.000000 volstreet-1.0.5/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:50:36.401147 volstreet-1.0.5/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-23 12:50:36.000000 volstreet-1.0.5/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-23 12:50:36.000000 volstreet-1.0.5/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 12:50:36.000000 volstreet-1.0.5/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-07-23 12:50:36.000000 volstreet-1.0.5/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-23 12:50:36.000000 volstreet-1.0.5/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 18:05:05.320165 volstreet-1.0.7/
+-rw-rw-rw-   0        0        0      497 2023-07-25 18:05:05.320165 volstreet-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.7/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-07-25 18:05:05.321669 volstreet-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 18:05:05.314186 volstreet-1.0.7/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.7/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.7/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.7/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.7/volstreet/constants.py
+-rw-rw-rw-   0        0        0    43796 2023-07-25 18:04:18.000000 volstreet-1.0.7/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   192160 2023-07-25 17:19:23.000000 volstreet-1.0.7/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.7/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.7/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.7/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    13488 2023-07-25 17:19:23.000000 volstreet-1.0.7/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:05:05.319170 volstreet-1.0.7/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.0.5/setup.cfg` & `volstreet-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 350d 0a61  rsion = 1.0.5..a
+00000020: 7273 696f 6e20 3d20 312e 302e 370d 0a61  rsion = 1.0.7..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-1.0.5/volstreet/SmartWebSocketV2.py` & `volstreet-1.0.7/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.5/volstreet/blackscholes.py` & `volstreet-1.0.7/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.5/volstreet/constants.py` & `volstreet-1.0.7/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.5/volstreet/datamodule.py` & `volstreet-1.0.7/volstreet/datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -861,14 +861,15 @@
 
 
 def backtest_intraday_trend(
     one_min_df,
     open_nth=0,
     beta=1,
     trend_threshold=1,
+    stop_loss=0.3,
     max_entries=3,
     eod_client=None,
     rolling_days=60,
 ):
     one_min_df = one_min_df.copy()
     if one_min_df.index.name == "date":
         one_min_df = one_min_df.reset_index()
@@ -910,14 +911,31 @@
     open_data["upper_bound"] = open_data["open"] * (
         1 + open_data["threshold_movement"] / 100
     )
     open_data["lower_bound"] = open_data["open"] * (
         1 - open_data["threshold_movement"] / 100
     )
     open_data["day_close"] = one_min_df.groupby(one_min_df["date"].dt.date).close.last()
+
+    daily_minute_vols = (
+        one_min_df.groupby(one_min_df["date"].dt.date)
+        .apply(lambda x: x["close"].pct_change().abs().mean() * 100)
+    )
+
+    daily_minute_vols_rolling = daily_minute_vols.rolling(rolling_days, min_periods=1).mean()
+
+    daily_open_to_close_trends = (
+        one_min_df.close.groupby(one_min_df["date"].dt.date)
+        .apply(lambda x: (x.iloc[-1] / x.iloc[0] - 1) * 100)
+    )
+
+    daily_open_to_close_trends_rolling = daily_open_to_close_trends.abs().rolling(rolling_days, min_periods=1).mean()
+
+    rolling_ratio = daily_open_to_close_trends_rolling / daily_minute_vols_rolling
+
     open_data.columns = [
         "day_open",
         "open_vix",
         "threshold_movement",
         "upper_bound",
         "lower_bound",
         "day_close",
@@ -933,14 +951,17 @@
         ]
     ] = open_data.loc[one_min_df["date"].dt.date].values
     one_min_df["change_from_open"] = (
         (one_min_df["close"] / one_min_df["day_open"]) - 1
     ) * 100
 
     def calculate_daily_trade_data(group):
+
+        """ The group is a dataframe """
+
         all_entries_in_a_day = {}
         # Find the first index where the absolute price change crosses the threshold
         entry = 1
         while entry <= max_entries:
             idx = group[
                 abs(group["change_from_open"]) >= group["threshold_movement"]
             ].first_valid_index()
@@ -957,29 +978,42 @@
                 cross_price = group.loc[idx, "close"]
                 cross_time = group.loc[idx, "date"]
 
                 # Determine the direction of the movement
                 direction = np.sign(group.loc[idx, "change_from_open"])
 
                 # Calculate the stoploss price
-                stoploss_price = cross_price * (1 - 0.003 * direction)
+                if stop_loss == 'dynamic':
+                    # Selecting previous days rolling ratio
+                    current_rolling_ratio = rolling_ratio.loc[:cross_time.date()].iloc[-1]
+                    # Calculating the stop_loss pct
+                    if current_rolling_ratio > 30:
+                        stop_loss_pct = 0.3
+                    elif current_rolling_ratio < 10:
+                        stop_loss_pct = 0.5
+                    else:
+                        stop_loss_pct = ((30 - current_rolling_ratio) / 100) + 0.3
+                else:
+                    stop_loss_pct = stop_loss
+
+                stoploss_price = cross_price * (1 - (stop_loss_pct / 100) * direction)
                 result_dict.update(
                     {
                         "trigger_time": cross_time,
                         "trigger_price": cross_price,
                         "trend_direction": direction,
                         "stop_loss_price": stoploss_price,
                     }
                 )
                 future_prices = group.loc[idx:, "close"]
 
                 if (direction == 1 and future_prices.min() <= stoploss_price) or (
                     direction == -1 and future_prices.max() >= stoploss_price
                 ):  # Stop loss was breached
-                    result_dict["returns"] = -0.30
+                    result_dict["returns"] = -stop_loss_pct
                     stoploss_time_idx = (
                         future_prices[
                             future_prices <= stoploss_price
                         ].first_valid_index()
                         if direction == 1
                         else future_prices[
                             future_prices >= stoploss_price
@@ -1021,40 +1055,26 @@
     merged = returns.merge(open_data, left_index=True, right_index=True)
     merged["total_returns"] = merged["trade_data"].apply(lambda x: x["total_returns"])
     merged = nav_drawdown_analyser(
         merged, column_to_convert="total_returns", profit_in_pct=True
     )
 
     # calculating the minute vol
-    merged["minute_vol"] = (
-        one_min_df.groupby(one_min_df["date"].dt.date)
-        .apply(lambda x: x["close"].pct_change().abs().mean() * 100)
-        .to_frame()
-    )
+    merged["minute_vol"] = daily_minute_vols
 
     # calculating the open to close trend
-    merged["open_to_close_trend"] = (
-        one_min_df.close.groupby(one_min_df["date"].dt.date)
-        .apply(lambda x: (x.iloc[-1] / x.iloc[0] - 1) * 100)
-        .abs()
-        .to_frame()
-    )
+    merged["open_to_close_trend"] = daily_open_to_close_trends
+
+    merged["open_to_close_trend_abs"] = merged["open_to_close_trend"].abs()
 
     # calculating the ratio and rolling mean
-    rolling_days = rolling_days
-    merged["minute_vol_rolling"] = (
-        merged["minute_vol"].rolling(rolling_days, min_periods=1).mean()
-    )
-    merged["open_to_close_trend_rolling"] = (
-        merged["open_to_close_trend"].rolling(rolling_days, min_periods=1).mean()
-    )
-    merged["ratio"] = merged["open_to_close_trend"] / merged["minute_vol"]
-    merged["rolling_ratio"] = (
-        merged["open_to_close_trend_rolling"] / merged["minute_vol_rolling"]
-    )
+    merged["minute_vol_rolling"] = daily_minute_vols_rolling
+    merged["open_to_close_trend_rolling"] = daily_open_to_close_trends_rolling
+    merged["ratio"] = merged["open_to_close_trend_abs"] / merged["minute_vol"]
+    merged["rolling_ratio"] = rolling_ratio
 
     return merged
 
 
 def calculate_intraday_return_drivers(
     symbol_one_min_df, day_wise_summary_df, rolling_days=60
 ):
```

### Comparing `volstreet-1.0.5/volstreet/dealingroom.py` & `volstreet-1.0.7/volstreet/dealingroom.py`

 * *Files 0% similar despite different names*

```diff
@@ -2938,14 +2938,16 @@
                     if stop_loss_justified:
                         info_dict[f"{side}_sl"] = True
 
             else:  # If stop loss order ids are provided
                 orderbook = fetch_orderbook_if_needed(
                     shared_data, refresh_needed=refresh_orderbook
                 )
+                if shared_data is None:
+                    sleep(3)
                 orders_triggered, orders_complete = process_stop_loss_order_statuses(
                     orderbook,
                     stop_loss_order_ids,
                     context=side,
                     notify_url=self.webhook_url,
                 )
                 if orders_triggered:
@@ -4227,15 +4229,15 @@
 
     filtered_df = scrips.loc[
         (scrips.name == name) & (scrips.exch_seg == "NFO") & expiry_mask
     ]
     lot_sizes = filtered_df.lotsize.values
 
     if len(set(lot_sizes)) > 1:
-        print(
+        logger.info(
             f"Multiple lot sizes found for {name}. Using the closest expiry lot size."
         )
         filtered_df = filtered_df.sort_values("expiry_dt")
         return filtered_df.lotsize.iloc[0]
 
     else:
         return lot_sizes[0]
```

### Comparing `volstreet-1.0.5/volstreet/discord_bot.py` & `volstreet-1.0.7/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.5/volstreet/nsefunctions.py` & `volstreet-1.0.7/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.5/volstreet/strategies.py` & `volstreet-1.0.7/volstreet/strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,34 +188,36 @@
     indices,
     client=None,
     user=None,
     pin=None,
     apikey=None,
     authkey=None,
     webhook_url=None,
+    special_parameters=None,
 ):
     """
 
     :param parameters: parameters for the strategy (refer to the strategy's docstring)
                        summary of parameters:
                        quantity_in_lots,
                        start_time=(9, 15, 58),
                        exit_time=(15, 27),
                        sleep_time=5,
                        threshold_movement=None,
-                       minutes_to_avg=45,
+                       seconds_to_avg=45,
                        beta=0.8,
                        max_entries=3
     :param indices: list of indices to trade
     :param client: client's name
     :param user: username
     :param pin: user's pin
     :param apikey: user apikey
     :param authkey: user authkey
     :param webhook_url: discord webhook url
+    :param special_parameters: special parameters for a particular index
 
     """
 
     user, pin, apikey, authkey, discord_webhook_url = get_user_data(
         client, user, pin, apikey, authkey, webhook_url
     )
 
@@ -229,16 +231,18 @@
         apikey=apikey,
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
 
     threads = []
     for index_symbol in indices:
+        index_parameters = parameters.copy()
+        index_parameters.update(special_parameters.get(index_symbol, {}))
         index = vs.Index(index_symbol, webhook_url=discord_webhook_url)
-        thread = threading.Thread(target=index.intraday_trend, kwargs=parameters)
+        thread = threading.Thread(target=index.intraday_trend, kwargs=index_parameters)
         threads.append(thread)
 
     for thread in threads:
         thread.start()
 
     for thread in threads:
         thread.join()
```

### Comparing `volstreet-1.0.5/volstreet.egg-info/requires.txt` & `volstreet-1.0.7/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

