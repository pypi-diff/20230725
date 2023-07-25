# Comparing `tmp/clientele-0.2.0.tar.gz` & `tmp/clientele-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clientele-0.2.0.tar", max compression
+gzip compressed data, was "clientele-0.3.0.tar", max compression
```

## Comparing `clientele-0.2.0.tar` & `clientele-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1607 2023-07-24 03:48:04.784855 clientele-0.2.0/README.md
--rw-r--r--   0        0        0      872 2023-07-24 04:21:34.493850 clientele-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.2.0/src/__init__.py
--rw-r--r--   0        0        0     1890 2023-07-24 03:57:17.660962 clientele-0.2.0/src/cli.py
--rw-r--r--   0        0        0     1355 2023-07-24 02:58:52.770829 clientele-0.2.0/src/generator.py
--rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.2.0/src/generators/__init__.py
--rw-r--r--   0        0        0     8426 2023-07-24 04:18:46.735999 clientele-0.2.0/src/generators/clients.py
--rw-r--r--   0        0        0     3793 2023-07-24 03:51:19.613122 clientele-0.2.0/src/generators/http.py
--rw-r--r--   0        0        0     3621 2023-07-24 04:14:37.896419 clientele-0.2.0/src/generators/schemas.py
--rw-r--r--   0        0        0      109 2023-07-24 01:55:07.678461 clientele-0.2.0/src/settings.py
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.2.0/src/template/__init__.py
--rw-r--r--   0        0        0       79 2023-07-24 03:49:46.038745 clientele-0.2.0/src/template/client.py
--rw-r--r--   0        0        0      697 2023-07-24 03:50:51.889574 clientele-0.2.0/src/template/http.py
--rw-r--r--   0        0        0       91 2023-07-24 01:55:07.678461 clientele-0.2.0/src/template/schemas.py
--rw-r--r--   0        0        0     1942 2023-07-24 04:16:31.046189 clientele-0.2.0/src/utils.py
--rw-r--r--   0        0        0      446 2023-07-24 03:32:58.998660 clientele-0.2.0/src/writer.py
--rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 clientele-0.2.0/setup.py
--rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 clientele-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1306 2023-07-25 02:54:52.074475 clientele-0.3.0/README.md
+-rw-r--r--   0        0        0      896 2023-07-25 00:37:07.430216 clientele-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.3.0/src/__init__.py
+-rw-r--r--   0        0        0     1894 2023-07-24 23:26:08.953873 clientele-0.3.0/src/cli.py
+-rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.3.0/src/constants_template.py
+-rw-r--r--   0        0        0     2055 2023-07-24 23:26:23.378037 clientele-0.3.0/src/generator.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.3.0/src/generators/__init__.py
+-rw-r--r--   0        0        0     7656 2023-07-24 21:16:51.549353 clientele-0.3.0/src/generators/clients.py
+-rw-r--r--   0        0        0     2976 2023-07-24 22:56:42.864879 clientele-0.3.0/src/generators/http.py
+-rw-r--r--   0        0        0     3621 2023-07-24 04:14:37.896419 clientele-0.3.0/src/generators/schemas.py
+-rw-r--r--   0        0        0      190 2023-07-24 21:03:06.895168 clientele-0.3.0/src/settings.py
+-rw-r--r--   0        0        0       61 2023-07-24 20:44:55.813864 clientele-0.3.0/src/template/MANIFEST
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.3.0/src/template/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.3.0/src/template/client.py
+-rw-r--r--   0        0        0      974 2023-07-24 21:23:51.037441 clientele-0.3.0/src/template/http.py
+-rw-r--r--   0        0        0       91 2023-07-24 01:55:07.678461 clientele-0.3.0/src/template/schemas.py
+-rw-r--r--   0        0        0     1942 2023-07-24 04:16:31.046189 clientele-0.3.0/src/utils.py
+-rw-r--r--   0        0        0      558 2023-07-24 21:04:10.212122 clientele-0.3.0/src/writer.py
+-rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 clientele-0.3.0/setup.py
+-rw-r--r--   0        0        0     2146 1970-01-01 00:00:00.000000 clientele-0.3.0/PKG-INFO
```

### Comparing `clientele-0.2.0/pyproject.toml` & `clientele-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "clientele"
-version = "0.2.0"
+version = "0.3.0"
 description = "Typed API Clients from OpenAPI specs"
 authors = ["Paul Hallett <paulandrewhallett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "src"}]
-homepage = "https://github.com/beckett-software/clientele"
+homepage = "https://beckett-software.github.io/clientele/"
 
 [tool.poetry.scripts]
 clientele = "src.cli:cli_group"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "^0.24.1"
 click = "^8.1.3"
-structlog = "^23.1.0"
-ipython = "^8.14.0"
 pydantic = "^2.0.3"
 rich = "^13.4.2"
 openapi-core = "0.18.0"
 pyyaml = "^6.0.1"
 types-pyyaml = "^6.0.12.11"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "1.4.0"
 ruff = "^0.0.272"
+mkdocs = "^1.4.3"
+ipython = "^8.14.0"
+mkdocs-material = "^9.1.19"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 120
```

### Comparing `clientele-0.2.0/src/cli.py` & `clientele-0.3.0/src/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,47 +20,48 @@
     Generate a new client from an openapi.json spec
     """
     from json import JSONDecodeError
 
     import yaml
     from httpx import Client
     from openapi_core import Spec
-    from structlog import get_logger
+    from rich.console import Console
+
+    console = Console()
 
     from src.generator import Generator
 
     assert url or file, "Must pass either a URL or a file"
 
-    log = get_logger(__name__)
     if url:
         client = Client()
         response = client.get(url)
         try:
             data = response.json()
         except JSONDecodeError:
             # It's probably yaml
             data = yaml.safe_load(response.content)
         spec = Spec.from_dict(data)
     else:
         with open(file, "r") as f:
             spec = Spec.from_file(f)
-    log.info(
+    console.log(
         f"Found API specification for {spec['info']['title']} | version {spec['info']['version']}"
     )
     major, _, _ = spec["openapi"].split(".")
     if int(major) < 3:
-        log.warning(
-            f"clientele only supports OpenAPI version 3.0.0 and up, and you have {spec['openapi']}"
+        console.log(
+            f"[red]clientele only supports OpenAPI version 3.0.0 and up, and you have {spec['openapi']}"
         )
         return
-    log.info(f"OpenAPI version {spec['openapi']}")
+    console.log(f"OpenAPI version {spec['openapi']}")
     if asyncio:
-        log.info("Generating async client...")
+        console.log("Generating async client...")
     else:
-        log.info("Generating sync client...")
-    Generator(spec=spec, asyncio=asyncio, output_dir=output).generate(url=url)
+        console.log("Generating sync client...")
+    Generator(spec=spec, asyncio=asyncio, output_dir=output).generate()
 
 
 cli_group.add_command(generate)
 
 if __name__ == "__main__":
     cli_group()
```

### Comparing `clientele-0.2.0/src/generators/clients.py` & `clientele-0.3.0/src/generators/clients.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from collections import defaultdict
 from typing import Any, Dict, List
-from urllib.parse import urlparse
 
 from openapi_core import Spec
 from rich.console import Console
 
 from src.generators.schemas import SchemasGenerator
 from src.utils import class_name_titled, clean_prop, get_func_name, get_type
 from src.writer import write_to_client
@@ -31,27 +30,20 @@
     ) -> None:
         self.spec = spec
         self.output_dir = output_dir
         self.results = defaultdict(int)
         self.schemas_generator = schemas_generator
         self.asyncio = asyncio
 
-    def generate_paths(self, api_url: str) -> None:
+    def generate_paths(self) -> None:
         for path in self.spec["paths"].items():
-            self.write_path_to_client(api_url=api_url, path=path)
+            self.write_path_to_client(path=path)
         console.log(f"Generated {self.results['get_methods']} GET methods...")
         console.log(f"Generated {self.results['post_methods']} POST methods...")
 
-    def parse_api_base_url(self, url: str) -> str:
-        """
-        Returns the base API URL for this service
-        """
-        url_parts = urlparse(url=url)
-        return f"{url_parts.scheme}://{url_parts.hostname}{f':{url_parts.port}' if url_parts.port not in [80, 443] else ''}"  # noqa
-
     def generate_function_args(self, parameters: List[Dict]) -> Dict[str, Any]:
         return_string_bits = []
         param_keys = []
         query_args = []
         path_args = []
         for p in parameters:
             if p.get("$ref"):
@@ -126,81 +118,73 @@
             return f"""typing.Union[{', '.join([f'schemas.{r}' for r in response_class_names])}]"""
         elif len(response_class_names) == 0:
             return "None"
         else:
             return f"schemas.{response_class_names[0]}"
 
     def generate_input_types(self, request_body: Dict) -> str:
-        input_class_names = self.get_input_class_names(inputs=request_body)
+        input_class_names = self.get_input_class_names(inputs={"": request_body})
         for input_class in input_class_names:
             if input_class not in self.schemas_generator.schemas.keys():
                 # It doesn't exist! Generate the schema for it
                 self.schemas_generator.generate_input_class(schema=request_body)
         if len(input_class_names) > 1:
             return f"""typing.Union[{', '.join([f'schemas.{r}' for r in input_class_names])}]"""
         elif len(input_class_names) == 0:
             return "None"
         else:
             return f"schemas.{input_class_names[0]}"
 
-    def generate_get_content(self, operation: Dict, api_url: str, path: str) -> None:
+    def generate_get_content(self, operation: Dict, path: str) -> None:
         response_types = self.generate_response_types(operation["responses"])
         func_name = get_func_name(operation, path)
         function_arguments = self.generate_function_args(
             operation.get("parameters", [])
         )
         if query_args := function_arguments["query_args"]:
-            api_url = f"{self.parse_api_base_url(api_url)}{path}"
             # TODO do this far more elegantly
             api_url = (
-                api_url + "?" + "&".join([f"{p}=" + "{" + p + "}" for p in query_args])
+                path + "?" + "&".join([f"{p}=" + "{" + p + "}" for p in query_args])
             )
         else:
-            api_url = f"{self.parse_api_base_url(api_url)}{path}"
+            api_url = path
         CONTENT = f"""
 {self.asyncio and "async " or ""}def {func_name}({function_arguments['return_string']}) -> {response_types}:
     response = {self.asyncio and "await " or ""}http.get(f"{api_url}")
     return http.handle_response({func_name}, response)
     """
         self.results["get_methods"] += 1
         write_to_client(content=CONTENT, output_dir=self.output_dir)
 
-    def generate_post_content(self, operation: Dict, api_url: str, path: str) -> None:
-        api_url = f"{self.parse_api_base_url(api_url)}{path}"
+    def generate_post_content(self, operation: Dict, path: str) -> None:
         response_types = self.generate_response_types(operation["responses"])
         func_name = get_func_name(operation, path)
         if not operation.get("requestBody"):
             input_class_name = "None"
         else:
-            input_class_name = self.generate_input_types(
-                {"": operation.get("requestBody")}
-            )
+            input_class_name = self.generate_input_types(operation.get("requestBody"))
         function_arguments = self.generate_function_args(
             operation.get("parameters", [])
         )
         FUNCTION_ARGS = f"""
 {function_arguments['return_string']}{function_arguments['return_string'] and ", "}data: {input_class_name}"""
         CONTENT = f"""
 {self.asyncio and "async " or ""}def {func_name}({FUNCTION_ARGS}) -> {response_types}:
-    response = {self.asyncio and "await " or ""}http.post(f"{api_url}", data=data and data.model_dump())
+    response = {self.asyncio and "await " or ""}http.post(f"{path}", data=data and data.model_dump())
     return http.handle_response({func_name}, response)
     """
         self.results["post_methods"] += 1
         write_to_client(content=CONTENT, output_dir=self.output_dir)
 
-    def write_path_to_client(self, api_url: str, path: Dict) -> None:
+    def write_path_to_client(self, path: Dict) -> None:
         url, operations = path
-        if servers := operations.get("servers"):
-            api_url = servers[0]["url"]
         for method, operation in operations.items():
             if method == "get":
                 self.generate_get_content(
                     operation=operation,
-                    api_url=api_url,
                     path=url,
                 )
             elif method == "post":
                 self.generate_post_content(
                     operation=operation,
-                    api_url=api_url,
                     path=url,
                 )
```

### Comparing `clientele-0.2.0/src/generators/http.py` & `clientele-0.3.0/src/generators/http.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,45 +5,42 @@
 from rich.console import Console
 
 from src.writer import write_to_http
 
 console = Console()
 
 BEARER_CLIENT = """
-AUTH_TOKEN = environ.get("{bearer_token_key}")
-headers = dict(Authorization=f'Bearer {{AUTH_TOKEN}}')
+headers = dict(Authorization=f'Bearer {c.get_bearer_token()}')
 client = httpx.{client_type}(headers=headers)
 """
 
 BASIC_CLIENT = """
-AUTH_USER = environ.get("{user_key}")
-AUTH_PASS = environ.get("{pass_key}")
-client = httpx.{client_type}(auth=(AUTH_USER, AUTH_PASS))
+client = httpx.{client_type}(auth=(c.get_user_key(), c.get_pass_key()))
 """
 
 NO_AUTH_CLIENT = """
 client = httpx.{client_type}()
 """
 
 SYNC_METHODS = """
 def get(url: str) -> httpx.Response:
-    return client.get(url)
+    return client.get(parse_url(url))
 
 
 def post(url: str, data: typing.Dict) -> httpx.Response:
-    return client.post(url, json=data)
+    return client.post(parse_url(url), json=data)
 """
 
 ASYNC_METHODS = """
 async def get(url: str) -> httpx.Response:
-    return await client.get(url)
+    return await client.get(parse_url(url))
 
 
 async def post(url: str, data: typing.Dict) -> httpx.Response:
-    return await client.post(url, json=data)
+    return await client.post(parse_url(url), json=data)
 """
 
 
 def env_var(output_dir: str, key: str) -> str:
     output_dir = output_dir.replace("/", "")
     return f"{output_dir.upper()}_{key.upper()}"
 
@@ -68,37 +65,24 @@
                 if (
                     info["type"] == "http"
                     and info["scheme"] in ["basic", "bearer"]
                     and client_generated is False
                 ):
                     client_generated = True
                     if info["scheme"] == "bearer":
-                        test_key = env_var(output_dir=self.output_dir, key="AUTH_KEY")
                         content = BEARER_CLIENT.format(
                             client_type=client_type,
-                            bearer_token_key=f"{test_key}",
-                        )
-                        console.log(
-                            f"[yellow]Please use \n* {test_key}\nenvironment variable to use bearer authentication"
                         )
                     else:  # Can only be "basic" at this point
-                        user_key = env_var(
-                            output_dir=self.output_dir, key="AUTH_USER_KEY"
-                        )
-                        pass_key = env_var(
-                            output_dir=self.output_dir, key="AUTH_PASS_KEY"
-                        )
-                        console.log(
-                            f"[yellow]Please set \n* {user_key}\n* {pass_key} \nenvironment variable to use basic authentication"  # noqa
-                        )
                         content = BASIC_CLIENT.format(
                             client_type=client_type,
-                            user_key=f"{user_key}",
-                            pass_key=f"{pass_key}",
                         )
+                    console.log(
+                        f"[yellow]Please see {self.output_dir}constants.py to set authentication variables"
+                    )
         if client_generated is False:
             console.log(f"Generating {'async' if self.asyncio else 'sync'} client...")
             content = NO_AUTH_CLIENT.format(client_type=client_type)
             client_generated = True
         write_to_http(content, output_dir=self.output_dir)
         if self.asyncio:
             write_to_http(ASYNC_METHODS, output_dir=self.output_dir)
```

### Comparing `clientele-0.2.0/src/generators/schemas.py` & `clientele-0.3.0/src/generators/schemas.py`

 * *Files identical despite different names*

### Comparing `clientele-0.2.0/src/utils.py` & `clientele-0.3.0/src/utils.py`

 * *Files identical despite different names*

### Comparing `clientele-0.2.0/setup.py` & `clientele-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,35 +6,33 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'httpx>=0.24.1,<0.25.0',
- 'ipython>=8.14.0,<9.0.0',
  'openapi-core==0.18.0',
  'pydantic>=2.0.3,<3.0.0',
  'pyyaml>=6.0.1,<7.0.0',
  'rich>=13.4.2,<14.0.0',
- 'structlog>=23.1.0,<24.0.0',
  'types-pyyaml>=6.0.12.11,<7.0.0.0']
 
 entry_points = \
 {'console_scripts': ['clientele = src.cli:cli_group']}
 
 setup_kwargs = {
     'name': 'clientele',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Typed API Clients from OpenAPI specs',
-    'long_description': "#  ⚜️ Clientele\n\n### Typed API Clients from OpenAPI specs\n\n![clientele_logo](https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true)\n\nClientele lets you generate fully-typed, functional, API Clients from OpenAPI specs.\n\nIt uses modern tools to be blazing fast and type safe. \n\nPlus - there is no complex boilerplate and the generated code is very small.\n\n## Features\n\n* Fully typed API Client using Pydantic.\n* Minimalist and easy to use - the generated code is tiny.\n* Choose either sync (default) or async - we support both.\n* Generates authentication code for you (curently only supports HTTP Bearer auth)\n* Written entirely in Python - no need to install other languages to use OpenAPI.\n\nWe're built on:\n\n* [Pydantic 2.0](https://docs.pydantic.dev/latest/)\n* [httpx](https://www.python-httpx.org/)\n* [openapi-core](https://openapi-core.readthedocs.io/en/latest/)\n\n## Install\n\n```sh\npoetry add clientele\n```\n\n## Usage\n\n### From URLs\n\n```sh\nclientele generate -u http://URL_TO_OPEN_API.json -o output/\n```\n\n### From files\n\n```sh\nclientele generate -f path/to/file.json -o output/\n```\n\n### Async Client\n\n```sh\nclientele generate -f path/to/file.json -o output/ --asyncio t\n```\n\n## Authentication\n\nIf your OpenAPI spec provides security information for the following authentication methods:\n\n* HTTP Bearer\n\nThen clientele will provide you information on the environment variables you need to set to\nmake this work during the generation. For example:\n\n```sh\nPlease set\n* MY_CLIENT_AUTH_USER_KEY\n* MY_CLIENT_AUTH_PASS_KEY\nenvironment variable to use basic authentication\n```\n",
+    'long_description': "# ⚜️ Clientele\n\n# Typed API Clients from OpenAPI specs\n\n![clientele_logo](https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true)\n\nClientele lets you generate fully-typed, functional, API Clients from OpenAPI specs.\n\nIt uses modern tools to be blazing fast and type safe.\n\nPlus - there is no complex boilerplate and the generated code is very small.\n\n## Features\n\n* Fully typed API Client using Pydantic.\n* Minimalist and easy to use - the generated code is designed for readability.\n* Choose either sync or async - we support both, and you can switch between them easily.\n* Supports authentication (curently only HTTP Bearer and HTTP Basic auth).\n* Written entirely in Python - no need to install other languages to use OpenAPI.\n* The client footprint is minimal - it only requires `httpx` and `pydantic`.\n* Supports your own configuration - we provide an entry point that will never be overwritten.\n\nWe're built on:\n\n* [Pydantic 2.0](https://docs.pydantic.dev/latest/)\n* [httpx](https://www.python-httpx.org/)\n* [openapi-core](https://openapi-core.readthedocs.io/en/latest/)\n\n## Install\n\n```sh\npoetry add clientele\n```\n\n## Usage\n\n```sh\nclientele generate -f path/to/file.json -o my_client/ --asyncio t\n```\n\n[Read the docs](https://beckett-software.github.io/clientele/)\n",
     'author': 'Paul Hallett',
     'author_email': 'paulandrewhallett@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/beckett-software/clientele',
+    'url': 'https://beckett-software.github.io/clientele/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `clientele-0.2.0/PKG-INFO` & `clientele-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: clientele
-Version: 0.2.0
+Version: 0.3.0
 Summary: Typed API Clients from OpenAPI specs
-Home-page: https://github.com/beckett-software/clientele
+Home-page: https://beckett-software.github.io/clientele/
 License: MIT
 Author: Paul Hallett
 Author-email: paulandrewhallett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: openapi-core (==0.18.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
-Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.11,<7.0.0.0)
 Description-Content-Type: text/markdown
 
-#  ⚜️ Clientele
+# ⚜️ Clientele
 
-### Typed API Clients from OpenAPI specs
+# Typed API Clients from OpenAPI specs
 
 ![clientele_logo](https://github.com/beckett-software/clientele/blob/main/docs/clientele.jpeg?raw=true)
 
 Clientele lets you generate fully-typed, functional, API Clients from OpenAPI specs.
 
-It uses modern tools to be blazing fast and type safe. 
+It uses modern tools to be blazing fast and type safe.
 
 Plus - there is no complex boilerplate and the generated code is very small.
 
 ## Features
 
 * Fully typed API Client using Pydantic.
-* Minimalist and easy to use - the generated code is tiny.
-* Choose either sync (default) or async - we support both.
-* Generates authentication code for you (curently only supports HTTP Bearer auth)
+* Minimalist and easy to use - the generated code is designed for readability.
+* Choose either sync or async - we support both, and you can switch between them easily.
+* Supports authentication (curently only HTTP Bearer and HTTP Basic auth).
 * Written entirely in Python - no need to install other languages to use OpenAPI.
+* The client footprint is minimal - it only requires `httpx` and `pydantic`.
+* Supports your own configuration - we provide an entry point that will never be overwritten.
 
 We're built on:
 
 * [Pydantic 2.0](https://docs.pydantic.dev/latest/)
 * [httpx](https://www.python-httpx.org/)
 * [openapi-core](https://openapi-core.readthedocs.io/en/latest/)
 
@@ -53,41 +53,13 @@
 
 ```sh
 poetry add clientele
 ```
 
 ## Usage
 
-### From URLs
-
-```sh
-clientele generate -u http://URL_TO_OPEN_API.json -o output/
-```
-
-### From files
-
 ```sh
-clientele generate -f path/to/file.json -o output/
+clientele generate -f path/to/file.json -o my_client/ --asyncio t
 ```
 
-### Async Client
-
-```sh
-clientele generate -f path/to/file.json -o output/ --asyncio t
-```
-
-## Authentication
-
-If your OpenAPI spec provides security information for the following authentication methods:
-
-* HTTP Bearer
-
-Then clientele will provide you information on the environment variables you need to set to
-make this work during the generation. For example:
-
-```sh
-Please set
-* MY_CLIENT_AUTH_USER_KEY
-* MY_CLIENT_AUTH_PASS_KEY
-environment variable to use basic authentication
-```
+[Read the docs](https://beckett-software.github.io/clientele/)
```

