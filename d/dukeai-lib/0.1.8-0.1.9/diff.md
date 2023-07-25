# Comparing `tmp/dukeai_lib-0.1.8.tar.gz` & `tmp/dukeai_lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukeai_lib-0.1.8.tar", last modified: Tue Jul 25 20:10:46 2023, max compression
+gzip compressed data, was "dukeai_lib-0.1.9.tar", last modified: Tue Jul 25 20:19:30 2023, max compression
```

## Comparing `dukeai_lib-0.1.8.tar` & `dukeai_lib-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:10:46.587574 dukeai_lib-0.1.8/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.8/LICENSE
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2161 2023-07-25 20:10:46.586575 dukeai_lib-0.1.8/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1546 2023-07-25 20:07:46.000000 dukeai_lib-0.1.8/README.md
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:10:46.568575 dukeai_lib-0.1.8/dukeai_lib/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      216 2023-07-25 20:10:31.000000 dukeai_lib-0.1.8/dukeai_lib/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.8/dukeai_lib/application.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:10:46.582574 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      227 2023-07-25 20:09:28.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8317 2023-07-25 19:48:24.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/accessorial.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    17454 2023-07-25 19:48:24.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/bill_of_lading.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    14693 2023-07-25 19:54:51.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/classification.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1294 2023-07-25 19:53:30.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/classification_exceptions.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    13797 2023-07-25 19:35:31.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/invoice.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8933 2023-07-25 19:35:31.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/noa_lor.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8824 2023-07-25 19:54:51.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/parse_classification_page_range.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    64257 2023-07-25 19:35:31.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/rate_confirmation.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     9397 2023-07-25 19:48:24.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/rsi_translator.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8445 2023-07-25 19:48:24.000000 dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/schema_utilities.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.8/dukeai_lib/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.8/dukeai_lib/utilities.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:10:46.572575 dukeai_lib-0.1.8/dukeai_lib.egg-info/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2161 2023-07-25 20:10:46.000000 dukeai_lib-0.1.8/dukeai_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      862 2023-07-25 20:10:46.000000 dukeai_lib-0.1.8/dukeai_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 20:10:46.000000 dukeai_lib-0.1.8/dukeai_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 20:10:46.000000 dukeai_lib-0.1.8/dukeai_lib.egg-info/requires.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-07-25 20:10:46.000000 dukeai_lib-0.1.8/dukeai_lib.egg-info/top_level.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      754 2023-07-25 20:10:31.000000 dukeai_lib-0.1.8/pyproject.toml
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 20:10:46.587574 dukeai_lib-0.1.8/setup.cfg
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      874 2023-07-25 20:10:30.000000 dukeai_lib-0.1.8/setup.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:10:46.585574 dukeai_lib-0.1.8/src/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      204 2023-07-25 18:46:18.000000 dukeai_lib-0.1.8/src/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3601 2023-07-25 18:56:49.000000 dukeai_lib-0.1.8/src/application.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.8/src/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.8/src/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.785006 dukeai_lib-0.1.9/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.9/LICENSE
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2161 2023-07-25 20:19:30.785006 dukeai_lib-0.1.9/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1546 2023-07-25 20:07:46.000000 dukeai_lib-0.1.9/README.md
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.766007 dukeai_lib-0.1.9/dukeai_lib/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      216 2023-07-25 20:19:22.000000 dukeai_lib-0.1.9/dukeai_lib/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.9/dukeai_lib/application.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.781007 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      227 2023-07-25 20:09:28.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8318 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/accessorial.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    17455 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/bill_of_lading.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    14694 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/classification.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1294 2023-07-25 19:53:30.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/classification_exceptions.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    13798 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/invoice.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8933 2023-07-25 19:35:31.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/noa_lor.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8825 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/parse_classification_page_range.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    64258 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/rate_confirmation.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     9397 2023-07-25 19:48:24.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/rsi_translator.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8445 2023-07-25 19:48:24.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/schema_utilities.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.9/dukeai_lib/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.9/dukeai_lib/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.770006 dukeai_lib-0.1.9/dukeai_lib.egg-info/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2161 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      862 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/requires.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      754 2023-07-25 20:19:22.000000 dukeai_lib-0.1.9/pyproject.toml
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 20:19:30.785006 dukeai_lib-0.1.9/setup.cfg
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      874 2023-07-25 20:19:22.000000 dukeai_lib-0.1.9/setup.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.784007 dukeai_lib-0.1.9/src/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      204 2023-07-25 18:46:18.000000 dukeai_lib-0.1.9/src/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3601 2023-07-25 18:56:49.000000 dukeai_lib-0.1.9/src/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.9/src/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.9/src/utilities.py
```

### Comparing `dukeai_lib-0.1.8/LICENSE` & `dukeai_lib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/PKG-INFO` & `dukeai_lib-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai_lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.1.8/README.md` & `dukeai_lib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/dukeai_lib/application.py` & `dukeai_lib-0.1.9/dukeai_lib/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/accessorial.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/accessorial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import json
 import traceback
-from schema_utilities import get_idtype, format_time
+from .schema_utilities import get_idtype, format_time
 
 
 """
 The following schemas and translation functions are intended to be used for any document that falls into the 
 'Accessorial' category >> Lumper, Drayage, Chassis, & Detention
 """
```

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/bill_of_lading.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/bill_of_lading.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import json
 import traceback
-from schema_utilities import get_idtype, format_time, format_state
+from .schema_utilities import get_idtype, format_time, format_state
 
 
 def get_flat_entity_schema():
     return {
         "type": None,
         "name": None,
         "address": None,
```

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/classification.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import traceback
 import json
 import decimal
-from parse_classification_page_range import parse_page_range
+from .parse_classification_page_range import parse_page_range
 
 
 def get_main_schema():
     main_schema = {
         "headers": {
             "Classify Document": {
                 "classification": "N/A"
```

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/classification_exceptions.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/classification_exceptions.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/invoice.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import json
 import re
 import traceback
-from schema_utilities import get_idtype, parse_incoming_address, parse_time, format_state
+from .schema_utilities import get_idtype, parse_incoming_address, parse_time, format_state
 
 
 def get_date_schema():
     return {
         "date": None,
         "time": None,
         "datetype": None
```

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/noa_lor.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/noa_lor.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/parse_classification_page_range.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/parse_classification_page_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 import traceback
-from classification_exceptions import SelectionOutOfRange, ReversedRange, UnbalancedPageRange, NotZeroIndex
+from .classification_exceptions import SelectionOutOfRange, ReversedRange, UnbalancedPageRange, NotZeroIndex
 
 
 """
 Functionality for parsing the page ranges for 'MULTIPLE' document classification scenarios.
 
 Who knows what the annotators will enter, so we account for all of the basic scenarios via RegEx.
 """
```

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/rate_confirmation.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/rate_confirmation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import traceback
 import re
 import datetime
 from dukeai_lib.utilities import DecimalEncoder
-from schema_utilities import get_idtype, REFERENCE_OPTIONS, STATES
+from .schema_utilities import get_idtype, REFERENCE_OPTIONS, STATES
 
 
 def get_main_schema():
     main_schema = {
         "headers": {
             "General": {},
             "Broker Details": {},
```

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/rsi_translator.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/rsi_translator.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/dukeai_lib/schema_kung_fu/schema_utilities.py` & `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/schema_utilities.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/dukeai_lib/tools.py` & `dukeai_lib-0.1.9/dukeai_lib/tools.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/dukeai_lib.egg-info/PKG-INFO` & `dukeai_lib-0.1.9/dukeai_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai-lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.1.8/dukeai_lib.egg-info/SOURCES.txt` & `dukeai_lib-0.1.9/dukeai_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/pyproject.toml` & `dukeai_lib-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-systems]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukeai_lib"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Blake Donahoo", email="blake@duke.ai" },
 ]
 description = "Common functions used across the DUKE.ai project environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dukeai_lib-0.1.8/setup.py` & `dukeai_lib-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dukeai_lib',
-    version="0.1.8",
+    version="0.1.9",
     description="Common functions used across the DUKE.ai project environments.",
     url='https://duke.ai',
     author='Blake Donahoo',
     author_email='blake@duke.ai',
     license='GNU General Public License v3 (GPLv3)',
     packages=find_packages(),
     keywords=['dukeai', 'duke.ai'],
```

### Comparing `dukeai_lib-0.1.8/src/application.py` & `dukeai_lib-0.1.9/src/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.8/src/tools.py` & `dukeai_lib-0.1.9/src/tools.py`

 * *Files identical despite different names*

