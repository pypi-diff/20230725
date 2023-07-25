# Comparing `tmp/StockExchange-0.0.2.tar.gz` & `tmp/StockExchange-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StockExchange-0.0.2.tar", last modified: Tue Jul 25 05:56:00 2023, max compression
+gzip compressed data, was "StockExchange-0.0.3.tar", last modified: Tue Jul 25 06:25:58 2023, max compression
```

## Comparing `StockExchange-0.0.2.tar` & `StockExchange-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 05:56:00.806900 StockExchange-0.0.2/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1075 2023-07-24 13:08:44.000000 StockExchange-0.0.2/LICENSE
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2668 2023-07-25 05:56:00.806900 StockExchange-0.0.2/PKG-INFO
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2117 2023-07-24 13:27:44.000000 StockExchange-0.0.2/README.md
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 05:56:00.802900 StockExchange-0.0.2/StockExchange/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       22 2023-07-24 13:02:46.000000 StockExchange-0.0.2/StockExchange/__init__.py
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     6669 2023-07-25 05:46:39.000000 StockExchange-0.0.2/StockExchange/nsestock.py
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 05:56:00.802900 StockExchange-0.0.2/StockExchange.egg-info/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2668 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/PKG-INFO
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)      262 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/SOURCES.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)        1 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/dependency_links.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       47 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/requires.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       14 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/top_level.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       38 2023-07-25 05:56:00.806900 StockExchange-0.0.2/setup.cfg
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1177 2023-07-25 05:53:23.000000 StockExchange-0.0.2/setup.py
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 06:25:58.990085 StockExchange-0.0.3/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1075 2023-07-24 13:08:44.000000 StockExchange-0.0.3/LICENSE
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     3845 2023-07-25 06:25:58.986085 StockExchange-0.0.3/PKG-INFO
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     3293 2023-07-25 06:23:03.000000 StockExchange-0.0.3/README.md
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 06:25:58.986085 StockExchange-0.0.3/StockExchange/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       87 2023-07-25 06:18:33.000000 StockExchange-0.0.3/StockExchange/__init__.py
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     6669 2023-07-25 06:18:41.000000 StockExchange-0.0.3/StockExchange/nsestock.py
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 06:25:58.986085 StockExchange-0.0.3/StockExchange.egg-info/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     3845 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/PKG-INFO
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)      262 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/SOURCES.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)        1 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/dependency_links.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       47 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/requires.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       14 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/top_level.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       38 2023-07-25 06:25:58.990085 StockExchange-0.0.3/setup.cfg
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1177 2023-07-25 06:23:40.000000 StockExchange-0.0.3/setup.py
```

### Comparing `StockExchange-0.0.2/LICENSE` & `StockExchange-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `StockExchange-0.0.2/PKG-INFO` & `StockExchange-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: StockExchange
-Version: 0.0.2
-Summary: indian stock data featch
-Author: Kaushal Zine
-Author-email: <kaushalzine.it@gmail.com>
-Keywords: python,nse,stock,sharemarket,Stock market,csv
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # StockExchange
 stock data featch
 
     1. nse_main() -
     2. CSV Model -
         Convert Payload json data  data to CSV using Data frame 
         read CSV File => data = pd.read_csv(filename)
@@ -76,7 +59,44 @@
                 createdAt
                 updatedAt
                 __v
                 VWAP
                 mTIMESTAMP
 
             • Plot graph in linear scal  using Graph method 
+
+
+    6. Equity List- 
+        NSE listed company List.
+        Method-  equitytop_loosers()
+        predata – MCAP31032023_0.xlsx (Download using link https://www.nseindia.com/regulations/listing-compliance/nse-market-capitalisation-all-companies)
+        output – Teminal output Symbol of listed company
+                Create CSV File 
+                    Sr. No.
+                    Symbol
+                    Company Name
+                    Market capitalization as on March 31, 2023 (Rs in Lakhs)
+
+    7. Fno List -
+        Futures and Options data file.
+        Method – fno_list()
+        Output - fnolist, count
+            CSV File 
+
+    8. Equity Top Gainers-
+        Method – equitytop_gainers()
+        output – create top gainer  csv file 
+
+
+    9. Equity Top Loosers-
+        Method – equitytop_loosers()
+
+    10.  Option Chain-
+        Option chain data dispaly in terminal 
+        Indices OPTION – NIFTY, FINNIFTY, BANKNIFTY
+        Equities  OPTION -  all symbol
+        method  -optionchain(symbol)
+        Use - fnolist = optionchain('NIFTY')		
+	
+    11 . Top 25  Valume -
+        method – top_valume()
+        output – create csv File
```

### Comparing `StockExchange-0.0.2/StockExchange/nsestock.py` & `StockExchange-0.0.3/StockExchange/nsestock.py`

 * *Files identical despite different names*

### Comparing `StockExchange-0.0.2/setup.py` & `StockExchange-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'indian stock data featch'
 LONG_DESCRIPTION = 'Featach difrant type of stock data, using nse baskend rest api. and create csv file and reprent graph format.'
 
 # Setting up
 setup(
     name="StockExchange",
     version=VERSION,
```

