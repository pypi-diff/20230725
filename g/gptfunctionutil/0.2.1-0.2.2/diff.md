# Comparing `tmp/gptfunctionutil-0.2.1.tar.gz` & `tmp/gptfunctionutil-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptfunctionutil-0.2.1.tar", last modified: Thu Jul 20 17:32:32 2023, max compression
+gzip compressed data, was "gptfunctionutil-0.2.2.tar", last modified: Tue Jul 25 20:34:51 2023, max compression
```

## Comparing `gptfunctionutil-0.2.1.tar` & `gptfunctionutil-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:32:32.319118 gptfunctionutil-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:32:32.315118 gptfunctionutil-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:32:32.315118 gptfunctionutil-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/.github/workflows/publishpackage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:32:32.315118 gptfunctionutil-0.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-07-20 17:32:32.319118 gptfunctionutil-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:32:32.319118 gptfunctionutil-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:32:32.319118 gptfunctionutil-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:32:32.319118 gptfunctionutil-0.2.1/src/gptfunctionutil/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/src/gptfunctionutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/src/gptfunctionutil/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/src/gptfunctionutil/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/src/gptfunctionutil/functionlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/src/gptfunctionutil/functionlib_discord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:32:32.319118 gptfunctionutil-0.2.1/src/gptfunctionutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-07-20 17:32:32.000000 gptfunctionutil-0.2.1/src/gptfunctionutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-20 17:32:32.000000 gptfunctionutil-0.2.1/src/gptfunctionutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:32:32.000000 gptfunctionutil-0.2.1/src/gptfunctionutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-20 17:32:32.000000 gptfunctionutil-0.2.1/src/gptfunctionutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 17:32:32.000000 gptfunctionutil-0.2.1/src/gptfunctionutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:32:32.319118 gptfunctionutil-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-20 17:32:12.000000 gptfunctionutil-0.2.1/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.229600 gptfunctionutil-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.221600 gptfunctionutil-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/.github/workflows/publishpackage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/examples/custom_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:34:51.229600 gptfunctionutil-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/src/gptfunctionutil/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/converter_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/convertutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/functionlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/functionlib_discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/tests/test_methods.py
```

### Comparing `gptfunctionutil-0.2.1/.github/workflows/publishpackage.yaml` & `gptfunctionutil-0.2.2/.github/workflows/publishpackage.yaml`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.1/.gitignore` & `gptfunctionutil-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.1/.vscode/settings.json` & `gptfunctionutil-0.2.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.1/LICENSE` & `gptfunctionutil-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.1/PKG-INFO` & `gptfunctionutil-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,32 +43,34 @@
 ##Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods based on the returned function_call attribute.
+- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods utilizing the Function Call field returned with a call to chat/completions.
 
 - **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
   + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
   + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
   + (`@LibParamSpec`) can apply additional keywords depending on the type. (see https://json-schema.org/understanding-json-schema/index.html for details.)
 
 
 - **Parameter Typing and Descriptions:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  The library utilizes a collection of converter objects to generate schema for each parameter based on type annotations.
 
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
-   +support for custom converters coming at a later date.
+   + Define Custom Converters to automatically use response arguments to initalize objects.
+     +  (see examples/custom_converters.py for an example.)
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
-   +Simply import gptfunctionutil into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
+   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
-   +The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if a function.) to invoke the corresponding function with the provided arguments.
+   + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
+   + Schema can also validate and convert responces returned from the chat/completions endpoint.
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.2.1/README.md` & `gptfunctionutil-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,32 +7,34 @@
 ##Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods based on the returned function_call attribute.
+- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods utilizing the Function Call field returned with a call to chat/completions.
 
 - **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
   + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
   + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
   + (`@LibParamSpec`) can apply additional keywords depending on the type. (see https://json-schema.org/understanding-json-schema/index.html for details.)
 
 
 - **Parameter Typing and Descriptions:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  The library utilizes a collection of converter objects to generate schema for each parameter based on type annotations.
 
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
-   +support for custom converters coming at a later date.
+   + Define Custom Converters to automatically use response arguments to initalize objects.
+     +  (see examples/custom_converters.py for an example.)
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
-   +Simply import gptfunctionutil into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
+   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
-   +The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if a function.) to invoke the corresponding function with the provided arguments.
+   + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
+   + Schema can also validate and convert responces returned from the chat/completions endpoint.
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.2.1/pyproject.toml` & `gptfunctionutil-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 [project]
 name = 'gptfunctionutil'
-version = "0.2.1"
+version = "0.2.2"
 license = {file = "LICENSE"}
 authors = [{name="Crosswave Omega",email= "xtream2pro@gmail.com"}]
 description = "A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API"
 readme = 'README.md'
 
 keywords = ['OpenAI', 'Function Calling API', 'GPT']
 requires-python = '>=3.10'
```

### Comparing `gptfunctionutil-0.2.1/src/gptfunctionutil/errors.py` & `gptfunctionutil-0.2.2/src/gptfunctionutil/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-
+from .logger import logs
 class GPTLibError(Exception):
     """Base exception class for the GPT Library."""
     pass
 
 class FunctionNotFound(GPTLibError):
     """Exception raised when a function with a certain name is not found."""
 
@@ -39,21 +39,30 @@
 
 class ConversionError(GPTLibError):
     """Exception raised when Something went wrong when converting/validating a responce."""
 
     def __init__(self, message):
         super().__init__(message)
 
-class ConversiontToError(ConversionError):
+class ConversionToError(ConversionError):
+
+    def __init__(self, param_name='', param='', schema={}, msg=''):
+        self.param_name=param_name
+        self.param=''
+        self.dec=schema
+        message=f"{msg} Param:{param_name} of type {param}.\n could not be converted into a schema!"
+        super().__init__(message)
+
+
+class ConversionAddError(ConversionError):
 
     def __init__(self, msg=''):
         super().__init__(msg)
 
 
-
 class ConversionFromError(ConversionError):
 
     def __init__(self, param_name='', value='', schema={}, msg=''):
         self.param_name=param_name
         self.value=value
         self.schema=schema
         message=f"{msg} Param:{param_name}. Value{value}.\n Schema:{str(schema)}"
```

### Comparing `gptfunctionutil-0.2.1/src/gptfunctionutil/functionlib.py` & `gptfunctionutil-0.2.2/src/gptfunctionutil/functionlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from .logger import logs
+
 import inspect
 import json
 import re
 from typing import Any, Coroutine, Dict, List, Union
 
 from enum import Enum, EnumMeta
 
 from datetime import datetime
 
 from .errors import *
-from .converter import ConvertStatic
+from .convertutil import ConvertStatic
 
 class CommandSingleton:
     _instance = None
     _commands = {}
 
     @classmethod
     def get_instance(cls):
@@ -48,15 +50,15 @@
         '''
         self.command=func
         self.internal_name=self.function_name=name
         self.comm_type='callable'
 
         if inspect.iscoroutinefunction(func):
             self.comm_type='coroutine'
-        print(self.function_name,self.comm_type)
+        logs.info("adding %s, comm type is %s",self.function_name,self.comm_type)
         my_schema= {
             'name': self.function_name,
             'description': description,
             'parameters':{'type': 'object','properties': {},'required': []}
         }
 
         self.function_schema=my_schema
@@ -76,15 +78,15 @@
         paramdict={}
         param_decorators={}
 
         sig = inspect.signature(func)
         if hasattr(func,'parameter_decorators'):
             paramdict=sig.parameters
             param_decorators=func.parameter_decorators
-        print("THE type is",self.comm_type)
+
         self.function_schema.update(
             { 'parameters': {'type': 'object','properties': {},'required': []}}
         )
         for param_name, param in paramdict.items():
             decs=param_decorators.get(param_name, '')
 
             param_info, converter=ConvertStatic.parameter_into_schema(param_name,param,dec=decs)
@@ -129,21 +131,23 @@
             gpt-3.5-turbo-0613
 
         Returns:
             Dict[str, Any]: The converted function argument dictionary.
         '''
         schema=self.function_schema
         parameters=schema['parameters']
-        print('args',function_args)
+        logs.info("converting args for function %s, args:%s", self.function_name,function_args)
+
         for i, v in parameters['properties'].items():
             if i in function_args:
                 converter=self.param_converters[i]
-                print('typehere','converter')
+
                 result=ConvertStatic.schema_validate(i,function_args[i],v,converter)
-                print(i,result)
+
+                logs.info("arg %s converted into %s", i,result)
                 function_args[i]=result
         return function_args
 
     def check_force(self,query:str) -> bool:
         '''
         Checks if the given query contains any of the command's force words.
 
@@ -246,30 +250,29 @@
             '''In case I want to change how I want to parse expressions later.'''
             expression_detect_pattern = r'(?<=:\s)([^"]*?[+\-*/][^"]*?)(?=(?:,|\s*\}))'
             return re.sub(expression_detect_pattern, lambda m: self.my_math_parser(m.group()), function_args)
         return function_args
 
     def parse_name_args(self, function_dict: Dict[str, Any]) -> Dict[str, Any]:
         '''parse the args within function_dict, and apply any needed corrections to the JSON.'''
-        print(function_dict)
         function_name = function_dict.get('name')
         function_args = function_dict.get('arguments', None)
         if function_name in self.FunctionDict:
             if isinstance(function_args,str):
                 #Making it so it won't break on poorly formatted function arguments.
                 function_args=function_args.replace("\\n",'\n')
                 quoteescapefixpattern = r"(?<=:\s\")(.*?)(?=\"(?:,|\s*\}))"
                 #In testing, I once had the API return a poorly escaped function_args attribute
                 #That could not be parsed by json.loads, so hence this regex.
                 function_args_str=re.sub(quoteescapefixpattern, lambda m: m.group().replace('"', r'\"'), function_args)
 
                 #This regex is for detecting if there's an expression as a value and not a single integer.
                 #Which has happened before during testing.
                 function_args_str=self.expression_match(function_args_str)
-                print(function_args_str)
+                logs.info('transformed json args for func %s.  result:\n%s',function_name,function_args_str)
                 try:
                     function_args=json.loads(function_args_str, strict=False)
                 except json.JSONDecodeError as e:
                     #Something went wrong while parsing, return where.
                     output=f"JSONDecodeError: {e.msg} at line {e.lineno} column {e.colno}: `{function_args_str[e.pos]}`"
                     raise ArgDecodeError(function_name=function_name,arguments=function_args_str,msg=f"{output}", er=e)
             return function_name,function_args
@@ -340,15 +343,14 @@
     Returns:
         The decorated function.
     """
     def decorator(func: callable) -> callable:
         if not hasattr(func, "parameter_decorators"):
             func.parameter_decorators = {}
         gen=genspec(name,description,**kwargs)
-        print(gen)
         func.parameter_decorators.update(gen)
         return func
     return decorator
 
 def LibParam(**kwargs: Any) -> Any:
     """
     Decorator to add descriptions to any valid parameter inside a GPTFunctionLibary method or discord.py bot command.
@@ -381,14 +383,13 @@
         required:List[str]: list of parameters you want the AI to always use reguardless of if they have defaults.
         force_words:List[str]: list of words that will be used to force this command to be triggered.
         enabled (bool): Whether or not this function is enabled by default.
     Returns:
         callable, Coroutine, or Command.
     """
     def decorator(func: Union[callable,Coroutine]):
-        print("ADDING CALLABLE",func,name)
         mycommand=LibCommand(func,name,description,required,force_words,enabled)
         func.libcommand=mycommand
 
         return func
 
     return decorator
```

### Comparing `gptfunctionutil-0.2.1/src/gptfunctionutil/functionlib_discord.py` & `gptfunctionutil-0.2.2/src/gptfunctionutil/functionlib_discord.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .logger import logs
 import inspect
 import json
 import re
 from typing import Any, Coroutine, Dict, List, Optional, Union
 
 from enum import Enum, EnumMeta
 
@@ -10,15 +11,15 @@
     Command,
     Context,
     Bot,
     CommandNotFound,
     CheckFailure
 )
 from .functionlib import GPTFunctionLibrary, LibCommand, genspec
-from .converter import ConvertStatic
+from .convertutil import ConvertStatic
 from .errors import *
 class CommandSingleton:
     _instance = None
     _commands = {}
 
     @classmethod
     def get_instance(cls):
@@ -62,15 +63,15 @@
         self.internal_name=self.function_name=name
         self.comm_type='callable'
 
         if isinstance(func, Command):
             self.function_name=func.qualified_name
             self.comm_type='command'
 
-            print(self.function_name,self.comm_type)
+            logs.info("adding %s, comm type is %s",self.function_name,self.comm_type)
             my_schema= {
                 'name': self.function_name,
                 'description': description,
                 'parameters':{'type': 'object','properties': {},'required': []}
             }
 
             self.function_schema=my_schema
@@ -95,15 +96,15 @@
                 paramdict=func.clean_params
                 param_decorators=func.parameter_decorators#['parameter_decorators']
         else:
             sig = inspect.signature(func)
             if hasattr(func,'parameter_decorators'):
                 paramdict=sig.parameters
                 param_decorators=func.parameter_decorators
-        #print("THE type is",self.comm_type)
+
         self.function_schema.update(
             { 'parameters': {'type': 'object','properties': {},'required': []}}
         )
         for param_name, param in paramdict.items():
             decs=param_decorators.get(param_name, '')
 
             param_info, converter=ConvertStatic.parameter_into_schema(param_name,param,dec=decs)
@@ -195,15 +196,16 @@
         """
         Update the FunctionDict with decorated discord.py bot commands.
         This has to be called somewhere before a call to the AI API if you
         want to use the commands.
         """
         for command in bot.walk_commands():
             if "libcommand" in command.extras:
-                print(command.qualified_name, command.extras["libcommand"])
+                logs.info("from command s%, adding %s",command.qualified_name,command.extras["libcommand"])
+
                 function_name = command.qualified_name
                 self.FunctionDict[function_name] = command.extras["libcommand"]
 
 
     async def call_by_dict_ctx(self, ctx:Context, function_dict: Dict[str, Any]) -> Coroutine:
         """
         Call a Coroutine or Bot Command based on the provided dictionary.
@@ -224,15 +226,15 @@
             function_name,function_args=self.parse_name_args(function_dict)
         except GPTLibError as e:
             if isinstance(e, FunctionNotFound):
                 return self.default_callback(e.function_name,e.arguments)
 
             result=str(e)
             return result
-        print(function_name, function_args,len(function_args))
+        logs.info('calling function %s with args %s',function_name, function_args)
         libmethod = self.FunctionDict.get(function_name)
         if libmethod.comm_type=='command':
             return await libmethod.invoke_command(ctx, function_args)
 
         else:
             if libmethod.comm_type=='coroutine':
                 if len(function_args)>0:
@@ -261,15 +263,14 @@
     Returns:
         The decorated function.
     """
     def decorator(func: callable) -> callable:
         if not hasattr(func, "parameter_decorators"):
             func.parameter_decorators = {}
         gen=genspec(name,description,**kwargs)
-        print(gen)
         func.parameter_decorators.update(gen)
         return func
     return decorator
 
 def LibParam(**kwargs: Any) -> Any:
     """
     Decorator to add descriptions to any valid parameter inside a GPTFunctionLibary method or discord.py bot command.
@@ -309,14 +310,13 @@
     def decorator(func: Union[Command,callable,Coroutine]):
         if isinstance(func, Command):
             #Added to the extras dictionary in the Command
             mycommand=LibCommandDisc(func,name,description,required,force_words,enabled)
             func.extras['libcommand']=mycommand
             return func
         else:
-            print("ADDING CALLABLE",func,name)
             mycommand=LibCommandDisc(func,name,description,required,force_words,enabled)
             func.libcommand=mycommand
 
             return func
 
     return decorator
```

### Comparing `gptfunctionutil-0.2.1/src/gptfunctionutil.egg-info/PKG-INFO` & `gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,32 +43,34 @@
 ##Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods based on the returned function_call attribute.
+- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods utilizing the Function Call field returned with a call to chat/completions.
 
 - **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
   + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
   + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
   + (`@LibParamSpec`) can apply additional keywords depending on the type. (see https://json-schema.org/understanding-json-schema/index.html for details.)
 
 
 - **Parameter Typing and Descriptions:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  The library utilizes a collection of converter objects to generate schema for each parameter based on type annotations.
 
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
-   +support for custom converters coming at a later date.
+   + Define Custom Converters to automatically use response arguments to initalize objects.
+     +  (see examples/custom_converters.py for an example.)
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
-   +Simply import gptfunctionutil into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
+   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
-   +The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if a function.) to invoke the corresponding function with the provided arguments.
+   + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
+   + Schema can also validate and convert responces returned from the chat/completions endpoint.
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.2.1/src/gptfunctionutil.egg-info/SOURCES.txt` & `gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 .gitattributes
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/publishpackage.yaml
 .vscode/settings.json
+examples/custom_converters.py
 src/README.md
 src/gptfunctionutil/__init__.py
-src/gptfunctionutil/converter.py
+src/gptfunctionutil/converter_core.py
+src/gptfunctionutil/convertutil.py
 src/gptfunctionutil/errors.py
 src/gptfunctionutil/functionlib.py
 src/gptfunctionutil/functionlib_discord.py
+src/gptfunctionutil/logger.py
 src/gptfunctionutil.egg-info/PKG-INFO
 src/gptfunctionutil.egg-info/SOURCES.txt
 src/gptfunctionutil.egg-info/dependency_links.txt
 src/gptfunctionutil.egg-info/requires.txt
 src/gptfunctionutil.egg-info/top_level.txt
 tests/conftest.py
 tests/test_methods.py
```

### Comparing `gptfunctionutil-0.2.1/tests/conftest.py` & `gptfunctionutil-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.1/tests/test_methods.py` & `gptfunctionutil-0.2.2/tests/test_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,27 +185,63 @@
     schema = {'type': 'integer', 'multipleOf': 3}
     with pytest.raises(ValueError):
         converter.from_schema(value, schema)
 
 @pytest.mark.asyncio
 async def test_array_converter_to_schema():
     converter = ArrayConverter()
-    param = inspect.Parameter('param', Parameter.POSITIONAL_OR_KEYWORD, annotation=list)
+    param = inspect.Parameter('param', Parameter.POSITIONAL_OR_KEYWORD, annotation=List[str])
     dec = {'minItems': 1, 'maxItems': 5, 'uniqueItems': True}
-    expected_schema = {'type': 'array', 'items': {}, 'minItems': 1, 'maxItems': 5, 'uniqueItems': True}
-    assert converter.to_schema(param, dec) == expected_schema
-
-@pytest.mark.asyncio
-async def test_array_converter_from_schema():
-    converter = ArrayConverter()
-    value = [1, 2, 3]
-    schema = {'type': 'array', 'items': {}, 'minItems': 1, 'maxItems': 5, 'uniqueItems': True}
-    expected_result = [1, 2, 3]
-    assert converter.from_schema(value, schema) == expected_result
+    expected_schema = {'type': 'array', 'items': {"type":'string'}, 'minItems': 1, 'maxItems': 5, 'uniqueItems': True}
+    schema=converter.to_schema(param, dec)
+    print(schema)
+    assert schema== expected_schema
 
 @pytest.mark.asyncio
 async def test_array_converter_from_schema_with_invalid_value():
     converter = ArrayConverter()
     value = 'test'
     schema = {'type': 'array'}
     with pytest.raises(ValueError):
         converter.from_schema(value, schema)
+
+@pytest.mark.asyncio
+async def test_check_converter():
+    class User:
+        def __init__(self, user):
+            self.user = user
+
+        def __str__(self):
+            return str(self.user)
+
+        def __repr__(self):
+            return str(self.user)
+    class UserConverter(StringConverter):
+        def to_schema(self, param: inspect.Parameter, dec: Dict[str, Any]) -> Dict[str, Any]:
+            schema=super().to_schema(param,dec)
+            schema['pattern']= r'<@!?(\d+)>'
+            return schema
+
+        def from_schema(self, value: Any, schema: Dict[str, Any]) -> Any:
+            value=super().from_schema(value,schema)
+            pat=schema.get('pattern',None)
+            if not pat:
+                raise ValueError("No pattern found.")
+            print(pat)
+            extract=re.match(pat,value)[1]
+            return extract
+    add_converter(User,UserConverter)
+    class MyTestLib6(GPTFunctionLibrary):
+        @AILibFunction(name='get_user',description='Get a specific user id')
+        @LibParam(targetuser='The user to retrieve')
+        def get_user(self,targetuser:User):
+            #This is an example of a decorated coroutine command.
+            return f"{targetuser}"
+
+    testlib3=MyTestLib6()
+    schema = testlib3.get_schema()
+    print(schema)
+
+
+    result=testlib3.call_by_dict({'name':'get_user','arguments':"{\"targetuser\":\"<@1234567890>\"}"})
+    assert result == "1234567890"
+
```

