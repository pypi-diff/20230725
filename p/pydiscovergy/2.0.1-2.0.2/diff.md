# Comparing `tmp/pydiscovergy-2.0.1.tar.gz` & `tmp/pydiscovergy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiscovergy-2.0.1.tar", max compression
+gzip compressed data, was "pydiscovergy-2.0.2.tar", max compression
```

## Comparing `pydiscovergy-2.0.1.tar` & `pydiscovergy-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1081 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/LICENSE
--rw-r--r--   0        0        0      575 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/README.md
--rw-r--r--   0        0        0      102 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/__init__.py
--rw-r--r--   0        0        0      330 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/authentication/__init__.py
--rw-r--r--   0        0        0      444 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/authentication/base.py
--rw-r--r--   0        0        0      658 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/authentication/basicauth.py
--rw-r--r--   0        0        0     7022 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/authentication/token.py
--rw-r--r--   0        0        0      646 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/const.py
--rw-r--r--   0        0        0     6278 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/discovergy.py
--rw-r--r--   0        0        0      547 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/error.py
--rw-r--r--   0        0        0     1041 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/marshmallow.py
--rw-r--r--   0        0        0     1318 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pydiscovergy/models.py
--rw-r--r--   0        0        0     1078 2023-07-25 10:17:42.084552 pydiscovergy-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 pydiscovergy-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/LICENSE
+-rw-r--r--   0        0        0      575 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/README.md
+-rw-r--r--   0        0        0      102 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/authentication/__init__.py
+-rw-r--r--   0        0        0      444 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/authentication/base.py
+-rw-r--r--   0        0        0      658 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/authentication/basicauth.py
+-rw-r--r--   0        0        0     7022 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/authentication/token.py
+-rw-r--r--   0        0        0      646 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/const.py
+-rw-r--r--   0        0        0     6278 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/discovergy.py
+-rw-r--r--   0        0        0      547 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/error.py
+-rw-r--r--   0        0        0     1041 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/marshmallow.py
+-rw-r--r--   0        0        0     1447 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/models.py
+-rw-r--r--   0        0        0     1095 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 pydiscovergy-2.0.2/PKG-INFO
```

### Comparing `pydiscovergy-2.0.1/LICENSE` & `pydiscovergy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.1/README.md` & `pydiscovergy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.1/pydiscovergy/authentication/basicauth.py` & `pydiscovergy-2.0.2/pydiscovergy/authentication/basicauth.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.1/pydiscovergy/authentication/token.py` & `pydiscovergy-2.0.2/pydiscovergy/authentication/token.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.1/pydiscovergy/const.py` & `pydiscovergy-2.0.2/pydiscovergy/const.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.1/pydiscovergy/discovergy.py` & `pydiscovergy-2.0.2/pydiscovergy/discovergy.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.1/pydiscovergy/error.py` & `pydiscovergy-2.0.2/pydiscovergy/error.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.1/pydiscovergy/marshmallow.py` & `pydiscovergy-2.0.2/pydiscovergy/marshmallow.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.1/pydiscovergy/models.py` & `pydiscovergy-2.0.2/pydiscovergy/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Models for Discovergy API."""
 from dataclasses import dataclass, field
 from datetime import datetime
 
+import pytz
 from dataclasses_json import CatchAll, LetterCase, Undefined, config, dataclass_json
 from marshmallow import fields
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(frozen=True)
 class Location:
@@ -26,14 +27,18 @@
     time: datetime = field(metadata=config(mm_field=fields.DateTime("timestamp_ms")))
     values: dict[str, float] = field(
         metadata=config(
             mm_field=fields.Dict(keys=fields.String(), values=fields.Float())
         )
     )
 
+    @property
+    def time_with_timezone(self) -> datetime:
+        return pytz.timezone("UTC").localize(self.time)
+
 
 @dataclass_json
 @dataclass(frozen=True)
 class Statistic:
     """Represents a meter statistic entry."""
 
     count: int
```

### Comparing `pydiscovergy-2.0.1/pyproject.toml` & `pydiscovergy-2.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pydiscovergy"
-version = "2.0.1"
+version = "2.0.2"
 description = "Async Python 3 library for interacting with Discovergy smart meters API"
 authors = ["Jan-Philipp Benecke <jan-philipp@bnck.me>"]
 repository = "https://github.com/jpbede/pydiscovergy"
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "pydiscovergy" }
@@ -17,14 +17,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 authlib = "<1.0.0"
 httpx = "^0.24.0"
 dataclasses-json = "^0.5.13"
 marshmallow = "^3.19.0"
+pytz = "^2023.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
 respx = "^0.20.1"
 black = "^23.1.0"
```

### Comparing `pydiscovergy-2.0.1/PKG-INFO` & `pydiscovergy-2.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiscovergy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Async Python 3 library for interacting with Discovergy smart meters API
 Home-page: https://github.com/jpbede/pydiscovergy
 License: MIT
 Keywords: discovergy,smart meter,smart home
 Author: Jan-Philipp Benecke
 Author-email: jan-philipp@bnck.me
 Requires-Python: >=3.9,<3.12
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: authlib (<1.0.0)
 Requires-Dist: dataclasses-json (>=0.5.13,<0.6.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: marshmallow (>=3.19.0,<4.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Project-URL: Repository, https://github.com/jpbede/pydiscovergy
 Description-Content-Type: text/markdown
 
 # pydiscovergy
 [![CI](https://github.com/jpbede/pydiscovergy/actions/workflows/ci.yml/badge.svg)](https://github.com/jpbede/pydiscovergy/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/jpbede/pydiscovergy/branch/dev/graph/badge.svg?token=JXB451BOSE)](https://codecov.io/gh/jpbede/pydiscovergy)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b093280986f7453391f132a46d834154)](https://www.codacy.com/gh/jpbede/pydiscovergy/dashboard)
```

