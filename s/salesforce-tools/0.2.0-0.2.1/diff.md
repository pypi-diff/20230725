# Comparing `tmp/salesforce_tools-0.2.0.tar.gz` & `tmp/salesforce_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce_tools-0.2.0.tar", max compression
+gzip compressed data, was "salesforce_tools-0.2.1.tar", max compression
```

## Comparing `salesforce_tools-0.2.0.tar` & `salesforce_tools-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      838 2023-07-18 18:11:24.446289 salesforce_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      548 2023-02-19 15:59:55.189773 salesforce_tools-0.2.0/salesforce_tools/__init__.py
--rw-r--r--   0        0        0      207 2022-12-03 15:34:19.193841 salesforce_tools-0.2.0/salesforce_tools/async_sf/__init__.py
--rw-r--r--   0        0        0     3862 2023-06-23 19:31:44.774633 salesforce_tools-0.2.0/salesforce_tools/async_sf/client.py
--rw-r--r--   0        0        0     3227 2023-02-18 15:51:24.662020 salesforce_tools-0.2.0/salesforce_tools/async_sf/metadata.py
--rw-r--r--   0        0        0     7544 2022-12-01 15:42:09.307115 salesforce_tools-0.2.0/salesforce_tools/auth.py
--rw-r--r--   0        0        0     6263 2023-06-29 17:05:59.004227 salesforce_tools-0.2.0/salesforce_tools/bulk.py
--rw-r--r--   0        0        0     5882 2023-06-29 17:05:16.303395 salesforce_tools-0.2.0/salesforce_tools/bulk_models.py
--rw-r--r--   0        0        0     1612 2022-11-12 16:32:21.055825 salesforce_tools-0.2.0/salesforce_tools/oauth_server.py
--rw-r--r--   0        0        0    82405 2023-06-29 17:06:14.252247 salesforce_tools-0.2.0/salesforce_tools/salesforce.py
--rw-r--r--   0        0        0     1879 2023-06-25 06:39:25.160760 salesforce_tools-0.2.0/salesforce_tools/util.py
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 salesforce_tools-0.2.0/setup.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 salesforce_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      838 2023-07-24 23:24:06.928110 salesforce_tools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      548 2023-02-19 15:59:55.189773 salesforce_tools-0.2.1/salesforce_tools/__init__.py
+-rw-r--r--   0        0        0      207 2022-12-03 15:34:19.193841 salesforce_tools-0.2.1/salesforce_tools/async_sf/__init__.py
+-rw-r--r--   0        0        0     3862 2023-06-23 19:31:44.774633 salesforce_tools-0.2.1/salesforce_tools/async_sf/client.py
+-rw-r--r--   0        0        0     3259 2023-07-24 23:23:48.279130 salesforce_tools-0.2.1/salesforce_tools/async_sf/metadata.py
+-rw-r--r--   0        0        0     7544 2022-12-01 15:42:09.307115 salesforce_tools-0.2.1/salesforce_tools/auth.py
+-rw-r--r--   0        0        0     6263 2023-06-29 17:05:59.004227 salesforce_tools-0.2.1/salesforce_tools/bulk.py
+-rw-r--r--   0        0        0     5882 2023-06-29 17:05:16.303395 salesforce_tools-0.2.1/salesforce_tools/bulk_models.py
+-rw-r--r--   0        0        0     1612 2022-11-12 16:32:21.055825 salesforce_tools-0.2.1/salesforce_tools/oauth_server.py
+-rw-r--r--   0        0        0    82405 2023-06-29 17:06:14.252247 salesforce_tools-0.2.1/salesforce_tools/salesforce.py
+-rw-r--r--   0        0        0     1879 2023-06-25 06:39:25.160760 salesforce_tools-0.2.1/salesforce_tools/util.py
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 salesforce_tools-0.2.1/setup.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 salesforce_tools-0.2.1/PKG-INFO
```

### Comparing `salesforce_tools-0.2.0/pyproject.toml` & `salesforce_tools-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salesforce-tools"
-version = "0.2.0"
+version = "0.2.1"
 description = "Salesforce API tools"
 authors = ["David Manuel <david@dcmanjr.com>"]
 license = "MIT"
 homepage = "https://github.com/dacmanj/salesforce-tools"
 repository = "https://github.com/dacmanj/salesforce-tools"
 
 [tool.poetry.dependencies]
```

### Comparing `salesforce_tools-0.2.0/salesforce_tools/__init__.py` & `salesforce_tools-0.2.1/salesforce_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce_tools-0.2.0/salesforce_tools/async_sf/client.py` & `salesforce_tools-0.2.1/salesforce_tools/async_sf/client.py`

 * *Files identical despite different names*

### Comparing `salesforce_tools-0.2.0/salesforce_tools/async_sf/metadata.py` & `salesforce_tools-0.2.1/salesforce_tools/async_sf/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
         self.client = client
         self._cache_sobject = {}
         self._cache_sobjects_list = []
         self.cache_file = cache_file
         if self.cache_file:
             self.load_cache(self.cache_file)
 
-    async def get_sobject_describe(self, obj, cache=True):
+    async def get_sobject_describe(self, obj, cache=True, timeout=30):
         if not cache or not self._cache_sobject.get(obj):
-            self._cache_sobject[obj] = (await self.client.get(f'sobjects/{obj}/describe', timeout=10.0)).json()
+            self._cache_sobject[obj] = (await self.client.get(f'sobjects/{obj}/describe', timeout=timeout)).json()
         return self._cache_sobject.get(obj)
 
     async def get_picklist_values(self, obj, field):
         obj_md = await self.get_sobject_describe(obj)
         return [f for f in obj_md['fields'] if f['name'] == field][0]['picklistValues']
 
     async def get_permissionable_fields(self, normalize=True):
@@ -29,17 +29,17 @@
                 sf_obj, fld = f.split('.')
                 if not permissionable_fields.get(sf_obj):
                     permissionable_fields[sf_obj] = []
                 permissionable_fields[sf_obj].append(fld)
             return permissionable_fields
         return pv
 
-    async def get_all_sobjects(self, cache=True):
+    async def get_all_sobjects(self, cache=True, timeout=30.0):
         if not cache or not self._cache_sobjects_list:
-            self._cache_sobjects_list = (await self.client.get("sobjects", timeout=10.0)).json()['sobjects']
+            self._cache_sobjects_list = (await self.client.get("sobjects", timeout=timeout)).json()['sobjects']
         return self._cache_sobjects_list
 
     async def get_all_sobject_request_coroutines(self, unfiltered=True, cache=True):
         objects_to_fetch = await self.get_all_sobjects(cache)
         tasks = []
         if not unfiltered:
             objects_to_fetch = [o for o in objects_to_fetch if
```

### Comparing `salesforce_tools-0.2.0/salesforce_tools/auth.py` & `salesforce_tools-0.2.1/salesforce_tools/auth.py`

 * *Files identical despite different names*

### Comparing `salesforce_tools-0.2.0/salesforce_tools/bulk.py` & `salesforce_tools-0.2.1/salesforce_tools/bulk.py`

 * *Files identical despite different names*

### Comparing `salesforce_tools-0.2.0/salesforce_tools/bulk_models.py` & `salesforce_tools-0.2.1/salesforce_tools/bulk_models.py`

 * *Files identical despite different names*

### Comparing `salesforce_tools-0.2.0/salesforce_tools/oauth_server.py` & `salesforce_tools-0.2.1/salesforce_tools/oauth_server.py`

 * *Files identical despite different names*

### Comparing `salesforce_tools-0.2.0/salesforce_tools/salesforce.py` & `salesforce_tools-0.2.1/salesforce_tools/salesforce.py`

 * *Files identical despite different names*

### Comparing `salesforce_tools-0.2.0/salesforce_tools/util.py` & `salesforce_tools-0.2.1/salesforce_tools/util.py`

 * *Files identical despite different names*

### Comparing `salesforce_tools-0.2.0/setup.py` & `salesforce_tools-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'salesforce-tools',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Salesforce API tools',
     'long_description': 'None',
     'author': 'David Manuel',
     'author_email': 'david@dcmanjr.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dacmanj/salesforce-tools',
```

### Comparing `salesforce_tools-0.2.0/PKG-INFO` & `salesforce_tools-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Salesforce API tools
 Home-page: https://github.com/dacmanj/salesforce-tools
 License: MIT
 Author: David Manuel
 Author-email: david@dcmanjr.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

