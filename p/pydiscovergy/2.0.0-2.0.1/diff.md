# Comparing `tmp/pydiscovergy-2.0.0.tar.gz` & `tmp/pydiscovergy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiscovergy-2.0.0.tar", max compression
+gzip compressed data, was "pydiscovergy-2.0.1.tar", max compression
```

## Comparing `pydiscovergy-2.0.0.tar` & `pydiscovergy-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1081 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/LICENSE
--rw-r--r--   0        0        0      575 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/README.md
--rw-r--r--   0        0        0      102 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/__init__.py
--rw-r--r--   0        0        0      330 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/authentication/__init__.py
--rw-r--r--   0        0        0      444 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/authentication/base.py
--rw-r--r--   0        0        0      658 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/authentication/basicauth.py
--rw-r--r--   0        0        0     7022 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/authentication/token.py
--rw-r--r--   0        0        0      646 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/const.py
--rw-r--r--   0        0        0     6278 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/discovergy.py
--rw-r--r--   0        0        0      547 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/error.py
--rw-r--r--   0        0        0     1041 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/marshmallow.py
--rw-r--r--   0        0        0     1318 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/models.py
--rw-r--r--   0        0        0     1068 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 pydiscovergy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/LICENSE
+-rw-r--r--   0        0        0      575 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/README.md
+-rw-r--r--   0        0        0      102 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/authentication/__init__.py
+-rw-r--r--   0        0        0      444 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/authentication/base.py
+-rw-r--r--   0        0        0      658 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/authentication/basicauth.py
+-rw-r--r--   0        0        0     7022 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/authentication/token.py
+-rw-r--r--   0        0        0      646 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/const.py
+-rw-r--r--   0        0        0     6278 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/discovergy.py
+-rw-r--r--   0        0        0      547 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/error.py
+-rw-r--r--   0        0        0     1041 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/marshmallow.py
+-rw-r--r--   0        0        0     1318 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/models.py
+-rw-r--r--   0        0        0     1078 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 pydiscovergy-2.0.1/PKG-INFO
```

### Comparing `pydiscovergy-2.0.0/LICENSE` & `pydiscovergy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/README.md` & `pydiscovergy-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/pydiscovergy/authentication/basicauth.py` & `pydiscovergy-2.0.1/pydiscovergy/authentication/basicauth.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/pydiscovergy/authentication/token.py` & `pydiscovergy-2.0.1/pydiscovergy/authentication/token.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/pydiscovergy/const.py` & `pydiscovergy-2.0.1/pydiscovergy/const.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/pydiscovergy/discovergy.py` & `pydiscovergy-2.0.1/pydiscovergy/discovergy.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/pydiscovergy/error.py` & `pydiscovergy-2.0.1/pydiscovergy/error.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/pydiscovergy/marshmallow.py` & `pydiscovergy-2.0.1/pydiscovergy/marshmallow.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/pydiscovergy/models.py` & `pydiscovergy-2.0.1/pydiscovergy/models.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.0/pyproject.toml` & `pydiscovergy-2.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pydiscovergy"
-version = "2.0.0"
+version = "2.0.1"
 description = "Async Python 3 library for interacting with Discovergy smart meters API"
 authors = ["Jan-Philipp Benecke <jan-philipp@bnck.me>"]
 repository = "https://github.com/jpbede/pydiscovergy"
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "pydiscovergy" }
 ]
 keywords = ["discovergy", "smart meter", "smart home"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-Authlib = "^1.2.0"
+python = ">=3.9, <3.12"
+authlib = "<1.0.0"
 httpx = "^0.24.0"
-dataclasses-json = "^0.5.9"
+dataclasses-json = "^0.5.13"
 marshmallow = "^3.19.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
 respx = "^0.20.1"
@@ -44,8 +44,8 @@
     "I",  # isort
     "UP",  # pyupgrade
     "W",  # pycodestyle
 ]
 
 ignore = [
   "E501"
-]
+]
```

### Comparing `pydiscovergy-2.0.0/PKG-INFO` & `pydiscovergy-2.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pydiscovergy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Async Python 3 library for interacting with Discovergy smart meters API
 Home-page: https://github.com/jpbede/pydiscovergy
 License: MIT
 Keywords: discovergy,smart meter,smart home
 Author: Jan-Philipp Benecke
 Author-email: jan-philipp@bnck.me
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Authlib (>=1.2.0,<2.0.0)
-Requires-Dist: dataclasses-json (>=0.5.9,<0.6.0)
+Requires-Dist: authlib (<1.0.0)
+Requires-Dist: dataclasses-json (>=0.5.13,<0.6.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: marshmallow (>=3.19.0,<4.0.0)
 Project-URL: Repository, https://github.com/jpbede/pydiscovergy
 Description-Content-Type: text/markdown
 
 # pydiscovergy
 [![CI](https://github.com/jpbede/pydiscovergy/actions/workflows/ci.yml/badge.svg)](https://github.com/jpbede/pydiscovergy/actions/workflows/ci.yml)
```

