# Comparing `tmp/dingodb-0.0.2.tar.gz` & `tmp/dingodb-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dingodb-0.0.2.tar", last modified: Thu Jul 20 09:36:11 2023, max compression
+gzip compressed data, was "dingodb-0.0.2rc1.tar", last modified: Tue Jul 25 09:03:22 2023, max compression
```

## Comparing `dingodb-0.0.2.tar` & `dingodb-0.0.2rc1.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-20 09:36:11.219554 dingodb-0.0.2/
--rw-rw-r--   0 gary      (1000) gary      (1000)      139 2023-07-18 06:02:01.000000 dingodb-0.0.2/.gitignore
--rw-rw-r--   0 gary      (1000) gary      (1000)       72 2023-07-20 09:31:54.000000 dingodb-0.0.2/MANIFEST.in
--rw-rw-r--   0 gary      (1000) gary      (1000)     5719 2023-07-20 09:36:11.219554 dingodb-0.0.2/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)     4314 2023-07-20 09:31:54.000000 dingodb-0.0.2/README.md
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-20 09:36:11.219554 dingodb-0.0.2/dingodb/
--rw-rw-r--   0 gary      (1000) gary      (1000)       60 2023-07-20 09:31:54.000000 dingodb-0.0.2/dingodb/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)        5 2023-07-20 09:36:07.000000 dingodb-0.0.2/dingodb/__version__
--rw-rw-r--   0 gary      (1000) gary      (1000)     1597 2023-07-20 09:31:54.000000 dingodb-0.0.2/dingodb/config.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    10983 2023-07-20 09:31:54.000000 dingodb-0.0.2/dingodb/db.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     6470 2023-07-20 09:31:54.000000 dingodb-0.0.2/dingodb/dingo_param.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-20 09:36:11.219554 dingodb-0.0.2/dingodb.egg-info/
--rw-rw-r--   0 gary      (1000) gary      (1000)     5719 2023-07-20 09:36:11.000000 dingodb-0.0.2/dingodb.egg-info/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)      330 2023-07-20 09:36:11.000000 dingodb-0.0.2/dingodb.egg-info/SOURCES.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-07-20 09:36:11.000000 dingodb-0.0.2/dingodb.egg-info/dependency_links.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       35 2023-07-20 09:36:11.000000 dingodb-0.0.2/dingodb.egg-info/requires.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        8 2023-07-20 09:36:11.000000 dingodb-0.0.2/dingodb.egg-info/top_level.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-07-13 06:19:14.000000 dingodb-0.0.2/pyproject.toml
--rw-rw-r--   0 gary      (1000) gary      (1000)       39 2023-07-14 07:04:50.000000 dingodb-0.0.2/requirements.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       38 2023-07-20 09:36:11.219554 dingodb-0.0.2/setup.cfg
--rw-rw-r--   0 gary      (1000) gary      (1000)     2006 2023-07-20 09:31:54.000000 dingodb-0.0.2/setup.py
--rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-07-13 05:53:08.000000 dingodb-0.0.2/tox.ini
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-25 09:03:22.153192 dingodb-0.0.2rc1/
+-rw-rw-r--   0 gary      (1000) gary      (1000)       72 2023-07-20 09:31:54.000000 dingodb-0.0.2rc1/MANIFEST.in
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5724 2023-07-25 09:03:22.153192 dingodb-0.0.2rc1/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)     4317 2023-07-20 09:40:52.000000 dingodb-0.0.2rc1/README.md
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-25 09:03:22.153192 dingodb-0.0.2rc1/dingodb/
+-rw-rw-r--   0 gary      (1000) gary      (1000)       60 2023-07-20 09:31:54.000000 dingodb-0.0.2rc1/dingodb/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)       10 2023-07-25 09:02:44.000000 dingodb-0.0.2rc1/dingodb/__version__
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1600 2023-07-24 17:07:31.000000 dingodb-0.0.2rc1/dingodb/config.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    14301 2023-07-25 07:10:40.000000 dingodb-0.0.2rc1/dingodb/db.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     7393 2023-07-25 07:10:40.000000 dingodb-0.0.2rc1/dingodb/dingo_param.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-25 09:03:22.153192 dingodb-0.0.2rc1/dingodb.egg-info/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5724 2023-07-25 09:03:22.000000 dingodb-0.0.2rc1/dingodb.egg-info/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)      311 2023-07-25 09:03:22.000000 dingodb-0.0.2rc1/dingodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-07-25 09:03:22.000000 dingodb-0.0.2rc1/dingodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       62 2023-07-25 09:03:22.000000 dingodb-0.0.2rc1/dingodb.egg-info/requires.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        8 2023-07-25 09:03:22.000000 dingodb-0.0.2rc1/dingodb.egg-info/top_level.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-07-13 06:19:14.000000 dingodb-0.0.2rc1/pyproject.toml
+-rw-rw-r--   0 gary      (1000) gary      (1000)       70 2023-07-24 17:07:31.000000 dingodb-0.0.2rc1/requirements.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       38 2023-07-25 09:03:22.153192 dingodb-0.0.2rc1/setup.cfg
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2006 2023-07-20 09:31:54.000000 dingodb-0.0.2rc1/setup.py
```

### Comparing `dingodb-0.0.2/PKG-INFO` & `dingodb-0.0.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingodb
-Version: 0.0.2
+Version: 0.0.2rc1
 Summary: dingodb is dingodb sdk
 Home-page: https://www.dingodb.com/
 Author: DingoDB
 Author-email: dingodb@zetyun.com
 License: Proprietary License
 Project-URL: Homepage, https://www.dingodb.com/
 Project-URL: Documentation, https://dingodb.readthedocs.io/en/latest/
@@ -29,17 +29,17 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # python-dingodb
-The DingDB python sdk
+The DingoDB python sdk
 
-First, you have prepared the DingDB environment, see the docs at https://github.com/dingodb/dingo-deploy.git
+First, you have prepared the DingoDB environment, see the docs at https://github.com/dingodb/dingo-deploy.git
 
 For more information, see the docs at https://dingodb.readthedocs.io/en/latest/
 
 ## Installation
 
 Install python-dingodb from pip:
 ```shell
```

### Comparing `dingodb-0.0.2/README.md` & `dingodb-0.0.2rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # python-dingodb
-The DingDB python sdk
+The DingoDB python sdk
 
-First, you have prepared the DingDB environment, see the docs at https://github.com/dingodb/dingo-deploy.git
+First, you have prepared the DingoDB environment, see the docs at https://github.com/dingodb/dingo-deploy.git
 
 For more information, see the docs at https://dingodb.readthedocs.io/en/latest/
 
 ## Installation
 
 Install python-dingodb from pip:
 ```shell
@@ -84,8 +84,8 @@
 ```
 
 ### Drop index
 The following example Drop one index.
 ```python
 >>> dingo_client.delete_index("testdingo")
 True
-```
+```
```

### Comparing `dingodb-0.0.2/dingodb/config.py` & `dingodb-0.0.2rc1/dingodb/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 metric_type = {
     "euclidean": "METRIC_TYPE_L2",
-    "product": "METRIC_TYPE_INNER_PRODUCT"
+    "dotproduct": "METRIC_TYPE_INNER_PRODUCT"
 }
 
 
 # proto
 index_config = {
     "flat": {
                 "flatParam": {
```

### Comparing `dingodb-0.0.2/dingodb/db.py` & `dingodb-0.0.2rc1/dingodb/db.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 import json
 import requests
 
 from .dingo_param import CheckClintParam, CheckCreateIndexParam, CheckVectorAddParam, CheckVectorSearchParam, \
-    CheckVectorGetParam, CheckVectorDeleteParam
+    CheckVectorGetParam, CheckVectorDeleteParam, CheckVectorScanParam
 
 
 class DingoDB:
     headers = {"Content-Type": "application/json"}
     requestProto = "http://"
     indexApi = "/index/api/dingo/"
     vectorApi = "/vector/api/dingo/"
@@ -21,62 +21,72 @@
             password (str): DingoDB password
             host (list): DingoDB host:port
         """
         params = CheckClintParam(user=user, password=password, host=host)
         self.user = params.user
         self.password = params.password
         self.host = params.host
+        self.session = requests.Session()
+    
+    def __del__(self):
+        self.session.close()
+        
+    def close(self):
+        self.session.close()
 
     def describe_index_info(self, index_name: str) -> dict:
         """
         describe_index_info index info
 
         Args:
             index_name (str): the name the index
 
         Raises:
             RuntimeError: return error
 
         Returns:
             dict: index info
         """
-        res = requests.get(f"{self.requestProto}{self.host[0]}{self.indexApi}{index_name}", headers=self.headers)
+        res = self.session.get(f"{self.requestProto}{self.host[0]}{self.indexApi}{index_name}", headers=self.headers)
+        
         if res.status_code == 200:
             return res.json()
         else:
             raise RuntimeError(res.json())
 
     def create_index(self,  index_name: str, dimension: int, index_type: str = "hnsw", metric_type: str = "euclidean",
                      replicas: int = 3, index_config: dict = None, metadata_config: dict = None,
-                     partition_rule: dict = None, operand: list = None, auto_id: bool = True) -> bool:
+                     partition_rule: dict = None, operand: list = None, auto_id: bool = True,
+                     start_id: int = 1) -> bool:
         """
         create_index create index
 
         Args:
             index_name (str): the name of index
             dimension (int): dimension of vector
             index_type (str, optional): index type, one of {"flat", "hnsw"}. Defaults to "hnsw".
             metric_type (str, optional): metric type, one of {"dotproduct", "euclidean"}. Defaults to "euclidean".
             replicas (int, optional): dingoDB store replicas. Defaults to 3.
             index_config (dict, optional): Advanced configuration options for the index. Defaults to None.
             metadata_config (dict, optional): metadata. Defaults to None.
             partition_rule (dict, optional): partition rule. Defaults to None.
             operand (list, optional): operand. Defaults to None.
             auto_id (bool, optional): isAutoIncrement or not isAutoIncrement. Defaults to True.
+            start_id (int, optional): autoIncrement start id. Defaults to 1.
 
         Raises:
-            RuntimeError: _description_
+            RuntimeError: return error
 
         Returns:
-            bool: _description_
+            bool: create table status
         """
         params = CheckCreateIndexParam(index_name=index_name, dimension=dimension, index_type=index_type,
                                        metric_type=metric_type, replicas=replicas, index_config=index_config,
                                        metadata_config=metadata_config, partition_rule=partition_rule, operand=operand,
-                                       auto_id=auto_id)
+                                       auto_id=auto_id, start_id=start_id)
 
         if params.partition_rule == {} and operand is not None and len(operand) != 0:
             details = []
             for item in operand:
                 details.append(
                     {
                         "operand": [item],
@@ -87,31 +97,31 @@
             partition_rule = {
                 "cols": [],
                 "details": details,
                 "funcName": ""
             }
 
         index_definition = {
-            "autoIncrement": 1,
+            "autoIncrement": params.start_id,
             "isAutoIncrement": "true" if params.auto_id else "false",
             "indexParameter": {
                 "indexType": "INDEX_TYPE_VECTOR",
                 "vectorIndexParameter": params.index_config
             },
             "name": params.index_name,
             "indexPartition": partition_rule if partition_rule is not None else params.partition_rule,
             "replica": params.replicas,
             "version": 0
         }
-
-        res = requests.post(f"{self.requestProto}{self.host[0]}{self.indexApi}", headers=self.headers,
-                            data=json.dumps(index_definition))
+        res = self.session.post(f"{self.requestProto}{self.host[0]}{self.indexApi}", headers=self.headers,
+                                data=json.dumps(index_definition))
         if res.status_code == 200:
             return True
-        raise RuntimeError(res.json())
+        else:
+            raise RuntimeError(res.json())
 
     def update_index_max_element(self, index_name: str, max_element: int) -> bool:
         """
         update_index_max_element change index max element
 
         only for hnsw
 
@@ -121,36 +131,39 @@
 
         Raises:
             RuntimeError: return error
 
         Returns:
             bool: True/False
         """
-        res = requests.put(f"{self.requestProto}{self.host[0]}{self.indexApi}{index_name}/{max_element}")
+        
+        res = self.session.put(f"{self.requestProto}{self.host[0]}{self.indexApi}{index_name}/{max_element}")
         if res.status_code == 200:
             return True
-        raise RuntimeError(res.json())
+        else:
+            raise RuntimeError(res.json())
     
     def delete_index(self, index_name: str) -> bool:
         """
         delete_index del/drop index
 
         Args:
             index_name (str): the name of index
 
         Raises:
             RuntimeError: return error
 
         Returns:
             bool: True/False
         """
-        res = requests.delete(f"{self.requestProto}{self.host[0]}{self.indexApi}{index_name}")
+        res = self.session.delete(f"{self.requestProto}{self.host[0]}{self.indexApi}{index_name}")
         if res.status_code == 200:
             return True
-        raise RuntimeError(res.json())
+        else:
+            raise RuntimeError(res.json())
 
     def vector_add(self, index_name: str, datas: list, vectors: list, ids: list = None) -> list:
         """
         vector_add add vector
 
         Args:
             index_name (str): the name of index
@@ -181,38 +194,100 @@
             record = {
                     "scalarData": scalar_data,
                     "vector": vector
                 }
             if ids is not None:
                 record.update({"id": params.ids[i]})
             
-            records.append(record) 
-            
-        res = requests.put(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}",
-                           headers=self.headers, data=json.dumps(records))
+            records.append(record)
+        res = self.session.put(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}",
+                               headers=self.headers, data=json.dumps(records))
         if res.status_code == 200:
             records = res.json()
             return records
-        raise RuntimeError(res.json())
+        else:
+            raise RuntimeError(res.json())
+    
+    def vector_count(self, index_name: str):
+        """
+        vector_count count in index
+
+        Args:
+            index_name (str): the name of in index
+        
+        Returns:
+            int: count num
+        """
+        res = self.session.get(f"{self.requestProto}{self.host[0]}{self.vectorApi}{index_name}", headers=self.headers)
+        if res.status_code == 200:
+            records = res.json()
+            return records.get("currentCount") - records.get("deletedCount")
+        else:
+            raise RuntimeError(res.json())
+        
+    def vector_scan(self, index_name: str, start_id: int, max_count: int = 1000, is_reverse: bool = False,
+                    with_scalar_data: bool = True, with_table_data: bool = True, without_vector_data: bool = False,
+                    filter_scalar: list = None) -> list:
+        """
+        vector_scan scan with start_id
 
+        Args:
+            index_name (str): the name of in index
+            start_id (int): start id
+            max_count (int, optional): max scan count. Defaults to 1000.
+            is_reverse (bool, optional): whether or not reverse. Defaults to False.
+            with_scalar_data (bool, optional): whether  with scalar info. Defaults to True.
+            with_table_data (bool, optional): whether  with table info. Defaults to True.
+            without_vector_data (bool, optional): whether with vector info. Defaults to False.
+            filter_scalar (list, optional): scalar filter filed. Defaults to [].
+
+        Raises:
+            RuntimeError: return error
+
+        Returns:
+            list:  scan info list
+        """
+        params = CheckVectorScanParam(index_name=index_name, start_id=start_id, max_count=max_count,
+                                      is_reverse=is_reverse, with_scalar_data=with_scalar_data,
+                                      with_table_data=with_table_data, without_vector_data=without_vector_data,
+                                      filter_scalar=filter_scalar)
+        payload = {
+            "isReverseScan": params.is_reverse,
+            "maxScanCount": params.max_count,
+            "selectedKeys": params.filter_scalar,
+            "startId": params.start_id,
+            "withScalarData": params.with_scalar_data,
+            "withTableData": params.with_table_data,
+            "withoutVectorData": params.without_vector_data
+        }
+        res = self.session.post(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}/scan",
+                                headers=self.headers, data=json.dumps(payload))
+        if res.status_code == 200:
+            records = res.json()
+            return records
+        else:
+            raise RuntimeError(res.json())
+        
     def get_index(self):
         """
         get_index get all index
 
         Raises:
             RuntimeError: return error
 
         Returns:
             list: all index list 
         """
-        res = requests.get(f"{self.requestProto}{self.host[0]}{self.indexApi}", headers=self.headers)
+
+        res = self.session.get(f"{self.requestProto}{self.host[0]}{self.indexApi}", headers=self.headers)
         if res.status_code == 200:
             indics = res.json()
             return indics
-        raise RuntimeError(res.json())
+        else:
+            raise RuntimeError(res.json())
 
     def get_max_index_row(self, index_name: str):
         """
         get_max_index_row get max id in index
 
         Args:
             index_name (str): the name of in index 
@@ -220,20 +295,22 @@
         Raises:
             RuntimeError: return error
 
         Returns:
             int: max id value
         """
         payload = {"isGetMin": "false"}
-        res = requests.get(f"{self.requestProto}{self.host[0]}{self.vectorApi}{index_name}/id", params=payload,
-                           headers=self.headers)
+
+        res = self.session.get(f"{self.requestProto}{self.host[0]}{self.vectorApi}{index_name}/id",
+                               params=payload, headers=self.headers)
         if res.status_code == 200:
-            id = res.json()
-            return id
-        raise RuntimeError(res.json())
+            max_id = res.json()
+            return max_id
+        else:
+            raise RuntimeError(res.json())
 
     def vector_search(self, index_name: str, xq: list, top_k: int = 10, search_params: dict = None) -> dict:
         """
         vector_search search vector
 
         Args:
             index_name (str): the name of the index 
@@ -245,20 +322,22 @@
             RuntimeError: return error
 
         Returns:
             List[dict]: search results
         """
         params = CheckVectorSearchParam(index_name=index_name, xq=xq, top_k=top_k, search_params=search_params)
         
-        res = requests.post(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}",
-                            headers=self.headers, data=json.dumps(params.search_params))
+        res = self.session.post(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}",
+                                headers=self.headers, data=json.dumps(params.search_params))
+        
         if res.status_code == 200:
             records = res.json()
             return records
-        raise RuntimeError(res.json())
+        else:
+            raise RuntimeError(res.json())
     
     def vector_get(self, index_name: str, ids: list, scalar: bool = True, vector: bool = True) -> list:
         """
         vector_get query vector
 
         Args:
             index_name (str): the name of the index
@@ -275,16 +354,18 @@
         params = CheckVectorGetParam(index_name=index_name, ids=ids, scalar=scalar, vector=vector)
         payload = {
             "ids": params.ids,
             "keys": [],
             "withScalarData": "true" if scalar else "false",
             "withoutVectorData": "false" if vector else "true"
         }
-        res = requests.post(f"{self.requestProto}{self.host[0]}{self.vectorApi}{ params.index_name}/get",
-                            headers=self.headers, data=json.dumps(payload))
+        
+        res = self.session.post(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}/get",
+                                headers=self.headers, data=json.dumps(payload))
+        
         if res.status_code == 200:
             records = res.json()
             return records
         else:
             raise RuntimeError(res.json())
 
     def vector_delete(self, index_name: str, ids: list):
@@ -298,13 +379,15 @@
         Raises:
             RuntimeError: return error
 
         Returns:
             list : [True, False, ...]
         """
         params = CheckVectorDeleteParam(index_name=index_name, ids=ids)
-        res = requests.delete(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}",
-                              headers=self.headers, data=json.dumps(params.ids))
+        
+        res = self.session.delete(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}",
+                                  headers=self.headers, data=json.dumps(params.ids))
+        
         if res.status_code == 200:
             return res.json()
         else:
             raise RuntimeError(res.json())
```

### Comparing `dingodb-0.0.2/dingodb/dingo_param.py` & `dingodb-0.0.2rc1/dingodb/dingo_param.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, List, Optional
+from typing import List
 import warnings
 
 from pydantic import BaseModel, validator
 from . import config
 
 
 class CheckClintParam(BaseModel):
@@ -18,14 +18,15 @@
     metric_type: str = "euclidean"
     replicas: int = 3
     index_config: dict = None
     metadata_config: dict = None
     partition_rule: dict = None
     operand: list = None
     auto_id: bool = True
+    start_id: int = 1
 
     @validator("index_type", always=True)
     def check_index_type(cls, value):
         if value not in config.index_config.keys():
             raise Exception(f"index_type  must in {list(config.index_config.keys())}")
         return value
     
@@ -46,27 +47,27 @@
     def check_index_config(cls, value, values):
         index_type = values.get("index_type")
         dimension = values.get("dimension")
         metric_type = values.get("metric_type")
         vector_index_parameter = config.index_config[index_type]
         
         if value is not None:
+            index_keys = vector_index_parameter[list(vector_index_parameter.keys())[0]].keys()
             for key, v in value.items():
-                index_keys = vector_index_parameter[list(vector_index_parameter.keys())[0]].keys()
                 if key in index_keys:
                     vector_index_parameter[list(vector_index_parameter.keys())[0]][key] = v
-                    if key == "efConstruction" and v > 500 or v < 100:
+                    if key == "efConstruction" and (v > 500 or v < 100):
                         if v < 0:
                             raise Exception(f"{key} must >= 0")
                         warnings.warn(f"efConstruction: {v} suggestion in 100-500")
-                    if key == "maxElements" and v > 1000000000 or v < 50000:
+                    if key == "maxElements" and (v > 1000000000 or v < 50000):
                         if v < 0:
                             raise Exception(f"{key} must >= 0")
                         warnings.warn(f"maxElements:{v} suggestion in 50000-1000000000")
-                    if key == "nlinks" and v > 64 or v < 16:
+                    if key == "nlinks" and (v > 64 or v < 16):
                         if v < 0:
                             raise Exception(f"{key} must >= 0")
                         warnings.warn(f"nlinks:{v} suggestion in 16-64")
                 else:
                     warnings.warn(f"index_config {key} not in {index_type}")
         
         vector_index_parameter[list(vector_index_parameter.keys())[0]]["dimension"] = dimension
@@ -97,14 +98,42 @@
                 f"length datas:{len(values.get('datas'))} vectors: {len(values.get('vectors'))} is not equal"
         else:
             assert len(values.get('datas')) == len(values.get('vectors')) == len(value), \
                 f"length datas:{len(values.get('datas'))} vectors: {len(values.get('vectors'))} ids:{len(value)} is not equal"
         return value
 
 
+class CheckVectorScanParam(BaseModel):
+    index_name: str
+    start_id: int
+    max_count: int = 1000
+    is_reverse: bool = False
+    with_scalar_data: bool = True
+    with_table_data: bool = True
+    without_vector_data: bool = False
+    filter_scalar: list = None
+    
+    @validator("*", always=True)
+    def check_input(cls, value, field):
+        if field.name == "start_id":
+            if not value > 0:
+                raise Exception("start_id must > 0")   
+        if field.name == "max_count":
+            if not value > 0:
+                raise Exception("max_count must > 0")
+        if field.name == "is_reverse" or field.name == "with_scalar_data" or field.name == "with_table_data" or \
+                field.name == "without_vector_data":
+            value = "true" if value else "false"
+        if field.name == "filter_scalar":
+            if value is None:
+                value = []
+
+        return value
+
+
 class CheckVectorSearchParam(BaseModel):
     index_name: str
     xq: list
     top_k: int = 10
     search_params: dict = None
 
     @validator("xq", always=True)
```

### Comparing `dingodb-0.0.2/dingodb.egg-info/PKG-INFO` & `dingodb-0.0.2rc1/dingodb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingodb
-Version: 0.0.2
+Version: 0.0.2rc1
 Summary: dingodb is dingodb sdk
 Home-page: https://www.dingodb.com/
 Author: DingoDB
 Author-email: dingodb@zetyun.com
 License: Proprietary License
 Project-URL: Homepage, https://www.dingodb.com/
 Project-URL: Documentation, https://dingodb.readthedocs.io/en/latest/
@@ -29,17 +29,17 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # python-dingodb
-The DingDB python sdk
+The DingoDB python sdk
 
-First, you have prepared the DingDB environment, see the docs at https://github.com/dingodb/dingo-deploy.git
+First, you have prepared the DingoDB environment, see the docs at https://github.com/dingodb/dingo-deploy.git
 
 For more information, see the docs at https://dingodb.readthedocs.io/en/latest/
 
 ## Installation
 
 Install python-dingodb from pip:
 ```shell
```

### Comparing `dingodb-0.0.2/setup.py` & `dingodb-0.0.2rc1/setup.py`

 * *Files identical despite different names*

