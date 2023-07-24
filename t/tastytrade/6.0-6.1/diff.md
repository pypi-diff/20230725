# Comparing `tmp/tastytrade-6.0.tar.gz` & `tmp/tastytrade-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-6.0.tar", last modified: Sat Jul 22 02:53:52 2023, max compression
+gzip compressed data, was "tastytrade-6.1.tar", last modified: Mon Jul 24 22:17:26 2023, max compression
```

## Comparing `tastytrade-6.0.tar` & `tastytrade-6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:53:52.341702 tastytrade-6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-22 02:53:43.000000 tastytrade-6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-22 02:53:52.337702 tastytrade-6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-22 02:53:43.000000 tastytrade-6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 02:53:52.341702 tastytrade-6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-22 02:53:43.000000 tastytrade-6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:53:52.333702 tastytrade-6.0/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35162 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:53:52.337702 tastytrade-6.0/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/underlying.py
--rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:53:52.337702 tastytrade-6.0/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:17:26.326877 tastytrade-6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 22:17:11.000000 tastytrade-6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-24 22:17:26.326877 tastytrade-6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-24 22:17:11.000000 tastytrade-6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 22:17:26.326877 tastytrade-6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 22:17:11.000000 tastytrade-6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:17:26.326877 tastytrade-6.1/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35162 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:17:26.326877 tastytrade-6.1/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/dxfeed/underlying.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-24 22:17:11.000000 tastytrade-6.1/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:17:26.326877 tastytrade-6.1/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-24 22:17:26.000000 tastytrade-6.1/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 22:17:26.000000 tastytrade-6.1/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:17:26.000000 tastytrade-6.1/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 22:17:26.000000 tastytrade-6.1/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 22:17:26.000000 tastytrade-6.1/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-6.0/LICENSE` & `tastytrade-6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/PKG-INFO` & `tastytrade-6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 6.0
+Version: 6.1
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -56,15 +56,15 @@
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
    await streamer.subscribe(EventType.QUOTE, subs_list)
    # this example fetches quotes once, then exits
    quotes = []
-   async for quote in streamer.listen():
+   async for quote in streamer.listen(EventType.QUOTE):
       quotes.append(quote)
       if len(quotes) >= len(subs_list):
          break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
@@ -128,15 +128,15 @@
    from datetime import date
 
    chain = get_option_chain(session, 'SPLG')
    subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
 
    await streamer.subscribe(EventType.GREEKS, subs_list)
    greeks = []
-   async for greek in streamer.listen():
+   async for greek in streamer.listen(EventType.GREEKS):
       greeks.append(greek)
       if len(greeks) >= len(subs_list):
          break
    print(greeks)
 
 >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
```

### Comparing `tastytrade-6.0/README.rst` & `tastytrade-6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
    await streamer.subscribe(EventType.QUOTE, subs_list)
    # this example fetches quotes once, then exits
    quotes = []
-   async for quote in streamer.listen():
+   async for quote in streamer.listen(EventType.QUOTE):
       quotes.append(quote)
       if len(quotes) >= len(subs_list):
          break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
@@ -117,15 +117,15 @@
    from datetime import date
 
    chain = get_option_chain(session, 'SPLG')
    subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
 
    await streamer.subscribe(EventType.GREEKS, subs_list)
    greeks = []
-   async for greek in streamer.listen():
+   async for greek in streamer.listen(EventType.GREEKS):
       greeks.append(greek)
       if len(greeks) >= len(subs_list):
          break
    print(greeks)
 
 >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
```

### Comparing `tastytrade-6.0/setup.py` & `tastytrade-6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 f = open('README.rst', 'r')
 LONG_DESCRIPTION = f.read()
 f.close()
 
 setup(
     name='tastytrade',
-    version='6.0',
+    version='6.1',
     description='An unofficial SDK for Tastytrade!',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     author='Graeme Holliday',
     author_email='graeme.holliday@pm.me',
     url='https://github.com/tastyware/tastytrade',
     license='MIT',
```

### Comparing `tastytrade-6.0/tastytrade/__init__.py` & `tastytrade-6.1/tastytrade/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 API_URL = 'https://api.tastyworks.com'
 CERT_URL = 'https://api.cert.tastyworks.com'
-VERSION = '6.0'
+VERSION = '6.1'
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 from .account import Account  # noqa: E402
 from .search import symbol_search  # noqa: E402
 from .session import CertificationSession, ProductionSession  # noqa: E402
```

### Comparing `tastytrade-6.0/tastytrade/account.py` & `tastytrade-6.1/tastytrade/account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/__init__.py` & `tastytrade-6.1/tastytrade/dxfeed/__init__.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/candle.py` & `tastytrade-6.1/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/event.py` & `tastytrade-6.1/tastytrade/dxfeed/event.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/greeks.py` & `tastytrade-6.1/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/profile.py` & `tastytrade-6.1/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/quote.py` & `tastytrade-6.1/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/summary.py` & `tastytrade-6.1/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/theoprice.py` & `tastytrade-6.1/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/timeandsale.py` & `tastytrade-6.1/tastytrade/dxfeed/timeandsale.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/trade.py` & `tastytrade-6.1/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/dxfeed/underlying.py` & `tastytrade-6.1/tastytrade/dxfeed/underlying.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/instruments.py` & `tastytrade-6.1/tastytrade/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/metrics.py` & `tastytrade-6.1/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/order.py` & `tastytrade-6.1/tastytrade/order.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/search.py` & `tastytrade-6.1/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/session.py` & `tastytrade-6.1/tastytrade/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABC, abstractmethod
+from abc import ABC
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import requests
 
 from tastytrade import API_URL, CERT_URL
 from tastytrade.dxfeed import (Candle, Event, EventType, Greeks, Profile,
@@ -11,33 +11,18 @@
 from tastytrade.utils import TastytradeError, validate_response
 
 
 class Session(ABC):
     """
     An abstract class which contains the basic functionality of a session.
     """
-    @property
-    @abstractmethod
-    def base_url(self) -> str:
-        pass
-
-    @property
-    @abstractmethod
-    def headers(self) -> Dict[str, str]:
-        pass
-
-    @property
-    @abstractmethod
-    def user(self) -> Dict[str, str]:
-        pass
-
-    @property
-    @abstractmethod
-    def session_token(self) -> str:
-        pass
+    base_url: str
+    headers: Dict[str, str]
+    user: Dict[str, str]
+    session_token: str
 
     def validate(self) -> bool:
         """
         Validates the current session by sending a request to the API.
 
         :return: True if the session is valid and False otherwise.
         """
```

### Comparing `tastytrade-6.0/tastytrade/streamer.py` & `tastytrade-6.1/tastytrade/streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/utils.py` & `tastytrade-6.1/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade/watchlists.py` & `tastytrade-6.1/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-6.0/tastytrade.egg-info/PKG-INFO` & `tastytrade-6.1/tastytrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 6.0
+Version: 6.1
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -56,15 +56,15 @@
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
    await streamer.subscribe(EventType.QUOTE, subs_list)
    # this example fetches quotes once, then exits
    quotes = []
-   async for quote in streamer.listen():
+   async for quote in streamer.listen(EventType.QUOTE):
       quotes.append(quote)
       if len(quotes) >= len(subs_list):
          break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
@@ -128,15 +128,15 @@
    from datetime import date
 
    chain = get_option_chain(session, 'SPLG')
    subs_list = [chain[date(2023, 6, 16)][0].streamer_symbol]
 
    await streamer.subscribe(EventType.GREEKS, subs_list)
    greeks = []
-   async for greek in streamer.listen():
+   async for greek in streamer.listen(EventType.GREEKS):
       greeks.append(greek)
       if len(greeks) >= len(subs_list):
          break
    print(greeks)
 
 >>> [Greeks(eventSymbol='.SPLG230616C23', eventTime=0, eventFlags=0, index=7235129486797176832, time=1684559855338, sequence=0, price=26.3380972233688, volatility=0.396983376650804, delta=0.999999999996191, gamma=4.81989763184255e-12, theta=-2.5212017514875e-12, rho=0.01834504287973133, vega=3.7003015672215e-12)]
```

### Comparing `tastytrade-6.0/tastytrade.egg-info/SOURCES.txt` & `tastytrade-6.1/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

