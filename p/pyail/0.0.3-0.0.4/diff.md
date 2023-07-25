# Comparing `tmp/pyail-0.0.3.tar.gz` & `tmp/pyail-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyail-0.0.3.tar", last modified: Wed Sep 14 07:51:11 2022, max compression
+gzip compressed data, was "pyail-0.0.4.tar", max compression
```

## Comparing `pyail-0.0.3.tar` & `pyail-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1517 2020-05-27 21:16:27.673125 pyail-0.0.3/LICENSE
--rw-r--r--   0        0        0      955 2021-04-19 14:29:11.953820 pyail-0.0.3/README.md
--rw-r--r--   0        0        0      921 2021-08-13 14:28:10.064995 pyail-0.0.3/pyail/__init__.py
--rw-r--r--   0        0        0     8255 2022-09-14 07:42:01.498624 pyail-0.0.3/pyail/api.py
--rw-r--r--   0        0        0      725 2021-08-13 14:07:15.294509 pyail-0.0.3/pyail/core.py
--rw-r--r--   0        0        0      539 2020-05-27 09:07:24.758326 pyail-0.0.3/pyail/exceptions.py
--rw-r--r--   0        0        0      426 2022-09-14 07:48:38.960168 pyail-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1631 2022-09-14 07:51:11.097616 pyail-0.0.3/setup.py
--rw-r--r--   0        0        0     1582 2022-09-14 07:51:11.097863 pyail-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1517 2020-05-27 21:16:27.000000 pyail-0.0.4/LICENSE
+-rw-r--r--   0        0        0      955 2021-04-19 14:29:11.000000 pyail-0.0.4/README.md
+-rw-r--r--   0        0        0      921 2021-08-13 14:28:10.000000 pyail-0.0.4/pyail/__init__.py
+-rw-r--r--   0        0        0     8730 2023-07-25 13:11:15.390972 pyail-0.0.4/pyail/api.py
+-rw-r--r--   0        0        0      725 2021-08-13 14:07:15.000000 pyail-0.0.4/pyail/core.py
+-rw-r--r--   0        0        0      539 2020-05-27 09:07:24.000000 pyail-0.0.4/pyail/exceptions.py
+-rw-r--r--   0        0        0      426 2023-07-25 13:40:01.459644 pyail-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 pyail-0.0.4/PKG-INFO
```

### Comparing `pyail-0.0.3/LICENSE` & `pyail-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyail-0.0.3/README.md` & `pyail-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyail-0.0.3/pyail/__init__.py` & `pyail-0.0.4/pyail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyail-0.0.3/pyail/api.py` & `pyail-0.0.4/pyail/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,20 +86,28 @@
         response = self._prepare_request('POST', f'api/{self.api_version}/import/json/item', data=dict_to_send)
         return self._check_json_response(response)
 
     # feed json file  -------------------
 
     # # TODO: return task uuid + add check status
     # Crawler #
-    def crawl_url(self, url, har=False, screenshot=False, depth_limit=1):
+    def crawl_url(self, url, har=False, screenshot=False, depth_limit=1, frequency=None, cookiejar=None, proxy='force_tor'):  # TODO frequency + cookiejar + proxy
         dict_to_send = {}
         dict_to_send['url'] = url
         dict_to_send['har'] = har
         dict_to_send['screenshot'] = screenshot
         dict_to_send['depth_limit'] = int(depth_limit)
+        if cookiejar:
+            dict_to_send['cookiejar'] = cookiejar
+        # can be set to 'web', 'onion', 'tor' or 'force_tor'
+        if proxy:
+            dict_to_send['proxy'] = proxy
+        # 'monthly', 'weekly', 'daily', 'hourly' or a dict {'minutes': 0, 'hours':0, 'days': 0, 'weeks': 0, 'months': 0}
+        if frequency:
+            dict_to_send['frequency'] = frequency
         response = self._prepare_request('POST', f'api/{self.api_version}/add/crawler/task', data=dict_to_send)
         return self._check_json_response(response)
 
     ## -- END Feed AIL -- ##
```

### Comparing `pyail-0.0.3/pyail/core.py` & `pyail-0.0.4/pyail/core.py`

 * *Files identical despite different names*

### Comparing `pyail-0.0.3/pyail/exceptions.py` & `pyail-0.0.4/pyail/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyail-0.0.3/PKG-INFO` & `pyail-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: pyail
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Home-page: https://github.com/ail-project/PyAIL
 License: BSD-2-Clause
 Author: Aurelien Thirion (terrtia)
 Author-email: aurelien.thirion@circl.lu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Project-URL: Repository, https://github.com/ail-project/PyAIL
 Description-Content-Type: text/markdown
 
 PyAIL
 ======
```

