# Comparing `tmp/finterion-0.3.tar.gz` & `tmp/finterion-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finterion-0.3.tar", last modified: Fri Jul 21 21:02:32 2023, max compression
+gzip compressed data, was "finterion-0.4.tar", last modified: Tue Jul 25 09:58:16 2023, max compression
```

## Comparing `finterion-0.3.tar` & `finterion-0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.631711 finterion-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-21 21:02:24.000000 finterion-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-21 21:02:32.631711 finterion-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-21 21:02:24.000000 finterion-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.627711 finterion-0.3/finterion/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-21 21:02:24.000000 finterion-0.3/finterion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.627711 finterion-0.3/finterion/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:24.000000 finterion-0.3/finterion/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 21:02:24.000000 finterion-0.3/finterion/configuration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 21:02:24.000000 finterion-0.3/finterion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-21 21:02:24.000000 finterion-0.3/finterion/finterion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.631711 finterion-0.3/finterion/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/algorithm_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/order_side.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/order_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-21 21:02:24.000000 finterion-0.3/finterion/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.627711 finterion-0.3/finterion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 21:02:32.631711 finterion-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-21 21:02:24.000000 finterion-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:16.931381 finterion-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-25 09:58:09.000000 finterion-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-25 09:58:16.931381 finterion-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-25 09:58:09.000000 finterion-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:16.927381 finterion-0.4/finterion/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-25 09:58:09.000000 finterion-0.4/finterion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:16.931381 finterion-0.4/finterion/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:09.000000 finterion-0.4/finterion/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-25 09:58:09.000000 finterion-0.4/finterion/configuration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-25 09:58:09.000000 finterion-0.4/finterion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-25 09:58:09.000000 finterion-0.4/finterion/finterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:16.931381 finterion-0.4/finterion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/algorithm_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-25 09:58:09.000000 finterion-0.4/finterion/models/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-25 09:58:09.000000 finterion-0.4/finterion/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:16.931381 finterion-0.4/finterion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-25 09:58:16.000000 finterion-0.4/finterion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-25 09:58:16.000000 finterion-0.4/finterion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:58:16.000000 finterion-0.4/finterion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 09:58:16.000000 finterion-0.4/finterion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 09:58:16.000000 finterion-0.4/finterion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:58:16.931381 finterion-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-25 09:58:09.000000 finterion-0.4/setup.py
```

### Comparing `finterion-0.3/LICENSE` & `finterion-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finterion-0.3/PKG-INFO` & `finterion-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion
-Version: 0.3
+Version: 0.4
 Summary: Official python client for Finterion
 Home-page: https://github.com/finterion/finterion-python-client.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `finterion-0.3/README.md` & `finterion-0.4/README.md`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/finterion.py` & `finterion-0.4/finterion/finterion.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/models/algorithm.py` & `finterion-0.4/finterion/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/models/algorithm_profile.py` & `finterion-0.4/finterion/models/algorithm_profile.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/models/order.py` & `finterion-0.4/finterion/models/order.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/models/order_side.py` & `finterion-0.4/finterion/models/order_side.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/models/order_status.py` & `finterion-0.4/finterion/models/order_status.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/models/order_type.py` & `finterion-0.4/finterion/models/order_type.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/models/portfolio.py` & `finterion-0.4/finterion/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/models/position.py` & `finterion-0.4/finterion/models/position.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion/services.py` & `finterion-0.4/finterion/services.py`

 * *Files identical despite different names*

### Comparing `finterion-0.3/finterion.egg-info/PKG-INFO` & `finterion-0.4/finterion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion
-Version: 0.3
+Version: 0.4
 Summary: Official python client for Finterion
 Home-page: https://github.com/finterion/finterion-python-client.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `finterion-0.3/finterion.egg-info/SOURCES.txt` & `finterion-0.4/finterion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finterion-0.3/setup.py` & `finterion-0.4/setup.py`

 * *Files identical despite different names*

