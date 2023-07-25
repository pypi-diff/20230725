# Comparing `tmp/SMAGrader-0.1.0.tar.gz` & `tmp/SMAGrader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMAGrader-0.1.0.tar", last modified: Tue Jul 25 18:50:37 2023, max compression
+gzip compressed data, was "SMAGrader-0.1.1.tar", last modified: Tue Jul 25 19:13:20 2023, max compression
```

## Comparing `SMAGrader-0.1.0.tar` & `SMAGrader-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:50:37.106936 SMAGrader-0.1.0/
--rw-rw-rw-   0        0        0      151 2023-07-25 18:50:37.105935 SMAGrader-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 18:50:37.082932 SMAGrader-0.1.0/SMAGrader/
--rw-rw-rw-   0        0        0        0 2023-06-26 19:41:13.000000 SMAGrader-0.1.0/SMAGrader/__init__.py
--rw-rw-rw-   0        0        0    18718 2023-07-25 18:16:10.000000 SMAGrader-0.1.0/SMAGrader/checker.py
--rw-rw-rw-   0        0        0      112 2023-07-11 20:15:42.000000 SMAGrader-0.1.0/SMAGrader/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:50:37.102934 SMAGrader-0.1.0/SMAGrader.egg-info/
--rw-rw-rw-   0        0        0      151 2023-07-25 18:50:36.000000 SMAGrader-0.1.0/SMAGrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-25 18:50:36.000000 SMAGrader-0.1.0/SMAGrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:50:36.000000 SMAGrader-0.1.0/SMAGrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-25 18:50:36.000000 SMAGrader-0.1.0/SMAGrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 18:50:36.000000 SMAGrader-0.1.0/SMAGrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 18:50:37.106936 SMAGrader-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-07-24 21:05:43.000000 SMAGrader-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:13:20.838900 SMAGrader-0.1.1/
+-rw-rw-rw-   0        0        0      151 2023-07-25 19:13:20.837900 SMAGrader-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 19:13:20.817626 SMAGrader-0.1.1/SMAGrader/
+-rw-rw-rw-   0        0        0       16 2023-07-25 19:00:48.000000 SMAGrader-0.1.1/SMAGrader/__init__.py
+-rw-rw-rw-   0        0        0    18855 2023-07-25 19:11:05.000000 SMAGrader-0.1.1/SMAGrader/checker.py
+-rw-rw-rw-   0        0        0      112 2023-07-11 20:15:42.000000 SMAGrader-0.1.1/SMAGrader/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:13:20.835901 SMAGrader-0.1.1/SMAGrader.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-07-25 19:13:20.000000 SMAGrader-0.1.1/SMAGrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-07-25 19:13:20.000000 SMAGrader-0.1.1/SMAGrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 19:13:20.000000 SMAGrader-0.1.1/SMAGrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-25 19:13:20.000000 SMAGrader-0.1.1/SMAGrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 19:13:20.000000 SMAGrader-0.1.1/SMAGrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 19:13:20.838900 SMAGrader-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      426 2023-07-25 19:12:54.000000 SMAGrader-0.1.1/setup.py
```

### Comparing `SMAGrader-0.1.0/SMAGrader/checker.py` & `SMAGrader-0.1.1/SMAGrader/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 import nltk
 from nltk.sentiment import SentimentIntensityAnalyzer
 from nltk import ne_chunk
 from nltk.tokenize import word_tokenize
 from nltk.tag import pos_tag
 import json
 import praw
-from constants import client_id, client_secret, user_agent
+
+# from constants import client_id, client_secret, user_agent
 import firebase_admin
 from firebase_admin import credentials, firestore
 import os
 
+client_id = os.environ.get("client_id")
+client_secret = os.environ.get("client_secret")
+user_agent = os.environ.get("user_agent")
 path = os.environ.get("google_credentials")
 cred = credentials.Certificate(path)
 firebase_admin.initialize_app(cred)
 db = firestore.client()
 
 
 def authenticate():
```

