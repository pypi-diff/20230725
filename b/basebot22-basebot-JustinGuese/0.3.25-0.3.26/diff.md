# Comparing `tmp/basebot22-basebot_JustinGuese-0.3.25.tar.gz` & `tmp/basebot22-basebot_JustinGuese-0.3.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.25.tar", last modified: Thu Jul 20 08:21:47 2023, max compression
+gzip compressed data, was "basebot22-basebot_JustinGuese-0.3.26.tar", last modified: Tue Jul 25 14:48:18 2023, max compression
```

## Comparing `basebot22-basebot_JustinGuese-0.3.25.tar` & `basebot22-basebot_JustinGuese-0.3.26.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-20 08:21:36.000000 basebot22-basebot_JustinGuese-0.3.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/basebot22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:36.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:36.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-07-20 08:21:36.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22/basebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 08:21:47.000000 basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-20 08:21:39.000000 basebot22-basebot_JustinGuese-0.3.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:21:47.412006 basebot22-basebot_JustinGuese-0.3.25/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:48:18.903762 basebot22-basebot_JustinGuese-0.3.26/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-25 14:48:18.903762 basebot22-basebot_JustinGuese-0.3.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-25 14:48:04.000000 basebot22-basebot_JustinGuese-0.3.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:48:18.899762 basebot22-basebot_JustinGuese-0.3.26/basebot22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:48:04.000000 basebot22-basebot_JustinGuese-0.3.26/basebot22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:48:04.000000 basebot22-basebot_JustinGuese-0.3.26/basebot22/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-07-25 14:48:04.000000 basebot22-basebot_JustinGuese-0.3.26/basebot22/basebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:48:18.899762 basebot22-basebot_JustinGuese-0.3.26/basebot22_basebot_JustinGuese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-25 14:48:18.000000 basebot22-basebot_JustinGuese-0.3.26/basebot22_basebot_JustinGuese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 14:48:18.000000 basebot22-basebot_JustinGuese-0.3.26/basebot22_basebot_JustinGuese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:48:18.000000 basebot22-basebot_JustinGuese-0.3.26/basebot22_basebot_JustinGuese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 14:48:18.000000 basebot22-basebot_JustinGuese-0.3.26/basebot22_basebot_JustinGuese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 14:48:18.000000 basebot22-basebot_JustinGuese-0.3.26/basebot22_basebot_JustinGuese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-25 14:48:09.000000 basebot22-basebot_JustinGuese-0.3.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:48:18.903762 basebot22-basebot_JustinGuese-0.3.26/setup.cfg
```

### Comparing `basebot22-basebot_JustinGuese-0.3.25/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.26/basebot22_basebot_JustinGuese.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: basebot22-basebot_JustinGuese
-Version: 0.3.25
+Name: basebot22-basebot-JustinGuese
+Version: 0.3.26
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.25/README.md` & `basebot22-basebot_JustinGuese-0.3.26/README.md`

 * *Files identical despite different names*

### Comparing `basebot22-basebot_JustinGuese-0.3.25/basebot22/basebot.py` & `basebot22-basebot_JustinGuese-0.3.26/basebot22/basebot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,61 +2,69 @@
 from math import sqrt
 from random import randint
 from typing import List
 from urllib.parse import quote_plus
 
 import numpy as np
 import pandas as pd
-from requests import get, post, put
+from requests import Session
 from scipy.signal import argrelextrema, savgol_filter
 
 
 class BaseBot:
 
     def __init__(self, name: str, backendurl: str = "http://127.0.0.1:8000", live: bool = False):
+        user, password = None, None
+        if "@" in backendurl:
+            user, password = backendurl.split("@")[0].split("//")[1].split(":")
+            backendurl = "https://" + backendurl.split("@")[1]
         self.backendurl: str = backendurl
+        self.session = Session()
+        if user is not None and password is not None:
+            self.session.auth = (user, password)
+
         self.headers: dict = { 'accept': 'application/json', 'Content-Type': 'application/json'}
         self.live: bool = live
         self.name: str = self.checkOrCreate(name, live)
     
     def checkOrCreate(self, name: str, live: bool = False) -> str:
         response = get(self.backendurl + '/bot/' + quote_plus(name), headers=self.headers)
         if response.status_code != 200:
             # create
             json_data = {
                 'name': name,
                 'description': 'created in basebot',
                 'live': live,
             }
-            response = put(self.backendurl + "/bot", json=json_data, headers=self.headers)
+            response = self.session.put(self.backendurl + "/bot", json=json_data, headers=self.headers)
         return name
 
     def getPortfolio(self) -> dict:
-        response = get(self.backendurl + '/bot/' + quote_plus(self.name), headers=self.headers)
+        response = self.session.get(self.backendurl + '/bot/' + quote_plus(self.name), headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting portfolio: ", response.text)
         return response.json()["portfolio"]
 
     def getPortfolioWorth(self) -> float:
-        response = get(self.backendurl + '/bot/%s/portfolioworth' % quote_plus(self.name), headers=self.headers)
+        response = self.session.get(self.backendurl + '/bot/%s/portfolioworth' % quote_plus(self.name), headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting portfolio worth: ", response.text)
         return float(response.text)
     
     def buy(self, ticker: str, amount: float = -1, amountInUSD: bool = False, short: bool = False, close_if_below: float = -1, close_if_above: float = -1, close_if_below_hardlimit: float = None, maximum_date: date = None):
         if close_if_above == -1 and close_if_below == -1 and maximum_date is None:
             # normal trade
             params = {
                 "botname": self.name,
                 'ticker': ticker,
                 'amount': amount,
                 "amountInUSD": amountInUSD,
                 "short": short,
             }
-            response = put(self.backendurl + '/buy/', params=params, headers=self.headers)
+            response = self.session.put(self.backendurl + '/buy/', params=params, headers=self.headers)
             if response.status_code != 200:
                 raise Exception("Error buying: ", response.text)
         elif close_if_above != -1 and close_if_below != -1:
             if maximum_date is None:
                 maximum_date = datetime.utcnow().date() + timedelta(365)
             # stoploss trade
             params = {
@@ -67,53 +75,53 @@
                 "short": short,
                 # stop loss specific stuff
                 "close_if_above": close_if_above,
                 "close_if_below": close_if_below,
                 "close_if_below_hardlimit" : close_if_below_hardlimit,
                 "maximum_date": datetime.combine(maximum_date, time.min), # man...
             }
-            response = put(self.backendurl + '/buy/stoploss/', params=params, headers=self.headers)
+            response = self.session.put(self.backendurl + '/buy/stoploss/', params=params, headers=self.headers)
             if response.status_code != 200:
                 raise Exception("Error stoploss buying: ", response.text)
         else:
             raise ValueError("close_if_above, close_if_below and maximum_date must be all set or both not set. if they are both set a stop loss / take profit trade is created")
 
     def sell(self, ticker: str, amount: float = -1, amountInUSD: bool = False, short: bool = False):
         params = {
             "botname": self.name,
             'ticker': ticker,
             'amount': amount,
             "amountInUSD": amountInUSD,
             "short": short,
         }
-        response = put(self.backendurl + '/sell/', params=params, headers=self.headers)
+        response = self.session.put(self.backendurl + '/sell/', params=params, headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error selling: ", ticker, response.text)
 
     def getData(self, ticker: str, start_date: date = (datetime.utcnow() - timedelta(7)).date(), 
         end_date: date = datetime.utcnow().date(), technical_indicators: list = []):
         json_data = {
             'ticker': ticker,
             'start_date': start_date.strftime("%Y-%m-%d"),
             'end_date': end_date.strftime("%Y-%m-%d"),
             'technical_analysis_columns': technical_indicators,
         }
-        response = post(self.backendurl + '/data/', json=json_data, headers=self.headers)
+        response = self.session.post(self.backendurl + '/data/', json=json_data, headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting data: ", response.text)
         df = pd.DataFrame(response.json())
         df.set_index("timestamp", inplace=True)
         df.sort_index(inplace=True)
         # somehow index gets converted to string
         df.index = pd.to_datetime(df.index)
         # df = df[::-1]
         return df
     
     def getCurrentPrice(self, ticker: str):
-        response = get(self.backendurl + '/data/current_price/' + quote_plus(ticker), headers=self.headers)
+        response = self.session.get(self.backendurl + '/data/current_price/' + quote_plus(ticker), headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting current price data for %s: " % ticker, response.text)
         return float(response.text)
     
     def getTrend(self, df: pd.DataFrame) -> pd.DataFrame:
         # see tradingbot22-tradingbots/jupyternotebooks/signalsmoothing.ipynb
         if "adj_close" not in df:
@@ -180,60 +188,60 @@
         
     ## basic backtest functionality
     def getDecision(self, row: pd.Series, ticker: str = "") -> int:
         # raise NotImplementedError("getDecision not implemented")
         return randint(-1, 1)
     
     def getEarningsCalendar(self, only_now: bool = True):
-        response = get(self.backendurl + '/data/earnings/calendar?now=%s' % str(only_now).lower() , headers=self.headers)
+        response = self.session.get(self.backendurl + '/data/earnings/calendar?now=%s' % str(only_now).lower() , headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting current earnings: ", response.text)
         response = response.json()
         return self.__fixTimeStampEarnings(response)
     
     def getEarningsCalendarPrevious(self, custom_date: date = date.today()):
         try:
-            response = get(self.backendurl + '/data/earnings/calendar-previous?custom_date=%s' % (custom_date.strftime("%Y-%m-%d")) , headers=self.headers)
+            response = self.session.get(self.backendurl + '/data/earnings/calendar-previous?custom_date=%s' % (custom_date.strftime("%Y-%m-%d")) , headers=self.headers)
         except TypeError as e:
             # not all fuck formatted during string formatting wtf
             raise TypeError("custom_date must be formattable by strftime(Y-m-d), it is: %s" % str(custom_date)) from e
         if response.status_code != 200:
             raise Exception("Error getting current earnings financials: ", response.text)
         response = response.json()
         return self.__fixTimeStampEarnings(response)
     
     def getEarningsFinancials(self, ticker: str, only_now: bool = True):
-        response = get(self.backendurl + '/data/earnings/financials?ticker=%s&now=%s' % (ticker, str(only_now).lower()) , headers=self.headers)
+        response = self.session.get(self.backendurl + '/data/earnings/financials?ticker=%s&now=%s' % (ticker, str(only_now).lower()) , headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting current earnings financials: ", response.text)
         response = response.json()
         return self.__fixTimeStampEarnings(response)
     
     def __decryptStringArray(self, stringarray: str) -> list:
         return [float(s.strip()) for s in stringarray[1:-1].split(",")]
     
     def getEarningsEffect(self, ticker: str):
-        response = get(self.backendurl + '/data/earnings/effect?ticker=%s' % (ticker) , headers=self.headers)
+        response = self.session.get(self.backendurl + '/data/earnings/effect?ticker=%s' % (ticker) , headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting current earnings effects: ", response.text)
         response = response.json()
         response = self.__fixTimeStampEarnings(response)
         # next fix all_changes_list to str conversion
         response["all_changes_list"] = self.__decryptStringArray(response["all_changes_list"]) # becasue we save it in the db as str
         return response
     
     def updateEarnings(self, ticker: str):
-        response = get(self.backendurl + '/update/earnings/?ticker=%s' % (ticker) , headers=self.headers)
+        response = self.session.get(self.backendurl + '/update/earnings/?ticker=%s' % (ticker) , headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting current earnings effects: ", response.text)
         response = response.json()
         return self.__fixTimeStampEarnings(response)
     
     def getEarningsRatings(self, ticker: str) -> dict:
-        response = get(self.backendurl + '/data/earnings/ratings/?ticker=%s' % (ticker) , headers=self.headers)
+        response = self.session.get(self.backendurl + '/data/earnings/ratings/?ticker=%s' % (ticker) , headers=self.headers)
         if response.status_code != 200:
             raise Exception("Error getting earnings ratings: ", response.text)
         response = response.json()
         response["timestamp"] = pd.to_datetime(response["timestamp"])
         return response
```

### Comparing `basebot22-basebot_JustinGuese-0.3.25/basebot22_basebot_JustinGuese.egg-info/PKG-INFO` & `basebot22-basebot_JustinGuese-0.3.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: basebot22-basebot-JustinGuese
-Version: 0.3.25
+Name: basebot22-basebot_JustinGuese
+Version: 0.3.26
 Summary: A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots
 Author-email: Justin Güse <guese.justin@gmail.com>
 Project-URL: Homepage, https://github.com/JustinGuese/tradingbot22-basebot
 Project-URL: Bug Tracker, https://github.com/JustinGuese/tradingbot22-basebot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basebot22-basebot_JustinGuese-0.3.25/pyproject.toml` & `basebot22-basebot_JustinGuese-0.3.26/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "basebot22-basebot_JustinGuese"
 authors = [
   { name="Justin Güse", email="guese.justin@gmail.com" },
 ]
 description = "A python package to interact with the tradingbot22 backend. used in tradingbot22-tradingbots"
 readme = "README.md"
-version = "0.3.25"
+version = "0.3.26"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

