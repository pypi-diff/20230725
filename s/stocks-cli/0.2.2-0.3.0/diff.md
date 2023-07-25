# Comparing `tmp/stocks-cli-0.2.2.tar.gz` & `tmp/stocks-cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocks-cli-0.2.2.tar", last modified: Wed Jul  5 12:47:54 2023, max compression
+gzip compressed data, was "stocks-cli-0.3.0.tar", last modified: Tue Jul 25 14:11:56 2023, max compression
```

## Comparing `stocks-cli-0.2.2.tar` & `stocks-cli-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.175620 stocks-cli-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-05 12:47:54.175620 stocks-cli-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4988 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.173620 stocks-cli-0.2.2/cli/
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     8914 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    60865 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/export.py
--rw-rw-rw-   0 root         (0) root         (0)     8634 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/export_eln_website_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    64937 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/export_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12896 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/fetch.py
--rw-rw-rw-   0 root         (0) root         (0)    37169 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/register.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/stockscli.ini
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 12:47:54.175620 stocks-cli-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.174620 stocks-cli-0.2.2/stocks/
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.174620 stocks-cli-0.2.2/stocks/assaysniffer/
--rw-rw-rw-   0 root         (0) root         (0)     3787 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/assaysniffer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3639 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/assaysniffer/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    39729 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/assaysniffer/sniffers.py
--rw-rw-rw-   0 root         (0) root         (0)    30404 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocks/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.174620 stocks-cli-0.2.2/stocks_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      647 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 12:47:54.000000 stocks-cli-0.2.2/stocks_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:47:54.175620 stocks-cli-0.2.2/stocksapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10815 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2607 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    74940 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    27299 2023-07-05 12:47:45.000000 stocks-cli-0.2.2/stocksapi/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.714431 stocks-cli-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-25 14:11:56.714431 stocks-cli-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4988 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.712431 stocks-cli-0.3.0/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8914 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    60509 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     8634 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/export_eln_website_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    64936 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/export_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12896 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)    37310 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/register.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/stockscli.ini
+-rw-rw-rw-   0 root         (0) root         (0)     7311 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4729 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/pypi_description.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 14:11:56.714431 stocks-cli-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.712431 stocks-cli-0.3.0/stocks/
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.713431 stocks-cli-0.3.0/stocks/assaysniffer/
+-rw-rw-rw-   0 root         (0) root         (0)     4129 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/assaysniffer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3624 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/assaysniffer/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    40236 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/assaysniffer/sniffers.py
+-rw-rw-rw-   0 root         (0) root         (0)    30518 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.713431 stocks-cli-0.3.0/stocks_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.714431 stocks-cli-0.3.0/stocksapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10865 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    81438 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    28467 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/models.py
```

### Comparing `stocks-cli-0.2.2/LICENSE.txt` & `stocks-cli-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.2/PKG-INFO` & `stocks-cli-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocks-cli
-Version: 0.2.2
+Version: 0.3.0
 Summary: Command Line Interface to the STOCKS server
 Home-page: https://www.embl.org/research/units/genome-biology/genome-biology-computational-support/
 Author: GBCS
 Author-email: gbcs@embl.de
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `stocks-cli-0.2.2/README.md` & `stocks-cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.2/cli/__init__.py` & `stocks-cli-0.3.0/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.2/cli/__main__.py` & `stocks-cli-0.3.0/cli/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from enum import Enum
 from typing import Optional
 import typer
-from cli import config, export, fetch, register, __app_name__, __version__
+from cli import config, export, fetch, register, validate, __app_name__, __version__
+
 
 class LogLevel(str, Enum):
     DEBUG = "DEBUG"
     INFO = "INFO"
     WARNING = "WARNING"
     ERROR = "ERROR"
     CRITICAL = "CRITICAL"
@@ -15,14 +16,15 @@
 # The main app
 app = typer.Typer()
 # app the different module, each one file in the cli package
 app.add_typer(config.app, name="config")
 app.add_typer(export.app, name="export")
 app.add_typer(fetch.app, name="fetch")
 app.add_typer(register.app, name="register")
+app.add_typer(validate.app, name="validate")
 
 
 # a method to print version and exit directly
 def _version_callback(value: bool) -> None:
     if value:
         typer.echo(f"{__app_name__} v{__version__}")
         raise typer.Exit()
@@ -38,29 +40,33 @@
             help="Show the application's version and exit.",
             callback=_version_callback,
             is_eager=True,
         )
 ) -> None:
     return
 
+
 @app.callback()
 def add_verbose_callback(
         log_level: LogLevel = typer.Option(
             "WARNING",
             "--log-level",
             case_sensitive=False,
             help="Sets the verbose level")
 ) -> None:
     logging.basicConfig(
         level=str(log_level.value),
-        #format='%(levelname)-8s  %(name)-23s  %(message)s'
         format='[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s',
         datefmt='%H:%M:%S'
     )
 
 
 def main():
-    app(prog_name=__app_name__)
+    try:
+        app(prog_name=__app_name__)
+    except Exception as err:
+        logging.exception("An unexpected error occurred during execution")
+        exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `stocks-cli-0.2.2/cli/config.py` & `stocks-cli-0.3.0/cli/config.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.2/cli/export.py` & `stocks-cli-0.3.0/cli/export.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,29 @@
 import getpass
 import re
 
 import typer
 
 from cli.export_eln_website_utils import get_experiment_export_dirname, build_static_web_site_for_eln_export
 from cli import get_default_config_file_path
-from stocks.models import Study, Assay, Protocol, SequencingAssay, Experiment, Project, DatasetFileCopy, \
-    AnnotationType, UserGroup
+from stocks.models import Study, Protocol, SequencingAssay, Experiment, Project, DatasetFileCopy, AnnotationType
 from stocksapi.client import StocksClient
 from stocksapi.manager import StocksManager
 from stocksapi.models import *
 from cli.export_utils import COMMENT_STOCKS_UUID, MAGETAB_RELEASE_DATE, \
     StudyExportFormat, add_default_submitter, add_owner_role, extract_protocol_list, extract_final_annotations, \
     write_df_in, create_annofactor_df, create_protocol_ref, create_idf_design, create_idf_experimental_factors, \
     create_idf_users, create_idf_protocol, add_user_institutions, owner_name, runtype_layout_map, \
     check_table_bools, stocks_annotare_library_contruction_map, single_cell_annotare_fillin, \
     MAGETAB_HEADER_SINGLE_CELL_ANNOTARE, merge_df_columns, to_ena_format, get_export_table, process_assays, \
     create_fake_data, ENA_TABLES_NAME, upload_ena_annotation, ena_credentials_file, parse_receipt, _ena_upload_cli, \
-    ANNOTATION_STOCKS_ENA_STUDY, TODO, TERM_SOURCE_REF, QUALITY_SCORING_SYSTEM, LIBRARY_ENCODING, ASCII_OFFSET, \
+    TODO, TERM_SOURCE_REF, QUALITY_SCORING_SYSTEM, LIBRARY_ENCODING, ASCII_OFFSET, \
     StudyValidationReport, write_report_file, Report, parse_html
 from cli.config import get_config
-from cli.utils import ModelType, HTMLFilter
+from cli.utils import ModelType
 
 logger = logging.getLogger(__name__)
 
 # name of this module (as appearing on the command line) is the last part of the __name__ eg cli.config -> config
 _MODULE_NAME = __name__.rsplit(".", 1)[-1]
 # list of command names offered in this module
 _CMD_EXPORT_ELN = "eln"
@@ -315,15 +314,15 @@
         export_dir: str = typer.Option(
             ...,
             "--odir",
             "-o",
             help="Path to where the study should be exported"
         ),
         filename: str = typer.Option(
-            "magetab.csv",
+            "magetab.txt",
             "--filename",
             "-f",
             help=f"The export filename (will be created in --odir). Only relevant when format is "
                  f"{StudyExportFormat.magetab}"
         ),
         stocks_comments: bool = typer.Option(
             True,
@@ -404,19 +403,20 @@
         raise typer.BadParameter(f"Failed to create dir_path at: {export_dir}")
     # Checks writing rights
     if not os.access(export_dir, os.W_OK):
         raise typer.BadParameter(f"You do not have writing rights at: {export_dir}")
 
     # Initiate/check folders and files
     # filename is required for some export format
+    outpath: Optional[Path] = None
     if format == StudyExportFormat.magetab or format == StudyExportFormat.tabular:
         if filename == "" or filename is None:
             raise typer.BadParameter(f"A filename is expected when export format is: {format}")
         # check file does not already exist
-        outpath: Path = Path(export_dir, filename)
+        outpath = Path(export_dir, filename)
         if outpath.exists():
             raise typer.BadParameter(f"File already exists, please remove: {str(outpath)}")
     elif format == StudyExportFormat.enatables:
         export_dir = os.path.abspath(export_dir) + '/'  # subprocess.call() doesnt handle relative paths
         ena_file_outpath = [f"{export_dir}ena_{t}_{study_id}.tsv" for t in ENA_TABLES_NAME]
         for f in ena_file_outpath:
             if Path(f).exists():
@@ -555,16 +555,16 @@
             help="Path to a directory where the links should be created"
         ),
         lnk_name_template: str = typer.Option(
             None,
             "--link-name-formulae",
             "-f",
             help="An template formulae to build link name, e.g. '{Sample}_{Read Type}.fastq.gz', where the {X} "
-                 "placeholders will be replaced by matching metadata value e.g. '{Sample}' is replaced by the sample name"
-                 "and {Read Type} by the read number."
+                 "placeholders will be replaced by matching metadata value e.g. '{Sample}' is replaced by the sample "
+                 "name and {Read Type} by the read number."
                  "Note that 'X' must match, case-sensitively, column headers of the data file metadata table. "
                  "While some column headers are always available, others are context specific e.g. annotations, assay "
                  "type... you can learn which headers are available in your context with --list-data-headers"
         ),
         list_metadata_fields: bool = typer.Option(
             False,
             "--list-data-headers / --no-list-data-headers",
@@ -626,58 +626,68 @@
             query_params = list(query_params)
         query_params.append(f"is_primary_copy=True")
     elif lnk_name_template:
         raise typer.BadParameter(
             f"--formulae can only be used when linking to primary data copies i.e. not with --all.")
 
     # use singular form in filter_type, we have only_count set to False to be able to post filter
+    filters: Dict[str, str] = {}
     if study:
         filter_uuid = study
         expected_type = "study"
-    elif project:
+        _check_item_type(stocks_manager=stocks_manager, uuid=filter_uuid, expected_type=expected_type)
+        filters[expected_type] = filter_uuid
+    if project:
         filter_uuid = project
         expected_type = "project"
-    elif assay:
+        _check_item_type(stocks_manager=stocks_manager, uuid=filter_uuid, expected_type=expected_type)
+        filters[expected_type] = filter_uuid
+    if assay:
         filter_uuid = assay
         expected_type = "assay"
-    elif dataset:
+        _check_item_type(stocks_manager=stocks_manager, uuid=filter_uuid, expected_type=expected_type)
+        filters[expected_type] = filter_uuid
+    if dataset:
         filter_uuid = dataset
         expected_type = "dataset"
-    elif collection:
+        _check_item_type(stocks_manager=stocks_manager, uuid=filter_uuid, expected_type=expected_type)
+        filters[expected_type] = filter_uuid
+    if collection:
         filter_uuid = collection
         expected_type = "datasetcollection"
         # not sure this works
-    else:
-        raise typer.BadParameter(f"one of --project, --study, --assay, --collection or --dataset must be provided")
+        _check_item_type(stocks_manager=stocks_manager, uuid=filter_uuid, expected_type=expected_type)
+        filters[expected_type] = filter_uuid
+
+    if not filters:
+        raise typer.BadParameter(f"At least one of --project, --study, --assay, --collection or --dataset is expected")
 
-    # check uuid is for indicated type
-    filter_type = _check_item_type(stocks_manager=stocks_manager, uuid=filter_uuid, expected_type=expected_type)
     # fetch data now
-    filecopies: List[DatasetFileCopy] = stocks_manager.list_datafilecopies(filter_type=filter_type,
-                                                                           filter_uuid=filter_uuid,
-                                                                           only_primary_copy=primary)
+    filecopies: List[DatasetFileCopy] = stocks_manager.\
+        list_datafilecopies(filtertype2uuids=filters, only_primary_copy=primary)
 
     use_subpath_for_uniqueness: bool = False
 
     # do we have custom link name, if so validate
     custom_lnk_names = {}
     # a dict storing all the individual datasetfile a link should be created and whether it was successfully created
     all_datasetfile_path: Dict[str, bool] = {}
     if lnk_name_template or list_metadata_fields:
         # fetch all dataset meta
-        dataset_meta = stocks_manager.fetch_dataset_metatable(uuid=filter_uuid)
+        dataset_meta = stocks_manager.fetch_dataset_metatable(uuid=list(filters.values()))
         # convert to panda DF
         metatable = pd.read_table(
             io.BytesIO(dataset_meta), dtype=str, sep=",", keep_default_na=False).fillna('').astype(str)
         if reduce:
             metatable.replace('', np.nan, inplace=True)
             # drop empty columns
             metatable.dropna(axis=1, how='all', inplace=True)
 
-        metatable.to_csv(Path(target_dir, f"datafiles_metadata_for_{expected_type}_{filter_uuid}.csv"), index=False)
+        metatable_fname = f"datafiles_metadata.csv"
+        metatable.to_csv(Path(target_dir, metatable_fname), index=False)
 
         if list_metadata_fields:
             print(f"Available headers in this data context: {list(metatable)}")
             sys.exit()
 
         p = re.compile(r'{([^{}]+)}', re.IGNORECASE)
         headers = p.findall(lnk_name_template)
@@ -721,15 +731,15 @@
                 break
             link_names.add(dfc_res.shortname)
 
     info = []
     info_headers = ["shortname", "linkname", "uri", "is_primary_copy", "copy_id", "dataset_id"]
 
     for dfc_res in filecopies:
-        logger.warning(dfc_res.uri)
+        logger.debug(dfc_res.uri)
         # by default get the no formulae link name
         lnk_name: str = _get_run_dir_relpath(dfc_res) if use_subpath_for_uniqueness else dfc_res.shortname
         if lnk_name_template:
             # then get the custum name
             lnk_name = custom_lnk_names[dfc_res.uri]
         target_path = Path(target_dir, lnk_name)
 
@@ -946,15 +956,15 @@
             if do_export:
                 # remove the whole dir
                 shutil.rmtree(exp_dir)
 
         exp_dir.mkdir(parents=True, exist_ok=True)
 
         if do_export:
-            atts: List[StocksAttachment] = None
+            atts: List[StocksAttachment] | None = None
             if e.is_frozen:
                 # fetch latest .gz
                 logging.debug(f"Exporting frozen exp {e.id} : {e.name}")
                 atts: List[StocksAttachment] = stocks_manager.list_experiment_archives(
                     experiment_id=e.id, most_recent_only=True)
             else:
                 # fetch latest PDF & html
@@ -985,15 +995,15 @@
             if e.project not in id_to_projects:
                 id_to_projects[e.project] = stocks_manager.fetch_project(uuid=e.project)
             e.project = id_to_projects[e.project]
             writer.writerow(_exp_as_row(e, export_dir=export_dir, stocks_server_url=default_url))
         tsv_file.close()
 
     build_static_web_site_for_eln_export(
-        dir_path=export_dir, exp_table_path=exp_table_path, export_username=export_username,
+        dir_path=Path(export_dir), exp_table_path=exp_table_path, export_username=export_username,
         is_personal_export=is_personal_export, exported_project=project,
         exported_group_name=group_name, exported_user=username)
 
 
 def _determine_output_format(file_path: Path) -> str | None:
     """
     Test output extension and converts it to xlsx (for .xls & .xlsx), csv or json
@@ -1009,34 +1019,14 @@
         return "xlsx"
     elif file_path.name.lower().endswith(".xlsx"):
         return "xlsx"
     elif file_path.name.lower().endswith((".csv", ".txt")):
         return "csv"
     return "json"
 
-
-def _find_experiment_file(e: Experiment, experiment_dir_path: Path, extension: str) -> Path | None:
-    """
-    look for the html or PDF file export for the given experiment
-    :param e: the experiment to look for
-    :param experiment_dir_path: the dir_path in which the experiment Zip export has been unpacked
-    :param extension: html or pdf
-    :return:
-    """
-    if extension != 'pdf' and extension != 'html':
-        raise ValueError("extension must be either pdf or html")
-
-    names: List[str] = glob.glob(f"{e.name}*.{extension}", root_dir=experiment_dir_path)
-    if not names:
-        logger.warning(f"Could not find experiment {extension} file in {str(experiment_dir_path)}")
-        return None
-
-    return Path(experiment_dir_path, names[0])  # we r not suppose to have more than one file
-
-
 def _exp_as_row(e: Optional[Experiment], export_dir: Path | str | None, stocks_server_url: Optional[str],
                 only_headers=False) -> List[str]:
     if only_headers:
         return ['UUID', 'Name', 'Project', 'Owner', 'Group', 'Completion Status',
                 'Is Frozen', 'Summary', 'Started', 'Completed', 'Last Modified', 'Last Modified By',
                 'Frozen', 'HTML', 'PDF', 'Experiment Live Link', 'Project Live Link']
     if stocks_server_url[-1] != "/":
@@ -1108,15 +1098,14 @@
     names: List[str] = glob.glob(f"{e.name}*.{extension}", root_dir=experiment_dir_path)
     if not names:
         logger.warning(f"Could not find experiment {extension} file in {str(experiment_dir_path)}")
         return None
 
     return Path(experiment_dir_path, names[0])  # we r not suppose to have more than one file
 
-
 def determine_output_format(output):
     if not output.name.endswith((".xls", ".xlsx", ".csv", ".txt")):
         return "json"
     elif output.name.endswith(".xls"):
         logger.warning("Notice that the output is written as .xlsx. Excel might complain about the extension not "
                        "matching the content.")
     elif output.name.endswith((".csv", ".txt")):
@@ -1249,16 +1238,16 @@
             else:
                 new_df.drop(columns=["Comment[Spike In]", "Comment[Spike in dilution]"], inplace=True)
         elif has_spike_ins:
             new_df["Comment[Spike In]"] = df["Kit name"]
             new_df["Comment[Spike in dilution]"] = df["Kit dilution"]
 
         new_df["temp"] = df['Assay ID'].apply(
-            lambda
-                x: f'Standard {assay_dict[x].instrumentrun.instrument.model} {assay_dict[x].runtype.value} Sequencing')
+            lambda x:
+            f'Standard {assay_dict[x].instrumentrun.instrument.model} {assay_dict[x].runtype.value} Sequencing')
         new_df.rename(columns={'temp': 'Protocol REF'}, inplace=True)
 
         new_df["Performer"] = df['Assay ID'].apply(lambda x: owner_name(assay_dict[x]))
         new_df["Assay Name"] = df["Assay Name"]
         if stocks_comments:
             new_df['Comment[Assay_stocks_id]'] = df["Assay ID"]
         new_df["Technology Type"] = df['Assay ID'].apply(lambda x: assay_dict[x].technology.value + ' assay')
@@ -1275,25 +1264,25 @@
                    to_del_credentials: bool, execute: bool, stocks_manager: StocksManager) -> None:
     cmd = f"cd {export_dir}; ena-upload-cli --action add --secret {ena_cred_path} --center embl"
     for name, p in ena_file_outpath.items():
         cmd = f"{cmd} --{name} {p}"
     if not execute:
         cmd = f"{cmd} --dev"
         # Create fake data if needed
-        FAKE_DIR = None
+        fake_dir = None
         if ena_file_outpath.get('run'):
-            FAKE_DIR = os.path.join(export_dir, 'fake_data')
-            while os.path.exists(FAKE_DIR):  # Making sure an already existing folder will not be deleted.
-                FAKE_DIR = FAKE_DIR + '_tmp'
-            create_fake_data(FAKE_DIR, pd.read_table(ena_file_outpath['run']))
-            cmd = f"{cmd} --data {os.path.join(FAKE_DIR, '*')}"
+            fake_dir = os.path.join(export_dir, 'fake_data')
+            while os.path.exists(fake_dir):  # Making sure an already existing folder will not be deleted.
+                fake_dir = fake_dir + '_tmp'
+            create_fake_data(fake_dir, pd.read_table(ena_file_outpath['run']))
+            cmd = f"{cmd} --data {os.path.join(fake_dir, '*')}"
         else:
             cmd = f"{cmd} --no_data_upload"
         # Call ena-upload-cli command with fake data in ENA test sandbox
-        _ena_upload_cli(cmd, to_del_credentials, ena_cred_path, FAKE_DIR)
+        _ena_upload_cli(cmd, to_del_credentials, ena_cred_path, fake_dir)
 
     else:
         # Call ena-upload-cli command for metadata submission to the ENA
         _ena_upload_cli(cmd, to_del_credentials, ena_cred_path)
 
     for name, f in ena_file_outpath.items():  # Replace old tables with updated ones
         os.remove(f)
```

### Comparing `stocks-cli-0.2.2/cli/export_eln_website_utils.py` & `stocks-cli-0.3.0/cli/export_eln_website_utils.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.2/cli/export_utils.py` & `stocks-cli-0.3.0/cli/export_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import io
 import os
 import re
 import shutil
 import subprocess
 from datetime import datetime
 from pathlib import Path
-from typing import List, Dict, Any, Type
+from typing import List, Dict, Any
 from collections import OrderedDict
 import xml.etree.ElementTree as ET
 
 import numpy as np
 import pandas as pd
 import yaml
 from dateutil.relativedelta import relativedelta
@@ -749,15 +749,15 @@
     :param stocks_manager:
     :return:
     """
     assay_list: List[Assay] = []
     assay_dict: Dict[str, Assay] = {}
     for row in assay_info_table.itertuples():
         logger.debug(f"Fetching assay ID: {row[1]}")
-        assay = stocks_manager.fetch_assay(row[1], load_ownership=True)
+        assay = stocks_manager.fetch_assay(uuid=row[1], load_ownership=True)
         assay.description = parse_html(assay.description)
         instrument = Instrument(name='instrument', model=row[2])
         assay.instrumentrun = InstrumentRun(name='instrumentrun', instrument=instrument, technology=assay.technology,
                                             managed=True, platform=assay.platform)
         assay_list.append(assay)
         assay_dict[row[1]] = assay
```

### Comparing `stocks-cli-0.2.2/cli/fetch.py` & `stocks-cli-0.3.0/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.2/cli/register.py` & `stocks-cli-0.3.0/cli/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,15 @@
                                      f"Registered sniffers: {registry.get_registered_sniffer_names()}")
 
         if not sniffer.is_sniffer_valid_for(technology=technology, platform=platform):
             raise typer.BadParameter(f"Sniffer '{sniffer_name}' is not valid for technology/platform:"
                                      f" {technology}/{platform}.")
         # looks good, snif the dir_path
         try:
+            sniffer.set_stocks_manager(stocks_manager=stocks_manager)
             runs = sniffer.sniff_instrument_run_assays(
                 dir_path=indir, username=logged_in_user.username, group=stocks_group_name)
         except AssayStructureError as err:
             logger.error(str(err))
             print(f"The data in {str(indir)} does not comply to the sniffer {sniffer_name} expectations!")
             sys.exit(1)
 
@@ -245,14 +246,15 @@
     else:
         ####################
         # loop over sniffers and try !
         ####################
         for sniffer_cls in registry.get_sniffers():
             # get instance
             sniffer = sniffer_cls()
+            sniffer.set_stocks_manager(stocks_manager=stocks_manager)
             logger.debug(sniffer)
             if sniffer.is_sniffer_valid_for(technology=technology, platform=platform):
                 # looks good, snif the dir_path
                 try:
                     runs: List[InstrumentRun] = sniffer.sniff_instrument_run_assays(dir_path=indir,
                                                                                     username=logged_in_user.username,
                                                                                     group=stocks_group_name)
@@ -335,15 +337,15 @@
                     submitted = True
                 else:
                     o: PyDatasetListPost = stocks_manager._create_instrument_run_post(
                         instrument_run=runs[0], run_dir=indir, owner=logged_in_user.username, owned_by_group=stocks_group_name,
                         allow_pooled_samples=allow_pooled_samples, transfer_whole_input_dir=transfer_whole_input_dir,
                         study_id=study_id)
                     logger.warning("Dry-run: would submit payload (JSON):")
-                    logger.warning("\n" + o.json(exclude_none=True, exclude_unset=True))
+                    logger.warning("\n" + o.json(exclude_none=True, exclude_unset=False))
                     submitted = True
         except Exception:
             logger.error(f"Error:\n {traceback.format_exc()}")
             logger.error(f"An unexcepted error occurred, please check error logs.")
             exit(1)
```

### Comparing `stocks-cli-0.2.2/cli/utils.py` & `stocks-cli-0.3.0/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import distutils
+import smtplib
 import logging
+from shutil import copytree
+from email.message import EmailMessage
 from enum import Enum
 from html.parser import HTMLParser
 from pathlib import Path
 from pwd import getpwuid
 from subprocess import Popen, PIPE
-import smtplib
-from email.message import EmailMessage
 from typing import Union
 from uuid import UUID
 
-from jsonpickle import encode, handlers
+from jsonpickle import handlers
+
 from cli import config_parser
 
 logger = logging.getLogger(__name__)
 
 ############################
 # Constants and common models
 #############################
@@ -56,14 +57,16 @@
     DATAFILECOPY = "datafilecopy"
     DATASETCOLLECTION = "datasetcollection"
     DROPBOX = "dropbox"
     EXPERIMENT = "experiment"
     GROUP = "group"
     INSTRUMENTMODEL = "instrumentmodel"
     INSTRUMENTRUN = "instrumentrun"
+    NGSILLUMINAASSAY = "NGSILLUMINAASSAY"
+    NANOPOREASSAY = "NANOPOREASSAY"
     PROJECT = "project"
     PROTOCOL = "protocol"
     STORAGE_VOLUME = "storagevolume"
     SAMPLE = "sample"
     SPECIMEN = "specimen"
     STORAGE_EQUIPMENT = "storageequipment"
     STUDY = "study"
@@ -169,15 +172,15 @@
     SUPER_HIGH_ACCURACY = 'super high accuracy'
     METHYLATION = 'methylation'
     OTHER = 'other'
     NONE = 'None'
 
 
 class ObjectState(ExtendedEnum):
-    INITIALIZED: 'INITIALIZED'
+    INITIALIZED = 'INITIALIZED'
     NEW = 'NEW'
     REGISTERED = 'REGISTERED'
     TEMPLATE = 'TEMPLATE'
 
 
 def find_owner(path: Path) -> str:
     """gets the owner name of a file or dir_path"""
@@ -206,18 +209,18 @@
     from shutil import which
 
     return which(name) is not None
 
 
 def copy_dir(src: str, dst: str):
     if is_tool('rsync'):
-        rsync(src=src + "/", dest=dst)  # we make sure source as a trailing '/'
+        rsync(source=src + "/", dest=dst)  # we make sure source as a trailing '/'
     else:
         logger.info(f"rsync not avail => python copy_tree {src} to {dst}")
-        distutils.dir_util.copy_tree(src=src, dst=dst)
+        copytree(src=src, dst=dst)
 
 
 def mail_admin(mess: str):
     (mail_host, mail_smtp, admin_name, admin_email) = config_parser.get_mailing_details()
 
     # Create a text/plain message
     msg = EmailMessage()
```

### Comparing `stocks-cli-0.2.2/setup.py` & `stocks-cli-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="stocks-cli",
-    version="0.2.2",
+    version="0.3.0",
     author="GBCS",
     author_email="gbcs@embl.de",
     packages=["cli", "stocks", "stocks.assaysniffer", "stocksapi"],
     data_files=[('cli', ['cli/stockscli.ini'])],
     include_package_data=True,
     install_requires=requirements,
     extras_require={
```

### Comparing `stocks-cli-0.2.2/stocks/__init__.py` & `stocks-cli-0.3.0/stocks/__init__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.2/stocks/assaysniffer/__init__.py` & `stocks-cli-0.3.0/stocks/assaysniffer/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from abc import ABC, abstractmethod
 from typing import List, Any, Optional
 from pathlib import Path
 import logging
 
 from stocks.models import InstrumentRun
 from cli.utils import Technology
+from stocksapi.manager import StocksManager
 
 logger = logging.getLogger(__name__)
 
 def check_valid_directory(path: Path) -> bool:
     if not path or not path.exists() or not path.is_dir():
         return False
     return True
 
 
 class AssaySniffer(ABC):
+
+    def __init__(self, stocks_manager: StocksManager = None, **kwargs):
+        self.stocks_manager = stocks_manager
     """
     An AssaySniffer is responsible to parse run folders and extract Assay and Dataset description corresponding
     to one or many InstrumentRun.
     """
 
     @classmethod
     @abstractmethod
@@ -51,14 +55,17 @@
     def get_sniffer_description(cls) -> str:
         """
         Describes how this assay sniffer works i.e. what (meta)data is extracted
         :return: a string explaining what the plugin expects to find / is looking for
         """
         pass
 
+    def set_stocks_manager(self, stocks_manager: StocksManager):
+        self.stocks_manager = stocks_manager
+
     def is_sniffer_valid_for(self, technology: Technology, platform: str | None = None,
                              enforce_platform_match: bool = False) -> bool:
         """
         checks if this sniffer can be used for a given Technology and, optionally, a specific platform.
         The platform filtering only happens if a valid platform name is given.
         When a platform is given, a sniffer of requested technology that does not restrict on specific platform is
         considered valid unless enforce_platform_match is True
@@ -89,16 +96,16 @@
         :return the list of discovered Assay
         :except : AssayStructureError if the dir_path structure does not match sniffer's expectations
         """
         pass
 
 
 class JSONAssaySniffer(AssaySniffer):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, stocks_manager: StocksManager = None, **kwargs):
+        super().__init__(stocks_manager=stocks_manager, **kwargs)
 
     @abstractmethod
     def get_json_schema(self, technology: Technology, platform: str) -> Any:
         """
         Returns the JSON schema this sniffer uses for the technology and platform.
         """
         pass
```

### Comparing `stocks-cli-0.2.2/stocks/assaysniffer/registry.py` & `stocks-cli-0.3.0/stocks/assaysniffer/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import sys
 from importlib import import_module
 from pathlib import Path
 from typing import Type, Iterable, List, Set, Optional
 
 from stocks.assaysniffer import AssaySniffer
 
-logger = logging.getLogger("AssaySnifferRegistry")
-
+logger = logging.getLogger(__name__)
 
 class AssaySnifferRegistry:
     """A registry for `Assay Sniffer` classes."""
 
     def __init__(self):
         self._sniffers = {}
```

### Comparing `stocks-cli-0.2.2/stocks/assaysniffer/sniffers.py` & `stocks-cli-0.3.0/stocks/assaysniffer/sniffers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from datetime import datetime
 import logging
 from pathlib import Path
 from typing import Optional, List, Dict, Any
 
 from jsonschema import validate
 from stocks.models import InstrumentRun, User, Instrument, SequencingLibrary, NanoporeAssay, Dataset, \
-    DatasetCollection, DatasetFile, FastqFile, Fast5File, FastqDir, Fast5Dir, DataProducer, SequencingAssay, UserGroup
+    DatasetCollection, DatasetFile, FastqFile, Fast5File, FastqDir, Fast5Dir, DataProducer, SequencingAssay, \
+    UserGroup, Sample
 from stocks import AssayStructureError
 from cli.utils import Technology, SequencingReadType, SequencingRunType, NanoporeLiveBaseCallingType
 from stocks.assaysniffer import JSONAssaySniffer, AssaySniffer, check_valid_directory
 from stocks.assaysniffer.registry import registry
 import pandas as pd
 
 logger = logging.getLogger(__name__)
@@ -130,15 +131,15 @@
     def nanopore_file_exists(a_dir: Path, filename_pattern: str):
         for x in a_dir.glob(pattern=filename_pattern):
             return x.exists()
         return False
 
     def sniff_instrument_run_assays(self, dir_path: Path, group: str, username: Optional[str] = None) \
             -> List[InstrumentRun]:
-        owner: User
+        owner: User | None = None
         if username:
             owner = User(username=username, groups=[UserGroup(name=group)])
 
         if not check_valid_directory(dir_path):
             mess = f"The dir_path {str(dir_path)} is either empty or does not point to a valid directory."
             raise AssayStructureError(mess)
 
@@ -229,18 +230,19 @@
 
                 if Path(path.parent, "fastq_fail").exists():
                     datasets.extend(self.get_nanopore_demultiplexed_datasets(
                         run_dir=path.parent, dir_name="fastq_fail", sample_base_name=sample_id, file_type="fastq",
                         barcode_number=self.MAX_BARCODE_NUMBER))
 
                 # get unique list of samples
-                name2lib = dict()
+                name2lib: dict[str, Sample] = dict()
                 for d in datasets:
-                    if d.sample.name not in name2lib:
-                        name2lib[d.sample.name] = d.sample
+                    for _smpl in d.samples:
+                        if _smpl.name not in name2lib:
+                            name2lib[_smpl.name] = _smpl
                 samples = list(name2lib.values())
 
             else:
                 # we have a single assay, a single sample
                 sample = SequencingLibrary(name=sample_id, barcode=None)
                 samples.append(sample)
                 # create the different dataset
@@ -567,18 +569,18 @@
                                     "type": "object",
                                     "properties": {
                                         "name": {"type": "string"},
                                         "lane": {"type": "integer"},
                                         "user": {"type": "string"},
                                         "email": {"type": "string", "format": "email"},
                                         "type": {"enum": ["single-end", "paired-end", "multi-end"]},
-                                        "multiplexed": {"enum": ["true", "false"]},
-                                        "readlength": {"type": "string"},
+                                        "multiplexed": {"enum": ["true", "false", "True", "False", True, False]},
+                                        "readlength": {"type": ["integer", "string"]},
                                         "runmode": {"type": "string"},
-                                        "demultiplexed": {"enum": ["true", "false"]},
+                                        "demultiplexed": {"enum": ["true", "false", "True", "False", True, False]},
                                         "samples": {
                                             "type": "object",
                                             "patternProperties": {
                                                 "^.+$": {
                                                     "type": "object",
                                                     "properties": {
                                                         "barcode": {"type": "string"},
@@ -709,76 +711,89 @@
                 mess = f"AssaySniffer {self.get_sniffer_name()}: Parsing JSON file {json_path} failed."
                 logger.exception(mess)
                 raise AssayStructureError(mess)
 
         return runs
 
     def load_run_from_json_file(self, json_path: Path, group: str, username: str | None = None) -> InstrumentRun:
+        # load the file as a dict
+        with open(json_path) as json_file:
+            data = json.load(json_file)
+            return self.load_run_from_json_obj(data=data, data_dir=json_path.parent, group=group, username=username)
+
+    def load_run_from_json_obj(self, data: Any, data_dir: Path, group: str, username: str | None = None) \
+            -> InstrumentRun:
+        """
+        parses the GeneCore json payload into a InstrumentRun
+        :param data: the json object
+        :param data_dir: the dir (aka run dir) containing the data described in this json
+        :param group: the group the data belongs to
+        :param username: the group the data belongs to
+        """
+
+        # validate JSON with json schema
+        validate(data, schema=self.get_json_schema(Technology.SEQUENCING, "ILLUMINA"))
+
         owner: Optional[User] = None
         if username:
             owner = User(username=username, groups=[UserGroup(name=group)])
-        # first load the file as a dict
-        with open(json_path) as json_file:
-            data = json.load(json_file)
-            # validate JSON with json schema
-            validate(data, schema=self.get_json_schema(Technology.SEQUENCING, "ILLUMINA"))
 
-            managed = bool(data['managed'])
-            payload = data['data']
-            # the payload potentially holds many runs
-            for run_data in payload:
-                flowcell: str = run_data['flowcell']
-                run_id: str = run_data['runid']
-                instrument: Instrument = Instrument(name=run_data['sequencer']['name'],
-                                                    model=run_data['sequencer']['model'],
-                                                    serial_number=run_data['sequencer']['serialnumber'])
-                run = InstrumentRun(name=run_id,
-                                    managed=managed,
-                                    technology=Technology.SEQUENCING,
-                                    platform="ILLUMINA",
-                                    instrument=instrument,
-                                    producer=DataProducer(run_data['producer']['name']))
+        managed = bool(data['managed'])
+        payload = data['data']
+        # the payload potentially holds many runs
+        for run_data in payload:
+            flowcell: str = run_data['flowcell']
+            run_id: str = run_data['runid']
+            instrument: Instrument = Instrument(name=run_data['sequencer']['name'],
+                                                model=run_data['sequencer']['model'],
+                                                serial_number=run_data['sequencer']['serialnumber'])
+            run = InstrumentRun(name=run_id,
+                                managed=managed,
+                                technology=Technology.SEQUENCING,
+                                platform="ILLUMINA",
+                                instrument=instrument,
+                                producer=DataProducer(run_data['producer']['name']))
+            if owner:
+                run.set_owner(owner=owner, also_set_group=True)
+            else:
+                run.group = group
+
+            for assay_dict in run_data['lanes']:
+                assay_lane: int = assay_dict['lane'] if 'lane' in assay_dict else 1
+                assay_name: str = assay_dict['name'] if 'name' in assay_dict else f"{flowcell}_lane{assay_lane}"
+                user: str = assay_dict['user']
+                email: str = assay_dict['email'] if 'email' in assay_dict else ""
+                if not owner:
+                    owner = User(username=user, groups=[UserGroup(name=group)])
+                owner.email = email
+
+                run_type: SequencingRunType = SequencingRunType(assay_dict['type'])
+                multiplexed: bool = bool(assay_dict['multiplexed'])
+                demultiplexed: bool = bool(assay_dict['demultiplexed'])
+                read_length: str = assay_dict['readlength'] if 'readlength' in assay_dict else ""
+                run_mode: str = assay_dict['runmode'] if 'runmode' in assay_dict else ""
+                samples: Dict[str, SequencingLibrary] = self.__decode_samples(assay_dict['samples'])
+                datasets: List[Dataset] = self.__decode_datasets(assay_dict['filelist'],
+                                                                 samples, run_type, data_dir=data_dir)
+                # create an SequencingAssay
+                assay: SequencingAssay = SequencingAssay(name=assay_name,
+                                                         flowcell=flowcell,
+                                                         platform=run.platform,
+                                                         datasets=datasets,
+                                                         samples=list(samples.values()),
+                                                         chemistry="",
+                                                         instrumentrun=run,
+                                                         lane=assay_lane,
+                                                         multiplexed=multiplexed,
+                                                         demultiplexed=demultiplexed,
+                                                         runtype=run_type,
+                                                         runmode=run_mode,
+                                                         readlength=read_length
+                                                         )
                 if owner:
-                    run.set_owner(owner=owner, also_set_group=True)
+                    assay.set_owner(owner=owner, also_set_group=True)
                 else:
-                    run.group = group
-
-                for assay_dict in run_data['lanes']:
-                    assay_lane: int = assay_dict['lane'] if 'lane' in assay_dict else 1
-                    assay_name: str = assay_dict['name'] if 'name' in assay_dict else f"{flowcell}_lane{assay_lane}"
-                    user: str = assay_dict['user']
-                    email: str = assay_dict['email'] if 'email' in assay_dict else ""
-                    if not owner:
-                        owner = User(username=user, groups=[UserGroup(name=group)])
-                    owner.email = email
-
-                    run_type: SequencingRunType = SequencingRunType(assay_dict['type'])
-                    multiplexed: bool = bool(assay_dict['multiplexed'])
-                    demultiplexed: bool = bool(assay_dict['demultiplexed'])
-                    read_length: str = assay_dict['readlength'] if 'readlength' in assay_dict else ""
-                    run_mode: str = assay_dict['runmode'] if 'runmode' in assay_dict else ""
-                    samples: Dict[str, SequencingLibrary] = self.__decode_samples(assay_dict['samples'])
-                    datasets: List[Dataset] = self.__decode_datasets(assay_dict['filelist'],
-                                                                     samples, run_type, json_path.parent)
-                    # create an SequencingAssay
-                    assay: SequencingAssay = SequencingAssay(name=assay_name,
-                                                             flowcell=flowcell,
-                                                             platform=run.platform,
-                                                             datasets=datasets,
-                                                             samples=list(samples.values()),
-                                                             chemistry="",
-                                                             instrumentrun=run,
-                                                             lane=assay_lane,
-                                                             multiplexed=multiplexed,
-                                                             demultiplexed=demultiplexed,
-                                                             runtype=run_type,
-                                                             runmode=run_mode,
-                                                             readlength=read_length
-                                                             )
-                    if owner:
-                        assay.set_owner(owner=owner, also_set_group=True)
-                    else:
-                        assay.group = group
+                    assay.group = group
 
-                    run.add_assay(assay)
+                run.add_assay(assay)
 
         return run
```

### Comparing `stocks-cli-0.2.2/stocks/models.py` & `stocks-cli-0.3.0/stocks/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,16 +195,16 @@
         self.unix_name: Optional[str] = None  # unix user name
         self.email: Optional[str] = email  # user email
         self.orcid: Optional[str] = None  # user ORCID ID
 
         self.groups: Dict[str, 'UserGroup'] = {}
         if groups:
             self.groups = {}
+            logger.warning(f"groups => {type(groups)}")
             if isinstance(groups, list):
-                logger.warning(f"groups => {type(groups)}")
                 for grp in groups:
                     logger.warning(f"grp {grp} of type \n {type(grp)}")
                     self.groups[grp.name] = grp
             elif isinstance(groups, dict):
                 self.groups = groups
         assert(isinstance(self.groups, dict))
 
@@ -607,15 +607,15 @@
 class SequencingAssay(Assay):
     def __init__(self, name: str, flowcell: str, id: Optional[str] = None,
                  platform: str = "ILLUMINA", description: Optional[str] = None,
                  datasets: Optional[List[Dataset]] = None, samples: Optional[List[Sample]] = None,
                  chemistry: str = "", instrumentrun: InstrumentRun | str = None, lane: int = 1,
                  multiplexed: bool = None, demultiplexed: bool = None,
                  runtype: SequencingRunType = SequencingRunType.SINGLE_END, runmode: str = "",
-                 readlength: str = None, **kwargs):
+                 readlength: str = None, info: str = None, **kwargs):
         super().__init__(name=name, id=id, description=description,
                          technology=Technology.SEQUENCING, platform=platform,
                          datasets=datasets, samples=samples, instrumentrun=instrumentrun,
                          multiplexed=multiplexed, **kwargs)
         self.stocks_model_type = "NGSILLUMINAASSAY"
 
         if demultiplexed is None:
@@ -631,14 +631,15 @@
         self.flowcell: str = flowcell
         self.flowcell_version: str = ""
         self.lane: int = lane
         self.runtype: SequencingRunType = runtype
         self.runmode: str = runmode
         self.readlength: str = readlength
         self.chemistry: str = chemistry
+        self.info: str = info  ## this slot is only avail on INITILAIZED ASSAY FROM GENECORE BRIDGE
 
 
 class NanoporeAssay(SequencingAssay):
     def __init__(self, name: str, flowcell: str, flowcell_version: str,
                  id: Optional[str] = None, description: Optional[str] = None,
                  datasets: Optional[List[Dataset]] = None, samples: Optional[List[Sample]] = None,
                  chemistry: str = "", instrumentrun: InstrumentRun | str = None,
```

### Comparing `stocks-cli-0.2.2/stocks_cli.egg-info/PKG-INFO` & `stocks-cli-0.3.0/stocks_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocks-cli
-Version: 0.2.2
+Version: 0.3.0
 Summary: Command Line Interface to the STOCKS server
 Home-page: https://www.embl.org/research/units/genome-biology/genome-biology-computational-support/
 Author: GBCS
 Author-email: gbcs@embl.de
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `stocks-cli-0.2.2/stocks_cli.egg-info/SOURCES.txt` & `stocks-cli-0.3.0/stocks_cli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENSE.txt
+MANIFEST.in
 README.md
+pypi_description.md
 setup.py
 cli/__init__.py
 cli/__main__.py
 cli/config.py
 cli/export.py
 cli/export_eln_website_utils.py
 cli/export_utils.py
 cli/fetch.py
 cli/register.py
 cli/stockscli.ini
 cli/utils.py
+cli/validate.py
 stocks/__init__.py
 stocks/models.py
 stocks/assaysniffer/__init__.py
 stocks/assaysniffer/registry.py
 stocks/assaysniffer/sniffers.py
 stocks_cli.egg-info/PKG-INFO
 stocks_cli.egg-info/SOURCES.txt
```

### Comparing `stocks-cli-0.2.2/stocksapi/client.py` & `stocks-cli-0.3.0/stocksapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,15 @@
         logger.debug("PUT to url: %s", url)
         logger.debug("With query params: %s", query_params)
         logger.debug("Payload: %s", payload)
         response = requests.put(url,
                                 json=payload,
                                 headers=self._get_headers(),
                                 params=query_params)
+        logger.debug(f"PUT response: {response}")
         return handle_response(response)
 
     def post(self, path, payload=None, file=None, query_params=None):
         url = urljoin(self.url, path)
         logger.debug("POST to url: %s", url)
         logger.debug("With query params: %s", query_params)
         logger.debug("Payload: %s", payload)
```

### Comparing `stocks-cli-0.2.2/stocksapi/exceptions.py` & `stocks-cli-0.3.0/stocksapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.2.2/stocksapi/manager.py` & `stocks-cli-0.3.0/stocksapi/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,31 +27,37 @@
 #     pydantic_dataset_to_dataset, pydantic_study_to_study
 from stocksapi.exceptions import HTTPException, MultipleObjectMatchedError, ItemNotFoundException
 from stocksapi.models import *
 from stocks.models import Protocol, Assay, Study, User, Dataset, AnnotationType, InstrumentRun, DatasetCollection, \
     Sample, SequencingAssay, Project, UserGroup, StocksCVTerm, Experiment, Ontology, OntologyTerm, \
     DatasetFileCopy, SimpleInstrumentRun, OwnableMixin, AnnotableMixin, StocksBaseItem,SequencingLibrary
 from stocksapi.client import StocksClient, model_to_url
-from cli.utils import HTMLFilter, ModelType, is_uuid, ExtendedEnum
+from cli.utils import HTMLFilter, ModelType, is_uuid, ExtendedEnum, ObjectState
 
 logger = logging.getLogger(__name__)
 
 
 def handle_response(response, fail_on_missing_permission=True) -> Any | None:
     """
     :param response: Response from the stocks API
     :param fail_on_missing_permission: raise PermissionError if unauthorized request unless false (return None)
     :return: request results or None
     :raises PermissionError if unauthorized request and fail_on_missing_permission True
     :raises ItemNotFoundException if 404 is returned
     :raises HTTPException if other error
     """
     code, results = response
-    if code in [200, 201, 204]:
+    if code in [200, 201, 202, 204]:
         return results
+    elif code == 400:
+        if fail_on_missing_permission:
+            raise ValueError(results['message'])
+        else:
+            logger.error(f"request error code {code}: Invalid ID.")
+            return None
     elif code == 401:
         if fail_on_missing_permission:
             # logger.debug(f"request error code {code}: Unauthorized.")
             raise PermissionError(results['message'])
         else:
             logger.error(f"request error code {code}: Unauthorized.")
             return None
@@ -206,42 +212,49 @@
         url = f'{model_to_url[model]}{id}/annotations/'
         query_params = self.get_query_params({"search": ann_type})
         res = _check_result(handle_response(self.client.get(url, query_params)), id, ann_type)
         if res:
             return res[0]["value"], res[0]["id"]
         return None
 
-    def fetch_dataset_metatable(self, uuid: str, format: str = "csv", for_magetab = False):
+    def fetch_dataset_metatable(self, uuid: str | List[str], format: str = "csv", for_magetab = False):
         """
         Fetch a dataset-oriented summary table for a given study.
-        :param uuid: the study/project/assay/datasetcollection UUID
+        :param uuid: one or more study/project/assay/datasetcollection UUID, note that a unique UUID per object type
+         (eg study) is supported. If multiple IDs are given for a given object type, the last one only will be used
         :param format: 'csv' or 'xlsx' (or raise a ValueError).
         :param for_magetab: this is a temp param, which you can turn to False to use the new generic API datafilemeta_export endpoint
         :return: csv formatted text or binary text if format is 'xlsx'
         """
         query_params = self.get_query_params(None)
         query_params["response_format"] = "flat"
         query_params["page_size"] = "max"
         if format not in ["xlsx", "csv"]:
             raise ValueError(f"Wrong format, must be xlsx or csv: {format}")
+
+        uuids: List[str] = uuid
+        if isinstance(uuid, str):
+            uuids = [uuid]
+
         # fetch
-        status, data = self.client.resolve(uuid)
-        if data["model_name"] == ModelType.STUDY.value:
-            query_params["study_id"] = uuid
-        elif data["model_name"] == ModelType.PROJECT.value:
-            query_params["project_id"] = uuid
-        elif data["model_name"] == ModelType.DATASETCOLLECTION.value:
-            query_params["datasetcollection_id"] = uuid
-        elif data["model_name"] == ModelType.ASSAY.value:
-            query_params["assay"] = uuid
-        elif data["model_name"] == ModelType.DATASET.value:
-            query_params["dataset_id"] = uuid
-        else:
-            raise ValueError(f'Wrong value provided in the UUID. This must be a Study/Project/Assay/DatasetCollection'
-                             f' UUID while {uuid} points to a {data["model_name"]} object')
+        for _id in uuids:
+            status, data = self.client.resolve(_id)
+            if data["model_name"] == ModelType.STUDY.value:
+                query_params["study_id"] = _id
+            elif data["model_name"] == ModelType.PROJECT.value:
+                query_params["project_id"] = _id
+            elif data["model_name"] == ModelType.DATASETCOLLECTION.value:
+                query_params["datasetcollection_id"] = _id
+            elif data["model_name"] == ModelType.ASSAY.value:
+                query_params["assay"] = _id
+            elif data["model_name"] == ModelType.DATASET.value:
+                query_params["dataset_id"] = _id
+            else:
+                raise ValueError(f'Wrong value provided in the UUID. This must be a Study/Project/Assay/DatasetCollection'
+                                 f' UUID while {_id} points to a {data["model_name"]} object')
 
         url = model_to_url[ModelType.DATASET]
         url = urljoin(url, "datafilemeta_export")
         data = handle_response(self.client.get(url, query_params))
         if data is None:
             logger.info(f"Request for metatable export yielded not results. Study ID: {uuid}")
         return data
@@ -276,40 +289,78 @@
             onto = Ontology(name=dbxref_id.split("/")[-1].replace(':', '_').split("_")[0], url=dbxref_id.rsplit("/", 1)[0])
             onto_term = OntologyTerm(name=pydantic_term.name, term_id=dbxref_id.split("/")[-1], ontology=onto)
             ontology_mappings = {onto.name: onto_term}
             d['ontology_mappings'] = ontology_mappings
         term: StocksCVTerm = StocksCVTerm(**d)
         return term
 
-    def fetch_assay(self, uuid: str, load_ownership: bool=False) -> SequencingAssay | None:
+    def fetch_assay(self, uuid: str = None, run_dir: str = None, load_ownership: bool=False) -> SequencingAssay | None:
         """
-        gets assay details
+        gets assay details by UUID or run dir path
         :param uuid: the assay's UUID
+        :param run_dir: the assay run directory path  UUID
         :param load_ownership: True to fetch User onject from stocks, else owner is username
         :return: a subclass of model.Assay from stocks package
         """
-        results = self.fetch_item(uuid, ModelType.ASSAY)
-        ass_type = None
-        if 'platform' in results and 'value' in results['platform']:
-            if isinstance(results["platform"]["value"], dict):
-                ass_type = results["platform"]["value"]["value"]
-            ass_type = results["platform"]["value"]
-        if not ass_type:
-            logger.error(f"Error when fetching assay from server: platform value is missing. Assay ID: {uuid}")
-            raise ValueError("Error when fetching assay from server: platform value is missing.")
+        if not uuid and not run_dir:
+            raise ValueError(f"One of uuid or run_dir must be provided to lookup an assay")
+
+        if uuid:
+            if not is_uuid(uuid):
+                raise TypeError(f"Value give for UUID is not a UUID: {uuid}")
+
+            results = self.fetch_item(uuid, ModelType.ASSAY)
+        else:
+            query_params = list()
+            query_params.append(f"run_dir={run_dir}")
+            results = self.list_items(model=ModelType.ASSAY.value, query_params=query_params)
+            if len(results) == 0:
+                results = None
+            elif len(results) > 1:
+                raise MultipleObjectMatchedError(results=results,
+                                                 message=f"Unexpected error: more than one assay are connected to the "
+                                                         f"run dir {run_dir}. Please report to admin.")
+            else:
+                results = results[0]
+
+        model_type = results['model_type']
+        assay_state = results['state']['value']
+
+        logger.debug(f"Assay platform: {model_type}")
+        if model_type.upper() in (ModelType.NGSILLUMINAASSAY.value,ModelType.NANOPOREASSAY.value) :
+            # is the assay initialized only?
+            if results['state']['value'] == ObjectState.INITIALIZED.value:
+                # grab details in json format from the 'info' slot; slot is only used in this situation
+                assay_info = json.loads(results['info'])
+                logger.debug(assay_info)
+                # we can only have one lane in one assay (as of now)
+                lane_info = assay_info['data'][0]['lanes'][0]
+                results['flowcell'] = assay_info['data'][0]['flowcell']
+                #logger.debug(lane_info)
+                results['demultiplexed'] = str(lane_info['demultiplexed']).lower() == 'true'
+                if 'multiplexed' not in results:
+                    results['multiplexed'] = results['nr_of_samples'] > 1
+                if 'runtype' not in results or not results['runtype']:
+                     results['runtype'] = lane_info['type']
+                if 'runmode' not in results or not results['runmode']:
+                    results['runmode'] = lane_info['runmode']
+                if 'state' not in results or not results['state']:
+                    results['state'] = assay_state
+                if 'lane' not in results or not results['lane']:
+                    results['lane'] = lane_info['lane']
+                if 'readlength' not in results or not results['readlength']:
+                    results['readlength'] = lane_info['readlength']
 
-        logger.debug(f"Assay platform: {ass_type}")
-        if ass_type.upper() == "ILLUMINA":
             pydantic_assay = PydanticSequencingAssay.parse_obj(results)
             d = pydantic_assay.dict()
             assay = SequencingAssay(**d)
 
         # TODO non-ILLUMINA assays
         else:
-            raise ValueError(f"Error when fetching assay with id {uuid}. Assay Type not supported: {ass_type}.")
+            raise ValueError(f"Error when fetching assay with id {uuid}. Assay Type not supported: {model_type}.")
             # assay = Assay(name='na', technology=Technology.OTHER)
 
         if load_ownership:
             self.init_ownership(assay)
         return assay
 
     def fetch_item(self, uuid: str, model: ModelType, query_params: dict | List = None) -> Any:
@@ -319,14 +370,15 @@
         :param model: the STOCKS model name
         :param query_params: either a dict or a list of 'key=value' filters
         :raises ItemNotFoundException on 404
         :return: JSON
         """
         if not isinstance(model, ModelType):
             raise TypeError(f"Parameter model should be of utils.ModelType")
+
         logger.debug(f"Fetching {model.value} with ID {uuid}")
         query_params = self.get_query_params(query_params)
         try:
             data = handle_response(self.client.get(urljoin(model_to_url.get(model), uuid), query_params))
             return _check_result(data, uuid, model.value)
         except ItemNotFoundException as e:
             e.type = model.value
@@ -383,14 +435,15 @@
         data = self.fetch_item(uuid=uuid, model=ModelType.INSTRUMENTMODEL)
         py: PydanticInstrumentModel = PydanticInstrumentModel.parse_obj(data)
         fields = py.dict(by_alias=True)
         return InstrumentModel(**fields)
 
     def fetch_instrument_run(self, uuid: str) -> InstrumentRun | None:
         data = self.fetch_item(uuid=uuid, model=ModelType.INSTRUMENTRUN)
+        logger.debug(data)
         py: PydanticSimpleInstrumentRun = PydanticSimpleInstrumentRun.parse_obj(data)
         instrument_id: str = py.instrument.id
         # fetch instruemnt details
         data_instr = self.fetch_item(uuid=instrument_id, model=ModelType.EQUIPMENT)
         instrument = PydanticInstrument.parse_obj(data_instr)
         # properly init the model
         data_instr_model = self.fetch_item(
@@ -574,28 +627,45 @@
         """
         query_params = {"fields": "name,id", "page_size": "max"}
         results = handle_response(self.client.get(model_to_url.get(ModelType.ANNOTATION), query_params))["results"]
         annotation_list = [AnnotationType(name=ann["name"], id=ann["id"]) for ann in results]
 
         return annotation_list
 
+
     def list_datafilecopies(self, filter_type: str = None, filter_uuid: str = None, only_primary_copy=True) \
             -> List[DatasetFileCopy]:
         """
         list datafile copies as DatasetFile
         :param filter_type: project, study, assay, dataset or datasetcollection
         :param filter_uuid: the uuid of the filter_type's object
         :param only_primary_copy: if only primary copies should be returned
 
         :return:
         """
+        if filter_uuid and filter_type:
+            return self.list_datafilecopies(filtertype2uuids={filter_type : filter_uuid},
+                                            only_primary_copy=only_primary_copy)
+        return self.list_datafilecopies(only_primary_copy=only_primary_copy)
+
+    def list_datafilecopies(self, filtertype2uuids: Dict[str,str] | None = None, only_primary_copy=True) \
+            -> List[DatasetFileCopy]:
+        """
+        list datafile copies as DatasetFile with 0 or many filters.
+        :param filtertype2uuids: a dict of filter_type (project, study, assay, dataset or datasetcollection) and
+        uuid specifying filter objects to which datafilecopies must belong
+        :param only_primary_copy: if only primary copies should be returned
+
+        :return:
+        """
         query_params = self.get_query_params()
 
-        if filter_uuid and filter_type:
-            query_params[f"{filter_type}_id"] = filter_uuid
+        if filtertype2uuids:
+            for filter_type, filter_uuid in filtertype2uuids.items():
+                query_params[f"{filter_type}_id"] = filter_uuid
 
         # the filter below is not yet avail and will be ignored by the server
         # we still have it here for when it becomes avail
         # for now, we set only_count=False in _list_items() calls and post-filter
         if only_primary_copy:
             query_params['is_primary_copy'] = True
 
@@ -1121,14 +1191,72 @@
 
         data = data['results']
         logger.debug(data)
         # TODO: we could return the assay object but then we need to make sure to share the code
         # with loadAssay()
         return data['id']
 
+    def validate_assay(self, assay: Assay, study_id: str, allow_pooled_samples: bool = True):
+        """
+        validates a pre-registered (i.e. 'INITIALIZED') SEQUENCING assay. Use PUT at
+        https://gbcs-dev.embl.de:81/api/v2/assays/assays/<assay uuid>/register/?allow_pooled_samples=false
+
+        @param assay: the assay to validate. Must have an existing UUID set in assay.id
+        @param study_id: the id under which all datasets will be registered.
+        """
+        if not assay.id or not is_uuid(assay.id):
+            raise ValueError("A valid UUID for the assay is required.")
+
+        assay_id:str = assay.id
+        query_params = {"allow_pooled_samples": allow_pooled_samples}
+
+        # assay validation uses a particular legacy payload, uses the PyAssayValidate* classes
+        da_lst: List[PyAssayValidateDataset] = list()
+        for d in assay.datasets:
+            o: User = d.owner
+            if not o or not isinstance(o, User):
+                o = assay.owner
+                if not o or not isinstance(o, User):
+                    raise ValueError("A valid User is expected in either dataset or assay's owner slot")
+            s: SequencingLibrary = d.samples[0]
+            if not s or not isinstance(s, SequencingLibrary):
+                raise ValueError(f"A SequencingLibrary object is expected for each dataset, got {type(s)} for dataset "
+                                 f"{d.name}")
+
+            datafiles: List[PyAssayValidateDatafile] = list()
+            f: FastqFile = None
+            for f in d.datafiles:
+                datafiles.append(PyAssayValidateDatafile(
+                    uri=f.uri,
+                    name=f.name,
+                    filetype=f.filetype,
+                    readtype=str(f.read_type),
+                    checksum= "" if not f.md5sum else f.md5sum,
+                    filesize=f.byte
+                ))
+
+            da: PyAssayValidateDataset = PyAssayValidateDataset(
+                datafiles=PyAssayValidateValueList(value=datafiles),
+                owner=PyAssayValidateValue(value = PyAssayValidateUser(id=o.id, username=o.username)),
+                sample=PyAssayValidateValue(value=s.name),
+                barcode=PyAssayValidateValue(value=s.barcode),
+                studies=PyAssayValidateValueList(value=[ PyAssayValidateId(id=study_id) ] )
+            )
+            da_lst.append(da)
+
+        put_obj = PyAssayValidate(datasets=da_lst)
+        payload_str = put_obj.json()
+        with open("/Users/girardot/Desktop/payload.json", "w") as text_file:
+            text_file.write(payload_str)
+        # PUT at https://gbcs-dev.embl.de:81/api/v2/assays/assays/<assay uuid>/register/?allow_pooled_samples=false
+        path = f"{model_to_url[ModelType.ASSAY]}{assay_id}/register/"
+        data = handle_response(
+            self.client.put(path, payload=json.loads(payload_str), query_params=query_params))
+        return(data)
+
     def _prepare_object_for_post(self, stocks_object: PydanticStocksBaseItem,
                                 alt_owner: PydanticUser | None = None,
                                 alt_owned_by: PydanticUserGroup | None = None):
         """
         operate conversion to produce a valid JSON
         """
```

### Comparing `stocks-cli-0.2.2/stocksapi/models.py` & `stocks-cli-0.3.0/stocksapi/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
     Various data models to communicate with the STOCKS API.
 """
 import logging
 from datetime import datetime, date
 from typing import Optional, List, Dict, Any
 
-from pydantic import BaseModel, Field, Extra, validator  # pylint:disable=E0611
+from pydantic import BaseModel, Field, Extra, validator, ValidationError  # pylint:disable=E0611
 
-from stocks.models import User, Instrument, DatasetFile, InstrumentModel, InstrumentRun, SimpleInstrumentRun, Assay, \
+from stocks.models import User, Instrument, DatasetFile, InstrumentModel, SimpleInstrumentRun, Assay, \
     UserGroup
 from cli.utils import Technology, SequencingRunType, ExperimentStatus, NanoporeLiveBaseCallingType, NanoporeAdaptiveMode
 from uuid import UUID
 
 logger = logging.getLogger(__name__)
 
 def _check_datetime_from_api(val, as_datetime=False) -> datetime | str | Dict | date:
@@ -586,15 +586,15 @@
 
 class PydanticSimpleInstrumentRun(PydanticStocksBaseItem):
     instrument: PydanticInstrument | PydanticReferencedStocksObject | str | None
     start_datetime: datetime | None
     end_datetime: datetime | None
     producer: str | None
     responsible_person: PydanticUser | str | None
-    assays: List["PydanticAssay"] = list()
+    assays: List["PydanticAssay"] | List[str] = list()
 
     @validator('instrument', pre=True)
     def check_instrument(cls, instrument):
         logging.debug(f"got instrument var of type {type(instrument)} :\n {instrument}")
         if isinstance(instrument, Instrument):
             return PydanticInstrument(**dict(vars(instrument)))
         elif isinstance(instrument, dict):
@@ -607,23 +607,26 @@
     @validator('assays', pre=True)
     def check_assays(cls, val):
         if not val:
             return list()
         if not isinstance(val, list):
             # let validation complain
             return val
-        l = list()
+        lst = list()
         for o in val:
             if isinstance(o, Assay):
-                l.append(PydanticAssay(**dict(vars(o))))
+                lst.append(PydanticAssay(**dict(vars(o))))
             elif isinstance(o, dict):
-                l.append(PydanticAssay(**o))
+                try:
+                    lst.append(PydanticAssay(**o))
+                except ValidationError:
+                    lst.append(o['id'])
             else:
-                l.append(o)  # will most likely raise an error if this is not an PydanticAssay
-        return l
+                lst.append(o)  # will most likely raise an error if this is not an PydanticAssay
+        return lst
 
 
 class PydanticSimpleInstrumentRunPost(BaseModel, extra=Extra.allow):
     """
     wrapper to POST a InstrumentRun
     """
     results: PydanticSimpleInstrumentRun
@@ -705,15 +708,16 @@
     readlength: str | None = None
     chemistry: str | None = None
     live_base_calling: NanoporeLiveBaseCallingType | PydanticValueField = NanoporeLiveBaseCallingType.NONE
     live_read_mapping: bool | None = None
     ref_genome: Optional[str] = None
     adaptive_mode: NanoporeAdaptiveMode | PydanticValueField = NanoporeAdaptiveMode.NONE
     adaptive_mode_details: str | None = None
-    demultiplexed: str | None = None
+    demultiplexed: bool | str | None = None
+    info: str | None = None  # this is to support the INITIALIZED ASSAY
 
     class Config:
         extra = Extra.ignore
 
     @validator('live_base_calling', pre=True)
     def extract_live_base_calling(cls, val):
         if isinstance(val, dict) and 'value' in val:
@@ -812,15 +816,15 @@
 class PydanticDataset(PydanticStocksBaseItem):
     qc: str | None = None
     dataset_type: str | None = None
     is_raw: bool | None = None
     is_managed: bool = False
     datafiles: List[PydanticDatasetFile]
     collection: str | None = None
-    samples: List[PydanticSample | str ] | None
+    samples: List[PydanticSample | str] | None
     # note the order is important as pydantic will follow this order when parsing objects
     parent_samples: List[str | PydanticSample | PydanticReferencedStocksObject] | None
     studies: List[str | PydanticStudy | PydanticReferencedStocksObject] | None
     assay: str | PydanticAssay | PydanticReferencedStocksObject | None
 
     @validator('qc', pre=True)
     def check_qc(cls, qc):
@@ -831,21 +835,21 @@
     @validator('dataset_type', pre=True)
     def check_dataset_type(cls, dataset_type):
         if isinstance(dataset_type, dict):
             return dataset_type['label']
         return dataset_type
 
 
-##
-## Pydantic classes used to post new datasets with optional samples, associated assays, collection
-## and instrument run
-## We have the following situations
-## - derived datasets with optional link to sample(s) and parent dataset(s); also reference to assay is possible
-## - raw dataset(s) with link to sample(s) and assay(s) information and run information
-##
+#
+# Pydantic classes used to post new datasets with optional samples, associated assays, collection
+# and instrument run
+# We have the following situations
+# - derived datasets with optional link to sample(s) and parent dataset(s); also reference to assay is possible
+# - raw dataset(s) with link to sample(s) and assay(s) information and run information
+#
 
 class PyDatasetListPost(BaseModel, extra=Extra.ignore):
     input_dir: str
     allow_pooled_samples: bool
     transfer_whole_input_dir: bool = True
     owned_by: str
     run: Optional[PydanticInstrumentRun]
@@ -855,7 +859,45 @@
     datasets: Optional[List[PydanticDataset]] = list()
 
 
 class PyOldDatasetListPost(PyDatasetListPost):
     class Config:
         extra = Extra.ignore
         fields = {'run': {'exclude': True}}
+
+
+# below are set of classes to support the assay_validate payload
+class PyAssayValidateUser(BaseModel, extra=Extra.ignore):
+    id: int
+    username: str
+
+
+class PyAssayValidateId(BaseModel, extra=Extra.ignore):
+    id: str
+
+
+class PyAssayValidateValue(BaseModel, extra=Extra.allow):
+    value: str | PyAssayValidateUser
+
+
+class PyAssayValidateDatafile(BaseModel, extra=Extra.ignore):
+    uri: str
+    name: str
+    filetype: str
+    readtype: str
+    checksum: str | None
+    filesize: int | None
+
+class PyAssayValidateValueList(BaseModel, extra=Extra.allow):
+    value: List[PyAssayValidateDatafile] | List[PyAssayValidateId]
+
+
+class PyAssayValidateDataset(BaseModel, extra=Extra.ignore):
+    datafiles: PyAssayValidateValueList
+    owner: PyAssayValidateValue
+    sample: PyAssayValidateValue
+    barcode: PyAssayValidateValue
+    studies: PyAssayValidateValueList
+
+
+class PyAssayValidate(BaseModel, extra=Extra.ignore):
+    datasets: List[PyAssayValidateDataset]
```

