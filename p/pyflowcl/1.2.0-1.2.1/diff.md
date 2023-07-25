# Comparing `tmp/pyflowcl-1.2.0.tar.gz` & `tmp/pyflowcl-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflowcl-1.2.0.tar", max compression
+gzip compressed data, was "pyflowcl-1.2.1.tar", max compression
```

## Comparing `pyflowcl-1.2.0.tar` & `pyflowcl-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-07-22 08:18:28.828508 pyflowcl-1.2.0/LICENSE
--rw-r--r--   0        0        0      774 2023-07-22 08:18:28.828508 pyflowcl-1.2.0/README.md
--rw-r--r--   0        0        0     2616 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/Clients.py
--rw-r--r--   0        0        0     6726 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/Payment.py
--rw-r--r--   0        0        0     2376 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/Refund.py
--rw-r--r--   0        0        0      136 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/__init__.py
--rw-r--r--   0        0        0     2271 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/cli.py
--rw-r--r--   0        0        0       88 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/exceptions.py
--rw-r--r--   0        0        0    18975 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/models.py
--rw-r--r--   0        0        0     3601 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/openapi3.py
--rw-r--r--   0        0        0     2022 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/utils.py
--rw-r--r--   0        0        0       22 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/version.py
--rw-r--r--   0        0        0   172982 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.live.min.yaml
--rw-r--r--   0        0        0   173070 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.min.yaml
--rw-r--r--   0        0        0   172983 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.sandbox.min.yaml
--rw-r--r--   0        0        0   189757 2023-07-22 08:18:28.836507 pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.yaml
--rw-r--r--   0        0        0     2052 2023-07-22 08:18:28.836507 pyflowcl-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 pyflowcl-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-25 20:31:33.104971 pyflowcl-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3075 2023-07-25 20:31:33.104971 pyflowcl-1.2.1/README.md
+-rw-r--r--   0        0        0     2616 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/Clients.py
+-rw-r--r--   0        0        0     6726 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/Payment.py
+-rw-r--r--   0        0        0     2376 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/Refund.py
+-rw-r--r--   0        0        0      136 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/__init__.py
+-rw-r--r--   0        0        0     2271 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/cli.py
+-rw-r--r--   0        0        0       88 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/exceptions.py
+-rw-r--r--   0        0        0    18975 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/models.py
+-rw-r--r--   0        0        0     3628 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/openapi3.py
+-rw-r--r--   0        0        0     2022 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/utils.py
+-rw-r--r--   0        0        0       22 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/version.py
+-rw-r--r--   0        0        0   172982 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/yaml_files/apiFlow.live.min.yaml
+-rw-r--r--   0        0        0   173070 2023-07-25 20:31:33.108971 pyflowcl-1.2.1/pyflowcl/yaml_files/apiFlow.min.yaml
+-rw-r--r--   0        0        0   172983 2023-07-25 20:31:33.112971 pyflowcl-1.2.1/pyflowcl/yaml_files/apiFlow.sandbox.min.yaml
+-rw-r--r--   0        0        0   189757 2023-07-25 20:31:33.112971 pyflowcl-1.2.1/pyflowcl/yaml_files/apiFlow.yaml
+-rw-r--r--   0        0        0     2036 2023-07-25 20:31:33.112971 pyflowcl-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4309 1970-01-01 00:00:00.000000 pyflowcl-1.2.1/PKG-INFO
```

### Comparing `pyflowcl-1.2.0/LICENSE` & `pyflowcl-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/Clients.py` & `pyflowcl-1.2.1/pyflowcl/Clients.py`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/Payment.py` & `pyflowcl-1.2.1/pyflowcl/Payment.py`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/Refund.py` & `pyflowcl-1.2.1/pyflowcl/Refund.py`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/cli.py` & `pyflowcl-1.2.1/pyflowcl/cli.py`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/models.py` & `pyflowcl-1.2.1/pyflowcl/models.py`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/openapi3.py` & `pyflowcl-1.2.1/pyflowcl/openapi3.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,29 @@
         api_key (str, optional): Clave de API para autenticación. Si no se proporciona, se tomará del entorno.
         api_secret (str, optional): Secreto de API para autenticación. Si no se proporciona, se tomará del entorno.
         endpoint (str, optional): Ambiente Flow para llamadas ("live" o "sandbox").
     """
 
     api_key: Union[None, str] = None
     api_secret: Union[None, str] = None
-    endpoint: str = "live"
+    endpoint: Union[None, str] = None
     _base_path: Any = Path(__file__).resolve().parent
     _yaml_file: Union[None, str] = None
     _openapi3: Union[None, OpenAPI] = field(init=False)
 
     def __post_init__(self):
         if not self.api_key:
             self.api_key = os.getenv("PYFLOWCL_API_KEY", None)
         if not self.api_secret:
             self.api_secret = os.getenv("PYFLOWCL_API_SECRET", None)
         if not self.endpoint:
             self.endpoint = os.getenv("PYFLOWCL_ENDPOINT", "live")
 
         try:
-            yaml_spec = load_yaml_file(f"{self._base_path}/yaml_files/apiFlow.min.yaml")
+            yaml_spec = load_yaml_file(f"{self._base_path}/yaml_files/apiFlow.{self.endpoint}.min.yaml")
         except Exception as e:
             raise Exception(f"No se pudo cargar el archivo: {e}")
         else:
             yaml_spec = self.fix_openapi3(yaml_spec)
             self._openapi3 = OpenAPI(yaml_spec)
 
     def fix_openapi3(self, flow_yaml_spec):
```

### Comparing `pyflowcl-1.2.0/pyflowcl/utils.py` & `pyflowcl-1.2.1/pyflowcl/utils.py`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.live.min.yaml` & `pyflowcl-1.2.1/pyflowcl/yaml_files/apiFlow.live.min.yaml`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.min.yaml` & `pyflowcl-1.2.1/pyflowcl/yaml_files/apiFlow.min.yaml`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.sandbox.min.yaml` & `pyflowcl-1.2.1/pyflowcl/yaml_files/apiFlow.sandbox.min.yaml`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.yaml` & `pyflowcl-1.2.1/pyflowcl/yaml_files/apiFlow.yaml`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.2.0/pyproject.toml` & `pyflowcl-1.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyflowcl"
-version = "1.2.0"
+version = "1.2.1"
 description = "Cliente para comunicacion con flowAPI-3 de flow.cl"
 authors = [
     "Mario Hernandez <yo@mariofix.com>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mariofix/pyflowcl"
@@ -38,19 +38,19 @@
 packages = [
     {include = "pyflowcl"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.5"
 certifi = "*"
-requests = "2.31.0"
-openapi3 = "1.8.1"
-python-fsutil = "0.10.0"
-python-slugify = "8.0.1"
-pyyaml = "6.0.1"
+requests = "*"
+openapi3 = "^1.8"
+python-fsutil = "*"
+python-slugify = "*"
+pyyaml = "^6.0"
 typer = {extras = ["all"], version = "^0.9.0"}
 
 [tool.poetry.scripts]
 flow-cli = "pyflowcl.cli:app"
 
 [tool.poetry.group.dev]
 optional = true
```

