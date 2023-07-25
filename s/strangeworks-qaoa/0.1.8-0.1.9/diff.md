# Comparing `tmp/strangeworks_qaoa-0.1.8.tar.gz` & `tmp/strangeworks_qaoa-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qaoa-0.1.8.tar", max compression
+gzip compressed data, was "strangeworks_qaoa-0.1.9.tar", max compression
```

## Comparing `strangeworks_qaoa-0.1.8.tar` & `strangeworks_qaoa-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/LICENSE
--rw-r--r--   0        0        0      679 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/README.md
--rw-r--r--   0        0        0      791 2023-07-18 10:42:11.867814 strangeworks_qaoa-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      194 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/strangeworks_qaoa/__init__.py
--rw-r--r--   0        0        0    17638 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/strangeworks_qaoa/sdk.py
--rw-r--r--   0        0        0      691 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/strangeworks_qaoa/serializer.py
--rw-r--r--   0        0        0    12428 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/strangeworks_qaoa/utils.py
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 18:11:11.830349 strangeworks_qaoa-0.1.9/LICENSE
+-rw-r--r--   0        0        0      679 2023-07-25 18:11:11.830349 strangeworks_qaoa-0.1.9/README.md
+-rw-r--r--   0        0        0      791 2023-07-25 18:11:30.110287 strangeworks_qaoa-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-07-25 18:11:11.834349 strangeworks_qaoa-0.1.9/strangeworks_qaoa/__init__.py
+-rw-r--r--   0        0        0    17804 2023-07-25 18:11:11.834349 strangeworks_qaoa-0.1.9/strangeworks_qaoa/sdk.py
+-rw-r--r--   0        0        0      691 2023-07-25 18:11:11.834349 strangeworks_qaoa-0.1.9/strangeworks_qaoa/serializer.py
+-rw-r--r--   0        0        0    12428 2023-07-25 18:11:11.834349 strangeworks_qaoa-0.1.9/strangeworks_qaoa/utils.py
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.9/PKG-INFO
```

### Comparing `strangeworks_qaoa-0.1.8/LICENSE` & `strangeworks_qaoa-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.8/README.md` & `strangeworks_qaoa-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.8/pyproject.toml` & `strangeworks_qaoa-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-qaoa"
-version = "0.1.8"
+version = "0.1.9"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qaoa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_qaoa-0.1.8/strangeworks_qaoa/sdk.py` & `strangeworks_qaoa-0.1.9/strangeworks_qaoa/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,19 @@
             else json.dumps(False)
         )
         problem_params["warm_start"] = (
             json.dumps(problem_params["warm_start"])
             if problem_params.get("warm_start")
             else json.dumps(False)
         )
+        problem_params["qrr"] = (
+            json.dumps(problem_params["qrr"])
+            if problem_params.get("qrr")
+            else json.dumps(False)
+        )
 
         if aws is True:
             input_params = {
                 "provider": "aws",
                 "backend": backend_id,
                 "hyperparams": json.dumps(problem_params),
             }
```

### Comparing `strangeworks_qaoa-0.1.8/strangeworks_qaoa/serializer.py` & `strangeworks_qaoa-0.1.9/strangeworks_qaoa/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.8/strangeworks_qaoa/utils.py` & `strangeworks_qaoa-0.1.9/strangeworks_qaoa/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.8/PKG-INFO` & `strangeworks_qaoa-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qaoa
-Version: 0.1.8
+Version: 0.1.9
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

