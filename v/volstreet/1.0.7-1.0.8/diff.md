# Comparing `tmp/volstreet-1.0.7.tar.gz` & `tmp/volstreet-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.0.7.tar", last modified: Tue Jul 25 18:05:05 2023, max compression
+gzip compressed data, was "volstreet-1.0.8.tar", last modified: Tue Jul 25 18:08:46 2023, max compression
```

## Comparing `volstreet-1.0.7.tar` & `volstreet-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:05:05.320165 volstreet-1.0.7/
--rw-rw-rw-   0        0        0      497 2023-07-25 18:05:05.320165 volstreet-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.7/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-07-25 18:05:05.321669 volstreet-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 18:05:05.314186 volstreet-1.0.7/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.7/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.7/volstreet/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.7/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.7/volstreet/constants.py
--rw-rw-rw-   0        0        0    43796 2023-07-25 18:04:18.000000 volstreet-1.0.7/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   192160 2023-07-25 17:19:23.000000 volstreet-1.0.7/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.7/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.7/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.7/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    13488 2023-07-25 17:19:23.000000 volstreet-1.0.7/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:05:05.319170 volstreet-1.0.7/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 18:05:05.000000 volstreet-1.0.7/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 18:08:46.106504 volstreet-1.0.8/
+-rw-rw-rw-   0        0        0      497 2023-07-25 18:08:46.107499 volstreet-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.8/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-07-25 18:08:46.107499 volstreet-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 18:08:46.102415 volstreet-1.0.8/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.8/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.8/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.8/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.8/volstreet/constants.py
+-rw-rw-rw-   0        0        0    43796 2023-07-25 18:04:18.000000 volstreet-1.0.8/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   192160 2023-07-25 17:19:23.000000 volstreet-1.0.8/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.8/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.8/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.8/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    13488 2023-07-25 17:19:23.000000 volstreet-1.0.8/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:08:46.106504 volstreet-1.0.8/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 18:08:46.000000 volstreet-1.0.8/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.0.7/setup.cfg` & `volstreet-1.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 370d 0a61  rsion = 1.0.7..a
+00000020: 7273 696f 6e20 3d20 312e 302e 380d 0a61  rsion = 1.0.8..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-1.0.7/volstreet/SmartWebSocketV2.py` & `volstreet-1.0.8/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.7/volstreet/blackscholes.py` & `volstreet-1.0.8/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.7/volstreet/constants.py` & `volstreet-1.0.8/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.7/volstreet/datamodule.py` & `volstreet-1.0.8/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.7/volstreet/dealingroom.py` & `volstreet-1.0.8/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.7/volstreet/discord_bot.py` & `volstreet-1.0.8/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.7/volstreet/nsefunctions.py` & `volstreet-1.0.8/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.7/volstreet/strategies.py` & `volstreet-1.0.8/volstreet/strategies.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.7/volstreet.egg-info/requires.txt` & `volstreet-1.0.8/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

