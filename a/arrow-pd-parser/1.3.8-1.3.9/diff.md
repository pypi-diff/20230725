# Comparing `tmp/arrow_pd_parser-1.3.8.tar.gz` & `tmp/arrow_pd_parser-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrow_pd_parser-1.3.8.tar", max compression
+gzip compressed data, was "arrow_pd_parser-1.3.9.tar", max compression
```

## Comparing `arrow_pd_parser-1.3.8.tar` & `arrow_pd_parser-1.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    12064 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/README.md
--rw-r--r--   0        0        0       22 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/__init__.py
--rw-r--r--   0        0        0    13642 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/_arrow_parsers.py
--rw-r--r--   0        0        0     4059 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/_export.py
--rw-r--r--   0        0        0    14789 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/_readers.py
--rw-r--r--   0        0        0    14430 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/_writers.py
--rw-r--r--   0        0        0    10434 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/caster.py
--rw-r--r--   0        0        0     4413 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/pa_pd.py
--rw-r--r--   0        0        0     2839 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/reader.py
--rw-r--r--   0        0        0     3815 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/utils.py
--rw-r--r--   0        0        0     1580 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/writer.py
--rw-r--r--   0        0        0     1460 2023-06-13 12:04:04.640679 arrow_pd_parser-1.3.8/pyproject.toml
--rw-r--r--   0        0        0    12859 1970-01-01 00:00:00.000000 arrow_pd_parser-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0    12064 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/README.md
+-rw-r--r--   0        0        0       22 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/__init__.py
+-rw-r--r--   0        0        0    13642 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/_arrow_parsers.py
+-rw-r--r--   0        0        0     4059 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/_export.py
+-rw-r--r--   0        0        0    14789 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/_readers.py
+-rw-r--r--   0        0        0    14430 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/_writers.py
+-rw-r--r--   0        0        0    10434 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/caster.py
+-rw-r--r--   0        0        0     4413 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/pa_pd.py
+-rw-r--r--   0        0        0     2839 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/reader.py
+-rw-r--r--   0        0        0     3815 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/utils.py
+-rw-r--r--   0        0        0     1580 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/arrow_pd_parser/writer.py
+-rw-r--r--   0        0        0     1459 2023-07-25 14:13:22.479236 arrow_pd_parser-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0    12909 1970-01-01 00:00:00.000000 arrow_pd_parser-1.3.9/PKG-INFO
```

### Comparing `arrow_pd_parser-1.3.8/README.md` & `arrow_pd_parser-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/_arrow_parsers.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/_arrow_parsers.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/_export.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/_export.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/_readers.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/_readers.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/_writers.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/_writers.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/caster.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/caster.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/pa_pd.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/pa_pd.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/reader.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/reader.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/utils.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/utils.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/arrow_pd_parser/writer.py` & `arrow_pd_parser-1.3.9/arrow_pd_parser/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.8/pyproject.toml` & `arrow_pd_parser-1.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arrow_pd_parser"
-version = "1.3.8"
+version = "1.3.9"
 description = "MoJ arrow-pd-parser"
 authors = ["Karik Isichei <karik.isichei@digital.justice.gov.uk>",
            "Alec Johnson <alec.johnson@digital.justice.gov.uk>",
            "Kimberley Brett <kimberley.brett@digital.justice.gov.uk>",
            "Thomas Hirsch <thomas.hirsch@digital.justice.gov.uk>",
            "Jacob Browning <jacob.browning@digital.justice.gov.uk>",
            "Jacob Hamblin-Pyke <jacob.hamblin-pyke@digital.justice.gov.uk>",
@@ -16,15 +16,15 @@
            ]
 
 readme = "README.md"
 repository = "https://github.com/moj-analytical-services/mojap-arrow-pd-parser"
 homepage = "https://github.com/moj-analytical-services/mojap-arrow-pd-parser"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<4.0"
 pandas = ">=1.2"
 pyarrow = ">=6.0.0"
 mojap-metadata = {version = "^1.10.0", extras = ["arrow"]}
 awswrangler = ">=2.4.0"
 smart-open = "^5.2.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `arrow_pd_parser-1.3.8/PKG-INFO` & `arrow_pd_parser-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: arrow-pd-parser
-Version: 1.3.8
+Version: 1.3.9
 Summary: MoJ arrow-pd-parser
 Home-page: https://github.com/moj-analytical-services/mojap-arrow-pd-parser
 Author: Karik Isichei
 Author-email: karik.isichei@digital.justice.gov.uk
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: awswrangler (>=2.4.0)
 Requires-Dist: mojap-metadata[arrow] (>=1.10.0,<2.0.0)
 Requires-Dist: pandas (>=1.2)
 Requires-Dist: pyarrow (>=6.0.0)
 Requires-Dist: smart-open (>=5.2.1,<6.0.0)
 Project-URL: Repository, https://github.com/moj-analytical-services/mojap-arrow-pd-parser
 Description-Content-Type: text/markdown
```

