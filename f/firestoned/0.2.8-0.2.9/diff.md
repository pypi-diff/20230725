# Comparing `tmp/firestoned-0.2.8.tar.gz` & `tmp/firestoned-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestoned-0.2.8.tar", max compression
+gzip compressed data, was "firestoned-0.2.9.tar", max compression
```

## Comparing `firestoned-0.2.8.tar` & `firestoned-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-28 01:24:07.908996 firestoned-0.2.8/LICENSE
--rw-r--r--   0        0        0     9344 2023-04-28 01:24:07.908996 firestoned-0.2.8/README.md
--rw-r--r--   0        0        0        0 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/__init__.py
--rw-r--r--   0        0        0     4872 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/__main__.py
--rw-r--r--   0        0        0     2045 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/resource.py
--rw-r--r--   0        0        0        0 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/schema/__init__.py
--rw-r--r--   0        0        0      322 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/schema/asyncapi.jinja2
--rw-r--r--   0        0        0     6151 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/schema/main.py.jinja2
--rw-r--r--   0        0        0      408 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/schema/openapi.jinja2
--rw-r--r--   0        0        0     2263 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/schema/resource.yaml
--rw-r--r--   0        0        0      175 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/__init__.py
--rw-r--r--   0        0        0      866 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/_base.py
--rw-r--r--   0        0        0    13390 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/asyncapi.py
--rw-r--r--   0        0        0     9184 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/cli.py
--rw-r--r--   0        0        0    16187 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/openapi.py
--rw-r--r--   0        0        0     1683 2023-04-28 01:24:07.912996 firestoned-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    10593 1970-01-01 00:00:00.000000 firestoned-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 03:33:21.966015 firestoned-0.2.9/LICENSE
+-rw-r--r--   0        0        0     9347 2023-07-25 03:33:21.966015 firestoned-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/__init__.py
+-rw-r--r--   0        0        0     5080 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/__main__.py
+-rw-r--r--   0        0        0     2045 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/resource.py
+-rw-r--r--   0        0        0        0 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/asyncapi.jinja2
+-rw-r--r--   0        0        0     7446 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/main.py.jinja2
+-rw-r--r--   0        0        0      437 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/openapi.jinja2
+-rw-r--r--   0        0        0     2263 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/schema/resource.yaml
+-rw-r--r--   0        0        0      175 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/__init__.py
+-rw-r--r--   0        0        0      866 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/_base.py
+-rw-r--r--   0        0        0    13390 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/asyncapi.py
+-rw-r--r--   0        0        0     9184 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/cli.py
+-rw-r--r--   0        0        0    18840 2023-07-25 03:33:21.970015 firestoned-0.2.9/firestone/spec/openapi.py
+-rw-r--r--   0        0        0     1664 2023-07-25 03:33:21.974015 firestoned-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    10556 1970-01-01 00:00:00.000000 firestoned-0.2.9/PKG-INFO
```

### Comparing `firestoned-0.2.8/LICENSE` & `firestoned-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.8/README.md` & `firestoned-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Last PR Build 🐍](https://github.com/firestoned/firestone/actions/workflows/pr.yml/badge.svg)](https://github.com/firestoned/firestone/actions/workflows/pr.yml)
 <!-- Pytest Coverage Comment:Begin -->
-<a href="https://github.com/firestoned/firestone/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-38%25-red.svg" /></a>
+<a href="https://github.com/firestoned/firestone/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-40%25-orange.svg" /></a>
 <!-- Pytest Coverage Comment:End -->
 
 # Firestone
 
 Resource-Based Approach to Building APIs
 
 ``firestone`` allows you to build OpenAPI, AsyncAPI and gRPC specs based off one or
```

### Comparing `firestoned-0.2.8/firestone/__main__.py` & `firestoned-0.2.9/firestone/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,30 +91,39 @@
 )
 @click.option(
     "--prefix",
     help="A prefix to all URLs, this will add a 'servers' section to the openapi spec doc",
 )
 @click.option(
     "--security",
-    help="Add security scheme to schema; examnple: "
-    '{"name": "bearer_auth", "scheme": "bearer", "type": "http", "bearerFormat": "JWT"}',
+    help=(
+        "Add security scheme to schema; e.g.: "
+        '{"name": "bearer_auth", "scheme": "bearer", "type": "http", "bearerFormat": "JWT"}'
+    ),
     type=firestone_cli.StrDict,
 )
+@click.option(
+    "--version",
+    help="Set the OpenAPI spec version",
+    show_default=True,
+    default=firestone_spec.openapi.DEFAULT_VERSION,
+)
 @click.pass_obj
-def openapi(rsrc_data, output, ui_server, prefix, security):
+def openapi(rsrc_data, output, ui_server, prefix, security, version):
     """Generate an OpenAPI specification for the given resource data."""
 
     openapi_spec = firestone_spec.openapi.generate(
         rsrc_data["data"],
         rsrc_data["title"],
         rsrc_data["desc"],
         rsrc_data["summary"],
         rsrc_data["version"],
         prefix=prefix,
         security=security,
+        openapi_version=version,
     )
     print(openapi_spec, file=output)
 
     if ui_server:
         # pylint: disable=import-outside-toplevel,import-error,no-member
         import quart
         import swagger_ui
```

### Comparing `firestoned-0.2.8/firestone/resource.py` & `firestoned-0.2.9/firestone/resource.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.8/firestone/schema/main.py.jinja2` & `firestoned-0.2.9/firestone/schema/main.py.jinja2`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 from firestone_lib import cli
 from firestone_lib import utils as firestone_utils
 
 from {{ client_pkg }} import api_client
 from {{ client_pkg }} import configuration
 from {{ client_pkg }} import exceptions
 {% for rsrc in rsrcs -%}
+{% set comp_name = rsrc["name"] if not rsrc["name"].endswith("s") else rsrc["name"][:-1] %}
 from {{ client_pkg }}.api import {{ rsrc["name"] }}_api
-from {{ client_pkg }}.models import {{ rsrc["name"] }} as {{ rsrc["name"] }}_model
+from {{ client_pkg }}.models import {{ comp_name }} as {{ comp_name }}_model
+from {{ client_pkg }}.models import create_{{ comp_name }} as create_{{ comp_name }}_model
+from {{ client_pkg }}.models import update_{{ comp_name }} as update_{{ comp_name }}_model
 {% endfor %}
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def api_exc(func):
     """Handle ApiExceptions in all functions."""
@@ -42,35 +45,53 @@
 @click.option(
     "--api-key",
     help="The API key to authorize against API",
     envvar="API_KEY",
 )
 @click.option(
     "--api-url",
-    help="The URL to the API",
-    required=True,
+    help="The API url, e.g. https://localhost",
     envvar="API_URL",
 )
+@click.option(
+    "--client-cert",
+    help="Path to the client cert for mutual TLS",
+    envvar="CLIENT_CERT",
+)
+@click.option(
+    "--client-key",
+    help="Path to the client key for mutual TLS",
+    envvar="CLIENT_KEY",
+)
 @click.option("--trust-proxy", help="Trust the proxy env vars", is_flag=True, default=False)
 @click.option("--threads", help="The number of threads for client side", type=int, default=1)
 @click.pass_context
-def main(ctx, debug, api_key, api_url, threads, trust_proxy):
+def main(ctx, debug, api_key, api_url, client_cert, client_key, threads, trust_proxy):
     """{{ title }}
 
     {{ description }}
     """
     if not trust_proxy:
+        # Convert to loop
         if "http_proxy" in os.environ:
             del os.environ["http_proxy"]
         if "https_proxy" in os.environ:
+            del os.environ["all_https_proxy"]
+        if "all_http_proxy" in os.environ:
+            del os.environ["all_http_proxy"]
+        if "all_https_proxy" in os.environ:
             del os.environ["https_proxy"]
         if "HTTP_PROXY" in os.environ:
             del os.environ["HTTP_PROXY"]
         if "HTTPS_PROXY" in os.environ:
             del os.environ["HTTPS_PROXY"]
+        if "ALL_HTTP_PROXY" in os.environ:
+            del os.environ["ALL_HTTP_PROXY"]
+        if "ALL_HTTPS_PROXY" in os.environ:
+            del os.environ["ALL_HTTPS_PROXY"]
 
     try:
         cli.init_logging("{{ pkg }}.resources.logging", "cli.conf")
     # pylint: disable=broad-except
     except Exception:
         logging.basicConfig(
             level=logging.INFO,
@@ -86,14 +107,18 @@
         logging.getLogger("urllib3").setLevel(logging.DEBUG)
         logging.getLogger("httplib").setLevel(logging.DEBUG)
 
     config = configuration.Configuration(host=api_url)
     config.debug = debug
     if api_key:
         config.access_token = api_key
+    if client_cert:
+        config.cert_file = client_cert
+    if client_key:
+        config.key_file = client_key
     aclient = api_client.ApiClient(configuration=config, pool_threads=threads)
 
     ctx.obj = {
         "api_client": aclient,
     }
     _LOGGER.debug(f"ctx.obj: {ctx.obj}")
 
@@ -121,16 +146,20 @@
     """{{ op["description"] }}"""
     api_obj = ctx_obj["api_obj"]
     params = {
         {% for attr in op["attrs"]|sort(attribute='name') -%}
         "{{ attr["name"] }}":  {{ attr["name"].replace("-", "_") }},
         {% endfor -%}
     }
+    {% set comp_name = rsrc["name"] if not rsrc["name"].endswith("s") else rsrc["name"][:-1] %}
     {% if op["name"] == "create" %}
-    req_body = {{ rsrc["name"] }}_model.{{ rsrc["name"].capitalize() }}(**params)
+    req_body = create_{{ comp_name }}_model.Create{{ comp_name.capitalize() }}(**params)
+    resp = await api_obj.{{ op["id"] }}(req_body)
+    {% elif op["name"] == "update" %}
+    req_body = update_{{ comp_name }}_model.Update{{ comp_name.capitalize() }}(**params)
     resp = await api_obj.{{ op["id"] }}(req_body)
     {% else %}
     resp = await api_obj.{{ op["id"] }}(**params)
     {% endif -%}
     _LOGGER.debug(f"resp: {resp}")
 
     if isinstance(resp, list):
```

### Comparing `firestoned-0.2.8/firestone/schema/resource.yaml` & `firestoned-0.2.9/firestone/schema/resource.yaml`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.8/firestone/spec/_base.py` & `firestoned-0.2.9/firestone/spec/_base.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.8/firestone/spec/asyncapi.py` & `firestoned-0.2.9/firestone/spec/asyncapi.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.8/firestone/spec/cli.py` & `firestoned-0.2.9/firestone/spec/cli.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.8/firestone/spec/openapi.py` & `firestoned-0.2.9/firestone/spec/openapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 # TODO: fix dupe code
 # pylint: disable=duplicate-code
 
 import copy
 import http.client
 import logging
 
-import yaml
-import inflect
-
 from firestone.spec import _base as spec_base
 
+DEFAULT_VERSION = "3.0.0"
+
 # This is a list of all HTTP methods supported on high-level resource base
 RSRC_HTTP_METHODS = ["delete", "get", "head", "patch", "post"]
 
 # This is a list of all HTTP methods supported on an instance of a resource
 RSRC_INST_HTTP_METHODS = ["delete", "get", "head", "patch", "put"]
 
 # This is a list of all HTTP methods supported on attributes of an instance of a resource
 RSRC_ATTR_HTTP_METHODS = ["delete", "get", "head", "put"]
 
-INFLECT_ENGINE = inflect.engine()
-
 _LOGGER = logging.getLogger(__name__)
 
 # TODO add support for JSON Patch: https://www.jvt.me/posts/2022/05/29/openapi-json-patch/
 
 
 def get_responses(
     method: str,
@@ -75,24 +72,34 @@
             "type": "array",
             "items": {"$ref": schema_value},
         }
 
     return responses
 
 
+def _get_comp_name(rsrc_name: str, method: str):
+    comp_name = rsrc_name if not rsrc_name.endswith("s") else rsrc_name[:-1]
+    if method == "post":
+        comp_name = f"Create{comp_name.capitalize()}"
+    if method == "put":
+        comp_name = f"Update{comp_name.capitalize()}"
+
+    return comp_name
+
+
 def get_method_op(
     path: str,
     method: str,
     schema: dict,
     desc: str = None,
     comp_name: str = None,
     attr_name: str = None,
     is_list: bool = None,
 ):
-    """Get the specified method seciton for the paths."""
+    """Get the specified method section for the paths."""
     if not desc:
         desc = f"{method} operation for {path}"
     content_type = spec_base.DEFAULT_CONTENT_TYPE
     opr = {
         "description": desc,
         "operationId": spec_base.get_opid(path, method),
     }
@@ -119,19 +126,20 @@
         if (
             http.client.CREATED in opr["responses"]
             and "$ref" in opr["responses"][http.client.CREATED]["content"][content_type]["schema"]
         ):
             request_schema = opr["responses"][http.client.CREATED]["content"][content_type][
                 "schema"
             ]
-
-        if "descriptions" in request_schema:
-            del request_schema["descriptions"]
     elif method == "put":
+        _LOGGER.debug(f"Getting {method} operation")
         request_schema = copy.deepcopy(schema)
+        if comp_name:
+            request_schema = {"$ref": f"#/components/schemas/{comp_name}"}
+    _LOGGER.debug(f"request_schema: {request_schema}")
 
     if request_schema:
         if "descriptions" in request_schema:
             del request_schema["descriptions"]
         if "key" in request_schema:
             del request_schema["key"]
         if "methods" in request_schema:
@@ -227,23 +235,27 @@
 
     paths[baseurl] = {}
 
     for method in RSRC_HTTP_METHODS:
         if methods and method not in methods:
             _LOGGER.info(
                 f"Skipping the definition of {method} in resource generation, "
-                "as it is not in the defined methods requested"
+                "as it is not defined in methods.resource requested"
             )
             continue
+
+        comp_name = _get_comp_name(rsrc_name, method)
+        _LOGGER.debug(f"comp_name: {comp_name}")
+
         paths[baseurl][method] = get_method_op(
             baseurl,
             method,
             schema,
             desc=descs.get(method),
-            comp_name=rsrc_name,
+            comp_name=comp_name,
             is_list=(method == "get"),
         )
         paths[baseurl][method]["tags"] = [orig_rsrc_name or rsrc_name]
 
         # Add parameters
         params = get_params(baseurl, method, schema, keys=keys)
         if default_query_params:
@@ -273,76 +285,85 @@
     :param dict paths: the paths
     """
     if not descs:
         descs = {}
 
     paths[baseurl] = {}
     for method in RSRC_INST_HTTP_METHODS:
+        _LOGGER.debug(f"baseurl: {baseurl}")
         if methods and method not in methods:
             _LOGGER.info(
                 f"Skipping the definition of {method} in resource instance generation, "
-                "as it is not in the defined methods requested"
+                "as it is not defined in methods.instance requested"
             )
             continue
+
+        comp_name = _get_comp_name(rsrc_name, method)
+        _LOGGER.debug(f"comp_name: {comp_name}")
+
         paths[baseurl][method] = get_method_op(
             baseurl,
             method,
             schema,
             desc=descs.get(method),
-            comp_name=rsrc_name,
+            comp_name=comp_name,
         )
 
         # Add parameters
         params = get_params(baseurl, method, schema, keys=keys)
         _LOGGER.debug(f"params: {params}")
         paths[baseurl][method]["parameters"] = params
 
         # Add tags
         paths[baseurl][method]["tags"] = [orig_rsrc_name or rsrc_name]
         _LOGGER.debug(f"paths[baseurl][{method}]: {paths[baseurl][method]}")
 
 
+# pylint: disable=too-many-locals
 def add_instance_attr_methods(
     rsrc_name: str,
     schema: dict,
     baseurl: str,
     paths: dict,
-    methods: list = None,
+    methods: dict = None,
     keys: list = None,
     default_query_params: dict = None,
     components: dict = None,
     orig_rsrc_name: str = None,
 ):
     """Add the instance attr methods to the paths.
 
     :param str rsrc_name: the resource name
     :param dict schema: the schema for this resource name
     :param str baseurl: the baseurl to use for paths
     :param list keys: the keys for the instance of this resource
     :param dict paths: the paths
     :param dict default_query_params: the paths
     """
+    inst_methods = methods.get("instance_attrs", [])
     for prop in schema["items"]["properties"]:
         path = "/".join([baseurl, prop])
         _LOGGER.debug(f"path: {path}")
         prop_schema = schema["items"]["properties"][prop]
 
         if "expose" in prop_schema and not prop_schema["expose"]:
             continue
 
         paths[path] = {}
         for method in RSRC_ATTR_HTTP_METHODS:
-            if methods and method not in methods:
+            if inst_methods and method not in inst_methods:
                 _LOGGER.info(
                     f"Skipping the definition of {method} in resource instance attribute generation, "
                     "as it is not in the defined methods requested"
                 )
                 continue
+
+            comp_name = rsrc_name if not rsrc_name.endswith("s") else rsrc_name[:-1]
             inst_attr_op = get_method_op(
-                path, method, prop_schema, comp_name=rsrc_name, attr_name=prop
+                path, method, prop_schema, comp_name=comp_name, attr_name=prop
             )
             _LOGGER.debug(f"inst_attr_op: {inst_attr_op}")
 
             paths[path][method] = inst_attr_op
 
             # Add parameters
             params = get_params(baseurl, method, schema, keys=keys)
@@ -351,22 +372,23 @@
 
             # Add tags
             paths[path][method]["tags"] = [orig_rsrc_name or rsrc_name]
             _LOGGER.debug(f"paths[{path}][{method}]: {paths[path][method]}")
 
             # Recursively get paths for this property
             _LOGGER.debug(f"prop: {prop}")
-            _LOGGER.debug(f"components: {yaml.dump(components['schemas'])}")
             if "schema" in prop_schema:
                 if "descriptions" in prop_schema["schema"]:
                     del prop_schema["schema"]["descriptions"]
                 if "descriptions" in prop_schema["schema"]["items"]:
                     del prop_schema["schema"]["items"]["descriptions"]
 
+                components = add_rsrc_components(components, prop, methods, prop_schema["schema"])
                 components["schemas"][prop] = prop_schema["schema"]["items"]
+
                 if (
                     rsrc_name in components["schemas"]
                     and prop in components["schemas"][rsrc_name]["properties"]
                 ):
                     components["schemas"][rsrc_name]["properties"][prop] = {
                         "$ref": f"#/components/schemas/{prop}"
                     }
@@ -445,49 +467,98 @@
 
     # 3. Add attribute path for instance of this resource
     add_instance_attr_methods(
         rsrc_name,
         schema,
         instance_baseurl,
         paths,
-        methods=methods.get("instance_attrs", []),
+        methods=methods,
         keys=keys,
         default_query_params=default_query_params,
         components=components,
         orig_rsrc_name=orig_rsrc_name,
     )
 
     return paths
 
 
+def add_rsrc_components(components: dict, rsrc_name: str, methods: dict, schema: dict):
+    """Get the components for this resource."""
+    comp_name = rsrc_name if not rsrc_name.endswith("s") else rsrc_name[:-1]
+
+    # Reosurce level component, without required
+    comp_schema = copy.deepcopy(schema["items"])
+    if "descriptions" in comp_schema:
+        del comp_schema["descriptions"]
+
+    components["schemas"][comp_name] = comp_schema
+
+    required = schema["items"].get("required", [])
+    if required:
+        del components["schemas"][comp_name]["required"]
+
+    rscr_methods = methods.get("resource", [])
+    rscr_inst_methods = methods.get("instance", [])
+    _LOGGER.debug(f"rscr_methods: {rscr_methods}")
+    _LOGGER.debug(f"rscr_inst_methods: {rscr_inst_methods}")
+
+    # Create resource model
+    if "post" in rscr_methods or "post" in rscr_inst_methods:
+        create_key = f"Create{comp_name.capitalize()}"
+        _LOGGER.info(f"Adding {create_key} to components")
+        components["schemas"][create_key] = {
+            "allOf": [
+                {"$ref": f"#/components/schemas/{comp_name}"},
+                {"type": "object"},
+            ]
+        }
+
+        if required:
+            components["schemas"][create_key]["allOf"][1]["required"] = required
+
+    # Update resource model
+    if "put" in rscr_methods or "put" in rscr_inst_methods:
+        update_key = f"Update{comp_name.capitalize()}"
+        _LOGGER.info(f"Adding {update_key} to components")
+        components["schemas"][update_key] = {
+            "allOf": [
+                {"$ref": f"#/components/schemas/{comp_name}"},
+                {"type": "object"},
+            ]
+        }
+
+    return components
+
+
 # pylint: disable=too-many-locals
 def generate(
     rsrc_data: list,
     title: str,
     desc: str,
     summary: str,
     version: str,
     prefix: str = None,
     security: str = None,
+    openapi_version: str = None,
 ):
     """Generate an OpenAPI spec based ont he resource data sent and other meta data."""
     components = {"schemas": {}}
     all_paths = {}
     for rsrc in rsrc_data:
         rsrc_name = rsrc["name"]
         baseurl = "/"
         if "version_in_path" in rsrc and rsrc["version_in_path"]:
             baseurl += f"v{rsrc['version']}/"
         baseurl += rsrc_name
         _LOGGER.debug(f"baseurl: {baseurl}")
 
         # Extract and set high-level resource component schema
-        rschema = rsrc["schema"]
-        comp_schema = copy.deepcopy(rschema["items"])
-        components["schemas"][rsrc_name] = comp_schema
+        methods = rsrc.get("methods", {})
+        components = add_rsrc_components(components, rsrc_name, methods, rsrc["schema"])
+        _LOGGER.debug(f"components: {components['schemas']}")
 
         default_query_params = rsrc.get("default_query_params", [])
         _LOGGER.debug(f"default_query_params: {default_query_params}")
 
         paths = get_paths(
             rsrc["name"],
             rsrc,
@@ -518,8 +589,9 @@
         summary=summary,
         description=desc,
         version=version,
         components=components,
         paths=all_paths,
         servers=servers,
         security_name=security_name,
+        openapi_version=openapi_version,
     )
```

### Comparing `firestoned-0.2.8/pyproject.toml` & `firestoned-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestoned"
-version = "0.2.8"
+version = "0.2.9"
 description = "Build OpenAPI and AsyncAPI specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/firestoned/firestone"
 packages = [
     { include = "firestone" }
@@ -19,15 +19,14 @@
 jsonschema = "^4.16.0"
 pyyaml = "^6.0"
 jsonref = "^1.0.0.post1"
 firestone-lib = "^0.1.0"
 pydantic = "^1.10.5"
 python-dateutil = "^2.8.2"
 aiohttp = "^3.8.4"
-inflect = "^6.0.4"
 
 [tool.poetry.group.asyncapi.dependencies]
 asyncapi = {extras = ["http"], version = "^0.14.1"}
 requests = "^2.28.1"
 websockets = "^10.4"
 typer = "^0.7.0"
 uvicorn = "^0.19.0"
```

### Comparing `firestoned-0.2.8/PKG-INFO` & `firestoned-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestoned
-Version: 0.2.8
+Version: 0.2.9
 Summary: Build OpenAPI and AsyncAPI specs based off one or more resource json schema files
 Home-page: https://github.com/firestoned/firestone
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -14,28 +14,27 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: caching
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: firestone-lib (>=0.1.0,<0.2.0)
-Requires-Dist: inflect (>=6.0.4,<7.0.0)
 Requires-Dist: jsonref (>=1.0.0.post1,<2.0.0)
 Requires-Dist: jsonschema (>=4.16.0,<5.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: quart (>=0.18.3,<0.19.0) ; extra == "caching"
 Requires-Dist: setuptools (>=65.5.0,<66.0.0)
 Project-URL: Repository, https://github.com/firestoned/firestone
 Description-Content-Type: text/markdown
 
 [![Last PR Build 🐍](https://github.com/firestoned/firestone/actions/workflows/pr.yml/badge.svg)](https://github.com/firestoned/firestone/actions/workflows/pr.yml)
 <!-- Pytest Coverage Comment:Begin -->
-<a href="https://github.com/firestoned/firestone/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-38%25-red.svg" /></a>
+<a href="https://github.com/firestoned/firestone/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-40%25-orange.svg" /></a>
 <!-- Pytest Coverage Comment:End -->
 
 # Firestone
 
 Resource-Based Approach to Building APIs
 
 ``firestone`` allows you to build OpenAPI, AsyncAPI and gRPC specs based off one or
```

#### html2text {}

```diff
@@ -1,130 +1,129 @@
-Metadata-Version: 2.1 Name: firestoned Version: 0.2.8 Summary: Build OpenAPI
+Metadata-Version: 2.1 Name: firestoned Version: 0.2.9 Summary: Build OpenAPI
 and AsyncAPI specs based off one or more resource json schema files Home-page:
 https://github.com/firestoned/firestone License: Apache 2.0 Author: Erick
 Bourgeois Author-email: erick@jeb.ca Requires-Python: >=3.8,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: caching
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: firestone-lib
-(>=0.1.0,<0.2.0) Requires-Dist: inflect (>=6.0.4,<7.0.0) Requires-Dist: jsonref
-(>=1.0.0.post1,<2.0.0) Requires-Dist: jsonschema (>=4.16.0,<5.0.0) Requires-
-Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist: python-dateutil
-(>=2.8.2,<3.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: quart
-(>=0.18.3,<0.19.0) ; extra == "caching" Requires-Dist: setuptools
-(>=65.5.0,<66.0.0) Project-URL: Repository, https://github.com/firestoned/
-firestone Description-Content-Type: text/markdown [![Last PR Build ð](https:
-//github.com/firestoned/firestone/actions/workflows/pr.yml/badge.svg)](https://
-github.com/firestoned/firestone/actions/workflows/pr.yml)  [Coverage]  #
-Firestone Resource-Based Approach to Building APIs ``firestone`` allows you to
-build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json
-schema files. This allows you to focus on what really matters, the resource you
-are developing! Once you have generated the appropriate specification file for
-your project, you can then use the myriad of libraries and frameworks to
-generate stub code for you. **The primary premise of this project is not to
-introduce any new "language" to describe your resources(s), use JSON Schema!**
-THis makes it easy to come up to speed and little to no prior knowledge to get
-going. Having said that, the schema for a resource provides additional helpful
-functionality, see [schema](#schema) section. ## Quick Start You can use pip or
-poetry to install and run ``firestone``. We suggest using pip if you wish to
-install `firestone`` machine-wide, else, for local use, use poetry. ### pip
-It's a simple as running the following ``pip`` command: ``` sudo pip install
-firestoned ``` NOTE: yes, `firestone**d**`, not `firestone`! This is because
-there already is a, albeit emtpy, repo on pypi.org with the same name... ###
-poetry [Poetry](https://python-poetry.org/) is a great build tool for python
-that allows you to build and run all locally in a virtual environment. This is
-great for checking out the tool and playing around with `firestone` itself. ```
-brew install poetry poetry install poetry build ``` ## Running Now that you
-have a copy of ``firestone``, let's try running it with the example resource
-provided, an addressbook! Note: if running within poetry build, simply prepend
-commands with ``poetry run`` For the remainder of this documentation, we will
-assume you have installed firestone. ### Generate an OpenAPI Spec ``` firestone
-\ generate \ --title 'Addressbook resource' \ --description 'A simple
-addressBook example' \ --resources examples/addressBook/resource.yaml \ openapi
---security '{"name": "bearer_auth", "scheme": "bearer", "type": "http",
-"bearerFormat": "JWT"}' \ ``` Let's quickly dissect this command: - we are
-telling firestone to generate an `openapi` spec, given the ``title``,
-``description`` and the two given resource files. - By default, this will
-output the specification file to stdout, alternatively you can provide the `-O`
-option to output to a specific file. You can also, add the command line `--ui-
-server` tot he end, which will launch a small webserver and run the Swagger UI
-to view this specification file. ``` firestone --debug generate --title
-'Example person and addressBook API' \ --description 'An example API with more
-than one resource' \ --resources examples/addressBook.yaml,examples/person.yaml
-\ openapi \ --security '{"name": "bearer_auth", "scheme": "bearer", "type":
-"http", "bearerFormat": "JWT"}' \ --ui-server # ... * Serving Quart app
-'firestone.__main__' * Environment: production * Please use an ASGI server
-(e.g. Hypercorn) directly in production * Debug mode: False * Running on http:/
-/127.0.0.1:5000 (CTRL + C to quit) [2022-10-31 02:47:17 -0500] [87590] [INFO]
-Running on http://127.0.0.1:5000 (CTRL + C to quit) # 2022-10-31 02:47:17,120 -
-[MainThread] hypercorn.error:102 INFO - Running on http://127.0.0.1:5000 (CTRL
-+ C to quit) ``` Now you can use your browser to navigate to `http://127.0.0.1:
-5000/apidocs` ## Schema It all begins with your resource definition! This is
-done using JSON schema and we have provided an example in our `examples`
-directory, called addressBook. We will use this to describe how the schema is
-setup and how you can adapt to your own. Here is the full file: ```yaml name:
-addressBook description: An example of an addressBook resource version: 1.0
-version_in_path: false default_query_params: - name: limit description: Limit
-the number of responses back in: params schema: type: integer - name: offset
-description: The offset to start returning resources in: params schema: type:
-integer descriptions: resource: get: List all addresses in this addressbook.
-head: Determine the existence and size of addresses in this addressbook. patch:
-Patch one or more addresses in this addressbook. post: Create a new address in
-this addressbook, a new address key will be created. delete: Delete all
-addresses from this addressbook. instance: get: Get a specific address from
-this addressbook. head: Determine the existence and size of this address.
-patch: Patch this address in the addressbook. put: Put a new address in this
-addressbook, with the given address key. delete: Delete an address from this
-addressbook. schema: type: array key: name: address_key schema: description: A
-unique identifier for an addressbook entry. type: string #responseCodes: # -
-200 # - 201 query_params: - name: city description: Filter by city name schema:
-type: string methods: - get items: type: object properties: addrtype:
-description: The address type, e.g. work or home type: string enum: - work -
-home street: description: The street and civic number of this address type:
-string city: description: The city of this address type: string state:
-description: The state of this address type: string country: description: The
-country of this address type: string ``` ### Metadata There is a certain amount
-of metadata that all of these specifications use/require, and this is done at
-the top of the resource,yaml; for posterity, they are: ```yaml name:
-addressBook description: An example of an addressBook resource version: 1.0 ```
-#### `name` The name is used in various places, including as the root to API
-URLs, for example in OpenAPI, `/addressBook` #### `description` This is self
-evident, I hope, the description of this resource and is used nt he generated
-specification files. #### `descriptions` This is a map/dict of either
-`resource` and/or `instance`, which itself is a map or methods to descriptions,
-e.g.: ```yaml descriptions: resource: get: List all addresses in this
-addressbook. head: Determine the existence and size of addresses in this
-addressbook. patch: Patch one or more addresses in this addressbook. post:
-Create a new address in this addressbook, a new address key will be created.
-delete: Delete all addresses from this addressbook. ``` #### `methods` This is
-a map/dict of `resource`, and/or `instance`, and/or `instance_attrs` (the
-instance attributes to expose), and a list of methods to explicitly expose,
-e.g.: ```yaml methods: resource: - get - post - put ``` #### `version` The
-version of this resource definition, this cna alternatively be used in the URL
-as well, see below `version_in_path` #### `version_in_path` This attribute
-defines whether to prepend the version defined above in the URL paths, e.g.,
-for the above, you would get: `/v1.0/addressBook`. #### `default_query_params`
-You can provide a list of default query parameters that will be added to all
-HTTP methods, or optionally you can provide a list of the HTTP methods, for
-which `firestone` will add. ### Generate OpenAPI Client Now, to generate your
-OpenAPI client, you will need the `openapi-generator` command, and this can be
-used to generate client code in many languages. For more details on this
-project, see [here](https://openapi-generator.tech/). This client code can then
-be used as an SDK or used by our CLI generation, see below. ``` openapi-
-generator generate \ -i examples/addressbook/openapi.yaml \ -g python-nextgen \
--o /tmp/addressbook-client \ --skip-validate-spec \ -c examples/addressbook/
-openapi-gen-config.json ``` ### Generate Python CRUD CLI Now that you have
-generated the client code, you can also generate a CRUD, Python Click-based CLI
-around your code. This generator creates a standalone script or as a module to
-be used in your console scripts, as part of your project build. Here is an
-example command we use to generate the example Addressbook. ``` firestone
-generate \ --title 'Addressbook CLI' \ --description 'This is the CLI for the
-example Addressbook' \ --resources examples/addressbook/
-addressbook.yaml,examples/addressbook/person.yaml \ --version 1.0 \ cli \ --pkg
-addressbook \ --client-pkg addressbook.client > examples/addressbook/main.py
+(>=0.1.0,<0.2.0) Requires-Dist: jsonref (>=1.0.0.post1,<2.0.0) Requires-Dist:
+jsonschema (>=4.16.0,<5.0.0) Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: pyyaml
+(>=6.0,<7.0) Requires-Dist: quart (>=0.18.3,<0.19.0) ; extra == "caching"
+Requires-Dist: setuptools (>=65.5.0,<66.0.0) Project-URL: Repository, https://
+github.com/firestoned/firestone Description-Content-Type: text/markdown [![Last
+PR Build ð](https://github.com/firestoned/firestone/actions/workflows/
+pr.yml/badge.svg)](https://github.com/firestoned/firestone/actions/workflows/
+pr.yml)  [Coverage]  # Firestone Resource-Based Approach to Building APIs
+``firestone`` allows you to build OpenAPI, AsyncAPI and gRPC specs based off
+one or more resource json schema files. This allows you to focus on what really
+matters, the resource you are developing! Once you have generated the
+appropriate specification file for your project, you can then use the myriad of
+libraries and frameworks to generate stub code for you. **The primary premise
+of this project is not to introduce any new "language" to describe your
+resources(s), use JSON Schema!** THis makes it easy to come up to speed and
+little to no prior knowledge to get going. Having said that, the schema for a
+resource provides additional helpful functionality, see [schema](#schema)
+section. ## Quick Start You can use pip or poetry to install and run
+``firestone``. We suggest using pip if you wish to install `firestone``
+machine-wide, else, for local use, use poetry. ### pip It's a simple as running
+the following ``pip`` command: ``` sudo pip install firestoned ``` NOTE: yes,
+`firestone**d**`, not `firestone`! This is because there already is a, albeit
+emtpy, repo on pypi.org with the same name... ### poetry [Poetry](https://
+python-poetry.org/) is a great build tool for python that allows you to build
+and run all locally in a virtual environment. This is great for checking out
+the tool and playing around with `firestone` itself. ``` brew install poetry
+poetry install poetry build ``` ## Running Now that you have a copy of
+``firestone``, let's try running it with the example resource provided, an
+addressbook! Note: if running within poetry build, simply prepend commands with
+``poetry run`` For the remainder of this documentation, we will assume you have
+installed firestone. ### Generate an OpenAPI Spec ``` firestone \ generate \ --
+title 'Addressbook resource' \ --description 'A simple addressBook example' \ -
+-resources examples/addressBook/resource.yaml \ openapi --security '{"name":
+"bearer_auth", "scheme": "bearer", "type": "http", "bearerFormat": "JWT"}' \
 ``` Let's quickly dissect this command: - we are telling firestone to generate
 an `openapi` spec, given the ``title``, ``description`` and the two given
 resource files. - By default, this will output the specification file to
 stdout, alternatively you can provide the `-O` option to output to a specific
-file. ## Contributing
+file. You can also, add the command line `--ui-server` tot he end, which will
+launch a small webserver and run the Swagger UI to view this specification
+file. ``` firestone --debug generate --title 'Example person and addressBook
+API' \ --description 'An example API with more than one resource' \ --resources
+examples/addressBook.yaml,examples/person.yaml \ openapi \ --security '{"name":
+"bearer_auth", "scheme": "bearer", "type": "http", "bearerFormat": "JWT"}' \ --
+ui-server # ... * Serving Quart app 'firestone.__main__' * Environment:
+production * Please use an ASGI server (e.g. Hypercorn) directly in production
+* Debug mode: False * Running on http://127.0.0.1:5000 (CTRL + C to quit)
+[2022-10-31 02:47:17 -0500] [87590] [INFO] Running on http://127.0.0.1:5000
+(CTRL + C to quit) # 2022-10-31 02:47:17,120 - [MainThread] hypercorn.error:102
+INFO - Running on http://127.0.0.1:5000 (CTRL + C to quit) ``` Now you can use
+your browser to navigate to `http://127.0.0.1:5000/apidocs` ## Schema It all
+begins with your resource definition! This is done using JSON schema and we
+have provided an example in our `examples` directory, called addressBook. We
+will use this to describe how the schema is setup and how you can adapt to your
+own. Here is the full file: ```yaml name: addressBook description: An example
+of an addressBook resource version: 1.0 version_in_path: false
+default_query_params: - name: limit description: Limit the number of responses
+back in: params schema: type: integer - name: offset description: The offset to
+start returning resources in: params schema: type: integer descriptions:
+resource: get: List all addresses in this addressbook. head: Determine the
+existence and size of addresses in this addressbook. patch: Patch one or more
+addresses in this addressbook. post: Create a new address in this addressbook,
+a new address key will be created. delete: Delete all addresses from this
+addressbook. instance: get: Get a specific address from this addressbook. head:
+Determine the existence and size of this address. patch: Patch this address in
+the addressbook. put: Put a new address in this addressbook, with the given
+address key. delete: Delete an address from this addressbook. schema: type:
+array key: name: address_key schema: description: A unique identifier for an
+addressbook entry. type: string #responseCodes: # - 200 # - 201 query_params: -
+name: city description: Filter by city name schema: type: string methods: - get
+items: type: object properties: addrtype: description: The address type, e.g.
+work or home type: string enum: - work - home street: description: The street
+and civic number of this address type: string city: description: The city of
+this address type: string state: description: The state of this address type:
+string country: description: The country of this address type: string ``` ###
+Metadata There is a certain amount of metadata that all of these specifications
+use/require, and this is done at the top of the resource,yaml; for posterity,
+they are: ```yaml name: addressBook description: An example of an addressBook
+resource version: 1.0 ``` #### `name` The name is used in various places,
+including as the root to API URLs, for example in OpenAPI, `/addressBook` ####
+`description` This is self evident, I hope, the description of this resource
+and is used nt he generated specification files. #### `descriptions` This is a
+map/dict of either `resource` and/or `instance`, which itself is a map or
+methods to descriptions, e.g.: ```yaml descriptions: resource: get: List all
+addresses in this addressbook. head: Determine the existence and size of
+addresses in this addressbook. patch: Patch one or more addresses in this
+addressbook. post: Create a new address in this addressbook, a new address key
+will be created. delete: Delete all addresses from this addressbook. ``` ####
+`methods` This is a map/dict of `resource`, and/or `instance`, and/or
+`instance_attrs` (the instance attributes to expose), and a list of methods to
+explicitly expose, e.g.: ```yaml methods: resource: - get - post - put ``` ####
+`version` The version of this resource definition, this cna alternatively be
+used in the URL as well, see below `version_in_path` #### `version_in_path`
+This attribute defines whether to prepend the version defined above in the URL
+paths, e.g., for the above, you would get: `/v1.0/addressBook`. ####
+`default_query_params` You can provide a list of default query parameters that
+will be added to all HTTP methods, or optionally you can provide a list of the
+HTTP methods, for which `firestone` will add. ### Generate OpenAPI Client Now,
+to generate your OpenAPI client, you will need the `openapi-generator` command,
+and this can be used to generate client code in many languages. For more
+details on this project, see [here](https://openapi-generator.tech/). This
+client code can then be used as an SDK or used by our CLI generation, see
+below. ``` openapi-generator generate \ -i examples/addressbook/openapi.yaml \
+-g python-nextgen \ -o /tmp/addressbook-client \ --skip-validate-spec \ -
+c examples/addressbook/openapi-gen-config.json ``` ### Generate Python CRUD CLI
+Now that you have generated the client code, you can also generate a CRUD,
+Python Click-based CLI around your code. This generator creates a standalone
+script or as a module to be used in your console scripts, as part of your
+project build. Here is an example command we use to generate the example
+Addressbook. ``` firestone generate \ --title 'Addressbook CLI' \ --description
+'This is the CLI for the example Addressbook' \ --resources examples/
+addressbook/addressbook.yaml,examples/addressbook/person.yaml \ --version 1.0 \
+cli \ --pkg addressbook \ --client-pkg addressbook.client > examples/
+addressbook/main.py ``` Let's quickly dissect this command: - we are telling
+firestone to generate an `openapi` spec, given the ``title``, ``description``
+and the two given resource files. - By default, this will output the
+specification file to stdout, alternatively you can provide the `-O` option to
+output to a specific file. ## Contributing
```

