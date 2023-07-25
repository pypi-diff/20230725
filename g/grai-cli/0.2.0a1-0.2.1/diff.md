# Comparing `tmp/grai_cli-0.2.0a1.tar.gz` & `tmp/grai_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_cli-0.2.0a1.tar", max compression
+gzip compressed data, was "grai_cli-0.2.1.tar", max compression
```

## Comparing `grai_cli-0.2.0a1.tar` & `grai_cli-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0      237 2023-05-19 11:07:12.863498 grai_cli-0.2.0a1/README.md
--rw-r--r--   0        0        0      323 2023-07-18 02:25:32.298110 grai_cli-0.2.0a1/grai_cli/__init__.py
--rw-r--r--   0        0        0       63 2022-11-09 15:55:13.272679 grai_cli-0.2.0a1/grai_cli/api/__init__.py
--rw-r--r--   0        0        0       51 2022-07-24 08:00:09.094234 grai_cli-0.2.0a1/grai_cli/api/config/__init__.py
--rw-r--r--   0        0        0     2024 2023-07-17 16:42:30.681148 grai_cli-0.2.0a1/grai_cli/api/config/config.py
--rw-r--r--   0        0        0     3632 2023-06-14 21:02:53.335424 grai_cli-0.2.0a1/grai_cli/api/config/set.py
--rw-r--r--   0        0        0      463 2023-06-14 21:02:53.375897 grai_cli-0.2.0a1/grai_cli/api/config/setup.py
--rw-r--r--   0        0        0     1317 2023-06-14 21:02:53.291370 grai_cli-0.2.0a1/grai_cli/api/entrypoint.py
--rw-r--r--   0        0        0       49 2022-07-24 08:00:09.100216 grai_cli-0.2.0a1/grai_cli/api/server/__init__.py
--rw-r--r--   0        0        0     6030 2023-07-17 20:13:45.162367 grai_cli-0.2.0a1/grai_cli/api/server/endpoints.py
--rw-r--r--   0        0        0     1094 2023-07-17 16:43:38.992726 grai_cli-0.2.0a1/grai_cli/api/server/setup.py
--rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273574 grai_cli-0.2.0a1/grai_cli/api/telemetry/__init__.py
--rw-r--r--   0        0        0      376 2023-06-14 21:02:53.379310 grai_cli-0.2.0a1/grai_cli/api/telemetry/commands.py
--rw-r--r--   0        0        0       89 2023-03-16 04:12:39.225317 grai_cli-0.2.0a1/grai_cli/config_default.yaml
--rw-r--r--   0        0        0        0 2022-07-24 06:33:14.647347 grai_cli-0.2.0a1/grai_cli/py.typed
--rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273862 grai_cli-0.2.0a1/grai_cli/settings/__init__.py
--rw-r--r--   0        0        0     2999 2023-07-18 01:57:07.330038 grai_cli-0.2.0a1/grai_cli/settings/cache.py
--rw-r--r--   0        0        0     6413 2023-07-18 02:21:27.966349 grai_cli-0.2.0a1/grai_cli/settings/config.py
--rw-r--r--   0        0        0       88 2023-01-10 17:15:31.923336 grai_cli-0.2.0a1/grai_cli/utilities/__init__.py
--rw-r--r--   0        0        0     1588 2023-06-01 16:01:43.233062 grai_cli-0.2.0a1/grai_cli/utilities/headers.py
--rw-r--r--   0        0        0     1180 2023-06-01 16:01:43.233302 grai_cli-0.2.0a1/grai_cli/utilities/styling.py
--rw-r--r--   0        0        0      796 2023-06-01 16:01:43.233445 grai_cli-0.2.0a1/grai_cli/utilities/telemetry.py
--rw-r--r--   0        0        0      507 2023-07-17 16:42:57.404252 grai_cli-0.2.0a1/grai_cli/utilities/test.py
--rw-r--r--   0        0        0     5013 2023-06-14 21:02:53.399455 grai_cli-0.2.0a1/grai_cli/utilities/utilities.py
--rw-r--r--   0        0        0     2305 2023-06-14 21:02:53.362258 grai_cli-0.2.0a1/grai_cli/utilities/validators.py
--rw-r--r--   0        0        0     1056 2023-07-18 02:25:32.292022 grai_cli-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 grai_cli-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0      237 2023-05-19 11:07:12.863498 grai_cli-0.2.1/README.md
+-rw-r--r--   0        0        0      265 2023-07-25 15:15:09.686075 grai_cli-0.2.1/grai_cli/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-25 06:08:43.207214 grai_cli-0.2.1/grai_cli/api/__init__.py
+-rw-r--r--   0        0        0       51 2022-07-24 08:00:09.094234 grai_cli-0.2.1/grai_cli/api/config/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-25 06:08:43.210234 grai_cli-0.2.1/grai_cli/api/config/config.py
+-rw-r--r--   0        0        0     3632 2023-06-14 21:02:53.335424 grai_cli-0.2.1/grai_cli/api/config/set.py
+-rw-r--r--   0        0        0      463 2023-07-24 17:33:15.107250 grai_cli-0.2.1/grai_cli/api/config/setup.py
+-rw-r--r--   0        0        0       47 2023-07-25 06:08:43.212315 grai_cli-0.2.1/grai_cli/api/demo/__init__.py
+-rw-r--r--   0        0        0     3862 2023-07-25 06:08:43.589331 grai_cli-0.2.1/grai_cli/api/demo/endpoints.py
+-rw-r--r--   0        0        0      280 2023-07-24 14:14:54.426309 grai_cli-0.2.1/grai_cli/api/demo/setup.py
+-rw-r--r--   0        0        0     1461 2023-07-25 06:08:43.211629 grai_cli-0.2.1/grai_cli/api/entrypoint.py
+-rw-r--r--   0        0        0       49 2022-07-24 08:00:09.100216 grai_cli-0.2.1/grai_cli/api/server/__init__.py
+-rw-r--r--   0        0        0     6016 2023-07-20 03:27:21.099359 grai_cli-0.2.1/grai_cli/api/server/endpoints.py
+-rw-r--r--   0        0        0     1094 2023-07-20 03:27:21.099456 grai_cli-0.2.1/grai_cli/api/server/setup.py
+-rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273574 grai_cli-0.2.1/grai_cli/api/telemetry/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-14 21:02:53.379310 grai_cli-0.2.1/grai_cli/api/telemetry/commands.py
+-rw-r--r--   0        0        0       89 2023-03-16 04:12:39.225317 grai_cli-0.2.1/grai_cli/config_default.yaml
+-rw-r--r--   0        0        0        0 2022-07-24 06:33:14.647347 grai_cli-0.2.1/grai_cli/py.typed
+-rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273862 grai_cli-0.2.1/grai_cli/settings/__init__.py
+-rw-r--r--   0        0        0     3896 2023-07-25 16:48:03.783918 grai_cli-0.2.1/grai_cli/settings/cache.py
+-rw-r--r--   0        0        0     5505 2023-07-25 06:08:43.628335 grai_cli-0.2.1/grai_cli/settings/config.py
+-rw-r--r--   0        0        0       88 2023-01-10 17:15:31.923336 grai_cli-0.2.1/grai_cli/utilities/__init__.py
+-rw-r--r--   0        0        0     1588 2023-06-01 16:01:43.233062 grai_cli-0.2.1/grai_cli/utilities/headers.py
+-rw-r--r--   0        0        0     1180 2023-06-01 16:01:43.233302 grai_cli-0.2.1/grai_cli/utilities/styling.py
+-rw-r--r--   0        0        0      796 2023-06-01 16:01:43.233445 grai_cli-0.2.1/grai_cli/utilities/telemetry.py
+-rw-r--r--   0        0        0      515 2023-07-20 03:27:21.099797 grai_cli-0.2.1/grai_cli/utilities/test.py
+-rw-r--r--   0        0        0     5013 2023-06-14 21:02:53.399455 grai_cli-0.2.1/grai_cli/utilities/utilities.py
+-rw-r--r--   0        0        0     2273 2023-07-25 01:04:41.595999 grai_cli-0.2.1/grai_cli/utilities/validators.py
+-rw-r--r--   0        0        0     1092 2023-07-24 19:39:17.060842 grai_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 grai_cli-0.2.1/PKG-INFO
```

### Comparing `grai_cli-0.2.0a1/grai_cli/api/config/config.py` & `grai_cli-0.2.1/grai_cli/api/config/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,54 +2,61 @@
 
 from grai_cli.api.config.setup import config_app
 from grai_cli.settings.config import BasicAuthSettings, ServerSettingsV1, config
 from grai_cli.utilities import utilities
 from grai_cli.utilities.styling import GraiColors, default_styler, strip_style
 from grai_cli.utilities.validators import (
     host_callback,
-    insecure_callback,
     password_callback,
-    port_callback,
     username_callback,
     workspace_callback,
 )
 
 
+class InitDefaults:
+    @staticmethod
+    def url_default():
+        return default_styler(config.server.url)
+
+    @staticmethod
+    def workspace_default():
+        return default_styler(config.server.workspace)
+
+
 @config_app.command("init")
 def cli_init_config(
     username: str = typer.Option(..., prompt=True, callback=username_callback, prompt_required=True),
     password: str = typer.Option(
         ...,
         prompt=True,
         prompt_required=True,
         hide_input=True,
         confirmation_prompt=True,
-        callback=strip_style(password_callback),
+        callback=typer.unstyle,
     ),
     url: str = typer.Option(
-        default=default_styler(config.server.url),
+        InitDefaults.url_default,
         prompt="Server URL",
         prompt_required=True,
-        callback=strip_style(host_callback),
+        callback=typer.unstyle,
     ),
     workspace: str = typer.Option(
-        default=default_styler(config.server.workspace),
+        InitDefaults.workspace_default,
         prompt="The Grai workspace for this config",
         prompt_required=True,
-        callback=strip_style(workspace_callback),
+        callback=typer.unstyle,
     ),
 ):
     """Initialize a new config file
 
     Args:
-        username:  (Default value = typer.Option(..., prompt=True, callback=username_callback, prompt_required=True))
-        password:  (Default value = typer.Option(...,prompt=True,prompt_required=True,hide_input=True,confirmation_prompt=True,callback=strip_style(password_callback))
-        ):
+        username:
+        password:
         url:
-        workspace:  (Default value = typer.Option(default=default_styler(config.server.workspace))
+        workspace:
 
     Returns:
 
     Raises:
 
     """
     config.auth = BasicAuthSettings(username=username, password=password)
```

### Comparing `grai_cli-0.2.0a1/grai_cli/api/config/set.py` & `grai_cli-0.2.1/grai_cli/api/config/set.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0a1/grai_cli/api/entrypoint.py` & `grai_cli-0.2.1/grai_cli/api/entrypoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 
 import click
 import typer
 
+import grai_cli
 from grai_cli.utilities.telemetry import Telemetry
-from grai_cli.utilities.utilities import HAS_RICH, default_callback
+from grai_cli.utilities.utilities import HAS_RICH, default_callback, print
 
 
 def result_callback(*args, **kwargs):
     """
 
     Args:
         *args:
@@ -55,7 +56,12 @@
 
     if telemetry is not None:
         from grai_cli.settings.cache import cache
 
         cache.set("telemetry_consent", telemetry)
 
     default_callback(ctx)
+
+
+@app.command("version", help="Returns the current CLI version")
+def get_cli_version():
+    print(grai_cli.__version__)
```

### Comparing `grai_cli-0.2.0a1/grai_cli/api/server/endpoints.py` & `grai_cli-0.2.1/grai_cli/api/server/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 from typing import Optional
 
 import typer
+from grai_client.schemas.schema import validate_file
 
 from grai_cli.api.entrypoint import app
 from grai_cli.api.server.setup import client_app, client_get_app, get_default_client
 from grai_cli.utilities import utilities
 from grai_cli.utilities.styling import default_styler
 from grai_cli.utilities.utilities import merge_dicts, write_yaml
-from grai_client.schemas.schema import validate_file
 
 
 @client_app.command("is_authenticated", help="Verify auth credentials are valid")
 def is_authenticated():
     """ """
     client = get_default_client()
     authentication_status = client.check_authentication()
@@ -20,19 +20,15 @@
         utilities.print("Authenticated")
     else:
         utilities.print(
             f"Failed to Authenticate: Code {authentication_status.status_code}, {authentication_status.content}"
         )
 
 
-def get_nodes(
-    print: bool = True,
-    to_file: Optional[Path] = None,
-    **kwargs
-):
+def get_nodes(print: bool = True, to_file: Optional[Path] = None, **kwargs):
     """
 
     Args:
         name (Optional[str], optional):  (Default value = None)
         namespace (Optional[str], optional):  (Default value = None)
         print (bool, optional):  (Default value = True)
         to_file (Optional[Path], optional):  (Default value = None)
```

### Comparing `grai_cli-0.2.0a1/grai_cli/api/server/setup.py` & `grai_cli-0.2.1/grai_cli/api/server/setup.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0a1/grai_cli/utilities/headers.py` & `grai_cli-0.2.1/grai_cli/utilities/headers.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0a1/grai_cli/utilities/styling.py` & `grai_cli-0.2.1/grai_cli/utilities/styling.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0a1/grai_cli/utilities/telemetry.py` & `grai_cli-0.2.1/grai_cli/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0a1/grai_cli/utilities/utilities.py` & `grai_cli-0.2.1/grai_cli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0a1/grai_cli/utilities/validators.py` & `grai_cli-0.2.1/grai_cli/utilities/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Returns:
 
     Raises:
 
     """
     if len(inp) == 0:
-        raise typer.BadParameter("Password is invalid for <reasons>")
+        raise typer.BadParameter("Password is empty")
     return inp
 
 
 def workspace_callback(inp: str):
     """
 
     Args:
@@ -29,15 +29,15 @@
 
     Returns:
 
     Raises:
 
     """
     if len(inp) == 0:
-        raise typer.BadParameter("workspace is invalid for <reasons>")
+        raise typer.BadParameter("workspace is empty")
     return inp
 
 
 def password_callback(inp: str):
     """
 
     Args:
```

### Comparing `grai_cli-0.2.0a1/pyproject.toml` & `grai_cli-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-cli"
-version = "0.2.0-alpha1"
+version = "0.2.1"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 readme = "README.md"
 packages = [{include = "grai_cli"}]
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-cli"
@@ -16,18 +16,19 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 multimethod = "^1.9"
 typer = "^0.7.0"
 confuse = "^2.0.0"
 requests = "^2.28.1"
 pydantic = "^1.10.11"
-grai-client = "^0.3.0-alpha25"
+grai-client = "^0.3.0"
 posthog = "^2.2.0"
 rich = "^12.6.0"
 grai-schemas = "^0.2.0a10"
+goodconf = {extras = ["yaml"], version = "^3.0.1"}
 
 [tool.isort]
 profile = "black"
 known_first_party = "grai_cli"
 
 [tool.black]
 line-length = 120
```

### Comparing `grai_cli-0.2.0a1/PKG-INFO` & `grai_cli-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-cli
-Version: 0.2.0a1
+Version: 0.2.1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: confuse (>=2.0.0,<3.0.0)
-Requires-Dist: grai-client (>=0.3.0-alpha25,<0.4.0)
+Requires-Dist: goodconf[yaml] (>=3.0.1,<4.0.0)
+Requires-Dist: grai-client (>=0.3.0,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a10,<0.3.0)
 Requires-Dist: multimethod (>=1.9,<2.0)
 Requires-Dist: posthog (>=2.2.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
```

