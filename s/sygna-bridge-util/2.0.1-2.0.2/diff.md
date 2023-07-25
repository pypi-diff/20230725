# Comparing `tmp/sygna-bridge-util-2.0.1.tar.gz` & `tmp/sygna-bridge-util-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sygna-bridge-util-2.0.1.tar", last modified: Wed Jul 21 03:17:24 2021, max compression
+gzip compressed data, was "dist/sygna-bridge-util-2.0.2.tar", last modified: Tue Jul 25 08:28:37 2023, max compression
```

## Comparing `sygna-bridge-util-2.0.1.tar` & `sygna-bridge-util-2.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9774 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7323 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      361 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/api/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9317 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/config/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/config/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/config/permissionstatus.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/config/rejectcode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)      716 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/ecies.py
--rw-r--r--   0 runner    (1001) docker     (121)     5703 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/sign.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/validator/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      320 2021-07-21 03:16:33.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util/validator/validatedata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9774 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      869 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-07-21 03:17:24.000000 sygna-bridge-util-2.0.1/src/sygna_bridge_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/config/permissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/config/rejectcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/ecies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-25 08:27:46.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util/validator/validatedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 08:28:37.000000 sygna-bridge-util-2.0.2/src/sygna_bridge_util.egg-info/top_level.txt
```

### Comparing `sygna-bridge-util-2.0.1/PKG-INFO` & `sygna-bridge-util-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sygna-bridge-util
-Version: 2.0.1
+Version: 2.0.2
 Summary: This is a Python library to help you build servers/services within Sygna Bridge Ecosystem.
 Home-page: https://github.com/CoolBitX-Technology/sygna-bridge-util-py
 Author: kunming.liu
 Author-email: kunming@coolbitx.com
 License: MIT
 Description: # 
         # Python Sygna Bridge Util
```

### Comparing `sygna-bridge-util-2.0.1/README.md` & `sygna-bridge-util-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sygna-bridge-util-2.0.1/setup.py` & `sygna-bridge-util-2.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     if '-i https://pypi.org/simple' in requirements_list:
         requirements_list.remove('-i https://pypi.org/simple')
     return requirements_list
 
 
 setup(
     name='sygna-bridge-util',
-    version='2.0.1',
+    version='2.0.2',
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=get_requirements(),
     tests_require=['pytest'],
     url='https://github.com/CoolBitX-Technology/sygna-bridge-util-py',
     license='MIT',
     author='kunming.liu',
```

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util/api/main.py` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util/api/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,30 +18,32 @@
 
         Args:
             url: str
 
         Returns:
             dict
         """
-        headers = {'x-api-key': self.api_key}
+        headers = {'x-api-key': self.api_key,
+                   'User-Agent': 'util-python/2.0.2'}
         response = requests.get(url, headers=headers, timeout=HTTP_TIMEOUT)
         return response.json()
 
     def post_sb(self, url: str, body: dict) -> dict:
         """HTTP Post request to Sygna Bridge
 
         Args:
             url: str
             body: dict
 
         Returns:
             dict
         """
         headers = {'Content-Type': 'application/json',
-                   'x-api-key': self.api_key}
+                   'x-api-key': self.api_key,
+                   'User-Agent': 'util-python/2.0.2'}
         response = requests.post(
             url,
             data=json.dumps(body),
             headers=headers,
             timeout=HTTP_TIMEOUT)
         return response.json()
```

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util/config/main.py` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util/config/main.py`

 * *Files identical despite different names*

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/__init__.py` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/ecies.py` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/ecies.py`

 * *Files identical despite different names*

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/main.py` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/main.py`

 * *Files identical despite different names*

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/sign.py` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/sign.py`

 * *Files identical despite different names*

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/utils.py` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/utils.py`

 * *Files identical despite different names*

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util/crypto/verify.py` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util/crypto/verify.py`

 * *Files identical despite different names*

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util.egg-info/PKG-INFO` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sygna-bridge-util
-Version: 2.0.1
+Version: 2.0.2
 Summary: This is a Python library to help you build servers/services within Sygna Bridge Ecosystem.
 Home-page: https://github.com/CoolBitX-Technology/sygna-bridge-util-py
 Author: kunming.liu
 Author-email: kunming@coolbitx.com
 License: MIT
 Description: # 
         # Python Sygna Bridge Util
```

### Comparing `sygna-bridge-util-2.0.1/src/sygna_bridge_util.egg-info/SOURCES.txt` & `sygna-bridge-util-2.0.2/src/sygna_bridge_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

