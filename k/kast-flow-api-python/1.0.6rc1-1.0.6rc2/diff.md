# Comparing `tmp/kast_flow_api_python-1.0.6rc1.tar.gz` & `tmp/kast_flow_api_python-1.0.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kast_flow_api_python-1.0.6rc1.tar", max compression
+gzip compressed data, was "kast_flow_api_python-1.0.6rc2.tar", max compression
```

## Comparing `kast_flow_api_python-1.0.6rc1.tar` & `kast_flow_api_python-1.0.6rc2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-05 08:45:28.809107 kast_flow_api_python-1.0.6rc1/kast_flow_api/__init__.py
--rw-r--r--   0        0        0     8970 2023-07-05 08:45:28.783107 kast_flow_api_python-1.0.6rc1/kast_flow_api/v1.py
--rw-r--r--   0        0        0      537 2023-07-05 08:45:48.563153 kast_flow_api_python-1.0.6rc1/pyproject.toml
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.6rc1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-25 13:58:20.243446 kast_flow_api_python-1.0.6rc2/kast_flow_api/__init__.py
+-rw-r--r--   0        0        0     9063 2023-07-25 13:58:20.217446 kast_flow_api_python-1.0.6rc2/kast_flow_api/v1.py
+-rw-r--r--   0        0        0      537 2023-07-25 13:58:40.250443 kast_flow_api_python-1.0.6rc2/pyproject.toml
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.6rc2/PKG-INFO
```

### Comparing `kast_flow_api_python-1.0.6rc1/kast_flow_api/v1.py` & `kast_flow_api_python-1.0.6rc2/kast_flow_api/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 
     def sql(self: Self, query: str) -> "KastDataFrame":
         ...
 
     def table_sql(self: Self, query: str) -> None:
         ...
 
+    def checkpoint(self: Self) -> "KastDataFrame":
+        ...
+
 
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class SideOutValue:
     out: str
     schema: str
 
 
@@ -144,14 +147,15 @@
         ...
 
 
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class KastFunction(Protocol):
     id: str
     registerSchema: bool = False
+    checkpoint: bool = False
     outs: KastOuts = field(default_factory=make_outs)
 
     def compute(
         self: Self,
         tool: KastTool,
         tables: list[KastDataFrame],
     ) -> KastDataFrame:
```

### Comparing `kast_flow_api_python-1.0.6rc1/pyproject.toml` & `kast_flow_api_python-1.0.6rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kast-flow-api-python"
-version = "1.0.6-preview1"
+version = "1.0.6-preview2"
 description = "kast python api unified processing engine"
 authors = ["kast"]
 packages = [
     { include = "kast_flow_api" }
 ]
 
 [tool.poetry.dependencies]
```

