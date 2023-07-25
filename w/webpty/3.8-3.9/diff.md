# Comparing `tmp/webpty-3.8.tar.gz` & `tmp/webpty-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpty-3.8.tar", max compression
+gzip compressed data, was "webpty-3.9.tar", max compression
```

## Comparing `webpty-3.8.tar` & `webpty-3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2022-12-16 06:19:27.884454 webpty-3.8/LICENSE
--rw-r--r--   0        0        0     1531 2022-12-16 06:19:27.884968 webpty-3.8/README.md
--rw-r--r--   0        0        0      514 2023-07-25 06:07:12.333576 webpty-3.8/pyproject.toml
--rw-r--r--   0        0        0      181 2022-12-16 11:42:16.018623 webpty-3.8/webpty/__init__.py
--rw-r--r--   0        0        0     1011 2023-07-25 06:05:13.399487 webpty-3.8/webpty/index.html
--rw-r--r--   0        0        0     6267 2022-12-16 11:42:16.019541 webpty-3.8/webpty/server.py
--rw-r--r--   0        0        0      232 2022-12-16 11:42:16.019787 webpty-3.8/webpty/static/webpty.css
--rw-r--r--   0        0        0     3043 2023-07-25 06:02:28.894895 webpty-3.8/webpty/static/webpty.js
--rw-r--r--   0        0        0      200 2022-12-16 11:42:16.020425 webpty-3.8/webpty/static/webpty.min.css
--rw-r--r--   0        0        0     1767 2023-07-25 06:05:02.484896 webpty-3.8/webpty/static/webpty.min.js
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 webpty-3.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-12-16 06:19:27.884454 webpty-3.9/LICENSE
+-rw-r--r--   0        0        0     1531 2022-12-16 06:19:27.884968 webpty-3.9/README.md
+-rw-r--r--   0        0        0      567 2023-07-25 06:38:13.870371 webpty-3.9/pyproject.toml
+-rw-r--r--   0        0        0      181 2022-12-16 11:42:16.018623 webpty-3.9/webpty/__init__.py
+-rw-r--r--   0        0        0     1011 2023-07-25 06:05:13.399487 webpty-3.9/webpty/index.html
+-rw-r--r--   0        0        0     6267 2022-12-16 11:42:16.019541 webpty-3.9/webpty/server.py
+-rw-r--r--   0        0        0      232 2022-12-16 11:42:16.019787 webpty-3.9/webpty/static/webpty.css
+-rw-r--r--   0        0        0     3043 2023-07-25 06:02:28.894895 webpty-3.9/webpty/static/webpty.js
+-rw-r--r--   0        0        0      200 2022-12-16 11:42:16.020425 webpty-3.9/webpty/static/webpty.min.css
+-rw-r--r--   0        0        0     1767 2023-07-25 06:05:02.484896 webpty-3.9/webpty/static/webpty.min.js
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 webpty-3.9/PKG-INFO
```

### Comparing `webpty-3.8/LICENSE` & `webpty-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `webpty-3.8/README.md` & `webpty-3.9/README.md`

 * *Files identical despite different names*

### Comparing `webpty-3.8/pyproject.toml` & `webpty-3.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webpty"
-version = "3.8"
+version = "3.9"
 description = "A web-based application to access shell & shell based applications via a browser"
 readme = "README.md"
 authors = ["Satheesh Kumar <mail@satheesh.dev>"]
 license = "OSI Approved :: MIT License"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<=3.10"
@@ -14,7 +14,10 @@
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+webpty = "webpty.server:main"
```

### Comparing `webpty-3.8/webpty/index.html` & `webpty-3.9/webpty/index.html`

 * *Files identical despite different names*

### Comparing `webpty-3.8/webpty/server.py` & `webpty-3.9/webpty/server.py`

 * *Files identical despite different names*

### Comparing `webpty-3.8/webpty/static/webpty.js` & `webpty-3.9/webpty/static/webpty.js`

 * *Files identical despite different names*

### Comparing `webpty-3.8/webpty/static/webpty.min.js` & `webpty-3.9/webpty/static/webpty.min.js`

 * *Files identical despite different names*

### Comparing `webpty-3.8/PKG-INFO` & `webpty-3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpty
-Version: 3.8
+Version: 3.9
 Summary: A web-based application to access shell & shell based applications via a browser
 License: OSI Approved :: MIT License
 Author: Satheesh Kumar
 Author-email: mail@satheesh.dev
 Requires-Python: >=3.7,<=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

