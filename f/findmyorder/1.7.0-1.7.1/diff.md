# Comparing `tmp/findmyorder-1.7.0.tar.gz` & `tmp/findmyorder-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.7.0.tar", max compression
+gzip compressed data, was "findmyorder-1.7.1.tar", max compression
```

## Comparing `findmyorder-1.7.0.tar` & `findmyorder-1.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-24 11:13:37.828631 findmyorder-1.7.0/LICENSE
--rw-r--r--   0        0        0     3022 2023-07-24 11:13:37.828631 findmyorder-1.7.0/README.md
--rw-r--r--   0        0        0      113 2023-07-24 11:13:41.748626 findmyorder-1.7.0/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-07-24 11:13:37.828631 findmyorder-1.7.0/findmyorder/config.py
--rw-r--r--   0        0        0     3221 2023-07-24 11:13:37.828631 findmyorder-1.7.0/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5931 2023-07-24 11:13:37.828631 findmyorder-1.7.0/findmyorder/main.py
--rw-r--r--   0        0        0     2977 2023-07-24 11:13:41.740626 findmyorder-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 findmyorder-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-25 19:53:10.390204 findmyorder-1.7.1/LICENSE
+-rw-r--r--   0        0        0     3022 2023-07-25 19:53:10.390204 findmyorder-1.7.1/README.md
+-rw-r--r--   0        0        0      113 2023-07-25 19:53:14.898631 findmyorder-1.7.1/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-25 19:53:10.390204 findmyorder-1.7.1/findmyorder/config.py
+-rw-r--r--   0        0        0     3221 2023-07-25 19:53:10.390204 findmyorder-1.7.1/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5931 2023-07-25 19:53:10.390204 findmyorder-1.7.1/findmyorder/main.py
+-rw-r--r--   0        0        0     3002 2023-07-25 19:53:14.890630 findmyorder-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 findmyorder-1.7.1/PKG-INFO
```

### Comparing `findmyorder-1.7.0/LICENSE` & `findmyorder-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.0/README.md` & `findmyorder-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.0/findmyorder/config.py` & `findmyorder-1.7.1/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.0/findmyorder/default_settings.toml` & `findmyorder-1.7.1/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.0/findmyorder/main.py` & `findmyorder-1.7.1/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.0/pyproject.toml` & `findmyorder-1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.7.0"
+version = "1.7.1"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -57,14 +57,15 @@
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
+pytest-loguru = "^0.2.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.0"
 sphinx_bootstrap_theme = "^0.8.1"
```

### Comparing `findmyorder-1.7.0/PKG-INFO` & `findmyorder-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.7.0 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.7.1 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist: loguru
```

