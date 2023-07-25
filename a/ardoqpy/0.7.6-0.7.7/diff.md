# Comparing `tmp/ardoqpy-0.7.6.tar.gz` & `tmp/ardoqpy-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardoqpy-0.7.6.tar", last modified: Fri Mar 31 07:23:10 2023, max compression
+gzip compressed data, was "ardoqpy-0.7.7.tar", last modified: Tue Jul 25 19:28:59 2023, max compression
```

## Comparing `ardoqpy-0.7.6.tar` & `ardoqpy-0.7.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-03-31 07:23:10.375885 ardoqpy-0.7.6/
--rw-r--r--   0 jason      (501) staff       (20)     1119 2016-04-11 06:32:09.000000 ardoqpy-0.7.6/LICENSE.txt
--rw-r--r--   0 jason      (501) staff       (20)       57 2021-05-01 13:21:49.000000 ardoqpy-0.7.6/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     6174 2023-03-31 07:23:10.375948 ardoqpy-0.7.6/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     5110 2023-03-30 13:28:46.000000 ardoqpy-0.7.6/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-03-31 07:23:10.373455 ardoqpy-0.7.6/ardoqpy/
--rw-r--r--   0 jason      (501) staff       (20)       51 2021-05-11 18:42:19.000000 ardoqpy-0.7.6/ardoqpy/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)      304 2022-02-12 20:17:55.000000 ardoqpy-0.7.6/ardoqpy/ardoqpy.cfg
--rw-r--r--   0 jason      (501) staff       (20)    17032 2023-01-05 10:53:57.000000 ardoqpy-0.7.6/ardoqpy/ardoqpy.py
--rw-r--r--   0 jason      (501) staff       (20)    11264 2023-03-31 06:55:34.000000 ardoqpy-0.7.6/ardoqpy/ardoqpy_sync.py
--rw-r--r--   0 jason      (501) staff       (20)     1128 2022-08-10 09:44:52.000000 ardoqpy-0.7.6/ardoqpy/test_ardoqpy.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-03-31 07:23:10.375681 ardoqpy-0.7.6/ardoqpy.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     6174 2023-03-31 07:23:10.000000 ardoqpy-0.7.6/ardoqpy.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      313 2023-03-31 07:23:10.000000 ardoqpy-0.7.6/ardoqpy.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2023-03-31 07:23:10.000000 ardoqpy-0.7.6/ardoqpy.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       32 2023-03-31 07:23:10.000000 ardoqpy-0.7.6/ardoqpy.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        8 2023-03-31 07:23:10.000000 ardoqpy-0.7.6/ardoqpy.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       79 2023-03-31 07:23:10.376310 ardoqpy-0.7.6/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1862 2023-03-31 07:16:00.000000 ardoqpy-0.7.6/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-25 19:28:59.520706 ardoqpy-0.7.7/
+-rw-r--r--   0 jason      (501) staff       (20)     1119 2016-04-11 06:32:09.000000 ardoqpy-0.7.7/LICENSE.txt
+-rw-r--r--   0 jason      (501) staff       (20)       57 2021-05-01 13:21:49.000000 ardoqpy-0.7.7/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     6229 2023-07-25 19:28:59.520796 ardoqpy-0.7.7/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     5165 2023-07-25 19:20:25.000000 ardoqpy-0.7.7/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-25 19:28:59.518845 ardoqpy-0.7.7/ardoqpy/
+-rw-r--r--   0 jason      (501) staff       (20)       51 2021-05-11 18:42:19.000000 ardoqpy-0.7.7/ardoqpy/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)      304 2022-02-12 20:17:55.000000 ardoqpy-0.7.7/ardoqpy/ardoqpy.cfg
+-rw-r--r--   0 jason      (501) staff       (20)    17453 2023-07-25 19:11:58.000000 ardoqpy-0.7.7/ardoqpy/ardoqpy.py
+-rw-r--r--   0 jason      (501) staff       (20)    11264 2023-03-31 06:55:34.000000 ardoqpy-0.7.7/ardoqpy/ardoqpy_sync.py
+-rw-r--r--   0 jason      (501) staff       (20)     1128 2022-08-10 09:44:52.000000 ardoqpy-0.7.7/ardoqpy/test_ardoqpy.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-25 19:28:59.520491 ardoqpy-0.7.7/ardoqpy.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     6229 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      313 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       32 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        8 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       79 2023-07-25 19:28:59.521157 ardoqpy-0.7.7/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1862 2023-07-25 19:20:25.000000 ardoqpy-0.7.7/setup.py
```

### Comparing `ardoqpy-0.7.6/LICENSE.txt` & `ardoqpy-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ardoqpy-0.7.6/PKG-INFO` & `ardoqpy-0.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardoqpy
-Version: 0.7.6
+Version: 0.7.7
 Summary: A python REST API wrapper for Ardoq - https://ardoq.com.
 Home-page: https://github.com/jbaragry/ardoq-python-client
 Author: Jason Baragry
 Author-email: jason.baragry@gmail.com
 License: MIT
 Keywords: architecture ardoq REST API wrapper tool
 Classifier: Development Status :: 3 - Alpha
@@ -82,14 +82,16 @@
     - create
     - update
     - delete
 - tag
     - get by ID
     - get all for workspace
     - create
+    - update
+    - delete
 - model
     - get by ID
     - get all models and templates
     - print model to get IDs for component and reference types
     - find reference_type by name
     - find component_type by name
 - folder
@@ -142,14 +144,16 @@
     from ardoqpy import ArdoqClient
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN')
     # to use v2 API
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN', version='v2')
     ardoq.get_workspaces()
 
 ## Changelog
+- 202307
+  - added del and update tag
 - 202303
   - added audit log for support for components created, updated, deleted, and skipped due to cache_hit
 - 202211
   - added support for Ardoq v2 REST API. Only for the ArdoqClient (not SyncClient)
 - 202207
   - add find_reference_type to return reftype definition from the metamodel for a workspace 
   - add find_component_type to return comptype definition from the metamodel for a workspace. Checks full hierarchy
@@ -191,13 +195,13 @@
     - first version of the sync client
 
 - 20160402
     - Initial dev
     
 
 ## TODO
-- complete the full REST-API for fields and tags
+- complete the full REST-API for fields
 
 ## License
 The ardoq-python-client is licensed under the MIT License
 
 See LICENSE.md
```

### Comparing `ardoqpy-0.7.6/README.md` & `ardoqpy-0.7.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     - create
     - update
     - delete
 - tag
     - get by ID
     - get all for workspace
     - create
+    - update
+    - delete
 - model
     - get by ID
     - get all models and templates
     - print model to get IDs for component and reference types
     - find reference_type by name
     - find component_type by name
 - folder
@@ -116,14 +118,16 @@
     from ardoqpy import ArdoqClient
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN')
     # to use v2 API
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN', version='v2')
     ardoq.get_workspaces()
 
 ## Changelog
+- 202307
+  - added del and update tag
 - 202303
   - added audit log for support for components created, updated, deleted, and skipped due to cache_hit
 - 202211
   - added support for Ardoq v2 REST API. Only for the ArdoqClient (not SyncClient)
 - 202207
   - add find_reference_type to return reftype definition from the metamodel for a workspace 
   - add find_component_type to return comptype definition from the metamodel for a workspace. Checks full hierarchy
@@ -165,13 +169,13 @@
     - first version of the sync client
 
 - 20160402
     - Initial dev
     
 
 ## TODO
-- complete the full REST-API for fields and tags
+- complete the full REST-API for fields
 
 ## License
 The ardoq-python-client is licensed under the MIT License
 
 See LICENSE.md
```

### Comparing `ardoqpy-0.7.6/ardoqpy/ardoqpy.py` & `ardoqpy-0.7.7/ardoqpy/ardoqpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,14 +430,26 @@
             raise ArdoqClientException('must provide a workspace id and/or tag id')
         if tag_id is not None:
             tag = self._get('tag/' + tag_id)
         if ws_id is not None and tag_id is None:
             tag = self._get('tag/' + 'workspace/' + ws_id)
         return tag
 
+    def update_tag(self, tag_id=None, tag=None):
+        if tag_id is None or tag is None:
+            raise ArdoqClientException('must provide a tag id, and tag')
+        res = self._put('tag/' + tag_id, tag)
+        return res
+
+    def del_tag(self, tag_id=None):
+        if tag_id is None:
+            raise ArdoqClientException('must provide a tag id')
+        res = self._delete('tag/' + tag_id)
+        return res
+
     def get_current_user(self):
         '''
 
         :return: information about the current user
         '''
         if self.version == 'v2':
             current_user = self._get('me/')
```

### Comparing `ardoqpy-0.7.6/ardoqpy/ardoqpy_sync.py` & `ardoqpy-0.7.7/ardoqpy/ardoqpy_sync.py`

 * *Files identical despite different names*

### Comparing `ardoqpy-0.7.6/ardoqpy/test_ardoqpy.py` & `ardoqpy-0.7.7/ardoqpy/test_ardoqpy.py`

 * *Files identical despite different names*

### Comparing `ardoqpy-0.7.6/ardoqpy.egg-info/PKG-INFO` & `ardoqpy-0.7.7/ardoqpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardoqpy
-Version: 0.7.6
+Version: 0.7.7
 Summary: A python REST API wrapper for Ardoq - https://ardoq.com.
 Home-page: https://github.com/jbaragry/ardoq-python-client
 Author: Jason Baragry
 Author-email: jason.baragry@gmail.com
 License: MIT
 Keywords: architecture ardoq REST API wrapper tool
 Classifier: Development Status :: 3 - Alpha
@@ -82,14 +82,16 @@
     - create
     - update
     - delete
 - tag
     - get by ID
     - get all for workspace
     - create
+    - update
+    - delete
 - model
     - get by ID
     - get all models and templates
     - print model to get IDs for component and reference types
     - find reference_type by name
     - find component_type by name
 - folder
@@ -142,14 +144,16 @@
     from ardoqpy import ArdoqClient
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN')
     # to use v2 API
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN', version='v2')
     ardoq.get_workspaces()
 
 ## Changelog
+- 202307
+  - added del and update tag
 - 202303
   - added audit log for support for components created, updated, deleted, and skipped due to cache_hit
 - 202211
   - added support for Ardoq v2 REST API. Only for the ArdoqClient (not SyncClient)
 - 202207
   - add find_reference_type to return reftype definition from the metamodel for a workspace 
   - add find_component_type to return comptype definition from the metamodel for a workspace. Checks full hierarchy
@@ -191,13 +195,13 @@
     - first version of the sync client
 
 - 20160402
     - Initial dev
     
 
 ## TODO
-- complete the full REST-API for fields and tags
+- complete the full REST-API for fields
 
 ## License
 The ardoq-python-client is licensed under the MIT License
 
 See LICENSE.md
```

### Comparing `ardoqpy-0.7.6/setup.py` & `ardoqpy-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from distutils.core import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ardoqpy',
-    version='0.7.6',
+    version='0.7.7',
     description='A python REST API wrapper for Ardoq - https://ardoq.com.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/jbaragry/ardoq-python-client',
     author='Jason Baragry',
     author_email='jason.baragry@gmail.com',
     license='MIT',
```

