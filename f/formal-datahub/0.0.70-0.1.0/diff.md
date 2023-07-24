# Comparing `tmp/formal-datahub-0.0.70.tar.gz` & `tmp/formal-datahub-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-datahub-0.0.70.tar", last modified: Mon Nov  7 20:43:36 2022, max compression
+gzip compressed data, was "formal-datahub-0.1.0.tar", last modified: Tue Nov  8 00:02:51 2022, max compression
```

## Comparing `formal-datahub-0.0.70.tar` & `formal-datahub-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-07 20:43:36.570845 formal-datahub-0.0.70/
--rw-r--r--   0 junyin     (501) staff       (20)     1073 2022-07-09 20:24:59.000000 formal-datahub-0.0.70/LICENSE
--rw-r--r--   0 junyin     (501) staff       (20)     2322 2022-11-07 20:43:36.570737 formal-datahub-0.0.70/PKG-INFO
--rw-r--r--   0 junyin     (501) staff       (20)      662 2022-07-14 17:35:37.000000 formal-datahub-0.0.70/README.md
--rw-r--r--   0 junyin     (501) staff       (20)      542 2022-11-07 20:43:30.000000 formal-datahub-0.0.70/pyproject.toml
--rw-r--r--   0 junyin     (501) staff       (20)       38 2022-11-07 20:43:36.570884 formal-datahub-0.0.70/setup.cfg
-drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-07 20:43:36.569352 formal-datahub-0.0.70/src/
-drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-07 20:43:36.570095 formal-datahub-0.0.70/src/formal-datahub/
--rw-r--r--   0 junyin     (501) staff       (20)        0 2022-07-09 20:21:32.000000 formal-datahub-0.0.70/src/formal-datahub/__init__.py
--rw-r--r--   0 junyin     (501) staff       (20)     2265 2022-07-14 15:19:46.000000 formal-datahub-0.0.70/src/formal-datahub/action.py
--rw-r--r--   0 junyin     (501) staff       (20)     8691 2022-11-07 16:36:44.000000 formal-datahub-0.0.70/src/formal-datahub/formal.py
-drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-07 20:43:36.570595 formal-datahub-0.0.70/src/formal_datahub.egg-info/
--rw-r--r--   0 junyin     (501) staff       (20)     2322 2022-11-07 20:43:36.000000 formal-datahub-0.0.70/src/formal_datahub.egg-info/PKG-INFO
--rw-r--r--   0 junyin     (501) staff       (20)      289 2022-11-07 20:43:36.000000 formal-datahub-0.0.70/src/formal_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 junyin     (501) staff       (20)        1 2022-11-07 20:43:36.000000 formal-datahub-0.0.70/src/formal_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 junyin     (501) staff       (20)       15 2022-11-07 20:43:36.000000 formal-datahub-0.0.70/src/formal_datahub.egg-info/top_level.txt
+drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-08 00:02:51.232240 formal-datahub-0.1.0/
+-rw-r--r--   0 junyin     (501) staff       (20)     1073 2022-07-09 20:24:59.000000 formal-datahub-0.1.0/LICENSE
+-rw-r--r--   0 junyin     (501) staff       (20)     2341 2022-11-08 00:02:51.232094 formal-datahub-0.1.0/PKG-INFO
+-rw-r--r--   0 junyin     (501) staff       (20)      683 2022-11-08 00:00:41.000000 formal-datahub-0.1.0/README.md
+-rw-r--r--   0 junyin     (501) staff       (20)      542 2022-11-08 00:02:38.000000 formal-datahub-0.1.0/pyproject.toml
+-rw-r--r--   0 junyin     (501) staff       (20)       38 2022-11-08 00:02:51.232288 formal-datahub-0.1.0/setup.cfg
+drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-08 00:02:51.230420 formal-datahub-0.1.0/src/
+drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-08 00:02:51.231416 formal-datahub-0.1.0/src/formal-datahub/
+-rw-r--r--   0 junyin     (501) staff       (20)        0 2022-07-09 20:21:32.000000 formal-datahub-0.1.0/src/formal-datahub/__init__.py
+-rw-r--r--   0 junyin     (501) staff       (20)     2265 2022-07-14 15:19:46.000000 formal-datahub-0.1.0/src/formal-datahub/action.py
+-rw-r--r--   0 junyin     (501) staff       (20)     8666 2022-11-08 00:00:41.000000 formal-datahub-0.1.0/src/formal-datahub/formal.py
+drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-08 00:02:51.231892 formal-datahub-0.1.0/src/formal_datahub.egg-info/
+-rw-r--r--   0 junyin     (501) staff       (20)     2341 2022-11-08 00:02:51.000000 formal-datahub-0.1.0/src/formal_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 junyin     (501) staff       (20)      289 2022-11-08 00:02:51.000000 formal-datahub-0.1.0/src/formal_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 junyin     (501) staff       (20)        1 2022-11-08 00:02:51.000000 formal-datahub-0.1.0/src/formal_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 junyin     (501) staff       (20)       15 2022-11-08 00:02:51.000000 formal-datahub-0.1.0/src/formal_datahub.egg-info/top_level.txt
```

### Comparing `formal-datahub-0.0.70/LICENSE` & `formal-datahub-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-datahub-0.0.70/PKG-INFO` & `formal-datahub-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-datahub
-Version: 0.0.70
+Version: 0.1.0
 Summary: Formal Datahub Plugin
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -44,19 +44,20 @@
 
 
 Install the Formal package:
 `pip install formal-datahub`
 
 
 
-See `example` for examples. Be sure to set your secrets in environment variables.
+See `/example` for examples. Be sure to set your secrets in environment variables.
 
 
 ---
 
+# Examples
 
-Ingestion: `datahub ingest -c ingest/formal_to_datahub.dhub.yaml`
+Run Ingestion: `datahub ingest -c ingest/formal_to_datahub.dhub.yaml`
 
-
-Action: `datahub actions -c actions/datahub_to_formal.yaml`
+Run Action: `datahub actions -c actions/datahub_to_formal.yaml`
 
 If you are having trouble installing on M1, see the following: https://segmentfault.com/a/1190000040867082/en
+
```

### Comparing `formal-datahub-0.0.70/README.md` & `formal-datahub-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 
 
 Install the Formal package:
 `pip install formal-datahub`
 
 
 
-See `example` for examples. Be sure to set your secrets in environment variables.
+See `/example` for examples. Be sure to set your secrets in environment variables.
 
 
 ---
 
+# Examples
 
-Ingestion: `datahub ingest -c ingest/formal_to_datahub.dhub.yaml`
+Run Ingestion: `datahub ingest -c ingest/formal_to_datahub.dhub.yaml`
 
+Run Action: `datahub actions -c actions/datahub_to_formal.yaml`
 
-Action: `datahub actions -c actions/datahub_to_formal.yaml`
+If you are having trouble installing on M1, see the following: https://segmentfault.com/a/1190000040867082/en
 
-If you are having trouble installing on M1, see the following: https://segmentfault.com/a/1190000040867082/en
```

### Comparing `formal-datahub-0.0.70/pyproject.toml` & `formal-datahub-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "formal-datahub"
-version = "0.0.70"
+version = "0.1.00"
 authors = [
   { name="Formal", email="hello@joinformal.com" },
 ]
 description = "Formal Datahub Plugin"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `formal-datahub-0.0.70/src/formal-datahub/action.py` & `formal-datahub-0.1.0/src/formal-datahub/action.py`

 * *Files identical despite different names*

### Comparing `formal-datahub-0.0.70/src/formal-datahub/formal.py` & `formal-datahub-0.1.0/src/formal-datahub/formal.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,14 @@
                     self.report.report_workunit(wu)
 
                     yield wu
                 else:
                     log = logging.getLogger(__name__)
                     logging.basicConfig(level=logging.INFO)
 
-                    log.info(
-                        f"Tag {tag_urn} already attached to column {inv_field}, omitting write")
+                    log.info(f"Tag {tag_urn} already attached to column {inv_field}, omitting write")
 
     def get_report(self):
         return self.report
 
     def close(self):
         pass
```

### Comparing `formal-datahub-0.0.70/src/formal_datahub.egg-info/PKG-INFO` & `formal-datahub-0.1.0/src/formal_datahub.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-datahub
-Version: 0.0.70
+Version: 0.1.0
 Summary: Formal Datahub Plugin
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -44,19 +44,20 @@
 
 
 Install the Formal package:
 `pip install formal-datahub`
 
 
 
-See `example` for examples. Be sure to set your secrets in environment variables.
+See `/example` for examples. Be sure to set your secrets in environment variables.
 
 
 ---
 
+# Examples
 
-Ingestion: `datahub ingest -c ingest/formal_to_datahub.dhub.yaml`
+Run Ingestion: `datahub ingest -c ingest/formal_to_datahub.dhub.yaml`
 
-
-Action: `datahub actions -c actions/datahub_to_formal.yaml`
+Run Action: `datahub actions -c actions/datahub_to_formal.yaml`
 
 If you are having trouble installing on M1, see the following: https://segmentfault.com/a/1190000040867082/en
+
```

