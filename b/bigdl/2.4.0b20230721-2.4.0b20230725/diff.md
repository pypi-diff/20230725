# Comparing `tmp/bigdl-2.4.0b20230721-py3-none-manylinux1_x86_64.whl.zip` & `tmp/bigdl-2.4.0b20230725-py3-none-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1757 bytes, number of entries: 5
--rw-------  2.0 unx     1118 b- defN 23-Jul-21 13:45 bigdl-2.4.0b20230721.dist-info/METADATA
--rw-------  2.0 unx      106 b- defN 23-Jul-21 13:45 bigdl-2.4.0b20230721.dist-info/WHEEL
--rw-------  2.0 unx       68 b- defN 23-Jul-21 13:45 bigdl-2.4.0b20230721.dist-info/dependency_links.txt
--rw-------  2.0 unx        1 b- defN 23-Jul-21 13:45 bigdl-2.4.0b20230721.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      432 b- defN 23-Jul-21 13:45 bigdl-2.4.0b20230721.dist-info/RECORD
-5 files, 1725 bytes uncompressed, 941 bytes compressed:  45.4%
+Zip file size: 1759 bytes, number of entries: 5
+-rw-------  2.0 unx     1118 b- defN 23-Jul-25 13:44 bigdl-2.4.0b20230725.dist-info/METADATA
+-rw-------  2.0 unx      106 b- defN 23-Jul-25 13:44 bigdl-2.4.0b20230725.dist-info/WHEEL
+-rw-------  2.0 unx       68 b- defN 23-Jul-25 13:44 bigdl-2.4.0b20230725.dist-info/dependency_links.txt
+-rw-------  2.0 unx        1 b- defN 23-Jul-25 13:44 bigdl-2.4.0b20230725.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      432 b- defN 23-Jul-25 13:44 bigdl-2.4.0b20230725.dist-info/RECORD
+5 files, 1725 bytes uncompressed, 943 bytes compressed:  45.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: bigdl-2.4.0b20230721.dist-info/METADATA
+Filename: bigdl-2.4.0b20230725.dist-info/METADATA
 Comment: 
 
-Filename: bigdl-2.4.0b20230721.dist-info/WHEEL
+Filename: bigdl-2.4.0b20230725.dist-info/WHEEL
 Comment: 
 
-Filename: bigdl-2.4.0b20230721.dist-info/dependency_links.txt
+Filename: bigdl-2.4.0b20230725.dist-info/dependency_links.txt
 Comment: 
 
-Filename: bigdl-2.4.0b20230721.dist-info/top_level.txt
+Filename: bigdl-2.4.0b20230725.dist-info/top_level.txt
 Comment: 
 
-Filename: bigdl-2.4.0b20230721.dist-info/RECORD
+Filename: bigdl-2.4.0b20230725.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bigdl-2.4.0b20230721.dist-info/METADATA` & `bigdl-2.4.0b20230725.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: bigdl
-Version: 2.4.0b20230721
+Version: 2.4.0b20230725
 Summary: Building Large-Scale AI Applications for Distributed Big Data
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: mac
 Platform: linux
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
-Requires-Dist: bigdl-orca (==2.4.0b20230721)
-Requires-Dist: bigdl-nano (==2.4.0b20230721)
-Requires-Dist: bigdl-chronos (==2.4.0b20230721)
-Requires-Dist: bigdl-friesian (==2.4.0b20230721)
-Requires-Dist: bigdl-serving (==2.4.0b20230721)
+Requires-Dist: bigdl-orca (==2.4.0b20230725)
+Requires-Dist: bigdl-nano (==2.4.0b20230725)
+Requires-Dist: bigdl-chronos (==2.4.0b20230725)
+Requires-Dist: bigdl-friesian (==2.4.0b20230725)
+Requires-Dist: bigdl-serving (==2.4.0b20230725)
 
 
 [**BigDL**](https://github.com/intel-analytics/BigDL/)
 makes it easy for data scientists and data engineers to build end-to-end, 
 distributed AI applications.
 
 For more information, you may [read the docs](https://bigdl.readthedocs.io/).
```

