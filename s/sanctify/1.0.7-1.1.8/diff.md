# Comparing `tmp/sanctify-1.0.7.tar.gz` & `tmp/sanctify-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.0.7.tar", last modified: Thu Jul 20 06:49:43 2023, max compression
+gzip compressed data, was "sanctify-1.1.8.tar", last modified: Tue Jul 25 19:43:34 2023, max compression
```

## Comparing `sanctify-1.0.7.tar` & `sanctify-1.1.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-20 06:49:43.340723 sanctify-1.0.7/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.7/LICENSE.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    14012 2023-07-20 06:49:43.340464 sanctify-1.0.7/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13397 2023-07-20 06:48:14.000000 sanctify-1.0.7/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1415 2023-07-20 06:48:22.000000 sanctify-1.0.7/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-20 06:49:43.339524 sanctify-1.0.7/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      852 2023-07-20 06:48:50.000000 sanctify-1.0.7/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7648 2023-07-17 13:52:28.000000 sanctify-1.0.7/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2632 2023-07-17 13:52:28.000000 sanctify-1.0.7/sanctify/constants.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.7/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12305 2023-07-20 06:48:50.000000 sanctify-1.0.7/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8782 2023-07-17 13:52:28.000000 sanctify-1.0.7/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3455 2023-07-17 13:52:28.000000 sanctify-1.0.7/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11128 2023-07-20 06:48:50.000000 sanctify-1.0.7/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-20 06:49:43.340202 sanctify-1.0.7/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    14012 2023-07-20 06:49:43.000000 sanctify-1.0.7/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-20 06:49:43.000000 sanctify-1.0.7/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-20 06:49:43.000000 sanctify-1.0.7/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-20 06:49:43.000000 sanctify-1.0.7/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-20 06:49:43.340794 sanctify-1.0.7/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-25 19:43:34.264052 sanctify-1.1.8/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.1.8/LICENSE
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18575 2023-07-25 19:43:34.262789 sanctify-1.1.8/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    17964 2023-07-25 19:38:03.000000 sanctify-1.1.8/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1415 2023-07-25 19:39:51.000000 sanctify-1.1.8/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-25 19:43:34.261698 sanctify-1.1.8/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1059 2023-07-25 19:40:02.000000 sanctify-1.1.8/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7648 2023-07-17 13:52:28.000000 sanctify-1.1.8/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2632 2023-07-17 13:52:28.000000 sanctify-1.1.8/sanctify/constants.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-07-25 19:35:23.000000 sanctify-1.1.8/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13269 2023-07-25 19:40:02.000000 sanctify-1.1.8/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-07-25 19:13:47.000000 sanctify-1.1.8/sanctify/serializer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8782 2023-07-17 13:52:28.000000 sanctify-1.1.8/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4545 2023-07-25 16:13:58.000000 sanctify-1.1.8/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11128 2023-07-25 19:40:02.000000 sanctify-1.1.8/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-25 19:43:34.262492 sanctify-1.1.8/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18575 2023-07-25 19:43:34.000000 sanctify-1.1.8/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      355 2023-07-25 19:43:34.000000 sanctify-1.1.8/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-25 19:43:34.000000 sanctify-1.1.8/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-25 19:43:34.000000 sanctify-1.1.8/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-25 19:43:34.264111 sanctify-1.1.8/setup.cfg
```

### Comparing `sanctify-1.0.7/PKG-INFO` & `sanctify-1.1.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.7
+Version: 1.1.8
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # Sanctify [![codecov](https://codecov.io/gh/skit-ai/sanctify/branch/main/graph/badge.svg?token=WZHSY8T8SC)](https://codecov.io/gh/skit-ai/sanctify)
 
 Sanctify is a Python package designed to facilitate data cleansing and validation operations on pandas DataFrames. It provides a set of predefined transformations and validations that can be applied to different columns of a DataFrame based on a column mapping. The package allows you to define data types, transformations, and validations for each column, making it easy to clean and validate your data.
 
 ## Features
 
@@ -32,14 +32,15 @@
 You can install Sanctify using pip:
 
 ```shell
 pip install sanctify
 ```
 
 ## Basic Usage
+
 ```python
 import pandas as pd
 
 from sanctify import Cleanser, Transformer, Validator, process_cleansed_df
 
 ###
 # The package provides a few built in enums for ease of use
@@ -177,14 +178,15 @@
         cleansed_output_file_path=cleansed_output_file_path,
         processed_output_file_path=processed_output_file_path,
         cleansed_processed_output_file_path=cleansed_processed_output_file_path,
     )
 ```
 
 ## Advanced Usage
+
 ```python
 import pandas as pd
 
 from sanctify import Cleanser, Transformer, Validator, process_cleansed_df
 
 ###
 # The package provides a few built in enums for ease of use
@@ -346,9 +348,172 @@
         input_file_path=input_file_path,
         cleansed_output_file_path=cleansed_output_file_path,
         processed_output_file_path=processed_output_file_path,
         cleansed_processed_output_file_path=cleansed_processed_output_file_path,
     )
 ```
 
+## Additional Classes: SchemaSerializer and SchemaDeSerializer
+
+Sanctify provides two additional classes to facilitate data serialization and deserialization to/from JSON format. These classes are **SchemaSerializer** and **SchemaDeSerializer**.
+
+### SchemaSerializer
+
+The **SchemaSerializer** class is used to serialize data into JSON format. It takes the data to be serialized as input and provides the serialized JSON data as output.
+
+#### Usage
+
+```python
+from sanctify.serializer import SchemaSerializer
+from sanctify.transformer import Transformer
+
+data_to_serialize = {
+    "first_name": {
+        "standard_column": "First Name",
+        "transformations": [
+            Transformer.convert_to_lowercase,
+            Transformer.replace_ii_with_II,
+            Transformer.convert_jr_to_Junior,
+            Transformer.convert_sr_to_Senior,
+            Transformer.remove_dot_from_string,
+        ],
+    },
+}
+
+# Serialize the data
+serializer = SchemaSerializer(data_to_serialize)
+serialized_data = serializer.data
+
+print(serialized_data)
+# Output:
+"""
+{
+    "first_name": {
+        "standard_column": "First Name",
+        "transformations": [
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_to_lowercase",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "replace_ii_with_II",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_jr_to_Junior",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_sr_to_Senior",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "remove_dot_from_string",
+                "static_method_args": [
+                    "value"
+                ]
+            }
+        ]
+    }
+}
+"""
+```
+
+### SchemaDeSerializer
+
+The **SchemaDeSerializer** class is used to deserialize JSON data back into Python data structures. It takes the JSON data as input and provides the deserialized data as output.
+
+#### Usage
+
+```python
+from sanctify.serializer import SchemaDeSerializer
+from sanctify.transformer import Transformer
+
+serialized_data = """
+{
+    "first_name": {
+        "standard_column": "First Name",
+        "transformations": [
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_to_lowercase",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "replace_ii_with_II",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_jr_to_Junior",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_sr_to_Senior",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "remove_dot_from_string",
+                "static_method_args": [
+                    "value"
+                ]
+            }
+        ]
+    }
+}
+"""
+
+# Deserialize the data
+deserializer = SchemaDeSerializer(serialized_data)
+deserialized_data = deserializer.data
+
+print(deserialized_data)
+# Output:
+"""
+{
+    "first_name": {
+        "standard_column": "First Name",
+        "transformations": [
+            Transformer.convert_to_lowercase,
+            Transformer.replace_ii_with_II,
+            Transformer.convert_jr_to_Junior,
+            Transformer.convert_sr_to_Senior,
+            Transformer.remove_dot_from_string,
+        ],
+    },
+}
+"""
+```
+
 ## Contributing
+
 Contributions to Sanctify are welcome! If you find any bugs, have feature requests, or want to contribute code, please open an issue or submit a pull request on the [GitHub repository](https://github.com/skit-ai/sanctify/).
+
+Before starting: Make sure to create a python3.11 virtual env install the pre-commit hook
+
+```shell
+python3.11 -m venv venv && source venv/bin/activate && pip install pre-commit && pre-commit install
+```
```

### Comparing `sanctify-1.0.7/pyproject.toml` & `sanctify-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.0.7"
+version = "1.1.8"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Column Mapping based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `sanctify-1.0.7/sanctify/__init__.py` & `sanctify-1.1.8/sanctify/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,26 +8,31 @@
     Constants,
     DateOrderTuples,
     DefaultColumns,
     PrimitiveDataTypes,
 )
 from sanctify.exception import DataTypeParseError, ValidationError
 from sanctify.processor import process_cleansed_df
+from sanctify.serializer import CustomJSONDecoder, CustomJSONEncoder, SchemaDeSerializer, SchemaSerializer
 from sanctify.transformer import Transformer
 from sanctify.validator import Validator
 
 __all__ = [
     "Cleanser",
     "PRIMITIVE_TO_NULLABLE_DATA_TYPE_MAP",
     "AbstractDataTypes",
     "CalendarDateComponents",
     "ComparisonOperations",
     "Constants",
+    "CustomJSONDecoder",
+    "CustomJSONEncoder",
     "DateOrderTuples",
     "DefaultColumns",
     "PrimitiveDataTypes",
     "DataTypeParseError",
     "ValidationError",
     "process_cleansed_df",
+    "SchemaDeSerializer",
+    "SchemaSerializer",
     "Transformer",
     "Validator",
 ]
```

### Comparing `sanctify-1.0.7/sanctify/cleanser.py` & `sanctify-1.1.8/sanctify/cleanser.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.7/sanctify/constants.py` & `sanctify-1.1.8/sanctify/constants.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.7/sanctify/processor.py` & `sanctify-1.1.8/sanctify/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -146,36 +146,48 @@
     transformations, validations = [], []
     if Constants.VALIDATIONS.value in col_config:
         validations = col_config[Constants.VALIDATIONS.value]
 
     return transformations, validations
 
 
-def handle_post_processing_dtype(col_config: dict, data_type_schema: dict) -> Callable | None:
+def handle_post_processing_dtype(col_config: dict, data_type_schema: dict) -> Callable or None:
     """
-    Handles post validation transformations for a column.
+    Handles post-validation transformations for a column.
 
     Args:
-        col_config (dict): Column configuration.
+        col_config (dict): Column configuration containing column-specific settings.
+        data_type_schema (dict): A schema containing data types and their configurations.
 
     Returns:
-       Callable if int or float post validation transformation if applicable else returns None
+        Callable or None: If post-validation transformation is applicable for int or float,
+        it returns the corresponding transformation function. Otherwise, it returns None.
     """
-    dtype_in_col_config = PRIMITIVE_TO_NULLABLE_DATA_TYPE_MAP.get(
-        col_config.get(Constants.POST_PROCESSING_DATA_TYPE.value, ""), None
-    )
-    if dtype_in_col_config is None:
-        data_type_name_for_column: str = col_config.get(Constants.DATA_TYPE.value, "")
-        data_type_config_for_column: dict = data_type_schema.get(data_type_name_for_column, {})
-        return PRIMITIVE_TO_NULLABLE_DATA_TYPE_MAP.get(
-            data_type_config_for_column.get(Constants.POST_PROCESSING_DATA_TYPE.value, ""),
-            None,
-        )
-    else:
-        return dtype_in_col_config
+
+    result = None
+
+    # Check if the column configuration contains a post-processing data type
+    if Constants.POST_PROCESSING_DATA_TYPE.value in col_config:
+        pp_datatype = col_config.get(Constants.POST_PROCESSING_DATA_TYPE.value)
+        # Get the corresponding post-validation transformation function from the mapping
+        result = PRIMITIVE_TO_NULLABLE_DATA_TYPE_MAP.get(pp_datatype, None)
+
+    # Check if the column configuration refers to a predefined data type in the schema
+    if Constants.DATA_TYPE.value in col_config:
+        data_type_name_for_column: str = col_config.get(Constants.DATA_TYPE.value, None)
+        if data_type_name_for_column is not None:
+            # Retrieve the configuration for the specified data type from the schema
+            data_type_config_for_column: dict = data_type_schema.get(data_type_name_for_column, {})
+            # Check if the data type configuration contains a post-processing data type
+            if Constants.POST_PROCESSING_DATA_TYPE.value in data_type_config_for_column:
+                pp_datatype = col_config.get(Constants.POST_PROCESSING_DATA_TYPE.value)
+                # Get the corresponding post-validation transformation function from the mapping
+                result = PRIMITIVE_TO_NULLABLE_DATA_TYPE_MAP.get(pp_datatype, None)
+
+    return result
 
 
 def apply_functions(value, col_name: str, functions: list[Callable | tuple[Callable, dict]]) -> pd.Series:
     """
     Applies a series of transformation and validation functions to a value.
 
     Args:
@@ -194,15 +206,15 @@
         func_value = None
 
     else:
         for function in functions:
             func = function
             kwargs = {}
 
-            if isinstance(function, tuple):
+            if isinstance(function, (list, tuple)):
                 func = function[0]
                 kwargs = function[1]
 
             logger.debug(f"Running {func.__name__ = } with {value = } | {kwargs = }")
 
             try:
                 func_value = func(func_value, **kwargs)
```

### Comparing `sanctify-1.0.7/sanctify/transformer.py` & `sanctify-1.1.8/sanctify/transformer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.7/sanctify/utils.py` & `sanctify-1.1.8/sanctify/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -85,7 +85,32 @@
         and adjusting for the birth month and day.
 
     Example:
         If the date of birth is '1990-05-15', and the current date is '2022-08-10',
         the calculated age will be 32.
     """
     return relativedelta(current_date, date_of_birth).years
+
+
+def convert_tuples_to_lists(input_data):
+    """
+    Recursively converts tuples to lists in a nested dictionary.
+
+    This function takes a nested data structure (dictionary, list, or tuple) as input
+    and traverses through it recursively to find tuples. Whenever a tuple is found,
+    it converts it into a list. The function handles nested dictionaries, lists, and tuples.
+
+    Parameters:
+        input_data (dict, list, tuple, or any): The nested data structure to process.
+
+    Returns:
+        The input data structure with tuples converted to lists.
+    """
+    if isinstance(input_data, dict):
+        # If the input is a dictionary, process its key-value pairs recursively.
+        return {key: convert_tuples_to_lists(value) for key, value in input_data.items()}
+    elif isinstance(input_data, (tuple, list)):
+        # If the input is a tuple or list, process its elements recursively.
+        return [convert_tuples_to_lists(item) for item in input_data]
+    else:
+        # If the input is not a dictionary, tuple, or list, return it unchanged.
+        return input_data
```

### Comparing `sanctify-1.0.7/sanctify/validator.py` & `sanctify-1.1.8/sanctify/validator.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.7/sanctify.egg-info/PKG-INFO` & `sanctify-1.1.8/sanctify.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.7
+Version: 1.1.8
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # Sanctify [![codecov](https://codecov.io/gh/skit-ai/sanctify/branch/main/graph/badge.svg?token=WZHSY8T8SC)](https://codecov.io/gh/skit-ai/sanctify)
 
 Sanctify is a Python package designed to facilitate data cleansing and validation operations on pandas DataFrames. It provides a set of predefined transformations and validations that can be applied to different columns of a DataFrame based on a column mapping. The package allows you to define data types, transformations, and validations for each column, making it easy to clean and validate your data.
 
 ## Features
 
@@ -32,14 +32,15 @@
 You can install Sanctify using pip:
 
 ```shell
 pip install sanctify
 ```
 
 ## Basic Usage
+
 ```python
 import pandas as pd
 
 from sanctify import Cleanser, Transformer, Validator, process_cleansed_df
 
 ###
 # The package provides a few built in enums for ease of use
@@ -177,14 +178,15 @@
         cleansed_output_file_path=cleansed_output_file_path,
         processed_output_file_path=processed_output_file_path,
         cleansed_processed_output_file_path=cleansed_processed_output_file_path,
     )
 ```
 
 ## Advanced Usage
+
 ```python
 import pandas as pd
 
 from sanctify import Cleanser, Transformer, Validator, process_cleansed_df
 
 ###
 # The package provides a few built in enums for ease of use
@@ -346,9 +348,172 @@
         input_file_path=input_file_path,
         cleansed_output_file_path=cleansed_output_file_path,
         processed_output_file_path=processed_output_file_path,
         cleansed_processed_output_file_path=cleansed_processed_output_file_path,
     )
 ```
 
+## Additional Classes: SchemaSerializer and SchemaDeSerializer
+
+Sanctify provides two additional classes to facilitate data serialization and deserialization to/from JSON format. These classes are **SchemaSerializer** and **SchemaDeSerializer**.
+
+### SchemaSerializer
+
+The **SchemaSerializer** class is used to serialize data into JSON format. It takes the data to be serialized as input and provides the serialized JSON data as output.
+
+#### Usage
+
+```python
+from sanctify.serializer import SchemaSerializer
+from sanctify.transformer import Transformer
+
+data_to_serialize = {
+    "first_name": {
+        "standard_column": "First Name",
+        "transformations": [
+            Transformer.convert_to_lowercase,
+            Transformer.replace_ii_with_II,
+            Transformer.convert_jr_to_Junior,
+            Transformer.convert_sr_to_Senior,
+            Transformer.remove_dot_from_string,
+        ],
+    },
+}
+
+# Serialize the data
+serializer = SchemaSerializer(data_to_serialize)
+serialized_data = serializer.data
+
+print(serialized_data)
+# Output:
+"""
+{
+    "first_name": {
+        "standard_column": "First Name",
+        "transformations": [
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_to_lowercase",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "replace_ii_with_II",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_jr_to_Junior",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_sr_to_Senior",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "remove_dot_from_string",
+                "static_method_args": [
+                    "value"
+                ]
+            }
+        ]
+    }
+}
+"""
+```
+
+### SchemaDeSerializer
+
+The **SchemaDeSerializer** class is used to deserialize JSON data back into Python data structures. It takes the JSON data as input and provides the deserialized data as output.
+
+#### Usage
+
+```python
+from sanctify.serializer import SchemaDeSerializer
+from sanctify.transformer import Transformer
+
+serialized_data = """
+{
+    "first_name": {
+        "standard_column": "First Name",
+        "transformations": [
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_to_lowercase",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "replace_ii_with_II",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_jr_to_Junior",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "convert_sr_to_Senior",
+                "static_method_args": [
+                    "value"
+                ]
+            },
+            {
+                "class_name": "Transformer",
+                "static_method_name": "remove_dot_from_string",
+                "static_method_args": [
+                    "value"
+                ]
+            }
+        ]
+    }
+}
+"""
+
+# Deserialize the data
+deserializer = SchemaDeSerializer(serialized_data)
+deserialized_data = deserializer.data
+
+print(deserialized_data)
+# Output:
+"""
+{
+    "first_name": {
+        "standard_column": "First Name",
+        "transformations": [
+            Transformer.convert_to_lowercase,
+            Transformer.replace_ii_with_II,
+            Transformer.convert_jr_to_Junior,
+            Transformer.convert_sr_to_Senior,
+            Transformer.remove_dot_from_string,
+        ],
+    },
+}
+"""
+```
+
 ## Contributing
+
 Contributions to Sanctify are welcome! If you find any bugs, have feature requests, or want to contribute code, please open an issue or submit a pull request on the [GitHub repository](https://github.com/skit-ai/sanctify/).
+
+Before starting: Make sure to create a python3.11 virtual env install the pre-commit hook
+
+```shell
+python3.11 -m venv venv && source venv/bin/activate && pip install pre-commit && pre-commit install
+```
```

