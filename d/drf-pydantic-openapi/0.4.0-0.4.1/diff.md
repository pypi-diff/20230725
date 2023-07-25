# Comparing `tmp/drf_pydantic_openapi-0.4.0.tar.gz` & `tmp/drf_pydantic_openapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pydantic_openapi-0.4.0.tar", max compression
+gzip compressed data, was "drf_pydantic_openapi-0.4.1.tar", max compression
```

## Comparing `drf_pydantic_openapi-0.4.0.tar` & `drf_pydantic_openapi-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.4.0/LICENSE
--rw-r--r--   0        0        0     2596 2023-05-09 09:59:45.223778 drf_pydantic_openapi-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/__init__.py
--rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/apps.py
--rw-r--r--   0        0        0     1456 2023-05-08 13:59:43.276920 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/errors.py
--rw-r--r--   0        0        0      489 2023-04-27 13:44:28.146816 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/exception_handler.py
--rw-r--r--   0        0        0     6091 2023-07-24 14:03:27.394681 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/generator.py
--rw-r--r--   0        0        0     2289 2023-06-02 08:27:03.420495 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/patches.py
--rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/path.py
--rw-r--r--   0        0        0     1517 2023-05-23 13:35:05.835776 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/ref_source.py
--rw-r--r--   0        0        0     4143 2023-05-26 14:34:32.395942 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/ref_utils.py
--rw-r--r--   0        0        0     1112 2023-07-24 14:01:09.538626 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/settings.py
--rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
--rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
--rw-r--r--   0        0        0      246 2023-07-24 13:38:54.240481 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/urls.py
--rw-r--r--   0        0        0     4085 2023-07-24 13:43:20.072536 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/utils.py
--rw-r--r--   0        0        0     2186 2023-07-24 14:04:40.140850 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/views.py
--rw-r--r--   0        0        0     1230 2023-07-24 14:05:12.043190 drf_pydantic_openapi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2596 2023-05-09 09:59:45.223778 drf_pydantic_openapi-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/apps.py
+-rw-r--r--   0        0        0     1456 2023-05-08 13:59:43.276920 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/errors.py
+-rw-r--r--   0        0        0      489 2023-04-27 13:44:28.146816 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/exception_handler.py
+-rw-r--r--   0        0        0     6097 2023-07-25 13:31:14.696792 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/generator.py
+-rw-r--r--   0        0        0     2289 2023-06-02 08:27:03.420495 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/patches.py
+-rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/path.py
+-rw-r--r--   0        0        0     1517 2023-05-23 13:35:05.835776 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/ref_source.py
+-rw-r--r--   0        0        0     4143 2023-05-26 14:34:32.395942 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/ref_utils.py
+-rw-r--r--   0        0        0     1112 2023-07-24 14:01:09.538626 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/settings.py
+-rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
+-rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
+-rw-r--r--   0        0        0      246 2023-07-24 13:38:54.240481 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/urls.py
+-rw-r--r--   0        0        0     4198 2023-07-25 13:30:08.336692 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/utils.py
+-rw-r--r--   0        0        0     2186 2023-07-24 14:04:40.140850 drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/views.py
+-rw-r--r--   0        0        0     1230 2023-07-25 13:37:47.392988 drf_pydantic_openapi-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.4.1/PKG-INFO
```

### Comparing `drf_pydantic_openapi-0.4.0/LICENSE` & `drf_pydantic_openapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/README.md` & `drf_pydantic_openapi-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/errors.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/errors.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/generator.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,18 @@
 
         if method.lower() in ("put", "patch", "post"):
             if docs and isclass(docs.body) and issubclass(docs.body, BaseModel):
                 schema = PydanticSchema(schema_class=docs.body)
                 request_body = RequestBody(content={"application/json": MediaType(schema=schema)})
 
         parameters = []
-        if docs and (path_param := docs.generate_parameter(ParameterLocation.PATH)):
-            parameters.append(path_param)
-        if docs and (query_param := docs.generate_parameter(ParameterLocation.QUERY)):
-            parameters.append(query_param)
+        if docs and (path_params := docs.generate_parameters(ParameterLocation.PATH)):
+            parameters.extend(path_params)
+        if docs and (query_params := docs.generate_parameters(ParameterLocation.QUERY)):
+            parameters.extend(query_params)
 
         return Operation(
             operation_id=path.get_operation_id(),
             requestBody=request_body,
             tags=path.get_tags(),
             responses=self.generate_responses(docstring, view_func),
             summary=docstring.short_description if docstring else "",
```

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/patches.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/patches.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/path.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/path.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/ref_source.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/ref_source.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/ref_utils.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/ref_utils.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/settings.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/settings.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/utils.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     ):
         self.errors = errors if errors is not None else []
         self.body = body
         self.query = query
         self.path = path
         self.response = response
 
-    def generate_parameter(self, parameter_location: ParameterLocation):
+    def generate_parameters(self, parameter_location: ParameterLocation):
+        params = []
         data = None
         if parameter_location == ParameterLocation.QUERY:
             data = self.query
         elif parameter_location == ParameterLocation.PATH:
             data = self.path
         elif parameter_location == ParameterLocation.BODY:
             data = self.body
@@ -72,21 +73,24 @@
                 if issubclass(type_, BaseModel):
                     schema = PydanticSchema(schema_class=type_)
                 else:
                     schema = Schema(type=get_builtin_type(type_))
 
                 description = field.field_info.description
 
-                return Parameter(
-                    name=field.name,
-                    description=description if description else "",
-                    param_in=parameter_location,
-                    param_schema=schema,
-                    required=field.required,
+                params.append(
+                    Parameter(
+                        name=field.name,
+                        description=description if description else "",
+                        param_in=parameter_location,
+                        param_schema=schema,
+                        required=field.required,
+                    )
                 )
+        return params
 
 
 def docs(
     errors: list[HttpError | Type[HttpError]] | None = None,
     body: BaseModel | None = None,
     query: BaseModel | None = None,
     path: BaseModel | None = None,
```

### Comparing `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/views.py` & `drf_pydantic_openapi-0.4.1/drf_pydantic_openapi/views.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.0/pyproject.toml` & `drf_pydantic_openapi-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-pydantic-openapi"
-version = "0.4.0"
+version = "0.4.1"
 description = "OpenAPI (v3) schema generation via Pydantic models using Django REST Framework."
 authors = ["iKlotho <umutkahrimanedu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drf_pydantic_openapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `drf_pydantic_openapi-0.4.0/PKG-INFO` & `drf_pydantic_openapi-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-pydantic-openapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: OpenAPI (v3) schema generation via Pydantic models using Django REST Framework.
 Author: iKlotho
 Author-email: umutkahrimanedu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

