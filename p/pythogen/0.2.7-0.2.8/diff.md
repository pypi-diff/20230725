# Comparing `tmp/pythogen-0.2.7.tar.gz` & `tmp/pythogen-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.7.tar", max compression
+gzip compressed data, was "pythogen-0.2.8.tar", max compression
```

## Comparing `pythogen-0.2.7.tar` & `pythogen-0.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1069 2023-07-24 22:37:11.228763 pythogen-0.2.7/LICENSE
--rw-r--r--   0        0        0     2097 2023-07-24 22:37:11.228763 pythogen-0.2.7/README.md
--rw-r--r--   0        0        0     1616 2023-07-24 22:37:11.232763 pythogen-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1585 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/main.py
--rw-r--r--   0        0        0     7660 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/models.py
--rw-r--r--   0        0        0     2355 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3239 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/response.py
--rw-r--r--   0        0        0    17663 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0    10836 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/renderer.py
--rw-r--r--   0        0        0      286 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/settings.py
--rw-r--r--   0        0        0    10789 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client/main.j2
--rw-r--r--   0        0        0     4320 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client/method.j2
--rw-r--r--   0        0        0     2487 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client/operation_params_schemas.j2
--rw-r--r--   0        0        0     1471 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client/request-metrics.j2
--rw-r--r--   0        0        0       33 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client_package/init-py.j2
--rw-r--r--   0        0        0      312 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client_package/pyproject-toml.j2
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 pythogen-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-25 15:38:38.807537 pythogen-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2206 2023-07-25 15:38:38.807537 pythogen-0.2.8/README.md
+-rw-r--r--   0        0        0     1650 2023-07-25 15:38:38.811537 pythogen-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1730 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/main.py
+-rw-r--r--   0        0        0     7660 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/models.py
+-rw-r--r--   0        0        0     2355 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3669 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    17663 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0    10836 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/renderer.py
+-rw-r--r--   0        0        0      286 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/settings.py
+-rw-r--r--   0        0        0    10789 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client/main.j2
+-rw-r--r--   0        0        0     4320 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client/method.j2
+-rw-r--r--   0        0        0     2487 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client/operation_params_schemas.j2
+-rw-r--r--   0        0        0     1471 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client/request-metrics.j2
+-rw-r--r--   0        0        0       33 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client_package/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client_package/pyproject-toml.j2
+-rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 pythogen-0.2.8/PKG-INFO
```

### Comparing `pythogen-0.2.7/LICENSE` & `pythogen-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/README.md` & `pythogen-0.2.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -46,11 +46,14 @@
 ```
 
 ## Usage
 ```python
 from petstore.client_async import Client
 from petstore.client_async import Pet
 from petstore.client_async import EmptyBody
+from petstore.client_async import FindPetsByStatusQueryParams
 
 client = Client(base_url="http://your.base.url")
-pets: list[Pet] | EmptyBody = await client.findPetsByStatus(status="available")
+pets: list[Pet] | EmptyBody = await client.findPetsByStatus(
+  query_params=FindPetsByStatusQueryParams(status="available"),
+)
 ```
```

### Comparing `pythogen-0.2.7/pyproject.toml` & `pythogen-0.2.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.7"
+version = "0.2.8"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
@@ -37,14 +37,15 @@
 rich = "^12.2.0"
 inflection = "^0.5.1"
 black = "^23.3.0"
 autoflake = "^2.2.0"
 isort = "^5.12.0"
 pydantic = "^2.0.2"
 pytest-cov = "^4.1.0"
+openapi-spec-validator = "^0.6.0"
 
 [tool.poetry.scripts]
 pythogen = 'pythogen.entrypoint:run'
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
```

### Comparing `pythogen-0.2.7/pythogen/models.py` & `pythogen-0.2.8/pythogen/models.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/packager.py` & `pythogen-0.2.8/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/parsers/document.py` & `pythogen-0.2.8/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.8/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/parsers/operations.py` & `pythogen-0.2.8/pythogen/parsers/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,25 @@
                 continue
 
             if response_data.get('$ref', None):
                 resolved_ref = self._ref_resolver.resolve(response_data['$ref'])
                 response_data = resolved_ref.ref_data
                 response_id = resolved_ref.ref_id
             else:
-                response_id = (
-                    f"{operation_data['operationId'].replace('_', ' ').title().replace(' ', '')}Response{status_code}"
-                )
+                operation_id: str = operation_data.get('operationId', '')
+                if not operation_id:
+                    operation_id = (
+                        path_str.removeprefix('/').replace('-', '_').replace('/', '_').replace('{', '').replace('}', '')
+                    )
+                    operation_id = method.value + '_' + operation_id
+                    operation_id = operation_id.lower()
+                else:
+                    operation_id = operation_id.replace('_', ' ').title().replace(' ', '')
+
+                response_id = f"{operation_id}Response{status_code}"
 
             responses[status_code] = self._response_parser.parse_item(response_id, response_data)
 
         request_body_data = operation_data.get('requestBody')
         if request_body_data:
             request_body = self._request_body_parser.parse_item(request_body_data, operation_data)
         else:
```

### Comparing `pythogen-0.2.7/pythogen/parsers/parameters.py` & `pythogen-0.2.8/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/parsers/paths.py` & `pythogen-0.2.8/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/parsers/references.py` & `pythogen-0.2.8/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/parsers/request_body.py` & `pythogen-0.2.8/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/parsers/response.py` & `pythogen-0.2.8/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/parsers/schemas.py` & `pythogen-0.2.8/pythogen/parsers/schemas.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/renderer.py` & `pythogen-0.2.8/pythogen/renderer.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/templates/http_client/main.j2` & `pythogen-0.2.8/pythogen/templates/http_client/main.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/templates/http_client/method.j2` & `pythogen-0.2.8/pythogen/templates/http_client/method.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/templates/http_client/operation_params_schemas.j2` & `pythogen-0.2.8/pythogen/templates/http_client/operation_params_schemas.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/pythogen/templates/http_client/request-metrics.j2` & `pythogen-0.2.8/pythogen/templates/http_client/request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.7/PKG-INFO` & `pythogen-0.2.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.7
+Version: 0.2.8
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
@@ -21,14 +21,15 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: autoflake (>=2.2.0,<3.0.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: jinja2 (>=3.1.1,<4.0.0)
+Requires-Dist: openapi-spec-validator (>=0.6.0,<0.7.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=12.2.0,<13.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/artsmolin/pythogen
 Description-Content-Type: text/markdown
@@ -81,12 +82,15 @@
 ```
 
 ## Usage
 ```python
 from petstore.client_async import Client
 from petstore.client_async import Pet
 from petstore.client_async import EmptyBody
+from petstore.client_async import FindPetsByStatusQueryParams
 
 client = Client(base_url="http://your.base.url")
-pets: list[Pet] | EmptyBody = await client.findPetsByStatus(status="available")
+pets: list[Pet] | EmptyBody = await client.findPetsByStatus(
+  query_params=FindPetsByStatusQueryParams(status="available"),
+)
 ```
```

