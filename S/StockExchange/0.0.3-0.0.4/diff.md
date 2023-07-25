# Comparing `tmp/StockExchange-0.0.3.tar.gz` & `tmp/StockExchange-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StockExchange-0.0.3.tar", last modified: Tue Jul 25 06:25:58 2023, max compression
+gzip compressed data, was "StockExchange-0.0.4.tar", last modified: Tue Jul 25 08:23:09 2023, max compression
```

## Comparing `StockExchange-0.0.3.tar` & `StockExchange-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 06:25:58.990085 StockExchange-0.0.3/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1075 2023-07-24 13:08:44.000000 StockExchange-0.0.3/LICENSE
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     3845 2023-07-25 06:25:58.986085 StockExchange-0.0.3/PKG-INFO
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     3293 2023-07-25 06:23:03.000000 StockExchange-0.0.3/README.md
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 06:25:58.986085 StockExchange-0.0.3/StockExchange/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       87 2023-07-25 06:18:33.000000 StockExchange-0.0.3/StockExchange/__init__.py
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     6669 2023-07-25 06:18:41.000000 StockExchange-0.0.3/StockExchange/nsestock.py
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 06:25:58.986085 StockExchange-0.0.3/StockExchange.egg-info/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     3845 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/PKG-INFO
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)      262 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/SOURCES.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)        1 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/dependency_links.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       47 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/requires.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       14 2023-07-25 06:25:58.000000 StockExchange-0.0.3/StockExchange.egg-info/top_level.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       38 2023-07-25 06:25:58.990085 StockExchange-0.0.3/setup.cfg
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1177 2023-07-25 06:23:40.000000 StockExchange-0.0.3/setup.py
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 08:23:09.991875 StockExchange-0.0.4/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1075 2023-07-24 13:08:44.000000 StockExchange-0.0.4/LICENSE
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     4341 2023-07-25 08:23:09.991875 StockExchange-0.0.4/PKG-INFO
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     3757 2023-07-25 06:55:47.000000 StockExchange-0.0.4/README.md
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 08:23:09.991875 StockExchange-0.0.4/StockExchange/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       87 2023-07-25 06:18:33.000000 StockExchange-0.0.4/StockExchange/__init__.py
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     6669 2023-07-25 06:18:41.000000 StockExchange-0.0.4/StockExchange/nsestock.py
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 08:23:09.991875 StockExchange-0.0.4/StockExchange.egg-info/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     4341 2023-07-25 08:23:09.000000 StockExchange-0.0.4/StockExchange.egg-info/PKG-INFO
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)      262 2023-07-25 08:23:09.000000 StockExchange-0.0.4/StockExchange.egg-info/SOURCES.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)        1 2023-07-25 08:23:09.000000 StockExchange-0.0.4/StockExchange.egg-info/dependency_links.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       60 2023-07-25 08:23:09.000000 StockExchange-0.0.4/StockExchange.egg-info/requires.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       14 2023-07-25 08:23:09.000000 StockExchange-0.0.4/StockExchange.egg-info/top_level.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       38 2023-07-25 08:23:09.991875 StockExchange-0.0.4/setup.cfg
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1224 2023-07-25 06:59:32.000000 StockExchange-0.0.4/setup.py
```

### Comparing `StockExchange-0.0.3/LICENSE` & `StockExchange-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `StockExchange-0.0.3/PKG-INFO` & `StockExchange-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: StockExchange
-Version: 0.0.3
-Summary: indian stock data featch
+Version: 0.0.4
+Summary: Indian Stock Data Featch and Represent Graphical Format 
 Author: Kaushal Zine
 Author-email: <kaushalzine.it@gmail.com>
 Keywords: python,nse,stock,sharemarket,Stock market,csv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -110,10 +110,24 @@
     10.  Option Chain-
         Option chain data dispaly in terminal 
         Indices OPTION – NIFTY, FINNIFTY, BANKNIFTY
         Equities  OPTION -  all symbol
         method  -optionchain(symbol)
         Use - fnolist = optionchain('NIFTY')		
 	
-    11 . Top 25  Valume -
+    11. Top 25  Valume -
         method – top_valume()
         output – create csv File 
+
+
+    12. MOST ACTIVE EQUITIES -
+        method – active_equities(Num)
+        parameter –> num – equities  num of stock 
+        use -  active_equities(10)
+        output -> create csv file top 10 active quities
+
+
+    13. 52week High / Low stock -
+        method – highorlow_52week(range)
+        parameter ->range – “high”  (52week High Stock)
+                          - “low”    (52week Low Stock)
+        use  - highorlow_52week(“ high”)
```

### Comparing `StockExchange-0.0.3/README.md` & `StockExchange-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -93,10 +93,24 @@
     10.  Option Chain-
         Option chain data dispaly in terminal 
         Indices OPTION – NIFTY, FINNIFTY, BANKNIFTY
         Equities  OPTION -  all symbol
         method  -optionchain(symbol)
         Use - fnolist = optionchain('NIFTY')		
 	
-    11 . Top 25  Valume -
+    11. Top 25  Valume -
         method – top_valume()
-        output – create csv File 
+        output – create csv File 
+
+
+    12. MOST ACTIVE EQUITIES -
+        method – active_equities(Num)
+        parameter –> num – equities  num of stock 
+        use -  active_equities(10)
+        output -> create csv file top 10 active quities
+
+
+    13. 52week High / Low stock -
+        method – highorlow_52week(range)
+        parameter ->range – “high”  (52week High Stock)
+                          - “low”    (52week Low Stock)
+        use  - highorlow_52week(“ high”)
```

### Comparing `StockExchange-0.0.3/StockExchange/nsestock.py` & `StockExchange-0.0.4/StockExchange/nsestock.py`

 * *Files identical despite different names*

### Comparing `StockExchange-0.0.3/StockExchange.egg-info/PKG-INFO` & `StockExchange-0.0.4/StockExchange.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: StockExchange
-Version: 0.0.3
-Summary: indian stock data featch
+Version: 0.0.4
+Summary: Indian Stock Data Featch and Represent Graphical Format 
 Author: Kaushal Zine
 Author-email: <kaushalzine.it@gmail.com>
 Keywords: python,nse,stock,sharemarket,Stock market,csv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -110,10 +110,24 @@
     10.  Option Chain-
         Option chain data dispaly in terminal 
         Indices OPTION – NIFTY, FINNIFTY, BANKNIFTY
         Equities  OPTION -  all symbol
         method  -optionchain(symbol)
         Use - fnolist = optionchain('NIFTY')		
 	
-    11 . Top 25  Valume -
+    11. Top 25  Valume -
         method – top_valume()
         output – create csv File 
+
+
+    12. MOST ACTIVE EQUITIES -
+        method – active_equities(Num)
+        parameter –> num – equities  num of stock 
+        use -  active_equities(10)
+        output -> create csv file top 10 active quities
+
+
+    13. 52week High / Low stock -
+        method – highorlow_52week(range)
+        parameter ->range – “high”  (52week High Stock)
+                          - “low”    (52week Low Stock)
+        use  - highorlow_52week(“ high”)
```

