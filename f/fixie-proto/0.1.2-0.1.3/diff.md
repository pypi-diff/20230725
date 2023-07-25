# Comparing `tmp/fixie_proto-0.1.2.tar.gz` & `tmp/fixie_proto-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixie_proto-0.1.2.tar", max compression
+gzip compressed data, was "fixie_proto-0.1.3.tar", max compression
```

## Comparing `fixie_proto-0.1.2.tar` & `fixie_proto-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     3428 2023-07-25 02:05:06.891240 fixie_proto-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-25 02:05:39.182147 fixie_proto-0.1.2/gen/python/fixie/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 02:05:39.186147 fixie_proto-0.1.2/gen/python/fixie/corpora/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 02:05:39.186147 fixie_proto-0.1.2/gen/python/fixie/corpora/v1/__init__.py
--rw-r--r--   0        0        0     1838 2023-07-25 02:05:39.170146 fixie_proto-0.1.2/gen/python/fixie/corpora/v1/common_pb2.py
--rw-r--r--   0        0        0     3595 2023-07-25 02:05:39.170146 fixie_proto-0.1.2/gen/python/fixie/corpora/v1/loader_pb2.py
--rw-r--r--   0        0        0      425 2023-07-25 02:05:06.891240 fixie_proto-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 fixie_proto-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3319 2023-07-25 15:09:30.649980 fixie_proto-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 15:10:12.374880 fixie_proto-0.1.3/gen/python/fixie_proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:10:12.378880 fixie_proto-0.1.3/gen/python/fixie_proto/fixie/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:10:12.378880 fixie_proto-0.1.3/gen/python/fixie_proto/fixie/corpora/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:10:12.378880 fixie_proto-0.1.3/gen/python/fixie_proto/fixie/corpora/v1/__init__.py
+-rw-r--r--   0        0        0     1838 2023-07-25 15:10:12.370880 fixie_proto-0.1.3/gen/python/fixie_proto/fixie/corpora/v1/common_pb2.py
+-rw-r--r--   0        0        0      847 2023-07-25 15:10:12.370880 fixie_proto-0.1.3/gen/python/fixie_proto/fixie/corpora/v1/common_pb2.pyi
+-rw-r--r--   0        0        0     3595 2023-07-25 15:10:12.370880 fixie_proto-0.1.3/gen/python/fixie_proto/fixie/corpora/v1/loader_pb2.py
+-rw-r--r--   0        0        0     2219 2023-07-25 15:10:12.370880 fixie_proto-0.1.3/gen/python/fixie_proto/fixie/corpora/v1/loader_pb2.pyi
+-rw-r--r--   0        0        0      434 2023-07-25 15:09:30.649980 fixie_proto-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 fixie_proto-0.1.3/PKG-INFO
```

### Comparing `fixie_proto-0.1.2/README.md` & `fixie_proto-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,14 @@
 
 ## Using JSON instead
 
 If you'd prefer not to deal with protos, we've got you covered! All of our APIs can accept and return JSON instead. Just set your Content-Type header to `application/json` instead of `application/proto`.
 
 Our OpenAPI spec matches the proto API. You can view it [here](https://petstore.swagger.io/?url=https://gist.githubusercontent.com/mdepinet/1382c315186d178f587f3d9ca382b74e/raw/be61192d0fe190e646cc52a494017ba7dbe3a33b/loader.swagger.json).
 
-<!-- TODO(mdepinet): Figure out how/where to publish the generated OpenAPI and then link to that here. -->
-
-
 ## Contributing
 
 ### Tools
 
 To work in this repository, you'll need to install Buf and Just. If you are using homebrew:
 
 ```
```

### Comparing `fixie_proto-0.1.2/gen/python/fixie/corpora/v1/common_pb2.py` & `fixie_proto-0.1.3/gen/python/fixie_proto/fixie/corpora/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `fixie_proto-0.1.2/gen/python/fixie/corpora/v1/loader_pb2.py` & `fixie_proto-0.1.3/gen/python/fixie_proto/fixie/corpora/v1/loader_pb2.py`

 * *Files identical despite different names*

### Comparing `fixie_proto-0.1.2/PKG-INFO` & `fixie_proto-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixie-proto
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Fixie.ai Team
 Author-email: founders@fixie.ai
 Requires-Python: >=3,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -60,17 +60,14 @@
 
 ## Using JSON instead
 
 If you'd prefer not to deal with protos, we've got you covered! All of our APIs can accept and return JSON instead. Just set your Content-Type header to `application/json` instead of `application/proto`.
 
 Our OpenAPI spec matches the proto API. You can view it [here](https://petstore.swagger.io/?url=https://gist.githubusercontent.com/mdepinet/1382c315186d178f587f3d9ca382b74e/raw/be61192d0fe190e646cc52a494017ba7dbe3a33b/loader.swagger.json).
 
-<!-- TODO(mdepinet): Figure out how/where to publish the generated OpenAPI and then link to that here. -->
-
-
 ## Contributing
 
 ### Tools
 
 To work in this repository, you'll need to install Buf and Just. If you are using homebrew:
 
 ```
```

