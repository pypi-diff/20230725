# Comparing `tmp/dxsp-4.2.1.tar.gz` & `tmp/dxsp-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.2.1.tar", max compression
+gzip compressed data, was "dxsp-4.2.2.tar", max compression
```

## Comparing `dxsp-4.2.1.tar` & `dxsp-4.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-24 11:14:21.402070 dxsp-4.2.1/LICENSE
--rw-r--r--   0        0        0     2857 2023-07-24 11:14:21.402070 dxsp-4.2.1/README.md
--rw-r--r--   0        0        0      158 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/config.py
--rw-r--r--   0        0        0    12100 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5743 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/main.py
--rw-r--r--   0        0        0      104 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1864 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1037 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4834 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6619 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1990 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-07-24 11:14:21.406070 dxsp-4.2.1/dxsp/utils/utils.py
--rw-r--r--   0        0        0     4055 2023-07-24 11:14:25.190171 dxsp-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 dxsp-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-25 19:43:39.050390 dxsp-4.2.2/LICENSE
+-rw-r--r--   0        0        0     2857 2023-07-25 19:43:39.050390 dxsp-4.2.2/README.md
+-rw-r--r--   0        0        0      158 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/config.py
+-rw-r--r--   0        0        0    12100 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5743 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4834 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-07-25 19:43:39.050390 dxsp-4.2.2/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     4057 2023-07-25 19:43:42.978444 dxsp-4.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 dxsp-4.2.2/PKG-INFO
```

### Comparing `dxsp-4.2.1/LICENSE` & `dxsp-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/README.md` & `dxsp-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/dxsp/default_settings.toml` & `dxsp-4.2.2/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/dxsp/main.py` & `dxsp-4.2.2/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/dxsp/protocols/oneinch.py` & `dxsp-4.2.2/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/dxsp/protocols/uniswap.py` & `dxsp-4.2.2/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/dxsp/protocols/zerox.py` & `dxsp-4.2.2/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/dxsp/utils/account_utils.py` & `dxsp-4.2.2/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/dxsp/utils/contract_utils.py` & `dxsp-4.2.2/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/dxsp/utils/explorer_utils.py` & `dxsp-4.2.2/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.1/pyproject.toml` & `dxsp-4.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.2.1"
+version = "4.2.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -46,14 +46,15 @@
 fixable = ["ALL"]
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 eth_tester = "^0.9.0b2"
@@ -73,14 +74,15 @@
     "*/config.py"
 ]
 
 
 
 
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.0"
 sphinx_bootstrap_theme = "^0.8.1"
 sphinx-autoapi = "^2.1.1"
```

### Comparing `dxsp-4.2.1/PKG-INFO` & `dxsp-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.2.1
+Version: 4.2.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.2.1 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.2.2 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist:
 pycoingecko (>=3.1.0,<4.0.0) Requires-Dist: uniswap-python (>=0.7.0,<0.8.0)
```

