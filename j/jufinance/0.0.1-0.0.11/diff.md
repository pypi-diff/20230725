# Comparing `tmp/jufinance-0.0.1.tar.gz` & `tmp/jufinance-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jufinance-0.0.1.tar", last modified: Tue Jul 25 21:23:01 2023, max compression
+gzip compressed data, was "jufinance-0.0.11.tar", last modified: Tue Jul 25 21:29:05 2023, max compression
```

## Comparing `jufinance-0.0.1.tar` & `jufinance-0.0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:23:01.377931 jufinance-0.0.1/
--rw-r--r--   0 prannay    (501) staff       (20)      633 2023-07-25 21:23:01.377713 jufinance-0.0.1/PKG-INFO
-drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:23:01.376258 jufinance-0.0.1/jufinance/
--rw-r--r--   0 prannay    (501) staff       (20)       47 2023-07-25 20:40:36.000000 jufinance-0.0.1/jufinance/__init__.py
--rw-r--r--   0 prannay    (501) staff       (20)       40 2023-04-16 20:00:34.000000 jufinance-0.0.1/jufinance/historical.py
--rw-r--r--   0 prannay    (501) staff       (20)     4816 2023-07-25 21:10:24.000000 jufinance-0.0.1/jufinance/quote.py
-drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:23:01.377454 jufinance-0.0.1/jufinance/scrapers/
--rw-r--r--   0 prannay    (501) staff       (20)       77 2023-07-25 20:47:32.000000 jufinance-0.0.1/jufinance/scrapers/__init__.py
--rw-r--r--   0 prannay    (501) staff       (20)     3133 2023-07-25 21:06:44.000000 jufinance-0.0.1/jufinance/scrapers/investing.py
--rw-r--r--   0 prannay    (501) staff       (20)     5840 2023-07-25 21:11:01.000000 jufinance-0.0.1/jufinance/scrapers/moneycontrol.py
--rw-r--r--   0 prannay    (501) staff       (20)     7986 2023-07-25 21:10:49.000000 jufinance-0.0.1/jufinance/scrapers/screener.py
-drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:23:01.376947 jufinance-0.0.1/jufinance.egg-info/
--rw-r--r--   0 prannay    (501) staff       (20)      633 2023-07-25 21:23:01.000000 jufinance-0.0.1/jufinance.egg-info/PKG-INFO
--rw-r--r--   0 prannay    (501) staff       (20)      366 2023-07-25 21:23:01.000000 jufinance-0.0.1/jufinance.egg-info/SOURCES.txt
--rw-r--r--   0 prannay    (501) staff       (20)        1 2023-07-25 21:23:01.000000 jufinance-0.0.1/jufinance.egg-info/dependency_links.txt
--rw-r--r--   0 prannay    (501) staff       (20)      253 2023-07-25 21:23:01.000000 jufinance-0.0.1/jufinance.egg-info/requires.txt
--rw-r--r--   0 prannay    (501) staff       (20)       10 2023-07-25 21:23:01.000000 jufinance-0.0.1/jufinance.egg-info/top_level.txt
--rw-r--r--   0 prannay    (501) staff       (20)       38 2023-07-25 21:23:01.377983 jufinance-0.0.1/setup.cfg
--rw-r--r--   0 prannay    (501) staff       (20)     1562 2023-07-25 21:21:54.000000 jufinance-0.0.1/setup.py
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:29:05.048964 jufinance-0.0.11/
+-rw-r--r--   0 prannay    (501) staff       (20)      634 2023-07-25 21:29:05.048816 jufinance-0.0.11/PKG-INFO
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:29:05.047333 jufinance-0.0.11/jufinance/
+-rw-r--r--   0 prannay    (501) staff       (20)       47 2023-07-25 20:40:36.000000 jufinance-0.0.11/jufinance/__init__.py
+-rw-r--r--   0 prannay    (501) staff       (20)       40 2023-04-16 20:00:34.000000 jufinance-0.0.11/jufinance/historical.py
+-rw-r--r--   0 prannay    (501) staff       (20)     4817 2023-07-25 21:27:22.000000 jufinance-0.0.11/jufinance/quote.py
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:29:05.048621 jufinance-0.0.11/jufinance/scrapers/
+-rw-r--r--   0 prannay    (501) staff       (20)       77 2023-07-25 20:47:32.000000 jufinance-0.0.11/jufinance/scrapers/__init__.py
+-rw-r--r--   0 prannay    (501) staff       (20)     3133 2023-07-25 21:06:44.000000 jufinance-0.0.11/jufinance/scrapers/investing.py
+-rw-r--r--   0 prannay    (501) staff       (20)     5840 2023-07-25 21:11:01.000000 jufinance-0.0.11/jufinance/scrapers/moneycontrol.py
+-rw-r--r--   0 prannay    (501) staff       (20)     7986 2023-07-25 21:10:49.000000 jufinance-0.0.11/jufinance/scrapers/screener.py
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:29:05.048046 jufinance-0.0.11/jufinance.egg-info/
+-rw-r--r--   0 prannay    (501) staff       (20)      634 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/PKG-INFO
+-rw-r--r--   0 prannay    (501) staff       (20)      366 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/SOURCES.txt
+-rw-r--r--   0 prannay    (501) staff       (20)        1 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/dependency_links.txt
+-rw-r--r--   0 prannay    (501) staff       (20)      253 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/requires.txt
+-rw-r--r--   0 prannay    (501) staff       (20)       10 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/top_level.txt
+-rw-r--r--   0 prannay    (501) staff       (20)       38 2023-07-25 21:29:05.049005 jufinance-0.0.11/setup.cfg
+-rw-r--r--   0 prannay    (501) staff       (20)     1563 2023-07-25 21:28:32.000000 jufinance-0.0.11/setup.py
```

### Comparing `jufinance-0.0.1/PKG-INFO` & `jufinance-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jufinance
-Version: 0.0.1
+Version: 0.0.11
 Summary: Python Package to access Indian Stock market data.
 Home-page: UNKNOWN
 Author: Prannay Kedia & Sparsh Gupta
 Author-email: <prannaykedia1@gmail.com>, <sparshgupta2407@gmail.com>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `jufinance-0.0.1/jufinance/quote.py` & `jufinance-0.0.11/jufinance/quote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Get the quote details
 # - current price, company info, etc.
 
-from efinance.scrapers import Investing, MoneyControl, Screener
+from jufinance.scrapers import Investing, MoneyControl, Screener
 
 
 class Quote:
     def __init__(self, ticker):
         # print("Invoked Quote module...")
         self.screener = Screener(ticker=ticker)
         self.screener.get_soup()
```

### Comparing `jufinance-0.0.1/jufinance/scrapers/investing.py` & `jufinance-0.0.11/jufinance/scrapers/investing.py`

 * *Files identical despite different names*

### Comparing `jufinance-0.0.1/jufinance/scrapers/moneycontrol.py` & `jufinance-0.0.11/jufinance/scrapers/moneycontrol.py`

 * *Files identical despite different names*

### Comparing `jufinance-0.0.1/jufinance/scrapers/screener.py` & `jufinance-0.0.11/jufinance/scrapers/screener.py`

 * *Files identical despite different names*

### Comparing `jufinance-0.0.1/jufinance.egg-info/PKG-INFO` & `jufinance-0.0.11/jufinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jufinance
-Version: 0.0.1
+Version: 0.0.11
 Summary: Python Package to access Indian Stock market data.
 Home-page: UNKNOWN
 Author: Prannay Kedia & Sparsh Gupta
 Author-email: <prannaykedia1@gmail.com>, <sparshgupta2407@gmail.com>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `jufinance-0.0.1/setup.py` & `jufinance-0.0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.11"
 DESCRIPTION = "Python Package to access Indian Stock market data."
 LONG_DESCRIPTION = "Python Package to access Indian Stock market data. This is for educational purposes only."
 
 # Setting up
 setup(
     name="jufinance",
     version=VERSION,
```

