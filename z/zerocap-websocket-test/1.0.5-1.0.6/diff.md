# Comparing `tmp/zerocap_websocket_test-1.0.5.tar.gz` & `tmp/zerocap_websocket_test-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocap_websocket_test-1.0.5.tar", last modified: Tue Jul 25 02:12:44 2023, max compression
+gzip compressed data, was "zerocap_websocket_test-1.0.6.tar", last modified: Tue Jul 25 02:22:02 2023, max compression
```

## Comparing `zerocap_websocket_test-1.0.5.tar` & `zerocap_websocket_test-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:12:44.722343 zerocap_websocket_test-1.0.5/
--rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.5/LICENSE.txt
--rw-r--r--   0 gao        (501) staff       (20)     1107 2023-07-25 02:12:44.721997 zerocap_websocket_test-1.0.5/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-25 02:12:44.722443 zerocap_websocket_test-1.0.5/setup.cfg
--rw-r--r--   0 gao        (501) staff       (20)      799 2023-07-25 02:12:37.000000 zerocap_websocket_test-1.0.5/setup.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:12:44.718724 zerocap_websocket_test-1.0.5/zerocap_websocket_test/
--rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test/__init__.py
--rw-r--r--   0 gao        (501) staff       (20)     3259 2023-07-25 01:52:08.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test/main.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:12:44.721542 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/
--rw-r--r--   0 gao        (501) staff       (20)     1107 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)      315 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/SOURCES.txt
--rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/dependency_links.txt
--rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/requires.txt
--rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-25 02:12:44.000000 zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/top_level.txt
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:22:02.544841 zerocap_websocket_test-1.0.6/
+-rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.6/LICENSE.txt
+-rw-r--r--   0 gao        (501) staff       (20)     1115 2023-07-25 02:22:02.544187 zerocap_websocket_test-1.0.6/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      727 2023-07-25 02:20:45.000000 zerocap_websocket_test-1.0.6/README.md
+-rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-25 02:22:02.545039 zerocap_websocket_test-1.0.6/setup.cfg
+-rw-r--r--   0 gao        (501) staff       (20)      799 2023-07-25 02:21:48.000000 zerocap_websocket_test-1.0.6/setup.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:22:02.540180 zerocap_websocket_test-1.0.6/zerocap_websocket_test/
+-rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.6/zerocap_websocket_test/__init__.py
+-rw-r--r--   0 gao        (501) staff       (20)     3259 2023-07-25 01:52:08.000000 zerocap_websocket_test-1.0.6/zerocap_websocket_test/main.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:22:02.543470 zerocap_websocket_test-1.0.6/zerocap_websocket_test.egg-info/
+-rw-r--r--   0 gao        (501) staff       (20)     1115 2023-07-25 02:22:02.000000 zerocap_websocket_test-1.0.6/zerocap_websocket_test.egg-info/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      325 2023-07-25 02:22:02.000000 zerocap_websocket_test-1.0.6/zerocap_websocket_test.egg-info/SOURCES.txt
+-rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-25 02:22:02.000000 zerocap_websocket_test-1.0.6/zerocap_websocket_test.egg-info/dependency_links.txt
+-rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-25 02:22:02.000000 zerocap_websocket_test-1.0.6/zerocap_websocket_test.egg-info/requires.txt
+-rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-25 02:22:02.000000 zerocap_websocket_test-1.0.6/zerocap_websocket_test.egg-info/top_level.txt
```

### Comparing `zerocap_websocket_test-1.0.5/LICENSE.txt` & `zerocap_websocket_test-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_websocket_test-1.0.5/PKG-INFO` & `zerocap_websocket_test-1.0.6/zerocap_websocket_test.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zerocap_websocket_test
-Version: 1.0.5
+Name: zerocap-websocket-test
+Version: 1.0.6
 Summary: websocket_test
 Home-page: 
 Author: jiayu.gao
 Author-email: y18362683626@gmail.com
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 License-File: LICENSE.txt
 
 # pip install zerocap-websocket-test -i https://www.pypi.org/simple/
 
 
 # demo:
 
+```
 # from zerocap_websocket_test import ZerocapWebsocketTest
 # # API key and secret required
 # apiKey = "coinroutes"
 # apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
 # 
 # websocket = ZerocapWebsocketTest(apiKey, apiSecret)
 # 
@@ -35,7 +36,8 @@
 #     # Get subscription messages
 #     message = websocket.get_message(market_connect)
 # 
 #     print(f"Receiving message from server: \n{message}")
 #     if not message:
 #         print("Connection close")
 #         break
+```
```

### Comparing `zerocap_websocket_test-1.0.5/setup.py` & `zerocap_websocket_test-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
 setup(name='zerocap_websocket_test',  # 包名
-      version='1.0.5',  # 版本号
+      version='1.0.6',  # 版本号
       description='websocket_test',
       long_description=long_description,
       author='jiayu.gao',
       author_email='y18362683626@gmail.com',
       url='',
       install_requires=REQUIRED,
       license='BSD License',
```

### Comparing `zerocap_websocket_test-1.0.5/zerocap_websocket_test/main.py` & `zerocap_websocket_test-1.0.6/zerocap_websocket_test/main.py`

 * *Files identical despite different names*

### Comparing `zerocap_websocket_test-1.0.5/zerocap_websocket_test.egg-info/PKG-INFO` & `zerocap_websocket_test-1.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zerocap-websocket-test
-Version: 1.0.5
+Name: zerocap_websocket_test
+Version: 1.0.6
 Summary: websocket_test
 Home-page: 
 Author: jiayu.gao
 Author-email: y18362683626@gmail.com
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 License-File: LICENSE.txt
 
 # pip install zerocap-websocket-test -i https://www.pypi.org/simple/
 
 
 # demo:
 
+```
 # from zerocap_websocket_test import ZerocapWebsocketTest
 # # API key and secret required
 # apiKey = "coinroutes"
 # apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
 # 
 # websocket = ZerocapWebsocketTest(apiKey, apiSecret)
 # 
@@ -35,7 +36,8 @@
 #     # Get subscription messages
 #     message = websocket.get_message(market_connect)
 # 
 #     print(f"Receiving message from server: \n{message}")
 #     if not message:
 #         print("Connection close")
 #         break
+```
```

