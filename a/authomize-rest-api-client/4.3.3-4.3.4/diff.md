# Comparing `tmp/authomize-rest-api-client-4.3.3.tar.gz` & `tmp/authomize-rest-api-client-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.3.3.tar", last modified: Mon Jul 24 16:47:56 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.4.tar", last modified: Tue Jul 25 08:36:04 2023, max compression
```

## Comparing `authomize-rest-api-client-4.3.3.tar` & `authomize-rest-api-client-4.3.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2846 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84645 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49598 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200535 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115884 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1117 2023-07-24 16:47:42.000000 authomize-rest-api-client-4.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84645 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49495 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   200535 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115884 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-25 08:35:49.000000 authomize-rest-api-client-4.3.4/setup.py
```

### Comparing `authomize-rest-api-client-4.3.3/LICENSE.txt` & `authomize-rest-api-client-4.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/README.md` & `authomize-rest-api-client-4.3.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -75,8 +75,10 @@
 3. Replace the content of `authomize/rest_api_client/generated/external_rest_api/schemas.py` from the newly created `__init__.py`  
 ```
  mv authomize/rest_api_client/generated/external_rest_api/__init__.py authomize/rest_api_client/generated/external_rest_api/schemas.py
  touch authomize/rest_api_client/generated/external_rest_api/__init__.py
 ```   
 4. Add the missing schemas from the other file to the end of `schemas.py`
 5. Fix the imports / errors in `schemas.py`
+  for example `from .field_class__authomize.external_rest_api.app.routes_schema import inventory`  
+  should be removed , and all references to inventory updated in the code
 6. Remove all the newly created files (leave only `schemas.py`)
```

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Extra, Field, conint, constr
 
-from .field_class__authomize.external_rest_api.app.routes_schema import inventory
-
 
 class AccessByType(Enum):
     account = 'account'
     grouping = 'grouping'
 
 
 class AccessToType(Enum):
@@ -1192,15 +1190,15 @@
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
     expand: Optional[List[AssetExpansion]] = Field(
         default=None, description='Expand fields (to show additional information)'
     )
-    filter: Optional[inventory.SearchAssetsFilterBody] = Field(
+    filter: Optional[SearchAssetsFilterBody] = Field(
         default=None, description='Search Assets Filter', title='Filter'
     )
 
 
 class SearchCampaignPermissionsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -1247,15 +1245,15 @@
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
     expand: Optional[List[GroupExpansion]] = Field(
         default=None, description='Expand fields (to show additional information)'
     )
-    filter: Optional[inventory.SearchGroupsFilterBody] = Field(
+    filter: Optional[SearchGroupsFilterBody] = Field(
         default=None, description='Search Groups Filter', title='Filter'
     )
 
 
 class SearchIdentitiesRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
```

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.3/setup.py` & `authomize-rest-api-client-4.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.3.3',
+        version='4.3.4',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

