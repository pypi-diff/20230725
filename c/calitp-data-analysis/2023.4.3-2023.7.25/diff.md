# Comparing `tmp/calitp_data_analysis-2023.4.3.tar.gz` & `tmp/calitp_data_analysis-2023.7.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_analysis-2023.4.3.tar", max compression
+gzip compressed data, was "calitp_data_analysis-2023.7.25.tar", max compression
```

## Comparing `calitp_data_analysis-2023.4.3.tar` & `calitp_data_analysis-2023.7.25.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-02-17 19:00:01.027281 calitp_data_analysis-2023.4.3/calitp_data_analysis/__init__.py
--rw-r--r--   0        0        0     1385 2023-02-17 19:00:01.029098 calitp_data_analysis-2023.4.3/calitp_data_analysis/magics.py
--rw-r--r--   0        0        0     5663 2023-02-17 19:00:01.029701 calitp_data_analysis-2023.4.3/calitp_data_analysis/sql.py
--rw-r--r--   0        0        0     3354 2023-02-17 19:00:01.030526 calitp_data_analysis-2023.4.3/calitp_data_analysis/tables.py
--rw-r--r--   0        0        0      605 2023-04-03 18:25:18.365708 calitp_data_analysis-2023.4.3/pyproject.toml
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 calitp_data_analysis-2023.4.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 20:14:34.415032 calitp_data_analysis-2023.7.25/calitp_data_analysis/__init__.py
+-rw-r--r--   0        0        0     1427 2023-07-24 20:14:34.415355 calitp_data_analysis-2023.7.25/calitp_data_analysis/magics.py
+-rw-r--r--   0        0        0     3981 2023-07-25 15:57:06.188713 calitp_data_analysis-2023.7.25/calitp_data_analysis/sql.py
+-rw-r--r--   0        0        0     3273 2023-07-25 15:55:15.481636 calitp_data_analysis-2023.7.25/calitp_data_analysis/tables.py
+-rw-r--r--   0        0        0      901 2023-07-25 19:38:01.858484 calitp_data_analysis-2023.7.25/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 calitp_data_analysis-2023.7.25/PKG-INFO
```

### Comparing `calitp_data_analysis-2023.4.3/calitp_data_analysis/magics.py` & `calitp_data_analysis-2023.7.25/calitp_data_analysis/magics.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 @argument(
     "-m",
     "--markdown",
     action="store_true",
     help="Print the code to markdown, in addition to running",
 )
 @argument("-o", "--output", type=str, help="A variable name to save the result as")
-@argument("-q", "--quiet", action="store_true", help="Whether to hide the result printout")
+@argument(
+    "-q", "--quiet", action="store_true", help="Whether to hide the result printout"
+)
 @register_cell_magic
 def sql(line, cell):
     # %%sql -m
     # %%sql -o tbl_result
     args = parse_argstring(sql, line)
 
     if args.markdown:
@@ -41,8 +43,12 @@
 @register_cell_magic
 def capture_parameters(line, cell):
     shell = get_ipython()
     shell.run_cell(cell, silent=True)
     # We assume the last line is a tuple
     tup = [s.strip() for s in cell.strip().split("\n")[-1].split(",")]
 
-    print(json.dumps({identifier: shell.user_ns[identifier] for identifier in tup if identifier}))
+    print(
+        json.dumps(
+            {identifier: shell.user_ns[identifier] for identifier in tup if identifier}
+        )
+    )
```

### Comparing `calitp_data_analysis-2023.4.3/calitp_data_analysis/tables.py` & `calitp_data_analysis-2023.7.25/calitp_data_analysis/tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from calitp_data.config import is_development
-from siuba.sql import LazyTbl
-from sqlalchemy.engine import Inspector
+from siuba.sql import LazyTbl  # type: ignore[import]
+from sqlalchemy.engine.reflection import Inspector
 
 from .sql import get_engine
 
 
 class AttributeDict:
     def __init__(self):
         self._d = {}
@@ -112,11 +111,10 @@
             </table>
             """
 
 
 tbls = AutoTable(
     get_engine(),
     lambda s: s,  # s.replace(".", "_"),
-    lambda s: "zzz_test_" not in s if not is_development() else True,
 )
 
 tbls._init()
```

### Comparing `calitp_data_analysis-2023.4.3/PKG-INFO` & `calitp_data_analysis-2023.7.25/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: calitp-data-analysis
-Version: 2023.4.3
+Version: 2023.7.25
 Summary: Shared code for querying Cal-ITP data in notebooks, primarily.
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: calitp-data (==2023.2.13.1)
+Requires-Dist: gcsfs (!=2022.7.1)
 Requires-Dist: ipython (>=8.9.0,<9.0.0)
 Requires-Dist: jinja2 (<3.1.0)
 Requires-Dist: pandas (<2)
 Requires-Dist: pandas-gbq (>=0.19.1,<0.20.0)
 Requires-Dist: siuba (>=0.4.2,<0.5.0)
 Requires-Dist: sqlalchemy-bigquery (>=1.6.1,<2.0.0)
```

