# Comparing `tmp/spark_utils-1.1.1.tar.gz` & `tmp/spark_utils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_utils-1.1.1.tar", max compression
+gzip compressed data, was "spark_utils-1.1.2.tar", max compression
```

## Comparing `spark_utils-1.1.1.tar` & `spark_utils-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-07-10 08:41:14.574930 spark_utils-1.1.1/LICENSE
--rw-r--r--   0        0        0     6766 2023-07-10 08:41:14.574930 spark_utils-1.1.1/README.md
--rw-r--r--   0        0        0      791 2023-07-10 08:41:35.873870 spark_utils-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/__init__.py
--rw-r--r--   0        0        0       22 2023-07-10 08:41:35.873870 spark_utils-1.1.1/spark_utils/_version.py
--rw-r--r--   0        0        0     1134 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/__init__.py
--rw-r--r--   0        0        0     4257 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/functions.py
--rw-r--r--   0        0        0     5977 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/spark_job_args.py
--rw-r--r--   0        0        0    11437 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/spark_session_provider.py
--rw-r--r--   0        0        0     3381 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/spark_sql_utils.py
--rw-r--r--   0        0        0     1449 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/common/spark_udf.py
--rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/__init__.py
--rw-r--r--   0        0        0    10376 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/functions.py
--rw-r--r--   0        0        0     2325 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/models.py
--rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/sets/__init__.py
--rw-r--r--   0        0        0     1631 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/dataframes/sets/functions.py
--rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/delta_lake/__init__.py
--rw-r--r--   0        0        0     1691 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/delta_lake/delta_log.py
--rw-r--r--   0        0        0     5982 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/delta_lake/functions.py
--rw-r--r--   0        0        0     1135 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/hive_metastore_config.py
--rw-r--r--   0        0        0     1318 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/hive_table.py
--rw-r--r--   0        0        0     1868 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/job_socket.py
--rw-r--r--   0        0        0     1129 2023-07-10 08:41:14.578930 spark_utils-1.1.1/spark_utils/models/k8s_config.py
--rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 spark_utils-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-25 14:18:04.838493 spark_utils-1.1.2/LICENSE
+-rw-r--r--   0        0        0     6766 2023-07-25 14:18:04.838493 spark_utils-1.1.2/README.md
+-rw-r--r--   0        0        0      791 2023-07-25 14:18:26.890892 spark_utils-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-25 14:18:26.890892 spark_utils-1.1.2/spark_utils/_version.py
+-rw-r--r--   0        0        0     1134 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/__init__.py
+-rw-r--r--   0        0        0     4257 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/functions.py
+-rw-r--r--   0        0        0     5977 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/spark_job_args.py
+-rw-r--r--   0        0        0    11709 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/spark_session_provider.py
+-rw-r--r--   0        0        0     3381 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/spark_sql_utils.py
+-rw-r--r--   0        0        0     1449 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/spark_udf.py
+-rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0    10376 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/functions.py
+-rw-r--r--   0        0        0     2325 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/models.py
+-rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/sets/__init__.py
+-rw-r--r--   0        0        0     1631 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/sets/functions.py
+-rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/delta_lake/__init__.py
+-rw-r--r--   0        0        0     1691 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/delta_lake/delta_log.py
+-rw-r--r--   0        0        0     5982 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/delta_lake/functions.py
+-rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/hive_metastore_config.py
+-rw-r--r--   0        0        0     1318 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/hive_table.py
+-rw-r--r--   0        0        0     1868 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/job_socket.py
+-rw-r--r--   0        0        0     1129 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/k8s_config.py
+-rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 spark_utils-1.1.2/PKG-INFO
```

### Comparing `spark_utils-1.1.1/LICENSE` & `spark_utils-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/README.md` & `spark_utils-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/pyproject.toml` & `spark_utils-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-utils"
-version = "1.1.1"
+version = "1.1.2"
 description = "Utility classes for comfy Spark job authoriing."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'MIT'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/spark-utils'
```

### Comparing `spark_utils-1.1.1/spark_utils/__init__.py` & `spark_utils-1.1.2/spark_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/common/__init__.py` & `spark_utils-1.1.2/spark_utils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/common/functions.py` & `spark_utils-1.1.2/spark_utils/common/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/common/spark_job_args.py` & `spark_utils-1.1.2/spark_utils/common/spark_job_args.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/common/spark_session_provider.py` & `spark_utils-1.1.2/spark_utils/common/spark_session_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
 
 class SparkSessionProvider:
     """
     Provider of a Spark session and related objects
     """
 
+    DELTA_CATALOG_EXTENSION = "io.delta.sql.DeltaSparkSessionExtension"
+    CASSANDRA_CATALOG_EXTENSION = "com.datastax.spark.connector.CassandraSparkExtensions"
+
     def __init__(
         self,
         *,
         delta_lake_version="2.12:2.4.0",
         hive_metastore_config: Optional[HiveMetastoreConfig] = None,
         additional_packages: Optional[List[str]] = None,
         additional_configs: Optional[Dict[str, str]] = None,
@@ -79,15 +82,15 @@
 
         packages = [f"io.delta:delta-core_{delta_lake_version}"]
         if additional_packages:
             packages.extend(additional_packages)
 
         self._spark_session_builder = (
             SparkSession.builder.config("spark.jars.packages", ",".join(packages))
-            .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension")
+            .config("spark.sql.extensions", SparkSessionProvider.DELTA_CATALOG_EXTENSION)
             .config("spark.sql.catalog.spark_catalog", "org.apache.spark.sql.delta.catalog.DeltaCatalog")
             .config("spark.jars.ivy", os.path.join(tempfile.gettempdir(), ".ivy2"))
             .config("spark.sql.parquet.datetimeRebaseModeInWrite", "CORRECTED")
             .config("spark.sql.parquet.int96RebaseModeInWrite", "CORRECTED")
         )
 
         if hive_metastore_config:
@@ -152,15 +155,18 @@
         os.makedirs(bundle_path, exist_ok=True)
 
         with open(os.path.join(bundle_path, bundle_file_name), "wb") as bundle_file:
             bundle_file.write(base64.b64decode(bundle_bytes))
 
         self._spark_session_builder = (
             self._spark_session_builder.config(
-                "spark.sql.extensions", "com.datastax.spark.connector.CassandraSparkExtensions"
+                "spark.sql.extensions",
+                ",".join(
+                    [SparkSessionProvider.DELTA_CATALOG_EXTENSION, SparkSessionProvider.CASSANDRA_CATALOG_EXTENSION]
+                ),
             )
             .config(f"spark.sql.catalog.{db_name}", "com.datastax.spark.connector.datasource.CassandraCatalog")
             .config("spark.files", os.path.join(bundle_path, bundle_file_name))
             .config("spark.cassandra.connection.config.cloud.path", bundle_file_name)
             .config("spark.cassandra.auth.username", client_id)
             .config("spark.cassandra.auth.password", client_secret)
             .config("spark.dse.continuousPagingEnabled", "false")
```

### Comparing `spark_utils-1.1.1/spark_utils/common/spark_sql_utils.py` & `spark_utils-1.1.2/spark_utils/common/spark_sql_utils.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/common/spark_udf.py` & `spark_utils-1.1.2/spark_utils/common/spark_udf.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/dataframes/__init__.py` & `spark_utils-1.1.2/spark_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/dataframes/functions.py` & `spark_utils-1.1.2/spark_utils/dataframes/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/dataframes/models.py` & `spark_utils-1.1.2/spark_utils/dataframes/models.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/dataframes/sets/__init__.py` & `spark_utils-1.1.2/spark_utils/dataframes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/dataframes/sets/functions.py` & `spark_utils-1.1.2/spark_utils/dataframes/sets/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/delta_lake/__init__.py` & `spark_utils-1.1.2/spark_utils/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/delta_lake/delta_log.py` & `spark_utils-1.1.2/spark_utils/delta_lake/delta_log.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/delta_lake/functions.py` & `spark_utils-1.1.2/spark_utils/delta_lake/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/models/__init__.py` & `spark_utils-1.1.2/spark_utils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/models/hive_metastore_config.py` & `spark_utils-1.1.2/spark_utils/models/hive_metastore_config.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/models/hive_table.py` & `spark_utils-1.1.2/spark_utils/models/hive_table.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/models/job_socket.py` & `spark_utils-1.1.2/spark_utils/models/job_socket.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/spark_utils/models/k8s_config.py` & `spark_utils-1.1.2/spark_utils/models/k8s_config.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.1/PKG-INFO` & `spark_utils-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-utils
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utility classes for comfy Spark job authoriing.
 Home-page: https://github.com/SneaksAndData/spark-utils
 License: MIT
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

