# Comparing `tmp/stockaid-0.1.tar.gz` & `tmp/stockaid-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockaid-0.1.tar", last modified: Fri Aug 26 00:10:25 2022, max compression
+gzip compressed data, was "stockaid-0.2.tar", last modified: Tue Jul 25 20:29:23 2023, max compression
```

## Comparing `stockaid-0.1.tar` & `stockaid-0.2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0       17 2022-08-25 23:55:06.477954 stockaid-0.1/.gitignore
--rw-r--r--   0        0        0    11357 2022-08-25 22:47:35.743106 stockaid-0.1/LICENSE
--rw-r--r--   0        0        0      592 2022-08-26 00:04:03.312933 stockaid-0.1/pyproject.toml
--rw-r--r--   0        0        0    18440 2022-08-25 23:49:29.477966 stockaid-0.1/stockaid/LSTM.py
--rw-r--r--   0        0        0     9466 2022-08-25 23:50:05.447965 stockaid-0.1/stockaid/MiniZinc/__init__.py
--rw-r--r--   0        0        0     7043 2022-08-25 23:49:41.438966 stockaid-0.1/stockaid/TDA.py
--rw-r--r--   0        0        0     1878 2022-08-25 23:49:24.002967 stockaid-0.1/stockaid/__init__.py
--rw-r--r--   0        0        0     8399 2022-08-25 23:49:03.875967 stockaid-0.1/stockaid/cache.py
--rw-r--r--   0        0        0     1495 2022-08-25 23:49:09.963967 stockaid-0.1/stockaid/future_algo.py
--rw-r--r--   0        0        0     5726 2022-08-25 23:49:48.909965 stockaid-0.1/stockaid/greeks/__init__.py
--rw-r--r--   0        0        0     5688 2022-08-25 23:49:16.496967 stockaid-0.1/stockaid/index.py
--rw-r--r--   0        0        0     1435 2022-08-25 23:49:58.197965 stockaid-0.1/stockaid/logging/__init__.py
--rw-r--r--   0        0        0     2114 2022-08-25 23:50:14.189964 stockaid-0.1/stockaid/throttle/__init__.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 stockaid-0.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2022-08-26 20:20:59.589182 stockaid-0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2022-08-26 20:20:59.589182 stockaid-0.2/LICENSE
+-rw-r--r--   0        0        0      380 2022-08-26 20:20:59.589182 stockaid-0.2/README.md
+-rw-r--r--   0        0        0     2072 2022-08-26 20:20:59.589182 stockaid-0.2/docs/source/api.rst
+-rw-r--r--   0        0        0        0 2022-08-26 20:20:59.589182 stockaid-0.2/docs/source/constraint.rst
+-rw-r--r--   0        0        0      294 2022-08-26 20:20:59.589182 stockaid-0.2/docs/source/index.rst
+-rw-r--r--   0        0        0     3293 2022-08-26 20:20:59.589182 stockaid-0.2/docs/source/quickstart.rst
+-rw-r--r--   0        0        0      592 2022-08-26 20:20:59.589182 stockaid-0.2/pyproject.toml
+-rw-r--r--   0        0        0    18440 2022-08-26 20:20:59.590182 stockaid-0.2/stockaid/LSTM.py
+-rw-r--r--   0        0        0     9466 2022-08-26 20:20:59.590182 stockaid-0.2/stockaid/MiniZinc/__init__.py
+-rw-r--r--   0        0        0     7041 2022-11-30 01:47:36.106610 stockaid-0.2/stockaid/TDA.py
+-rw-r--r--   0        0        0     1878 2023-07-25 20:29:17.432707 stockaid-0.2/stockaid/__init__.py
+-rw-r--r--   0        0        0     8399 2022-08-26 20:20:59.590182 stockaid-0.2/stockaid/cache.py
+-rw-r--r--   0        0        0     1495 2022-08-26 20:20:59.590182 stockaid-0.2/stockaid/future_algo.py
+-rw-r--r--   0        0        0     5726 2022-08-26 20:20:59.591182 stockaid-0.2/stockaid/greeks/__init__.py
+-rw-r--r--   0        0        0     5688 2022-08-26 20:20:59.591182 stockaid-0.2/stockaid/index.py
+-rw-r--r--   0        0        0     1435 2022-08-26 20:20:59.591182 stockaid-0.2/stockaid/logging/__init__.py
+-rw-r--r--   0        0        0     2114 2022-08-26 20:20:59.591182 stockaid-0.2/stockaid/throttle/__init__.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 stockaid-0.2/PKG-INFO
```

### Comparing `stockaid-0.1/LICENSE` & `stockaid-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/pyproject.toml` & `stockaid-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/stockaid/LSTM.py` & `stockaid-0.2/stockaid/LSTM.py`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/stockaid/MiniZinc/__init__.py` & `stockaid-0.2/stockaid/MiniZinc/__init__.py`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/stockaid/TDA.py` & `stockaid-0.2/stockaid/TDA.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 # lastSize lowPrice marginable mark markChangeInDouble
 # markPercentChangeInDouble nAV netChange netPercentChangeInDouble openPrice
 # peRatio quoteTimeInLong realtimeEntitled regularMarketLastPrice
 # regularMarketLastSize regularMarketNetChange
 # regularMarketPercentChangeInDouble regularMarketTradeTimeInLong
 # securityStatus shortable symbol totalVolume tradeTimeInLong volatility
 def pandify_quote(resp):
-    return pd.read_json(resp, orient='records', convert_dates=False)
+    return pd.read_json(resp, orient='index', convert_dates=False)
 
 
 # columns=['datetime','open','close','high','low','volume']
 def pandify_history(resp):
     try:
         obj = json.loads(resp)
         if obj['empty']:
@@ -134,15 +134,15 @@
     except:
         return None
 
     return df
 
 
 def register_TDA(cache):
-    throt = LazyTokenBucket(120)
+    throt = LazyTokenBucket(100)
     cache.register_provider('TDA',
                        'https://api.tdameritrade.com/v1/marketdata/', throt)
     cache.register_api('TDA', 'quote', '{symbol}/quotes', 'symbol',
                        pandify_quote, key_map={'apikey':'TDA'},
                        url_params=['symbol'], cache_secs=60)
     cache.register_api('TDA', 'history', '{symbol}/pricehistory', 'symbol',
                        pandify_history, key_map={'apikey':'TDA'},
```

### Comparing `stockaid-0.1/stockaid/__init__.py` & `stockaid-0.2/stockaid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Fetching and ML pre-processing of (free) stock data.
    Also included are utilities for interfacing with MiniZinc programs, and for
    using option Greeks to convert predictions about stock prices into
    predictions about option prices.
 """
 
-__version__ = "0.1"
+__version__ = "0.2"
 
 _stockaid_cache = None
 
 from .cache import APICache
 from .future_algo import Future
 from .index import register_index
 from .TDA import register_TDA
```

### Comparing `stockaid-0.1/stockaid/cache.py` & `stockaid-0.2/stockaid/cache.py`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/stockaid/future_algo.py` & `stockaid-0.2/stockaid/future_algo.py`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/stockaid/greeks/__init__.py` & `stockaid-0.2/stockaid/greeks/__init__.py`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/stockaid/index.py` & `stockaid-0.2/stockaid/index.py`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/stockaid/logging/__init__.py` & `stockaid-0.2/stockaid/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/stockaid/throttle/__init__.py` & `stockaid-0.2/stockaid/throttle/__init__.py`

 * *Files identical despite different names*

### Comparing `stockaid-0.1/PKG-INFO` & `stockaid-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockaid
-Version: 0.1
+Version: 0.2
 Summary: Fetching and ML pre-processing of (free) stock data.
 Author-email: Jesse Dutton <jessedutton@gmail.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

