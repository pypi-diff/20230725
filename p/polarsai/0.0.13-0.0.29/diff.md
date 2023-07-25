# Comparing `tmp/polarsai-0.0.13.tar.gz` & `tmp/polarsai-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polarsai-0.0.13.tar", last modified: Fri Jul 21 19:18:43 2023, max compression
+gzip compressed data, was "polarsai-0.0.29.tar", last modified: Tue Jul 25 18:44:50 2023, max compression
```

## Comparing `polarsai-0.0.13.tar` & `polarsai-0.0.29.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 19:18:43.623059 polarsai-0.0.13/
--rw-rw-rw-   0        0        0    35823 2023-07-20 15:34:22.000000 polarsai-0.0.13/LICENSE
--rw-rw-rw-   0        0        0      933 2023-07-21 19:18:43.623059 polarsai-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-20 15:03:35.000000 polarsai-0.0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 19:18:43.545117 polarsai-0.0.13/polarsai/
-drwxrwxrwx   0        0        0        0 2023-07-21 19:18:43.572115 polarsai-0.0.13/polarsai/helpers/
--rw-rw-rw-   0        0        0        0 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/__init__.py
--rw-rw-rw-   0        0        0     3940 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/_optional.py
--rw-rw-rw-   0        0        0     1812 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/cache.py
--rw-rw-rw-   0        0        0     1318 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/constants.py
--rw-rw-rw-   0        0        0     1582 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/exceptions.py
--rw-rw-rw-   0        0        0      590 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/from_excel.py
--rw-rw-rw-   0        0        0     1542 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/notebook.py
--rw-rw-rw-   0        0        0     3587 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/save_chart.py
--rw-rw-rw-   0        0        0    10287 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/helpers/shortcuts.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:18:43.580116 polarsai-0.0.13/polarsai/llm/
--rw-rw-rw-   0        0        0        0 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/llm/__init__.py
--rw-rw-rw-   0        0        0     2763 2023-07-20 17:36:44.000000 polarsai-0.0.13/polarsai/llm/base.py
--rw-rw-rw-   0        0        0      521 2023-07-20 16:01:05.000000 polarsai-0.0.13/polarsai/llm/langchain_base.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:18:43.604060 polarsai-0.0.13/polarsai/polarsai.egg-info/
--rw-rw-rw-   0        0        0      933 2023-07-21 19:18:43.000000 polarsai-0.0.13/polarsai/polarsai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-07-21 19:18:43.000000 polarsai-0.0.13/polarsai/polarsai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 19:18:43.000000 polarsai-0.0.13/polarsai/polarsai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-21 19:18:43.000000 polarsai-0.0.13/polarsai/polarsai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-21 19:18:43.000000 polarsai-0.0.13/polarsai/polarsai.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 19:18:43.621060 polarsai-0.0.13/polarsai/prompts/
--rw-rw-rw-   0        0        0        0 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/prompts/__init__.py
--rw-rw-rw-   0        0        0      683 2023-07-20 17:36:54.000000 polarsai-0.0.13/polarsai/prompts/base.py
--rw-rw-rw-   0        0        0     1357 2023-07-18 18:50:22.000000 polarsai-0.0.13/polarsai/prompts/correct_error_prompt.py
--rw-rw-rw-   0        0        0     1113 2023-07-18 15:52:31.000000 polarsai-0.0.13/polarsai/prompts/correct_multiples_prompt.py
--rw-rw-rw-   0        0        0     1155 2023-07-03 18:23:41.000000 polarsai-0.0.13/polarsai/prompts/generate_python_code.py
--rw-rw-rw-   0        0        0      482 2023-06-30 20:32:59.000000 polarsai-0.0.13/polarsai/prompts/generate_response.py
--rw-rw-rw-   0        0        0     1140 2023-07-07 18:02:32.000000 polarsai-0.0.13/polarsai/prompts/multiple_dataframes.py
--rw-rw-rw-   0        0        0      102 2023-07-20 15:04:46.000000 polarsai-0.0.13/pyproject.toml
--rw-rw-rw-   0        0        0      943 2023-07-21 19:18:43.632056 polarsai-0.0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 18:44:50.469164 polarsai-0.0.29/
+-rw-rw-rw-   0        0        0    35823 2023-07-20 15:34:22.000000 polarsai-0.0.29/LICENSE
+-rw-rw-rw-   0        0        0      933 2023-07-25 18:44:50.470162 polarsai-0.0.29/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-20 15:03:35.000000 polarsai-0.0.29/README.md
+-rw-rw-rw-   0        0        0      102 2023-07-20 15:04:46.000000 polarsai-0.0.29/pyproject.toml
+-rw-rw-rw-   0        0        0      917 2023-07-25 18:44:50.478164 polarsai-0.0.29/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 18:44:50.396163 polarsai-0.0.29/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:44:50.408162 polarsai-0.0.29/src/polarsai/
+-rw-rw-rw-   0        0        0        0 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/__init__.py
+-rw-rw-rw-   0        0        0    20989 2023-07-25 18:32:13.000000 polarsai-0.0.29/src/polarsai/core.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:44:50.448164 polarsai-0.0.29/src/polarsai/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/__init__.py
+-rw-rw-rw-   0        0        0     3940 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/_optional.py
+-rw-rw-rw-   0        0        0     1812 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/cache.py
+-rw-rw-rw-   0        0        0     1318 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/constants.py
+-rw-rw-rw-   0        0        0     1582 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/exceptions.py
+-rw-rw-rw-   0        0        0      590 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/from_excel.py
+-rw-rw-rw-   0        0        0     1542 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/notebook.py
+-rw-rw-rw-   0        0        0     3587 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/save_chart.py
+-rw-rw-rw-   0        0        0    10287 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/helpers/shortcuts.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:44:50.454164 polarsai-0.0.29/src/polarsai/llm/
+-rw-rw-rw-   0        0        0        0 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/llm/__init__.py
+-rw-rw-rw-   0        0        0     2754 2023-07-25 18:36:18.000000 polarsai-0.0.29/src/polarsai/llm/base.py
+-rw-rw-rw-   0        0        0      523 2023-07-25 18:43:23.000000 polarsai-0.0.29/src/polarsai/llm/langchain_base.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:44:50.468164 polarsai-0.0.29/src/polarsai/prompts/
+-rw-rw-rw-   0        0        0        0 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/prompts/__init__.py
+-rw-rw-rw-   0        0        0      685 2023-07-25 18:36:35.000000 polarsai-0.0.29/src/polarsai/prompts/base.py
+-rw-rw-rw-   0        0        0     1357 2023-07-18 18:50:22.000000 polarsai-0.0.29/src/polarsai/prompts/correct_error_prompt.py
+-rw-rw-rw-   0        0        0     1113 2023-07-18 15:52:31.000000 polarsai-0.0.29/src/polarsai/prompts/correct_multiples_prompt.py
+-rw-rw-rw-   0        0        0     1155 2023-07-03 18:23:41.000000 polarsai-0.0.29/src/polarsai/prompts/generate_python_code.py
+-rw-rw-rw-   0        0        0      482 2023-06-30 20:32:59.000000 polarsai-0.0.29/src/polarsai/prompts/generate_response.py
+-rw-rw-rw-   0        0        0     1140 2023-07-07 18:02:32.000000 polarsai-0.0.29/src/polarsai/prompts/multiple_dataframes.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:44:50.431162 polarsai-0.0.29/src/polarsai.egg-info/
+-rw-rw-rw-   0        0        0      933 2023-07-25 18:44:50.000000 polarsai-0.0.29/src/polarsai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2023-07-25 18:44:50.000000 polarsai-0.0.29/src/polarsai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:44:50.000000 polarsai-0.0.29/src/polarsai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-07-25 18:44:50.000000 polarsai-0.0.29/src/polarsai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 18:44:50.000000 polarsai-0.0.29/src/polarsai.egg-info/top_level.txt
```

### Comparing `polarsai-0.0.13/LICENSE` & `polarsai-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/PKG-INFO` & `polarsai-0.0.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarsai
-Version: 0.0.13
+Version: 0.0.29
 Summary: poalrsai is an integration between the Python Polars library and LLM models created by Aimpoint Digital, LP
 Home-page: https://github.com/Aimpoint-Digital/polars-ai
 Author: Aaron McClendon
 Author-email: aaron.mcclendon@aimpointdigital.com
 Project-URL: Bug Tracker, https://github.com/Aimpoint-Digital/polars-ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `polarsai-0.0.13/polarsai/helpers/_optional.py` & `polarsai-0.0.29/src/polarsai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/helpers/cache.py` & `polarsai-0.0.29/src/polarsai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/helpers/constants.py` & `polarsai-0.0.29/src/polarsai/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/helpers/exceptions.py` & `polarsai-0.0.29/src/polarsai/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/helpers/from_excel.py` & `polarsai-0.0.29/src/polarsai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/helpers/notebook.py` & `polarsai-0.0.29/src/polarsai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/helpers/save_chart.py` & `polarsai-0.0.29/src/polarsai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/helpers/shortcuts.py` & `polarsai-0.0.29/src/polarsai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/llm/base.py` & `polarsai-0.0.29/src/polarsai/llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,23 @@
 from langchain.llms.sagemaker_endpoint import LLMContentHandler, SagemakerEndpoint
 import sys
 
 
 import openai
 import requests
 
-from helpers.exceptions import (
+from ..helpers.exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
 
-from helpers._optional import import_dependency
-from prompts.base import Prompt
+from ..helpers._optional import import_dependency
+from ..prompts.base import Prompt
 
-load_dotenv()
 
 class Query:
 
     def _polish_code(self, code: str) -> str:
         """
         Polish the code by removing the leading "python" or "py",  \
         removing the imports and removing trailing spaces and new lines.
```

### Comparing `polarsai-0.0.13/polarsai/llm/langchain_base.py` & `polarsai-0.0.29/src/polarsai/llm/langchain_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from prompts.base import Prompt
+from ..prompts.base import Prompt
 
 
 class LangchainLLM:
     """
     Class to wrap Langchain LLMs 
     """
```

### Comparing `polarsai-0.0.13/polarsai/polarsai.egg-info/PKG-INFO` & `polarsai-0.0.29/src/polarsai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarsai
-Version: 0.0.13
+Version: 0.0.29
 Summary: poalrsai is an integration between the Python Polars library and LLM models created by Aimpoint Digital, LP
 Home-page: https://github.com/Aimpoint-Digital/polars-ai
 Author: Aaron McClendon
 Author-email: aaron.mcclendon@aimpointdigital.com
 Project-URL: Bug Tracker, https://github.com/Aimpoint-Digital/polars-ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `polarsai-0.0.13/polarsai/prompts/base.py` & `polarsai-0.0.29/src/polarsai/prompts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Base class to implement a new Prompt
 In order to better handle the instructions, this prompt module is written.
 """
 import sys
-from helpers.exceptions import MethodNotImplementedError
+from ..helpers.exceptions import MethodNotImplementedError
 
 
 class Prompt:
     """Base class to implement a new Prompt"""
 
     text = None
     _args = {}
```

### Comparing `polarsai-0.0.13/polarsai/prompts/correct_error_prompt.py` & `polarsai-0.0.29/src/polarsai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/prompts/correct_multiples_prompt.py` & `polarsai-0.0.29/src/polarsai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/prompts/generate_python_code.py` & `polarsai-0.0.29/src/polarsai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/polarsai/prompts/multiple_dataframes.py` & `polarsai-0.0.29/src/polarsai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `polarsai-0.0.13/setup.cfg` & `polarsai-0.0.29/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6c 6172 7361 690d 0a76 6572   = polarsai..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e31 330d 0a61  sion = 0.0.13..a
+00000020: 7369 6f6e 203d 2030 2e30 2e32 390d 0a61  sion = 0.0.29..a
 00000030: 7574 686f 7220 3d20 4161 726f 6e20 4d63  uthor = Aaron Mc
 00000040: 436c 656e 646f 6e0d 0a61 7574 686f 725f  Clendon..author_
 00000050: 656d 6169 6c20 3d20 6161 726f 6e2e 6d63  email = aaron.mc
 00000060: 636c 656e 646f 6e40 6169 6d70 6f69 6e74  clendon@aimpoint
 00000070: 6469 6769 7461 6c2e 636f 6d0d 0a64 6573  digital.com..des
 00000080: 6372 6970 7469 6f6e 203d 2070 6f61 6c72  cription = poalr
 00000090: 7361 6920 6973 2061 6e20 696e 7465 6772  sai is an integr
@@ -34,26 +34,25 @@
 00000210: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
 00000220: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
 00000230: 6c69 6320 4c69 6365 6e73 6520 7633 2028  lic License v3 (
 00000240: 4750 4c76 3329 0d0a 094f 7065 7261 7469  GPLv3)...Operati
 00000250: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
 00000260: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
 00000270: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000280: 655f 6469 7220 3d20 0d0a 093d 2070 6f6c  e_dir = ...= pol
-00000290: 6172 7361 690d 0a70 6163 6b61 6765 7320  arsai..packages 
-000002a0: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-000002b0: 7265 7175 6972 6573 203d 203e 3d33 2e31  requires = >=3.1
-000002c0: 300d 0a69 6e63 6c75 6465 5f70 6163 6b61  0..include_packa
-000002d0: 6765 5f64 6174 6120 3d20 7472 7565 0d0a  ge_data = true..
-000002e0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-000002f0: 203d 200d 0a09 6173 746f 720d 0a09 6970   = ...astor...ip
-00000300: 7974 686f 6e0d 0a09 6c61 6e67 6368 6169  ython...langchai
-00000310: 6e0d 0a09 7061 6e64 6173 0d0a 0970 616e  n...pandas...pan
-00000320: 6461 7361 690d 0a09 706f 6c61 7273 0d0a  dasai...polars..
-00000330: 0970 7974 686f 6e2d 646f 7465 6e76 0d0a  .python-dotenv..
-00000340: 0952 6571 7565 7374 730d 0a09 7665 7274  .Requests...vert
-00000350: 6578 6169 0d0a 0d0a 5b6f 7074 696f 6e73  exai....[options
-00000360: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000370: 0a77 6865 7265 203d 2070 6f6c 6172 7361  .where = polarsa
-00000380: 690d 0a0d 0a5b 6567 675f 696e 666f 5d0d  i....[egg_info].
-00000390: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000003a0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000280: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
+00000290: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+000002a0: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+000002b0: 7265 7320 3d20 3e3d 332e 3130 0d0a 696e  res = >=3.10..in
+000002c0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+000002d0: 7461 203d 2074 7275 650d 0a69 6e73 7461  ta = true..insta
+000002e0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+000002f0: 0961 7374 6f72 0d0a 0969 7079 7468 6f6e  .astor...ipython
+00000300: 0d0a 096c 616e 6763 6861 696e 0d0a 0970  ...langchain...p
+00000310: 616e 6461 730d 0a09 7061 6e64 6173 6169  andas...pandasai
+00000320: 0d0a 0970 6f6c 6172 730d 0a09 5265 7175  ...polars...Requ
+00000330: 6573 7473 0d0a 0976 6572 7465 7861 690d  ests...vertexai.
+00000340: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000350: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000360: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
+00000370: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000380: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000390: 300d 0a0d 0a                             0....
```

