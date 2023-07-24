# Comparing `tmp/pythogen-0.2.6.tar.gz` & `tmp/pythogen-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.6.tar", max compression
+gzip compressed data, was "pythogen-0.2.7.tar", max compression
```

## Comparing `pythogen-0.2.6.tar` & `pythogen-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1069 2023-07-21 22:56:27.787128 pythogen-0.2.6/LICENSE
--rw-r--r--   0        0        0     2097 2023-07-21 22:56:27.787128 pythogen-0.2.6/README.md
--rw-r--r--   0        0        0     1616 2023-07-21 22:56:27.791128 pythogen-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1585 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/main.py
--rw-r--r--   0        0        0     7660 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/models.py
--rw-r--r--   0        0        0     2355 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3239 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/parsers/response.py
--rw-r--r--   0        0        0    17663 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0    10037 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/renderer.py
--rw-r--r--   0        0        0      286 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/settings.py
--rw-r--r--   0        0        0    10891 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client/main.j2
--rw-r--r--   0        0        0     5136 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client/method.j2
--rw-r--r--   0        0        0     1513 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client/request-metrics.j2
--rw-r--r--   0        0        0       33 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client_package/init-py.j2
--rw-r--r--   0        0        0      312 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client_package/pyproject-toml.j2
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 pythogen-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-24 22:37:11.228763 pythogen-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2097 2023-07-24 22:37:11.228763 pythogen-0.2.7/README.md
+-rw-r--r--   0        0        0     1616 2023-07-24 22:37:11.232763 pythogen-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1585 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/main.py
+-rw-r--r--   0        0        0     7660 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/models.py
+-rw-r--r--   0        0        0     2355 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3239 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    17663 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0    10836 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/renderer.py
+-rw-r--r--   0        0        0      286 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/settings.py
+-rw-r--r--   0        0        0    10789 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client/main.j2
+-rw-r--r--   0        0        0     4320 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client/method.j2
+-rw-r--r--   0        0        0     2487 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client/operation_params_schemas.j2
+-rw-r--r--   0        0        0     1471 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client/request-metrics.j2
+-rw-r--r--   0        0        0       33 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client_package/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-24 22:37:11.232763 pythogen-0.2.7/pythogen/templates/http_client_package/pyproject-toml.j2
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 pythogen-0.2.7/PKG-INFO
```

### Comparing `pythogen-0.2.6/LICENSE` & `pythogen-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/README.md` & `pythogen-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pyproject.toml` & `pythogen-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.6"
+version = "0.2.7"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
```

### Comparing `pythogen-0.2.6/pythogen/main.py` & `pythogen-0.2.7/pythogen/main.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/models.py` & `pythogen-0.2.7/pythogen/models.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/packager.py` & `pythogen-0.2.7/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/document.py` & `pythogen-0.2.7/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.7/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/operations.py` & `pythogen-0.2.7/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/parameters.py` & `pythogen-0.2.7/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/paths.py` & `pythogen-0.2.7/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/references.py` & `pythogen-0.2.7/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/request_body.py` & `pythogen-0.2.7/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/response.py` & `pythogen-0.2.7/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/parsers/schemas.py` & `pythogen-0.2.7/pythogen/parsers/schemas.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.6/pythogen/renderer.py` & `pythogen-0.2.7/pythogen/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         settings.CLIENT_TEMPLATE_NAME,
         globals={
             'varname': varname,
             'classname': classname,
             'typerepr': j2_typerepr,
             'responserepr': j2_responserepr,
             'iterresponsemap': iterresponsemap,
+            'parameterfield': parameterfield,
         },
     )
 
     prepared_operations = prepare_operations(document)
 
     rendered_client = template.render(
         document=document,
@@ -70,16 +71,17 @@
         post_no_body=prepared_operations.post_no_body,
         put=prepared_operations.put,
         delete_no_body=prepared_operations.delete_no_body,
         sync=sync,
         metrics=metrics,
         discriminator_base_class_schemas=document.discriminator_base_class_schemas,
         required_headers=required_headers,
+        operations=prepared_operations.all(),
     )
-    rendered_client = black.format_str(rendered_client, mode=black.FileMode())
+    rendered_client = black.format_str(rendered_client, mode=black.Mode(line_length=120))
     rendered_client = isort.code(
         rendered_client,
         force_grid_wrap=2,
         lines_after_imports=2,
         force_single_line=True,
         line_length=120,
     )
@@ -96,14 +98,24 @@
     get: dict[PathStr, models.OperationObject]
     post: dict[PathStr, models.OperationObject]
     post_no_body: dict[PathStr, models.OperationObject]
     put: dict[PathStr, models.OperationObject]
     patch: dict[PathStr, models.OperationObject]
     delete_no_body: dict[PathStr, models.OperationObject]
 
+    def all(self) -> tuple[models.OperationObject, ...]:
+        return (
+            *self.get.values(),
+            *self.post.values(),
+            *self.post_no_body.values(),
+            *self.put.values(),
+            *self.patch.values(),
+            *self.delete_no_body.values(),
+        )
+
 
 def prepare_operations(document: models.Document) -> PreparedOperations:
     prepared_operations: PreparedOperations = PreparedOperations(
         get={},
         post={},
         post_no_body={},
         put={},
@@ -203,15 +215,15 @@
         if not response.schema:
             types.append('EmptyBody')
         elif response.schema.type in [models.Type.string, models.Type.integer]:
             types.append(classname(response.schema.id))
         else:
             types.append(j2_typerepr(response.schema))
 
-    types = list(set(types))
+    types = sorted(list(set(types)))
 
     if not types:
         return 'None'
 
     elif len(types) == 1:
         return f'{types[0]} | None'
     else:
@@ -276,14 +288,25 @@
 
 
 def classname(value: str) -> str:
     value = value.replace('.', '')
     return inflection.camelize(value)
 
 
+def parameterfield(parameter: models.ParameterObject) -> str:
+    args: list[str] = []
+    if not parameter.required:
+        args.append('None')
+    if parameter.safety_key != parameter.orig_key:
+        args.append(f'alias="{parameter.orig_key}"')
+    if parameter.description:
+        args.append(f'description="{parameter.description}"')
+    return 'Field(' + ', '.join(args) + ')'
+
+
 PRIMITIVE_TYPE_MAPPING = {
     models.Type.integer: 'int',
     models.Type.number: 'float',
     models.Type.boolean: 'bool',
     models.Type.string: 'str',
     models.Type.null: 'None',
 }
```

### Comparing `pythogen-0.2.6/pythogen/templates/http_client/main.j2` & `pythogen-0.2.7/pythogen/templates/http_client/main.j2`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,18 @@
 try:
     DEFAULT_AUTH = httpx.USE_CLIENT_DEFAULT
 except AttributeError:
     DEFAULT_AUTH = None
 
 
 class MetricsIntegration(Protocol):
-    def on_request_error(self, client_name: str, error: Exception, http_method: str, http_target: str) -> None:
+    def on_request_error(self, client_name: str, error: Exception, http_method: str, http_target: str,) -> None:
         ...
 
-    def on_request_success(self, client_name: str, response, http_method: str, http_target: str) -> None:
+    def on_request_success(self, client_name: str, response, http_method: str, http_target: str,) -> None:
         ...
 
     def shadow_path(self) -> bool:
         ...
 
 
 {%- if metrics %}
@@ -202,14 +202,17 @@
 {%- endif %}
 {%- endfor %}
 
 class EmptyBody(BaseModel):
     status_code: int
     text: str
 
+
+{% include 'operation_params_schemas.j2' %}
+
 {% for schema in discriminator_base_class_schemas %}
 class {{ schema.name }}(BaseModel):
     {{ schema.attr }}: str
 
     @field_validator("{{ schema.attr }}", mode='before')
     def check(cls, v: str, info: FieldValidationInfo) -> str:
         type_hints = get_type_hints(cls)
@@ -230,24 +233,22 @@
     """
     {{ model.title }}
     """
     model_config = ConfigDict(
         populate_by_name=True,  # Addressing by field name, even if there is an alias.
     )
 
-    {% if model.required_properties|length > 0 %}# required ---{% endif %}
     {%- for property in model.required_properties %}
         {%- if property.schema.description %}
     {{ property.key }}: {{ typerepr(property.schema, document) }} = Field(description="{{ property.schema.description }}"{%- if property.safety_key %}, alias="{{ property.orig_key }}"{%- endif %})
         {%- else %}
     {{ property.key }}: {{ typerepr(property.schema, document) }}
         {%- endif %}
     {%- endfor %}
 
-    {% if model.optional_properties|length > 0 %}# optional ---{% endif %}
     {%- for property in model.optional_properties %}
         {%- if property.schema.description %}
     {{ property.key }}: {{ typerepr(property.schema, document) }} | None = Field(None, description="{{ property.schema.description }}"{%- if property.safety_key %}, alias="{{ property.orig_key }}"{%- endif %})
         {%- else %}
     {{ property.key }}: {{ typerepr(property.schema, document) }} | None = None
         {%- endif %}
     {%- endfor %}
```

### Comparing `pythogen-0.2.6/pythogen/templates/http_client/method.j2` & `pythogen-0.2.7/pythogen/templates/http_client/method.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,81 @@
     {%- for path, operation in items %}
     {%- if sync %}
     def {{ operation.fn_name }}(
     {%- else %}
     async def {{ operation.fn_name }}(
     {%- endif %}
         self,
+        {#- path params -#}
+        {% if operation.path_params %}
+        path_params: {{ classname(operation.fn_name) }}PathParams | dict[str, Any],
+        {% endif %}
+
+        {#- query params -#}
+        {% if operation.query_params %}
+        query_params: {{ classname(operation.fn_name) }}QueryParams | dict[str, Any],
+        {% endif %}
+
         {%- if operation.request_body and operation.request_body.is_multipart_form_data and operation.request_body.are_files_required %}
         files: Mapping[str, FileTypes] | Sequence[tuple[str, FileTypes]],
         {%- endif %}
-        {#- path params -#}
-        {%- for parameter in operation.path_params %}
-        {{ parameter.key }}: {{ typerepr(parameter.schema) }},
-        {%- endfor %}
-        {#- required query params -#}
-        {%- for parameter in operation.query_params -%}
-        {%- if parameter.required %}
-        {{ varname(parameter.key) }}: {{ typerepr(parameter.schema) }},
-        {%- endif %}
-        {%- endfor %}
-        {#- required headers -#}
-        {%- for parameter in operation.headers -%}
-        {%- if parameter.required %}
-        {{ varname(parameter.key) }}: {{ typerepr(parameter.schema) }},
-        {%- endif %}
-        {%- endfor %}
-        {%- if operation.request_body %}
-        body: {{ typerepr(operation.request_body.schema) }} | dict[str, Any] | None = None,
-        {%- endif %}
-        {#- optional query params -#}
-        {%- for parameter in operation.query_params -%}
-        {%- if not parameter.required %}
-        {{ varname(parameter.key) }}: {{ typerepr(parameter.schema) }} | None = None,
-        {%- endif %}
-        {%- endfor %}
-        {#- optional headers -#}
-        {%- for parameter in operation.headers -%}
-        {%- if not parameter.required %}
-        {{ varname(parameter.key) }}: {{ typerepr(parameter.schema) }} | None = None,
-        {%- endif %}
-        {%- endfor %}
+
         auth: BasicAuth | None = None,
         content: str | bytes | None = None,
         {%- if operation.request_body and operation.request_body.is_multipart_form_data and not operation.request_body.are_files_required %}
         files: Mapping[str, FileTypes] | Sequence[tuple[str, FileTypes]] | None = None,
         {%- endif %}
-        headers: dict[str, Any] | None = None,
-    ) -> {{ responserepr(operation.responses) }}:
-        url = self._get_url(f'{{ path }}')
 
-        params = {
-            {%- for parameter in operation.query_params %}
-            {%- if parameter.required %}
-            '{{ parameter.orig_key }}': {{ varname(parameter.key) }},
-            {%- endif %}
-            {%- endfor %}
-        }
-        {%- for parameter in operation.query_params %}
-        {%- if not parameter.required %}
-        if {{ varname(parameter.key) }} is not None:
-            params['{{ parameter.orig_key }}'] = {{ varname(parameter.key) }}
+        {%- if operation.request_body %}
+        body: {{ typerepr(operation.request_body.schema) }} | dict[str, Any] | None = None,
         {%- endif %}
-        {%- endfor %}
+
+        {#- headers -#}
+        {% if operation.headers %}
+        headers: {{ classname(operation.fn_name) }}Headers | dict[str, Any] | None = None,
+        {% endif %}
+    ) -> {{ responserepr(operation.responses) }}:
+
+        method = "{{ method }}"
+
+        {% if operation.path_params %}
+        if isinstance(path_params, {{ classname(operation.fn_name) }}PathParams):
+            path = '{{ path }}'.format(**path_params.model_dump(by_alias=True))
+        else:
+            path = '{{ path }}'.format(**path_params)
+        {% else %}
+        path = '{{ path }}'
+        {% endif %}
+        url = f"{self.base_url}{path}"
+
+        {% if operation.query_params %}
+        if isinstance(query_params, {{ classname(operation.fn_name) }}QueryParams):
+            params = query_params.model_dump(by_alias=True, exclude_none=True)
+        else:
+            params = query_params
+        {% else %}
+        params = None
+        {% endif %}
 
         headers_ = self.headers.copy()
 
-        {%- for parameter in operation.headers %}
-        {%- if parameter.required %}
-        headers_['{{ parameter.key }}'] = {{ varname(parameter.key) }}
-        {%- endif  %}
-        {%- endfor %}
-
-        {%- for parameter in operation.headers %}
-        {%- if not parameter.required %}
-        if {{ varname(parameter.key) }} is not None:
-            headers_['{{ parameter.key }}'] = {{ varname(parameter.key) }}
-        {%- endif %}
-        {%- endfor %}
+        {% if operation.headers %}
+        if isinstance(headers, {{ classname(operation.fn_name) }}Headers):
+            headers_ = headers.model_dump(by_alias=True, exclude_none=True)
+        elif isinstance(headers, dict):
+            headers_ = headers
+        {% endif %}
 
         if auth is None:
             auth_ = DEFAULT_AUTH
         elif isinstance(auth, httpx.Auth):
             auth_ = auth
         else:
             auth_ = (auth.username, auth.password)
+
         {% if operation.request_body %}
         if isinstance(body, dict):
             json = body
         elif isinstance(body, {{typerepr(operation.request_body.schema)}}):
             json = body.model_dump(by_alias=True)
         else:
             json = None
@@ -95,38 +84,36 @@
         {%- if operation.request_body and operation.request_body.is_form_data %}
         headers_.update({'Content-Type': 'application/x-www-form-urlencoded'})
         {%- elif operation.request_body and operation.request_body.is_multipart_form_data %}
         # Content-Type=multipart/form-data doesn't work, because header MUST contain boundaries
         # let library do it for us
         headers_.pop("Content-Type", None)
         {% endif %}
-        if headers:
-            headers_ = headers
 
 {%- with req_body=operation.request_body -%}
 {% include 'request-metrics.j2' %}
 {%- endwith %}
+
         req = RequestBox(
             client_name=self.client_name,
-            method="{{ method }}",
+            method=method,
             url=url,
             params=params,
             headers=headers_,
             content=content,
         )
 
         resp = ResponseBox(
             status_code=response.status_code,
         )
 
         {%- for code, mapper in iterresponsemap(operation.responses) %}
 
         if response.status_code == {{ code }}:
             {% if code | int >= 400 -%}
-            method = "{{ method }}"
             if response.content is None:
                 content = None
             else:
                 content = response.content[:500]
 
             if self.logs_integration:
                 self.logs_integration.log_error(req, resp)
```

### Comparing `pythogen-0.2.6/pythogen/templates/http_client/request-metrics.j2` & `pythogen-0.2.7/pythogen/templates/http_client/request-metrics.j2`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
         try:
-            response = {% if not sync %}await {% endif %}self.client.request("{{ method }}", url, {%- if operation.request_body %} {%- if req_body.is_form_data or req_body.is_multipart_form_data %} data{%- else %} json{%- endif %}=json, {%- endif %} headers=headers_, params=params, content=content, auth=auth_{%- if operation.request_body and req_body.is_multipart_form_data %}, files=files{%- endif %})
+            response = {% if not sync %}await {% endif %}self.client.request(method, url, {%- if operation.request_body %} {%- if req_body.is_form_data or req_body.is_multipart_form_data %} data{%- else %} json{%- endif %}=json, {%- endif %} headers=headers_, params=params, content=content, auth=auth_{%- if operation.request_body and req_body.is_multipart_form_data %}, files=files{%- endif %})
         except Exception as exc:
             if self.metrics_integration:
                 if self.metrics_integration.shadow_path():
                     metrics_path = "{{ path | replace('{', ':') | replace('}', '') }}"
                 else:
-                    metrics_path = f"{{ path }}"
-                self.metrics_integration.on_request_error(self.client_name, exc, "{{ method }}", metrics_path)
+                    metrics_path = path
+                self.metrics_integration.on_request_error(self.client_name, exc, method, metrics_path)
 
             raise exc
         {#
             https://www.python-httpx.org/api/#response
             .elapsed - The amount of time elapsed between sending the request
             and calling close() on the corresponding response received for that request.
             total_seconds() to correctly get the total elapsed seconds.
         #}
         if self.metrics_integration:
             if self.metrics_integration.shadow_path():
                 metrics_path = "{{ path | replace('{', ':') | replace('}', '') }}"
             else:
-                metrics_path = f"{{ path }}"
-            self.metrics_integration.on_request_success(self.client_name, response, "{{ method }}",  metrics_path)
+                metrics_path = path
+            self.metrics_integration.on_request_success(self.client_name, response, method,  metrics_path)
```

### Comparing `pythogen-0.2.6/PKG-INFO` & `pythogen-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.6
+Version: 0.2.7
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
```

