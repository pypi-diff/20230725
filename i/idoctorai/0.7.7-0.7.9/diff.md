# Comparing `tmp/idoctorai-0.7.7.tar.gz` & `tmp/idoctorai-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.7.7.tar", max compression
+gzip compressed data, was "idoctorai-0.7.9.tar", max compression
```

## Comparing `idoctorai-0.7.7.tar` & `idoctorai-0.7.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.7.7/LICENSE
--rw-r--r--   0        0        0    27947 2023-07-18 12:42:54.467639 idoctorai-0.7.7/pandasai/__init__.py
--rw-r--r--   0        0        0     1318 2023-07-07 01:08:43.311575 idoctorai-0.7.7/pandasai/constants.py
--rw-r--r--   0        0        0     1582 2023-07-07 01:01:47.982275 idoctorai-0.7.7/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.7.7/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3940 2023-07-07 01:01:47.982275 idoctorai-0.7.7/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5613 2023-07-07 01:01:47.983273 idoctorai-0.7.7/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1812 2023-07-07 01:01:47.984270 idoctorai-0.7.7/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.7.7/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1542 2023-07-07 01:01:47.984270 idoctorai-0.7.7/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3643 2023-07-18 13:15:27.413098 idoctorai-0.7.7/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0    10287 2023-07-07 01:01:47.985267 idoctorai-0.7.7/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0     4643 2023-07-08 01:22:44.839806 idoctorai-0.7.7/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0       68 2023-07-17 02:43:35.387669 idoctorai-0.7.7/pandasai/langchain/agents.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.7.7/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4466 2023-07-07 01:01:47.986265 idoctorai-0.7.7/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    14051 2023-07-12 13:05:59.808678 idoctorai-0.7.7/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.7.7/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1264 2023-07-07 01:01:47.986265 idoctorai-0.7.7/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4609 2023-07-07 01:01:47.986265 idoctorai-0.7.7/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      599 2023-07-07 01:01:47.987262 idoctorai-0.7.7/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     4154 2023-07-07 14:00:39.632140 idoctorai-0.7.7/pandasai/llm/model.py
--rw-r--r--   0        0        0     1535 2023-07-07 01:01:47.988259 idoctorai-0.7.7/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3599 2023-07-07 14:00:39.633137 idoctorai-0.7.7/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.7.7/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-07 01:01:47.988259 idoctorai-0.7.7/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      693 2023-07-07 01:01:47.988259 idoctorai-0.7.7/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      986 2023-07-07 01:01:47.989256 idoctorai-0.7.7/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      678 2023-07-07 01:01:47.989256 idoctorai-0.7.7/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.7.7/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      674 2023-07-07 01:01:47.990254 idoctorai-0.7.7/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1349 2023-07-07 14:00:39.634134 idoctorai-0.7.7/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1125 2023-07-07 14:00:39.635132 idoctorai-0.7.7/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1295 2023-07-07 14:00:39.636130 idoctorai-0.7.7/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      482 2023-07-07 01:01:47.990254 idoctorai-0.7.7/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1339 2023-07-07 14:00:39.637343 idoctorai-0.7.7/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     2064 2023-07-18 13:16:35.876443 idoctorai-0.7.7/pyproject.toml
--rw-r--r--   0        0        0       96 2023-07-07 14:00:39.620963 idoctorai-0.7.7/README.md
--rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 idoctorai-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.7.9/LICENSE
+-rw-r--r--   0        0        0    28474 2023-07-25 08:19:48.259599 idoctorai-0.7.9/pandasai/__init__.py
+-rw-r--r--   0        0        0     1318 2023-07-07 01:08:43.311575 idoctorai-0.7.9/pandasai/constants.py
+-rw-r--r--   0        0        0     1582 2023-07-07 01:01:47.982275 idoctorai-0.7.9/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.7.9/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3940 2023-07-07 01:01:47.982275 idoctorai-0.7.9/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5613 2023-07-07 01:01:47.983273 idoctorai-0.7.9/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1812 2023-07-07 01:01:47.984270 idoctorai-0.7.9/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.7.9/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1542 2023-07-07 01:01:47.984270 idoctorai-0.7.9/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3704 2023-07-25 08:09:02.017916 idoctorai-0.7.9/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0    10287 2023-07-07 01:01:47.985267 idoctorai-0.7.9/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0     4703 2023-07-19 22:40:03.950905 idoctorai-0.7.9/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-17 02:43:35.387669 idoctorai-0.7.9/pandasai/langchain/agents.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.7.9/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4466 2023-07-07 01:01:47.986265 idoctorai-0.7.9/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    14051 2023-07-12 13:05:59.808678 idoctorai-0.7.9/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.7.9/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1264 2023-07-07 01:01:47.986265 idoctorai-0.7.9/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4609 2023-07-07 01:01:47.986265 idoctorai-0.7.9/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      599 2023-07-07 01:01:47.987262 idoctorai-0.7.9/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     4154 2023-07-07 14:00:39.632140 idoctorai-0.7.9/pandasai/llm/model.py
+-rw-r--r--   0        0        0     1535 2023-07-07 01:01:47.988259 idoctorai-0.7.9/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3599 2023-07-07 14:00:39.633137 idoctorai-0.7.9/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.7.9/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-07 01:01:47.988259 idoctorai-0.7.9/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      693 2023-07-07 01:01:47.988259 idoctorai-0.7.9/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      986 2023-07-07 01:01:47.989256 idoctorai-0.7.9/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      678 2023-07-07 01:01:47.989256 idoctorai-0.7.9/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.7.9/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      674 2023-07-07 01:01:47.990254 idoctorai-0.7.9/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1349 2023-07-07 14:00:39.634134 idoctorai-0.7.9/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1125 2023-07-07 14:00:39.635132 idoctorai-0.7.9/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1295 2023-07-07 14:00:39.636130 idoctorai-0.7.9/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      482 2023-07-07 01:01:47.990254 idoctorai-0.7.9/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1339 2023-07-07 14:00:39.637343 idoctorai-0.7.9/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     2064 2023-07-25 08:19:56.298637 idoctorai-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-07-07 14:00:39.620963 idoctorai-0.7.9/README.md
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 idoctorai-0.7.9/PKG-INFO
```

### Comparing `idoctorai-0.7.7/LICENSE` & `idoctorai-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/__init__.py` & `idoctorai-0.7.9/pandasai/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -655,14 +655,17 @@
 
         Returns (str): String representation of the result of the code execution.
 
         """
 
         multiple: bool = isinstance(data_frame, list)
 
+        # code = "import pandas as pd\nimport matplotlib.pyplot as plt\n\ndf1 = pd.read_csv('path/to/df1.csv') # assuming data is in a csv file\ndf1['SITE_LATITUDE'] = pd.to_numeric(df1['SITE_LATITUDE']) # convert latitude column to numeric\ndf1['SITE_LONGITUDE'] = pd.to_numeric(df1['SITE_LONGITUDE']) # convert longitude column to numeric\n\nplt.scatter(df1['SITE_LONGITUDE'], df1['SITE_LATITUDE'])\nplt.xlabel('Longitude')\nplt.ylabel('Latitude')\nplt.show(block=False)\n\n"
+        # code = "plt.show(block=False)\n\n"
+
         # Add save chart code
         if self._save_charts:
             obj = add_save_chart(
                 code, self._prompt_id, self._save_charts_path, not self._verbose
             )
             # record img save path
             code = obj[0]
```

### Comparing `idoctorai-0.7.7/pandasai/constants.py` & `idoctorai-0.7.9/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/exceptions.py` & `idoctorai-0.7.9/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/helpers/_optional.py` & `idoctorai-0.7.9/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/helpers/anonymizer.py` & `idoctorai-0.7.9/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/helpers/cache.py` & `idoctorai-0.7.9/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/helpers/from_excel.py` & `idoctorai-0.7.9/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/helpers/notebook.py` & `idoctorai-0.7.9/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/helpers/save_chart.py` & `idoctorai-0.7.9/pandasai/helpers/save_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     if type(node1) is not type(node2):
         return False
 
     if isinstance(node1, ast.AST):
         for k, node in vars(node1).items():
             if k in {"lineno", "end_lineno", "col_offset", "end_col_offset", "ctx"}:
                 continue
-            if ignore_args and k == "args":
+            # ignore args and keywords
+            if ignore_args and (k == "args" or k == "keywords"):
                 continue
             if not compare_ast(node, getattr(node2, k), ignore_args):
                 return False
         return True
 
     if isinstance(node1, list) and isinstance(node2, list):
         return all(
```

### Comparing `idoctorai-0.7.7/pandasai/helpers/shortcuts.py` & `idoctorai-0.7.9/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/langchain/__init__.py` & `idoctorai-0.7.9/pandasai/langchain/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
 {history}
 Human: {human_input}
 Assistant:"""
 
     template= """Assistant is a large language model trained by OpenAI.Assistant can complete the prediction based on the incomplete data I provided.
 
+mark text descriptions unrelated to the code as comments
+
 {history}
 Human: {human_input}
 Assistant:"""
 
     def __init__(self, llm: AzureOpenAI, **kwargs,):
         # self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0)
         if llm is None:
```

### Comparing `idoctorai-0.7.7/pandasai/llm/azure_openai.py` & `idoctorai-0.7.9/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/base.py` & `idoctorai-0.7.9/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/fake.py` & `idoctorai-0.7.9/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/falcon.py` & `idoctorai-0.7.9/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/google_palm.py` & `idoctorai-0.7.9/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/langchain.py` & `idoctorai-0.7.9/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/model.py` & `idoctorai-0.7.9/pandasai/llm/model.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/open_assistant.py` & `idoctorai-0.7.9/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/openai.py` & `idoctorai-0.7.9/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/llm/starcoder.py` & `idoctorai-0.7.9/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/middlewares/base.py` & `idoctorai-0.7.9/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/middlewares/charts.py` & `idoctorai-0.7.9/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/middlewares/streamlit.py` & `idoctorai-0.7.9/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/prompts/base.py` & `idoctorai-0.7.9/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.7.9/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.7.9/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/prompts/generate_python_code.py` & `idoctorai-0.7.9/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.7.9/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.7/pyproject.toml` & `idoctorai-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.7.7"
+version = "0.7.9"
 description = "Idoctor AI is a Python library that integrates generative artificial intelligence capabilities into Pandas."
 authors = ["FH"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `idoctorai-0.7.7/PKG-INFO` & `idoctorai-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.7.7
+Version: 0.7.9
 Summary: Idoctor AI is a Python library that integrates generative artificial intelligence capabilities into Pandas.
 License: MIT
 Author: FH
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

