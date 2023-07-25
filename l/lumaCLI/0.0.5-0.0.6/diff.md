# Comparing `tmp/lumacli-0.0.5.tar.gz` & `tmp/lumacli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumacli-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lumacli-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lumacli-0.0.5.tar` & `lumacli-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      821 2023-07-25 12:47:16.023886 lumacli-0.0.5/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     3166 2023-07-25 12:47:16.023886 lumacli-0.0.5/.gitignore
--rw-r--r--   0        0        0     1064 2023-07-25 12:47:16.023886 lumacli-0.0.5/LICENSE
--rw-r--r--   0        0        0     3040 2023-07-25 12:47:16.023886 lumacli-0.0.5/README.md
--rw-r--r--   0        0        0      502 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/__init__.py
--rw-r--r--   0        0        0     6146 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/dbt.py
--rw-r--r--   0        0        0      483 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/luma.py
--rw-r--r--   0        0        0     2401 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/postgres.py
--rw-r--r--   0        0        0        0 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/__init__.py
--rw-r--r--   0        0        0     3817 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/conftest.py
--rw-r--r--   0        0        0     8087 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/catalog.json
--rw-r--r--   0        0        0        0 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/file.txt
--rw-r--r--   0        0        0      260 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/invalid_json.json
--rw-r--r--   0        0        0   173474 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/manifest.json
--rw-r--r--   0        0        0     5109 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/postgres_dump_file.sql
--rw-r--r--   0        0        0    10271 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/run_results.json
--rw-r--r--   0        0        0     9716 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/metadata_dir/sources.json
--rw-r--r--   0        0        0       90 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/requirements.txt
--rw-r--r--   0        0        0      691 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/test_dbt.py
--rw-r--r--   0        0        0     3981 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/test_dbt_utils.py
--rw-r--r--   0        0        0      305 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/test_postgres.py
--rw-r--r--   0        0        0     3002 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/test_postgres_utils.py
--rw-r--r--   0        0        0      394 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/tests/utils.py
--rw-r--r--   0        0        0      320 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/utils/__init__.py
--rw-r--r--   0        0        0     2287 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/utils/dbt_utils.py
--rw-r--r--   0        0        0     8456 2023-07-25 12:47:16.023886 lumacli-0.0.5/lumaCLI/utils/postgres_utils.py
--rw-r--r--   0        0        0     1371 2023-07-25 12:47:16.023886 lumacli-0.0.5/playground.py
--rw-r--r--   0        0        0     1064 2023-07-25 12:47:16.023886 lumacli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 lumacli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-07-25 13:44:33.261588 lumacli-0.0.6/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     3166 2023-07-25 13:44:33.261588 lumacli-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1064 2023-07-25 13:44:33.261588 lumacli-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3040 2023-07-25 13:44:33.261588 lumacli-0.0.6/README.md
+-rw-r--r--   0        0        0      502 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/__init__.py
+-rw-r--r--   0        0        0     6146 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/dbt.py
+-rw-r--r--   0        0        0      483 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/luma.py
+-rw-r--r--   0        0        0     2401 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/__init__.py
+-rw-r--r--   0        0        0     3817 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/conftest.py
+-rw-r--r--   0        0        0     8087 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/catalog.json
+-rw-r--r--   0        0        0        0 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/file.txt
+-rw-r--r--   0        0        0      260 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/invalid_json.json
+-rw-r--r--   0        0        0   173474 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/manifest.json
+-rw-r--r--   0        0        0     5109 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/postgres_dump_file.sql
+-rw-r--r--   0        0        0    10271 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/run_results.json
+-rw-r--r--   0        0        0     9716 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/sources.json
+-rw-r--r--   0        0        0       90 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/requirements.txt
+-rw-r--r--   0        0        0      691 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/test_dbt.py
+-rw-r--r--   0        0        0     3981 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/test_dbt_utils.py
+-rw-r--r--   0        0        0      305 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/test_postgres.py
+-rw-r--r--   0        0        0     3002 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/test_postgres_utils.py
+-rw-r--r--   0        0        0      394 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/utils.py
+-rw-r--r--   0        0        0      320 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/utils/__init__.py
+-rw-r--r--   0        0        0     2287 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/utils/dbt_utils.py
+-rw-r--r--   0        0        0     8456 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/utils/postgres_utils.py
+-rw-r--r--   0        0        0     1371 2023-07-25 13:44:33.261588 lumacli-0.0.6/playground.py
+-rw-r--r--   0        0        0     1072 2023-07-25 13:44:33.265588 lumacli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 lumacli-0.0.6/PKG-INFO
```

### Comparing `lumacli-0.0.5/.github/workflows/publish_to_pypi.yml` & `lumacli-0.0.6/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/.gitignore` & `lumacli-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/LICENSE` & `lumacli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/README.md` & `lumacli-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/dbt.py` & `lumacli-0.0.6/lumaCLI/dbt.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/postgres.py` & `lumacli-0.0.6/lumaCLI/postgres.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/conftest.py` & `lumacli-0.0.6/lumaCLI/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/metadata_dir/catalog.json` & `lumacli-0.0.6/lumaCLI/tests/metadata_dir/catalog.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/metadata_dir/manifest.json` & `lumacli-0.0.6/lumaCLI/tests/metadata_dir/manifest.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/metadata_dir/postgres_dump_file.sql` & `lumacli-0.0.6/lumaCLI/tests/metadata_dir/postgres_dump_file.sql`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/metadata_dir/run_results.json` & `lumacli-0.0.6/lumaCLI/tests/metadata_dir/run_results.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/metadata_dir/sources.json` & `lumacli-0.0.6/lumaCLI/tests/metadata_dir/sources.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/test_dbt.py` & `lumacli-0.0.6/lumaCLI/tests/test_dbt.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/test_dbt_utils.py` & `lumacli-0.0.6/lumaCLI/tests/test_dbt_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/tests/test_postgres_utils.py` & `lumacli-0.0.6/lumaCLI/tests/test_postgres_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/utils/dbt_utils.py` & `lumacli-0.0.6/lumaCLI/utils/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/lumaCLI/utils/postgres_utils.py` & `lumacli-0.0.6/lumaCLI/utils/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/playground.py` & `lumacli-0.0.6/playground.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.5/pyproject.toml` & `lumacli-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "lumaCLI"
 description = "A CLI tool for managing the data catalog platform."
 readme = "README.md"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name="Facundo Goiriz", email="fgoiriz@dyvenia.com" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["cli", "dbt", "luma", "data", "catalog"]
 requires-python = ">=3.8, <4"
 dependencies = [
     "typer[all]~=0.9.0",
     "psycopg2-binary~=2.9",
-    "requests~=2.28.2",
+    "requests>=2.20.0, <3.0.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.1,<8.0",
     "pytest-cov>=3.0,<4",
     "coverage>=6.4,<7",
```

### Comparing `lumacli-0.0.5/PKG-INFO` & `lumacli-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lumaCLI
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CLI tool for managing the data catalog platform.
 Keywords: cli,dbt,luma,data,catalog
 Author-email: Facundo Goiriz <fgoiriz@dyvenia.com>
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: typer[all]~=0.9.0
 Requires-Dist: psycopg2-binary~=2.9
-Requires-Dist: requests~=2.28.2
+Requires-Dist: requests>=2.20.0, <3.0.0
 Requires-Dist: pytest>=7.1,<8.0 ; extra == "test"
 Requires-Dist: pytest-cov>=3.0,<4 ; extra == "test"
 Requires-Dist: coverage>=6.4,<7 ; extra == "test"
 Requires-Dist: black>=22.6,<23 ; extra == "test"
 Provides-Extra: test
 
 **Installation 📦**
```

