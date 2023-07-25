# Comparing `tmp/aiohttp_deps-0.2.1.tar.gz` & `tmp/aiohttp_deps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_deps-0.2.1.tar", max compression
+gzip compressed data, was "aiohttp_deps-0.3.0.tar", max compression
```

## Comparing `aiohttp_deps-0.2.1.tar` & `aiohttp_deps-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/LICENSE
--rw-r--r--   0        0        0     8540 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/README.md
--rw-r--r--   0        0        0      497 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/initializer.py
--rw-r--r--   0        0        0        0 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/py.typed
--rw-r--r--   0        0        0     1250 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/router.py
--rw-r--r--   0        0        0      898 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/router.pyi
--rw-r--r--   0        0        0     9363 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/swagger.py
--rw-r--r--   0        0        0     9138 2023-06-22 13:26:41.632729 aiohttp_deps-0.2.1/aiohttp_deps/utils.py
--rw-r--r--   0        0        0     1385 2023-06-22 13:26:41.636729 aiohttp_deps-0.2.1/aiohttp_deps/view.py
--rw-r--r--   0        0        0     1763 2023-06-22 13:26:41.636729 aiohttp_deps-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9652 1970-01-01 00:00:00.000000 aiohttp_deps-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9687 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/README.md
+-rw-r--r--   0        0        0      539 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/__init__.py
+-rw-r--r--   0        0        0     3265 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/initializer.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/py.typed
+-rw-r--r--   0        0        0     1250 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/router.py
+-rw-r--r--   0        0        0      898 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/router.pyi
+-rw-r--r--   0        0        0    11067 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/swagger.py
+-rw-r--r--   0        0        0    10950 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/utils.py
+-rw-r--r--   0        0        0     1385 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/view.py
+-rw-r--r--   0        0        0     1784 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10841 1970-01-01 00:00:00.000000 aiohttp_deps-0.3.0/PKG-INFO
```

### Comparing `aiohttp_deps-0.2.1/LICENSE` & `aiohttp_deps-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.1/README.md` & `aiohttp_deps-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,29 +65,71 @@
 main_router.add_routes(memes_router, prefix="/memes")
 ```
 
 ## Swagger
 
 If you use dependencies in you handlers, we can easily generate swagger for you.
 We have some limitations:
-1. We don't support string type annotation for detecting required parameters in openapi. Like `a: "Optional[int]"`.
-2. We don't have support for 3.10 style Option annotations. E.G. `int | None`
+1. We don't support resolving type aliases if hint is a string.
+    If you define variable like this: `myvar = int | None` and then in handler
+    you'd create annotation like this: `param: "str | myvar"` it will fail.
+    You need to unquote type hint in order to get it work.
 
 We will try to fix these limitations later.
 
 To enable swagger, just add it to your startup.
 
 ```python
 from aiohttp_deps import init, setup_swagger
 
 app = web.Application()
 
 app.on_startup.extend([init, setup_swagger()])
 ```
 
+### Responses
+
+You can define schema for responses using dataclasses or
+pydantic models. This would not affect handlers in any way,
+it's only for documentation purposes, if you want to actually
+validate values your handler returns, please write your own wrapper.
+
+```python
+from dataclasses import dataclass
+
+from aiohttp import web
+from pydantic import BaseModel
+
+from aiohttp_deps import Router, openapi_response
+
+router = Router()
+
+
+@dataclass
+class Success:
+    data: str
+
+
+class Unauthorized(BaseModel):
+    why: str
+
+
+@router.get("/")
+@openapi_response(200, Success, content_type="application/xml")
+@openapi_response(200, Success)
+@openapi_response(401, Unauthorized, description="When token is not correct")
+async def handler() -> web.Response:
+    ...
+```
+
+This example illustrates how much you can do with this decorator. You
+can have multiple content-types for a single status, or you can have different
+possble statuses. This function is pretty simple and if you want to make
+your own decorator for your responses, it won't be hard.
+
 
 ## Default dependencies
 
 By default this library provides only two injectables. `web.Request` and `web.Application`.
 
 ```python
 
@@ -150,29 +192,29 @@
 
 class UserInfo(BaseModel):
     name: str
 
 
 @router.post("/users")
 async def new_data(user: UserInfo = Depends(Json())):
-    return web.json_response({"user": user.dict()})
+    return web.json_response({"user": user.model_dump()})
 
 ```
 
 This dependency automatically validates data and send
 errors if the data doesn't orrelate with schema or body is not a valid json.
 
 If you want to make this data optional, just mark it as optional.
 
 ```python
 @router.post("/users")
 async def new_data(user: Optional[UserInfo] = Depends(Json())):
     if user is None:
         return web.json_response({"user": None})
-    return web.json_response({"user": user.dict()})
+    return web.json_response({"user": user.model_dump()})
 
 ```
 
 ## Headers
 
 You can get and validate headers using `Header` dependency.
 
@@ -271,27 +313,26 @@
 ## Forms
 
 Now you can easiy get and validate form data from your request.
 To make the magic happen, please add `arbitrary_types_allowed` to the config of your model.
 
 
 ```python
-from pydantic import BaseModel
+import pydantic
 from aiohttp_deps import Router, Depends, Form
 from aiohttp import web
 
 router = Router()
 
 
-class MyForm(BaseModel):
+class MyForm(pydantic.BaseModel):
     id: int
     file: web.FileField
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
 
 
 @router.post("/")
 async def handler(my_form: MyForm = Depends(Form())):
     with open("my_file", "wb") as f:
         f.write(my_form.file.file.read())
     return web.json_response({"id": my_form.id})
```

### Comparing `aiohttp_deps-0.2.1/aiohttp_deps/initializer.py` & `aiohttp_deps-0.3.0/aiohttp_deps/initializer.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.1/aiohttp_deps/router.py` & `aiohttp_deps-0.3.0/aiohttp_deps/router.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.1/aiohttp_deps/router.pyi` & `aiohttp_deps-0.3.0/aiohttp_deps/router.pyi`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.1/aiohttp_deps/swagger.py` & `aiohttp_deps-0.3.0/aiohttp_deps/swagger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import inspect
 from collections import defaultdict
 from logging import getLogger
-from typing import Any, Awaitable, Callable, Dict, Optional, Union
+from typing import Any, Awaitable, Callable, Dict, Optional, TypeVar, get_type_hints
 
+import pydantic
 from aiohttp import web
-from pydantic import schema_of
-from pydantic.utils import deep_update
+from deepmerge import always_merger
 from taskiq_dependencies import DependencyGraph
 
 from aiohttp_deps.initializer import InjectableFuncHandler, InjectableViewHandler
 from aiohttp_deps.utils import Form, Header, Json, Path, Query
 
-REF_TEMPLATE = "#/components/schemas/{model}"
+_T = TypeVar("_T")  # noqa: WPS111
+
 SCHEMA_KEY = "openapi_schema"
 SWAGGER_HTML_TEMPALTE = """
 <html lang="en">
 
 <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
@@ -63,95 +64,104 @@
 
 def _is_optional(annotation: Optional[inspect.Parameter]) -> bool:
     # If it's an empty annotation,
     # we guess that the value can be optional.
     if annotation is None or annotation.annotation == annotation.empty:
         return True
 
-    origin = getattr(annotation.annotation, "__origin__", None)
-    if origin is None:
-        return False
-
-    if origin == Union:
-        args = getattr(annotation.annotation, "__args__", ())
-        for arg in args:
-            if arg is type(None):  # noqa: E721, WPS516
-                return True
-    return False
+    def dummy(_var: annotation.annotation) -> None:  # type: ignore
+        """Dummy function to use for type resolution."""
+
+    var = get_type_hints(dummy).get("_var")
+    return var == Optional[var]
 
 
-def _add_route_def(  # noqa: C901
+def _add_route_def(  # noqa: C901, WPS210
     openapi_schema: Dict[str, Any],
     route: web.ResourceRoute,
     method: str,
     graph: DependencyGraph,
     extra_openapi: Dict[str, Any],
 ) -> None:
     route_info: Dict[str, Any] = {
         "description": inspect.getdoc(graph.target),
         "responses": {},
         "parameters": [],
     }
     if route.resource is None:  # pragma: no cover
         return
 
+    params: Dict[tuple[str, str], Any] = {}
+
+    def _insert_in_params(data: Dict[str, Any]) -> None:
+        element = params.get((data["name"], data["in"]))
+        if element is None:
+            params[(data["name"], data["in"])] = data
+            return
+        element["required"] = element.get("required") or data.get("required")
+        element["allowEmptyValue"] = bool(element.get("allowEmptyValue")) and bool(
+            data.get("allowEmptyValue"),
+        )
+        params[(data["name"], data["in"])] = element
+
     for dependency in graph.ordered_deps:
         if isinstance(dependency.dependency, (Json, Form)):
             content_type = "application/json"
             if isinstance(dependency.dependency, Form):
                 content_type = "application/x-www-form-urlencoded"
             if (
                 dependency.signature
                 and dependency.signature.annotation != inspect.Parameter.empty
             ):
-                input_schema = schema_of(
+                input_schema = pydantic.TypeAdapter(
                     dependency.signature.annotation,
-                    ref_template=REF_TEMPLATE,
-                )
+                ).json_schema()
                 openapi_schema["components"]["schemas"].update(
                     input_schema.pop("definitions", {}),
                 )
                 route_info["requestBody"] = {
                     "content": {content_type: {"schema": input_schema}},
                 }
             else:
                 route_info["requestBody"] = {
                     "content": {content_type: {}},
                 }
         elif isinstance(dependency.dependency, Query):
-            route_info["parameters"].append(
+            _insert_in_params(
                 {
                     "name": dependency.dependency.alias or dependency.param_name,
                     "in": "query",
                     "description": dependency.dependency.description,
                     "required": not _is_optional(dependency.signature),
                 },
             )
         elif isinstance(dependency.dependency, Header):
-            route_info["parameters"].append(
+            name = dependency.dependency.alias or dependency.param_name
+            _insert_in_params(
                 {
-                    "name": dependency.dependency.alias or dependency.param_name,
+                    "name": name.capitalize(),
                     "in": "header",
                     "description": dependency.dependency.description,
                     "required": not _is_optional(dependency.signature),
                 },
             )
         elif isinstance(dependency.dependency, Path):
-            route_info["parameters"].append(
+            _insert_in_params(
                 {
                     "name": dependency.dependency.alias or dependency.param_name,
                     "in": "path",
                     "description": dependency.dependency.description,
                     "required": not _is_optional(dependency.signature),
                     "allowEmptyValue": _is_optional(dependency.signature),
                 },
             )
 
+    route_info["parameters"] = list(params.values())
     openapi_schema["paths"][route.resource.canonical].update(
-        {method.lower(): deep_update(route_info, extra_openapi)},
+        {method.lower(): always_merger.merge(route_info, extra_openapi)},
     )
 
 
 def setup_swagger(  # noqa: C901, WPS211
     schema_url: str = "/openapi.json",
     swagger_ui_url: str = "/docs",
     enable_ui: bool = True,
@@ -260,23 +270,61 @@
                     SWAGGER_HTML_TEMPALTE.replace("{schema_url}", schema_url),
                 ),
             )
 
     return event_handler
 
 
-def extra_openapi(additional_schema: Dict[str, Any]) -> Callable[..., Any]:
+def extra_openapi(additional_schema: Dict[str, Any]) -> Callable[[_T], _T]:
     """
     Add extra openapi schema.
 
     This function just adds a parameter for later use
     by openapi schema generator.
 
     :param additional_schema: dict with updates.
     :return: same function with new attributes.
     """
 
-    def decorator(func: Any) -> Any:
-        func.__extra_openapi__ = additional_schema
+    def decorator(func: _T) -> _T:
+        func.__extra_openapi__ = additional_schema  # type: ignore
+        return func
+
+    return decorator
+
+
+def openapi_response(
+    status: int,
+    model: Any,
+    *,
+    content_type: str = "application/json",
+    description: Optional[str] = None,
+) -> Callable[[_T], _T]:
+    """
+    Add response schema to the endpoint.
+
+    This function takes a status and model,
+    which is going to represent the response.
+
+    :param status: Status of a response.
+    :param model: Response model.
+    :param content_type: Content-type of a response.
+    :param description: Response's description.
+
+    :returns: decorator that modifies your function.
+    """
+
+    def decorator(func: _T) -> _T:
+        openapi = getattr(func, "__extra_openapi__", {})
+        adapter: "pydantic.TypeAdapter[Any]" = pydantic.TypeAdapter(model)
+        responses = openapi.get("responses", {})
+        status_response = responses.get(status, {})
+        if not status_response:
+            status_response["description"] = description
+        status_response["content"] = status_response.get("content", {})
+        status_response["content"][content_type] = {"schema": adapter.json_schema()}
+        responses[status] = status_response
+        openapi["responses"] = responses
+        func.__extra_openapi__ = openapi  # type: ignore
         return func
 
     return decorator
```

### Comparing `aiohttp_deps-0.2.1/aiohttp_deps/utils.py` & `aiohttp_deps-0.3.0/aiohttp_deps/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 import json
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 import pydantic
 from aiohttp import web
 from taskiq_dependencies import Depends, ParamInfo
 
 
 class Header:
@@ -28,16 +28,18 @@
         multiple: bool = False,
         description: str = "",
     ):
         self.default = default
         self.alias = alias
         self.multiple = multiple
         self.description = description
+        self.type_initialized = False
+        self.type_cache: "Union[pydantic.TypeAdapter[Any], None]" = None
 
-    def __call__(  # noqa: C901, WPS210
+    def __call__(  # noqa: C901
         self,
         param_info: ParamInfo = Depends(),
         request: web.Request = Depends(),
     ) -> Any:
         """
         Performs actual logic, described above.
 
@@ -48,52 +50,60 @@
         :return: parsed data.
         """
         header_name = self.alias or param_info.name
         default_value = None
         if self.default is not ...:
             default_value = self.default
 
+        if not self.type_initialized:
+            if (
+                param_info.definition
+                and param_info.definition.annotation != inspect.Parameter.empty
+            ):
+                self.type_cache = pydantic.TypeAdapter(param_info.definition.annotation)
+            else:
+                self.type_cache = None
+            self.type_initialized = True
+
         if self.multiple:
             value = request.headers.getall(header_name, default_value)
         else:
             value = request.headers.getone(header_name, default_value)
 
-        definition = None
-        if (
-            param_info.definition
-            and param_info.definition.annotation != inspect.Parameter.empty
-        ):
-            definition = param_info.definition.annotation
-
-        if definition is None:
+        if self.type_cache is None:
             return value
 
         try:
-            return pydantic.parse_obj_as(definition, value)
+            return self.type_cache.validate_python(value)
         except pydantic.ValidationError as err:
-            errors = err.errors()
+            errors = err.errors(include_url=False)
             for error in errors:
                 error["loc"] = (
                     "header",
                     header_name,
                 ) + error["loc"]
+                error.pop("input", None)  # type: ignore
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
 
 
 class Json:
     """
     Get and parse the body as json.
 
     This dependency, gets body, tries to parse it as json,
     and then converts it to type from your typehints.
     """
 
+    def __init__(self) -> None:
+        self.type_initialized = False
+        self.type_cache: "Union[pydantic.TypeAdapter[Any], None]" = None
+
     async def __call__(  # noqa: C901
         self,
         param_info: ParamInfo = Depends(),
         request: web.Request = Depends(),
     ) -> Any:
         """
         Performs actual logic, described above.
@@ -105,30 +115,34 @@
         :return: parsed data.
         """
         try:
             body = await request.json()
         except ValueError:
             body = None
 
-        definition = None
-        if (
-            param_info.definition
-            and param_info.definition.annotation != inspect.Parameter.empty
-        ):
-            definition = param_info.definition.annotation
+        if not self.type_initialized:
+            if (
+                param_info.definition
+                and param_info.definition.annotation != inspect.Parameter.empty
+            ):
+                self.type_cache = pydantic.TypeAdapter(param_info.definition.annotation)
+            else:
+                self.type_cache = None
+            self.type_initialized = True
 
-        if definition is None:
+        if self.type_cache is None:
             return body
 
         try:
-            return pydantic.parse_obj_as(definition, body)
+            return self.type_cache.validate_python(body)
         except pydantic.ValidationError as err:
-            errors = err.errors()
+            errors = err.errors(include_url=False)
             for error in errors:
                 error["loc"] = ("body",) + error["loc"]
+                error.pop("input", None)  # type: ignore
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
 
 
 class Query:
@@ -152,16 +166,18 @@
         multiple: bool = False,
         description: str = "",
     ):
         self.default = default
         self.alias = alias
         self.multiple = multiple
         self.description = description
+        self.type_initialized = False
+        self.type_cache: "Union[pydantic.TypeAdapter[Any], None]" = None
 
-    def __call__(  # noqa: C901, WPS210
+    def __call__(  # noqa: C901
         self,
         param_info: ParamInfo = Depends(),
         request: web.Request = Depends(),
     ) -> Any:
         """
         Performs actual logic, described above.
 
@@ -172,38 +188,42 @@
         :return: parsed data.
         """
         param_name = self.alias or param_info.name
         default_value = None
         if self.default is not ...:
             default_value = self.default
 
+        if not self.type_initialized:
+            if (
+                param_info.definition
+                and param_info.definition.annotation != inspect.Parameter.empty
+            ):
+                self.type_cache = pydantic.TypeAdapter(param_info.definition.annotation)
+            else:
+                self.type_cache = None
+            self.type_initialized = True
+
         if self.multiple:
             value = request.query.getall(param_name, default_value)
         else:
             value = request.query.getone(param_name, default_value)
 
-        definition = None
-        if (
-            param_info.definition
-            and param_info.definition.annotation != inspect.Parameter.empty
-        ):
-            definition = param_info.definition.annotation
-
-        if definition is None:
+        if self.type_cache is None:
             return value
 
         try:
-            return pydantic.parse_obj_as(definition, value)
+            return self.type_cache.validate_python(value)
         except pydantic.ValidationError as err:
-            errors = err.errors()
+            errors = err.errors(include_url=False)
             for error in errors:
                 error["loc"] = (
                     "query",
                     param_name,
                 ) + error["loc"]
+                error.pop("input", None)  # type: ignore
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
 
 
 class Form:
@@ -212,44 +232,53 @@
 
     This dependency grabs form data and validates
     it against given schema.
 
     You should provide schema with typehints.
     """
 
-    async def __call__(
+    def __init__(self) -> None:
+        self.type_initialized = False
+        self.type_cache: "Union[pydantic.TypeAdapter[Any], None]" = None
+
+    async def __call__(  # noqa: C901
         self,
         param_info: ParamInfo = Depends(),
         request: web.Request = Depends(),
     ) -> Any:
         """
         Performs actual logic, described above.
 
         :param param_info: information about how the dependency
             was defined with name and type.
         :param request: current request.
         :raises HTTPBadRequest: if incorrect data was found.
         :return: parsed data.
         """
         form_data = await request.post()
-        definition = None
-        if (
-            param_info.definition
-            and param_info.definition.annotation != inspect.Parameter.empty
-        ):
-            definition = param_info.definition.annotation
 
-        if definition is None:
+        if not self.type_initialized:
+            if (
+                param_info.definition
+                and param_info.definition.annotation != inspect.Parameter.empty
+            ):
+                self.type_cache = pydantic.TypeAdapter(param_info.definition.annotation)
+            else:
+                self.type_cache = None
+            self.type_initialized = True
+
+        if self.type_cache is None:
             return form_data
 
         try:
-            return pydantic.parse_obj_as(definition, form_data)
+            return self.type_cache.validate_python(form_data)
         except pydantic.ValidationError as err:
-            errors = err.errors()
+            errors = err.errors(include_url=False)
             for error in errors:
+                error.pop("input", None)  # type: ignore
                 error["loc"] = ("form",) + error["loc"]
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
 
 
@@ -268,43 +297,50 @@
         *,
         alias: Optional[str] = None,
         description: str = "",
     ) -> None:
         self.default = default
         self.alias = alias
         self.description = description
+        self.type_initialized = False
+        self.type_cache: "Union[pydantic.TypeAdapter[Any], None]" = None
 
-    def __call__(
+    def __call__(  # noqa: C901
         self,
         param_info: ParamInfo = Depends(),
         request: web.Request = Depends(),
     ) -> Any:
         """
         Performs actual logic, described above.
 
         :param param_info: information about how the dependency
             was defined with name and type.
         :param request: current request.
         :raises HTTPBadRequest: if incorrect data was found.
         :return: parsed data.
         """
         matched_data = request.match_info.get(self.alias or param_info.name)
-        definition = None
-        if (
-            param_info.definition
-            and param_info.definition.annotation != inspect.Parameter.empty
-        ):
-            definition = param_info.definition.annotation
 
-        if definition is None:
+        if not self.type_initialized:
+            if (
+                param_info.definition
+                and param_info.definition.annotation != inspect.Parameter.empty
+            ):
+                self.type_cache = pydantic.TypeAdapter(param_info.definition.annotation)
+            else:
+                self.type_cache = None
+            self.type_initialized = True
+
+        if self.type_cache is None:
             return matched_data
 
         try:
-            return pydantic.parse_obj_as(definition, matched_data)
+            return self.type_cache.validate_python(matched_data)
         except pydantic.ValidationError as err:
-            errors = err.errors()
+            errors = err.errors(include_url=False)
             for error in errors:
+                error.pop("input", None)  # type: ignore
                 error["loc"] = ("path",) + error["loc"]
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
```

### Comparing `aiohttp_deps-0.2.1/aiohttp_deps/view.py` & `aiohttp_deps-0.3.0/aiohttp_deps/view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.2.1/pyproject.toml` & `aiohttp_deps-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "aiohttp-deps"
 description = "Dependency injection for AioHTTP"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.2.1"
+version = "0.3.0"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -23,15 +23,16 @@
 keywords = ["aiohttp", "taskiq-dependencies"]
 homepage = "https://github.com/taskiq-python/aiohttp-deps"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 aiohttp = "^3"
 taskiq-dependencies = "^1"
-pydantic = "^1"
+pydantic = "^2"
+deepmerge = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 flake8 = "^6"
 isort = "^5.10.1"
 mypy = "^0.971"
 pre-commit = "^2.20.0"
```

### Comparing `aiohttp_deps-0.2.1/PKG-INFO` & `aiohttp_deps-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-deps
-Version: 0.2.1
+Version: 0.3.0
 Summary: Dependency injection for AioHTTP
 Home-page: https://github.com/taskiq-python/aiohttp-deps
 License: LICENSE
 Keywords: aiohttp,taskiq-dependencies
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
@@ -20,15 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3,<4)
-Requires-Dist: pydantic (>=1,<2)
+Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
+Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: taskiq-dependencies (>=1,<2)
 Description-Content-Type: text/markdown
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiohttp-deps?style=for-the-badge)](https://pypi.org/project/aiohttp-deps/)
 [![PyPI](https://img.shields.io/pypi/v/aiohttp-deps?style=for-the-badge)](https://pypi.org/project/aiohttp-deps/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/aiohttp-deps?style=for-the-badge)](https://pypistats.org/packages/aiohttp-deps)
 
@@ -95,29 +96,71 @@
 main_router.add_routes(memes_router, prefix="/memes")
 ```
 
 ## Swagger
 
 If you use dependencies in you handlers, we can easily generate swagger for you.
 We have some limitations:
-1. We don't support string type annotation for detecting required parameters in openapi. Like `a: "Optional[int]"`.
-2. We don't have support for 3.10 style Option annotations. E.G. `int | None`
+1. We don't support resolving type aliases if hint is a string.
+    If you define variable like this: `myvar = int | None` and then in handler
+    you'd create annotation like this: `param: "str | myvar"` it will fail.
+    You need to unquote type hint in order to get it work.
 
 We will try to fix these limitations later.
 
 To enable swagger, just add it to your startup.
 
 ```python
 from aiohttp_deps import init, setup_swagger
 
 app = web.Application()
 
 app.on_startup.extend([init, setup_swagger()])
 ```
 
+### Responses
+
+You can define schema for responses using dataclasses or
+pydantic models. This would not affect handlers in any way,
+it's only for documentation purposes, if you want to actually
+validate values your handler returns, please write your own wrapper.
+
+```python
+from dataclasses import dataclass
+
+from aiohttp import web
+from pydantic import BaseModel
+
+from aiohttp_deps import Router, openapi_response
+
+router = Router()
+
+
+@dataclass
+class Success:
+    data: str
+
+
+class Unauthorized(BaseModel):
+    why: str
+
+
+@router.get("/")
+@openapi_response(200, Success, content_type="application/xml")
+@openapi_response(200, Success)
+@openapi_response(401, Unauthorized, description="When token is not correct")
+async def handler() -> web.Response:
+    ...
+```
+
+This example illustrates how much you can do with this decorator. You
+can have multiple content-types for a single status, or you can have different
+possble statuses. This function is pretty simple and if you want to make
+your own decorator for your responses, it won't be hard.
+
 
 ## Default dependencies
 
 By default this library provides only two injectables. `web.Request` and `web.Application`.
 
 ```python
 
@@ -180,29 +223,29 @@
 
 class UserInfo(BaseModel):
     name: str
 
 
 @router.post("/users")
 async def new_data(user: UserInfo = Depends(Json())):
-    return web.json_response({"user": user.dict()})
+    return web.json_response({"user": user.model_dump()})
 
 ```
 
 This dependency automatically validates data and send
 errors if the data doesn't orrelate with schema or body is not a valid json.
 
 If you want to make this data optional, just mark it as optional.
 
 ```python
 @router.post("/users")
 async def new_data(user: Optional[UserInfo] = Depends(Json())):
     if user is None:
         return web.json_response({"user": None})
-    return web.json_response({"user": user.dict()})
+    return web.json_response({"user": user.model_dump()})
 
 ```
 
 ## Headers
 
 You can get and validate headers using `Header` dependency.
 
@@ -301,27 +344,26 @@
 ## Forms
 
 Now you can easiy get and validate form data from your request.
 To make the magic happen, please add `arbitrary_types_allowed` to the config of your model.
 
 
 ```python
-from pydantic import BaseModel
+import pydantic
 from aiohttp_deps import Router, Depends, Form
 from aiohttp import web
 
 router = Router()
 
 
-class MyForm(BaseModel):
+class MyForm(pydantic.BaseModel):
     id: int
     file: web.FileField
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
 
 
 @router.post("/")
 async def handler(my_form: MyForm = Depends(Form())):
     with open("my_file", "wb") as f:
         f.write(my_form.file.file.read())
     return web.json_response({"id": my_form.id})
```

