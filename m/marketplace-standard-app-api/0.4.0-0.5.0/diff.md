# Comparing `tmp/marketplace-standard-app-api-0.4.0.tar.gz` & `tmp/marketplace_standard_app_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketplace-standard-app-api-0.4.0.tar", last modified: Wed Apr  5 09:31:07 2023, max compression
+gzip compressed data, was "marketplace_standard_app_api-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `marketplace-standard-app-api-0.4.0.tar` & `marketplace_standard_app_api-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      448 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/.flake8
--rw-r--r--   0        0        0     1713 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      964 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       43 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/.gitignore
--rw-r--r--   0        0        0     2001 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1078 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/LICENSE
--rw-r--r--   0        0        0     2779 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/README.md
--rw-r--r--   0        0        0      346 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/__init__.py
--rw-r--r--   0        0        0     1028 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/__main__.py
--rw-r--r--   0        0        0     1877 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/main.py
--rw-r--r--   0        0        0        0 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/__init__.py
--rw-r--r--   0        0        0      795 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/message_broker.py
--rw-r--r--   0        0        0      963 2023-04-05 09:30:59.177854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/object_storage.py
--rw-r--r--   0        0        0      763 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/system.py
--rw-r--r--   0        0        0     1773 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/transformation.py
--rw-r--r--   0        0        0        0 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/routers/__init__.py
--rw-r--r--   0        0        0      482 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/routers/frontend.py
--rw-r--r--   0        0        0    11140 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/routers/object_storage.py
--rw-r--r--   0        0        0     1071 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/routers/system.py
--rw-r--r--   0        0        0     3974 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/routers/transformation.py
--rw-r--r--   0        0        0      513 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/security.py
--rw-r--r--   0        0        0       22 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/version.py
--rw-r--r--   0        0        0    53939 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/openapi.json
--rw-r--r--   0        0        0     1426 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      601 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      375 2023-04-05 09:30:59.181854 marketplace-standard-app-api-0.4.0/tests/test_schema.py
--rw-r--r--   0        0        0     3520 1970-01-01 00:00:00.000000 marketplace-standard-app-api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      448 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/.flake8
+-rw-r--r--   0        0        0     1713 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      964 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       43 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2001 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1078 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2779 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/README.md
+-rw-r--r--   0        0        0      346 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/__init__.py
+-rw-r--r--   0        0        0     1028 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/__main__.py
+-rw-r--r--   0        0        0     1877 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/main.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/__init__.py
+-rw-r--r--   0        0        0      795 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/message_broker.py
+-rw-r--r--   0        0        0     1153 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/object_storage.py
+-rw-r--r--   0        0        0      763 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/system.py
+-rw-r--r--   0        0        0     1773 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/transformation.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/routers/__init__.py
+-rw-r--r--   0        0        0      482 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/routers/frontend.py
+-rw-r--r--   0        0        0    13001 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/routers/object_storage.py
+-rw-r--r--   0        0        0     1071 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/routers/system.py
+-rw-r--r--   0        0        0     3974 2023-07-25 12:58:30.758441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/routers/transformation.py
+-rw-r--r--   0        0        0      513 2023-07-25 12:58:30.762441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/security.py
+-rw-r--r--   0        0        0       22 2023-07-25 12:58:30.762441 marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/version.py
+-rw-r--r--   0        0        0    61381 2023-07-25 12:58:30.762441 marketplace_standard_app_api-0.5.0/openapi.json
+-rw-r--r--   0        0        0     1431 2023-07-25 12:58:30.762441 marketplace_standard_app_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      601 2023-07-25 12:58:30.762441 marketplace_standard_app_api-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      375 2023-07-25 12:58:30.762441 marketplace_standard_app_api-0.5.0/tests/test_schema.py
+-rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 marketplace_standard_app_api-0.5.0/PKG-INFO
```

### Comparing `marketplace-standard-app-api-0.4.0/.github/workflows/ci.yml` & `marketplace_standard_app_api-0.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/.github/workflows/release.yml` & `marketplace_standard_app_api-0.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/.pre-commit-config.yaml` & `marketplace_standard_app_api-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/LICENSE` & `marketplace_standard_app_api-0.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Materials MarketPlace
+Copyright (c) 2023 Materials MarketPlace
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `marketplace-standard-app-api-0.4.0/README.md` & `marketplace_standard_app_api-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # README
 
 ## About
 
 This repository contains the specification of the Materials MarketPlace Standard App API.
 The API is used as basis for the interaction between apps on the Materials MarketPlace platform.
 
-This repository contains the API version: 0.4.0.
+This repository contains the API version: 0.5.0.
 
 ## Authors
 
 - Simon Adorf (simon.adorf@epfl.ch)
 - MarketPlace consortium partners
 
 ## Specification
```

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/__main__.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/__main__.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/main.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/main.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/message_broker.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/message_broker.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/object_storage.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/object_storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,41 +5,49 @@
 
 
 class CollectionName(ConstrainedStr):
     min_length = 1
     max_length = 255
 
 
-class CollectionListItemModel(BaseModel):
-    count: int
-    bytes: int
+class CollectionModel(BaseModel):
+    count: Optional[int]
+    bytes: Optional[int]
+    id: Optional[str]
     name: CollectionName
     last_modified: Optional[datetime]
 
 
-CollectionListResponse = List[CollectionListItemModel]
+class CollectionResponseModel(BaseModel):
+    items: List[CollectionModel]
+
+
+class CollectionCreateResponse(BaseModel):
+    last_modified: datetime
+    collection_id: Optional[str]
 
 
 class DatasetName(ConstrainedStr):
     min_length = 1
 
 
 class DatasetCreateResponse(BaseModel):
     last_modified: datetime
 
 
 class DatasetModel(BaseModel):
-    id: DatasetName
+    name: DatasetName
     hash: Optional[str]
     bytes: Optional[int]
     content_type: Optional[str]
     last_modified: Optional[datetime]
 
 
-DatasetListResponse = List[DatasetModel]
+class DatasetResponseModel(BaseModel):
+    items: List[DatasetModel]
 
 
 class SemanticMappingName(ConstrainedStr):
     min_length = 1
 
 
 class SemanticMappingModel(BaseModel):
```

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/system.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/system.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/models/transformation.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/models/transformation.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/routers/object_storage.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/routers/object_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional, Union
 
 from fastapi import APIRouter, HTTPException, Request, UploadFile
 from fastapi.responses import Response
 
 from ..models.object_storage import (
-    CollectionListResponse,
     CollectionName,
+    CollectionResponseModel,
     DatasetCreateResponse,
-    DatasetListResponse,
     DatasetName,
+    DatasetResponseModel,
     SemanticMappingListResponse,
     SemanticMappingModel,
 )
 
 router = APIRouter(
     prefix="/data",
     responses={
@@ -22,40 +22,40 @@
 
 
 @router.get(
     "",
     operation_id="listCollections",
     summary="List all collections",
     tags=["DataSource", "DataSink"],
-    response_model=CollectionListResponse,
+    response_model=CollectionResponseModel,
     responses={
         204: {"description": "No collections found."},
     },
 )
 async def list_collections(
     limit: int = 100, offset: int = 0
-) -> Union[CollectionListResponse, Response]:
+) -> Union[CollectionResponseModel, Response]:
     """List all collections."""
     raise HTTPException(status_code=501, detail="Not implemented.")
 
 
 @router.get(
     "/{collection_name}",
     operation_id="listDatasets",
     summary="List all datasets in a collection",
     tags=["DataSource"],
-    response_model=DatasetListResponse,
+    response_model=DatasetResponseModel,
     responses={
         204: {"description": "No datasets found."},
         404: {"description": "Container not found."},
     },
 )
 async def list_datasets(
     collection_name: CollectionName, limit: int = 100, offset: int = 0
-) -> Union[DatasetListResponse, Response]:
+) -> Union[DatasetResponseModel, Response]:
     """List all datasets."""
     raise HTTPException(status_code=501, detail="Not implemented.")
 
 
 CREATE_COLLECTION_DESCRIPTION = """
 To add custom metadata, add keys to the header of the form:
 
@@ -362,7 +362,69 @@
     },
 )
 async def get_semantic_mapping(
     semantic_mapping_id,
 ) -> Union[SemanticMappingModel, Response]:
     """Get a semantic mapping."""
     raise HTTPException(status_code=501, detail="Not implemented.")
+
+
+@router.get(
+    "/metadata/dcat/{collection_name}",
+    name="Get DCAT Collection Metadata",
+    operation_id="getCollectionMetadataDcat",
+    summary="Get a collection's DCAT metadata",
+    tags=["DataSource"],
+    response_class=Response,
+    responses={
+        404: {"description": "Not found."},
+    },
+)
+async def get_collection_metadata_dcat(collection_name: CollectionName) -> Response:
+    """Get the DCAT metadata for a collection."""
+    raise HTTPException(status_code=501, detail="Not implemented.")
+
+
+@router.get(
+    "/metadata/dcat/{collection_name}/{dataset_name}",
+    name="Get DCAT Dataset Metadata",
+    operation_id="getDatasetMetadataDcat",
+    summary="Get a dataset's DCAT metadata",
+    tags=["DataSource"],
+    response_class=Response,
+    responses={
+        404: {"description": "Not found."},
+    },
+)
+async def get_dataset_metadata_dcat(
+    collection_name: CollectionName, dataset_name: DatasetName
+) -> Response:
+    """Get the DCAT metadata for a dataset."""
+    raise HTTPException(status_code=501, detail="Not implemented.")
+
+
+@router.post(
+    "/query",
+    operation_id="query",
+    summary="execute a search query on datastore",
+    tags=["DataSource"],
+    responses={
+        400: {"description": "improper query."},
+    },
+)
+async def query(limit: int = 100, offset: int = 0):
+    """returns matching triples"""
+    raise HTTPException(status_code=501, detail="Not implemented.")
+
+
+@router.post(
+    "/query/{collection_name}/{dataset_name}",
+    operation_id="queryDataset",
+    summary="execute a search query on specific dataset in datastore",
+    tags=["DataSource"],
+    responses={
+        400: {"description": "improper query."},
+    },
+)
+async def query_dataset(limit: int = 100, offset: int = 0):
+    """returns matching triples"""
+    raise HTTPException(status_code=501, detail="Not implemented.")
```

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/routers/system.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/routers/system.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/routers/transformation.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/routers/transformation.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/marketplace_standard_app_api/security.py` & `marketplace_standard_app_api-0.5.0/marketplace_standard_app_api/security.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/openapi.json` & `marketplace_standard_app_api-0.5.0/openapi.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9520111320081419%*

 * *Differences: {"'components'": "{'schemas': {'DatasetModel': {'required': ['name'], 'properties': {'name': "*

 * *                 "OrderedDict([('title', 'Name'), ('minLength', 1), ('type', 'string')]), delete: "*

 * *                 "['id']}}, 'CollectionModel': OrderedDict([('title', 'CollectionModel'), "*

 * *                 "('required', ['name']), ('type', 'object'), ('properties', "*

 * *                 "OrderedDict([('count', OrderedDict([('title', 'Count'), ('type', 'integer')])), "*

 * *                 "('bytes', OrderedDict([('tit […]*

```diff
@@ -25,42 +25,60 @@
                 },
                 "required": [
                     "file"
                 ],
                 "title": "Body_createOrReplaceDataset",
                 "type": "object"
             },
-            "CollectionListItemModel": {
+            "CollectionModel": {
                 "properties": {
                     "bytes": {
                         "title": "Bytes",
                         "type": "integer"
                     },
                     "count": {
                         "title": "Count",
                         "type": "integer"
                     },
+                    "id": {
+                        "title": "Id",
+                        "type": "string"
+                    },
                     "last_modified": {
                         "format": "date-time",
                         "title": "Last Modified",
                         "type": "string"
                     },
                     "name": {
                         "maxLength": 255,
                         "minLength": 1,
                         "title": "Name",
                         "type": "string"
                     }
                 },
                 "required": [
-                    "count",
-                    "bytes",
                     "name"
                 ],
-                "title": "CollectionListItemModel",
+                "title": "CollectionModel",
+                "type": "object"
+            },
+            "CollectionResponseModel": {
+                "properties": {
+                    "items": {
+                        "items": {
+                            "$ref": "#/components/schemas/CollectionModel"
+                        },
+                        "title": "Items",
+                        "type": "array"
+                    }
+                },
+                "required": [
+                    "items"
+                ],
+                "title": "CollectionResponseModel",
                 "type": "object"
             },
             "DatasetCreateResponse": {
                 "properties": {
                     "last_modified": {
                         "format": "date-time",
                         "title": "Last Modified",
@@ -83,31 +101,47 @@
                         "title": "Content Type",
                         "type": "string"
                     },
                     "hash": {
                         "title": "Hash",
                         "type": "string"
                     },
-                    "id": {
-                        "minLength": 1,
-                        "title": "Id",
-                        "type": "string"
-                    },
                     "last_modified": {
                         "format": "date-time",
                         "title": "Last Modified",
                         "type": "string"
+                    },
+                    "name": {
+                        "minLength": 1,
+                        "title": "Name",
+                        "type": "string"
                     }
                 },
                 "required": [
-                    "id"
+                    "name"
                 ],
                 "title": "DatasetModel",
                 "type": "object"
             },
+            "DatasetResponseModel": {
+                "properties": {
+                    "items": {
+                        "items": {
+                            "$ref": "#/components/schemas/DatasetModel"
+                        },
+                        "title": "Items",
+                        "type": "array"
+                    }
+                },
+                "required": [
+                    "items"
+                ],
+                "title": "DatasetResponseModel",
+                "type": "object"
+            },
             "GlobalSearchResponse": {
                 "properties": {
                     "items": {
                         "items": {
                             "$ref": "#/components/schemas/GlobalSearchResponseItemModel"
                         },
                         "title": "Items",
@@ -381,15 +415,15 @@
         },
         "description": "Standard app API for the MarketPlace applications.",
         "license": {
             "name": "MIT",
             "url": "https://opensource.org/licenses/MIT"
         },
         "title": "MarketPlace Standard App API",
-        "version": "0.4.0"
+        "version": "0.5.0"
     },
     "openapi": "3.0.2",
     "paths": {
         "/": {
             "get": {
                 "description": "Open the frontpage of the app.",
                 "operationId": "frontend",
@@ -455,19 +489,15 @@
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
-                                    "items": {
-                                        "$ref": "#/components/schemas/CollectionListItemModel"
-                                    },
-                                    "title": "Response Listcollections",
-                                    "type": "array"
+                                    "$ref": "#/components/schemas/CollectionResponseModel"
                                 }
                             }
                         },
                         "description": "Successful Response"
                     },
                     "204": {
                         "description": "No collections found."
@@ -564,14 +594,284 @@
                 ],
                 "summary": "Create a collection",
                 "tags": [
                     "DataSink"
                 ]
             }
         },
+        "/data/metadata/dcat/{collection_name}": {
+            "get": {
+                "description": "Get the DCAT metadata for a collection.",
+                "operationId": "getCollectionMetadataDcat",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "collection_name",
+                        "required": true,
+                        "schema": {
+                            "maxLength": 255,
+                            "minLength": 1,
+                            "title": "Collection Name",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "description": "Successful Response"
+                    },
+                    "401": {
+                        "description": "Not authenticated."
+                    },
+                    "404": {
+                        "description": "Not found."
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    },
+                    "500": {
+                        "description": "Internal server error."
+                    },
+                    "501": {
+                        "description": "Not implemented."
+                    },
+                    "503": {
+                        "description": "Service unavailable."
+                    }
+                },
+                "security": [
+                    {
+                        "AuthTokenBearer": []
+                    }
+                ],
+                "summary": "Get a collection's DCAT metadata",
+                "tags": [
+                    "DataSource"
+                ]
+            }
+        },
+        "/data/metadata/dcat/{collection_name}/{dataset_name}": {
+            "get": {
+                "description": "Get the DCAT metadata for a dataset.",
+                "operationId": "getDatasetMetadataDcat",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "collection_name",
+                        "required": true,
+                        "schema": {
+                            "maxLength": 255,
+                            "minLength": 1,
+                            "title": "Collection Name",
+                            "type": "string"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "dataset_name",
+                        "required": true,
+                        "schema": {
+                            "minLength": 1,
+                            "title": "Dataset Name",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "description": "Successful Response"
+                    },
+                    "401": {
+                        "description": "Not authenticated."
+                    },
+                    "404": {
+                        "description": "Not found."
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    },
+                    "500": {
+                        "description": "Internal server error."
+                    },
+                    "501": {
+                        "description": "Not implemented."
+                    },
+                    "503": {
+                        "description": "Service unavailable."
+                    }
+                },
+                "security": [
+                    {
+                        "AuthTokenBearer": []
+                    }
+                ],
+                "summary": "Get a dataset's DCAT metadata",
+                "tags": [
+                    "DataSource"
+                ]
+            }
+        },
+        "/data/query": {
+            "post": {
+                "description": "returns matching triples",
+                "operationId": "query",
+                "parameters": [
+                    {
+                        "in": "query",
+                        "name": "limit",
+                        "required": false,
+                        "schema": {
+                            "default": 100,
+                            "title": "Limit",
+                            "type": "integer"
+                        }
+                    },
+                    {
+                        "in": "query",
+                        "name": "offset",
+                        "required": false,
+                        "schema": {
+                            "default": 0,
+                            "title": "Offset",
+                            "type": "integer"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {}
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "400": {
+                        "description": "improper query."
+                    },
+                    "401": {
+                        "description": "Not authenticated."
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    },
+                    "500": {
+                        "description": "Internal server error."
+                    },
+                    "501": {
+                        "description": "Not implemented."
+                    },
+                    "503": {
+                        "description": "Service unavailable."
+                    }
+                },
+                "security": [
+                    {
+                        "AuthTokenBearer": []
+                    }
+                ],
+                "summary": "execute a search query on datastore",
+                "tags": [
+                    "DataSource"
+                ]
+            }
+        },
+        "/data/query/{collection_name}/{dataset_name}": {
+            "post": {
+                "description": "returns matching triples",
+                "operationId": "queryDataset",
+                "parameters": [
+                    {
+                        "in": "query",
+                        "name": "limit",
+                        "required": false,
+                        "schema": {
+                            "default": 100,
+                            "title": "Limit",
+                            "type": "integer"
+                        }
+                    },
+                    {
+                        "in": "query",
+                        "name": "offset",
+                        "required": false,
+                        "schema": {
+                            "default": 0,
+                            "title": "Offset",
+                            "type": "integer"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {}
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "400": {
+                        "description": "improper query."
+                    },
+                    "401": {
+                        "description": "Not authenticated."
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    },
+                    "500": {
+                        "description": "Internal server error."
+                    },
+                    "501": {
+                        "description": "Not implemented."
+                    },
+                    "503": {
+                        "description": "Service unavailable."
+                    }
+                },
+                "security": [
+                    {
+                        "AuthTokenBearer": []
+                    }
+                ],
+                "summary": "execute a search query on specific dataset in datastore",
+                "tags": [
+                    "DataSource"
+                ]
+            }
+        },
         "/data/semanticMappings": {
             "get": {
                 "description": "List all semantic mappings.",
                 "operationId": "listSemanticMappings",
                 "parameters": [
                     {
                         "in": "query",
@@ -801,19 +1101,15 @@
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
-                                    "items": {
-                                        "$ref": "#/components/schemas/DatasetModel"
-                                    },
-                                    "title": "Response Listdatasets",
-                                    "type": "array"
+                                    "$ref": "#/components/schemas/DatasetResponseModel"
                                 }
                             }
                         },
                         "description": "Successful Response"
                     },
                     "204": {
                         "description": "No datasets found."
```

### Comparing `marketplace-standard-app-api-0.4.0/pyproject.toml` & `marketplace_standard_app_api-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 authors = [{name = "Carl Simon Adorf et al", email = "simon.adorf@epfl.ch"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8,<4"
 dependencies = [
-  "email-validator<2.0, >=1.2.1",
-  "fastapi<1.0, >0.75",
+  "email-validator<=2.0, >=1.2.1",
+  "fastapi<=0.95.1, >0.75",
   "python-multipart<=0.1, >0.0.5",
   "requests<3.0, >2.26.0",
 ]
 
 [project.urls]
 Home = "https://github.com/materials-marketplace/standard-app-api"
 
@@ -38,15 +38,15 @@
 name = "marketplace_standard_app_api"
 
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 
 [tool.bumpver]
-current_version = "v0.4.0"
+current_version = "v0.5.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `marketplace-standard-app-api-0.4.0/tests/conftest.py` & `marketplace_standard_app_api-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `marketplace-standard-app-api-0.4.0/PKG-INFO` & `marketplace_standard_app_api-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: marketplace-standard-app-api
-Version: 0.4.0
+Version: 0.5.0
 Summary: Materials-MarketPlace Standard App API
 Author-email: Carl Simon Adorf et al <simon.adorf@epfl.ch>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: email-validator<2.0, >=1.2.1
-Requires-Dist: fastapi<1.0, >0.75
+Requires-Dist: email-validator<=2.0, >=1.2.1
+Requires-Dist: fastapi<=0.95.1, >0.75
 Requires-Dist: python-multipart<=0.1, >0.0.5
 Requires-Dist: requests<3.0, >2.26.0
 Requires-Dist: click==8.1.3 ; extra == "cli"
 Requires-Dist: bumpver==2021.1114 ; extra == "dev"
 Requires-Dist: pytest==7.1.2 ; extra == "tests"
 Project-URL: Home, https://github.com/materials-marketplace/standard-app-api
 Provides-Extra: cli
@@ -21,15 +21,15 @@
 # README
 
 ## About
 
 This repository contains the specification of the Materials MarketPlace Standard App API.
 The API is used as basis for the interaction between apps on the Materials MarketPlace platform.
 
-This repository contains the API version: 0.4.0.
+This repository contains the API version: 0.5.0.
 
 ## Authors
 
 - Simon Adorf (simon.adorf@epfl.ch)
 - MarketPlace consortium partners
 
 ## Specification
```

