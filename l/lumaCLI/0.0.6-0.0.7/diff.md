# Comparing `tmp/lumacli-0.0.6.tar.gz` & `tmp/lumacli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumacli-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lumacli-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lumacli-0.0.6.tar` & `lumacli-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      821 2023-07-25 13:44:33.261588 lumacli-0.0.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     3166 2023-07-25 13:44:33.261588 lumacli-0.0.6/.gitignore
--rw-r--r--   0        0        0     1064 2023-07-25 13:44:33.261588 lumacli-0.0.6/LICENSE
--rw-r--r--   0        0        0     3040 2023-07-25 13:44:33.261588 lumacli-0.0.6/README.md
--rw-r--r--   0        0        0      502 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/__init__.py
--rw-r--r--   0        0        0     6146 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/dbt.py
--rw-r--r--   0        0        0      483 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/luma.py
--rw-r--r--   0        0        0     2401 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/postgres.py
--rw-r--r--   0        0        0        0 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/__init__.py
--rw-r--r--   0        0        0     3817 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/conftest.py
--rw-r--r--   0        0        0     8087 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/catalog.json
--rw-r--r--   0        0        0        0 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/file.txt
--rw-r--r--   0        0        0      260 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/invalid_json.json
--rw-r--r--   0        0        0   173474 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/manifest.json
--rw-r--r--   0        0        0     5109 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/postgres_dump_file.sql
--rw-r--r--   0        0        0    10271 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/run_results.json
--rw-r--r--   0        0        0     9716 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/metadata_dir/sources.json
--rw-r--r--   0        0        0       90 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/requirements.txt
--rw-r--r--   0        0        0      691 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/test_dbt.py
--rw-r--r--   0        0        0     3981 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/test_dbt_utils.py
--rw-r--r--   0        0        0      305 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/test_postgres.py
--rw-r--r--   0        0        0     3002 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/test_postgres_utils.py
--rw-r--r--   0        0        0      394 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/tests/utils.py
--rw-r--r--   0        0        0      320 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/utils/__init__.py
--rw-r--r--   0        0        0     2287 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/utils/dbt_utils.py
--rw-r--r--   0        0        0     8456 2023-07-25 13:44:33.261588 lumacli-0.0.6/lumaCLI/utils/postgres_utils.py
--rw-r--r--   0        0        0     1371 2023-07-25 13:44:33.261588 lumacli-0.0.6/playground.py
--rw-r--r--   0        0        0     1072 2023-07-25 13:44:33.265588 lumacli-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 lumacli-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-07-25 16:05:58.854011 lumacli-0.0.7/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     3166 2023-07-25 16:05:58.854011 lumacli-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1064 2023-07-25 16:05:58.854011 lumacli-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3040 2023-07-25 16:05:58.854011 lumacli-0.0.7/README.md
+-rw-r--r--   0        0        0      502 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/__init__.py
+-rw-r--r--   0        0        0     6146 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/dbt.py
+-rw-r--r--   0        0        0      483 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/luma.py
+-rw-r--r--   0        0        0     2818 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/__init__.py
+-rw-r--r--   0        0        0     3817 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/conftest.py
+-rw-r--r--   0        0        0     8087 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/metadata_dir/catalog.json
+-rw-r--r--   0        0        0        0 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/metadata_dir/file.txt
+-rw-r--r--   0        0        0      260 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/metadata_dir/invalid_json.json
+-rw-r--r--   0        0        0   173474 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/metadata_dir/manifest.json
+-rw-r--r--   0        0        0     5109 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/metadata_dir/postgres_dump_file.sql
+-rw-r--r--   0        0        0    10271 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/metadata_dir/run_results.json
+-rw-r--r--   0        0        0     9716 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/metadata_dir/sources.json
+-rw-r--r--   0        0        0       90 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/requirements.txt
+-rw-r--r--   0        0        0      691 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/test_dbt.py
+-rw-r--r--   0        0        0     3981 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/test_dbt_utils.py
+-rw-r--r--   0        0        0      305 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/test_postgres.py
+-rw-r--r--   0        0        0     3002 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/test_postgres_utils.py
+-rw-r--r--   0        0        0      394 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/tests/utils.py
+-rw-r--r--   0        0        0      320 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/utils/__init__.py
+-rw-r--r--   0        0        0     2287 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/utils/dbt_utils.py
+-rw-r--r--   0        0        0     9000 2023-07-25 16:05:58.854011 lumacli-0.0.7/lumaCLI/utils/postgres_utils.py
+-rw-r--r--   0        0        0     1371 2023-07-25 16:05:58.854011 lumacli-0.0.7/playground.py
+-rw-r--r--   0        0        0     1072 2023-07-25 16:05:58.854011 lumacli-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 lumacli-0.0.7/PKG-INFO
```

### Comparing `lumacli-0.0.6/.github/workflows/publish_to_pypi.yml` & `lumacli-0.0.7/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/.gitignore` & `lumacli-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/LICENSE` & `lumacli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/README.md` & `lumacli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/dbt.py` & `lumacli-0.0.7/lumaCLI/dbt.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/postgres.py` & `lumacli-0.0.7/lumaCLI/postgres.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,31 @@
     get_db_metadata,
 )
 
 
 app = typer.Typer(no_args_is_help=True, pretty_exceptions_show_locals=False)
 
 
+def ask_for_endpoint_if_not_dry_run(endpoint, ctx: typer.Context):
+    if ctx.resilient_parsing:
+        return
+    dry_run = ctx.params.get("dry_run", False)
+
+    if endpoint or dry_run:
+        return endpoint
+
+    # Raise a typer.BadParameter exception to simulate the same error as missing 'endpoint'
+    raise typer.BadParameter("Missing argument 'ENDPOINT'")
+
+
 @app.command()
 def ingest(
     endpoint: str = typer.Argument(
-        ...,
+        None,
+        callback=ask_for_endpoint_if_not_dry_run,
         envvar="LUMA_POSTGRES_INGEST_ENDPOINT",
         help="URL of the Luma Postgres ingestion endpoint.",
     ),
     username: str = typer.Option(
         ...,
         "--username",
         "-u",
@@ -63,15 +76,14 @@
         "-D",
         help="Whether to do a dry run. Print but not send the payload",
     ),
 ):
     """
     Creates dictionary with Postgres Metadata Information and sends it to the Luma Postgres ingest endpoint.
     """
-
     db_metadata: dict[str, list[dict]] = get_db_metadata(
         username=username, database=database, host=host, port=port, password=password
     )
 
     if dry_run:
         print(db_metadata)
         return db_metadata
```

### Comparing `lumacli-0.0.6/lumaCLI/tests/conftest.py` & `lumacli-0.0.7/lumaCLI/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/tests/metadata_dir/catalog.json` & `lumacli-0.0.7/lumaCLI/tests/metadata_dir/catalog.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/tests/metadata_dir/manifest.json` & `lumacli-0.0.7/lumaCLI/tests/metadata_dir/manifest.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/tests/metadata_dir/postgres_dump_file.sql` & `lumacli-0.0.7/lumaCLI/tests/metadata_dir/postgres_dump_file.sql`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/tests/metadata_dir/run_results.json` & `lumacli-0.0.7/lumaCLI/tests/metadata_dir/run_results.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/tests/metadata_dir/sources.json` & `lumacli-0.0.7/lumaCLI/tests/metadata_dir/sources.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/tests/test_dbt.py` & `lumacli-0.0.7/lumaCLI/tests/test_dbt.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/tests/test_dbt_utils.py` & `lumacli-0.0.7/lumaCLI/tests/test_dbt_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/tests/test_postgres_utils.py` & `lumacli-0.0.7/lumaCLI/tests/test_postgres_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/utils/dbt_utils.py` & `lumacli-0.0.7/lumaCLI/utils/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/lumaCLI/utils/postgres_utils.py` & `lumacli-0.0.7/lumaCLI/utils/postgres_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 import subprocess
 import typer
+from typing import Optional
 import re
 import psycopg2
 import os
+from rich.console import Console
+from rich.panel import Panel
 
+console = Console()
 
-def run_command(command: str, capture_output: bool = False) -> None | str:
+
+def run_command(command: str, capture_output: bool = False) -> Optional[str]:
     """
     Run a shell command and optionally capture its output.
     """
     try:
         if capture_output:
             result = subprocess.run(
                 command, shell=True, check=True, capture_output=True, text=True
             )
             return result.stdout.strip()
         else:
             subprocess.run(command, shell=True, check=True)
             return None
     except subprocess.CalledProcessError as e:
-        typer.echo(f"An error occurred while running the command: {e}")
-        raise typer.Exit(1)
+        console.print(
+            Panel.fit(
+                "[bold red]ERROR[/bold red]: An error occurred while running the command: [bold yellow]{}[/bold yellow]".format(
+                    e
+                ),
+                title="Error",
+                border_style="red",
+            )
+        )
+        if e.output:
+            console.print("[bold cyan]Output[/bold cyan]: {}".format(e.output))
+        if e.stderr:
+            console.print("[bold red]Error[/bold red]: {}".format(e.stderr))
+    raise typer.Exit(1)
 
 
 def create_conn(username, password, host, port, database):
     return psycopg2.connect(
         user=username, password=password, host=host, port=port, dbname=database
     )
```

### Comparing `lumacli-0.0.6/playground.py` & `lumacli-0.0.7/playground.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.6/pyproject.toml` & `lumacli-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "lumaCLI"
 description = "A CLI tool for managing the data catalog platform."
 readme = "README.md"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name="Facundo Goiriz", email="fgoiriz@dyvenia.com" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `lumacli-0.0.6/PKG-INFO` & `lumacli-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumaCLI
-Version: 0.0.6
+Version: 0.0.7
 Summary: A CLI tool for managing the data catalog platform.
 Keywords: cli,dbt,luma,data,catalog
 Author-email: Facundo Goiriz <fgoiriz@dyvenia.com>
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

