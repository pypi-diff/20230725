# Comparing `tmp/StockExchange-0.0.1.tar.gz` & `tmp/StockExchange-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StockExchange-0.0.1.tar", last modified: Mon Jul 24 13:33:42 2023, max compression
+gzip compressed data, was "StockExchange-0.0.2.tar", last modified: Tue Jul 25 05:56:00 2023, max compression
```

## Comparing `StockExchange-0.0.1.tar` & `StockExchange-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-24 13:33:42.262288 StockExchange-0.0.1/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1075 2023-07-24 13:08:44.000000 StockExchange-0.0.1/LICENSE
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2669 2023-07-24 13:33:42.262288 StockExchange-0.0.1/PKG-INFO
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2117 2023-07-24 13:27:44.000000 StockExchange-0.0.1/README.md
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-24 13:33:42.262288 StockExchange-0.0.1/StockExchange/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       22 2023-07-24 13:02:46.000000 StockExchange-0.0.1/StockExchange/__init__.py
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     6693 2023-07-24 13:02:46.000000 StockExchange-0.0.1/StockExchange/nsestock.py
-drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-24 13:33:42.262288 StockExchange-0.0.1/StockExchange.egg-info/
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2669 2023-07-24 13:33:42.000000 StockExchange-0.0.1/StockExchange.egg-info/PKG-INFO
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)      262 2023-07-24 13:33:42.000000 StockExchange-0.0.1/StockExchange.egg-info/SOURCES.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)        1 2023-07-24 13:33:42.000000 StockExchange-0.0.1/StockExchange.egg-info/dependency_links.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       47 2023-07-24 13:33:42.000000 StockExchange-0.0.1/StockExchange.egg-info/requires.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       14 2023-07-24 13:33:42.000000 StockExchange-0.0.1/StockExchange.egg-info/top_level.txt
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       38 2023-07-24 13:33:42.262288 StockExchange-0.0.1/setup.cfg
--rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1178 2023-07-24 13:07:10.000000 StockExchange-0.0.1/setup.py
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 05:56:00.806900 StockExchange-0.0.2/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1075 2023-07-24 13:08:44.000000 StockExchange-0.0.2/LICENSE
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2668 2023-07-25 05:56:00.806900 StockExchange-0.0.2/PKG-INFO
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2117 2023-07-24 13:27:44.000000 StockExchange-0.0.2/README.md
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 05:56:00.802900 StockExchange-0.0.2/StockExchange/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       22 2023-07-24 13:02:46.000000 StockExchange-0.0.2/StockExchange/__init__.py
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     6669 2023-07-25 05:46:39.000000 StockExchange-0.0.2/StockExchange/nsestock.py
+drwxrwxr-x   0 kausahl   (1000) kausahl   (1000)        0 2023-07-25 05:56:00.802900 StockExchange-0.0.2/StockExchange.egg-info/
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     2668 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/PKG-INFO
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)      262 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/SOURCES.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)        1 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/dependency_links.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       47 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/requires.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       14 2023-07-25 05:56:00.000000 StockExchange-0.0.2/StockExchange.egg-info/top_level.txt
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)       38 2023-07-25 05:56:00.806900 StockExchange-0.0.2/setup.cfg
+-rw-rw-r--   0 kausahl   (1000) kausahl   (1000)     1177 2023-07-25 05:53:23.000000 StockExchange-0.0.2/setup.py
```

### Comparing `StockExchange-0.0.1/LICENSE` & `StockExchange-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `StockExchange-0.0.1/PKG-INFO` & `StockExchange-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: StockExchange
-Version: 0.0.1
+Version: 0.0.2
 Summary: indian stock data featch
 Author: Kaushal Zine
 Author-email: <kaushalzine.it@gmail.com>
-Keywords: python,nse,stream,sharemarket,Stock market,csv
+Keywords: python,nse,stock,sharemarket,Stock market,csv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `StockExchange-0.0.1/README.md` & `StockExchange-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `StockExchange-0.0.1/StockExchange/nsestock.py` & `StockExchange-0.0.2/StockExchange/nsestock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from nsepython import *
 import requests
 from datetime import datetime
 import json
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import csv
```

### Comparing `StockExchange-0.0.1/StockExchange.egg-info/PKG-INFO` & `StockExchange-0.0.2/StockExchange.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: StockExchange
-Version: 0.0.1
+Version: 0.0.2
 Summary: indian stock data featch
 Author: Kaushal Zine
 Author-email: <kaushalzine.it@gmail.com>
-Keywords: python,nse,stream,sharemarket,Stock market,csv
+Keywords: python,nse,stock,sharemarket,Stock market,csv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `StockExchange-0.0.1/setup.py` & `StockExchange-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'indian stock data featch'
 LONG_DESCRIPTION = 'Featach difrant type of stock data, using nse baskend rest api. and create csv file and reprent graph format.'
 
 # Setting up
 setup(
     name="StockExchange",
     version=VERSION,
     author="Kaushal Zine",
     author_email="<kaushalzine.it@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['opencv-python', 'numpy', 'pandas', 'matplotlib','datetime'],
-    keywords=['python', 'nse', 'stream', 'sharemarket', 'Stock market', 'csv'],
+    keywords=['python', 'nse', 'stock', 'sharemarket', 'Stock market', 'csv'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

