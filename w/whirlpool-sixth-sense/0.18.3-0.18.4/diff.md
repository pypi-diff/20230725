# Comparing `tmp/whirlpool_sixth_sense-0.18.3.tar.gz` & `tmp/whirlpool_sixth_sense-0.18.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whirlpool_sixth_sense-0.18.3.tar", last modified: Sat Apr 22 00:35:51 2023, max compression
+gzip compressed data, was "whirlpool_sixth_sense-0.18.4.tar", last modified: Tue Jul 25 21:17:56 2023, max compression
```

## Comparing `whirlpool_sixth_sense-0.18.3.tar` & `whirlpool_sixth_sense-0.18.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:51.134040 whirlpool_sixth_sense-0.18.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-22 00:35:51.134040 whirlpool_sixth_sense-0.18.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:35:51.134040 whirlpool_sixth_sense-0.18.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:51.130040 whirlpool_sixth_sense-0.18.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/tests/test_aircon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    86676 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/tests/test_oven.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:51.130040 whirlpool_sixth_sense-0.18.3/whirlpool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/aircon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/appliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/appliancesmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/backendselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/eventsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/oven.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-22 00:35:29.000000 whirlpool_sixth_sense-0.18.3/whirlpool/washerdryer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:35:51.134040 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 00:35:51.000000 whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:17:56.303775 whirlpool_sixth_sense-0.18.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-25 21:17:56.303775 whirlpool_sixth_sense-0.18.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:17:56.303775 whirlpool_sixth_sense-0.18.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:17:56.303775 whirlpool_sixth_sense-0.18.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/tests/test_aircon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86676 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/tests/test_oven.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:17:56.303775 whirlpool_sixth_sense-0.18.4/whirlpool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/aircon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/appliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/appliancesmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/backendselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/eventsocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/oven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-25 21:17:42.000000 whirlpool_sixth_sense-0.18.4/whirlpool/washerdryer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:17:56.303775 whirlpool_sixth_sense-0.18.4/whirlpool_sixth_sense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-25 21:17:56.000000 whirlpool_sixth_sense-0.18.4/whirlpool_sixth_sense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-25 21:17:56.000000 whirlpool_sixth_sense-0.18.4/whirlpool_sixth_sense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:17:56.000000 whirlpool_sixth_sense-0.18.4/whirlpool_sixth_sense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 21:17:56.000000 whirlpool_sixth_sense-0.18.4/whirlpool_sixth_sense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 21:17:56.000000 whirlpool_sixth_sense-0.18.4/whirlpool_sixth_sense.egg-info/top_level.txt
```

### Comparing `whirlpool_sixth_sense-0.18.3/LICENSE` & `whirlpool_sixth_sense-0.18.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/PKG-INFO` & `whirlpool_sixth_sense-0.18.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whirlpool_sixth_sense
-Version: 0.18.3
+Version: 0.18.4
 Summary: Unofficial API for Whirlpool's 6th Sense appliances
 Author-email: Abílio Costa <amfcalt@gmail.com>
 Project-URL: Homepage, https://github.com/abmantis/whirlpool-sixth-sense/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `whirlpool_sixth_sense-0.18.3/README.md` & `whirlpool_sixth_sense-0.18.4/README.md`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/pyproject.toml` & `whirlpool_sixth_sense-0.18.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whirlpool_sixth_sense"
-version = "0.18.3"
+version = "0.18.4"
 authors = [{name = "Abílio Costa", email = "amfcalt@gmail.com"}]
 description = "Unofficial API for Whirlpool's 6th Sense appliances"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `whirlpool_sixth_sense-0.18.3/tests/test_aircon.py` & `whirlpool_sixth_sense-0.18.4/tests/test_aircon.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/tests/test_auth.py` & `whirlpool_sixth_sense-0.18.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/tests/test_oven.py` & `whirlpool_sixth_sense-0.18.4/tests/test_oven.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool/aircon.py` & `whirlpool_sixth_sense-0.18.4/whirlpool/aircon.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool/appliance.py` & `whirlpool_sixth_sense-0.18.4/whirlpool/appliance.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 
         uri = f"{self._backend_selector.base_url}/api/v1/appliance/{self._said}"
         for n in range(REQUEST_RETRY_COUNT):
             async with async_timeout.timeout(30):
                 async with self._session.get(uri, headers=self._create_headers()) as r:
                     if r.status == 200:
                         self._data_dict = json.loads(await r.text())
+                        for callback in self._attr_changed:
+                            callback()
                         return True
                     elif r.status == 401:
                         LOGGER.error(
                             "Fetching data failed (%s). Doing reauth", r.status
                         )
                         await self._auth.do_auth()
                     else:
```

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool/appliancesmanager.py` & `whirlpool_sixth_sense-0.18.4/whirlpool/appliancesmanager.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool/auth.py` & `whirlpool_sixth_sense-0.18.4/whirlpool/auth.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool/backendselector.py` & `whirlpool_sixth_sense-0.18.4/whirlpool/backendselector.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool/eventsocket.py` & `whirlpool_sixth_sense-0.18.4/whirlpool/eventsocket.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool/oven.py` & `whirlpool_sixth_sense-0.18.4/whirlpool/oven.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool/washerdryer.py` & `whirlpool_sixth_sense-0.18.4/whirlpool/washerdryer.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/PKG-INFO` & `whirlpool_sixth_sense-0.18.4/whirlpool_sixth_sense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whirlpool-sixth-sense
-Version: 0.18.3
+Version: 0.18.4
 Summary: Unofficial API for Whirlpool's 6th Sense appliances
 Author-email: Abílio Costa <amfcalt@gmail.com>
 Project-URL: Homepage, https://github.com/abmantis/whirlpool-sixth-sense/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `whirlpool_sixth_sense-0.18.3/whirlpool_sixth_sense.egg-info/SOURCES.txt` & `whirlpool_sixth_sense-0.18.4/whirlpool_sixth_sense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

