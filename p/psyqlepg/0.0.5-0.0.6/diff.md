# Comparing `tmp/psyqlepg-0.0.5.tar.gz` & `tmp/psyqlepg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyqlepg-0.0.5.tar", last modified: Tue Jul 25 13:45:48 2023, max compression
+gzip compressed data, was "psyqlepg-0.0.6.tar", last modified: Tue Jul 25 13:49:13 2023, max compression
```

## Comparing `psyqlepg-0.0.5.tar` & `psyqlepg-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:45:48.984132 psyqlepg-0.0.5/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     1515 2023-07-19 09:19:30.000000 psyqlepg-0.0.5/LICENSE
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-07-25 13:45:48.984132 psyqlepg-0.0.5/PKG-INFO
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      219 2023-07-19 09:40:34.000000 psyqlepg-0.0.5/README.md
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      502 2023-07-25 13:45:33.000000 psyqlepg-0.0.5/pyproject.toml
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       38 2023-07-25 13:45:48.984132 psyqlepg-0.0.5/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:45:48.982132 psyqlepg-0.0.5/src/
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:45:48.983132 psyqlepg-0.0.5/src/psyqlepg/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     4590 2023-07-25 13:45:19.000000 psyqlepg-0.0.5/src/psyqlepg/__init__.py
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:45:48.984132 psyqlepg-0.0.5/src/psyqlepg.egg-info/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-07-25 13:45:48.000000 psyqlepg-0.0.5/src/psyqlepg.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      201 2023-07-25 13:45:48.000000 psyqlepg-0.0.5/src/psyqlepg.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        1 2023-07-25 13:45:48.000000 psyqlepg-0.0.5/src/psyqlepg.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        9 2023-07-25 13:45:48.000000 psyqlepg-0.0.5/src/psyqlepg.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:49:13.712839 psyqlepg-0.0.6/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     1515 2023-07-19 09:19:30.000000 psyqlepg-0.0.6/LICENSE
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-07-25 13:49:13.711839 psyqlepg-0.0.6/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      219 2023-07-19 09:40:34.000000 psyqlepg-0.0.6/README.md
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      502 2023-07-25 13:48:58.000000 psyqlepg-0.0.6/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       38 2023-07-25 13:49:13.712839 psyqlepg-0.0.6/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:49:13.709839 psyqlepg-0.0.6/src/
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:49:13.710839 psyqlepg-0.0.6/src/psyqlepg/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     4593 2023-07-25 13:48:36.000000 psyqlepg-0.0.6/src/psyqlepg/__init__.py
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-25 13:49:13.711839 psyqlepg-0.0.6/src/psyqlepg.egg-info/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-07-25 13:49:13.000000 psyqlepg-0.0.6/src/psyqlepg.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      201 2023-07-25 13:49:13.000000 psyqlepg-0.0.6/src/psyqlepg.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        1 2023-07-25 13:49:13.000000 psyqlepg-0.0.6/src/psyqlepg.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        9 2023-07-25 13:49:13.000000 psyqlepg-0.0.6/src/psyqlepg.egg-info/top_level.txt
```

### Comparing `psyqlepg-0.0.5/LICENSE` & `psyqlepg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psyqlepg-0.0.5/PKG-INFO` & `psyqlepg-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyqlepg
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple SQL library for psycopg3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/psyqlepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/psyqlepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `psyqlepg-0.0.5/src/psyqlepg/__init__.py` & `psyqlepg-0.0.6/src/psyqlepg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,19 @@
 
 def selectall(conn, table, where=Where(), order_by=None):
     if (order_by):
         query = sql.SQL('''
             select *
             from {table}
             where {where}
-            order_by {order_by}
+            order by {order_by}
         ''').format(
                 where=where.clause(),
                 table=sql.Identifier(table),
-                order_by=sql.Identifier(table))
+                order_by=sql.Identifier(order_by))
     else:
         query = sql.SQL('''
             select *
             from {table}
             where {where}
         ''').format(
                 where=where.clause(),
```

### Comparing `psyqlepg-0.0.5/src/psyqlepg.egg-info/PKG-INFO` & `psyqlepg-0.0.6/src/psyqlepg.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyqlepg
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple SQL library for psycopg3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/psyqlepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/psyqlepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

