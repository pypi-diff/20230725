# Comparing `tmp/neosctl-0.9.1.tar.gz` & `tmp/neosctl-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.9.1.tar", max compression
+gzip compressed data, was "neosctl-0.9.2.tar", max compression
```

## Comparing `neosctl-0.9.1.tar` & `neosctl-0.9.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2962 2023-07-25 12:02:32.690170 neosctl-0.9.1/README.md
--rw-r--r--   0        0        0       22 2023-07-25 12:02:32.690170 neosctl-0.9.1/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/constant.py
--rw-r--r--   0        0        0     4654 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/profile.py
--rw-r--r--   0        0        0     2668 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    14331 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-07-25 12:02:32.691170 neosctl-0.9.1/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     5491 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     4556 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3490 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1409 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0    14484 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0     1283 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3978 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      184 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-07-25 12:02:32.692170 neosctl-0.9.1/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     7848 2023-07-25 12:02:32.693170 neosctl-0.9.1/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    14103 2023-07-25 12:02:32.693170 neosctl-0.9.1/neosctl/util.py
--rw-r--r--   0        0        0     3053 2023-07-25 12:02:32.693170 neosctl-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 neosctl-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2962 2023-07-25 12:24:22.852816 neosctl-0.9.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-25 12:24:22.852816 neosctl-0.9.2/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/constant.py
+-rw-r--r--   0        0        0     4654 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/profile.py
+-rw-r--r--   0        0        0     2668 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14331 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     5491 2023-07-25 12:24:22.853817 neosctl-0.9.2/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     4556 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3490 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1409 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0    14484 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0     1283 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     4168 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      184 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     7848 2023-07-25 12:24:22.854817 neosctl-0.9.2/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    14103 2023-07-25 12:24:22.855817 neosctl-0.9.2/neosctl/util.py
+-rw-r--r--   0        0        0     3053 2023-07-25 12:24:22.855817 neosctl-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 neosctl-0.9.2/PKG-INFO
```

### Comparing `neosctl-0.9.1/README.md` & `neosctl-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.9.1
+# Core CLI v0.9.2
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.9.1/neosctl/auth.py` & `neosctl-0.9.2/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/cli.py` & `neosctl-0.9.2/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/profile.py` & `neosctl-0.9.2/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/schema.py` & `neosctl-0.9.2/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/__init__.py` & `neosctl-0.9.2/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/data_product.py` & `neosctl-0.9.2/neosctl/services/gateway/data_product.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/data_source.py` & `neosctl-0.9.2/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/data_system.py` & `neosctl-0.9.2/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/data_unit.py` & `neosctl-0.9.2/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/entity.py` & `neosctl-0.9.2/neosctl/services/gateway/entity.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/link.py` & `neosctl-0.9.2/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/output.py` & `neosctl-0.9.2/neosctl/services/gateway/output.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/schema.py` & `neosctl-0.9.2/neosctl/services/gateway/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/secret.py` & `neosctl-0.9.2/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/spark.py` & `neosctl-0.9.2/neosctl/services/gateway/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/gateway/tag.py` & `neosctl-0.9.2/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/iam/iam.py` & `neosctl-0.9.2/neosctl/services/iam/iam.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/iam/schema.py` & `neosctl-0.9.2/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/services/registry/registry.py` & `neosctl-0.9.2/neosctl/services/registry/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,50 @@
+import typing
+
 import httpx
 import typer
 
 from neosctl import util
 from neosctl.services.registry.schema import MigrateCore, RegisterCore, RemoveCore
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
+ACCOUNT_ARG = typer.Option(None, help="Account override (root only).", callback=util.sanitize)
+
+
 def _core_url(registry_api_url: str) -> str:
     return "{}/core".format(registry_api_url.rstrip("/"))
 
 
 def _data_product_url(registry_api_url: str, postfix: str = "") -> str:
     return "{}/data_product{}".format(registry_api_url.rstrip("/"), postfix)
 
 
 @app.command(name="register-core")
 def register_core(
     ctx: typer.Context,
     partition: str = typer.Argument(..., help="Core partition", callback=util.sanitize),
     name: str = typer.Argument(..., help="Core name", callback=util.sanitize),
+    account: typing.Optional[str] = ACCOUNT_ARG,
 ) -> None:
     """Register a core.
 
     Register a core to receive an identifier and access key for use in deployment.
     """
 
     @util.ensure_login
     def _request(ctx: typer.Context, rc: RegisterCore) -> httpx.Response:
         return util.post(
             ctx,
             _core_url(ctx.obj.get_registry_api_url()),
             json=rc.dict(exclude_none=True),
             headers={"X-Partition": partition},
+            account=account,
         )
 
     rc = RegisterCore(name=name)
 
     r = _request(ctx, rc)
     process_response(r)
```

### Comparing `neosctl-0.9.1/neosctl/services/storage/storage.py` & `neosctl-0.9.2/neosctl/services/storage/storage.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/neosctl/util.py` & `neosctl-0.9.2/neosctl/util.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.9.1/pyproject.toml` & `neosctl-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.9.1"
+version = "0.9.2"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.9.1/PKG-INFO` & `neosctl-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.9.1
+Version: 0.9.2
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.9.1
+# Core CLI v0.9.2
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

