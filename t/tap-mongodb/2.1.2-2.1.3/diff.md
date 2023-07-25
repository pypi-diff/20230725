# Comparing `tmp/tap-mongodb-2.1.2.tar.gz` & `tmp/tap-mongodb-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mongodb-2.1.2.tar", last modified: Fri Jul  1 13:31:26 2022, max compression
+gzip compressed data, was "tap-mongodb-2.1.3.tar", last modified: Tue Jul 25 19:32:34 2023, max compression
```

## Comparing `tap-mongodb-2.1.2.tar` & `tap-mongodb-2.1.3.tar`

### file list

```diff
@@ -1,20 +1,43 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-01 13:31:26.019934 tap-mongodb-2.1.2/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    32386 2020-12-15 18:13:24.000000 tap-mongodb-2.1.2/LICENSE
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      298 2022-07-01 13:31:26.019934 tap-mongodb-2.1.2/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3667 2020-12-15 18:13:24.000000 tap-mongodb-2.1.2/README.md
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       38 2022-07-01 13:31:26.019934 tap-mongodb-2.1.2/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      782 2022-07-01 13:30:49.000000 tap-mongodb-2.1.2/setup.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-01 13:31:26.015934 tap-mongodb-2.1.2/tap_mongodb/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14726 2022-04-15 15:04:26.000000 tap-mongodb-2.1.2/tap_mongodb/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-01 13:31:26.019934 tap-mongodb-2.1.2/tap_mongodb/sync_strategies/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    13349 2021-09-27 18:34:42.000000 tap-mongodb-2.1.2/tap_mongodb/sync_strategies/common.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6791 2022-04-18 18:46:22.000000 tap-mongodb-2.1.2/tap_mongodb/sync_strategies/full_table.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5170 2022-04-18 18:46:22.000000 tap-mongodb-2.1.2/tap_mongodb/sync_strategies/incremental.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10900 2022-04-18 18:46:22.000000 tap-mongodb-2.1.2/tap_mongodb/sync_strategies/oplog.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-01 13:31:26.019934 tap-mongodb-2.1.2/tap_mongodb.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      298 2022-07-01 13:31:25.000000 tap-mongodb-2.1.2/tap_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      422 2022-07-01 13:31:25.000000 tap-mongodb-2.1.2/tap_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2022-07-01 13:31:25.000000 tap-mongodb-2.1.2/tap_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       49 2022-07-01 13:31:25.000000 tap-mongodb-2.1.2/tap_mongodb.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       98 2022-07-01 13:31:25.000000 tap-mongodb-2.1.2/tap_mongodb.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       12 2022-07-01 13:31:25.000000 tap-mongodb-2.1.2/tap_mongodb.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.252862 tap-mongodb-2.1.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32386 2023-04-20 13:58:35.000000 tap-mongodb-2.1.3/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-07-25 19:32:34.252862 tap-mongodb-2.1.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3667 2023-04-20 13:58:35.000000 tap-mongodb-2.1.3/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-25 19:32:34.252862 tap-mongodb-2.1.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      782 2023-07-25 19:32:02.000000 tap-mongodb-2.1.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.236862 tap-mongodb-2.1.3/tap_mongodb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14726 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tap_mongodb/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.240862 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13349 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6988 2023-07-25 18:29:25.000000 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/full_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5170 2023-04-20 13:58:35.000000 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/incremental.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10900 2023-07-25 17:28:52.000000 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/oplog.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.236862 tap-mongodb-2.1.3/tap_mongodb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1253 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.252862 tap-mongodb-2.1.3/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11331 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_cname_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6918 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_configurable_properties.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10014 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_datatype.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11497 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13941 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_fname_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12712 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_full_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10542 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_full_table_id.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10412 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_full_table_interruptible.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10648 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_id_pk_variations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25133 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_incremental.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13090 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_incremental_open_transactions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6285 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14615 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_log_based_interruptible.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12493 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_name_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11531 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_namespace_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11077 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_oplog.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6753 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_oplog_aged_out.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9714 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_oplog_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9763 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_projection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12817 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_table_reset_inc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8070 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_table_reset_log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5635 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_views.py
```

### Comparing `tap-mongodb-2.1.2/LICENSE` & `tap-mongodb-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.2/README.md` & `tap-mongodb-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.2/setup.py` & `tap-mongodb-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-mongodb',
-      version='2.1.2',
+      version='2.1.3',
       description='Singer.io tap for extracting data from MongoDB',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mongodb'],
       install_requires=[
           'singer-python==5.8.0',
```

### Comparing `tap-mongodb-2.1.2/tap_mongodb/__init__.py` & `tap-mongodb-2.1.3/tap_mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.2/tap_mongodb/sync_strategies/common.py` & `tap-mongodb-2.1.3/tap_mongodb/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.2/tap_mongodb/sync_strategies/full_table.py` & `tap-mongodb-2.1.3/tap_mongodb/sync_strategies/full_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 import pymongo
 import singer
 from singer import metadata, utils
 import tap_mongodb.sync_strategies.common as common
 
 LOGGER = singer.get_logger()
 
-def get_max_id_value(collection):
-    row = collection.find_one(sort=[("_id", pymongo.DESCENDING)])
+def get_max_id_value(collection, projection=None):
+    if projection is None:
+        row = collection.find_one(sort=[("_id", pymongo.DESCENDING)])
+    else:
+        row = collection.find_one(sort=[("_id", pymongo.DESCENDING)],
+                                  projection=projection)
     if row:
         return row['_id']
 
     LOGGER.info("No max id found for collection: collection is likely empty")
     return None
 
 
@@ -60,15 +64,15 @@
 
     if singer.get_bookmark(state, stream['tap_stream_id'], 'max_id_value'):
         # There is a bookmark
         max_id_value = singer.get_bookmark(state, stream['tap_stream_id'], 'max_id_value')
         max_id_type = singer.get_bookmark(state, stream['tap_stream_id'], 'max_id_type')
         max_id_value = common.string_to_class(max_id_value, max_id_type)
     else:
-        max_id_value = get_max_id_value(collection)
+        max_id_value = get_max_id_value(collection, projection)
 
     last_id_fetched = singer.get_bookmark(state,
                                           stream['tap_stream_id'],
                                           'last_id_fetched')
 
     if max_id_value:
         # Write the bookmark if max_id_value is defined
```

### Comparing `tap-mongodb-2.1.2/tap_mongodb/sync_strategies/incremental.py` & `tap-mongodb-2.1.3/tap_mongodb/sync_strategies/incremental.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.2/tap_mongodb/sync_strategies/oplog.py` & `tap-mongodb-2.1.3/tap_mongodb/sync_strategies/oplog.py`

 * *Files identical despite different names*

