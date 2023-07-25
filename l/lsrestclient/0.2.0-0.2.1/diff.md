# Comparing `tmp/lsrestclient-0.2.0.tar.gz` & `tmp/lsrestclient-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsrestclient-0.2.0.tar", max compression
+gzip compressed data, was "lsrestclient-0.2.1.tar", max compression
```

## Comparing `lsrestclient-0.2.0.tar` & `lsrestclient-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.2.0/README.md
--rw-r--r--   0        0        0     3117 2023-07-25 14:47:43.639742 lsrestclient-0.2.0/lsrestclient/__init__.py
--rw-r--r--   0        0        0      707 2023-07-25 14:51:03.406972 lsrestclient-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6623 1970-01-01 00:00:00.000000 lsrestclient-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.2.1/README.md
+-rw-r--r--   0        0        0     3142 2023-07-25 14:53:36.290062 lsrestclient-0.2.1/lsrestclient/__init__.py
+-rw-r--r--   0        0        0      707 2023-07-25 14:53:46.217996 lsrestclient-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6623 1970-01-01 00:00:00.000000 lsrestclient-0.2.1/PKG-INFO
```

### Comparing `lsrestclient-0.2.0/README.md` & `lsrestclient-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lsrestclient-0.2.0/lsrestclient/__init__.py` & `lsrestclient-0.2.1/lsrestclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import lsjsonclasses
 import requests
 from requests import Session, Response
 from requests.structures import CaseInsensitiveDict
 
 
+find_parameters_regex = re.compile("\{(.*?)\}")
+
 @dataclass
 class LsRestClientResponse:
     status_code: int
     content: str
     headers: CaseInsensitiveDict
 
     _json: Optional[dict] = None
@@ -48,16 +50,15 @@
         self._clients[name] = self
 
     def full_url(self, url: str, params: dict | None = None) -> str:
         if params is None:
             params = {}
 
         full_url = f"{self.base_url}{url}"
-        regex = re.compile("\{(.*?)\}")
-        found = regex.findall(full_url)
+        found = find_parameters_regex.findall(full_url)
         url_params = {p: params[p] for p in found}
         for p in found:
             del params[p]
         return full_url.format(**url_params)
 
     def request(
         self,
```

### Comparing `lsrestclient-0.2.0/pyproject.toml` & `lsrestclient-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lsrestclient"
-version = "0.2.0"
+version = "0.2.1"
 description = "REST Api Client"
 authors = ["mba <bartel@electronic-shop.lu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

### Comparing `lsrestclient-0.2.0/PKG-INFO` & `lsrestclient-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsrestclient
-Version: 0.2.0
+Version: 0.2.1
 Summary: REST Api Client
 Author: mba
 Author-email: bartel@electronic-shop.lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

