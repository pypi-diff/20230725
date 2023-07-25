# Comparing `tmp/sol_orm_lib-0.1.1.tar.gz` & `tmp/sol_orm_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sol_orm_lib-0.1.1.tar", max compression
+gzip compressed data, was "sol_orm_lib-0.1.2.tar", max compression
```

## Comparing `sol_orm_lib-0.1.1.tar` & `sol_orm_lib-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      778 2023-07-11 17:20:01.717941 sol_orm_lib-0.1.1/README.md
--rw-r--r--   0        0        0      470 2023-07-11 17:20:01.717941 sol_orm_lib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 17:20:01.717941 sol_orm_lib-0.1.1/sol_orm_lib/__init__.py
--rw-r--r--   0        0        0      503 2023-07-11 17:20:01.717941 sol_orm_lib-0.1.1/sol_orm_lib/database.py
--rw-r--r--   0        0        0      440 2023-07-11 17:20:01.717941 sol_orm_lib-0.1.1/sol_orm_lib/models.py
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 sol_orm_lib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      684 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/README.md
+-rw-r--r--   0        0        0      511 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/sol_orm_lib/__init__.py
+-rw-r--r--   0        0        0     2742 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/sol_orm_lib/models.py
+-rw-r--r--   0        0        0     4646 2023-07-25 15:39:54.031463 sol_orm_lib-0.1.2/sol_orm_lib/sol_orm.py
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 sol_orm_lib-0.1.2/PKG-INFO
```

### Comparing `sol_orm_lib-0.1.1/PKG-INFO` & `sol_orm_lib-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Metadata-Version: 2.1
 Name: sol-orm-lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/idener/SOL-Python-ORM-Library
 Author: Antonio Gomez
 Author-email: antonio.gomez@idener.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: pydantic (==1.10.9)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/idener/SOL-Python-ORM-Library
 Description-Content-Type: text/markdown
 
 # SOL Python ORM Library
 
 ## Installation
 ```
 pip install sol-orm-lib
 ```
 
 ## Example usage
 ```python
-from sol_orm_lib.models import TACs, TICs
-from sol_orm_lib.database import post_tics_data
+from sol_orm_lib.models import *
+from sol_orm_lib.sol_orm import SolORM
 
-tics_data = TICs(
-    timestamp=1625779123,
-    pvPlannedDown=True,
-    stgPlannedDown=True,
-    allPlannedDown=True,
-    taCs=[
-        TACs(k=1, ktic='some_string', n=1, timestamp=1625779123),
-        # add more objects if needed
-    ]
+# Instantiate SolORM object
+db = SolORM("https://db-api.sol.idener.es")
+
+# Create an object 
+mw = MeasuredWeather(
+    rad_ar=27.2,
+    temp_ar=39,
+    wind_ar=12,
+    timestamp=current_milli_time(),
 )
 
-reponse = post_tics_data(tics_data)
+# Add it to the DB
+response = db.add_entity(mw)
 print(response)
 ```
 
-**NOTE**: The library expects the environment variable 'DB_API_URL' to be set.
-
 ## Release process
 To release a new version of the package, update the version number in the `pyproject.toml` file and publish a release with the same tag. The CI will build and publish the package to PyPI.
```

