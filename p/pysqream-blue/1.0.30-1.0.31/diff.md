# Comparing `tmp/pysqream-blue-1.0.30.tar.gz` & `tmp/pysqream-blue-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysqream-blue-1.0.30.tar", last modified: Tue Jul 18 12:11:30 2023, max compression
+gzip compressed data, was "dist/pysqream-blue-1.0.31.tar", last modified: Tue Jul 25 13:59:09 2023, max compression
```

## Comparing `pysqream-blue-1.0.30.tar` & `pysqream-blue-1.0.31.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/protos/
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/authentication_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/authentication_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/authentication_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/authentication_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/client_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/client_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/queryhandler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/protos/queryhandler_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/pysqream_blue/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/pysqream_blue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/pysqream_blue/casting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/pysqream_blue/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/pysqream_blue/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/pysqream_blue/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/pysqream_blue/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3124 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/pysqream_blue/pysqream_blue.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/pysqream_blue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/pysqream_blue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/pysqream_blue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/pysqream_blue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/pysqream_blue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/pysqream_blue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/pysqream_blue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 12:11:30.000000 pysqream-blue-1.0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-18 12:11:07.000000 pysqream-blue-1.0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/authentication_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/authentication_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/authentication_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/authentication_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/client_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/client_info_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/queryhandler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/protos/queryhandler_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/pysqream_blue/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/pysqream_blue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/pysqream_blue/casting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/pysqream_blue/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17702 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/pysqream_blue/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/pysqream_blue/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/pysqream_blue/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3124 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/pysqream_blue/pysqream_blue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/pysqream_blue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/pysqream_blue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/pysqream_blue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/pysqream_blue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/pysqream_blue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/pysqream_blue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/pysqream_blue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:59:09.000000 pysqream-blue-1.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-25 13:58:51.000000 pysqream-blue-1.0.31/setup.py
```

### Comparing `pysqream-blue-1.0.30/LICENSE` & `pysqream-blue-1.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/PKG-INFO` & `pysqream-blue-1.0.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.30
+Version: 1.0.31
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 Keywords: database db-api sqream sqreamdbV2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.30
+* **Version:**  1.0.31
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.30/README.rst` & `pysqream-blue-1.0.31/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.30
+* **Version:**  1.0.31
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.30/protos/authentication_pb2.py` & `pysqream-blue-1.0.31/protos/authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/protos/authentication_pb2_grpc.py` & `pysqream-blue-1.0.31/protos/authentication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/protos/authentication_type_pb2.py` & `pysqream-blue-1.0.31/protos/authentication_type_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/protos/client_info_pb2.py` & `pysqream-blue-1.0.31/protos/client_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/protos/error_pb2.py` & `pysqream-blue-1.0.31/protos/error_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/protos/queryhandler_pb2.py` & `pysqream-blue-1.0.31/protos/queryhandler_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from protos import error_pb2 as protos_dot_error__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/queryhandler.proto\x12\x1d\x63om.sqream.cloud.generated.v1\x1a\x12protos/error.proto\"Z\n\x0e\x43ompileRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\x0c\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x15\n\rquery_timeout\x18\x04 \x01(\x03\"\xd8\x01\n\x0f\x43ompileResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12>\n\x07\x63olumns\x18\x02 \x03(\x0b\x32-.com.sqream.cloud.generated.v1.ColumnMetadata\x12<\n\nquery_type\x18\x03 \x01(\x0e\x32(.com.sqream.cloud.generated.v1.QueryType\x12\x33\n\x05\x65rror\x18\x04 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rStatusRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"\x8a\x01\n\x0eStatusResponse\x12\x43\n\x06status\x18\x01 \x01(\x0e\x32\x33.com.sqream.cloud.generated.v1.QueryExecutionStatus\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"$\n\x0e\x45xecuteRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"Z\n\x0f\x45xecuteResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"\xb4\x01\n\x0e\x43olumnMetadata\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\x12\x10\n\x08nullable\x18\x02 \x01(\x08\x12\x13\n\x0btru_varchar\x18\x03 \x01(\x08\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x12\n\nvalue_size\x18\x05 \x01(\x03\x12\r\n\x05scale\x18\x06 \x01(\x05\x12\x11\n\tprecision\x18\x07 \x01(\x05\"\"\n\x0c\x46\x65tchRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"Z\n\rFetchResponse\x12\x14\n\x0cquery_result\x18\x01 \x01(\x0c\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"[\n\x15\x43loseStatementRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"^\n\x16\x43loseStatementResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"Y\n\x13\x43loseSessionRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"\\\n\x14\x43loseSessionResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"\"\n\x0c\x43loseRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"T\n\rCloseResponse\x12\x0e\n\x06\x63losed\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rCancelRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"W\n\x0e\x43\x61ncelResponse\x12\x10\n\x08\x63\x61nceled\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error*\xa2\x03\n\nColumnType\x12\x1b\n\x17\x43OLUMN_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43OLUMN_TYPE_LONG_INT\x10\x01\x12\x19\n\x15\x43OLUMN_TYPE_ULONG_INT\x10\x02\x12\x13\n\x0f\x43OLUMN_TYPE_INT\x10\x04\x12\x14\n\x10\x43OLUMN_TYPE_UINT\x10\x05\x12\x17\n\x13\x43OLUMN_TYPE_VARCHAR\x10\x06\x12\x16\n\x12\x43OLUMN_TYPE_DOUBLE\x10\x07\x12\x14\n\x10\x43OLUMN_TYPE_BYTE\x10\x08\x12\x15\n\x11\x43OLUMN_TYPE_UBYTE\x10\t\x12\x15\n\x11\x43OLUMN_TYPE_SHORT\x10\n\x12\x16\n\x12\x43OLUMN_TYPE_USHORT\x10\x0b\x12\x15\n\x11\x43OLUMN_TYPE_FLOAT\x10\x0c\x12\x14\n\x10\x43OLUMN_TYPE_DATE\x10\r\x12\x18\n\x14\x43OLUMN_TYPE_DATETIME\x10\x0e\x12\x14\n\x10\x43OLUMN_TYPE_BOOL\x10\x0f\x12\x14\n\x10\x43OLUMN_TYPE_BLOB\x10\x10\x12\x17\n\x13\x43OLUMN_TYPE_NUMERIC\x10\x11*W\n\tQueryType\x12\x1a\n\x16QUERY_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10QUERY_TYPE_QUERY\x10\x01\x12\x18\n\x14QUERY_TYPE_NON_QUERY\x10\x02*\x98\x02\n\x14QueryExecutionStatus\x12&\n\"QUERY_EXECUTION_STATUS_UNSPECIFIED\x10\x00\x12\"\n\x1eQUERY_EXECUTION_STATUS_RUNNING\x10\x01\x12$\n QUERY_EXECUTION_STATUS_SUCCEEDED\x10\x02\x12!\n\x1dQUERY_EXECUTION_STATUS_FAILED\x10\x03\x12$\n QUERY_EXECUTION_STATUS_CANCELLED\x10\x04\x12\"\n\x1eQUERY_EXECUTION_STATUS_ABORTED\x10\x05\x12!\n\x1dQUERY_EXECUTION_STATUS_QUEUED\x10\x06\x32\x93\x06\n\x13QueryHandlerService\x12h\n\x07\x43ompile\x12-.com.sqream.cloud.generated.v1.CompileRequest\x1a..com.sqream.cloud.generated.v1.CompileResponse\x12h\n\x07\x45xecute\x12-.com.sqream.cloud.generated.v1.ExecuteRequest\x1a..com.sqream.cloud.generated.v1.ExecuteResponse\x12\x65\n\x06Status\x12,.com.sqream.cloud.generated.v1.StatusRequest\x1a-.com.sqream.cloud.generated.v1.StatusResponse\x12\x62\n\x05\x46\x65tch\x12+.com.sqream.cloud.generated.v1.FetchRequest\x1a,.com.sqream.cloud.generated.v1.FetchResponse\x12}\n\x0e\x43loseStatement\x12\x34.com.sqream.cloud.generated.v1.CloseStatementRequest\x1a\x35.com.sqream.cloud.generated.v1.CloseStatementResponse\x12\x65\n\x06\x43\x61ncel\x12,.com.sqream.cloud.generated.v1.CancelRequest\x1a-.com.sqream.cloud.generated.v1.CancelResponse\x12w\n\x0c\x43loseSession\x12\x32.com.sqream.cloud.generated.v1.CloseSessionRequest\x1a\x33.com.sqream.cloud.generated.v1.CloseSessionResponseB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/queryhandler.proto\x12\x1d\x63om.sqream.cloud.generated.v1\x1a\x12protos/error.proto\"Z\n\x0e\x43ompileRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\x0c\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x15\n\rquery_timeout\x18\x04 \x01(\x03\"\xd8\x01\n\x0f\x43ompileResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12>\n\x07\x63olumns\x18\x02 \x03(\x0b\x32-.com.sqream.cloud.generated.v1.ColumnMetadata\x12<\n\nquery_type\x18\x03 \x01(\x0e\x32(.com.sqream.cloud.generated.v1.QueryType\x12\x33\n\x05\x65rror\x18\x04 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rStatusRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"\x8a\x01\n\x0eStatusResponse\x12\x43\n\x06status\x18\x01 \x01(\x0e\x32\x33.com.sqream.cloud.generated.v1.QueryExecutionStatus\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"$\n\x0e\x45xecuteRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"Z\n\x0f\x45xecuteResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"\xb4\x01\n\x0e\x43olumnMetadata\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\x12\x10\n\x08nullable\x18\x02 \x01(\x08\x12\x13\n\x0btru_varchar\x18\x03 \x01(\x08\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x12\n\nvalue_size\x18\x05 \x01(\x03\x12\r\n\x05scale\x18\x06 \x01(\x05\x12\x11\n\tprecision\x18\x07 \x01(\x05\"\"\n\x0c\x46\x65tchRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"o\n\rFetchResponse\x12\x14\n\x0cquery_result\x18\x01 \x01(\x0c\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\x12\x13\n\x0bretry_fetch\x18\x03 \x01(\x08\"[\n\x15\x43loseStatementRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"^\n\x16\x43loseStatementResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"Y\n\x13\x43loseSessionRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"\\\n\x14\x43loseSessionResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"\"\n\x0c\x43loseRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"T\n\rCloseResponse\x12\x0e\n\x06\x63losed\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rCancelRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"W\n\x0e\x43\x61ncelResponse\x12\x10\n\x08\x63\x61nceled\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error*\xa2\x03\n\nColumnType\x12\x1b\n\x17\x43OLUMN_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43OLUMN_TYPE_LONG_INT\x10\x01\x12\x19\n\x15\x43OLUMN_TYPE_ULONG_INT\x10\x02\x12\x13\n\x0f\x43OLUMN_TYPE_INT\x10\x04\x12\x14\n\x10\x43OLUMN_TYPE_UINT\x10\x05\x12\x17\n\x13\x43OLUMN_TYPE_VARCHAR\x10\x06\x12\x16\n\x12\x43OLUMN_TYPE_DOUBLE\x10\x07\x12\x14\n\x10\x43OLUMN_TYPE_BYTE\x10\x08\x12\x15\n\x11\x43OLUMN_TYPE_UBYTE\x10\t\x12\x15\n\x11\x43OLUMN_TYPE_SHORT\x10\n\x12\x16\n\x12\x43OLUMN_TYPE_USHORT\x10\x0b\x12\x15\n\x11\x43OLUMN_TYPE_FLOAT\x10\x0c\x12\x14\n\x10\x43OLUMN_TYPE_DATE\x10\r\x12\x18\n\x14\x43OLUMN_TYPE_DATETIME\x10\x0e\x12\x14\n\x10\x43OLUMN_TYPE_BOOL\x10\x0f\x12\x14\n\x10\x43OLUMN_TYPE_BLOB\x10\x10\x12\x17\n\x13\x43OLUMN_TYPE_NUMERIC\x10\x11*W\n\tQueryType\x12\x1a\n\x16QUERY_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10QUERY_TYPE_QUERY\x10\x01\x12\x18\n\x14QUERY_TYPE_NON_QUERY\x10\x02*\x98\x02\n\x14QueryExecutionStatus\x12&\n\"QUERY_EXECUTION_STATUS_UNSPECIFIED\x10\x00\x12\"\n\x1eQUERY_EXECUTION_STATUS_RUNNING\x10\x01\x12$\n QUERY_EXECUTION_STATUS_SUCCEEDED\x10\x02\x12!\n\x1dQUERY_EXECUTION_STATUS_FAILED\x10\x03\x12$\n QUERY_EXECUTION_STATUS_CANCELLED\x10\x04\x12\"\n\x1eQUERY_EXECUTION_STATUS_ABORTED\x10\x05\x12!\n\x1dQUERY_EXECUTION_STATUS_QUEUED\x10\x06\x32\x93\x06\n\x13QueryHandlerService\x12h\n\x07\x43ompile\x12-.com.sqream.cloud.generated.v1.CompileRequest\x1a..com.sqream.cloud.generated.v1.CompileResponse\x12h\n\x07\x45xecute\x12-.com.sqream.cloud.generated.v1.ExecuteRequest\x1a..com.sqream.cloud.generated.v1.ExecuteResponse\x12\x65\n\x06Status\x12,.com.sqream.cloud.generated.v1.StatusRequest\x1a-.com.sqream.cloud.generated.v1.StatusResponse\x12\x62\n\x05\x46\x65tch\x12+.com.sqream.cloud.generated.v1.FetchRequest\x1a,.com.sqream.cloud.generated.v1.FetchResponse\x12}\n\x0e\x43loseStatement\x12\x34.com.sqream.cloud.generated.v1.CloseStatementRequest\x1a\x35.com.sqream.cloud.generated.v1.CloseStatementResponse\x12\x65\n\x06\x43\x61ncel\x12,.com.sqream.cloud.generated.v1.CancelRequest\x1a-.com.sqream.cloud.generated.v1.CancelResponse\x12w\n\x0c\x43loseSession\x12\x32.com.sqream.cloud.generated.v1.CloseSessionRequest\x1a\x33.com.sqream.cloud.generated.v1.CloseSessionResponseB\x02P\x01\x62\x06proto3')
 
 _COLUMNTYPE = DESCRIPTOR.enum_types_by_name['ColumnType']
 ColumnType = enum_type_wrapper.EnumTypeWrapper(_COLUMNTYPE)
 _QUERYTYPE = DESCRIPTOR.enum_types_by_name['QueryType']
 QueryType = enum_type_wrapper.EnumTypeWrapper(_QUERYTYPE)
 _QUERYEXECUTIONSTATUS = DESCRIPTOR.enum_types_by_name['QueryExecutionStatus']
 QueryExecutionStatus = enum_type_wrapper.EnumTypeWrapper(_QUERYEXECUTIONSTATUS)
@@ -190,20 +190,20 @@
 _sym_db.RegisterMessage(CancelResponse)
 
 _QUERYHANDLERSERVICE = DESCRIPTOR.services_by_name['QueryHandlerService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'P\001'
-  _COLUMNTYPE._serialized_start=1633
-  _COLUMNTYPE._serialized_end=2051
-  _QUERYTYPE._serialized_start=2053
-  _QUERYTYPE._serialized_end=2140
-  _QUERYEXECUTIONSTATUS._serialized_start=2143
-  _QUERYEXECUTIONSTATUS._serialized_end=2423
+  _COLUMNTYPE._serialized_start=1654
+  _COLUMNTYPE._serialized_end=2072
+  _QUERYTYPE._serialized_start=2074
+  _QUERYTYPE._serialized_end=2161
+  _QUERYEXECUTIONSTATUS._serialized_start=2164
+  _QUERYEXECUTIONSTATUS._serialized_end=2444
   _COMPILEREQUEST._serialized_start=80
   _COMPILEREQUEST._serialized_end=170
   _COMPILERESPONSE._serialized_start=173
   _COMPILERESPONSE._serialized_end=389
   _STATUSREQUEST._serialized_start=391
   _STATUSREQUEST._serialized_end=426
   _STATUSRESPONSE._serialized_start=429
@@ -213,27 +213,27 @@
   _EXECUTERESPONSE._serialized_start=607
   _EXECUTERESPONSE._serialized_end=697
   _COLUMNMETADATA._serialized_start=700
   _COLUMNMETADATA._serialized_end=880
   _FETCHREQUEST._serialized_start=882
   _FETCHREQUEST._serialized_end=916
   _FETCHRESPONSE._serialized_start=918
-  _FETCHRESPONSE._serialized_end=1008
-  _CLOSESTATEMENTREQUEST._serialized_start=1010
-  _CLOSESTATEMENTREQUEST._serialized_end=1101
-  _CLOSESTATEMENTRESPONSE._serialized_start=1103
-  _CLOSESTATEMENTRESPONSE._serialized_end=1197
-  _CLOSESESSIONREQUEST._serialized_start=1199
-  _CLOSESESSIONREQUEST._serialized_end=1288
-  _CLOSESESSIONRESPONSE._serialized_start=1290
-  _CLOSESESSIONRESPONSE._serialized_end=1382
-  _CLOSEREQUEST._serialized_start=1384
-  _CLOSEREQUEST._serialized_end=1418
-  _CLOSERESPONSE._serialized_start=1420
-  _CLOSERESPONSE._serialized_end=1504
-  _CANCELREQUEST._serialized_start=1506
-  _CANCELREQUEST._serialized_end=1541
-  _CANCELRESPONSE._serialized_start=1543
-  _CANCELRESPONSE._serialized_end=1630
-  _QUERYHANDLERSERVICE._serialized_start=2426
-  _QUERYHANDLERSERVICE._serialized_end=3213
+  _FETCHRESPONSE._serialized_end=1029
+  _CLOSESTATEMENTREQUEST._serialized_start=1031
+  _CLOSESTATEMENTREQUEST._serialized_end=1122
+  _CLOSESTATEMENTRESPONSE._serialized_start=1124
+  _CLOSESTATEMENTRESPONSE._serialized_end=1218
+  _CLOSESESSIONREQUEST._serialized_start=1220
+  _CLOSESESSIONREQUEST._serialized_end=1309
+  _CLOSESESSIONRESPONSE._serialized_start=1311
+  _CLOSESESSIONRESPONSE._serialized_end=1403
+  _CLOSEREQUEST._serialized_start=1405
+  _CLOSEREQUEST._serialized_end=1439
+  _CLOSERESPONSE._serialized_start=1441
+  _CLOSERESPONSE._serialized_end=1525
+  _CANCELREQUEST._serialized_start=1527
+  _CANCELREQUEST._serialized_end=1562
+  _CANCELRESPONSE._serialized_start=1564
+  _CANCELRESPONSE._serialized_end=1651
+  _QUERYHANDLERSERVICE._serialized_start=2447
+  _QUERYHANDLERSERVICE._serialized_end=3234
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pysqream-blue-1.0.30/protos/queryhandler_pb2_grpc.py` & `pysqream-blue-1.0.31/protos/queryhandler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/pysqream_blue/casting.py` & `pysqream-blue-1.0.31/pysqream_blue/casting.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/pysqream_blue/connection.py` & `pysqream-blue-1.0.31/pysqream_blue/connection.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/pysqream_blue/cursor.py` & `pysqream-blue-1.0.31/pysqream_blue/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,25 +237,31 @@
                                    column.nullable))
                             for column in self.columns_metadata]
         self.column_list = [{'name': column.name, 'type': [type_to_v1_tpye[column.type], ]} for column in
                             self.columns_metadata]
 
     def _request_fetch(self):
         fetch_response = None
-        try:
-            fetch_response: qh_messages.FetchResponse = self._fetch()
-        except grpc.RpcError as rpc_error:
-            log_and_raise(ProgrammingError,
-                          f'Query id: {self.stmt_id}. Error from grpc while attempting to fetch the results.\n{rpc_error}')
-
-            if is_token_expired(str(rpc_error)):
-                auth_response = self.client.auth_access_token()
-                self.client.token = auth_response.token
-                self.call_credentialds = grpc.access_token_call_credentials(self.client.token)
+        retry = True
+        while retry:
+            try:
                 fetch_response: qh_messages.FetchResponse = self._fetch()
+                retry = fetch_response.retry_fetch
+            except grpc.RpcError as rpc_error:
+                retry = False
+                log_and_raise(ProgrammingError,
+                              f'Query id: {self.stmt_id}. Error from grpc while attempting to fetch the results.\n{rpc_error}')
+
+                if is_token_expired(str(rpc_error)):
+                    log_info("Token expired on the middle of fetch, try to fetch again")
+                    auth_response = self.client.auth_access_token()
+                    self.client.token = auth_response.token
+                    self.call_credentialds = grpc.access_token_call_credentials(self.client.token)
+                    fetch_response: qh_messages.FetchResponse = self._fetch()
+                    retry = fetch_response.retry_fetch
 
         if fetch_response.HasField('error'):
             log_and_raise(OperationalError,
                           f'Query id: {self.stmt_id}. Error while attempting to fetch the results.\n{fetch_response.error}')
 
         res_bytes = fetch_response.query_result
         header_size = int.from_bytes(res_bytes[:8], 'little')
```

### Comparing `pysqream-blue-1.0.30/pysqream_blue/globals.py` & `pysqream-blue-1.0.31/pysqream_blue/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import protos.queryhandler_pb2_grpc as qh_services
 import protos.authentication_pb2 as auth_messages
 import protos.authentication_pb2_grpc as auth_services
 import protos.client_info_pb2 as cl_messages
 import protos.client_info_pb2_grpc as cl_services
 import protos.authentication_type_pb2 as auth_type_messages
 
-__version__ = '1.0.30'
+__version__ = '1.0.31'
 
 dbapi_typecodes = {
     qh_messages.COLUMN_TYPE_LONG_INT:  'NUMBER',
     qh_messages.COLUMN_TYPE_ULONG_INT: 'NUMBER',
     qh_messages.COLUMN_TYPE_INT:       'NUMBER',
     qh_messages.COLUMN_TYPE_UINT:      'NUMBER',
     qh_messages.COLUMN_TYPE_VARCHAR:   'STRING',
```

### Comparing `pysqream-blue-1.0.30/pysqream_blue/logger.py` & `pysqream-blue-1.0.31/pysqream_blue/logger.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/pysqream_blue/pysqream_blue.py` & `pysqream-blue-1.0.31/pysqream_blue/pysqream_blue.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/pysqream_blue/utils.py` & `pysqream-blue-1.0.31/pysqream_blue/utils.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/pysqream_blue.egg-info/PKG-INFO` & `pysqream-blue-1.0.31/pysqream_blue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.30
+Version: 1.0.31
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 Keywords: database db-api sqream sqreamdbV2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.30
+* **Version:**  1.0.31
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.30/pysqream_blue.egg-info/SOURCES.txt` & `pysqream-blue-1.0.31/pysqream_blue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.30/setup.py` & `pysqream-blue-1.0.31/setup.py`

 * *Files identical despite different names*

