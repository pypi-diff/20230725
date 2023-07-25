# Comparing `tmp/meltanolabs_target_snowflake-0.4.2.tar.gz` & `tmp/meltanolabs_target_snowflake-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.4.2.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.4.3.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.4.2.tar` & `meltanolabs_target_snowflake-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3860 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/LICENSE
--rw-r--r--   0        0        0     5010 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/README.md
--rw-r--r--   0        0        0     1332 2023-07-13 16:55:52.014536 meltanolabs_target_snowflake-0.4.2/pyproject.toml
--rw-r--r--   0        0        0       89 2023-07-13 16:55:52.014536 meltanolabs_target_snowflake-0.4.2/target_snowflake/__init__.py
--rw-r--r--   0        0        0    19556 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/connector.py
--rw-r--r--   0        0        0     2651 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/initializer.py
--rw-r--r--   0        0        0     8248 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/sinks.py
--rw-r--r--   0        0        0      724 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/snowflake_types.py
--rw-r--r--   0        0        0     3147 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/target.py
--rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-07-25 14:21:16.715534 meltanolabs_target_snowflake-0.4.3/LICENSE
+-rw-r--r--   0        0        0     5010 2023-07-25 14:21:16.715534 meltanolabs_target_snowflake-0.4.3/README.md
+-rw-r--r--   0        0        0     1332 2023-07-25 14:21:38.100645 meltanolabs_target_snowflake-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-07-25 14:21:38.104645 meltanolabs_target_snowflake-0.4.3/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    21078 2023-07-25 14:21:16.715534 meltanolabs_target_snowflake-0.4.3/target_snowflake/connector.py
+-rw-r--r--   0        0        0     2651 2023-07-25 14:21:16.715534 meltanolabs_target_snowflake-0.4.3/target_snowflake/initializer.py
+-rw-r--r--   0        0        0     8248 2023-07-25 14:21:16.715534 meltanolabs_target_snowflake-0.4.3/target_snowflake/sinks.py
+-rw-r--r--   0        0        0      724 2023-07-25 14:21:16.715534 meltanolabs_target_snowflake-0.4.3/target_snowflake/snowflake_types.py
+-rw-r--r--   0        0        0     3147 2023-07-25 14:21:16.719534 meltanolabs_target_snowflake-0.4.3/target_snowflake/target.py
+-rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.4.3/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.4.2/LICENSE` & `meltanolabs_target_snowflake-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.2/README.md` & `meltanolabs_target_snowflake-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.2/pyproject.toml` & `meltanolabs_target_snowflake-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.4.2"
+version = "0.4.3"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
```

### Comparing `meltanolabs_target_snowflake-0.4.2/target_snowflake/connector.py` & `meltanolabs_target_snowflake-0.4.3/target_snowflake/connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from snowflake.sqlalchemy.snowdialect import SnowflakeDialect
 from sqlalchemy.engine import Engine
 from sqlalchemy.sql import text
 
 from target_snowflake.snowflake_types import NUMBER, TIMESTAMP_NTZ, VARIANT
 
 SNOWFLAKE_MAX_STRING_LENGTH = 16777216
+SNOWFLAKE_MAX_NUMBER_PRECISION = 38
+SNOWFLAKE_MAX_NUMBER_SCALE = 0
 
 class TypeMap:
     def __init__(self, operator, map_value, match_value=None):
         self.operator = operator
         self.map_value = map_value
         self.match_value = match_value
 
@@ -89,15 +91,15 @@
             self.table_cache[full_table_name] = parsed_columns
             return parsed_columns
 
     def _convert_type(self, sql_type):
         if isinstance(sql_type, sct.TIMESTAMP_NTZ):
             return TIMESTAMP_NTZ
         elif isinstance(sql_type, sct.NUMBER):
-            return NUMBER
+            return NUMBER(precision=sql_type.precision, scale=sql_type.scale)
         elif isinstance(sql_type, sct.VARIANT):
             return VARIANT
         else:
             return sql_type
 
     def get_sqlalchemy_url(self, config: dict) -> str:
         """Generates a SQLAlchemy URL for Snowflake.
@@ -128,23 +130,29 @@
         This method exists solely so that tap/target developers can override it
         on their subclass of SQLConnector to perform custom engine creation
         logic.
 
         Returns:
             A new SQLAlchemy Engine.
         """
-        return sqlalchemy.create_engine(
+        engine = sqlalchemy.create_engine(
             self.sqlalchemy_url,
             connect_args={
                 "session_parameters": {
                     "QUOTED_IDENTIFIERS_IGNORE_CASE": "TRUE",
                 }
             },
             echo=False,
         )
+        connection = engine.connect()
+        db_names = [db[1] for db in connection.execute(text("SHOW DATABASES;")).fetchall()]
+        if self.config["database"] not in db_names:
+            raise Exception(f"Database '{self.config['database']}' does not exist or the user/role doesn't have access to it.")
+        return engine
+
 
     def prepare_column(
         self,
         full_table_name: str,
         column_name: str,
         sql_type: sqlalchemy.types.TypeEngine,
     ) -> None:
@@ -209,14 +217,36 @@
         """Alter jsonschema representations to limit max length to Snowflake's VARCHAR length."""
         max_length = jsonschema_type.get("maxLength")
         if max_length and max_length > SNOWFLAKE_MAX_STRING_LENGTH:
             jsonschema_type["maxLength"] = SNOWFLAKE_MAX_STRING_LENGTH
         return jsonschema_type
 
     @staticmethod
+    def _get_numeric_precision(jsonschema_type):
+        return SNOWFLAKE_MAX_NUMBER_PRECISION
+
+    @staticmethod
+    def _get_numeric_scale(jsonschema_type):
+        precision = SNOWFLAKE_MAX_NUMBER_SCALE
+        if jsonschema_type.get("exclusiveMinimum"):
+            if str(jsonschema_type[attrib])[-1] == 1:
+                return len(str(jsonschema_type[attrib]).split(".")[1]) - 1
+            else:
+                return len(str(jsonschema_type[attrib]).split(".")[1])
+        attribs_to_check = [
+            "multipleOf",
+            "min",
+            "max",
+        ]
+        for attrib in attribs_to_check:
+            if jsonschema_type.get(attrib):
+                precision = max(precision, len(str(jsonschema_type[attrib]).split(".")[1]))
+        return precision
+
+    @staticmethod
     def to_sql_type(jsonschema_type: dict) -> sqlalchemy.types.TypeEngine:
         """Return a JSON Schema representation of the provided type.
 
         Uses custom Snowflake types from [snowflake-sqlalchemy](https://github.com/snowflakedb/snowflake-sqlalchemy/blob/main/src/snowflake/sqlalchemy/custom_types.py)
 
         Args:
             jsonschema_type: The JSON Schema representation of the source type.
@@ -226,25 +256,28 @@
         """
         # start with default implementation
         jsonschema_type = SnowflakeConnector._conform_max_length(jsonschema_type)
         target_type = SQLConnector.to_sql_type(jsonschema_type)
         # snowflake max and default varchar length
         # https://docs.snowflake.com/en/sql-reference/intro-summary-data-types.html
         maxlength = jsonschema_type.get("maxLength", SNOWFLAKE_MAX_STRING_LENGTH)
+        num_precision = SnowflakeConnector._get_numeric_precision(jsonschema_type)
+        num_scale = SnowflakeConnector._get_numeric_scale(jsonschema_type)
         # define type maps
         string_submaps = [
             TypeMap(eq, TIMESTAMP_NTZ(), "date-time"),
             TypeMap(contains, sqlalchemy.types.TIME(), "time"),
             TypeMap(eq, sqlalchemy.types.DATE(), "date"),
             TypeMap(eq, sqlalchemy.types.VARCHAR(maxlength), None),
         ]
         type_maps = [
             TypeMap(th._jsonschema_type_check, NUMBER(), ("integer",)),
             TypeMap(th._jsonschema_type_check, VARIANT(), ("object",)),
             TypeMap(th._jsonschema_type_check, VARIANT(), ("array",)),
+            TypeMap(th._jsonschema_type_check, NUMBER(precision=num_precision, scale=num_scale), ("number",)),
         ]
         # apply type maps
         if th._jsonschema_type_check(jsonschema_type, ("string",)):
             datelike_type = th.get_datelike_property_type(jsonschema_type)
             target_type = evaluate_typemaps(string_submaps, datelike_type, target_type)
         else:
             target_type = evaluate_typemaps(type_maps, jsonschema_type, target_type)
```

### Comparing `meltanolabs_target_snowflake-0.4.2/target_snowflake/initializer.py` & `meltanolabs_target_snowflake-0.4.3/target_snowflake/initializer.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.2/target_snowflake/sinks.py` & `meltanolabs_target_snowflake-0.4.3/target_snowflake/sinks.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.2/target_snowflake/snowflake_types.py` & `meltanolabs_target_snowflake-0.4.3/target_snowflake/snowflake_types.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.2/target_snowflake/target.py` & `meltanolabs_target_snowflake-0.4.3/target_snowflake/target.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.2/PKG-INFO` & `meltanolabs_target_snowflake-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltanolabs-target-snowflake
-Version: 0.4.2
+Version: 0.4.3
 Summary: `target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,Snowflake
 Author: Ken Payne
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

