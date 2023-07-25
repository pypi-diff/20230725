# Comparing `tmp/bento_meta-0.2.2.tar.gz` & `tmp/bento_meta-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_meta-0.2.2.tar", max compression
+gzip compressed data, was "bento_meta-0.2.3.tar", max compression
```

## Comparing `bento_meta-0.2.2.tar` & `bento_meta-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0    11446 2023-07-21 22:20:26.966968 bento_meta-0.2.2/LICENSE
--rw-r--r--   0        0        0      157 2023-07-21 22:20:26.966968 bento_meta-0.2.2/README.md
--rw-r--r--   0        0        0     2772 2023-07-21 22:20:26.970968 bento_meta-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    10416 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/compare_models.py
--rw-r--r--   0        0        0     5809 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/compare_val_set_terms.py
--rw-r--r--   0        0        0    15577 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/make_diff_changelog.py
--rw-r--r--   0        0        0    10021 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/make_mapping_changelog.py
--rw-r--r--   0        0        0    11554 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/make_model_changelog.py
--rw-r--r--   0        0        0       70 2023-07-21 22:20:26.970968 bento_meta-0.2.2/src/bento_meta/__init__.py
--rw-r--r--   0        0        0    23264 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/entity.py
--rw-r--r--   0        0        0      502 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/logs/log.ini
--rw-r--r--   0        0        0      388 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/__init__.py
--rw-r--r--   0        0        0     8997 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/loaders.py
--rw-r--r--   0        0        0    13439 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/mdb.py
--rw-r--r--   0        0        0       89 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/mdb_tools/__init__.py
--rw-r--r--   0        0        0    31805 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/mdb_tools/mdb_tools.py
--rw-r--r--   0        0        0     3606 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/searchable.py
--rw-r--r--   0        0        0     2426 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/writeable.py
--rw-r--r--   0        0        0    19629 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/model.py
--rw-r--r--   0        0        0    26098 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/object_map.py
--rw-r--r--   0        0        0    11048 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/objects.py
--rw-r--r--   0        0        0      196 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/__init__.py
--rw-r--r--   0        0        0    15507 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/_engine.py
--rw-r--r--   0        0        0       87 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/cypher/__init__.py
--rw-r--r--   0        0        0     9414 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/cypher/clauses.py
--rw-r--r--   0        0        0    19302 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/cypher/entities.py
--rw-r--r--   0        0        0     2067 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/cypher/functions.py
--rw-r--r--   0        0        0     2532 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/makeq.py
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 bento_meta-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11446 2020-10-16 17:49:04.916483 bento_meta-0.2.3/LICENSE
+-rw-r--r--   0        0        0      157 2020-10-16 17:49:04.917102 bento_meta-0.2.3/README.md
+-rw-r--r--   0        0        0     2772 2023-07-25 02:13:20.437592 bento_meta-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    10416 2023-07-25 02:04:10.033275 bento_meta-0.2.3/scripts/compare_models.py
+-rw-r--r--   0        0        0     5809 2023-07-25 02:04:10.033829 bento_meta-0.2.3/scripts/compare_val_set_terms.py
+-rw-r--r--   0        0        0    15577 2023-07-25 02:04:10.034290 bento_meta-0.2.3/scripts/make_diff_changelog.py
+-rw-r--r--   0        0        0    10021 2023-07-25 02:04:10.034525 bento_meta-0.2.3/scripts/make_mapping_changelog.py
+-rw-r--r--   0        0        0    11554 2023-07-25 02:04:10.034824 bento_meta-0.2.3/scripts/make_model_changelog.py
+-rw-r--r--   0        0        0       70 2023-02-08 23:10:38.928433 bento_meta-0.2.3/src/bento_meta/__init__.py
+-rw-r--r--   0        0        0    23264 2023-07-25 02:04:10.035350 bento_meta-0.2.3/src/bento_meta/entity.py
+-rw-r--r--   0        0        0      502 2023-02-12 23:42:52.168386 bento_meta-0.2.3/src/bento_meta/logs/log.ini
+-rw-r--r--   0        0        0      388 2023-02-08 23:10:38.930201 bento_meta-0.2.3/src/bento_meta/mdb/__init__.py
+-rw-r--r--   0        0        0     8997 2023-05-23 18:53:13.655094 bento_meta-0.2.3/src/bento_meta/mdb/loaders.py
+-rw-r--r--   0        0        0    13470 2023-07-25 02:13:20.438536 bento_meta-0.2.3/src/bento_meta/mdb/mdb.py
+-rw-r--r--   0        0        0       89 2023-07-25 02:04:10.035731 bento_meta-0.2.3/src/bento_meta/mdb/mdb_tools/__init__.py
+-rw-r--r--   0        0        0    31805 2023-07-25 02:04:10.036192 bento_meta-0.2.3/src/bento_meta/mdb/mdb_tools/mdb_tools.py
+-rw-r--r--   0        0        0     3606 2023-07-10 20:45:05.642211 bento_meta-0.2.3/src/bento_meta/mdb/searchable.py
+-rw-r--r--   0        0        0     2426 2023-02-08 23:10:38.934620 bento_meta-0.2.3/src/bento_meta/mdb/writeable.py
+-rw-r--r--   0        0        0    19629 2023-05-23 18:53:13.656567 bento_meta-0.2.3/src/bento_meta/model.py
+-rw-r--r--   0        0        0    26098 2023-07-10 20:45:05.643169 bento_meta-0.2.3/src/bento_meta/object_map.py
+-rw-r--r--   0        0        0    11048 2023-07-25 02:04:10.036650 bento_meta-0.2.3/src/bento_meta/objects.py
+-rw-r--r--   0        0        0      196 2023-02-08 23:10:38.940527 bento_meta-0.2.3/src/bento_meta/util/__init__.py
+-rw-r--r--   0        0        0    15507 2023-02-08 23:10:38.941405 bento_meta-0.2.3/src/bento_meta/util/_engine.py
+-rw-r--r--   0        0        0       87 2023-02-08 23:10:38.942242 bento_meta-0.2.3/src/bento_meta/util/cypher/__init__.py
+-rw-r--r--   0        0        0     9414 2023-07-25 02:04:10.037159 bento_meta-0.2.3/src/bento_meta/util/cypher/clauses.py
+-rw-r--r--   0        0        0    19302 2023-02-08 23:10:38.944679 bento_meta-0.2.3/src/bento_meta/util/cypher/entities.py
+-rw-r--r--   0        0        0     2067 2023-02-08 23:10:38.945608 bento_meta-0.2.3/src/bento_meta/util/cypher/functions.py
+-rw-r--r--   0        0        0    24424 2022-02-25 15:35:38.969950 bento_meta-0.2.3/src/bento_meta/util/cypher.py.old
+-rw-r--r--   0        0        0     2532 2023-02-08 23:10:38.946393 bento_meta-0.2.3/src/bento_meta/util/makeq.py
+-rw-r--r--   0        0        0     4910 2022-01-28 18:56:52.458052 bento_meta-0.2.3/src/bento_meta/util/query_paths.yml
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 bento_meta-0.2.3/setup.py
+-rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 bento_meta-0.2.3/PKG-INFO
```

### Comparing `bento_meta-0.2.2/LICENSE` & `bento_meta-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/pyproject.toml` & `bento_meta-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bento-meta"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python drivers for Bento Metamodel Database"
 authors = [
   { name="Mark A. Jensen", email = "mark.jensen@nih.gov"},
   { name="Mark Benson", email = "mark.benson@nih.gov"},
   { name="Nelson Moore", email = "nelson.moore@essential-soft.com"}
 ]
 requires-python = ">=3.8"
@@ -16,15 +16,15 @@
 
 [project.urls]
 "Homepage" = "https://cbiit.github.io/bento-meta/"
 "Bug Tracker" = "https://github.com/CBIIT/bento-meta/issues"
 
 [tool.poetry]
 name = "bento-meta"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python drivers for Bento Metamodel Database"
 authors = [
     "Mark A. Jensen <mark.jensen@nih.gov>",
     "Mark Benson <mark.benson@nih.gov>",
     "Nelson Moore <nelson.moore@essential-soft.com>"
 ]
 license = "Apache 2.0"
```

### Comparing `bento_meta-0.2.2/scripts/compare_models.py` & `bento_meta-0.2.3/scripts/compare_models.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/scripts/compare_val_set_terms.py` & `bento_meta-0.2.3/scripts/compare_val_set_terms.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/scripts/make_diff_changelog.py` & `bento_meta-0.2.3/scripts/make_diff_changelog.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/scripts/make_mapping_changelog.py` & `bento_meta-0.2.3/scripts/make_mapping_changelog.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/scripts/make_model_changelog.py` & `bento_meta-0.2.3/scripts/make_model_changelog.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/entity.py` & `bento_meta-0.2.3/src/bento_meta/entity.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/mdb/loaders.py` & `bento_meta-0.2.3/src/bento_meta/mdb/loaders.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/mdb/mdb.py` & `bento_meta-0.2.3/src/bento_meta/mdb/mdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,16 +240,16 @@
     @read_txn_data
     def get_term_by_id(self, nanoid):
         """Get a term having the given nanoid, with its origin.
         Returns {term, origin}."""
         qry = (
             "match (t:term {nanoid:$nanoid}) "
             "where not exists(t._to) "
-            "with t "
-            "optional match (t)-[:has_origin]->(o:origin) "
+            "with t, t.origin_name as origin_name "
+            "optional match (o:origin {name: origin_name}) "
             "where not exists(o._to) "
             "return t as term, o as origin "
             )
         return (qry, {"nanoid": nanoid})
 
     @read_txn_data
     def get_props_and_terms_by_model(self, model=None):
```

### Comparing `bento_meta-0.2.2/src/bento_meta/mdb/mdb_tools/mdb_tools.py` & `bento_meta-0.2.3/src/bento_meta/mdb/mdb_tools/mdb_tools.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/mdb/searchable.py` & `bento_meta-0.2.3/src/bento_meta/mdb/searchable.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/mdb/writeable.py` & `bento_meta-0.2.3/src/bento_meta/mdb/writeable.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/model.py` & `bento_meta-0.2.3/src/bento_meta/model.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/object_map.py` & `bento_meta-0.2.3/src/bento_meta/object_map.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/objects.py` & `bento_meta-0.2.3/src/bento_meta/objects.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/util/_engine.py` & `bento_meta-0.2.3/src/bento_meta/util/_engine.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/util/cypher/clauses.py` & `bento_meta-0.2.3/src/bento_meta/util/cypher/clauses.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/util/cypher/entities.py` & `bento_meta-0.2.3/src/bento_meta/util/cypher/entities.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/util/cypher/functions.py` & `bento_meta-0.2.3/src/bento_meta/util/cypher/functions.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/src/bento_meta/util/makeq.py` & `bento_meta-0.2.3/src/bento_meta/util/makeq.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.2.2/PKG-INFO` & `bento_meta-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-meta
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python drivers for Bento Metamodel Database
 License: Apache 2.0
 Author: Mark A. Jensen
 Author-email: mark.jensen@nih.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

