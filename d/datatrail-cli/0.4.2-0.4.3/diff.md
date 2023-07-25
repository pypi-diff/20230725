# Comparing `tmp/datatrail_cli-0.4.2.tar.gz` & `tmp/datatrail_cli-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.4.2.tar", max compression
+gzip compressed data, was "datatrail_cli-0.4.3.tar", max compression
```

## Comparing `datatrail_cli-0.4.2.tar` & `datatrail_cli-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2023-06-14 14:18:45.516688 datatrail_cli-0.4.2/LICENSE
--rw-r--r--   0        0        0     3558 2023-06-14 14:18:45.516688 datatrail_cli-0.4.2/README.md
--rw-r--r--   0        0        0      214 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/__init__.py
--rw-r--r--   0        0        0     4399 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/clear.py
--rw-r--r--   0        0        0      929 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/cli.py
--rw-r--r--   0        0        0     3714 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/config.py
--rw-r--r--   0        0        0     1062 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/config.yaml
--rw-r--r--   0        0        0     3442 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/ls.py
--rw-r--r--   0        0        0     6108 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/ps.py
--rw-r--r--   0        0        0     4336 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/pull.py
--rw-r--r--   0        0        0    14068 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/src/functions.py
--rw-r--r--   0        0        0     9241 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     1493 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1048 2023-06-14 14:18:45.524688 datatrail_cli-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datatrail_cli-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-25 19:02:01.121542 datatrail_cli-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3558 2023-07-25 19:02:01.121542 datatrail_cli-0.4.3/README.md
+-rw-r--r--   0        0        0      214 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/__init__.py
+-rw-r--r--   0        0        0     4399 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/clear.py
+-rw-r--r--   0        0        0     1437 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/cli.py
+-rw-r--r--   0        0        0     3714 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/config.yaml
+-rw-r--r--   0        0        0     3433 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/ls.py
+-rw-r--r--   0        0        0     6108 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/ps.py
+-rw-r--r--   0        0        0     4528 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/pull.py
+-rw-r--r--   0        0        0    14626 2023-07-25 19:02:01.129542 datatrail_cli-0.4.3/dtcli/src/functions.py
+-rw-r--r--   0        0        0     9241 2023-07-25 19:02:01.133542 datatrail_cli-0.4.3/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     2755 2023-07-25 19:02:01.133542 datatrail_cli-0.4.3/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1048 2023-07-25 19:02:01.133542 datatrail_cli-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datatrail_cli-0.4.3/PKG-INFO
```

### Comparing `datatrail_cli-0.4.2/LICENSE` & `datatrail_cli-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.4.2/README.md` & `datatrail_cli-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.4.2/dtcli/clear.py` & `datatrail_cli-0.4.3/dtcli/clear.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.4.2/dtcli/cli.py` & `datatrail_cli-0.4.3/dtcli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 import click
 from click_aliasing import ClickAliasedGroup
 from pkg_resources import get_distribution
 from rich import console, pretty
 
 from dtcli import clear, config, ls, ps, pull
+from dtcli.utilities import utilities
 
 pretty.install()
 terminal = console.Console()
 
 
 # Main CLI
 @click.group(cls=ClickAliasedGroup)
 def cli():
     """Datatrail Command Line Interface."""
-    pass
+    check_version()
 
 
 @cli.command(name="version", help="Show versions.")
 def version():
     """Show version."""
     terminal.print(
         "Datatrail Versions",
@@ -37,9 +38,22 @@
 
 cli.add_command(ls.list, aliases=["ls"])
 cli.add_command(ps.ps)
 cli.add_command(pull.pull)
 cli.add_command(clear.clear)
 cli.add_command(config.config)
 
+
+def check_version() -> None:
+    """Check if CLI is latest release."""
+    if not utilities.cli_is_latest_release():
+        current_version = get_distribution("datatrail-cli").version
+        latest_version = utilities.get_latest_released_version()
+        terminal.print(
+            f"A new release of datatrail-cli is available: {current_version} → {latest_version}",  # noqa: E501
+            style="bold yellow",
+        )
+        terminal.print()
+
+
 if __name__ == "__main__":
     cli()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `datatrail_cli-0.4.2/dtcli/config.py` & `datatrail_cli-0.4.3/dtcli/config.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.4.2/dtcli/config.yaml` & `datatrail_cli-0.4.3/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.4.2/dtcli/ls.py` & `datatrail_cli-0.4.3/dtcli/ls.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         table.add_column("Larger datasets", justify="center")
         table.add_row("\t".join(results["larger_datasets"]))
         with console.pager(styles=False):
             console.print(table)
 
     # Display datasets in parent dataset for scope.
     if "datasets" in results.keys():
-        results["datasets"] = sorted(results["datasets"], key=int, reverse=True)
+        results["datasets"] = sorted(results["datasets"], reverse=True)
         if write:
             with open(f"./dataset_list_for_{scope}_{datasets}.txt", "w") as file:
                 json.dump(results, file)
 
         table = Table(
             title=f"Datatrail: Child Datasets {datasets} {scope}",
             header_style="magenta",
```

### Comparing `datatrail_cli-0.4.2/dtcli/ps.py` & `datatrail_cli-0.4.3/dtcli/ps.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.4.2/dtcli/pull.py` & `datatrail_cli-0.4.3/dtcli/pull.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,30 +91,32 @@
         raise click.Abort()
 
     if not validate_scope(scope):
         raise ValueError("Scope does not exist.")
 
     # Find files missing from localhost.
     console.print(f"\nSearching for files for {dataset} {scope}...\n")
-    files = find_missing_dataset_files(scope, dataset)
-    if len(files["missing"]) == 0:
+    files = find_missing_dataset_files(scope, dataset, directory, verbose)
+    if len(files["missing"]) == 0 and len(files["existing"]) == 0:
         console.print("No files found at minoc.", style="bold red")
         return None
     files_paths = [f.replace("cadc:CHIMEFRB", "") for f in files["missing"]]
-    common_path = path.commonpath(["/" + f for f in files_paths])
-    try:
-        to_download_size = size(common_path)
-    except SSLError:
-        error_console.print(
-            """
+    to_download_size = 0.0
+    if len(files_paths) > 0:
+        common_path = path.commonpath(["/" + f for f in files_paths])
+        try:
+            to_download_size = size(common_path)
+        except SSLError:
+            error_console.print(
+                """
 No valid CADC certificate found.
 Create one using 'cadc-get-cert -u <USERNAME>'.
 """
-        )
-        return None
+            )
+            return None
     console.print(
         f" - {len(files['existing'])} files found at {site}.",
         style="green",
     )
     console.print(
         f" - {len(files['missing'])} files can be downloaded from minoc.",
         style="yellow",
@@ -123,14 +125,16 @@
         f"     - Size to download: {to_download_size:.2f} GB.\n",
         style="yellow",
     )
 
     # Confirm download.
     if force:
         is_download = True
+    elif to_download_size == 0:
+        return None
     else:
         is_download = Confirm.ask(
             f"Download {len(files['missing'])} files?",
         )
 
     # Download missing files.
     if is_download:
```

### Comparing `datatrail_cli-0.4.2/dtcli/src/functions.py` & `datatrail_cli-0.4.3/dtcli/src/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,56 +212,66 @@
             return {"error": f"Could not find {dataset} {scope} in Datatrail."}
         return response  # type: ignore
     except requests.exceptions.ConnectionError as e:
         logger.error(e)
         return {"error": "Datatrail Server at CHIME is not responding."}
 
 
-def find_missing_dataset_files(scope: str, dataset: str) -> Dict:
+def find_missing_dataset_files(
+    scope: str, dataset: str, root_path: Optional[str] = None, verbose: int = 0
+) -> Dict:
     """List missing files for a dataset.
 
     Args:
         scope (str): Scope of dataset. Defaults to None.
         dataset (str): Name of dataset. Defaults to None.
+        root_path (Optional[str]): Path to download files to. Defaults to None.
+        verbose (int): Verbosity. Defaults to 0.
 
     Returns:
         Dict: Dictionary of results.
     """
-    # Load configuration.
-    config = procure()
-    SITE = config["site"]
+    # Set logging level.
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
     # find dataset
-    dataset_locations = get_dataset_file_info(scope, dataset)
+    dataset_locations = get_dataset_file_info(scope, dataset, verbose=verbose)
     if isinstance(dataset_locations, str):
         print(f"Could not find the dataset: {scope}, {dataset}")
         return {}
 
-    # stage dataset
-    site_locations = ["chime", "allenby", "gbo", "hatcreek", "canfar"]
-
     # check for local copy of the data.
-    if SITE in site_locations and dataset_locations["file_replica_locations"].get(SITE):
-        file_uris = dataset_locations["file_replica_locations"][SITE]
-        print(f"Files found at {SITE}")
+    logger.info("Checking for local copies of files.")
+    if dataset_locations["file_replica_locations"].get("minoc"):
+        file_uris = dataset_locations["file_replica_locations"]["minoc"]
+        file_paths = []
+        # Clean up file paths
+        for f in file_uris:
+            if f.startswith("data/"):
+                file_paths.append(f)
+            elif f.startswith("cadc:CHIMEFRB/"):
+                file_paths.append(f.replace("//", "/").replace("cadc:CHIMEFRB/", ""))
+            elif f.startswith("/"):
+                file_paths.append(f.replace("//", "/")[1:])
         # check for missing files
         missing_files = []
         existing_files = []
-        for f in file_uris:
-            if Path(f).exists():
+        for f in file_paths:
+            if Path(root_path + f).exists():
+                logger.debug(f"- {f} : ✔")
                 existing_files.append(f)
             else:
+                logger.debug(f"- {f} : ✘")
                 missing_files.append(f)
 
-    # For local, assume no files exist.
     else:
-        file_replicas = dataset_locations.get("file_replica_locations")
-        if file_replicas:
-            missing_files = file_replicas.get("minoc")
-        else:
-            missing_files = []
+        missing_files = []
         existing_files = []
     return {"missing": missing_files, "existing": existing_files}
 
 
 def get_files(
     files: List[str],
     site: str,
@@ -293,15 +303,17 @@
     # download missing files.
     if len(files) > 0:
         print(f"{len(files)} files missing.")
         print(f"Downloading {len(files)} missing files.")
         files = [f.replace("cadc:CHIMEFRB/", "") for f in files]
         if not directory:
             directory = mounts[site]
-        destinations = [directory + "/" + f for f in files]
+        if not directory.endswith("/"):
+            directory += "/"
+        destinations = [(directory + f).replace("//", "/") for f in files]
         # make directory structure if it does not exist.
         folders = {os.path.dirname(path) for path in destinations}
         for folder in folders:
             os.makedirs(folder, exist_ok=True)
         cadcclient.pget(
             source=files, destination=destinations, processors=cores, verbose=verbose
         )
```

### Comparing `datatrail_cli-0.4.2/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.4.3/dtcli/utilities/cadcclient.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.4.2/pyproject.toml` & `datatrail_cli-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.4.2"
+version = "0.4.3"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.4.2/PKG-INFO` & `datatrail_cli-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.4.2
+Version: 0.4.3
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.4.2 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.4.3 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: cadcdata (>=2.4,<3.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```

