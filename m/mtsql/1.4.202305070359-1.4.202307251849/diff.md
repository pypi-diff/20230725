# Comparing `tmp/mtsql-1.4.202305070359-py3-none-any.whl.zip` & `tmp/mtsql-1.4.202307251849-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19241 bytes, number of entries: 11
--rw-r--r--  2.0 unx       44 b- defN 22-Dec-30 06:14 mt/sql/__init__.py
--rw-r--r--  2.0 unx     9994 b- defN 23-May-07 03:59 mt/sql/base.py
--rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 12:37 mt/sql/mysql.py
--rw-r--r--  2.0 unx    65252 b- defN 23-May-07 03:37 mt/sql/psql.py
--rw-r--r--  2.0 unx     8678 b- defN 23-Feb-27 00:37 mt/sql/sqlite.py
--rw-r--r--  2.0 unx      396 b- defN 23-May-07 03:59 mt/sql/version.py
--rw-r--r--  2.0 unx     1070 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/LICENSE
--rw-r--r--  2.0 unx      597 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 23-May-07 03:59 mtsql-1.4.202305070359.dist-info/RECORD
-11 files, 91883 bytes uncompressed, 17787 bytes compressed:  80.6%
+Zip file size: 19220 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       44 b- defN 23-Jan-22 22:24 mt/sql/__init__.py
+-rw-r--r--  2.0 unx     9994 b- defN 23-May-11 07:16 mt/sql/base.py
+-rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 11:50 mt/sql/mysql.py
+-rw-r--r--  2.0 unx    65224 b- defN 23-Jul-25 18:48 mt/sql/psql.py
+-rw-r--r--  2.0 unx     8678 b- defN 23-Feb-23 10:22 mt/sql/sqlite.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Jul-25 18:49 mt/sql/version.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/LICENSE
+-rw-r--r--  2.0 unx      597 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/RECORD
+11 files, 91855 bytes uncompressed, 17766 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mt/sql/sqlite.py
 Comment: 
 
 Filename: mt/sql/version.py
 Comment: 
 
-Filename: mtsql-1.4.202305070359.dist-info/LICENSE
+Filename: mtsql-1.4.202307251849.dist-info/LICENSE
 Comment: 
 
-Filename: mtsql-1.4.202305070359.dist-info/METADATA
+Filename: mtsql-1.4.202307251849.dist-info/METADATA
 Comment: 
 
-Filename: mtsql-1.4.202305070359.dist-info/WHEEL
+Filename: mtsql-1.4.202307251849.dist-info/WHEEL
 Comment: 
 
-Filename: mtsql-1.4.202305070359.dist-info/top_level.txt
+Filename: mtsql-1.4.202307251849.dist-info/top_level.txt
 Comment: 
 
-Filename: mtsql-1.4.202305070359.dist-info/RECORD
+Filename: mtsql-1.4.202307251849.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/sql/psql.py

```diff
@@ -2,18 +2,16 @@
 
 import sqlalchemy as sa
 import re
 import psycopg2 as ps
 import sqlalchemy.exc as se
 from tqdm import tqdm  # nice progress bar
 
-from mt import tp, logg, pd, np
-import mt.base.path as _p
+from mt import tp, logg, pd, np, path, ctx
 from mt.base.bg_invoke import BgInvoke
-from mt.base.with_utils import dummy_scope
 
 from .base import *
 
 
 __all__ = [
     "pg_get_locked_transactions",
     "pg_cancel_backend",
@@ -1369,21 +1367,21 @@
     frame_sql_str = frame_sql(table_name, schema=schema)
 
     with logger.scoped_debug(
         "Comparing table: local '{}' <-> remote '{}'".format(
             df_filepath, frame_sql_str
         ),
         curly=False,
-    ) if logger else dummy_scope:
+    ) if logger else ctx.nullcontext():
         # make sure the folder containing the CSV file exists
-        data_dir = _p.dirname(df_filepath)
-        _p.make_dirs(data_dir)
+        data_dir = path.dirname(df_filepath)
+        path.make_dirs(data_dir)
 
         # local_df
-        if _p.exists(df_filepath):
+        if path.exists(df_filepath):
             try:
                 if df_filepath.endswith(".parquet"):
                     local_df = pd.dfload(df_filepath, show_progress=True)
                 else:
                     local_df = pd.dfload(
                         df_filepath, index_col=id_name, show_progress=True
                     )
@@ -1436,15 +1434,15 @@
             else:
                 query_str = "select {}, md5({}) as {} from {}".format(
                     id_name, text, hash_name, frame_sql_str
                 )
 
             with logger.scoped_debug(
                 "Range of '{}'".format(id_name), curly=False
-            ) if logger else dummy_scope:
+            ) if logger else ctx.nullcontext():
                 qsql = "SELECT min({}) AS val FROM ({}) ct_t0".format(
                     id_name, query_str
                 )
                 df = read_sql(qsql, engine, nb_trials=nb_trials, logger=logger)
                 min_id = df["val"][0]
                 if logger:
                     logger.debug("Min: {}".format(min_id))
@@ -1645,15 +1643,15 @@
                     "Keyword argument 'conn_ro' is becoming deprecated. Please replace it 'engine_ro' instead."
                 )
             engine_ro = conn_ro
     frame_sql_str = frame_sql(table_name, schema=schema)
     with logger.scoped_debug(
         "Writing table: local '{}' -> remote '{}'".format(df_filepath, frame_sql_str),
         curly=False,
-    ) if logger else dummy_scope:
+    ) if logger else ctx.nullcontext():
         (
             local_df,
             remote_md5_df,
             same_keys,
             diff_keys,
             local_only_keys,
             remote_only_keys,
@@ -1888,15 +1886,15 @@
         If bg_write_csv is True, this represents the background thread for writing the updated CSV
         file. If no background thread is needed, None is returned.
     """
     frame_sql_str = frame_sql(table_name, schema=schema)
     with logger.scoped_debug(
         "Reading table: local '{}' <- remote '{}'".format(df_filepath, frame_sql_str),
         curly=False,
-    ) if logger else dummy_scope:
+    ) if logger else ctx.nullcontext():
         (
             local_df,
             remote_md5_df,
             same_keys,
             diff_keys,
             local_only_keys,
             remote_only_keys,
```

## mt/sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('05')
-VERSION_DAY = int('07')
-VERSION_HOUR = int('03')
-VERSION_MINUTE = int('59')
+VERSION_MONTH = int('07')
+VERSION_DAY = int('25')
+VERSION_HOUR = int('18')
+VERSION_MINUTE = int('49')
 MAJOR_VERSION = 1
 MINOR_VERSION = 4
-PATCH_VERSION = 202305070359
-version_date = '2023/05/07 03:59'
+PATCH_VERSION = 202307251849
+version_date = '2023/07/25 18:49'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtsql-1.4.202305070359.dist-info/LICENSE` & `mtsql-1.4.202307251849.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtsql-1.4.202305070359.dist-info/METADATA` & `mtsql-1.4.202307251849.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsql
-Version: 1.4.202305070359
+Version: 1.4.202307251849
 Summary: Extra Python modules to deal with the interaction between pandas dataframes and remote SQL servers, for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtsql
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.sql/mt.sql.html
 Project-URL: Source Code, https://github.com/inteplus/mtsql
 License-File: LICENSE
 Requires-Dist: sqlalchemy (>=2.0)
```

