# Comparing `tmp/adsctl-0.4.0.tar.gz` & `tmp/adsctl-0.4.1.tar.gz`

## Comparing `adsctl-0.4.0.tar` & `adsctl-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,60 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 adsctl-0.4.0/.DS_Store
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 adsctl-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 adsctl-0.4.0/.python-version
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 adsctl-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 adsctl-0.4.0/RELEASE.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 adsctl-0.4.0/TESTING.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 adsctl-0.4.0/Taskfile.yml
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 adsctl-0.4.0/requirements-dev.lock
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 adsctl-0.4.0/requirements.lock
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/__about__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/__init__.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/application.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/client.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/parse.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/queries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/__init__.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/asset/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/asset/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/campaign/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/campaign/budget.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/campaign/main.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/campaign/status.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/__init__.py
--rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/auth.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/cli.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/config.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/create/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/create/asset.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/create/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/edit/__init__.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/edit/campaign.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/edit/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/config/__init__.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/config/config_file.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/config/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/__init__.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/cli.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/completer.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/key_bindings.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/prompt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/utils/__init__.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/utils/fs.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/test_config_file.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/test_parse.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/test_pkg.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/templates/config_1.toml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/templates/config_invalid_id.toml
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 adsctl-0.4.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 adsctl-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 adsctl-0.4.0/README.md
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 adsctl-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 adsctl-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 adsctl-0.4.1/.DS_Store
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 adsctl-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 adsctl-0.4.1/.python-version
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 adsctl-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 adsctl-0.4.1/RELEASE.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 adsctl-0.4.1/TESTING.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 adsctl-0.4.1/Taskfile.yml
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 adsctl-0.4.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 adsctl-0.4.1/requirements.lock
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/__about__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/__init__.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/application.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/client.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/parse.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/queries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/api/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/api/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/api/asset/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/api/asset/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/api/campaign/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/api/campaign/budget.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/api/campaign/main.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/api/campaign/status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/__init__.py
+-rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/auth.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/cli.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/config.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/create/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/create/asset.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/create/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/edit/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/edit/campaign.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/edit/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/get/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/get/campaign.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/cli/get/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/config/__init__.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/config/config_file.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/config/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/prompt/__init__.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/prompt/cli.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/prompt/completer.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/prompt/key_bindings.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/utils/__init__.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 adsctl-0.4.1/src/adsctl/utils/fs.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 adsctl-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 adsctl-0.4.1/tests/test_config_file.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 adsctl-0.4.1/tests/test_parse.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 adsctl-0.4.1/tests/test_pkg.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 adsctl-0.4.1/tests/templates/config_1.toml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 adsctl-0.4.1/tests/templates/config_invalid_id.toml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 adsctl-0.4.1/tmp/case_location_view.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 adsctl-0.4.1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 adsctl-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 adsctl-0.4.1/README.md
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 adsctl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 adsctl-0.4.1/PKG-INFO
```

### Comparing `adsctl-0.4.0/.DS_Store` & `adsctl-0.4.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/.pre-commit-config.yaml` & `adsctl-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/Taskfile.yml` & `adsctl-0.4.1/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/requirements-dev.lock` & `adsctl-0.4.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/requirements.lock` & `adsctl-0.4.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/application.py` & `adsctl-0.4.1/src/adsctl/application.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,39 +56,74 @@
 
     def create_client(self):
         gads_config = self.config_file.account.clientSettings()
         client_ = client_utils.get_client(gads_config, version=self.api_version)
         self.client = client_
         return client_
 
-    def query(self, query, customer_id=None, params: Union[dict, None] = None):
+    def query(
+        self, query, customer_id=None, params: Union[dict, None] = None, **kwargs
+    ):
         if params is None:
             params = {}
         customer_id = customer_id or self.config_file.account.customer_id
-        myclient = self.create_client()
-        stream = self.search_stream(query=query, client=myclient, params=params)
-        tables = parseStream(stream)
+
+        results = self.search_stream(query=query, params=params, **kwargs)
+
+        tables = parseStream(results)
         return tables
 
-    def search(self, query, client, customer_id=None, params: Union[dict, None] = None):
+    def search(
+        self, query, customer_id=None, params: Union[dict, None] = None, **kwargs
+    ):
         if params is None:
             params = {}
         customer_id = customer_id or self.customer_id or self.account.customer_id
         query_ = client_utils.render_template(query.strip(), **params)
 
-        ga_service = client.get_service("GoogleAdsService")
-        return ga_service.search(query=query_, customer_id=customer_id)
+        myclient = self.create_client()
+        ga_service = myclient.get_service("GoogleAdsService")
+
+        request = kwargs or {}
+        request["query"] = query_
+        request["customer_id"] = customer_id
+
+        results = ga_service.search(request=request)
+        rows = []
+        for row in results:
+            rows.append(row)
+
+        if results.summary_row:
+            rows.append(results.summary_row)
+
+        return rows
 
     def search_stream(
-        self, query, client, customer_id=None, params: Union[dict, None] = None
+        self, query, customer_id=None, params: Union[dict, None] = None, **kwargs
     ):
         if params is None:
             params = {}
         customer_id = customer_id or self.customer_id or self.account.customer_id
         query_ = client_utils.render_template(query.strip(), **params)
 
-        ga_service = client.get_service("GoogleAdsService")
-        return ga_service.search_stream(query=query_, customer_id=customer_id)
+        myclient = self.create_client()
+        ga_service = myclient.get_service("GoogleAdsService")
+
+        request = kwargs or {}
+        request["query"] = query_
+        request["customer_id"] = customer_id
+
+        stream = ga_service.search_stream(request=request)
+
+        rows = []
+        for batch in stream:
+            for row in batch.results:
+                rows.append(row)
+
+            if batch.summary_row:
+                rows.append(batch.summary_row)
+
+        return rows
 
 
 # Alias
 GoogleAds = Application
```

### Comparing `adsctl-0.4.0/src/adsctl/client.py` & `adsctl-0.4.1/src/adsctl/client.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/parse.py` & `adsctl-0.4.1/src/adsctl/parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import pandas as pd
 from google.protobuf.json_format import MessageToDict
 
 
-def parseStream(stream, ignoreFields=None, pandas=True):
+def parseStream(results, ignoreFields=None, pandas=True):
     """
     This one doesn't flatten the results, so you get multiple tables
     """
     tables = {}
 
     if ignoreFields is None:
         ignoreFields = ()
 
-    for batch in stream:
-        for row in batch.results:
-            if hasattr(row, "_pb"):
-                results_dict = MessageToDict(row._pb)
-            else:
-                results_dict = MessageToDict(row)
-
-            for resource_name, values in results_dict.items():
-                if resource_name not in tables:
-                    tables[resource_name] = {}
-
-                for col, value in values.items():
-                    if col not in ignoreFields:
-                        if col not in tables[resource_name]:
-                            tables[resource_name][col] = []
-                        tables[resource_name][col].append(value)
+    for row in results:
+        if hasattr(row, "_pb"):
+            results_dict = MessageToDict(row._pb)
+        else:
+            results_dict = MessageToDict(row)
+
+        for resource_name, values in results_dict.items():
+            if resource_name not in tables:
+                tables[resource_name] = {}
+
+            for col, value in values.items():
+                if col not in ignoreFields:
+                    if col not in tables[resource_name]:
+                        tables[resource_name][col] = []
+                    tables[resource_name][col].append(value)
 
     if pandas:
         return toPandas(tables)
     return tables
 
 
 def toPandas(tables):
```

### Comparing `adsctl-0.4.0/src/adsctl/queries.py` & `adsctl-0.4.1/src/adsctl/queries.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/api/asset/image.py` & `adsctl-0.4.1/src/adsctl/api/asset/image.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/api/campaign/budget.py` & `adsctl-0.4.1/src/adsctl/api/campaign/budget.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/api/campaign/status.py` & `adsctl-0.4.1/src/adsctl/api/campaign/status.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/cli/auth.py` & `adsctl-0.4.1/src/adsctl/cli/auth.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/cli/cli.py` & `adsctl-0.4.1/src/adsctl/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import click
 
 from adsctl.__about__ import __version__
 from adsctl.cli.auth import auth
 from adsctl.cli.config import config
 from adsctl.cli.create.main import create
 from adsctl.cli.edit.main import edit
+from adsctl.cli.get.main import get
 from adsctl.cli.utils import create_app
 
 
 @click.group()
 @click.option(
     "--config-file",
     "-f",
@@ -41,14 +42,15 @@
         app = create_app(config_file_path)
         ctx.obj = app
     except Exception as e:
         click.echo(f"Error loading config: {e}")
 
 
 main.add_command(auth)
+main.add_command(get)
 main.add_command(edit)
 main.add_command(create)
 main.add_command(config)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `adsctl-0.4.0/src/adsctl/cli/config.py` & `adsctl-0.4.1/src/adsctl/cli/config.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/cli/utils.py` & `adsctl-0.4.1/src/adsctl/cli/utils.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/cli/edit/campaign.py` & `adsctl-0.4.1/src/adsctl/cli/edit/campaign.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/config/config_file.py` & `adsctl-0.4.1/src/adsctl/config/config_file.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/config/model.py` & `adsctl-0.4.1/src/adsctl/config/model.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/prompt/cli.py` & `adsctl-0.4.1/src/adsctl/prompt/cli.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/prompt/completer.py` & `adsctl-0.4.1/src/adsctl/prompt/completer.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/prompt/key_bindings.py` & `adsctl-0.4.1/src/adsctl/prompt/key_bindings.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/src/adsctl/prompt/prompt.py` & `adsctl-0.4.1/src/adsctl/prompt/prompt.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from google.ads.googleads.errors import GoogleAdsException
 from prompt_toolkit import PromptSession
 from prompt_toolkit.completion import FuzzyCompleter, ThreadedCompleter
 from prompt_toolkit.history import FileHistory
 from tabulate import tabulate
 
 from adsctl.application import Application
-from adsctl.parse import parseStream
 from adsctl.prompt.completer import MyCustomCompleter
 from adsctl.prompt.key_bindings import adsctl_bindings
 
 
 def prompt_loop(app: Application, output="table", params: Union[dict, None] = None):
     if app.config_file_path is None:
         my_history = None
@@ -38,15 +37,25 @@
             if not query:
                 continue
 
             if query == "exit":
                 sys.exit(0)
 
             results = app.query(query=query, params=params)
-            # results = make_query(ga_service, customer_id, query, output=output)
+
+            print(results)
+
+            if output == "plain":
+                results = []
+                for batch in results:
+                    for row in batch.results:
+                        results.append(row)
+            elif output in ("table", "csv", "csv-files"):
+                for table, df in results.items():
+                    results[table] = df
 
             if results is None:
                 continue
 
             print_results(results, output=output)
 
         except GoogleAdsException as ex:
@@ -55,35 +64,14 @@
         except KeyboardInterrupt:
             pass
         except EOFError:
             # Control-D pressed
             sys.exit()
 
 
-def make_query(
-    app: Application, query, output="table", params: Union[dict, None] = None
-) -> None | list | dict:
-    results = None
-    stream = app.search_stream(query, params=params)
-
-    if output == "plain":
-        results = []
-        for batch in stream:
-            for row in batch.results:
-                results.append(row)
-    elif output in ("table", "csv", "csv-files"):
-        results = {}
-        tables = parseStream(stream, pandas=True)
-
-        for table, df in tables.items():
-            results[table] = df
-
-    return results
-
-
 def print_results(results, output="table"):
     if output == "plain":
         if len(results) == 0:
             click.echo("No results found")
         for row in results:
             click.echo(row)
     elif output == "table":
```

### Comparing `adsctl-0.4.0/src/adsctl/utils/fs.py` & `adsctl-0.4.1/src/adsctl/utils/fs.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/tests/conftest.py` & `adsctl-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/tests/test_config_file.py` & `adsctl-0.4.1/tests/test_config_file.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/tests/test_parse.py` & `adsctl-0.4.1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/.gitignore` & `adsctl-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/LICENSE.txt` & `adsctl-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/README.md` & `adsctl-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -168,25 +168,52 @@
 You can overwrite the account and customer ID using the `-a` and `-i` options.
 See `gaql --help` for more details.
 
 ## CLI
 
 ### Campaign Management
 
-#### Status management
+#### Get campaigns
+
+````shell
+
+```shell
+adsctl get campaign
+````
+
+```plain
+Name                                          Status             Id
+--------------------------------------------  --------  -----------
+Interplanetary Cruise Campaign #168961427368  Paused    20370195066
+Interplanetary Cruise Campaign #168961215970  Paused    20379497161
+```
+
+#### Status Management
 
 ```shell
-adsctl campaign -i <campaign-id> status enabled
-adsctl campaign -i <campaign-id> status paused
+adsctl edit campaign -i <campaign-id> status enabled
+
+adsctl edit campaign -i 20370195066 status enabled
+```
+
+```shell
+adsctl get campaign
+```
+
+```plain
+Name                                          Status             Id
+--------------------------------------------  --------  -----------
+Interplanetary Cruise Campaign #168961427368  Enabled   20370195066
+Interplanetary Cruise Campaign #168961215970  Paused    20379497161
 ```
 
 #### Update budget
 
 ```shell
-adsctl campaign -i <campaign-id> budget <amount>
+adsctl edit campaign -i <campaign-id> budget <amount>
 ```
 
 ## Python API
 
 You can also use the Python API to easily execute GAQL queries
 and get the results as a Python dict or pandas DataFrame.
 
@@ -210,15 +237,15 @@
   metrics.cost_micros,
   campaign.bidding_strategy_type
 FROM campaign
 WHERE segments.date DURING LAST_7_DAYS
   AND campaign.status != '{{ status }}'
 """
 
-tables = adsctl.query(get_campaigns_query, params={"status": "REMOVED"}})
+tables = google_ads.query(get_campaigns_query, params={"status": "REMOVED"}})
 
 # Print Pandas DataFrames
 for table_name, table in tables.items():
     print(table_name)
     print(table, "\n")
 ```
 
@@ -233,24 +260,13 @@
 0    210    6730050  0.011457  32047.857143       18330
 
 campaignBudget
                                        resourceName amountMicros
 0  customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ      1000000
 ```
 
-Or directly get a client to use search_stream directly:
-
-```python
-gads_client = google_ads.create_client()
-stream = self.search_stream(query, client=myclient)
-
-for batch in stream:
-    for row in batch.results:
-        ...
-```
-
 ## Disclaimer
 
 _This is not an official Google product_.
 
 This repository is maintained by a Googler but is not a supported Google product.
 Code and issues here are answered by maintainers and other community members on GitHub on a best-effort basis.
```

#### html2text {}

```diff
@@ -50,32 +50,37 @@
 specified in the `-v` options. ```shell gaql -c 'SELECT campaign.id,
 campaign.name FROM campaign WHERE campaign.id = {{ id }} ORDER BY campaign.id'
 -v id=123456789 ``` You can also pass `-v` without a command and use this the
 variables in the prompt queries: ```shell $ gaql -v id=123456789 -v field=name
 >>> SELECT campaign.id, campaign.{{ field }} FROM campaign WHERE campaign.id =
 {{ id }} ORDER BY campaign.id ``` ### Other options You can overwrite the
 account and customer ID using the `-a` and `-i` options. See `gaql --help` for
-more details. ## CLI ### Campaign Management #### Status management ```shell
-adsctl campaign -i  status enabled adsctl campaign -i  status paused ``` ####
-Update budget ```shell adsctl campaign -i  budget  ``` ## Python API You can
-also use the Python API to easily execute GAQL queries and get the results as a
-Python dict or pandas DataFrame. ```python import adsctl as ads # Read config
-file and creates the Google Ads client google_ads = ads.GoogleAds() # Execute
-GAQL query get_campaigns_query = """ SELECT campaign.name,
-campaign_budget.amount_micros, campaign.status, campaign.optimization_score,
-campaign.advertising_channel_type, metrics.clicks, metrics.impressions,
-metrics.ctr, metrics.average_cpc, metrics.cost_micros,
+more details. ## CLI ### Campaign Management #### Get campaigns ````shell
+```shell adsctl get campaign ```` ```plain Name Status Id ---------------------
+----------------------- -------- ----------- Interplanetary Cruise Campaign
+#168961427368 Paused 20370195066 Interplanetary Cruise Campaign #168961215970
+Paused 20379497161 ``` #### Status Management ```shell adsctl edit campaign -
+i  status enabled adsctl edit campaign -i 20370195066 status enabled ```
+```shell adsctl get campaign ``` ```plain Name Status Id ----------------------
+---------------------- -------- ----------- Interplanetary Cruise Campaign
+#168961427368 Enabled 20370195066 Interplanetary Cruise Campaign #168961215970
+Paused 20379497161 ``` #### Update budget ```shell adsctl edit campaign -
+i  budget  ``` ## Python API You can also use the Python API to easily execute
+GAQL queries and get the results as a Python dict or pandas DataFrame.
+```python import adsctl as ads # Read config file and creates the Google Ads
+client google_ads = ads.GoogleAds() # Execute GAQL query get_campaigns_query =
+""" SELECT campaign.name, campaign_budget.amount_micros, campaign.status,
+campaign.optimization_score, campaign.advertising_channel_type, metrics.clicks,
+metrics.impressions, metrics.ctr, metrics.average_cpc, metrics.cost_micros,
 campaign.bidding_strategy_type FROM campaign WHERE segments.date DURING
-LAST_7_DAYS AND campaign.status != '{{ status }}' """ tables = adsctl.query
+LAST_7_DAYS AND campaign.status != '{{ status }}' """ tables = google_ads.query
 (get_campaigns_query, params={"status": "REMOVED"}}) # Print Pandas DataFrames
 for table_name, table in tables.items(): print(table_name) print(table, "\n")
 ``` ```plain campaign resourceName status ... name optimizationScore 0
 customers/XXXXXXXXXX/campaigns/YYYYYYYYYYY ENABLED ... my-campaign 0.839904 [1
 rows x 6 columns] metrics clicks costMicros ctr averageCpc impressions 0 210
 6730050 0.011457 32047.857143 18330 campaignBudget resourceName amountMicros 0
-customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ 1000000 ``` Or directly get a
-client to use search_stream directly: ```python gads_client =
-google_ads.create_client() stream = self.search_stream(query, client=myclient)
-for batch in stream: for row in batch.results: ... ``` ## Disclaimer _This is
-not an official Google product_. This repository is maintained by a Googler but
-is not a supported Google product. Code and issues here are answered by
-maintainers and other community members on GitHub on a best-effort basis.
+customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ 1000000 ``` ## Disclaimer
+_This is not an official Google product_. This repository is maintained by a
+Googler but is not a supported Google product. Code and issues here are
+answered by maintainers and other community members on GitHub on a best-effort
+basis.
```

### Comparing `adsctl-0.4.0/pyproject.toml` & `adsctl-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adsctl-0.4.0/PKG-INFO` & `adsctl-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsctl
-Version: 0.4.0
+Version: 0.4.1
 Summary: Google Ads Control CLI and Prompt
 Project-URL: Documentation, https://github.com/danielfrg/adsctl#readme
 Project-URL: Issues, https://github.com/danielfrg/adsctl/issues
 Project-URL: Source, https://github.com/danielfrg/adsctl
 Author-email: Daniel Rodriguez <daniel@danielfrg.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -204,25 +204,52 @@
 You can overwrite the account and customer ID using the `-a` and `-i` options.
 See `gaql --help` for more details.
 
 ## CLI
 
 ### Campaign Management
 
-#### Status management
+#### Get campaigns
+
+````shell
+
+```shell
+adsctl get campaign
+````
+
+```plain
+Name                                          Status             Id
+--------------------------------------------  --------  -----------
+Interplanetary Cruise Campaign #168961427368  Paused    20370195066
+Interplanetary Cruise Campaign #168961215970  Paused    20379497161
+```
+
+#### Status Management
 
 ```shell
-adsctl campaign -i <campaign-id> status enabled
-adsctl campaign -i <campaign-id> status paused
+adsctl edit campaign -i <campaign-id> status enabled
+
+adsctl edit campaign -i 20370195066 status enabled
+```
+
+```shell
+adsctl get campaign
+```
+
+```plain
+Name                                          Status             Id
+--------------------------------------------  --------  -----------
+Interplanetary Cruise Campaign #168961427368  Enabled   20370195066
+Interplanetary Cruise Campaign #168961215970  Paused    20379497161
 ```
 
 #### Update budget
 
 ```shell
-adsctl campaign -i <campaign-id> budget <amount>
+adsctl edit campaign -i <campaign-id> budget <amount>
 ```
 
 ## Python API
 
 You can also use the Python API to easily execute GAQL queries
 and get the results as a Python dict or pandas DataFrame.
 
@@ -246,15 +273,15 @@
   metrics.cost_micros,
   campaign.bidding_strategy_type
 FROM campaign
 WHERE segments.date DURING LAST_7_DAYS
   AND campaign.status != '{{ status }}'
 """
 
-tables = adsctl.query(get_campaigns_query, params={"status": "REMOVED"}})
+tables = google_ads.query(get_campaigns_query, params={"status": "REMOVED"}})
 
 # Print Pandas DataFrames
 for table_name, table in tables.items():
     print(table_name)
     print(table, "\n")
 ```
 
@@ -269,24 +296,13 @@
 0    210    6730050  0.011457  32047.857143       18330
 
 campaignBudget
                                        resourceName amountMicros
 0  customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ      1000000
 ```
 
-Or directly get a client to use search_stream directly:
-
-```python
-gads_client = google_ads.create_client()
-stream = self.search_stream(query, client=myclient)
-
-for batch in stream:
-    for row in batch.results:
-        ...
-```
-
 ## Disclaimer
 
 _This is not an official Google product_.
 
 This repository is maintained by a Googler but is not a supported Google product.
 Code and issues here are answered by maintainers and other community members on GitHub on a best-effort basis.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adsctl Version: 0.4.0 Summary: Google Ads Control
+Metadata-Version: 2.1 Name: adsctl Version: 0.4.1 Summary: Google Ads Control
 CLI and Prompt Project-URL: Documentation, https://github.com/danielfrg/
 adsctl#readme Project-URL: Issues, https://github.com/danielfrg/adsctl/issues
 Project-URL: Source, https://github.com/danielfrg/adsctl Author-email: Daniel
 Rodriguez
 danielfrg.com> License-Expression: Apache-2.0 License-File: LICENSE.txt
 Keywords: cli,google ads,google ads api,prompt Classifier: Development Status
 :: 4 - Beta Classifier: Programming Language :: Python Classifier: Programming
@@ -69,32 +69,37 @@
 specified in the `-v` options. ```shell gaql -c 'SELECT campaign.id,
 campaign.name FROM campaign WHERE campaign.id = {{ id }} ORDER BY campaign.id'
 -v id=123456789 ``` You can also pass `-v` without a command and use this the
 variables in the prompt queries: ```shell $ gaql -v id=123456789 -v field=name
 >>> SELECT campaign.id, campaign.{{ field }} FROM campaign WHERE campaign.id =
 {{ id }} ORDER BY campaign.id ``` ### Other options You can overwrite the
 account and customer ID using the `-a` and `-i` options. See `gaql --help` for
-more details. ## CLI ### Campaign Management #### Status management ```shell
-adsctl campaign -i  status enabled adsctl campaign -i  status paused ``` ####
-Update budget ```shell adsctl campaign -i  budget  ``` ## Python API You can
-also use the Python API to easily execute GAQL queries and get the results as a
-Python dict or pandas DataFrame. ```python import adsctl as ads # Read config
-file and creates the Google Ads client google_ads = ads.GoogleAds() # Execute
-GAQL query get_campaigns_query = """ SELECT campaign.name,
-campaign_budget.amount_micros, campaign.status, campaign.optimization_score,
-campaign.advertising_channel_type, metrics.clicks, metrics.impressions,
-metrics.ctr, metrics.average_cpc, metrics.cost_micros,
+more details. ## CLI ### Campaign Management #### Get campaigns ````shell
+```shell adsctl get campaign ```` ```plain Name Status Id ---------------------
+----------------------- -------- ----------- Interplanetary Cruise Campaign
+#168961427368 Paused 20370195066 Interplanetary Cruise Campaign #168961215970
+Paused 20379497161 ``` #### Status Management ```shell adsctl edit campaign -
+i  status enabled adsctl edit campaign -i 20370195066 status enabled ```
+```shell adsctl get campaign ``` ```plain Name Status Id ----------------------
+---------------------- -------- ----------- Interplanetary Cruise Campaign
+#168961427368 Enabled 20370195066 Interplanetary Cruise Campaign #168961215970
+Paused 20379497161 ``` #### Update budget ```shell adsctl edit campaign -
+i  budget  ``` ## Python API You can also use the Python API to easily execute
+GAQL queries and get the results as a Python dict or pandas DataFrame.
+```python import adsctl as ads # Read config file and creates the Google Ads
+client google_ads = ads.GoogleAds() # Execute GAQL query get_campaigns_query =
+""" SELECT campaign.name, campaign_budget.amount_micros, campaign.status,
+campaign.optimization_score, campaign.advertising_channel_type, metrics.clicks,
+metrics.impressions, metrics.ctr, metrics.average_cpc, metrics.cost_micros,
 campaign.bidding_strategy_type FROM campaign WHERE segments.date DURING
-LAST_7_DAYS AND campaign.status != '{{ status }}' """ tables = adsctl.query
+LAST_7_DAYS AND campaign.status != '{{ status }}' """ tables = google_ads.query
 (get_campaigns_query, params={"status": "REMOVED"}}) # Print Pandas DataFrames
 for table_name, table in tables.items(): print(table_name) print(table, "\n")
 ``` ```plain campaign resourceName status ... name optimizationScore 0
 customers/XXXXXXXXXX/campaigns/YYYYYYYYYYY ENABLED ... my-campaign 0.839904 [1
 rows x 6 columns] metrics clicks costMicros ctr averageCpc impressions 0 210
 6730050 0.011457 32047.857143 18330 campaignBudget resourceName amountMicros 0
-customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ 1000000 ``` Or directly get a
-client to use search_stream directly: ```python gads_client =
-google_ads.create_client() stream = self.search_stream(query, client=myclient)
-for batch in stream: for row in batch.results: ... ``` ## Disclaimer _This is
-not an official Google product_. This repository is maintained by a Googler but
-is not a supported Google product. Code and issues here are answered by
-maintainers and other community members on GitHub on a best-effort basis.
+customers/XXXXXXXXXX/campaignBudgets/ZZZZZZZZZZZ 1000000 ``` ## Disclaimer
+_This is not an official Google product_. This repository is maintained by a
+Googler but is not a supported Google product. Code and issues here are
+answered by maintainers and other community members on GitHub on a best-effort
+basis.
```

