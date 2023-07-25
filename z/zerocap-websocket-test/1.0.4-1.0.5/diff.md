# Comparing `tmp/zerocap_websocket_test-1.0.4.tar.gz` & `tmp/zerocap_websocket_test-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocap_websocket_test-1.0.4.tar", last modified: Tue Jul 25 02:11:05 2023, max compression
+gzip compressed data, was "zerocap_websocket_test-1.0.5.tar", last modified: Tue Jul 25 02:12:44 2023, max compression
```

## Comparing `zerocap_websocket_test-1.0.4.tar` & `zerocap_websocket_test-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:11:05.734766 zerocap_websocket_test-1.0.4/
--rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.4/LICENSE.txt
--rw-r--r--   0 gao        (501) staff       (20)     1227 2023-07-25 02:11:05.734459 zerocap_websocket_test-1.0.4/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-25 02:11:05.734855 zerocap_websocket_test-1.0.4/setup.cfg
--rw-r--r--   0 gao        (501) staff       (20)      799 2023-07-25 02:11:02.000000 zerocap_websocket_test-1.0.4/setup.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:11:05.731888 zerocap_websocket_test-1.0.4/zerocap_websocket_test/
--rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.4/zerocap_websocket_test/__init__.py
--rw-r--r--   0 gao        (501) staff       (20)     3259 2023-07-25 01:52:08.000000 zerocap_websocket_test-1.0.4/zerocap_websocket_test/main.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:11:05.733956 zerocap_websocket_test-1.0.4/zerocap_websocket_test.egg-info/
--rw-r--r--   0 gao        (501) staff       (20)     1227 2023-07-25 02:11:05.000000 zerocap_websocket_test-1.0.4/zerocap_websocket_test.egg-info/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)      315 2023-07-25 02:11:05.000000 zerocap_websocket_test-1.0.4/zerocap_websocket_test.egg-info/SOURCES.txt
--rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-25 02:11:05.000000 zerocap_websocket_test-1.0.4/zerocap_websocket_test.egg-info/dependency_links.txt
--rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-25 02:11:05.000000 zerocap_websocket_test-1.0.4/zerocap_websocket_test.egg-info/requires.txt
--rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-25 02:11:05.000000 zerocap_websocket_test-1.0.4/zerocap_websocket_test.egg-info/top_level.txt
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:12:44.722343 zerocap_websocket_test-1.0.5/
+-rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.5/LICENSE.txt
+-rw-r--r--   0 gao        (501) staff       (20)     1107 2023-07-25 02:12:44.721997 zerocap_websocket_test-1.0.5/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-25 02:12:44.722443 zerocap_websocket_test-1.0.5/setup.cfg
+-rw-r--r--   0 gao        (501) staff       (20)      799 2023-07-25 02:12:37.000000 zerocap_websocket_test-1.0.5/setup.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:12:44.718724 zerocap_websocket_test-1.0.5/zerocap_websocket_test/
+-rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test/__init__.py
+-rw-r--r--   0 gao        (501) staff       (20)     3259 2023-07-25 01:52:08.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test/main.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:12:44.721542 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/
+-rw-r--r--   0 gao        (501) staff       (20)     1107 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      315 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/SOURCES.txt
+-rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/dependency_links.txt
+-rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/requires.txt
+-rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/top_level.txt
```

### Comparing `zerocap_websocket_test-1.0.4/LICENSE.txt` & `zerocap_websocket_test-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_websocket_test-1.0.4/PKG-INFO` & `zerocap_websocket_test-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap_websocket_test
-Version: 1.0.4
+Version: 1.0.5
 Summary: websocket_test
 Home-page: 
 Author: jiayu.gao
 Author-email: y18362683626@gmail.com
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -15,32 +15,27 @@
 
 # pip install zerocap-websocket-test -i https://www.pypi.org/simple/
 
 
 # demo:
 
 # from zerocap_websocket_test import ZerocapWebsocketTest
-# def run():
-#     # API key and secret required
-#     apiKey = "coinroutes"
-#     apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
-# 
-#     websocket = ZerocapWebsocketTest(apiKey, apiSecret)
-# 
-#     # Subscribe to Market data
-#     market_connect = websocket.get_market()
-# 
-#     # Subscription order updates and transaction records
-#     orders_connect = websocket.get_orders()
-# 
-#     while True:
-#         # Get subscription messages
-#         message = websocket.get_message(market_connect)
-# 
-#         print(f"Receiving message from server: \n{message}")
-#         if not message:
-#             print("Connection close")
-#             break
-# 
-# 
-# if __name__ == "__main__":
-#     run()
+# # API key and secret required
+# apiKey = "coinroutes"
+# apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
+# 
+# websocket = ZerocapWebsocketTest(apiKey, apiSecret)
+# 
+# # Subscribe to Market data
+# market_connect = websocket.get_market()
+# 
+# # Subscription order updates and transaction records
+# orders_connect = websocket.get_orders()
+# 
+# while True:
+#     # Get subscription messages
+#     message = websocket.get_message(market_connect)
+# 
+#     print(f"Receiving message from server: \n{message}")
+#     if not message:
+#         print("Connection close")
+#         break
```

### Comparing `zerocap_websocket_test-1.0.4/setup.py` & `zerocap_websocket_test-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
 setup(name='zerocap_websocket_test',  # 包名
-      version='1.0.4',  # 版本号
+      version='1.0.5',  # 版本号
       description='websocket_test',
       long_description=long_description,
       author='jiayu.gao',
       author_email='y18362683626@gmail.com',
       url='',
       install_requires=REQUIRED,
       license='BSD License',
```

### Comparing `zerocap_websocket_test-1.0.4/zerocap_websocket_test/main.py` & `zerocap_websocket_test-1.0.5/zerocap_websocket_test/main.py`

 * *Files identical despite different names*

### Comparing `zerocap_websocket_test-1.0.4/zerocap_websocket_test.egg-info/PKG-INFO` & `zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap-websocket-test
-Version: 1.0.4
+Version: 1.0.5
 Summary: websocket_test
 Home-page: 
 Author: jiayu.gao
 Author-email: y18362683626@gmail.com
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -15,32 +15,27 @@
 
 # pip install zerocap-websocket-test -i https://www.pypi.org/simple/
 
 
 # demo:
 
 # from zerocap_websocket_test import ZerocapWebsocketTest
-# def run():
-#     # API key and secret required
-#     apiKey = "coinroutes"
-#     apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
-# 
-#     websocket = ZerocapWebsocketTest(apiKey, apiSecret)
-# 
-#     # Subscribe to Market data
-#     market_connect = websocket.get_market()
-# 
-#     # Subscription order updates and transaction records
-#     orders_connect = websocket.get_orders()
-# 
-#     while True:
-#         # Get subscription messages
-#         message = websocket.get_message(market_connect)
-# 
-#         print(f"Receiving message from server: \n{message}")
-#         if not message:
-#             print("Connection close")
-#             break
-# 
-# 
-# if __name__ == "__main__":
-#     run()
+# # API key and secret required
+# apiKey = "coinroutes"
+# apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
+# 
+# websocket = ZerocapWebsocketTest(apiKey, apiSecret)
+# 
+# # Subscribe to Market data
+# market_connect = websocket.get_market()
+# 
+# # Subscription order updates and transaction records
+# orders_connect = websocket.get_orders()
+# 
+# while True:
+#     # Get subscription messages
+#     message = websocket.get_message(market_connect)
+# 
+#     print(f"Receiving message from server: \n{message}")
+#     if not message:
+#         print("Connection close")
+#         break
```

