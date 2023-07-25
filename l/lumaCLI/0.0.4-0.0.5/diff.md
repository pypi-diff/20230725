# Comparing `tmp/lumacli-0.0.4.tar.gz` & `tmp/lumacli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumacli-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lumacli-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lumacli-0.0.4.tar` & `lumacli-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      821 2023-07-24 10:07:59.207682 lumacli-0.0.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     3166 2023-07-24 10:07:59.207682 lumacli-0.0.4/.gitignore
--rw-r--r--   0        0        0     1064 2023-07-24 10:07:59.207682 lumacli-0.0.4/LICENSE
--rw-r--r--   0        0        0     3390 2023-07-24 10:07:59.207682 lumacli-0.0.4/README.md
--rw-r--r--   0        0        0      502 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/__init__.py
--rw-r--r--   0        0        0     6528 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/dbt.py
--rw-r--r--   0        0        0      483 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/luma.py
--rw-r--r--   0        0        0     2401 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/postgres.py
--rw-r--r--   0        0        0        0 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/__init__.py
--rw-r--r--   0        0        0     3817 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/conftest.py
--rw-r--r--   0        0        0     8087 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/catalog.json
--rw-r--r--   0        0        0        0 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/file.txt
--rw-r--r--   0        0        0      260 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/invalid_json.json
--rw-r--r--   0        0        0   173474 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/manifest.json
--rw-r--r--   0        0        0     5109 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/postgres_dump_file.sql
--rw-r--r--   0        0        0    10271 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/run_results.json
--rw-r--r--   0        0        0     9716 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/metadata_dir/sources.json
--rw-r--r--   0        0        0       90 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/requirements.txt
--rw-r--r--   0        0        0      691 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/test_dbt.py
--rw-r--r--   0        0        0     3981 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/test_dbt_utils.py
--rw-r--r--   0        0        0      305 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/test_postgres.py
--rw-r--r--   0        0        0     3002 2023-07-24 10:07:59.207682 lumacli-0.0.4/lumaCLI/tests/test_postgres_utils.py
--rw-r--r--   0        0        0      394 2023-07-24 10:07:59.211682 lumacli-0.0.4/lumaCLI/tests/utils.py
--rw-r--r--   0        0        0      320 2023-07-24 10:07:59.211682 lumacli-0.0.4/lumaCLI/utils/__init__.py
--rw-r--r--   0        0        0     2287 2023-07-24 10:07:59.211682 lumacli-0.0.4/lumaCLI/utils/dbt_utils.py
--rw-r--r--   0        0        0     8456 2023-07-24 10:07:59.211682 lumacli-0.0.4/lumaCLI/utils/postgres_utils.py
--rw-r--r--   0        0        0     1371 2023-07-24 10:07:59.211682 lumacli-0.0.4/playground.py
--rw-r--r--   0        0        0     1065 2023-07-24 10:07:59.211682 lumacli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 lumacli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-07-25 12:47:16.023886 lumacli-0.0.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     3166 2023-07-25 12:47:16.023886 lumacli-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1064 2023-07-25 12:47:16.023886 lumacli-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3040 2023-07-25 12:47:16.023886 lumacli-0.0.5/README.md
+-rw-r--r--   0        0        0      502 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/__init__.py
+-rw-r--r--   0        0        0     6146 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/dbt.py
+-rw-r--r--   0        0        0      483 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/luma.py
+-rw-r--r--   0        0        0     2401 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/__init__.py
+-rw-r--r--   0        0        0     3817 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/conftest.py
+-rw-r--r--   0        0        0     8087 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/catalog.json
+-rw-r--r--   0        0        0        0 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/file.txt
+-rw-r--r--   0        0        0      260 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/invalid_json.json
+-rw-r--r--   0        0        0   173474 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/manifest.json
+-rw-r--r--   0        0        0     5109 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/postgres_dump_file.sql
+-rw-r--r--   0        0        0    10271 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/run_results.json
+-rw-r--r--   0        0        0     9716 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/sources.json
+-rw-r--r--   0        0        0       90 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/requirements.txt
+-rw-r--r--   0        0        0      691 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/test_dbt.py
+-rw-r--r--   0        0        0     3981 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/test_dbt_utils.py
+-rw-r--r--   0        0        0      305 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/test_postgres.py
+-rw-r--r--   0        0        0     3002 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/test_postgres_utils.py
+-rw-r--r--   0        0        0      394 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/utils.py
+-rw-r--r--   0        0        0      320 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/utils/__init__.py
+-rw-r--r--   0        0        0     2287 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/utils/dbt_utils.py
+-rw-r--r--   0        0        0     8456 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/utils/postgres_utils.py
+-rw-r--r--   0        0        0     1371 2023-07-25 12:47:16.023886 lumacli-0.0.5/playground.py
+-rw-r--r--   0        0        0     1064 2023-07-25 12:47:16.023886 lumacli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 lumacli-0.0.5/PKG-INFO
```

### Comparing `lumacli-0.0.4/.github/workflows/publish_to_pypi.yml` & `lumacli-0.0.5/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/.gitignore` & `lumacli-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/LICENSE` & `lumacli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/README.md` & `lumacli-0.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -38,22 +38,16 @@
 **Commands**:
 
 * `ingest`: Sends a bundle of JSON files...
 * `send-test-results`: Sends the run_results.json file located in...
 
 ### `lumaCLI dbt ingest`
 
-Sends a bundle of JSON files (manifest.json, catalog.json, sources.json, run_results.json) to a Luma endpoint. If 'metadata_dir' is not specified, the current working directory is used.
-
-Args:
-    metadata_dir (str, optional): Directory path containing all the metadata files. Defaults to current working directory if not provided.
-    endpoint (str): The endpoint URL for ingestion.
-
-Returns:
-    response: The HTTP response obtained from the endpoint.
+Sends a bundle of JSON files (manifest.json, catalog.json, sources.json, run_results.json) located in the specified directory to a Luma endpoint.
+If any of these files is not present in the directory, the command will fail. Uses the current working directory if 'metadata_dir' is not specified.
 
 **Usage**:
 
 ```console
 $ lumaCLI dbt ingest [OPTIONS] [METADATA_DIR]
 ```
 
@@ -64,22 +58,16 @@
 **Options**:
 
 * `-e, --endpoint TEXT`: URL of the ingestion endpoint.  [env var: LUMA_DBT_INGEST_ENDPOINT; required]
 * `--help`: Show this message and exit.
 
 ### `lumaCLI dbt send-test-results`
 
-Sends the run_results.json file located in the specified directory to a Luma endpoint. If 'metadata_dir' is not specified, the current working directory is used.
-
-Args:
-    metadata_dir (str, optional): Directory path containing the run_results.json file. Defaults to current working directory if not provided.
-    endpoint (str): The endpoint URL for ingestion.
-
-Returns:
-    response: The HTTP response obtained from the endpoint.
+Sends the run_results.json file located in the specified directory to a Luma endpoint.
+The command will fail if the run_results.json file is not present in the directory. Uses the current working directory if 'metadata_dir' is not specified.
 
 **Usage**:
 
 ```console
 $ lumaCLI dbt send-test-results [OPTIONS] [METADATA_DIR]
 ```
```

### Comparing `lumacli-0.0.4/lumaCLI/dbt.py` & `lumacli-0.0.5/lumaCLI/dbt.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,22 +42,16 @@
         "--endpoint",
         "-e",
         envvar="LUMA_DBT_INGEST_ENDPOINT",
         help="URL of the ingestion endpoint.",
     ),
 ):
     """
-    Sends a bundle of JSON files (manifest.json, catalog.json, sources.json, run_results.json) to a Luma endpoint. If 'metadata_dir' is not specified, the current working directory is used.
-
-    Args:
-        metadata_dir (str, optional): Directory path containing all the metadata files. Defaults to current working directory if not provided.
-        endpoint (str): The endpoint URL for ingestion.
-
-    Returns:
-        response: The HTTP response obtained from the endpoint.
+    Sends a bundle of JSON files (manifest.json, catalog.json, sources.json, run_results.json) located in the specified directory to a Luma endpoint.
+    If any of these files is not present in the directory, the command will fail. Uses the current working directory if 'metadata_dir' is not specified.
     """
 
     # Define JSON paths
 
     manifest_json_path = metadata_dir / "manifest.json"
     catalog_json_path = metadata_dir / "catalog.json"
     sources_json_path = metadata_dir / "sources.json"
@@ -138,22 +132,16 @@
         "--endpoint",
         "-e",
         envvar="LUMA_DBT_SEND-TEST-RESULTS_ENDPOINT",
         help="URL of the ingestion endpoint.",
     ),
 ):
     """
-    Sends the run_results.json file located in the specified directory to a Luma endpoint. If 'metadata_dir' is not specified, the current working directory is used.
-
-    Args:
-        metadata_dir (str, optional): Directory path containing the run_results.json file. Defaults to current working directory if not provided.
-        endpoint (str): The endpoint URL for ingestion.
-
-    Returns:
-        response: The HTTP response obtained from the endpoint.
+    Sends the run_results.json file located in the specified directory to a Luma endpoint.
+    The command will fail if the run_results.json file is not present in the directory. Uses the current working directory if 'metadata_dir' is not specified.
     """
     if metadata_dir is None:
         metadata_dir = os.getcwd()
         print(
             Panel(
                 f"[yellow]'metadata_dir' not specified, using current working directory {metadata_dir}[/yellow]"
             )
```

### Comparing `lumacli-0.0.4/lumaCLI/postgres.py` & `lumacli-0.0.5/lumaCLI/postgres.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/conftest.py` & `lumacli-0.0.5/lumaCLI/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/metadata_dir/catalog.json` & `lumacli-0.0.5/lumaCLI/tests/metadata_dir/catalog.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/metadata_dir/manifest.json` & `lumacli-0.0.5/lumaCLI/tests/metadata_dir/manifest.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/metadata_dir/postgres_dump_file.sql` & `lumacli-0.0.5/lumaCLI/tests/metadata_dir/postgres_dump_file.sql`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/metadata_dir/run_results.json` & `lumacli-0.0.5/lumaCLI/tests/metadata_dir/run_results.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/metadata_dir/sources.json` & `lumacli-0.0.5/lumaCLI/tests/metadata_dir/sources.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/test_dbt.py` & `lumacli-0.0.5/lumaCLI/tests/test_dbt.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/test_dbt_utils.py` & `lumacli-0.0.5/lumaCLI/tests/test_dbt_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/tests/test_postgres_utils.py` & `lumacli-0.0.5/lumaCLI/tests/test_postgres_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/utils/dbt_utils.py` & `lumacli-0.0.5/lumaCLI/utils/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/lumaCLI/utils/postgres_utils.py` & `lumacli-0.0.5/lumaCLI/utils/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/playground.py` & `lumacli-0.0.5/playground.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.4/pyproject.toml` & `lumacli-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "lumaCLI"
 description = "A CLI tool for managing the data catalog platform."
 readme = "README.md"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name="Facundo Goiriz", email="fgoiriz@dyvenia.com" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["cli", "dbt", "luma", "data", "catalog"]
-requires-python = ">=3.10, <4"
+requires-python = ">=3.8, <4"
 dependencies = [
     "typer[all]~=0.9.0",
     "psycopg2-binary~=2.9",
     "requests~=2.28.2",
 ]
 
 [project.optional-dependencies]
```

### Comparing `lumacli-0.0.4/PKG-INFO` & `lumacli-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lumaCLI
-Version: 0.0.4
+Version: 0.0.5
 Summary: A CLI tool for managing the data catalog platform.
 Keywords: cli,dbt,luma,data,catalog
 Author-email: Facundo Goiriz <fgoiriz@dyvenia.com>
-Requires-Python: >=3.10, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: typer[all]~=0.9.0
 Requires-Dist: psycopg2-binary~=2.9
@@ -59,22 +59,16 @@
 **Commands**:
 
 * `ingest`: Sends a bundle of JSON files...
 * `send-test-results`: Sends the run_results.json file located in...
 
 ### `lumaCLI dbt ingest`
 
-Sends a bundle of JSON files (manifest.json, catalog.json, sources.json, run_results.json) to a Luma endpoint. If 'metadata_dir' is not specified, the current working directory is used.
-
-Args:
-    metadata_dir (str, optional): Directory path containing all the metadata files. Defaults to current working directory if not provided.
-    endpoint (str): The endpoint URL for ingestion.
-
-Returns:
-    response: The HTTP response obtained from the endpoint.
+Sends a bundle of JSON files (manifest.json, catalog.json, sources.json, run_results.json) located in the specified directory to a Luma endpoint.
+If any of these files is not present in the directory, the command will fail. Uses the current working directory if 'metadata_dir' is not specified.
 
 **Usage**:
 
 ```console
 $ lumaCLI dbt ingest [OPTIONS] [METADATA_DIR]
 ```
 
@@ -85,22 +79,16 @@
 **Options**:
 
 * `-e, --endpoint TEXT`: URL of the ingestion endpoint.  [env var: LUMA_DBT_INGEST_ENDPOINT; required]
 * `--help`: Show this message and exit.
 
 ### `lumaCLI dbt send-test-results`
 
-Sends the run_results.json file located in the specified directory to a Luma endpoint. If 'metadata_dir' is not specified, the current working directory is used.
-
-Args:
-    metadata_dir (str, optional): Directory path containing the run_results.json file. Defaults to current working directory if not provided.
-    endpoint (str): The endpoint URL for ingestion.
-
-Returns:
-    response: The HTTP response obtained from the endpoint.
+Sends the run_results.json file located in the specified directory to a Luma endpoint.
+The command will fail if the run_results.json file is not present in the directory. Uses the current working directory if 'metadata_dir' is not specified.
 
 **Usage**:
 
 ```console
 $ lumaCLI dbt send-test-results [OPTIONS] [METADATA_DIR]
 ```
```

