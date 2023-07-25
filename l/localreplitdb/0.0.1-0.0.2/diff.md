# Comparing `tmp/localreplitdb-0.0.1.tar.gz` & `tmp/localreplitdb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localreplitdb-0.0.1.tar", max compression
+gzip compressed data, was "localreplitdb-0.0.2.tar", max compression
```

## Comparing `localreplitdb-0.0.1.tar` & `localreplitdb-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      733 2023-07-25 19:02:42.143278 localreplitdb-0.0.1/LICENSE
--rw-r--r--   0        0        0      191 2023-07-25 19:06:29.783865 localreplitdb-0.0.1/README.md
--rw-r--r--   0        0        0      197 2023-07-25 20:27:32.634017 localreplitdb-0.0.1/localreplitdb/__init__.py
--rw-r--r--   0        0        0     2894 2023-07-25 20:19:48.582079 localreplitdb-0.0.1/localreplitdb/localreplitdb.py
--rw-r--r--   0        0        0      337 2023-07-25 20:24:40.582439 localreplitdb-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    19297 2023-07-25 19:02:43.055297 localreplitdb-0.0.1/replit-py/src/replit/database/database.py
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 localreplitdb-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      733 2023-07-25 19:02:42.143278 localreplitdb-0.0.2/LICENSE
+-rw-r--r--   0        0        0      269 2023-07-25 20:43:04.649866 localreplitdb-0.0.2/README.md
+-rw-r--r--   0        0        0      201 2023-07-25 20:42:15.844100 localreplitdb-0.0.2/localreplitdb/__init__.py
+-rw-r--r--   0        0        0     2898 2023-07-25 20:31:11.108341 localreplitdb-0.0.2/localreplitdb/localreplitdb.py
+-rw-r--r--   0        0        0    19297 2023-07-25 20:42:01.328871 localreplitdb-0.0.2/localreplitdb/realreplitdb.py
+-rw-r--r--   0        0        0      337 2023-07-25 20:43:29.497255 localreplitdb-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    19297 2023-07-25 19:02:43.055297 localreplitdb-0.0.2/replit-py/src/replit/database/database.py
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 localreplitdb-0.0.2/PKG-INFO
```

### Comparing `localreplitdb-0.0.1/LICENSE` & `localreplitdb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `localreplitdb-0.0.1/localreplitdb/localreplitdb.py` & `localreplitdb-0.0.2/localreplitdb/localreplitdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,10 +82,10 @@
         """Close the database file handle."""
         self.db.close()
 
 
 db_path = "local_replit_db.db"
 db: LocalDatabase | None = LocalDatabase(db_path)
 
-if not db:
+if db is None:
     # The user will see errors if they try to use the database.
     print('Warning: error initializing database. Replit DB is not configured.')
```

### Comparing `localreplitdb-0.0.1/replit-py/src/replit/database/database.py` & `localreplitdb-0.0.2/localreplitdb/realreplitdb.py`

 * *Files identical despite different names*

### Comparing `localreplitdb-0.0.1/PKG-INFO` & `localreplitdb-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localreplitdb
-Version: 0.0.1
+Version: 0.0.2
 Summary: JSON file-backed DB emuulating replit db's API
 License: ISC
 Author: Dev380
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,7 +17,11 @@
 
 # Local Replit DB
 
 Replit DB but as a local file because I can't be bothered to use a real DB when migrating off replit. Backed by TinyDB.
 
 Default db is a file in current working directory.
 
+### Building
+
+Please run prebuild.sh because of some stupid symlink thing :D
+
```

