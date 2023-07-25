# Comparing `tmp/alacorder-80.8.9.tar.gz` & `tmp/alacorder-81.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.8.9.tar", max compression
+gzip compressed data, was "alacorder-81.0.0.tar", max compression
```

## Comparing `alacorder-80.8.9.tar` & `alacorder-81.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.9/LICENSE
--rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.9/README.md
--rw-r--r--   0        0        0      697 2023-06-30 15:20:31.008120 alacorder-80.8.9/pyproject.toml
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   293108 2023-06-30 15:20:17.400313 alacorder-80.8.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   293108 2023-06-30 15:20:10.717636 alacorder-80.8.9/src/alacorder/alac.py
--rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 alacorder-80.8.9/PKG-INFO
+-rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.0.0/README.md
+-rw-r--r--   0        0        0     6148 2023-07-25 18:33:29.627273 alacorder-81.0.0/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-25 02:41:14.357279 alacorder-81.0.0/alacorder/__init__.py
+-rw-r--r--   0        0        0   198912 2023-07-25 18:29:15.087459 alacorder-81.0.0/alacorder/__main__.py
+-rw-r--r--   0        0        0   198912 2023-07-25 18:31:14.118594 alacorder-81.0.0/alacorder/alac.py
+-rw-r--r--   0        0        0      557 2023-07-25 18:34:50.889343 alacorder-81.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.0.0/PKG-INFO
```

### Comparing `alacorder-80.8.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-81.0.0/alacorder/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,5786 +1,3060 @@
 """
-ALACORDER --------------------
-╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
-╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
-╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
-(c) 2023 Sam Robson ----------
-
-Dependencies: 
-    python 3.9+, brotli ^1.0.9, click ^8.1.3,
-    polars ^0.17.6, PyMuPDF ^1.21.1,
-    PySimpleGUI ^4.60.4, selenium ^4.8.3, 
-    tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
-Optional dependencies:
-    pyarrow required to export summary to .xls, .xlsx,
-    Google Chrome required to fetch cases from Alacourt
-"""
+┏┓┓ ┏┓┏┓┏┓┳┓┳┓┏┓┳┓
+┣┫┃ ┣┫┃ ┃┃┣┫┃┃┣ ┣┫
+┛┗┗┛┛┗┗┛┗┛┛┗┻┛┗┛┛┗
+(c) 2023 Sam Robson
 
-name = "ALACORDER"
-long_version = "snowpalace"
-version = "80.6.5"
+Dependencies: Python 3.9+, Google Chrome, brotli 1.0.9+, polars 0.18.1+, pymupdf 1.21.1+, rich 13.3.3+, selenium 4.8.3+, typer 0.9.0+, xlsx2csv 0.8.1+, xlsxwriter 3.0.9+
+"""
 
-_autoload_graphical_user_interface = False
+__version__ = "81.0.0"
 
+import os
+import re
+import glob
+import time
+import typer
+from typing_extensions import Annotated
+from pathlib import Path
+from rich.progress import Progress, MofNCompleteColumn
+from rich.console import Console
+import fitz
 import polars as pl
-import os, sys, time, glob, re, math
-import click, fitz, selenium, xlsxwriter
-from tqdm.auto import tqdm
-from random import sample
-from datetime import datetime
+import xlsxwriter
+from bs4 import BeautifulSoup
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
-from selenium.webdriver.chrome.options import Options
-
-
-#   #   #   #                LOGS                #   #   #   #
-
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
 
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(100)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_dataframe_shape_below(True)
 pl.Config.set_tbl_hide_column_data_types(True)
-CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
-FNAME = f"{name} {version}"
-FSHORT_NAME = f"{name} {'.'.join(version.split('.')[0:-1])}"
-
-prt = print
-
 
-def plog(*msg, cf=None):
-    global prt
-    if len(msg) == 1:
-        msg = msg[0]
-        if isinstance(cf, dict):
-            try:
-                if cf["LOG"] == True:
-                    prt(msg)
-            except:
-                prt(msg)
-        elif cf == None:
-            prt(msg)
-        elif type(cf) == bool and cf:
-            prt(msg)
-    elif len(msg) > 1:
-        for m in msg:
-            if isinstance(cf, dict):
-                try:
-                    if cf["LOG"] == True:
-                        prt(m)
-                except:
-                    prt(m)
-            elif cf == None:
-                prt(m)
-            elif type(cf) == bool and cf:
-                prt(m)
-
-
-print = plog
-
-
-def dlog(*msg, cf=None):
-    if type(cf) == bool:
-        if cf:
-            for m in msg:
-                print(m)
-            return msg
-        else:
-            return None
-    elif type(cf) == dict:
-        if cf["DEBUG"]:
-            for m in msg:
-                print(m)
-            return msg
-        else:
-            return None
-    else:
-        return None
-
-
-def error(*msg, cf=None):
-    message = ""
-    for m in msg:
-        message += f"{m} "
-    message = message.strip()
-    if cf:
-        if cf["WINDOW"]:
-            cf["WINDOW"].write_event_value("POPUP", message)
-            cf["WINDOW"].write_event_value("ERROR", message)
-        elif cf["FORCE"]:
-            print(message)
-        else:
-            raise Exception(message)
-    else:
-        raise Exception(message)
-
-
-def popup(*msg, cf=None):
-    message = ""
-    for m in msg:
-        message += f"{m} "
-    message = message.strip()
-    if isinstance(cf, dict):
-        if cf["WINDOW"]:
-            cf["WINDOW"].write_event_value("POPUP", message)
-        else:
-            print(message)
-    elif cf != None: # if Window
-        cf.write_event_value("POPUP", message)
+console = Console()
+progress_bar = Progress(*Progress.get_default_columns(), MofNCompleteColumn())
+app = typer.Typer(help="Alacorder collects case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes.", no_args_is_help=True, pretty_exceptions_show_locals=False, add_completion=False)
+
+def write(output: dict, path: str, log: bool = False):
+    """
+    Write each value in {'name': pl.DataFrame} to path. (Supports .xls, .xlsx, .csv, .json, and .parquet)
+    """
+    def _write(output: dict, path: str):
+        if isinstance(output, pl.DataFrame): # convert to dict
+            if "AllPagesTextNoNewLine" in output.columns:
+                output = output.select(pl.exclude("AllPagesTextNoNewLine"))
+            output = {'table': output}
+        ext = os.path.splitext(path)[1]
+        assert ext in (".xlsx", ".xls") or len(output) == 1 # multitable export only to .xlsx/.xls files
+        assert ext in (".xlsx", ".xls", ".csv", ".json", ".parquet") # supported file extensions only
+        if ext in (".xlsx", ".xls"):
+            with xlsxwriter.Workbook(path) as workbook:
+                for o in output:
+                    output[o].write_excel(
+                        workbook=workbook,
+                        worksheet=o,
+                        autofit=True,
+                        float_precision=2
+                   )
+        if ext in (".parquet", ".json", ".csv"):
+            output = list(output.values())[0]
+            if ext == ".parquet":
+                output.write_parquet(path, compression="brotli")
+            if ext == ".json":
+                output.write_json(path),
+            if ext == ".csv":
+                output.write_csv(path)
+    if log:
+        with console.status("Writing to output path..."):
+            _write(output, path)
     else:
-        print(message)
-
-
-#   #   #   #            TABLE PARSERS           #   #   #   #
-
-
-def archive(cf):
-    """
-    Write a full text archive from inputs using configuration `cf`.
-    """
-    start = time.time()
-    a = read(cf)
-    write(a, cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-MA", True)
-    return a
-
-
-def multi(cf):
-    """
-    Start multitable collection using configuration object `cf`.
-    """
-    start = time.time()
-    df = read(cf)
-    print("Parsing case info...", cf=cf)
-    ca = _split_cases(df, debug=cf["DEBUG"])
-    print("Parsing charges...", cf=cf)
-    ac = _explode_charges(df, debug=cf["DEBUG"])
-    ch = _split_charges(ac, debug=cf["DEBUG"])
-    print("Parsing fees...", cf=cf)
-    af = _explode_fees(df, debug=cf["DEBUG"])
-    fs = _split_fees(af, debug=cf["DEBUG"])
-    print("Parsing financial history...", cf=cf)
-    fh = _explode_split_financial_history(df, debug=cf["DEBUG"])
-    print("Parsing sentences...", cf=cf)
-    sent = _explode_split_sentences(df, debug=cf["DEBUG"])
-    print("Parsing settings...", cf=cf)
-    settings = _explode_settings(df)
-    print("Parsing case action summaries...", cf=cf)
-    cas = _explode_case_action_summary(df)
-    print("Parsing witnesses...", cf=cf)
-    wit = _explode_witnesses(df)
-    print("Parsing attorneys...", cf=cf)
-    att = _explode_attorneys(df)
-    print("Parsing images...", cf=cf)
-    img = _explode_images(df)
-    dlog(ca, ch, fs, settings, cas, wit, att, img, cf=cf)
-    ch_filing = ch.filter(pl.col("Filing")).select(
-        pl.exclude("CourtAction", "CourtActionDate", "PaymentToRestore", "TotalBalance", "Filing", "Disposition", "CERVDisqConviction", "PardonDisqConviction", "PermanentDisqConviction", "Conviction")
-    )
-    ch_disposition = ch.filter(pl.col("Disposition")).select(
-        pl.exclude("Filing", "Disposition")
-    )
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(
-            [ca, ch_filing, ch_disposition, fs, fh, sent, settings, cas, wit, att, img],
-            sheet_names=[
-                "cases",
-                "filing-charges",
-                "disposition-charges",
-                "fees",
-                "financial-history",
-                "sentences",
-                "settings",
-                "case-action-summary",
-                "witnesses",
-                "attorneys",
-                "images",
-            ],
-            cf=cf,
-        )
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    out = {
-        "cases": ca,
-        "charges": ch,
-        "filing-charges": ch_filing,
-        "disposition-charges": ch_disposition,
-        "fees": fs,
-        "financial-history": fh,
-        "sentences": sent,
-        "settings": settings,
-        "case-action-summary": cas,
-        "witnesses": wit,
-        "attorneys": att,
-        "images": img,
-    }
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    return out
-
-
-def cases(cf):
-    """
-    Start cases table collection using configuration object `cf`.
-    """
-    start = time.time()
-    df = read(cf)
-    print("Parsing case info...", cf=cf)
-    ca = _split_cases(df)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...")
-        write(ca, cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return ca
-
-
-def charges(cf):
-    """
-    Start charges table collection using configuration object `cf`.
-    """
-    start = time.time()
-    df = read(cf)
-    print("Parsing charges...", cf=cf)
-    ac = _explode_charges(df)
-    ch = _split_charges(ac)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(ch, cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return ch
-
-
-def fees(cf):
-    """
-    Start fee sheet collection using configuration object `cf`.
-    """
-    start = time.time()
-    df = read(cf)
-    print("Parsing fee sheets...", cf=cf)
-    af = _explode_fees(df)
-    fs = _split_fees(af)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(fs, cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return fs
-
-
-def witnesses(cf):
-    """
-    Collect witnesses tables using configuration object `cf`.
-    """
-    start = time.time()
-    q = read(cf)
-    print("Parsing witnesses...", cf=cf)
-    out = _explode_witnesses(q)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(out, sheet_names=["witnesses"], cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
+        _write(output, path)
 
-
-def financial_history(cf):
-    """
-    Collect witnesses tables using configuration object `cf`.
-    """
-    start = time.time()
-    q = read(cf)
-    print("Parsing financial history...", cf=cf)
-    out = _explode_split_financial_history(q)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(out, sheet_names=["financial-history"], cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
-
-
-def sentences(cf):
-    """
-    Collect witnesses tables using configuration object `cf`.
-    """
-    start = time.time()
-    q = read(cf)
-    print("Parsing sentences...", cf=cf)
-    out = _explode_split_sentences(q)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(out, sheet_names=["sentences"], cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
-
-
-def cas(cf):
-    """
-    Collect case action summaries using configuration object `cf`.
-    """
-    start = time.time()
-    print("Parsing case action summaries...", cf=cf)
-    q = read(cf["QUEUE"])
-    out = _explode_case_action_summary(q)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(out, sheet_names=["case-action-summary"], cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
-
-
-def attorneys(cf):
-    """
-    Collect attorneys tables using configuration object `cf`.
-    """
-    start = time.time()
-    q = read(cf)
-    print("Parsing attorneys...", cf=cf)
-    out = _explode_attorneys(q)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(out, sheet_names=["attorneys"], cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
-
-
-def settings(cf):
-    """
-    Collect settings tables using configuration object `cf`.
-    """
-    start = time.time()
-    q = read(cf)
-    out = _explode_settings(q)
-    print("Parsing settings...", cf=cf)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(out, sheet_names=["settings"], cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
-
-
-def images(cf):
-    """
-    Collect images tables using configuration object `cf`.
-    """
-    start = time.time()
-    q = read(cf)
-    print("Parsing images...", cf=cf)
-    out = _explode_images(q)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(out, sheet_names=["images"], cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
-
-
-def vrr_summary(cf):
-    """
-    Summarize voting rights status from pairs using configuration object `cf`.
-    """
-    start = time.time()
-    print("Creating voting rights summary...", cf=cf)
-    if not cf["NO_WRITE"] and cf["OUTPUT_PATH"] != None:
-        if os.path.splitext(cf["OUTPUT_PATH"])[1] in (".xls",".xlsx",".json",".parquet",".csv"):
-            if os.path.isfile(cf["OUTPUT_PATH"]) and not cf["OVERWRITE"]:
-                error("File already exists! Repeat in overwrite mode.")
-            vrr = _vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], cf["OUTPUT_PATH"], cf["WINDOW"])
-        else:
-            error("File extension not supported!")
-    if cf["NO_WRITE"] or cf["OUTPUT_PATH"] == None:
-        vrr = _vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], None, cf['WINDOW'])
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
-    return vrr
-
-
-#   #   #   #         CONFIGURATION & I/O        #   #   #   #
-
-
-def set(
-    inputs,
-    outputs=None,
-    count=0,
-    table="",
-    archive=False,
-    log=False,
-    no_prompt=True,
-    debug=False,
-    overwrite=False,
-    no_write=False,
-    fetch=False,
-    cID="",
-    uID="",
-    pwd="",
-    criminal_only=False,
-    pairs=None,
-    vrr_summary=False,
-    append=False,
-    window=None,
-    force=False,
-    no_update=False,
-    now=False,
-):
-    """
-    Check inputs and outputs and return a configuration object for Alacorder table parser functions to receive as parameter and complete task, or set `now = True` to run immediately.
-
-    Args:
-        inputs (Path | DataFrame): PDF directory, query, archive path, or DataFrame input
-        outputs (Path | DataFrame, optional): Path to archive, directory, or file output
-        count (int, optional): Max cases to pull from input
-        table (str, optional): Table (all, cases, fees, financial-history, charges, sentences, settings, witnesses, attorneys, case_action_summaries, images)
-        archive (bool, optional): Write a full text archive from a directory of case detail PDFs
-        log (bool, optional): Print logs and progress to console
-        no_prompt (bool, optional): Skip user input / confirmation prompts
-        debug (bool, optional): Print verbose logs to console for developers
-        overwrite (bool, optional): Overwrite existing files at output path
-        no_write (bool, optional): Do not export to output path
-        fetch (bool, optional): Retrieve case detail PDFs from Alacourt.com
-        cID (str, optional): Customer ID on Alacourt.com
-        uID (str, optional): User ID on Alacourt.com
-        pwd (str, optional): Password on Alacourt.com
-        criminal_only (bool, optional): Only fetch criminal cases
-        pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
-        vrr_summary (bool, optional): Create voting rights summary from pairs
-        append (bool, optional): Append one archive to another
-        window (None, optional): PySimpleGUI window element
-        force (bool, optional): Do not raise exceptions
-        no_update (bool, optional): Do not mark input query when fetching cases
-        now (bool, optional): Start Alacorder upon successful configuration
-    """
-    return cf(
-        inputs=inputs,
-        outputs=outputs,
-        count=count,
-        table=table,
-        archive=archive,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-        overwrite=overwrite,
-        no_write=no_write,
-        fetch=fetch,
-        cID=cID,
-        uID=uID,
-        pwd=pwd,
-        criminal_only=criminal_only,
-        pairs=pairs,
-        vrr_summary=vrr_summary,
-        append=append,
-        window=window,
-        force=force,
-        no_update=no_update,
-        now=now,
-    )
-
-
-def cf(
-    inputs,
-    outputs=None,
-    count=0,
-    table="",
-    archive=False,
-    log=False,
-    no_prompt=True,
-    debug=False,
-    overwrite=False,
-    no_write=False,
-    fetch=False,
-    cID="",
-    uID="",
-    pwd="",
-    criminal_only=False,
-    pairs=None,
-    vrr_summary=False,
-    append=False,
-    window=None,
-    force=False,
-    no_update=False,
-    now=False,
-):
+def read(source, all_sheets=False):
     """
-    Check inputs and outputs and return a configuration object for Alacorder table parser functions to receive as parameter and complete task, or set `now = True` to run immediately.
-
-    Args:
-        inputs (Path | DataFrame): PDF directory, query, archive path, or DataFrame input
-        outputs (Path | DataFrame, optional): Path to archive, directory, or file output
-        count (int, optional): Max cases to pull from input
-        table (str, optional): Table (all, cases, fees, financial-history, charges, sentences, settings, witnesses, attorneys, case_action_summaries, images)
-        archive (bool, optional): Write a full text archive from a directory of case detail PDFs
-        log (bool, optional): Print logs and progress to console
-        no_prompt (bool, optional): Skip user input / confirmation prompts
-        debug (bool, optional): Print verbose logs to console for developers
-        overwrite (bool, optional): Overwrite existing files at output path
-        no_write (bool, optional): Do not export to output path
-        fetch (bool, optional): Retrieve case detail PDFs from Alacourt.com
-        cID (str, optional): Customer ID on Alacourt.com
-        uID (str, optional): User ID on Alacourt.com
-        pwd (str, optional): Password on Alacourt.com
-        criminal_only (bool, optional): Only fetch criminal cases
-        pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
-        vrr_summary (bool, optional): Create voting rights summary from pairs
-        append (bool, optional): Append one archive to another
-        window (None, optional): PySimpleGUI Window element
-        force (bool, optional): Do not raise exceptions
-        no_update (bool, optional): Do not mark input query when fetching cases
-        now (bool, optional): Start Alacorder upon successful configuration
+    Read input into pl.DataFrame. If directory, reads PDFs into archive df. 
     """
-    good = True
-    outputs = None if no_write else outputs
-    no_write = True if outputs == None else no_write
-    found = 0
-
-    if debug:
-        sys.tracebacklimit = 10
-        pl.Config.set_verbose(True)
-        pl.Config.set_tbl_rows(100)
-    else:
-        sys.tracebacklimit = 0
-        pl.Config.set_verbose(False)
-
-    # raise overwrite error
-    if no_write:
-        outputext = "none"
-        existing_output = False
-    elif os.path.isdir(outputs):
-        outputext = "directory"
-        existing_output = False
-    elif os.path.isfile(outputs):
-        if not overwrite and not append:
-            error(
-                "Existing file at output path. Repeat in overwrite mode.",
-                cf={"WINDOW": window, "FORCE": force},
-            )
-        outputext = os.path.splitext(outputs)[1]
-        existing_output = True
-    else:
-        outputext = os.path.splitext(str(outputs))[1]
-        existing_output = False
-
-    support_multitable = True if outputext in (".xls", ".xlsx", "none") else False
-    support_singletable = (
-        True
-        if outputext in (".xls", ".xlsx", "none", ".json", ".parquet", ".csv")
-        else False
-    )
-    support_archive = (
-        True
-        if outputext in (".xls", ".xlsx", ".csv", ".parquet", ".json", "none")
-        else False
-    )
-    if force not in (  # raise file extension not supported
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".parquet",
-        ".json",
-        ".csv",
-        "none",
-        "directory",
-    ) and outputext not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".parquet",
-        ".json",
-        ".csv",
-        "none",
-        "directory",
-    ):
-        error(
-            "File extension not supported.\nRepeat with .xls, .xlsx, .parquet, .csv, or .json.",
-            cf={"WINDOW": window, "FORCE": force},
-        )
-
-    if (  # raise no table selection
-        support_multitable == False
-        and archive == False
-        and fetch == False
-        and vrr_summary == False
-        and table
-        not in (
-            "cases",
-            "charges",
-            "fees",
-            "financial-history",
-            "history",
-            "disposition",
-            "disposition-charges",
-            "filing",
-            "filing-charges",
-            "attorneys",
-            "sentences",
-            "settings",
-            "images",
-            "case-action-summary",
-            "witnesses",
-        )
-    ):
-        error(
-            "Single table export choice required! (cases, charges, fees, financial-history, disposition, filing, sentences, settings, attorneys, images, case-action-summary, witnesses)",
-            cf={"WINDOW": window, "FORCE": force},
-        )
-
-    if archive and append and existing_output and not no_write:  # raise append failure
+    def extract_text(path) -> str:
+        """
+        From path, return full text of PDF as string (PyMuPdf engine required!)
+        """
         try:
-            old_archive = read(outputs)
+            doc = fitz.open(path)
         except:
-            error(
-                "Append failed! Archive at output path could not be read.",
-                cf={"WINDOW": window, "FORCE": force},
-            )
-
-    if isinstance(inputs, pl.dataframe.frame.DataFrame):  # DataFrame inputs
-        if not force and not "AllPagesText" in inputs.columns:
-            error(
-                "Alacorder could not read archive. Try again with another file.",
-                cf={"WINDOW": window, "FORCE": force},
-            )
-        elif not force and not "ALABAMA" in inputs["AllPagesText"][0]:
-            error(
-                "Alacorder could not read archive. Try again with another file.",
-                cf={"WINDOW": window, "FORCE": force},
-            )
-        queue = inputs
-        found = queue.shape[0]
-        is_full_text = True
-        itype = "object"
-    elif isinstance(inputs, pl.series.series.Series):  # series input
-        if not force and not "AllPagesText" in pl.DataFrame(inputs).columns:
-            error(
-                "Alacorder could not read archive. Try again with another file.",
-                cf={"WINDOW": window, "FORCE": force},
-            )
-        elif not force and not "ALABAMA" in inputs[0]:
-            error(
-                "Alacorder could not read archive. Try again with another file.",
-                cf={"WINDOW": window, "FORCE": force},
-            )
-        queue = inputs
-        found = queue.shape[0]
-        is_full_text = True
-        itype = "object"
-    elif os.path.isdir(inputs):  # directory inputs
-        queue = glob.glob(inputs + "**/*.pdf", recursive=True)
-        found = len(queue)
-        if not force and not found > 0:
-            error("No cases found in archive.", cf={"WINDOW": window, "FORCE": force})
-        is_full_text = False
-        itype = "directory"
-    elif os.path.isfile(inputs):  # file inputs
-        queue = read(inputs)
-        found = queue.shape[0]
-        is_full_text = True
-        itype = (
-            "query" if os.path.splitext(inputs)[1] in (".xls", ".xlsx") else "archive"
-        )
-    else:
-        error("Failed to determine input type.", cf={"WINDOW": window, "FORCE": force})
-
-    if count == 0:
-        count = found
-    if count > found:
-        count = found
-    if found > count:
-        if isinstance(queue, pl.dataframe.frame.DataFrame):
-            queue = queue.sample(count)
-        elif isinstance(queue, list):
-            queue = sample(queue, count)
-
-    out = {
-        "QUEUE": queue,
-        "INPUTS": inputs,
-        "NEEDTEXT": bool(not is_full_text),
-        "INPUT_TYPE": itype,
-        "FOUND": found,
-        "COUNT": count,
-        "OUTPUT_PATH": outputs,
-        "OUTPUT_EXT": outputext,
-        "SUPPORT_MULTITABLE": support_multitable,
-        "SUPPORT_SINGLETABLE": support_singletable,
-        "SUPPORT_ARCHIVE": support_archive,
-        "TABLE": table,
-        "ARCHIVE": archive,
-        "PAIRS": pairs,
-        "VRR_SUMMARY": vrr_summary,
-        "APPEND": append,
-        "NO_UPDATE": no_update,
-        "FETCH": fetch,
-        "ALA_CUSTOMER_ID": cID,
-        "ALA_USER_ID": uID,
-        "ALA_PASSWORD": pwd,
-        "CRIMINAL_ONLY": criminal_only,
-        "LOG": log,
-        "NO_WRITE": no_write,
-        "NO_PROMPT": no_prompt,
-        "OVERWRITE": overwrite,
-        "EXISTING_OUTPUT": existing_output,
-        "DEBUG": debug,
-        "WINDOW": window,
-    }
-    dlog(out, cf=debug)
-    if now:
-        return init(out)
-    return out
-
-
-def read(cf):
-    """
-    Read `cf` input PDF directory or case text archive into memory.
-    """
-    if isinstance(cf, pl.dataframe.frame.DataFrame):  # df input
-        df = cf
-        if "AllPagesTextNoNewLine" not in df.columns and "AllPagesText" in df.columns:
+            return ""
+        text = ""
+        for pg in doc:
             try:
-                df = df.with_columns(
-                    pl.col("AllPagesText")
-                    .str.replace_all(r"\n", " ")
-                    .alias("AllPagesTextNoNewLine")
+                text += " \n ".join(
+                    x[4].replace("\n", " ") for x in pg.get_text(option="blocks")
                 )
             except:
                 pass
-            return df
-        else:
-            return df
-    elif isinstance(cf, list):  # [paths] input
-        queue = cf
-        aptxt = []
-        for pp in queue:
-            aptxt += [extract_text(pp)]
-        archive = pl.DataFrame(
-            {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
-        )
-        archive = archive.with_columns(
-            pl.col("AllPagesText")
-            .str.replace_all(r"\n", " ")
-            .alias("AllPagesTextNoNewLine")
-        )
-        return archive
-    elif isinstance(cf, dict):  # cf input
-        if cf["NEEDTEXT"] == False or "ALABAMA" in cf["QUEUE"][0]:
-            return cf["QUEUE"]
-        if cf["NEEDTEXT"] == True:
-            queue = cf["QUEUE"]
-            aptxt = []
-            print("Extracting text...", cf=cf)
-            if cf["WINDOW"]:
-                cf["WINDOW"].write_event_value("PROGRESS_TOTAL", len(queue))
-                for i, pp in enumerate(queue):
-                    aptxt += [extract_text(pp)]
-                    cf["WINDOW"].write_event_value("PROGRESS", i + 1)
-            elif cf["LOG"]:
-                for pp in tqdm(queue):
-                    aptxt += [extract_text(pp)]
-            else:
-                for pp in queue:
-                    aptxt += [extract_text(pp)]
-        archive = pl.DataFrame(
-            {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
-        )
-        archive = archive.with_columns(
-            pl.col("AllPagesText")
-            .str.replace_all(r"\n", " ")
-            .alias("AllPagesTextNoNewLine")
-        )
-        return archive
-    elif os.path.isdir(cf):  # directory path input
-        queue = glob.glob(cf + "**/*.pdf", recursive=True)
-        aptxt = []
-        print("Extracting text...", cf=cf)
-        if cf["WINDOW"]:
-            cf["WINDOW"].write_event_value("PROGRESS_TOTAL", len(queue))
-            for i, pp in enumerate(queue):
-                aptxt += [extract_text(pp)]
-                cf["WINDOW"].write_event_value("PROGRESS", i + 1)
-        elif cf["LOG"]:
-            for pp in tqdm(queue):
-                aptxt += [extract_text(pp)]
+        text = re.sub(r"(<image\:.+?>)", "", text).strip()
+        return text
+    if isinstance(source, str):
+        source = os.path.abspath(source)
+        if os.path.isfile(source):
+            ext = os.path.splitext(source)[1]
+            if ext in (".xls", ".xlsx"):
+                if all_sheets:
+                    output = pl.read_excel(
+                        source, 
+                        sheet_id=0,
+                        xlsx2csv_options={"ignore_errors": True},
+                        read_csv_options={"ignore_errors": True}
+                    )
+                else:
+                    output = pl.read_excel(
+                        source, 
+                        xlsx2csv_options={"ignore_errors": True},
+                        read_csv_options={"ignore_errors": True}
+                    )
+            if ext == ".json":
+                output = pl.read_json(source)
+            if ext == ".csv":
+                output = pl.read_csv(source, ignore_errors=True)
+            if ext == ".parquet":
+                output = pl.read_parquet(source)
+            if ext == ".txt":
+                with open(source) as file:
+                    output = file.read()
+            if ext == ".pdf":
+                output = extract_text(source)
+        if os.path.isdir(source):
+            paths = glob.glob(source + "**/*.pdf", recursive=True)
+            all_text = []
+            with progress_bar as p:
+                for path in p.track(paths, description="Reading PDFs..."):
+                    all_text += [extract_text(path)]
+            output = pl.DataFrame({
+                "Timestamp": time.time(),
+                "AllPagesText": all_text,
+                "Path": paths
+            })
+    if isinstance(source, list):
+        all_text = []
+        with progress_bar as p:
+            for path in p.track(source, description="Reading PDFs..."):
+                all_text += [extract_text(path)]
+        output = pl.DataFrame({
+            "Timestamp": time.time(),
+            "AllPagesText": all_text,
+            "Path": paths
+        })
+    if isinstance(source, pl.DataFrame):
+        output = source
+    if isinstance(output, pl.DataFrame):
+        if "CaseNumber" not in output.columns and "AllPagesText" in output.columns:
+            output = output.with_columns(
+                pl.concat_str(
+                    [
+                        pl.col("AllPagesText").str.extract(
+                            r"(County: )(\d{2})", group_index=2
+                        ),
+                        pl.lit("-"),
+                        pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                    ]
+                ).alias("CaseNumber")
+            )
+        if "AllPagesTextNoNewLine" not in output.columns and "AllPagesText" in output.columns:
+            output = output.with_columns(
+                pl.col("AllPagesText").str.replace_all(r"\n"," ").alias("AllPagesTextNoNewLine")
+            )
+    return output
+
+class AlacourtDriver():
+    
+    # config
+    def __init__(self, dirpath=None, headless=True):
+        opt = webdriver.ChromeOptions()
+        if headless:
+            opt.add_argument("--headless=new")
+        if dirpath != None:
+            opt.add_experimental_option(
+                "prefs",
+                {
+                    "download.default_directory": os.path.abspath(dirpath),
+                    "download.prompt_for_download": False,
+                    "download.directory_upgrade": True,
+                    "plugins.always_open_pdf_externally": True
+                }
+            )
         else:
-            for pp in queue:
-                aptxt += [extract_text(pp)]
-        archive = pl.DataFrame(
-            {"Timestamp": time.time(), "AllPagesText": aptxt, "Path": queue}
-        )
-        archive = archive.with_columns(
-            pl.col("AllPagesText")
-            .str.replace_all(r"\n", " ")
-            .alias("AllPagesTextNoNewLine")
-        )
-        return archive
-    elif os.path.isfile(cf):  # file path input
-        ext = os.path.splitext(cf)[1]
-        if ext in (".xls", ".xlsx"):
-            archive = pl.read_excel(
-                cf,
-                xlsx2csv_options={"ignore_errors": True},
-                read_csv_options={"ignore_errors": True},
+            opt.add_experimental_option(
+                "prefs",
+                {
+                    "download.prompt_for_download": False,
+                    "download.directory_upgrade": True,
+                    "plugins.always_open_pdf_externally": True
+                }
             )
-            return archive
-        elif ext == ".json":
-            archive = pl.read_json(cf)
-            if "AllPagesText" in archive.columns:
-                archive = archive.with_columns(
-                    pl.col("AllPagesText")
-                    .str.replace_all(r"\n", " ")
-                    .alias("AllPagesTextNoNewLine")
+        if dirpath != None:
+            self.dirpath = os.path.abspath(dirpath)
+        else:
+            self.dirpath = None
+        self.headless = headless
+        with console.status("Starting WebDriver (requires Google Chrome)..."):
+            self.driver = webdriver.Chrome(options=opt)
+        self.queue = None
+        self.case_number_queue = None
+        self.output = None
+    
+    def login(self, cID, uID, pwd) -> None:
+        """
+        Login to Alacourt using provided credentials.
+        """
+        with console.status("Logging in to Alacourt..."):
+            self.driver.get("https://v2.alacourt.com")
+            cID_box = self.driver.find_element(by=By.ID, value="ContentPlaceHolder_txtCusid")
+            uID_box = self.driver.find_element(by=By.ID, value="ContentPlaceHolder_txtUserId")
+            pwd_box = self.driver.find_element(by=By.ID, value="ContentPlaceHolder_txtPassword")
+            login_button = self.driver.find_element(by=By.ID, value="ContentPlaceHolder_btLogin")
+            cID_box.send_keys(cID)
+            uID_box.send_keys(uID)
+            pwd_box.send_keys(pwd)
+            login_button.click()
+            continue_button = self.driver.find_elements(by=By.ID, value="ContentPlaceHolder_btnContinueLogin")
+            if len(continue_button) > 0:
+                continue_button[0].click()
+            try:
+                WebDriverWait(self.driver, 5).until(EC.visibility_of_element_located((By.ID, "btnLogOff")))
+                return True
+            except:
+                raise Exception("Invalid Alacourt credentials.")
+    
+    # party search
+    def set_party_search_queue(self, queue) -> None:
+        """
+        Set path to Party Search queue spreadsheet.
+        """
+        if isinstance(queue, pl.DataFrame):
+            self.queue_path = None
+            self.queue = queue
+        if isinstance(queue, str):
+            if os.path.isfile(queue):
+                self.queue_path = queue
+                self.queue = read(queue)
+            else:
+                raise Exception("Could not read input.")
+        for col in ["Retrieved", "Timestamp", "Case Count"]:
+            if col not in self.queue.columns:
+                self.queue = self.queue.with_columns(
+                    pl.lit("").alias(col)
                 )
-            return archive
-        elif ext == ".csv":
-            archive = pl.read_csv(cf, ignore_errors=True)
-            if "AllPagesText" in archive.columns:
-                archive = archive.with_columns(
-                    pl.col("AllPagesText")
-                    .str.replace_all(r"\n", " ")
-                    .alias("AllPagesTextNoNewLine")
+        pscols = ["NAME", "PARTY_TYPE", "SSN", "DOB", "COUNTY", "DIVISION", "CASE_YEAR", "NO_RECORDS", "FILED_BEFORE", "FILED_AFTER"]
+        col_dict = {}
+        for col in self.queue.columns:
+            d = {re.sub(" ", "_", col.upper()): col}
+            col_dict.update(d)
+        for key in col_dict:
+            if key in pscols:
+                self.queue = self.queue.with_columns(
+                    pl.col(col_dict[key]).alias("TEMP_" + key)
                 )
-            return archive
-        elif ext == ".parquet":
-            archive = pl.read_parquet(cf)
-            if "AllPagesText" in archive.columns:
-                archive = archive.with_columns(
-                    pl.col("AllPagesText")
-                    .str.replace_all(r"\n", " ")
-                    .alias("AllPagesTextNoNewLine")
+        temp_pscols = ["TEMP_" + col for col in pscols]
+        for col in temp_pscols:
+            if col not in self.queue.columns:
+                self.queue = self.queue.with_columns(
+                    pl.lit("").alias(col)
                 )
-            return archive
-        elif ext == ".txt":
-            with open(cf) as f:
-                text = f.read()
-            return text
-        elif ext == ".pdf":
-            text = extract_text(cf)
-            return text
-    else:
-        error("Could not read input.")
-
-
-def write(outputs, sheet_names=[], cf=None, path=None, overwrite=False):
-    """Write `outputs` to output path at `cf['OUTPUT_PATH']` or `path`.
-
-    Args:
-        outputs ([DataFrame]): DataFrame(s) to write to output
-        sheet_names (List[str], optional): Output Excel worksheet names
-
-        cf (dict): Configuration object
+        for col in self.queue.columns:
+            self.queue = self.queue.with_columns(
+                pl.when(pl.col(col)==None).then('').otherwise(pl.col(col)).alias(col)
+            )
+    
+    def set_party_search_output(self, output_path) -> None:
+        """
+        Set path to Party Search output spreadsheet.
+        """
+        self.output = output_path
+    
+    def party_search(self, name='', party_type='', ssn='', dob='', county='', division='', case_year='', filed_before='', filed_after='', no_records = '', criminal_only=False) -> None:
+        """
+        Alacourt Party Search with fields provided.
+        """
+        self.driver.implicitly_wait(10)
+        try:
+            if "frmIndexSearchForm" not in self.driver.current_url:
+                self.driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
+        except:
+            self.driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
 
-        or:
-            path (str): Output path
-            overwrite (bool): Allow overwrite
-    """
-    if cf == None:
-        cf = {
-            "OUTPUT_PATH": path,
-            "OUTPUT_EXT": os.path.splitext(path)[1],
-            "NO_WRITE": False,
-            "OVERWRITE": True,
-            "FORCE": False,
-        }
-    else:  # cf trumps params if both given
-        path = cf["OUTPUT_PATH"]
-        overwrite = cf["OVERWRITE"]
-    if isinstance(outputs, list):
-        if len(outputs) != len(sheet_names) and len(outputs) != 1:
-            error(
-                "alac.write() missing sheet_names parameter. See documentation for details.",
-                cf=cf,
-            )
-    if isinstance(outputs, pl.dataframe.frame.DataFrame):  # df input
-        if "AllPagesTextNoNewLine" in outputs.columns:
-            outputs = outputs.select(pl.exclude("AllPagesTextNoNewLine"))
-    if cf["NO_WRITE"] == True:
-        return outputs
-    elif not cf["OVERWRITE"] and os.path.isfile(cf["OUTPUT_PATH"]):
-        error(
-            "Could not write to output path because overwrite mode is not enabled.",
-            cf=cf,
-        )
-    elif cf["OUTPUT_EXT"] in (".xlsx", ".xls"):
-        with xlsxwriter.Workbook(cf["OUTPUT_PATH"]) as workbook:
-            if not isinstance(outputs, list):
-                outputs = [outputs]
-            if len(sheet_names) > 0:
-                for i, x in enumerate(outputs):
-                    x.write_excel(
-                        workbook=workbook,
-                        worksheet=sheet_names[i],
-                        autofit=True,
-                        float_precision=2,
+        if "frmlogin" in self.driver.current_url:
+            raise Exception("Must be logged into Alacourt before party searching.")
+        
+        # locators
+        party_name_box = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")
+        ssn_box = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN")
+        dob_box = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtDOB")
+        plaintiffs_pt_select = self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_rdlPartyType_0")
+        defendants_pt_select = self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_rdlPartyType_1")
+        all_pt_select = self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_rdlPartyType_2")
+        division_select = Select(self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_UcddlDivisions1_ddlDivision"))
+        county_select = Select(self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_ddlCounties"))
+        case_year_select = Select(self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear"))
+        no_records_select = Select(self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfRecords"))
+        filed_before_box = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtFrom")
+        filed_after_box = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtTo")
+        search_button = self.driver.find_element(by=By.ID, value="searchButton")
+        
+        # set fields
+        if name != "":
+            party_name_box.send_keys(name)
+        if ssn != "":
+            ssn_box.send_keys(ssn)
+        if dob != "":
+            dob_box.send_keys(dob)
+        if party_type == "Plaintiffs":
+            plaintiffs_pt_select.click()
+        if party_type == "Defendants":
+            defendants_pt_select.click()
+        if party_type == "ALL":
+            all_pt_select.click()
+        if division == "" and not criminal_only:
+            division = "All Divisions"
+        if criminal_only:
+            division = "Criminal Only"
+        division_select.select_by_visible_text(division)
+        if county != "":
+            county_select.select_by_visible_text(county)
+        if case_year != "":
+            case_year_select.select_by_visible_text(str(case_year))
+        if filed_before != "":
+            filed_before_box.send_keys(filed_before)
+        if filed_after != "":
+            filed_after_box.send_keys(filed_after)
+        if no_records != "":
+            no_records_select.select_by_visible_text(str(no_records))
+        else:
+            no_records_select.select_by_visible_text('1000')
+        
+        # submit
+        search_button.click()
+        
+        # wait for table
+        WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.ID, "ContentPlaceHolder1_dg")))
+                    
+    def read_results_page(self) -> pl.DataFrame:
+        """
+        Read current Party Search results page.
+        """
+        if "frmIndexSearchList" not in self.driver.current_url:
+            raise Exception("Try again on party search results page.")    
+        soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+        table = soup.find("table", {"id": "ContentPlaceHolder1_dg"})
+        rows = table.find_all("tr")
+        rows_text = []
+        clean_rows = []
+        for row in rows:
+            cells = row.find_all("td")
+            cells = [cell.text for cell in cells]
+            rows_text += [cells]
+        for row in rows_text:
+            if len(row) > 10:
+                clean_rows += [row]
+        df = pl.DataFrame({'Row': clean_rows})
+        if df.shape[0] > 0:
+            df = df.select([
+                pl.col("Row").list.get(0).alias("County"),
+                pl.col("Row").list.get(16).alias("CaseNumber"),
+                pl.col("Row").list.get(6).alias("Name"), 
+                pl.col("Row").list.get(7).alias("JID"), 
+                pl.col("Row").list.get(8).alias("OriginalCharge"),
+                pl.col("Row").list.get(9).alias("Bond"),
+                pl.col("Row").list.get(10).alias("DOB"),
+                pl.col("Row").list.get(11).alias("Sex"),
+                pl.col("Row").list.get(12).alias("Race"),
+                pl.col("Row").list.get(13).alias("CourtActionDate"),
+                pl.col("Row").list.get(15).alias("SSN"),
+            ])
+        else:
+            return pl.DataFrame()
+        df = df.filter(pl.col("CaseNumber").is_null().is_not())
+        return df
+    
+    def read_all_results(self) -> pl.DataFrame:
+        """
+        Read all current Party Search results pages.
+        """
+        soup = BeautifulSoup(self.driver.page_source, 'html.parser')  
+        try:
+            total_pages = int(soup.find("td", {"id": "ContentPlaceHolder1_dg_tcPageXofY"}).text.split()[-1])
+        except:
+            total_pages = 1
+        df = self.read_results_page()
+        for i in range(2, total_pages + 1):
+            table = self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_dg")
+            page_select = Select(self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_dg_ddlPages"))
+            page_select.select_by_visible_text(str(i))
+            WebDriverWait(self.driver, 10).until(EC.staleness_of(table))
+            table = self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_dg")
+            df = pl.concat([df, self.read_results_page()])
+        return df   
+    
+    def start_party_search_queue(self, queue=None, output_path=None, criminal_only=False) -> pl.DataFrame:
+        """
+        From `queue`, conduct Party Search and record results tables to `output_path`.
+        """
+        if isinstance(queue, pl.DataFrame) or isinstance(queue, str):
+            self.set_party_search_queue(queue)
+        elif self.queue == None:
+            raise Exception("Must set queue to start.")
+        if output_path != None:
+            self.set_party_search_output(output_path)
+        try:
+            results_df = read(self.output)
+            for col in results_df.columns:
+                results_df = results_df.with_columns(
+                    pl.col(col).cast(pl.Utf8)
+                )
+            print("Appending to existing table at output path.")
+        except:
+            results_df = pl.DataFrame()
+        with progress_bar as p:
+            for i, r in enumerate(p.track(self.queue.rows(named=True), description="Party searching...")):
+                if r['Retrieved'] in ('', None):
+                    self.party_search(
+                        name=r['TEMP_NAME'],
+                        party_type=r['TEMP_PARTY_TYPE'],
+                        ssn=r['TEMP_SSN'],
+                        dob=r['TEMP_DOB'],
+                        county=r['TEMP_COUNTY'],
+                        division=r['TEMP_DIVISION'],
+                        case_year=r['TEMP_CASE_YEAR'],
+                        filed_before=r['TEMP_FILED_BEFORE'],
+                        filed_after=r['TEMP_FILED_AFTER'],
+                        no_records=r['TEMP_NO_RECORDS'],
+                        criminal_only=criminal_only
                     )
-            else:
-                outputs[0].write_excel(
-                    workbook=workbook, autofit=True, float_precision=2
+                    df = self.read_all_results()
+                    df = df.with_columns(pl.lit(r['TEMP_NAME']).alias("Search"))
+                    for col in ["Retrieved", "Timestamp", "Destination"]:
+                        if col in results_df.columns:
+                            df = df.with_columns(pl.lit('').alias(col))
+                    if df.shape[0] > 1:
+                        results_df = pl.concat([results_df, df])
+                    self.queue[i, 'Retrieved'] = "Y"
+                    self.queue[i, 'Case Count'] = df.shape[0]
+                    self.queue[i, 'Timestamp'] = time.time()
+                    if self.queue_path != None and i % 10 == 0:
+                        write_queue = self.queue.select(pl.exclude("TEMP_NAME", "TEMP_PARTY_TYPE", "TEMP_SSN", "TEMP_DOB", "TEMP_COUNTY", "TEMP_DIVISION", "TEMP_CASE_YEAR", "TEMP_FILED_BEFORE", "TEMP_FILED_AFTER", "TEMP_NO_RECORDS"))
+                        write({'queue': write_queue}, self.queue_path)
+                    if self.output != None and i % 10 == 0:
+                        write({'results': results_df}, self.output)
+            if self.queue_path != None:
+                write_queue = self.queue.select(pl.exclude("TEMP_NAME", "TEMP_PARTY_TYPE", "TEMP_SSN", "TEMP_DOB", "TEMP_COUNTY", "TEMP_DIVISION", "TEMP_CASE_YEAR", "TEMP_FILED_BEFORE", "TEMP_FILED_AFTER", "TEMP_NO_RECORDS"))
+                write({'queue': write_queue}, self.queue_path)
+            if self.output != None:
+                write({'results': results_df}, self.output)
+        return results_df
+    
+    # case number search
+    def set_case_number_queue(self, queue) -> None:
+        """
+        Set case number queue.
+        """
+        if isinstance(queue, pl.DataFrame):
+            self.case_number_queue = queue
+        if isinstance(queue, str):
+            self.case_number_queue_path = queue
+            self.case_number_queue = read(queue)
+        for col in ["Retrieved", "Timestamp", "Destination"]:
+            if col not in self.case_number_queue.columns:
+                self.case_number_queue = self.case_number_queue.with_columns(
+                    pl.lit('').alias(col)
                 )
-    elif cf["OUTPUT_EXT"] == ".parquet":
-        outputs.write_parquet(cf["OUTPUT_PATH"], compression="brotli")
-    elif cf["OUTPUT_EXT"] == ".json":
-        outputs.write_json(cf["OUTPUT_PATH"])
-    elif cf["OUTPUT_EXT"] in (".csv", ".txt"):
-        outputs.write_csv(cf["OUTPUT_PATH"])
-    elif cf["OUTPUT_EXT"] not in ("none", "", "directory", None):
-        outputs.write_csv(cf["OUTPUT_PATH"])
-    else:
-        pass
-    return outputs
-
-
-def pairs(cf):
-    """
-    Create AIS / Unique ID pairs template using configuration object `cf`.
-    """
-    print("Creating empty pairs template...", cf=cf)
-    df = read(cf)
-    tp = _make_pairs_template(df)
-    if not cf["NO_WRITE"]:
-        print("Writing to output path...", cf=cf)
-        write(
-            tp, sheet_names=["Pairs"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
-        )
-    print("Created template successfully.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("MT-COMPLETE", True)
-    return tp
-
-
-def init(cf):
-    """
-    Start Alacorder using configuration object `cf`.
-    """
-    if cf["FETCH"] == True:
-        ft = fetch(cf=cf)
-        return ft
-    elif cf["ARCHIVE"] == True:
-        ar = archive(cf)
-        return ar
-    elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
-        vr = vrr_summary(cf)
-        return vr
-    elif (
-        cf["TABLE"].lower() in ("charges", "disposition", "filing")
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        ch = charges(cf)
-        return ch
-    elif cf["TABLE"].lower() in ("cases", "caseinfo") and cf["SUPPORT_SINGLETABLE"]:
-        ca = cases(cf)
-        return ca
-    elif (
-        cf["TABLE"].lower() in ("fees", "feesheet", "fines")
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        fs = fees(cf)
-        return fs
-    elif cf["TABLE"].lower() in ("financial-history", "history"):
-        fh = financial_history(cf)
-        return fh
-    elif cf["TABLE"].lower() in ("witnesses", "witness") and cf["SUPPORT_SINGLETABLE"]:
-        out = witnesses(cf)
-        return out
-    elif (
-        cf["TABLE"].lower()
-        in (
-            "case-action-summary",
-            "cas",
-        )
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        out = cas(cf)
-        return out
-    elif cf["TABLE"].lower() in ("settings", "set") and cf["SUPPORT_SINGLETABLE"]:
-        out = settings(cf)
-        return out
-    elif cf["TABLE"].lower() == "sentences":
-        sent = sentences(cf)
-        return sent
-    elif cf["TABLE"].lower() in ("images", "imgs", "img") and cf["SUPPORT_SINGLETABLE"]:
-        out = images(cf)
-        return out
-    elif cf["TABLE"] in ("attorneys", "att") and cf["SUPPORT_SINGLETABLE"]:
-        out = attorneys(cf)
-        return out
-    elif (
-        cf["TABLE"].lower() in ("all", "", "multi", "multitable")
-        and cf["SUPPORT_MULTITABLE"]
-    ):
-        mult = multi(cf)
-        return mult
-    else:
-        print("Job not specified. Select a mode and reconfigure to start.")
-        return None
-
-
-#   #   #   #        PRIVATE / INTERNALS         #   #   #   #
+        if "CaseNumber" not in self.case_number_queue.columns and "Case Number" in self.case_number_queue.columns:
+            self.case_number_queue = self.case_number_queue.with_columns(pl.col("Case Number").alias("CaseNumber"))
 
+    def case_number_search(self, case_number='', download=True) -> bool:
+        """
+        Use Alacourt Case Lookup to search for a case by number. If `download` is true, will also download case detail PDF. Returns False if case detail is unavailable.
+        """
+        self.driver.get("https://v2.alacourt.com/frmcaselookupform.aspx")
+
+        if "frmlogin" in self.driver.current_url:
+            raise Exception("Must be logged into Alacourt before fetching cases.")
+
+        county_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCounty")
+        division_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlDivision")
+        case_year_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear")
+        case_number_input = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtCaseNumber")
+        case_extension_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlExt")
+        number_of_cases_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfCases")
+        cmap = pl.DataFrame(
+                {
+                    'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+                    'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+                    'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+                }
+        )
+        dmap = pl.DataFrame({'Code': ['CC', 'CS', 'CV', 'DC', 'DR', 'DV', 'EQ', 'JU', 'MC', 'SM', 'TP', 'TR'], 'Selection': ['CC - CIRCUIT-CRIMINAL', 'CS - CHILD SUPPORT', 'CV - CIRCUIT-CIVIL', 'DC - DISTRICT-CRIMINAL', 'DR - DOMESTIC RELATIONS', 'DV - DISTRICT-CIVIL', 'EQ - EQUITY-CASES', 'JU - JUVENILE', 'MC - MUNICIPAL-CRIMINAL', 'SM - SMALL CLAIMS', 'TP - MUNICIPAL-PARKING', 'TR - TRAFFIC'] })
+        county_number = case_number[0:2]
+        division_code = case_number[3:5]
+        case_year = case_number[6:10]
+        six_digit = case_number[11:17]
+        if len(case_number) >= 20:
+            extension = case_number[18:20]
+        else:
+            extension = "00"
+        county = cmap.filter(pl.col("CountyNumber")==county_number).select("Selection").to_series()[0]
+        division = dmap.filter(pl.col("Code")==division_code).select("Selection").to_series()[0]
+        county_select.send_keys(county)
+        division_select.send_keys(division)
+        case_year_select.send_keys(case_year)
+        case_number_input.send_keys(six_digit)
+        search_button = self.driver.find_element(by=By.ID, value="searchButton")
+        search_button.click()
+        if download:
+            if "NoCaseDetails" in self.driver.current_url:
+                return False
+            else:
+                try:
+                    WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.ID, "ContentPlaceHolder1_lnkPrint")))
+                except:
+                    return False
+                self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_lnkPrint").click()
+                WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.ID, "divPrintCase")))
+                self.driver.find_element(by=By.ID, value="btnPrintCase").click()
+                return True
+
+    def start_case_number_queue(self, queue=None):
+        if isinstance(queue, pl.DataFrame) or isinstance(queue, str):
+            self.set_case_number_queue(queue)
+        elif self.case_number_queue == None:
+            raise Exception("Must set queue to start.")
+        with progress_bar as p:
+            for i, r in enumerate(p.track(self.case_number_queue.rows(named=True), description="Fetching cases...")):
+                if r['Retrieved'] in ('', None):
+                    if self.case_number_search(r['CaseNumber']):
+                        self.case_number_queue[i, 'Retrieved'] = "Y"
+                        self.case_number_queue[i, 'Timestamp'] = time.time()
+                        self.case_number_queue[i, 'Destination'] = self.dirpath
+                    else:
+                        self.case_number_queue[i, 'Retrieved'] = "PDF Not Available"
+                        self.case_number_queue[i, 'Timestamp'] = time.time()
+                    if self.case_number_queue_path != None and i % 10 == 0:
+                        write({'queue': self.case_number_queue}, self.case_number_queue_path)
+            if self.case_number_queue_path != None:
+                write({'queue': self.case_number_queue}, self.case_number_queue_path)
+
+class ADOCDriver():
+
+    def __init__(self, output_path=None, headless=True):
+        if output_path != None:
+            self.output = os.path.abspath(output_path)
+        opt = webdriver.ChromeOptions()
+        if headless:
+            opt.add_argument('--headless=new')
+        with console.status("Starting WebDriver (requires Google Chrome)..."):
+            self.driver = webdriver.Chrome(options=opt)
+        self.driver.get("https://doc.alabama.gov/inmatesearch")
+
+    def crawl(self, output_path=None) -> pl.DataFrame:
+        """
+        Collect all results in ADOC Inmate Search by searching last name by letter.
+        """
+        if output_path != None:
+            self.output = output_path
+        alphabet = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z"]
+        results = pl.DataFrame()
+        with progress_bar as p:
+            for letter in p.track(alphabet, description="Crawling ADOC..."):
+                self.driver.get("https://doc.alabama.gov/inmatesearch")
+                self.driver.find_element(by=By.ID, value="MainContent_txtLName").send_keys(letter)
+                self.driver.find_element(by=By.ID, value="MainContent_btnSearch").click()
+                WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.ID, "MainContent_gvInmateResults")))
+                soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+                try:
+                    total_pages = int(soup.find("span", {"id": "MainContent_gvInmateResults_lblPages"}).text)
+                except:
+                    total_pages = 1
+                for i in range(1, total_pages + 1):
+                    soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+                    table = soup.find("table", {"id": "MainContent_gvInmateResults"})
+                    rows = table.find_all("tr")
+                    rows_text = []
+                    for row in rows:
+                        cells = [cell.text for cell in row.find_all("td")]
+                        rows_text += [cells]
+                    df = pl.DataFrame({'Row': rows_text})
+                    df = df.filter(pl.col("Row").list.lengths() > 3)
+                    df = df.select([
+                        pl.col("Row").list.get(0).alias("AIS"),
+                        pl.col("Row").list.get(1).str.replace("\n","").alias("Name"),
+                        pl.col("Row").list.get(2).alias("Sex"),
+                        pl.col("Row").list.get(3).alias("Race"),
+                        pl.col("Row").list.get(4).cast(pl.Int64, strict=False).alias("BirthYear"),
+                        pl.col("Row").list.get(5).alias("Institution"),
+                        pl.col("Row").list.get(6).str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate"),
+                        pl.col("Row").list.get(7).alias("Code")
+                    ])
+                    results = pl.concat([results, df])
+                    table_selenium = self.driver.find_element(by=By.ID, value="MainContent_gvInmateResults")
+                    if total_pages > 1:
+                        self.driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext").click()
+                        WebDriverWait(self.driver, 10).until(EC.staleness_of(table_selenium))
+                if self.output not in (None, ''):
+                    write({'results': results}, self.output)
+        return results
+
+    def search(self, ais='', first_name='', last_name='') -> None:
+        """
+        Search ADOC Inmate Search with provided fields.
+        """
+        if self.driver.current_url != "https://doc.alabama.gov/InmateSearch":
+            self.driver.get("https://doc.alabama.gov/InmateSearch")
+        ais_box = self.driver.find_element(by=By.ID, value="MainContent_txtAIS")
+        first_name_box = self.driver.find_element(by=By.ID, value="MainContent_txtFName")
+        last_name_box = self.driver.find_element(by=By.ID, value="MainContent_txtLName")
+        search_button = self.driver.find_element(by=By.ID, value="MainContent_btnSearch")
+        ais_box.send_keys(ais)
+        first_name_box.send_keys(first_name)
+        last_name_box.send_keys(last_name)
+        search_button.click()
+        WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.ID, "MainContent_lblMessage")))
 
-def extract_text(path) -> str:
-    """
-    From path, return full text of PDF as string (PyMuPdf engine required!)
-    """
-    try:
-        doc = fitz.open(path)
-    except:
-        return ""
-    text = ""
-    for pg in doc:
+    def select_result(self, index=0) -> bool:
+        """
+        Select result at index from ADOC Inmate Search results table page.
+        Returns false if no result at index.
+        """
+        soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+        urls = soup.find_all("a", {"id": re.compile(r'MainContent_gvInmateResults_lnkInmateName_\d+')})
         try:
-            text += " \n ".join(
-                x[4].replace("\n", " ") for x in pg.get_text(option="blocks")
-            )
+            self.driver.find_element(by=By.ID, value=urls[index]['id']).click()
+            return True
         except:
-            pass
-    text = re.sub(r"(<image\:.+?>)", "", text).strip()
-    return text
-
+            return False
 
-def extract_text_pg_one(path) -> str:
-    """
-    From path, return text of first page of PDF as string (PyMuPdf engine required!)
-    """
-    try:
-        doc = fitz.open(path)
-    except:
-        return ""
-    text = " \n ".join(
-        x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
-    )
-    return text
-
-
-def append_archive(inpath="", outpath="", cf=None):
-    """
-    Append the contents of one archive to another.
-
-    Args:
-        inpath (str): Input archive
-        outpath (str): Output archive
-        cf (dict): Configuration object
-
-    Returns:
-        DataFrame: Appended archive object
-    """
-    if cf and inpath == "":
-        inpath = cf["INPUTS"]
-
-    if cf and outpath == "":
-        outpath = cf["OUTPUT_PATH"]
-
-    if not os.path.isfile(inpath) and not os.path.isfile(outpath):
-        error("Invalid path.", cf=cf)
-
-    inarc = read(inpath)
-    outarc = read(outpath)
-
-    try:
-        inarc = inarc.select("AllPagesText", "Path", "Timestamp")
-        outarc = outarc.select("AllPagesText", "Path", "Timestamp")
-    except:
+    def read_results_page(self) -> dict:
+        """
+        Read current Inmate History page from ADOC Inmate Search.
+        """
+        if "InmateHistory" not in self.driver.current_url:
+            return None
+        soup = BeautifulSoup(self.driver.page_source, 'html.parser')
+        # inmate details
+        name = soup.find("span", {"id": "MainContent_DetailsView2_Label1"}).text
+        ais = soup.find("span", {"id": "MainContent_DetailsView2_Label2"}).text
+        institution = soup.find("span", {"id": "MainContent_DetailsView2_Label3"}).text
+        details_table_text = soup.find("table", {"id": "MainContent_DetailsView1"}).text
         try:
-            dlog(inarc, outarc, cf=conf)
-            print("Warning! Could not find column Timestamp in archive.")
-            inarc = inarc.select("AllPagesText", "Path")
-            outarc = outarc.select("AllPagesText", "Path")
+            race = re.search(r'Race\:(.)', details_table_text).group(1)
         except:
-            dlog(inarc, outarc, cf=conf)
-            print("Warning! Could not find column Path in archive.")
-            inarc = inarc.select("AllPagesText")
-            outarc = outarc.select("AllPagesText")
-
-    out = pl.concat([inarc, outarc])
-
-    if window:
-        window.write_event_value("COMPLETE-AA", True)
-    write(out, path=outpath, overwrite=True)
-    return out
-
-
-def rename_pdfs(cf):
-    if isinstance(cf, dict):
-        q = cf["QUEUE"]
-    elif isinstance(cf, pl.dataframe.frame.DataFrame):
-        if "Path" in cf.columns:
-            q = cf.select("Path").to_series().to_list()
-            cf = {"LOG": False}
-    else:
-        q = cf
-        cf = {"LOG": False}
-    if cf["LOG"] and not cf["WINDOW"]:
-        print("Renaming cases...")
-        for path in tqdm(q):
-            text = extract_text_pg_one(path)
-            try:
-                cnum = (
-                    re.search(r"County: (\d\d)", str(text)).group(1)
-                    + "-"
-                    + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
-                )
-            except:
-                cnum = os.path.split(path)[1]
-            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
-            os.rename(path, newpath)
-    elif not cf["LOG"]:
-        for path in q:
-            text = extract_text_pg_one(path)
-            try:
-                cnum = (
-                    re.search(r"County: (\d\d)", str(text)).group(1)
-                    + "-"
-                    + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
-                )
-            except:
-                cnum = os.path.split(path)[1]
-            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
-            os.rename(path, newpath)
-    elif cf["LOG"] and cf["WINDOW"]:
-        print("Renaming cases...")
-        cf["WINDOW"].write_event_value("PROGRESS_TOTAL", len(q))
-        for i, path in enumerate(q):
-            text = [extract_text_pg_one(path)]
-            try:
-                cnum = (
-                    re.search(r"County: (\d\d)", str(text)).group(1)
-                    + "-"
-                    + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
-                )
-            except:
-                cnum = os.path.split(path)[1]
-            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
-            os.rename(path, newpath)
-            cf["WINDOW"].write_event_value("PROGRESS", i + 1)
-        cf["WINDOW"].write_event_value("RN-COMPLETE", True)
-
-
-def _make_pairs_template(df, debug=False):
-    if isinstance(df, str):
-        df = read(df)
-    names = df.with_columns(
-        [
-            pl.concat_str(
-                [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
-                ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract(
-                r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
-                group_index=1,
-            )
-            .str.replace_all("Case Number:", "", literal=True)
-            .str.replace(r"C$", "")
-            .str.strip()
-            .alias("Name"),
-            pl.col("AllPagesText")
-            .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
-            .str.replace_all(r"[^\d/]", "")
-            .str.strip()
-            .alias("DOB"),
-            pl.col("AllPagesTextNoNewLine")
-            .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
-            .str.replace(r"(SSN)", "")
-            .str.replace(r"Alias", "")
-            .str.replace(r"\:", "")
-            .str.strip()
-            .alias("Alias"),
-        ]
-    )
-    names = (
-        names.groupby("Name")
-        .agg("CaseNumber", "Alias", "DOB")
-        .select(
+            race = ''
+        try:
+            sex = re.search(r'Sex\:(.)', details_table_text).group(1)
+        except:
+            sex = ''
+        try:
+            hair_color = re.search(r'Hair Color\:([A-Z]+)', details_table_text).group(1)
+        except:
+            hair_color = ''
+        try:
+            eye_color = re.search(r'Eye Color\:([A-Z]+)', details_table_text).group(1)
+        except:
+            eye_color = ''
+        try:
+            height = re.search(r'Height\:(.+)', details_table_text).group(1)
+        except:
+            height = ''
+        try:
+            weight = re.search(r'Weight\:(.+)', details_table_text).group(1)
+        except:
+            weight = ''
+        try:
+            birth_year = re.search(r'Birth Year\:(.+)', details_table_text).group(1)
+        except:
+            birth_year = ''
+        try:
+            custody = re.search(r'Custody\n\n(.+)', details_table_text).group(1).strip()
+        except:
+            custody = ''
+        aliases = "; ".join([re.sub('\"|,', '', cell.text).strip() for cell in soup.find_all("span", {"id": re.compile(r'MainContent_lvAlias_AliasLabel0_\d')})])
+        aliases = re.sub("No known Aliases", "", aliases)
+        scars_marks_tattoos = "; ".join([re.sub('\"|,', '', cell.text).strip() for cell in soup.find_all("span", {"id": re.compile(r'MainContent_lvScars_descriptLabel_\d')})])
+        scars_marks_tattoos = re.sub("No known scars marks or tattoos", "", scars_marks_tattoos)
+        inmate_details_df = pl.DataFrame({
+            'Name': [name],
+            'AIS': [ais],
+            'Institution': [institution],
+            'Race': [race],
+            'Sex': [sex],
+            'HairColor': [hair_color],
+            'EyeColor': [eye_color],
+            'Height': [height],
+            'Weight': [int(weight)],
+            'BirthYear': [int(birth_year)],
+            'Custody': [custody],
+            'Aliases': [aliases],
+            'ScarsMarksTattoos': [scars_marks_tattoos]
+        })
+        # black header "Sentences" tables
+        black_tables = soup.find_all("table", {"id": re.compile(r"MainContent_gvSentence_GridView1_\d+")})
+        black_tables_df = pl.DataFrame()
+        for i, black_table in enumerate(black_tables):
+            rows = black_table.find_all("tr")
+            table_list = []
+            for row in rows:
+                table_list += [[cell.text for cell in row.find_all("td")]]
+            df = pl.DataFrame({'Row': table_list})
+            df = df.select([
+                pl.lit(ais).alias("AIS"),
+                pl.lit(name).alias("Name"),
+                pl.lit(i+1).alias("TableNo").cast(pl.Int64, strict=False),
+                pl.col("Row").list.get(0).str.replace_all(r'\n','').alias("CaseNo"),
+                pl.col("Row").list.get(1).str.replace_all(r'\n','').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
+                pl.col("Row").list.get(2).str.replace_all(r'\n','').str.strip().alias("Offense"),
+                pl.col("Row").list.get(3).str.replace_all(r'\n','').alias("Term"),
+                pl.col("Row").list.get(4).str.replace_all(r'\n','').cast(pl.Int64, strict=False).alias("JailCredit"),
+                pl.col("Row").list.get(5).str.replace_all(r'\n','').cast(pl.Int64, strict=False).alias("PreTimeServed"),
+                pl.col("Row").list.get(6).str.replace_all(r'\n','').alias("Type"),
+                pl.col("Row").list.get(7).str.replace_all(r'\n','').alias("CommitCounty")
+            ])
+            df = df.filter(pl.col("CaseNo").is_null().is_not())
+            black_tables_df = pl.concat([black_tables_df, df])
+        # blue header tables
+        table = soup.find("table", {"id": "MainContent_gvSentence"})
+        rows = table.find_all("tr")
+        blue_tables_df = pl.DataFrame()
+        start_blue_row = False
+        table_no = 0
+        for row in rows:
+            if "SUFAdmit" in row.text:
+                start_blue_row = True
+                table_no += 1
+            elif start_blue_row and "Case No." not in row.text:
+                cells = [cell.text for cell in row.find_all("td")]
+                df = pl.DataFrame({'TableNo': [table_no], 'Row': [cells]})
+                blue_tables_df = pl.concat([blue_tables_df, df])
+            elif "Case No." in row.text:
+                start_blue_row = False
+        blue_tables_df = blue_tables_df.select(
             [
-                pl.lit("").alias("AIS / Unique ID"),
-                pl.col("Name"),
-                pl.col("Alias").arr.get(0),
-                pl.col("DOB").arr.get(0),
-                pl.col("CaseNumber").arr.lengths().alias("CaseCount"),
-                pl.col("CaseNumber").arr.join(", ").alias("Cases"),
+                pl.lit(name).alias("Name"),
+                pl.lit(ais).alias("AIS"),
+                pl.col("TableNo"),
+                pl.col("Row").list.get(0).alias("SUF"),
+                pl.col("Row").list.get(1).alias("AdmitDate").str.to_date('%m/%d/%Y', strict=False),
+                pl.col("Row").list.get(2).alias("TotalTerm"),
+                pl.col("Row").list.get(3).alias("TimeServed"),
+                pl.col("Row").list.get(4).alias("JailCredit").cast(pl.Int64, strict=False),
+                pl.col("Row").list.get(5).alias("GoodTimeReceived"),
+                pl.col("Row").list.get(6).alias("GoodTimeRevoked"),
+                pl.col("Row").list.get(7).alias("MinReleaseDate").str.to_date('%m/%d/%Y', strict=False),
+                pl.col("Row").list.get(8).alias("ParoleConsiderationDate").str.to_date('%m/%d/%Y', strict=False),
+                pl.col("Row").list.get(9).alias("ParoleStatus")
             ]
         )
-    )
-    names = names.sort("Name")
-    return names
-
-
-def _vrr_summary_from_pairs(src, pairs, dest=None, window=None, debug=False):
-    if isinstance(src, str):
-        cases = cf(src, table="cases", now=True)
-        charges = cf(src, table="charges", now=True)
-    if isinstance(pairs, str):
-        pairs = read(pairs)
-    cases = cases.select("CaseNumber", "Name", "DOB", "Race", "Sex")
-    cases = cases.with_columns(
-        [
-            pl.col("Race").cast(pl.Utf8, strict=False),
-            pl.col("Sex").cast(pl.Utf8, strict=False),
-        ]
-    )
-    fch = charges.filter(pl.col("Filing"))
-    fch = fch.join(pairs, on="Name", how="outer")
-    fch = fch.groupby("AIS / Unique ID").all()
-    fch = fch.select(
-        [
-            pl.col("AIS / Unique ID"),
-            pl.col("CERVDisqCharge").arr.count_match(True).alias("CERVChargesCount"),
-            pl.col("PardonDisqCharge")
-            .arr.count_match(True)
-            .alias("PardonToVoteChargesCount"),
-            pl.col("PermanentDisqCharge")
-            .arr.count_match(True)
-            .alias("PermanentDisqChargesCount"),
-            pl.col("ChargesSummary").arr.join(", ")
-            .str.replace_all(r"null,?", "")
-            .str.strip()
-            .str.replace(r",$", "")
-            .str.replace_all(r"\s+", " ")
-            .alias("FilingCharges"),
+        return {
+            'InmateDetails': inmate_details_df, 
+            'BlueTables': blue_tables_df,
+            'BlackTables': black_tables_df
+        }
 
-        ]
-    )
-    conv = charges.filter(pl.col("Disposition") & pl.col("Conviction"))
-    conv = conv.join(pairs, on="Name", how="outer")
-    conv = conv.groupby("AIS / Unique ID").all()
-    conv = conv.select(
-        [
-            pl.col("AIS / Unique ID"),
-            pl.col("Conviction")
-            .arr.count_match(True)
-            .alias("ConvictionCount"),
-            pl.col("CERVDisqConviction")
-            .arr.count_match(True)
-            .alias("CERVConvictionCount"),
-            pl.col("PardonDisqConviction")
-            .arr.count_match(True)
-            .alias("PardonToVoteConvictionCount"),
-            pl.col("PermanentDisqConviction")
-            .arr.count_match(True)
-            .alias("PermanentDisqConvictionCount"),
-            pl.col("PaymentToRestore").arr.mean(),
-            pl.col("ChargesSummary").arr.join(", ")
-            .str.replace_all(r"null,?", "")
-            .str.strip()
-            .str.replace(r",$", "")
-            .str.replace_all(r"\s+", " ")
-            .alias("Convictions"),
-        ]
-    )
-    vrr = charges.filter(
-        pl.col("CERVDisqConviction")
-        | pl.col("PardonDisqConviction")
-        | pl.col("PermanentDisqConviction")
-    )
-    vrr = vrr.join(pairs, on="Name", how="outer")
-    vrr = vrr.groupby("AIS / Unique ID").all()
-    vrr = vrr.select(
-        [
-            pl.col("AIS / Unique ID"),
-            pl.col("ChargesSummary").arr.join(", ")
-            .str.replace_all(r"null,?", "")
-            .str.strip()
-            .str.replace(r",$", "")
-            .str.replace_all(r"\s+", " ")
-            .alias("DisqualifyingConvictions")
-        ]
-    )
-    cases = cases.join(pairs, on="Name", how="outer")
-    cases = cases.groupby("AIS / Unique ID").all()
-    cases = cases.join(vrr, on="AIS / Unique ID", how="outer")
-    cases = cases.join(conv, on="AIS / Unique ID", how="outer")
-    cases = cases.join(fch, on="AIS / Unique ID", how="outer")
-    cases = cases.select(
-        [
-            pl.col("AIS / Unique ID"),
-            pl.col("Name").arr.first(),
-            pl.col("DOB").arr.first(),
-            pl.col("Race").arr.first(),
-            pl.col("Sex").arr.first(),
-            pl.col("PaymentToRestore"),
-            pl.col("ConvictionCount"),
-            pl.col("CERVChargesCount"),
-            pl.col("CERVConvictionCount"),
-            pl.col("PardonToVoteChargesCount"),
-            pl.col("PardonToVoteConvictionCount"),
-            pl.col("PermanentDisqChargesCount"),
-            pl.col("PermanentDisqConvictionCount"),
-            pl.col("DisqualifyingConvictions"),
-            pl.col("Convictions"),
-            pl.col("FilingCharges"),
-            pl.col("CaseNumber").arr.join(", ")            
-            .str.replace_all(r"null,?", "")
-            .str.strip()
-            .str.replace(r",$", "")
-            .str.replace_all(r"\s+", " ")
-            .alias("Cases")
-        ]
-    )
-    cases = cases.sort("Name")
-    if dest == None:
-        pass
-    elif os.path.splitext(dest)[1] == '.csv':
-        cases.write_csv(dest)
-    elif os.path.splitext(dest)[1] in ('.xls','.xlsx'):
+    def set_output_path(self, output_path) -> None:
+        """
+        Set results output path for start_queue().
+        """
+        self.output = output_path
+
+    def set_queue(self, queue, output_path='') -> None:
+        """
+        Set queue from dataframe or spreadsheet with "Last Name", "First Name", and "AIS" columns.
+        """
+        if isinstance(queue, str):
+            self.queue_path = queue
+            self.queue = read(queue)
+        if isinstance(queue, pl.DataFrame): 
+            self.queue_path = None
+            self.queue = queue
+        for col in ["Retrieved", "Timestamp"]:
+            if col not in self.queue.columns:
+                self.queue = self.queue.with_columns(pl.lit('').alias(col))
+        for col in self.queue.columns:
+            if re.sub(' ','_', col).upper() in ["LAST_NAME", "FIRST_NAME", "AIS"]:
+                self.queue = self.queue.with_columns(pl.col(col).alias(f"TEMP_{re.sub(' ','_', col).upper()}"))
+        if "TEMP_LAST_NAME" not in self.queue.columns and "TEMP_FIRST_NAME" not in self.queue.columns and "Name" in self.queue.columns:
+            self.queue = self.queue.with_columns([
+                pl.col("Name").str.extract(r'([A-Z]+)').alias("TEMP_LAST_NAME"),
+                pl.col("Name").str.extract(r' ([A-Z]+)').alias("TEMP_FIRST_NAME")
+            ])
+        for col in ["TEMP_LAST_NAME", "TEMP_FIRST_NAME", "TEMP_AIS"]:
+            if col not in self.queue.columns:
+                self.queue = self.queue.with_columns(pl.lit('').alias(col))
+
+    def start_queue(self, queue=None, output_path=None):
+        """
+        ADOC Inmate Search for each in `queue`, and save results to `output_path`.
+        """
+        if isinstance(queue, pl.DataFrame) or isinstance(queue, str):
+            self.set_queue(queue)
+        elif self.queue == None:
+            raise Exception("Must set queue to start.")
+        if output_path != None:
+            self.set_output_path(output_path)
         try:
-            cases = cases.with_columns(
-                [
-                    pl.col("DOB").cast(pl.Utf8, strict=False)
-                ]
-            )
-            cases.to_pandas().to_excel(dest)
+            inmate_details = pl.read_excel(self.output, sheet_name="inmate-details").with_columns(pl.col("AIS").cast(pl.Utf8))
+            blue_tables = pl.read_excel(self.output, sheet_name="blue-tables").with_columns([
+                pl.col("AIS").cast(pl.Utf8),
+                pl.col("TableNo").cast(pl.Int64, strict=False),
+                pl.col("AdmitDate").str.to_date('%Y-%m-%d', strict=False),
+                pl.col("MinReleaseDate").str.to_date('%Y-%m-%d', strict=False),
+                pl.col("ParoleConsiderationDate").str.to_date('%Y-%m-%d', strict=False)
+            ])
+            black_tables = pl.read_excel(self.output, sheet_name="black-tables").with_columns([
+                pl.col("AIS").cast(pl.Utf8),
+                pl.col("TableNo").cast(pl.Int64, strict=False),
+                pl.col("Sentenced").str.to_date('%Y-%m-%d', strict=False)
+            ])
+            print("Appending to existing tables at output path.")
         except:
-            popup("Warning: failsafe exported to .csv.", cf=window)
-            cases.write_csv(os.path.splitext(dest)[0]+".csv")
-    elif os.path.splitext(dest)[1] == '.parquet':
-        cases.write_parquet(dest)
-    elif os.path.splitext(dest)[1] == '.json':
-        cases.write_json(dest)
-    return cases
+            inmate_details = pl.DataFrame()
+            blue_tables = pl.DataFrame()
+            black_tables = pl.DataFrame()
+        with progress_bar as p:
+            for i, r in enumerate(p.track(self.queue.rows(named=True), description="Searching ADOC...")):
+                if r['Retrieved'] in (None, ""):
+                    self.search(ais=r['TEMP_AIS'], first_name=r['TEMP_FIRST_NAME'], last_name=r['TEMP_LAST_NAME'])
+                    if self.select_result(0):
+                        results = self.read_results_page()
+                        inmate_details = pl.concat([inmate_details, results['InmateDetails']])
+                        blue_tables = pl.concat([blue_tables, results['BlueTables']])
+                        black_tables = pl.concat([black_tables, results['BlackTables']])
+                        self.queue[i, 'Retrieved'] = "Y"
+                        self.queue[i, 'Timestamp'] = time.time()
+                    else:
+                        self.queue[i, 'Retrieved'] = "NO RESULTS"
+                        self.queue[i, 'Timestamp'] = time.time()
+                    if self.output != None and i % 10 == 0:
+                        write({'inmate-details': inmate_details, 'blue-tables': blue_tables, 'black-tables': black_tables}, self.output)
+                    if self.queue_path != None and i % 10 == 0:
+                        write_queue = self.queue.select(pl.exclude("TEMP_LAST_NAME", "TEMP_FIRST_NAME", "TEMP_AIS"))
+                        write({'queue': write_queue}, self.queue_path)
+            if self.output != None:
+                write({'inmate-details': inmate_details, 'blue-tables': blue_tables, 'black-tables': black_tables}, self.output)
+            if self.queue_path != None:
+                write_queue = self.queue.select(pl.exclude("TEMP_LAST_NAME", "TEMP_FIRST_NAME", "TEMP_AIS"))
+                write({'queue': write_queue}, self.queue_path)
+        return {
+            'inmate-details': inmate_details,
+            'blue-tables': blue_tables,
+            'black-tables': black_tables
+        }
 
+class Cases():
 
-def _explode_charges(df, debug=False):
-    all_charges = df.with_columns(
-        [
-            pl.concat_str(
+    def __init__(self, archive):
+        if isinstance(archive, str):
+            if os.path.isdir(archive):
+                self.archive = archive
+                self.is_read = False
+            elif os.path.isfile(archive):
+                self.archive = read(archive)
+                self.is_read = True
+            else:
+                raise Exception("Could not read input.")
+        if isinstance(archive, pl.DataFrame):
+            self.archive = read(archive)
+            self.is_read = True
+        self._cases = None
+        self._fees = None
+        self._charges = None
+        self._sentences = None
+        self._financial_history = None
+        self._settings = None
+        self._case_action_summary = None
+        self._witnesses = None
+        self._attorneys = None
+        self._images = None
+    
+    def read(self):
+        self.archive = read(self.archive)
+        self.is_read = True
+        return self.archive
+    
+    def cases(self):
+        if isinstance(self._cases, pl.DataFrame):
+            return self._cases
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing cases table..."):
+                cases = self.archive.with_columns(
+                    [
+                        pl.col("AllPagesText")
+                        .str.extract(
+                            r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
+                            group_index=1,
+                        )
+                        .str.replace("Case Number:", "", literal=True)
+                        .str.replace(r"C$", "")
+                        .str.strip()
+                        .alias("Name"),
+                        pl.col("AllPagesTextNoNewLine")
+                        .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
+                        .str.replace(r"(SSN)", "")
+                        .str.replace(r"Alias", "")
+                        .str.replace(r"\:", "")
+                        .str.strip()
+                        .alias("Alias"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
+                        .str.replace(r"[^\d/]", "")  # _all
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("DOB"),
+                        pl.concat_str(
+                            [
+                                pl.col("AllPagesText").str.extract(
+                                    r"(County: )(\d{2})", group_index=2
+                                ),
+                                pl.lit("-"),
+                                pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                            ]
+                        ).alias("CaseNumber"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(Phone: )(.+)", group_index=2)
+                        .str.replace_all(r"[^0-9]", "")
+                        .str.slice(0, 10)
+                        .str.replace(r"(.{3}0000000)", "")  # _all
+                        .alias("RE_Phone"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(B|W|H|A)/(?:F|M)")
+                        .cast(pl.Categorical)
+                        .alias("Race"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(?:B|W|H|A)/(F|M)")
+                        .cast(pl.Categorical)
+                        .alias("Sex"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(?:Address 1:)(.+)(?:Phone)*?", group_index=1)
+                        .str.replace(r"(Phone.+)", "")
+                        .str.strip()
+                        .alias("Address1"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(?:Address 2:)(.+)")
+                        .str.strip()
+                        .alias("Address2"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(?:Zip: )(.+)", group_index=1)
+                        .str.replace(r"[A-Za-z\:\s]+", "")
+                        .str.strip()
+                        .alias("ZipCode"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
+                        .str.strip()
+                        .alias("City"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=2)
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("State"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(Total:.+\$[^\n]*)")
+                        .str.replace_all(r"[^0-9|\.|\s|\$]", "")
+                        .str.extract_all(r"\s\$\d+\.\d{2}")
+                        .alias("TOTALS"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
+                        .str.extract_all(r"\$\d+\.\d{2}")
+                        .list.get(-1)
+                        .str.replace(r"[\$\s]", "")
+                        .cast(pl.Float64, strict=False)
+                        .alias("D999RAW"),
+                        pl.col("AllPagesText")
+                        .str.extract_all(r"(\w{2}\d{12})")
+                        .list.join("/")
+                        .alias("RelatedCases"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("FilingDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("CaseInitiationDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("ArrestDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("OffenseDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("IndictmentDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("YouthfulDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"AL Institutional Service Num: ([^\na-z])")
+                        .str.strip()
+                        .alias("ALInstitutionalServiceNum"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("Retrieved"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Jury Demand: ([A-Z]+)")
+                        .cast(pl.Categorical)
+                        .alias("JuryDemand"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
+                        .cast(pl.Categorical)
+                        .alias("InpatientTreatmentOrdered"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Trial Type: ([A-Z]+)")
+                        .str.replace(r"[S|N]$", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("TrialType"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Case Number: (\d\d-\w+) County:")
+                        .str.strip()
+                        .alias("County"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Judge: ([A-Z\-\.\s]+)")
+                        .str.rstrip("T")
+                        .str.strip()
+                        .alias("Judge"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Probation Office \#: ([0-9\-]+)")
+                        .alias("PROBATIONOFFICENUMBERRAW"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Defendant Status: ([A-Z\s]+)")
+                        .str.rstrip("J")
+                        .str.replace(r"\n", " ")
+                        .str.replace(r"\s+", " ")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("DefendantStatus"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"([^0-9]+) Arresting Agency Type:")
+                        .str.replace(r"^\-.+", "")
+                        .str.replace(r"County\:", "")
+                        .str.replace(r"Defendant Status\:", "")
+                        .str.replace(r"Judge\:", "")
+                        .str.replace(r"Trial Type\:", "")
+                        .str.replace(r"Probation Office \#\:", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("ArrestingAgencyType"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Arresting Officer: ([A-Z\s]+)")
+                        .str.replace(r"[\s\n]+[A-Z0-9]$", "")
+                        .str.strip()
+                        .alias("ArrestingOfficer"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Probation Office Name: ([A-Z0-9]+)")
+                        .alias("ProbationOfficeName"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Traffic Citation \#: ([A-Z0-9]+)")
+                        .alias("TrafficCitationNumber"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Previous DUI Convictions: (\d{3})")
+                        .str.strip()
+                        .cast(pl.Int64, strict=False)
+                        .alias("PreviousDUIConvictions"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Case Initiation Type: ([A-Z\s]+)")
+                        .str.rstrip("J")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("CaseInitiationType"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Domestic Violence: ([YES|NO])")
+                        .cast(pl.Categorical)
+                        .alias("DomesticViolence"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Agency ORI: ([A-Z\s]+)")
+                        .str.rstrip("C")
+                        .str.replace(r"\n", "")
+                        .str.replace_all(r"\s+", " ")
+                        .str.strip()
+                        .alias("AgencyORI"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Driver License N°: ([A-Z0-9]+)")
+                        .alias("DLRAW"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"SSN: ([X\d]{3}\-[X\d]{2}-[X\d]{4})")
+                        .alias("SSN"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"([A-Z0-9]{11}?) State ID:")
+                        .alias("SIDRAW"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Weight: (\d*)", group_index=1)
+                        .cast(pl.Int64, strict=False)
+                        .alias("Weight"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Height : (\d'\d{2})")
+                        .alias("RAWHEIGHT"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Eyes/Hair: (\w{3})/(\w{3})", group_index=1)
+                        .alias("Eyes"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Eyes/Hair: (\w{3})/(\w{3})", group_index=2)
+                        .alias("Hair"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Country: (\w*+)")
+                        .str.replace(r"(Enforcement|Party)", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("Country"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("WarrantIssuanceDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("WarrantActionDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Warrant Issuance Status: (\w+)")
+                        .str.replace(r"Description", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("WarrantIssuanceStatus"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Warrant Action Status: (\w+)")
+                        .str.replace(r"Description", "")
+                        .str.strip()
+                        .alias("WarrantActionStatus"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Warrant Location Status: (\w+)")
+                        .str.replace(r"Description", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("WarrantLocationStatus"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Number Of Warrants: (\d{3}\s\d{3})")
+                        .str.strip()
+                        .alias("NumberOfWarrants"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Bond Type: (\w+)")  # +
+                        .str.replace(r"Bond", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("BondType"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Bond Type Desc: ([A-Z\s]+)")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("BondTypeDesc"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"([\d\.]+) Bond Amount:")
+                        .cast(pl.Float64, strict=False)
+                        .alias("BondAmt"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Bond Company: ([A-Z0-9]+)")
+                        .str.rstrip("S")
+                        .alias("BondCompany"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Surety Code: ([A-Z0-9]{4})")
+                        .alias("SuretyCode"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("BondReleaseDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("FailedToAppearDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(
+                            r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:"
+                        )
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("BondsmanProcessIssuance"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Bondsman Process Return: (.*?) Number of Subponeas")
+                        .str.strip()
+                        .alias("BondsmanProcessReturn"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"([\n\s/\d]*?) Appeal Court:")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("AppealDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"([A-Z\-\s]+) Appeal Case Number")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("AppealCourt"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Orgin Of Appeal: ([A-Z\-\s]+)")
+                        .str.rstrip("L")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("OriginOfAppeal"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Appeal To Desc: ([A-Z\-\s]+)")
+                        .str.replace(r"[\s\n]+[A-Z0-9]$", "")
+                        .str.rstrip("O")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("AppealToDesc"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
+                        .str.rstrip("A")
+                        .str.replace_all(r"\n", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("AppealStatus"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Appeal To: (\w*) Appeal")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("AppealTo"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.replace_all(r"[\n\s:\-]", "")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("LowerCourtAppealDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.replace_all(r"[\n\s:\-]", "")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("DispositionDateOfAppeal"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Disposition Type Of Appeal: [^A-Za-z]+")
+                        .str.replace_all(r"[\n\s:\-]", "")
+                        .str.strip()
+                        .alias("DispositionTypeOfAppeal"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Number of Subponeas: (\d{3})")
+                        .str.replace_all(r"[^0-9]", "")
+                        .str.strip()
+                        .cast(pl.Int64, strict=False)
+                        .alias("NumberOfSubpoenas"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Updated By: (\w{3})")
+                        .str.strip()
+                        .alias("AdminUpdatedBy"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("TransferToAdminDocDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)")
+                        .str.replace_all(r"(Transfer Desc:)", "")
+                        .str.strip()
+                        .alias("TransferDesc"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("TBNV1"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)")
+                        .str.replace(r"Financial", "")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("TBNV2"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("TurnOverDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"TurnOver Amt\: \$(\d+\.\d\d)")
+                        .cast(pl.Float64, strict=False)
+                        .alias("TurnOverAmt"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Frequency Amt\: \$(\d+\.\d\d)")
+                        .cast(pl.Float64, strict=False)
+                        .alias("FrequencyAmt"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("DueDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("LastPaidDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Payor\: ([A-Z0-9]{4})")
+                        .cast(pl.Categorical)
+                        .alias("Payor"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Enforcement Status\: ([A-Z\:,\s]+)")
+                        .str.replace_all(r"\s+", " ")
+                        .str.replace(r" F$", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("EnforcementStatus"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Frequency\: ([W|M])")
+                        .str.replace(r"Cost Paid By\:", "")
+                        .str.strip()
+                        .alias("Frequency"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Placement Status\: (.+)")
+                        .str.strip()
+                        .alias("PlacementStatus"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"PreTrial\: (YES|NO)")
+                        .cast(pl.Categorical)
+                        .alias("PreTrial"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"PreTrail Date\: (.+)PreTrial")
+                        .str.strip()
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("PreTrialDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"PreTrial Terms\: (YES|NO)")
+                        .cast(pl.Categorical)
+                        .alias("PreTrialTerms"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("PreTermsDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Delinquent\: (YES|NO)")
+                        .cast(pl.Categorical)
+                        .alias("Delinquent"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("DelinquentDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"DA Mailer\: (YES|NO)")
+                        .cast(pl.Categorical)
+                        .alias("DAMailer"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("DAMailerDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Warrant Mailer\: (YES|NO)")
+                        .cast(pl.Categorical)
+                        .alias("WarrantMailer"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("WarrantMailerDate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("EnforcementLastUpdate"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"Updated By\: ([A-Z]{3})")
+                        .alias("EnforcementUpdatedBy"),
+                    ]
+                )
+                cases = cases.with_columns(
+                    [
+                        pl.when(pl.col("D999RAW").is_null())
+                        .then(pl.lit(0))
+                        .otherwise(pl.col("D999RAW"))
+                        .alias("D999")
+                    ]
+                )
+                # clean columns, unnest totals
+                cases = cases.with_columns(
+                    pl.col("RE_Phone")
+                    .str.replace_all(r"[^0-9]|2050000000", "")
+                    .alias("CLEAN_Phone"),
+                    pl.concat_str([pl.col("Address1"), pl.lit(" "), pl.col("Address2")])
+                    .str.replace_all(r"JID: \w{3} Hardship.*|Defendant Information.*", "")
+                    .str.strip()
+                    .alias("StreetAddress"),
+                    pl.col("Name"),
+                    pl.when(pl.col("PROBATIONOFFICENUMBERRAW") == "0-000000-00")
+                    .then(pl.lit(""))
+                    .otherwise(pl.col("PROBATIONOFFICENUMBERRAW"))
+                    .alias("ProbationOfficeName"),
+                    pl.when(pl.col("DLRAW") == "AL")
+                    .then(pl.lit(""))
+                    .otherwise(pl.col("DLRAW"))
+                    .alias("DriverLicenseNo"),
+                    pl.when(pl.col("SIDRAW") == "AL000000000")
+                    .then(pl.lit(""))
+                    .otherwise(pl.col("SIDRAW"))
+                    .alias("StateID"),
+                    pl.col("TOTALS")
+                    .list.get(0)
+                    .str.replace_all(r"[^0-9\.]", "")
+                    .cast(pl.Float64, strict=False)
+                    .alias("TotalAmtDue"),
+                    pl.col("TOTALS")
+                    .list.get(1)
+                    .str.replace_all(r"[^0-9\.]", "")
+                    .cast(pl.Float64, strict=False)
+                    .alias("TotalAmtPaid"),
+                    pl.col("TOTALS")
+                    .list.get(2)
+                    .str.replace_all(r"[^0-9\.]", "")
+                    .cast(pl.Float64, strict=False)
+                    .alias("TotalBalance"),
+                    pl.col("TOTALS")
+                    .list.get(3)
+                    .str.replace_all(r"[^0-9\.]", "")
+                    .cast(pl.Float64, strict=False)
+                    .alias("TotalAmtHold"),
+                )
+                cases = cases.with_columns(
+                    pl.when(pl.col("CLEAN_Phone").str.n_chars() < 7)
+                    .then(None)
+                    .otherwise(pl.col("CLEAN_Phone"))
+                    .alias("Phone"),
+                )
+                cases = cases.fill_null("")
+                cases = cases.select(
+                    "Retrieved",
+                    "CaseNumber",
+                    "Name",
+                    "Alias",
+                    "DOB",
+                    "Race",
+                    "Sex",
+                    "TotalAmtDue",
+                    "TotalAmtPaid",
+                    "TotalBalance",
+                    "TotalAmtHold",
+                    "D999",
+                    "BondAmt",
+                    "Phone",
+                    "StreetAddress",
+                    "City",
+                    "State",
+                    "ZipCode",
+                    "County",
+                    "Country",
+                    "SSN",
+                    "Weight",
+                    "Eyes",
+                    "Hair",
+                    "FilingDate",
+                    "CaseInitiationDate",
+                    "ArrestDate",
+                    "OffenseDate",
+                    "IndictmentDate",
+                    "JuryDemand",
+                    "InpatientTreatmentOrdered",
+                    "TrialType",
+                    "Judge",
+                    "DefendantStatus",
+                    "ArrestingAgencyType",
+                    "ArrestingOfficer",
+                    "ProbationOfficeName",
+                    "PreviousDUIConvictions",
+                    "CaseInitiationType",
+                    "DomesticViolence",
+                    "AgencyORI",
+                    "WarrantIssuanceDate",
+                    "WarrantActionDate",
+                    "WarrantIssuanceStatus",
+                    "WarrantActionStatus",
+                    "WarrantLocationStatus",
+                    "NumberOfWarrants",
+                    "BondType",
+                    "BondTypeDesc",
+                    "BondCompany",
+                    "SuretyCode",
+                    "BondReleaseDate",
+                    "FailedToAppearDate",
+                    "BondsmanProcessIssuance",
+                    "AppealDate",
+                    "AppealCourt",
+                    "OriginOfAppeal",
+                    "AppealToDesc",
+                    "AppealStatus",
+                    "AppealTo",
+                    "NumberOfSubpoenas",
+                    "AdminUpdatedBy",
+                    "TransferDesc",
+                    "TBNV1",
+                    "TBNV2",
+                    "DriverLicenseNo",
+                    "StateID",
+                    "TurnOverDate",
+                    "TurnOverAmt",
+                    "FrequencyAmt",
+                    "DueDate",
+                    "LastPaidDate",
+                    "Payor",
+                    "EnforcementStatus",
+                    "Frequency",
+                    "PlacementStatus",
+                    "PreTrial",
+                    "PreTrialDate",
+                    "PreTrialTerms",
+                    "PreTermsDate",
+                    "Delinquent",
+                    "DelinquentDate",
+                    "DAMailer",
+                    "DAMailerDate",
+                    "WarrantMailer",
+                    "WarrantMailerDate",
+                    "EnforcementLastUpdate",
+                    "EnforcementUpdatedBy",
+                )
+            self._cases = cases
+            return self._cases
+    
+    def fees(self):
+        if isinstance(self._fees, pl.DataFrame):
+            return self._fees
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing fee sheets..."):
+                cases = self.archive.with_columns(
+                    pl.col("AllPagesText")
+                    .str.extract_all(
+                        r"(ACTIVE [^\(\n]+\$[^\(\n]+ACTIVE[^\(\n]+[^\n]|Total:.+\$[^\n]*)"
+                    )
+                    .alias("RE_Fees")
+                )
+                all_fees = cases.explode("RE_Fees").select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("RE_Fees")
+                        .str.replace_all(r"[^A-Z0-9|\.|\s|\$|\n]", " ")
+                        .str.strip()
+                        .alias("Fees"),
+                    ]
+                )
+                df = all_fees.with_columns(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("Fees")
+                        .str.replace(r"(?:\$\d{1,2})( )", "\2")
+                        .str.split(" ")
+                        .alias("SPACE_SEP"),
+                        pl.col("Fees")
+                        .str.strip()
+                        .str.replace(" ", "")
+                        .str.extract_all(r"\s\$\d+\.\d{2}")
+                        .alias("FEE_SEP"),
+                    ]
+                )
+                df = df.with_columns(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("SPACE_SEP").list.get(0).alias("FeeStatus1"),
+                        pl.col("FEE_SEP").list.get(0).str.replace(r"\$", "").alias("AmtDue"),  # good
+                        pl.col("FEE_SEP")
+                        .list.get(1)
+                        .str.replace(r"\$", "")
+                        .alias("AmtPaid"),  # good
+                        pl.col("FEE_SEP").list.get(2).str.replace(r"\$", "").alias("Balance1"),
+                        pl.col("SPACE_SEP").list.get(5).alias("FeeCode"),
+                        pl.col("Fees").str.extract(r"(\w00\d)").alias("Payor"),
+                        pl.col("Fees").str.extract(r"\s(\d\d\d)\s").alias("Payee"),
+                    ]
+                )
+                out = df.with_columns(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.when(pl.col("FeeStatus1") != "ACTIVE")
+                        .then(True)
+                        .otherwise(False)
+                        .alias("TOT"),
+                        pl.when(pl.col("Balance1").is_in(["L", pl.Null]))
+                        .then("$0.00")
+                        .otherwise(pl.col("Balance1").str.replace_all(r"[A-Z]|\$", ""))
+                        .alias("AmtHold2"),
+                    ]
+                )
+                out = out.with_columns(
+                    pl.col("Fees").str.extract(r'\s(Y|N)\s').alias("AdminFee"),
+                    pl.when(pl.col("TOT") == True)
+                    .then(pl.col("FEE_SEP").list.get(-1).str.replace(r"\$", ""))
+                    .otherwise(pl.col("FEE_SEP").list.get(2).str.replace(r"\$", ""))
+                    .alias("AmtHold"),
+                    pl.when(pl.col("TOT") == False)
+                    .then(pl.col("SPACE_SEP").list.get(0))
+                    .otherwise(pl.lit(""))
+                    .alias("FeeStatus"),
+                    pl.when(pl.col("TOT") == True)
+                    .then(pl.lit("Total:"))
+                    .otherwise(pl.lit(""))
+                    .alias("Total"),
+                )
+                out = out.with_columns(
+                    [
+                        pl.col("AmtDue").str.strip().cast(pl.Float64, strict=False),
+                        pl.col("AmtPaid").str.strip().cast(pl.Float64, strict=False),
+                        pl.col("AmtHold").str.strip().cast(pl.Float64, strict=False),
+                    ]
+                )
+                out = out.with_columns([pl.col("AmtDue").sub(pl.col("AmtPaid")).alias("Balance")])
+                out = out.select(
+                    "CaseNumber",
+                    "Total",
+                    "FeeStatus",
+                    "AdminFee",
+                    "FeeCode",
+                    "Payor",
+                    "Payee",
+                    "AmtDue",
+                    "AmtPaid",
+                    "Balance",
+                    "AmtHold",
+                )
+                out = out.fill_null("")
+                out = out.drop_nulls("AmtDue")
+            self._fees = out
+            return self._fees
+    
+    def charges(self):
+        if isinstance(self._charges, pl.DataFrame):
+            return self._charges
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing charges..."):
+                all_charges = self.archive.with_columns(
+                    [
+                        pl.col("AllPagesText")
+                        .str.extract(
+                            r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
+                            group_index=1,
+                        )
+                        .str.replace_all("Case Number:", "", literal=True)
+                        .str.replace(r"C$", "")
+                        .str.strip()
+                        .alias("Name"),
+                        pl.col("AllPagesText")
+                        .str.extract_all(
+                            r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
+                        )
+                        .alias("RE_Charges"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(Total:.+\$[^\n]*)")
+                        .str.replace_all(r"[^0-9|\.|\s|\$]", "")
+                        .str.extract_all(r"\s\$\d+\.\d{2}")
+                        .list.get(2)
+                        .str.replace_all(r"[^0-9\.]", "")
+                        .cast(pl.Float64, strict=False)
+                        .alias("RAWTotalBalance"),
+                        pl.col("AllPagesText")
+                        .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
+                        .str.extract_all(r"\$\d+\.\d{2}")
+                        .list.get(-1)
+                        .str.replace(r"[\$\s]", "")
+                        .cast(pl.Float64, strict=False)
+                        .alias("RAWD999"),
+                    ]
+                )
+                all_charges = all_charges.explode("RE_Charges").select(
+                    [
+                        pl.col("Name"),
+                        pl.col("CaseNumber"),
+                        pl.col("RE_Charges")
+                        .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
+                        .str.strip()
+                        .alias("Charges"),
+                        pl.when(pl.col("RAWTotalBalance").is_null())
+                        .then(pl.lit(0.0))
+                        .otherwise(pl.col("RAWTotalBalance"))
+                        .alias("TotalBalance"),
+                        pl.when(pl.col("RAWD999").is_null())
+                        .then(pl.lit(0.0))
+                        .otherwise(pl.col("RAWD999"))
+                        .alias("TotalD999"),
+                    ]
+                )
+                charges = all_charges.with_columns(
+                    [
+                        pl.col("Name"),
+                        pl.col("CaseNumber"),
+                        pl.col("Charges").str.slice(0, 3).alias("Num"),
+                        pl.col("Charges").str.slice(4, 4).alias("Code"),
+                        pl.col("Charges").str.slice(9, 1).alias("Sort"),
+                        pl.col("Charges")
+                        .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)", group_index=1)
+                        .alias("CourtActionDate"),
+                        pl.col("Charges")
+                        .str.extract(
+                            r"[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}\({0,1}[A-Z]{0,1}\){0,1}\.{0,1}\d{0,1}",
+                            group_index=0,
+                        )
+                        .alias("RAWCITE"),
+                        pl.col("Charges")
+                        .str.extract(
+                            r"(BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)",
+                            group_index=1,
+                        )
+                        .alias("CourtAction"),
+                        pl.col("Charges")
+                        .apply(
+                            lambda x: re.split(
+                                r"[A-Z0-9]{3}\s*?-[A-Z0-9]{3}\s*?-[A-Z0-9]{3}\(*?[A-Z]*?\)*?\(*?[A-Z0-9]*?\)*?\.*?\d*?",
+                                str(x),
+                            )
+                        )
+                        .alias("Split"),
+                    ]
+                )
+                charges = charges.filter(pl.col("Num").str.contains("0"))
+                charges = charges.with_columns(
+                    [
+                        pl.col("Charges")
+                        .str.contains(r"\d\d?/\d\d?/\d\d\d\d")
+                        .alias("Disposition"),
+                        pl.col("Charges").str.contains(pl.lit("FELONY")).alias("Felony"),
+                        pl.col("Charges").str.contains("GUILTY PLEA").alias("GUILTY_PLEA"),
+                        pl.col("Charges").str.contains("CONVICTED").alias("CONVICTED"),
+                    ]
+                )
+                charges = charges.with_columns(
+                    [
+                        pl.when(pl.col("Disposition"))
+                        .then(pl.col("Split").list.get(1))
+                        .otherwise(pl.col("Split").list.get(0).str.slice(9))
+                        .str.replace(r"-   -", "", literal=True)
+                        .str.replace("1STS", "1ST", literal=True)
+                        .str.strip()
+                        .alias("RAWDESC"),
+                        pl.when(pl.col("Disposition"))
+                        .then(pl.col("Split").list.get(0).str.slice(19))
+                        .otherwise(pl.col("Split").list.get(1))
+                        .str.strip()
+                        .alias("SEG_2"),
+                        pl.when(pl.col("Disposition") == True)
+                        .then(False)
+                        .otherwise(True)
+                        .alias("Filing"),
+                    ]
+                )        
+                charges = charges.with_columns(
+                    [
+                        pl.col("SEG_2")
+                        .str.extract(
+                            r"(TRAFFIC MISDEMEANOR|BOND|FELONY|MISDEMEANOR|OTHER|TRAFFIC|VIOLATION)",
+                            group_index=1,
+                        )
+                        .str.replace("TRAFFIC MISDEMEANOR", "MISDEMEANOR")
+                        .alias("TypeDescription"),
+                        pl.col("SEG_2")
+                        .str.extract(
+                            r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
+                            group_index=1,
+                        )
+                        .alias("Category"),
+                        pl.col("RAWDESC")
+                        .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY|CONSPIRACY|SOLICIT[^I]*[^O]*[^N]*)")
+                        .is_not()
+                        .alias("A_S_C_DISQ"),
+                        pl.col("Code")
+                        .str.contains(
+                            r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
+                        )
+                        .alias("CERV_DISQ_MATCH"),
+                        pl.col("Code")
+                        .str.contains(
+                            r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
+                        )
+                        .alias("PARDON_DISQ_MATCH"),
+                        pl.col("Charges")
+                        .str.contains(r"(CM\d\d|CMUR|CAPITAL)")
+                        .alias("PERM_DISQ_MATCH"),
+                    ]
+                )
+                charges = charges.with_columns(
+                    [
+                        pl.when(pl.col("A_S_C_DISQ")==None)
+                        .then(True)
+                        .otherwise(pl.col("A_S_C_DISQ"))
+                        .alias("A_S_C_DISQ")
+                    ]
+                )
+                charges = charges.filter(pl.col("TypeDescription").str.contains(r"[A-Za-z]"))
+                charges = charges.with_columns(
+                    [
+                        pl.when(pl.col("GUILTY_PLEA") | pl.col("CONVICTED"))
+                        .then(True)
+                        .otherwise(False)
+                        .alias("Conviction")
+                    ]
+                )
+                charges = charges.with_columns(
+                    [
+                        pl.when(
+                            pl.col("CERV_DISQ_MATCH")
+                            & pl.col("Felony")
+                            & pl.col("Conviction")
+                            & pl.col("A_S_C_DISQ")
+                        )
+                        .then(True)
+                        .otherwise(False)
+                        .alias("CERVDisqConviction"),
+                        pl.when(pl.col("CERV_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
+                        .then(True)
+                        .otherwise(False)
+                        .alias("CERVDisqCharge"),
+                        pl.when(
+                            pl.col("PARDON_DISQ_MATCH")
+                            & pl.col("A_S_C_DISQ")
+                            & pl.col("Conviction")
+                            & pl.col("Felony")
+                        )
+                        .then(True)
+                        .otherwise(False)
+                        .alias("PardonDisqConviction"),
+                        pl.when(
+                            pl.col("PARDON_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ")
+                        )
+                        .then(True)
+                        .otherwise(False)
+                        .alias("PardonDisqCharge"),
+                        pl.when(
+                            pl.col("PERM_DISQ_MATCH")
+                            & pl.col("A_S_C_DISQ")
+                            & pl.col("Felony")
+                            & pl.col("Conviction")
+                        )
+                        .then(True)
+                        .otherwise(False)
+                        .alias("PermanentDisqConviction"),
+                        pl.when(pl.col("PERM_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
+                        .then(True)
+                        .otherwise(False)
+                        .alias("PermanentDisqCharge"),
+                        pl.concat_str([pl.col("CaseNumber"), pl.lit("-"), pl.col("Num")]).alias(
+                            "CASENONUM"
+                        ),
+                    ]
+                )
+                charges = charges.with_columns(
+                    [
+                        pl.col("TotalBalance"),
+                        pl.when(
+                            pl.col("CERVDisqConviction")
+                            | pl.col("PardonDisqConviction")
+                            | pl.col("PermanentDisqConviction")
+                        )
+                        .then((pl.col("TotalBalance") - pl.col("TotalD999")))
+                        .otherwise(None)
+                        .alias("PaymentToRestore"),
+                        pl.col("RAWDESC").alias("Description"),
+                        pl.col("RAWCITE").alias("Cite")
+                    ]
+                )
+                charges = charges.fill_null("")
+                fillers = pl.DataFrame({
+                    'Code': ['PFI3', 'NWNI', 'VDR1', 'UPCS', 'FRCC', 'T003', 'PMIO', 'UPCC', 'BEMV', 'HARA', 'TET3', 'T042', 'T707', 'SX12', 'TRAK', 'FCDC', 'TOD3', 'UAUV', 'T012', 'FR3D', 'HCOM', 'TP3D', 'VPCC', 'FORF', 'CECE', 'UDCS', 'PRO2', 'MCS1', 'ACHA', 'CECD', 'T627', 'FTCS', 'MCS2', 'PRO3', 'UAUM', 'T527', 'BRA3', 'FMUR', 'MURR', 'FPCC', 'PREC', 'STSA', 'T582', 'CM02', 'VDR4', 'VAPP', 'MAN1', 'VDR1', 'T755', 'TRAO', 'FORM', 'SVIA', 'TRAG', 'DSF1', 'MISC', 'BRA1', 'CEM1', 'CM04', 'IPCD', 'T005', 'T525', 'CM15', 'DUIF', 'T169', 'DUIM', 'T718', 'DVHF', 'TROP', 'CM10', 'CM17', 'CM01', 'VDRU', 'T770', 'ACAL', 'VDRY', 'TRFT', 'FNLE', 'RS3D', 'T806', 'TOS3', 'TSIB', 'T011', 'VAPD', 'T128', 'BHER', 'APPL', 'MRDI', 'UAUY', 'T019', 'T006', 'MAN2', 'CM18', 'NUSE', 'FBAP', 'VDRO', 'CM16', 'EDCO', 'T096', 'THBV', 'ASTM', 'SAVI', 'DVFC', 'T128', 'T071', 'CM07', 'TRBF', 'T813', 'CM03', 'TRMA', 'T783', 'T091', 'T072', 'TOS2', 'DV36', 'DSF2', 'CM08', 'DOG1', 'CEM3', 'PACS', 'T097', 'VDR2', 'BRA2', 'DVFC', 'TS3D', 'CODL', 'HAR2', 'T506', 'HGAR', 'TRCN', 'T773', 'PCUR', 'PPRE', 'T507', 'T081', 'PARA', 'MAAL', 'PCAB', 'DOG2', 'SFUF', 'OSUA', 'OSUA', 'EPH7', 'POBM', 'HWL2', 'FCPF', 'HNRL', 'DVAF', 'CPFP', 'VSMA', 'CM09', 'COMR', 'VDR5', 'TH3D', 'STG2', 'CM13', 'CNAR', 'VDR3', 'SCEF', 'CM06', 'T632', 'TRAA', 'CM13', "UUID", 'VIM2', 'TRSC', "OFFP", 'TRAY', 'COMF', 'SCR4', 'TRAT', 'TLT3', 'AGSF', 'EPH8', 'TER1', 'ECNF', 'DVE3', 'CM19', 'PSMF', 'TPCS', 'TRMF', 'CNVS', 'UPID', 'SCR6', 'COME', 'TRAQ', 'CM05', 'EAS1', 'FELO', 'CEM2', 'TS2D', 'DALE', 'CDMV', 'CM14', 'VAUA', 'COMM', 'AAPC', 'DVBF', 'TRAJ', 'DVMF', 'DV37', 'ASL1','BORK', 'T767', 'CNRR', 'PMDH', 'T043', 'LRAL', 'PUSF', 'SADV', 'TILU', 'T592', 'T513', 'FWPO', 'VPRA', 'FEED', 'T574', 'DOOM', 'CLCI', 'CODT', 'CRAB', 'STA2', 'NCOS', 'T731', 'BOCK', 'T031', 'PLUG', 'HLAG', 'CONT', 'T594', 'TREZ', 'T515', 'INSM', 'T802', 'SESS', 'HAMV', 'T505', 'TS4T', 'WOSO', 'T753', 'SIGN', 'T588', 'BLIC', 'T040', 'FIWO', 'VIM3', 'HUFV', 'TMOV', 'SETO', 'TMVV', 'LIFE', 'HWOL', 'T037', 'T622', 'T523', "PRFC", 'SHOW', 'VAUC', 'MAND', 'PCON', 'NBTR', 'UAUX', 'T799', 'TID1', 'T827', 'PDPM', 'CONS', 'SCFA', 'T116', 'T178', 'TRFM', 'TID2', 'FORT', 'T8LR', 'PAUL', 'DUIT', 'T309', 'TOWS', 'TZ67', 'APAA', 'BWNP', 'OFFM', 'UCR1', 'WAUB', 'TSTD', 'ASPC', 'APRE', 'SWOL', 'T082', 'MSTR', 'VSEX', 'MSDE', 'VAPR', 'TRWL', 'VLAT', 'OVES', 'TLEF', 'EPH5', 'AGSR', 'PLFV', 'STAA', 'T591', 'ROB1', 'TECH', 'PERT', 'PAGR', 'MCSD', 'EPHM', 'T590', 'EPHK', 'CC05', 'ELD1', 'TOFS', 'TRAZ', 'T601', 'UNLA', 'URNB', 'ESOC', 'OBUS', 'COMK', 'SOID', 'PRO1', 'UNLA'],
+                    'Description':  ['POSSESS FORGED INSTRUMENT 3RD', 'NEGOTIATING WORTHLESS INST', 'USE/POSSESS DRUG PARAPHERNALIA', 'POSS. CONTR. SUBS', 'FRAUD USE CREDIT/DEBIT CARD', 'NO DRIVERS LICENSE', 'PORN POSS MATERIAL MINORS', 'POSS CONTR SUBS INTENT DISTRIB', 'BREAK/ENTER VEHICLE', 'HARASSMENT', 'THEFT OF PROPERTY 3RD DEGREE', 'OVERWEIGHT TRUCK', 'FAIL DISPLAY INSURANCE', 'SEX ABUSE-CHILD LESS 12 YOA', 'TRAFFICKING-METHAMPHETAMINE', 'FRAUD USE CREDIT/DEBIT CARD', 'THEFT/DECEPTION 3RD', 'UNAUTHORIZED USE VEHICLE', 'FAIL STOP SIGN', 'FORGERY 3RD', 'HARASSING COMMUNICATIONS', 'THEFT OF PROPERTY 3RD DEGREE', 'POSS CONTROLLED SUBST BY FRAUD', 'BOND FORF-FELONY', 'CHEM END CHILD-EXP/CTN CTR SUB', 'UNLAW DISTRIB/FURN CONT SUBST', 'PROMOTING PROSTITUTION 2ND', 'UNLAW MANF CTN SUBS 1ST DEGREE', 'AGGRAVATED CHILD ABUSE', 'CHEM END CHILD-DEATH', 'LANE CHANGE W/O PROPER SIGNAL', 'FACILITATE TRAVEL F/ CHILD SEX', 'UNLAW MANF CTN SUBS 2ND DEGREE', 'PROMOTING PROSTITUTION 3RD', 'UNAUTHORIZED USE MOTOR VEHICLE', 'DUI-CONTROLLED SUBSTANCE', 'BURGLARY 3RD (UNOCCUPIED BLDG)', 'FELONY MURDER', 'MURDER-RECKLESS', 'ILL POSSESS CREDIT/DEBIT CARD', 'POSS/SELL PRECURSOR CHEMICALS', 'SEXUAL TORTURE/ABUSE', 'EXPIRED LICENSE', 'MURDER CAPITAL-ROBBERY', 'PARAPHERNALIA - SELL/DELIVER', 'POSSESS MARIHUANA 1ST DEGREE', 'MANSLAUGHTER-RECKLESS', 'USE/POSSESS DRUG PARAPHERNALIA', 'NO/IMP TAG LIGHT', 'TRAFFICKING-HEROIN', 'BOND FORF-MISD', 'SALVIA MISDEMEANOR POSSESSION', 'TRAFFICKING-SYNTHETIC DRUGS', 'DISCHARGE GUN OCC BLDG/VEHICLE', 'MISCELLANEOUS FILING', 'BURGLARY 3RD - DWELLING', 'CHEMICAL ENDANGER MINOR', 'MURDER CAPITAL-BURGLARY', 'ILL POSSESS CREDIT/DEBIT CARD', 'UNDER INFLUENCE CONT. SUBSTANC', 'DUI: ANY SUB WHICH IMPAIRS', 'MURDER CAPITAL-UNDER 14 YEARS', 'DUI - FELONY', 'SPEED/ 70+ MPH OR 65+ MPH', 'DUI - MISD', 'DUI: UNDER INFLU ALCOHOL', 'FELONY DV 3RD HARRASSMENT', 'TRAFFICKING-OPIUM', 'MURDER CAPITAL-TWO OR MORE PER', 'MURDER CAPITAL-VEH FR OUTSIDE', 'MURDER CAPITAL-KIDNAP', 'TRAFFICKING-MORPHINE', 'INOPERABLE BRAKE LIGHTS', 'AGGRAVATED CHILD ABUSE < SIX', 'TRAFFICKING-COCAINE', 'TRAFFICKING FENTANYL', 'GIVING FALSE NAME TO OFF', 'REC STOLEN PROP 3RD', 'NO DRIVERS LICENSE', 'THEFT OF SERVICES 3RD', 'TRAFFICKING STOLEN IDENTITIES', 'DRIVING WRONG SIDE HWY', 'POSSESS MARIHUANA 1ST DEGREE', 'NO TAG REGIS IN VEHICLE', 'BOND HEARING', 'CASE APPEALED ON', 'MURDER - INTENTIONAL', 'UNAUTHORIZED USE VEHICLE', 'FAILURE TO DIM LIGHTS', 'FAIL YIELD ROW', 'MANSLAUGHTER-INTENT, PASSION', 'MURDER CAPITAL-FIRED FROM VEHI', 'NO USER PERMIT', 'FRAUD BY AUTHORIZED PERSONS', 'DRUG PARAPHERNALIA TO MINOR', 'MURDER CAPITAL-DWELL FR OUTSID', 'ENDG WELFARE CHILD-OCCUPATION', 'MOVING TRAFFIC VIO', 'HOMICIDE BY VEHICLE', 'ALCOHOL-SALE/PERMIT UNDER AGE', 'SALVIA FELONY POSSESSION', 'FELONY DV CRIM MISCHIEF 2D/3D', 'NO TAG REGIS IN VEHICLE', 'COMBINED INFLUENCE', 'MURDER CAPITAL-FOR HIRE', 'TR-FORT.', 'MOVE OVER LAW', 'MURDER CAPITAL-RAPE/SODOMY', 'TRAFFICKING-MARIJUANA', 'IMPEDING FLOW TRAFFIC', 'DUI', 'UNDER INFLU - ANY SUBSTANCE', 'THEFT OF SERVICES 2ND', 'FELONY DV CRIM MISCHIEF 2ND', 'DISCHARGE GUN UNOCC BLDG/VEH', 'MURDER CAPITAL-SEXUAL ABUSE', 'DOG/CAT CRUELTY 1ST DEGREE', 'CHEMICAL ENDANGER MINOR/DEATH', 'PROHIBITED ACTS-MAIN BLD/DWL', 'OTHER NON MOVING VIO', 'DEL/SALE DRUG PARAPHERNALIA', 'BURGLARY 3RD - OCCUPIED BLDG', 'FELONY DV CRIM MISCHIEF 2D/3D', 'THEFT OF SERVICES 3RD DEGREE', 'CONTRIBUTING TO THE DELINQUENC', 'HARASSMENT - THREAT', 'FAIL TO YIELD EMER VEHICLE', 'FAILURE TO COMPLY - GARBAGE', 'TR-CONTEMPT', 'IMP TAIL LIGHTS-TRAILER', 'FAIL CPLY REPORTS-PRECUR CHEMS', 'POSS OF PRE-CURSOR CHEMICALS', 'FAIL TO YIELD RIGHT OF WAY', 'NO HDLGTS WHEN REQUIRED', 'FAILURE COMPLY PARK CONDITIONS', 'ALCOHOL- MINOR/POSS/CONSUME', 'POSS/CONT ALCOHOL-STATE PARK', 'DOG/CAT CRUELTY 2ND DEGREE', 'SETTING FIRE-UNCL FOREST/WOOD', 'OMMISSION/MISREP SALE SECURITI', 'OMMISSION/MISREP SALE SECURITI', 'ILL PURCHASE EPHEDRINE-INDIVID', 'PORN INTENT TO DISSEMINATE', 'HUNT-W/O NONRESIDENT LICENSE', 'FIREARM-PERSONS FORBIDDEN/POSS', 'HUNT-LEND RESIDENT LICENSE', 'FELONY DV 3RD ASSAULT 3RD', 'PISTOL-CERTAIN PERSONS FORBIDD', 'UNLAWFUL DISTRIB MARIHUANA', 'MURDER CAPITAL-ARSON', 'COMM NOTIF ACT-SCHOOL/CHILD CR', 'MANUFACTURE PARAPHERN/FIREARM', 'THEFT BY DECEPTION 3RD', 'AGGRAVATED STALKING 2ND DEGREE', 'MURDER CAPITAL-20YR PRIOR CON', 'COMM NOTIFICATION-DECLARATION', 'DEL/SALE DRUG PARAPHERNALIA', 'SCHOOL EMPLOYEE SEXUAL CONTACT', 'MURDER CAPITAL-LIFE SENTENCE', 'DUI FELONY', 'TRAFF/CONTR SUBSTANCE', 'MURDER CAPITAL-20YR PRIOR CON', "UNAUTH USE ID #", 'IMITATION DRUG DIST TO MONOR', 'SCRAP METAL/FALSIFY STATEMENT',"USE POSITION-PERSONAL GAIN", 'TRAFFICKING-HYDROMORPHONE','COMM NOTIF ACT-VICTIM/VIC FAMI', 'ILLEGAL DISPOSAL/ SCRAP TIRES', 'TRAFFICKING-3,4 METHYL AMPHETA','THEFT OF LOST PROPERTY 3RD', 'AGGRAVATED SURVEILLANCE FELONY', 'ILL PURCHASE EPHEDRINE-INDIVID', 'TERRORISM', 'ERROR CORAM NOBIS - FELONY', 'FELONY DV 3RD ONE PRIOR FELONY','CAPITAL MURDER - PROTECT ORDER', 'OBSCENE MATERIAL- DIST/POSS', 'THEFT 2ND CONTROLLED SUBSTANCE', 'TRAFF CANNABIS-W/POSS FIREARM', 'COMM NOTIF-10 DAY VERIF SUBMIT', 'POSS CONTR SUBS INTENT DISTRIB', 'SCRAP METAL/FALSE INFO', 'COM NOTIF ACT-NONRESIDENT', 'TRAFFICKING-LSD', 'MURDER CAPITAL-LAW OFF/GUARD', 'EXPLOITATION OF ASSETS 1ST', 'FELONY CASE', 'CHEMICAL ENDANGER INJURY', 'THEFT OF SERVICES 2ND DEGREE', 'DISARMING LAW ENFORCEMENT', 'UNAUTH USE MTR VEH - BY FORCE', 'MURDER CAPITAL-WITNESS', 'UNEMPLOYMENT COMP-CLASS B FEL', 'COMM NOTIF ACT-MINOR RESIDENCE', 'AIDS/ABETS PERSON COMMIT OFFEN', 'FELONY DV 3RD HARRASS COMMUNIC', 'TRAFFICKING-AMPHETAMINE', 'FELONY DV 3RD MENACING', 'FELONY DV CRIM MISCHIEF 3RD', 'ASSAULT 1ST DEGREE (DUI/BUI)','BOAT-RECKLESS OPER VESSEL', 'IMPROPER LOAD-UNSECURED', 'COMM NOTIF RESIDENCE REQ', 'HUNT/FEED AREA', 'OVERWIDE TRUCK', 'PERMITTING LIVESTOCK TO RUN AT', 'POSSESSING UNDERSIZE FISH', 'BOAT-VESS W/O SAFETY DEV/LGHT', 'IMPROPER LOAD', 'ALCOHOL-CONSUM/COMM VEH', 'DRIVE THRU BARRICADE', 'FISHING W/O PERMISSION OWNER', 'VIO. PARENTAL RESPONSIBILTY AC', 'HUNT-AREA FEEDING TAKEN PLACE', 'SPILLING LOAD ON ROAD', 'DISSEMINATE OBSCENE MATERIAL', 'CHANGING LIC PLATE-CONCEAL ID', 'CONT TO TRUANCY', 'POSS UNDERSIZED BLUE CRABS', 'STALKING  2ND DEGREE', 'NO CUT OFF SWITCH LANYARD', 'HITCHHIKING', 'BOAT-CARELESS OPER VESSEL', 'ONEWAY STREET', 'ILLEGAL ARMS - TURKEY HUNTING', 'HUNT W/O LICENSE (ALL GAME)', 'CONTEMPT OF COURT', 'BOATING UNDER THE INFLUENCE', 'FAIL/YIELD EMERG VEHICLE', 'OVERSIZED LOAD LIMIT', 'OPER VEH W/O INSURANCE', 'CAUSE/ALLOW LITTER-ROADWAY', 'SOLICIT SEX ACT WITH STUDENT', 'HUNT-BY AID MOTORIZED VESSEL', 'BLUE LIGHT LAW', 'THEFT OF SERVICES 4TH DEGREE', 'NO/ATTACHED SHUT-OFF SWITCH', 'IMP LIGHT COLORING', 'BOAT-VIO. RESTRICTIVE SIGN', 'STOPPING ON HIGHWAY', 'BOATING W/O LICENSE/CERTIF', 'OVERHEIGHT TRUCK', 'FISH-WO PERMISSION', 'IMITATION DRUG POSSESSION', 'HUNT-FROM VEHICLE', 'MOVE OVER/EMERGENCY VEHICLE', 'DIST OBSCENE MATERIAL/SCHOOL', 'MOVE OVER LAW VIOLATIONS', 'BOAT-VESSEL W/O LIFE PRE.', 'HUNT-W/O LICENSE', 'MOTORCYCLE NO-HELMET', 'NO TAG - UTILITY TRAILER', 'DUI 0.08 BAC OR ABOVE', 'PT-RL F/CN', 'SHOW CAUSE DKT/HEARING', 'UNEMPLOYMENT COMP-VIOLATION', 'WIRT OF MANDAMUS', 'PISTOL-CERTAIN PERSONS FORBIDD', 'NO ANT BUCK/TURKEY HAR RECORD', 'UNAUTHORIZED USE VEHICLE', 'PEDESTRIAN-SOL EMPLY/BUSN/CONT', 'IGNITION INTERLOCK MISDEMEANOR', 'FAIL UPDATE DL NAME/ADDRESS', 'DISTRIB HARMFUL MATERIAL-MINOR', 'CONSERVATION', 'SCIRE FACI', 'CMV W/O PROPER DOCUMENTS', 'DUI .08 OR MORE', 'TRAFFIC/MISC', 'IGNITION INTERLOCK VIOLATIONS', 'FORFEITURE-TRAFFIC', 'CAUSE/ALLOW LITTER ON ROADWAY', 'ALCOHOL-POSS UNTAXED LIQ', 'DUI TRIAL DOCKET', 'FAIL TO STOP AS REQUIRED', 'BOAT-SKING W/O MIRROR\\OBSERVER', 'CZ SLOWING/STOP W/O PROPER SIG', 'ALCOHOL - ON PUBLIC ACCESS AREA', 'BURN W/OUT NECESSARY PRECAUTIO', 'USE OFF POSITION- PERSONAL GAIN', 'UNIFIED CARRIER REGISTRATION', 'WHLSE SALE ALCOHOL UNA BUYER', 'KNOWINGLY TRANSMIT EXPOSE STD', 'ASPC-OTHER', 'ALCOHOL-ON OFF PREMISES LI', 'ALCOHOL-SELL W/O LICENSE', 'FAILURE TO DIM HEADLIGHTS', 'NO MASTER PLUMBER CERTIFICATE', 'VIOLATION COMMUNITY NOT ACT', 'MISDEMEANOR', 'VIOL POSTED RULE-WILDLIFE AREA', 'WASH SHRIMP TRAWL- CLOSED AREA', 'VIOLATION', 'OPER VESSEL W/O EMERG SHUTOFF', 'INTERSTATE/LEFT LANE 1.5 MILES', 'SINGLE SALE-EPHEDRINE PRODUCT', 'AGGRAVATED SURVEILLANCE MISD', 'HUNT-POSS LOAD GUN IN VEH', 'STALKING AGGRAVATED 1ST DEGREE', 'HANDICAPPED PARKING VIOLATION', 'ROBBERY 1ST', 'TECH VIOL PROBATION', 'UNLAW SALE TOBACCO W/O PERMIT', 'ALCOHOL-POSS MORE THAN 5 GAL.', 'WRONG1MANF CTN SUBS 1ST DEGREE', 'DRUG OFFENDER EPHEDRINE MISD', 'FAIL TO STOP EXIT PARKING LOT', 'SALE EPHEDRINE 2ND CONVICTION', 'CRIM CONSPIRACY -FELONY A', 'ELDER ABUSE AND NEGLECT 1ST', 'FALSE STATEMENT/EXPIRED TAG', 'FAILURE TO PARTICIPATE IN GARG', 'CROSS MEDIAN/IMP USE DIV HGWY', 'UNLAWFUL ASSEMBLY', 'ILLEGAL USE OF SYNTHETIC URINE', 'ELECTRONIC SOLICITION OF CHILD', 'SHOOT/DISC FIREARM OCC BUS/BLD', 'VIOL COM NOTIF ACT/EMPLOYMENT', 'SEX OFFENDER MANDATORY ID', 'PROMOTING PROSTITUTION 1ST', 'UNLAWFUL ASSEMBLY'],
+                    'Cite': ['13A-009-006.1', '13A-009-013.1', '13A-012-260(C)', '13A-012-212(A)', '13A-012-212(A)', '032-006-001(A)', '13A-012-192(B)', '013-012-192(B)', '13A-008-011(B)', '13A-011-008(A)', '13A-008-004.1', '032-009-020(4)', '032-07A-016(B)', '13A-006-069.1', '13A-012-231(11)', '13A-009-014(B)', '13A-008-004.1', '13A-008-011(A)', '032-05A-112(B)', '13A-009-003.1', '13A-011-008(B)', '13A-008-4.1', '13A-012-212(A)', '- -BOND FORT', '026-015-003.2(A)', '13A-012-211', '13A-012-112', '13A-012-218', '026-015-003.1(A)', '026-015-003.2(A)', '032-05A-133', '13A-006-125', '13A-012-217', '13A-012-113', '032-008-081', '032-05A-191(A)', '13A-007-007(A)', '13A-006-002(A)', '13A-006-002(A)', '13A-009-014(A)', '020-002-190(B)', '13A-006-065.1', '032-006-001(B)', '13A-005-040(A)', '13A-012-260(D)', '13A-012-213(A)', '13A-006-003(A)', '13A-012-260(C)', '032-005-240(C)', '13A-012-231(3)', '- -BOND FORT', '13A-012-214.1', '13A-012-231(12)', '13A-011-061(B)', '', '13A-007-007(A)', '026-015-3.2(A)', '13A-005-040(A)', '13A-009-014(A)', '032-05A-191(A)', '032-05A-191(A)', '13A-005-040(A)', '032-05A-191(A)', '032-05A-171(4)', '032-05A-191(A)', '032-05A-191(A)', '13A-006-132(D)', '13A-012-231(3)', '13A-005-040(A)', '13A-005-040(A)', '13A-005-040(A)', '13A-012-231(3)', '032-005-241(B)', '025-015-03.1(B)', '13A-012-231(2)', '13A-012-231(13)', '13A-009-018.1', '13A-008-18.1', '032-006-018(A)', '13A-008-010.3', '13A-008-193(B)', '032-05A-080(A)', '13A-012-213(A)', '040-012-260(B)', '', '', '13A-006-002(A)', '13A-008-011(A)', '032-005-242(C)', '032-05A-112(C)', '13A-006-003(A)', '13A-005-040(A)', '033-015-007(C)', '13A-009-014.1', '13A-012-260(E)', '13A-005-040(A)', '13A-013-006(A)', '', '032-05A-190.1', '028-03A-025(A)', '13A-012-214.1', '13A-006-132(D)', '040-012-260(B)', '032-05A-191(A)', '13A-005-040(A)', '', '032-05A-058.2', '13A-005-040(A)', '13A-012-231(1)', '032-05A-080(B)', '032-05A-191(A)', '032-05A-191(A)', '13A-008-010.2', '13A-006-132(D)', '13A-011-061(C)', '13A-005-040(A)', '13A-011-241(A)', '026-015-3.2(A)', '020-002-071(A)', '', '13A-012-260(E)', '13A-007-007(A)', '13A-006-132(D)', '13A-008-010.25', '012-015-111(A)', '13A-011-008(A)', '032-05A-115(A)', '022-027-003(A)', '', '032-005-240(C)', '020-002-190(A)', '020-002-181(D)', '032-05A-082(2)', '032-005-240(A)', '220-005-013(2)', '028-03A-025(A)', '220-005-016(4)', '13A-011-241(B)', '009-013-011(B)', '008-006-017(A)', '008-006-017(A)', '020-002-190(C)', '13A-012-192(A)', '009-011-051(C)', '13A-011-072(A)', '009-011-051(B)', '13A-006-132(D)', '13A-011-072(A)', '13A-012-211(A)', '13A-005-040(A)', '015-020-026(A)', '13A-012-260(D)', '13A-008-04.1', '13A-006-091.1', '13A-005-040(A)', '015-020-022(A)', '13A-012-260(E)', '13A-006-082(A)', '13A-005-040(A)', '032-05A-191(A)', '13A-012-231(12)', '13A-005-040(A)', "032-008-086(D)", '020-008-086(D)', '032-008-087(S)(2)', '036-025-005(A)','13A-012-231(5)', '015-020-026(B)', '022-40A-19(A)(4)', '13A-012-231(6)', '13A-008-008.1', '13A-011-32.1', '020-002-190(C)(4)', '13A-010-152(A)', '', '13A-006-132(E)', '13A-005-040(19)', '13A-012-200.2(1)', '13A-008-004(D)', '13A-012-231(13)', '015-020-024(B)', '13A-012-211(C)', '13A-008-031(D)', '015-020-25.1', '13A-012-231(9)', '13A-005-040(A)(5)', '038-009-007(G)', '', '026-015-3.2(A)(2)', '13A-008-010.2', '13A-010-005.1', '13A-008-011(A)(4)', '13A-005-040(A)(14)', '025-004-145(A)(1)A', '015-020-026(C)', '13A-002-023(2)', '13A-006-132(D)', '13A-012-231(10)', '13A-006-132(D)', '13A-006-132(D)', '13A-006-020(A)(5)','033-005-070(A)', '032-005-076(B)', '015-020-021(C)', '220-002-011(8', '032-009-020(1', '003-005-002(D)', '220-003-030(2', '033-005-022(A)', '032-005-076(B)', '032-006-049.1', '023-005-002(B)', '220-002-044(6', '016-028-012(A)', '220-002-011(8', '032-005-076(A)', '13A-012-200.3', '032-008-086(E)', '012-015-013(A)', '220-003-031(1', '13A-006-090.1', '033-005-051(C)', '032-05A-216(A)', '033-005-070(B)', '032-05A-087(B)', '220-002-002(3', '009-011-051(A)', '012-011-030', '032-05A-191.3', '032-05A-115(A)', '032-009-029(A)', '032-07A-016(1', '032-005-076(C)', '13A-006-082(B)', '220-002-011(1', '032-05A-115(C)', '13A-008-010.3', '033-005-072(A)', '032-005-242(G)', '220-006-019(4', '032-05A-136(A)', '033-005-052(A)', '032-009-020(2', '009-011-091(A)', '020-002-143(C)', '220-002-011(1', '032-05A-058.2', '13A-006-082.1', '032-05A-058.2', '220-006-011(1', '009-011-051(A)', '032-05A-245(A)', '040-012-252(A)', '032-05A-191(A)1','','','025-004-145(A)(1)C','','13A-011-072(B)', '220-002-146(2)', '13A-008-011(A)2', '032-05A-216(B)', '032-05A-191.4(J)', '760-X-1-07(7)', '13A-012-200.5(1)', '', '', '', '032-05A-191(A)1', '', '032-05A-191.4(L)','- -BOND FORT', '032-005-076(C)(1)', '028-04-020', '','','033-005-026(A)', '032-05A-133(C)', '220-002-037(13)', '009-013-011(B)(2)', '036-025-005(A)', 'PSC-3.2-016', '028-03A-025(A)(2)', '022-11A-021(C)', '', '028-03A-025(A)(4)', '028-03A-025(A)(14)', '032-005-242(C)(2)', '034-037-001(8)', '', '', '220-002-055(1)(BB)', '220-003-001(5)', '', '033-005-072(B)', '032-05A-080(D)(1)', '020-002-190(C)(2)', '13A-011-32.1', '220-002-055(1)(K)', '13A-006-091', '032-006-233.1', '13A-008-041', '015-022-054.1', '028-011-008', '028-004-115', '13A-012-218', '020-002-190.2(K)', '032-05A-153', '020-002-190.2(K)', '13A-006-192', '032-006-219', '022-027-007', '032-05A-090', '13A-011-005', '13A-012-340', '13A-006-122', '13A-004-003', '13A-011-061.1', '015-020-023.1', '015-020-026.2', '13A-012-111', '13A-011-005'] 
+                    }
+                )
+                for r in fillers.rows():
+                    charges = charges.with_columns(
+                        [
+                            pl.when(pl.col("Code")==r[0])
+                            .then(r[1])
+                            .otherwise(pl.col("Description"))
+                            .alias("Description"),
+                            pl.when(pl.col("Code")==r[0])
+                            .then(r[2])
+                            .otherwise(pl.col("Cite"))
+                            .alias("Cite")
+                        ]
+                    )
+                charges = charges.with_columns(
+                    [
+                        pl.when((pl.col("Code")=="VIM1") & (pl.col("Description").eq("")))
+                        .then("IMITATION DRUG MANUF/DIST")
+                        .otherwise(pl.col("Description"))
+                        .alias("Description"),
+                        pl.when((pl.col("Code")=="VIM1") & (pl.col("Cite").eq("")))
+                        .then("020-002-143(A)")
+                        .otherwise(pl.col("Cite"))
+                        .alias("Cite")
+                    ]
+                )
+                charges = charges.with_columns(
+                    [
+                        pl.col("Charges").str.extract(r'\s(A|S|C|P)\s').alias("ID"),
+                        pl.concat_str(
+                            [
+                                pl.col("CaseNumber"),
+                                pl.lit(" - "),
+                                pl.col("Num"),
+                                pl.lit(" "),
+                                pl.col("Cite"),
+                                pl.lit(" "),
+                                pl.col("Description"),
+                                pl.lit(" "),
+                                pl.col("TypeDescription"),
+                                pl.lit(" "),
+                                pl.col("CourtAction"),
+                                pl.lit(" "),
+                                pl.col("CourtActionDate"),
+                            ]
+                        )
+                        .str.strip()
+                        .str.replace(r",$", "")
+                        .str.replace_all(r"\s+", " ")
+                        .str.replace(r"\.\s\.\s", ".")
+                        .str.replace(r'\s[ASC]\s'," ")
+                        .alias("ChargesSummary")
+                    ]
+                )
+                charges = charges.with_columns(
+                    [
+                        pl.when(pl.col("Charges").str.contains("ATTEMPT").is_not() & pl.col("ID").eq("A"))
+                        .then("")
+                        .otherwise(pl.col("ID"))
+                        .alias("ID"),
+                        pl.col("Description")
+                        .str.replace(r'^\.\d?\s','')
+                        .str.replace(r'\s[ASC]\s', " ")
+                        .str.replace(r'^[ASC]\s', "")
+                    ]
+                )
+                charges = charges.with_columns(
+                    [
+                        pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
+                        .then("CONSPIRACY -ROBBERY 1ST DEGREE")
+                        .otherwise(pl.col("Description"))
+                        .alias("Description"),
+                        pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
+                        .then(False)
+                        .otherwise(pl.col("CERVDisqCharge"))
+                        .alias("CERVDisqCharge")
+                    ]
+                )
+                charges = charges.with_columns(
+                    [
+                        pl.when(pl.col("Charges").str.contains("WILFULL FAILURE TO RETURN TO P"))
+                        .then("")
+                        .otherwise(pl.col("ID"))
+                        .alias("ID")
+                    ])
+                charges = charges.fill_null('')
+                charges = charges.with_columns(
+                    [
+                        pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
+                        pl.col("Category").cast(pl.Categorical),
+                        pl.col("TypeDescription").cast(pl.Categorical),
+                        pl.col("CourtAction").cast(pl.Categorical),
+                    ]
+                )
+                charges = charges.select(
+                    "Name",
+                    "CaseNumber",
+                    "Num",
+                    "Code",
+                    "Cite",
+                    "ID",
+                    "Description",
+                    "TypeDescription",
+                    "Category",
+                    "CourtAction",
+                    "CourtActionDate",
+                    "TotalBalance",
+                    "PaymentToRestore",
+                    "Conviction",
+                    "Felony",
+                    "CERVDisqCharge",
+                    "CERVDisqConviction",
+                    "PardonDisqCharge",
+                    "PardonDisqConviction",
+                    "PermanentDisqCharge",
+                    "PermanentDisqConviction",
+                    "Filing",
+                    "Disposition",
+                    "ChargesSummary"
+                )
+            self._charges = charges
+            return self._charges
+    
+    def sentences(self):
+        if isinstance(self._sentences, pl.DataFrame):
+            return self._sentences
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing sentences..."):
+                sent = self.archive.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("AllPagesTextNoNewLine")
+                        .str.extract_all(r"Sentence\s\d\s.+?(Linked Cases)")
+                        .alias("Sentence"),
+                    ]
+                )
+                sent = sent.explode("Sentence")
+                sent = sent.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("Sentence")
+                        .str.extract(r"Sentence\s(\d)\s")
+                        .cast(pl.Int64, strict=False)
+                        .alias("Number"),
+                        pl.col("Sentence")
+                        .str.extract(
+                            r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}"
+                        )
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("LastUpdate"),
+                        pl.col("Sentence")
+                        .str.extract(
+                            r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})"
+                        )
+                        .alias("UpdatedBy"),
+                        pl.col("Sentence")
+                        .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
+                        .str.replace(r"Sentence.*", "")
+                        .str.replace(r"License.+", "")
+                        .str.strip()
+                        .str.to_date('%m/%d/%Y', strict=False)
+                        .alias("ProbationRevoke"),
+                        pl.col("Sentence")
+                        .str.extract(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
+                        .alias("LicenseSuspPeriod"),
+                        pl.col("Sentence")
+                        .str.extract(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+")
+                        .alias("JailCreditPeriod"),
+                        pl.col("Sentence")
+                        .str.extract(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
+                        .alias("ProbationPeriod"),
+                        pl.col("Sentence")
+                        .str.extract(r"Sentence Provisions\: ([YN])")
+                        .cast(pl.Categorical)
+                        .alias("Provisions"),
+                        pl.col("Sentence")
+                        .str.extract(r"Requrements Completed\: (YES|NO)")
+                        .cast(pl.Categorical)
+                        .alias("RequirementsCompleted"),
+                        pl.col("Sentence")
+                        .str.extract(r"Sentence Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("SentenceDate"),
+                        pl.col("Sentence")
+                        .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("StartDate"),
+                        pl.col("Sentence")
+                        .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("EndDate"),
+                        pl.col("Sentence")
+                        .str.extract(r"Jail Fee\:(.+?)Costs")
+                        .str.replace(r"[A-Z]-\$", "")
+                        .str.strip()
+                        .cast(pl.Float64, strict=False)
+                        .alias("JailFee"),
+                        pl.col("Sentence")
+                        .str.extract(r"Costs\: (.+?)Fine\:")
+                        .str.replace(r"Fine.+", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("Costs"),
+                        pl.col("Sentence")
+                        .str.extract(r"Fine\:(.+?)Crime Victims")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("Fine"),
+                        pl.col("Sentence")
+                        .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
+                        .str.strip()
+                        .alias("CrimeVictimsFee"),
+                        pl.col("Sentence")
+                        .str.extract(r"Municipal Court\:(.+?)Fine Suspended")  ## NONE
+                        .str.replace(r"X-\$", "")
+                        .str.strip()
+                        .cast(pl.Float64, strict=False)
+                        .alias("MunicipalCourt"),
+                        pl.col("Sentence")
+                        .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
+                        .str.strip()
+                        .alias("FineSuspended"),
+                        pl.col("Sentence")
+                        .str.extract(r"Immigration Fine\: (.+?)Fine")
+                        .str.replace(r"X\-\$", "")
+                        .str.strip()
+                        .cast(pl.Float64, strict=False)
+                        .alias("ImmigrationFine"),
+                        pl.col("Sentence")
+                        .str.extract(r"Fine Imposed\: (.+?) Alias Warrant")
+                        .str.strip()
+                        .cast(pl.Float64, strict=False)
+                        .alias("FineImposed"),
+                        pl.col("Sentence")
+                        .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing")
+                        .str.replace(r"Prelim Hearing.+", "")
+                        .str.strip()
+                        .alias("DrugDocketFees"),
+                        pl.col("Sentence")
+                        .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
+                        .str.replace(r"Amt.+", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("PrelimHearing"),
+                        pl.col("Sentence")
+                        .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
+                        .str.replace_all(r"[A-Z\s]|\-|\$", "")
+                        .cast(pl.Float64, strict=False)
+                        .alias("AmtOverMinimumCVF"),
+                        pl.col("Sentence")
+                        .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
+                        .str.strip()
+                        .alias("WCFeeDA"),
+                        pl.col("Sentence")
+                        .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
+                        .str.strip()
+                        .alias("RemovalBill"),
+                        pl.col("Sentence")
+                        .str.extract(r"Crime History Fee\: (.+?) SX10")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("CrimeHistoryFee"),
+                        pl.col("Sentence")
+                        .str.extract(r"SX10\: (.+?)License Suspension Fee")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("SX10"),
+                        pl.col("Sentence")
+                        .str.extract(r"License Suspension Fee\: (.+?) WC Fee 85%")
+                        .str.replace_all(r"[A-Z\s]+", "")
+                        .cast(pl.Float64, strict=False)
+                        .alias("LicenseSuspensionFee"),
+                        pl.col("Sentence")
+                        .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:")
+                        .str.replace(r"Demand Reduction Hearing.+", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("WCFee85"),
+                        pl.col("Sentence")
+                        .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee")
+                        .str.replace_all(r"[A-Z]\-|\s|\$", "")
+                        .str.strip()
+                        .cast(pl.Float64, strict=False)
+                        .alias("DemandReductionHearing"),
+                        pl.col("Sentence")
+                        .str.extract(r"Drug User Fee\: (.+?) Subpoena")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("DrugUserFee"),
+                        pl.col("Sentence")
+                        .str.extract(r"Subpoena\: (.+?) Attorney Fees")
+                        .str.replace_all(r"[X\-\s\$]", "")
+                        .cast(pl.Float64, strict=False)
+                        .alias("Subpoena"),
+                        pl.col("Sentence")
+                        .str.extract(
+                            r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
+                        )
+                        .alias("ImposedConfinementPeriod"),
+                        pl.col("Sentence")
+                        .str.extract(
+                            r"Total Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
+                        )
+                        .alias("TotalConfinementPeriod"),
+                        pl.col("Sentence")
+                        .str.extract(
+                            r"Suspended Confinement Period (\d+ Years, \d+ Months, \d+ Days\.)"
+                        )
+                        .alias("SuspendedConfinementPeriod"),
+                        pl.col("Sentence")
+                        .str.extract(r"Boot Camp\: (.+?) (Penitentiary|Life Without Parole)")
+                        .str.replace(r"Penitentiary.+", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("BootCamp"),
+                        pl.col("Sentence")
+                        .str.extract(
+                            r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1
+                        )
+                        .str.replace(r"Death.+", "")
+                        .str.replace(r"Restitution.+", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("LifeWithoutParole"),
+                        pl.col("Sentence")
+                        .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1)
+                        .str.strip()
+                        .alias("Split"),
+                        pl.col("Sentence")
+                        .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
+                        .str.strip()
+                        .alias("ConcurrentSentence"),
+                        pl.col("Sentence")
+                        .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
+                        .str.strip()
+                        .alias("ConsecutiveSentence"),
+                        pl.col("Sentence")
+                        .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
+                        .str.replace_all(r"[-0\s]", "")
+                        .cast(pl.Categorical)
+                        .alias("ElectronicMonitoring"),
+                        pl.col("Sentence")
+                        .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
+                        .str.replace_all(r"Death\: Life\:", "")
+                        .str.replace(r'Life Without Parole\: ?X?','')
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("ReverseSplit"),
+                        pl.col("Sentence")
+                        .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
+                        .alias("CoterminousSentence"),
+                        pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
+                        pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
+                        pl.col("Sentence")
+                        .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("ChainGang"),
+                        pl.col("Sentence")
+                        .str.extract(r"Jail\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("Jail"),
+                        pl.col("Sentence")
+                        .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)")
+                        .alias("CommunityServiceHrs"),
+                        pl.col("Sentence")
+                        .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("JailDiversion"),
+                        pl.col("Sentence")
+                        .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
+                        .cast(pl.Categorical)
+                        .alias("Alcoholics Anonymous"),
+                        pl.col("Sentence")
+                        .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
+                        .cast(pl.Categorical)
+                        .alias("BadCheckSchool"),
+                        pl.col("Sentence")
+                        .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("InformalProbation"),
+                        pl.col("Sentence")
+                        .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s")
+                        .cast(pl.Categorical)
+                        .alias("CourtReferralProgram"),
+                        pl.col("Sentence")
+                        .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
+                        .alias("CommunityService"),
+                        pl.col("Sentence")
+                        .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
+                        .alias("AlternativeSentencing"),
+                        pl.col("Sentence")
+                        .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
+                        .alias("PreTrialDiversion"),
+                        pl.col("Sentence")
+                        .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
+                        .cast(pl.Categorical)
+                        .alias("DUISchool"),
+                        pl.col("Sentence")
+                        .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
+                        .cast(pl.Categorical)
+                        .alias("DefensiveDrivingSchool"),
+                        pl.col("Sentence")
+                        .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("DocCommunityCorrections"),
+                        pl.col("Sentence")
+                        .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("JailCommunityCorrections"),
+                        pl.col("Sentence")
+                        .str.extract(r"Mental Health\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("MentalHealth"),
+                        pl.col("Sentence")
+                        .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("AngerManagementProgram"),
+                        pl.col("Sentence")
+                        .str.extract(r"Drug Court\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("DrugCourt"),
+                        pl.col("Sentence")
+                        .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
+                        .cast(pl.Categorical)
+                        .alias("DocDrugProgram"),
+                        pl.col("Sentence")
+                        .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("DrugMeasureUnit"),
+                        pl.col("Sentence")
+                        .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("DrugNearProject"),
+                        pl.col("Sentence")
+                        .str.extract(r"Drugs Near School\: (.+?)Habitual Offender")
+                        .str.replace(r"Habitual Offender\:", "")
+                        .str.replace(r"Sex Offender Community Notification\:", "")
+                        .str.replace(r"Drug Volume\:", "")
+                        .str.replace(r"Drug\:", "")
+                        .str.replace(r"Drug Code\:\s?\d*", "")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("DrugsNearSchool"),
+                        pl.col("Sentence")
+                        .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
+                        .str.strip()
+                        .cast(pl.Categorical)
+                        .alias("HabitualOffender"),
+                        pl.col("Sentence")
+                        .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
+                        .str.replace_all(r"[X\s0-9]", "")
+                        .str.replace(r"\.", "")
+                        .cast(pl.Categorical)
+                        .alias("SexOffenderCommunityNotification"),
+                        pl.col("Sentence")
+                        .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
+                        .cast(pl.Float64, strict=False)
+                        .alias("DrugVolume"),
+                        pl.col("Sentence")
+                        .str.extract(r"Drug Code\: (.+?)Habitual Offender Number")
+                        .str.strip()
+                        .cast(pl.Int64, strict=False)
+                        .alias("DrugCode"),
+                        pl.col("Sentence")
+                        .str.extract(r"Habitual Offender Number\: (.+?)Victim")
+                        .str.strip()
+                        .alias("HabitualOffenderNumber"),
+                        pl.col("Sentence")
+                        .str.extract(r"Victim DOB\:\s+(\d?\d?/?\d?\d?/?\d?\d?\d?\d?)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("VictimDOB"),
+                    ]
+                )
+                sent = sent.drop_nulls("Number")
+                sent = sent.fill_null("")
+            self._sentences = sent
+            return self._sentences
+    
+    def settings(self):
+        if isinstance(self._settings, pl.DataFrame):
+            return self._settings
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing settings..."):
+                df = self.archive.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("AllPagesText").str.extract(r'Description\:\s*\n\s*(?s)Settings(.+?)Court Action').str.split("\n").alias("Settings")
+                    ]
+                )
+                df = df.explode("Settings")
+                df = df.with_columns(pl.col("Settings").str.strip())
+                df = df.filter(pl.col("Settings").str.contains("[A-Z]"))
+                df = df.filter(pl.col("Settings").str.contains("Date").is_not())
+                df = df.filter(pl.col("Settings").is_null().is_not())
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("Settings").str.extract(r'^(\d) ').cast(pl.Int64, strict=False).alias("Number"),
+                    pl.col("Settings").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
+                    pl.col("Settings").str.extract(r'\d\d?/\d\d?/\d\d\d\d (\d\d\d)').alias("Que"),
+                    pl.col("Settings").str.extract(r'\d\d?/\d\d?/\d\d\d\d \d\d\d (\d\d?\:\d\d [A|P]M)').alias("Time"),
+                    pl.col("Settings").str.extract(r'\d\d?/\d\d?/\d\d\d\d \d\d\d \d\d?\:\d\d [A|P]M (.+)').alias("Description")
+                ])
+            self._settings = df
+            return self._settings
+    
+    def case_action_summary(self):
+        if isinstance(self._case_action_summary, pl.DataFrame):
+            return self._case_action_summary
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing case action summaries..."):
+                cas = self.archive.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("AllPagesText")
+                        .str.extract(r'(?s)Case Action Summary\s*\n\s*Operator\s*\n\s*(.+?)Date')
+                        .str.split("\n")
+                        .alias("CAS"),
+                    ]
+                )
+                cas = cas.explode("CAS")
+                cas = cas.with_columns(pl.col("CAS").str.strip().str.replace(r'^(..Alacourt\.com \d\d?/\d\d?/\d\d\d\d \d)','').str.strip())
+                cas = cas.filter(pl.col("CAS").str.contains("[A-Z]"))
+                cas = cas.with_columns([
+                    pl.col("CAS").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)$').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
+                    pl.col("CAS").str.extract(r'(\d\d?\:\d\d [A|P]M) \d\d?/\d\d?/\d\d\d\d$').alias("Time"),
+                    pl.col("CAS").str.extract(r'([^\s]{4}) \d\d?\:\d\d [A|P]M \d\d?/\d\d?/\d\d\d\d$').alias("Code"),
+                    pl.col("CAS").str.extract(r'(.+) [^\s]{4} \d\d?\:\d\d [A|P]M \d\d?/\d\d?/\d\d\d\d$').str.replace(r'^([A-Z]{3} )','').alias("Comments"),
+                    pl.col("CAS").str.extract(r'^([A-Z]{3}) ').alias("Operator")
+                ])
+                cas = cas.select("CaseNumber", "Date", "Time", "Code", "Comments", "Operator")
+                cas = cas.filter(pl.col("Date").is_null().is_not())
+            self._case_action_summary = cas
+            return self._case_action_summary
+    
+    def financial_history(self):
+        if isinstance(self._financial_history, pl.DataFrame):
+            return self._financial_history
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing financial history..."):
+                fh = self.archive.with_columns(
+                    pl.col("AllPagesText")
+                    .str.extract_all(
+                        r"(\d\d/\d\d/\d\d\d\d)\s(RECEIPT|CREDIT)\s(\$\d+\.\d\d)\s(\w\d\d\d)\s(\d\d\d)\s(\w)\s(....)\s(\d{8})\s(\d{7})\s(\w{3})"
+                    )
+                    .alias("FinancialHistory")
+                )
+                fh = fh.explode("FinancialHistory")
+                fh = fh.with_columns(
+                    [
+                        pl.col("FinancialHistory")
+                        .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
+                        .str.to_date("%m/%d/%Y", strict=False)
+                        .alias("TransactionDate"),
+                        pl.col("FinancialHistory")
+                        .str.extract(r"(RECEIPT|CREDIT)")
+                        .alias("Description"),
+                        pl.col("FinancialHistory")
+                        .str.extract(r"(\$\d+\.\d\d)")
+                        .str.replace(r"\$", "")
+                        .str.strip()
+                        .cast(pl.Float64, strict=False)
+                        .alias("Amount"),
+                        pl.col("FinancialHistory")
+                        .str.extract(r"\s(\w\d\d\d)\s")
+                        .alias("FromParty"),
+                        pl.col("FinancialHistory").str.extract(r"\s(\d\d\d)\s").alias("ToParty"),
+                        pl.col("FinancialHistory").str.extract(r"\s(\w)\s").alias("AdminFee"),
+                        pl.col("FinancialHistory")
+                        .str.extract(r"\s([A-Z]{2}[A-Z0-9]{2})\s")
+                        .alias("DisbursementAccount"),
+                        pl.col("FinancialHistory")
+                        .str.extract(r"\s([0-9]{8})\s")
+                        .alias("ReceiptNumber"),
+                        pl.col("FinancialHistory")
+                        .str.extract(r"\s([0-9]{7})\s")
+                        .alias("TransactionBatch"),
+                        pl.col("FinancialHistory").str.extract(r"\s([A-Z]{3})$").alias("Operator"),
+                    ]
+                )
+                fh = fh.select(
+                    "CaseNumber",
+                    "TransactionDate",
+                    "Description",
+                    "DisbursementAccount",
+                    "TransactionBatch",
+                    "ReceiptNumber",
+                    "Amount",
+                    "FromParty",
+                    "ToParty",
+                    "AdminFee",
+                    "Operator",
+                )
+                fh = fh.drop_nulls()
+                fh = fh.fill_null("")
+            self._financial_history = fh
+            return self._financial_history
+    
+    def witnesses(self):
+        if isinstance(self._witnesses, pl.DataFrame):
+            return self._witnesses
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing witnesses tables..."):
+                df = self.archive
+                df = df.with_columns(
+                    pl.col("AllPagesText").str.extract(r'(?s)SJIS Witness List\s*\n\s*Date Issued\s*\n\s*Subpoena(.+?)Date').alias("Witnesses")
+                )
+                df = df.with_columns(
+                    pl.col("Witnesses").apply(lambda x: re.split(r'( [A-Z0-9]{4}\s*\n)', x))
+                )
+                df = df.with_columns([
+                    pl.col("Witnesses").apply(lambda x: x[1::2]).alias("WitnessNo"),
+                    pl.col("Witnesses").apply(lambda x: x[0::2][0:-1]).alias("Row")
+                ])
+                df = df.explode("WitnessNo","Row")
+                df = df.with_columns([
+                    pl.col("WitnessNo").str.strip(),
+                    pl.col("Row").str.replace("\n","").str.strip()
+                ])
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("WitnessNo").str.strip(),
+                    pl.col("Row").str.extract(r'^(.+?) \d\d\d').str.replace("PROCESS SERVER", "").str.replace("SERVED PERSONALLY","").str.replace("CERTIFIED MAIL","").str.replace("OTHER","").str.replace(r'..Alacourt\.com \d\d?/\d\d/\d\d\d\d \d','').str.strip().alias("Name"),
+                    pl.col("Row").str.extract(r' (\d\d\d) ').alias("RequestingParty"),\
+                    pl.col("Row").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)$').alias("DateIssued"),
+                    pl.col("Row").str.extract(r' \d\d\d ([A-Z\s]+)').str.strip().alias("IssuedType"),
+                    pl.col("Row").str.extract(r' \d\d\d [A-Z\s]+ (\d\d?/\d\d?/\d\d\d\d) \d\d?/\d\d?/\d\d\d\d').alias("DateServed"),
+                    pl.col("Row").str.extract(r'^(SERVED PERSONALLY|CERTIFIED MAIL|PROCESS SERVER|OTHER)').alias("ServiceType")
+                ])
+                df = df.drop_nulls("WitnessNo")
+            self._witnesses = df
+            return self._witnesses
+    
+    def attorneys(self):
+        if isinstance(self._attorneys, pl.DataFrame):
+            return self._attorneys
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing attorneys tables..."):
+                df = self.archive.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("AllPagesText").str.extract(r'(?s)Attorney Code\s*\n\s*(.+?)Warrant').alias("Attorneys")
+                    ]
+                )
+                df = df.drop_nulls("Attorneys")
+                df = df.with_columns(
+                    pl.col("Attorneys").apply(lambda x: re.split(r'(\s*[A-Z0-9]{6}\s*\n)', x))
+                )
+                df = df.with_columns([
+                    pl.col("Attorneys").apply(lambda x: x[0::2][0:-1]).alias("Row"),
+                    pl.col("Attorneys").apply(lambda x: x[1::2]).alias("AttorneyCode")
+                ])
+                df = df.explode("Row", "AttorneyCode")
+                df = df.with_columns(pl.col("Row").str.strip())
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("Row").str.extract(r'(Attorney \d+|Prosecutor \d+)$').alias("Number"),
+                    pl.col("AttorneyCode").str.strip(),
+                    pl.col("Row").str.extract(r'^(\w-\w+)').alias("TypeOfCounsel"),
+                    pl.col("Row").str.extract(r'^(\w-\w+\s)?(.+?)([^\s]+\s?@\s?[^\s\.]+\s?\.\s?[A-Z]+)', group_index=2).str.strip().alias("Name"),
+                    pl.col("Row").str.extract(r'([^\s]+\s?@\s?[^\s\.]+\s?\.\s?[A-Z]+)', group_index=1).str.replace(r' ','').alias("Email"),
+                    pl.col("Row").str.extract(r'(\(\d\d\d\) \d\d\d-\d\d\d\d) (Attorney \d+|Prosecutor \d+)', group_index=1).alias("Phone")
+                ])
+            self._attorneys = df
+            return self._attorneys
+    
+    def images(self):
+        if isinstance(self._images, pl.DataFrame):
+            return self._images
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing images tables..."):
+                images = self.archive.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("AllPagesText")
+                        .str.extract(
+                            r"(Images\s+?Pages)([^\\n]*)(END OF THE REPORT)", group_index=2
+                        )
+                        .str.strip()
+                        .alias("ImagesChunk"),
+                    ]
+                )
+                images = images.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("ImagesChunk")
+                        .str.replace_all("© Alacourt.com", "", literal=True)
+                        .str.split("\n")
+                        .alias("Images"),
+                    ]
+                )
+                images = images.explode("Images")
+                images = images.filter(pl.col("Images").str.contains(r"[A-Za-z0-9]"))
+                images = images.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("Images")
+                        .str.replace_all(r"[A-Z][a-z]+", " ")
+                        .str.replace_all(r"[\s\:]+", " ")
+                        .str.strip(),
+                    ]
+                )
+                images = images.select(
+                    [
+                        pl.col("CaseNumber"),
+                        pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=1).str.to_date('%-m/%-d/%Y', strict=False).alias("Date"),
+                        pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=2).alias("Time"),
+                        pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').cast(pl.Int64, strict=False).alias("Doc#"),
+                        pl.col("Images").str.extract(r'^\d\s(.+?)\s\d').alias("Title"),
+                        pl.col("Images").str.extract(r'^\d\s.+?\s\d\s(.+?)\s\d\d?/\d\d?/\d\d\d\d').alias("Description"),
+                        pl.col("Images").str.extract(r'^(\d)\s').cast(pl.Int64, strict=False).alias("Pages")
+                    ])
+                images = images.with_columns(
+                    pl.concat_str([
+                        pl.col("Time").str.extract(r'^(\d\d?)'),
+                        pl.lit(":"),
+                        pl.col("Time").str.extract(r'\d\d? (\d\d)'),
+                        pl.lit(":"),
+                        pl.col("Time").str.extract(r'\d\d? \d\d (\d\d [A|P]M)')
+                    ]).alias("Time")
+                )
+                images = images.filter(pl.col("Date").is_null().is_not())
+                images = images.fill_null('')
+            self._images = images
+            return self._images
+    
+    def tables(self):
+        return {
+            'cases': self.cases(),
+            'charges': self.charges(),
+            'fees': self.fees(),
+            'sentences': self.sentences(),
+            'financial-history': self.financial_history(),
+            'witnesses': self.witnesses(),
+            'attorneys': self.attorneys(),
+            'images': self.images(),
+            'case-action-summary': self.case_action_summary()
+        }
+    
+    def summary(self, pairs):
+        if isinstance(pairs, str):
+            self._pairs = read(pairs)
+        if "Search" in self._pairs.columns:
+            self._pairs = self._pairs.select([
+                pl.col("Name"),
+                pl.col("Search").alias("AIS / Unique ID")
+            ])
+            self._pairs = self._pairs.unique()
+        if not self.is_read:
+            self.read()
+        cases = self.cases()
+        charges = self.charges()
+        with console.status("Creating summary..."):
+            cases = cases.select("CaseNumber", "Name", "DOB", "Race", "Sex")
+            cases = cases.with_columns(
                 [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                    pl.col("Race").cast(pl.Utf8, strict=False),
+                    pl.col("Sex").cast(pl.Utf8, strict=False),
                 ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract(
-                r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
-                group_index=1,
             )
-            .str.replace_all("Case Number:", "", literal=True)
-            .str.replace(r"C$", "")
-            .str.strip()
-            .alias("Name"),
-            pl.col("AllPagesText")
-            .str.extract_all(
-                r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
-            )
-            .alias("RE_Charges"),
-            pl.col("AllPagesText")
-            .str.extract(r"(Total:.+\$[^\n]*)")
-            .str.replace_all(r"[^0-9|\.|\s|\$]", "")
-            .str.extract_all(r"\s\$\d+\.\d{2}")
-            .arr.get(2)
-            .str.replace_all(r"[^0-9\.]", "")
-            .cast(pl.Float64, strict=False)
-            .alias("RAWTotalBalance"),
-            pl.col("AllPagesText")
-            .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
-            .str.extract_all(r"\$\d+\.\d{2}")
-            .arr.get(-1)
-            .str.replace(r"[\$\s]", "")
-            .cast(pl.Float64, strict=False)
-            .alias("RAWD999"),
-        ]
-    )
-
-    all_charges = all_charges.explode("RE_Charges").select(
-        [
-            pl.col("Name"),
-            pl.col("CaseNumber"),
-            pl.col("RE_Charges")
-            .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
-            .str.strip()
-            .alias("Charges"),
-            pl.when(pl.col("RAWTotalBalance").is_null())
-            .then(pl.lit(0.0))
-            .otherwise(pl.col("RAWTotalBalance"))
-            .alias("TotalBalance"),
-            pl.when(pl.col("RAWD999").is_null())
-            .then(pl.lit(0.0))
-            .otherwise(pl.col("RAWD999"))
-            .alias("TotalD999"),
-        ]
-    )
-
-    dlog(all_charges, all_charges.columns, cf=debug)
-    return all_charges
-
-
-def _explode_fees(df, debug=False):
-    cases = df.with_columns(
-        [
-            pl.concat_str(
+            fch = charges.filter(pl.col("Filing"))
+            fch = fch.join(self._pairs, on="Name", how="outer")
+            fch = fch.groupby("AIS / Unique ID").all()
+            fch = fch.select(
                 [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
-                ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract_all(
-                r"(ACTIVE [^\(\n]+\$[^\(\n]+ACTIVE[^\(\n]+[^\n]|Total:.+\$[^\n]*)"
-            )
-            .alias("RE_Fees"),
-        ]
-    )
-    all_fees = cases.explode("RE_Fees").select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("RE_Fees")
-            .str.replace_all(r"[^A-Z0-9|\.|\s|\$|\n]", " ")
-            .str.strip()
-            .alias("Fees"),
-        ]
-    )
-    dlog(all_fees.columns, cf=debug)
-    return all_fees
-
+                    pl.col("AIS / Unique ID"),
+                    pl.col("CERVDisqCharge").list.count_match(True).alias("CERVChargesCount"),
+                    pl.col("PardonDisqCharge")
+                    .list.count_match(True)
+                    .alias("PardonToVoteChargesCount"),
+                    pl.col("PermanentDisqCharge")
+                    .list.count_match(True)
+                    .alias("PermanentDisqChargesCount"),
+                    pl.col("ChargesSummary").list.join(", ")
+                    .str.replace_all(r"null,?", "")
+                    .str.strip()
+                    .str.replace(r",$", "")
+                    .str.replace_all(r"\s+", " ")
+                    .alias("FilingCharges"),
 
-def _split_cases(df, debug=False):
-    cases = df.with_columns(
-        [
-            pl.col("AllPagesText")
-            .str.extract(
-                r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
-                group_index=1,
-            )
-            .str.replace("Case Number:", "", literal=True)
-            .str.replace(r"C$", "")
-            .str.strip()
-            .alias("Name"),
-            pl.col("AllPagesTextNoNewLine")
-            .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
-            .str.replace(r"(SSN)", "")
-            .str.replace(r"Alias", "")
-            .str.replace(r"\:", "")
-            .str.strip()
-            .alias("Alias"),
-            pl.col("AllPagesText")
-            .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
-            .str.replace(r"[^\d/]", "")  # _all
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("DOB"),
-            pl.concat_str(
-                [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
                 ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract(r"(Phone: )(.+)", group_index=2)
-            .str.replace_all(r"[^0-9]", "")
-            .str.slice(0, 10)
-            .str.replace(r"(.{3}0000000)", "")  # _all
-            .alias("RE_Phone"),
-            pl.col("AllPagesText")
-            .str.extract(r"(B|W|H|A)/(?:F|M)")
-            .cast(pl.Categorical)
-            .alias("Race"),
-            pl.col("AllPagesText")
-            .str.extract(r"(?:B|W|H|A)/(F|M)")
-            .cast(pl.Categorical)
-            .alias("Sex"),
-            pl.col("AllPagesText")
-            .str.extract(r"(?:Address 1:)(.+)(?:Phone)*?", group_index=1)
-            .str.replace(r"(Phone.+)", "")
-            .str.strip()
-            .alias("Address1"),
-            pl.col("AllPagesText")
-            .str.extract(r"(?:Address 2:)(.+)")
-            .str.strip()
-            .alias("Address2"),
-            pl.col("AllPagesText")
-            .str.extract(r"(?:Zip: )(.+)", group_index=1)
-            .str.replace(r"[A-Za-z\:\s]+", "")
-            .str.strip()
-            .alias("ZipCode"),
-            pl.col("AllPagesText")
-            .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
-            .str.strip()
-            .alias("City"),
-            pl.col("AllPagesText")
-            .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=2)
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("State"),
-            pl.col("AllPagesText")
-            .str.extract(r"(Total:.+\$[^\n]*)")
-            .str.replace_all(r"[^0-9|\.|\s|\$]", "")
-            .str.extract_all(r"\s\$\d+\.\d{2}")
-            .alias("TOTALS"),
-            pl.col("AllPagesText")
-            .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
-            .str.extract_all(r"\$\d+\.\d{2}")
-            .arr.get(-1)
-            .str.replace(r"[\$\s]", "")
-            .cast(pl.Float64, strict=False)
-            .alias("D999RAW"),
-            pl.col("AllPagesText")
-            .str.extract_all(r"(\w{2}\d{12})")
-            .arr.join("/")
-            .alias("RelatedCases"),
-            pl.col("AllPagesText")
-            .str.extract(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("FilingDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("CaseInitiationDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("ArrestDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("OffenseDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("IndictmentDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("YouthfulDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"AL Institutional Service Num: ([^\na-z])")
-            .str.strip()
-            .alias("ALInstitutionalServiceNum"),
-            pl.col("AllPagesText")
-            .str.extract(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("Retrieved"),
-            pl.col("AllPagesText")
-            .str.extract(r"Jury Demand: ([A-Z]+)")
-            .cast(pl.Categorical)
-            .alias("JuryDemand"),
-            pl.col("AllPagesText")
-            .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
-            .cast(pl.Categorical)
-            .alias("InpatientTreatmentOrdered"),
-            pl.col("AllPagesText")
-            .str.extract(r"Trial Type: ([A-Z]+)")
-            .str.replace(r"[S|N]$", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("TrialType"),
-            pl.col("AllPagesText")
-            .str.extract(r"Case Number: (\d\d-\w+) County:")
-            .str.strip()
-            .alias("County"),
-            pl.col("AllPagesText")
-            .str.extract(r"Judge: ([A-Z\-\.\s]+)")
-            .str.rstrip("T")
-            .str.strip()
-            .alias("Judge"),
-            pl.col("AllPagesText")
-            .str.extract(r"Probation Office \#: ([0-9\-]+)")
-            .alias("PROBATIONOFFICENUMBERRAW"),
-            pl.col("AllPagesText")
-            .str.extract(r"Defendant Status: ([A-Z\s]+)")
-            .str.rstrip("J")
-            .str.replace(r"\n", " ")
-            .str.replace(r"\s+", " ")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("DefendantStatus"),
-            pl.col("AllPagesText")
-            .str.extract(r"([^0-9]+) Arresting Agency Type:")
-            .str.replace(r"^\-.+", "")
-            .str.replace(r"County\:", "")
-            .str.replace(r"Defendant Status\:", "")
-            .str.replace(r"Judge\:", "")
-            .str.replace(r"Trial Type\:", "")
-            .str.replace(r"Probation Office \#\:", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("ArrestingAgencyType"),
-            pl.col("AllPagesText")
-            .str.extract(r"Arresting Officer: ([A-Z\s]+)")
-            .str.replace(r"[\s\n]+[A-Z0-9]$", "")
-            .str.strip()
-            .alias("ArrestingOfficer"),
-            pl.col("AllPagesText")
-            .str.extract(r"Probation Office Name: ([A-Z0-9]+)")
-            .alias("ProbationOfficeName"),
-            pl.col("AllPagesText")
-            .str.extract(r"Traffic Citation \#: ([A-Z0-9]+)")
-            .alias("TrafficCitationNumber"),
-            pl.col("AllPagesText")
-            .str.extract(r"Previous DUI Convictions: (\d{3})")
-            .str.strip()
-            .cast(pl.Int64, strict=False)
-            .alias("PreviousDUIConvictions"),
-            pl.col("AllPagesText")
-            .str.extract(r"Case Initiation Type: ([A-Z\s]+)")
-            .str.rstrip("J")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("CaseInitiationType"),
-            pl.col("AllPagesText")
-            .str.extract(r"Domestic Violence: ([YES|NO])")
-            .cast(pl.Categorical)
-            .alias("DomesticViolence"),
-            pl.col("AllPagesText")
-            .str.extract(r"Agency ORI: ([A-Z\s]+)")
-            .str.rstrip("C")
-            .str.replace(r"\n", "")
-            .str.replace_all(r"\s+", " ")
-            .str.strip()
-            .alias("AgencyORI"),
-            pl.col("AllPagesText")
-            .str.extract(r"Driver License N°: ([A-Z0-9]+)")
-            .alias("DLRAW"),
-            pl.col("AllPagesText")
-            .str.extract(r"SSN: ([X\d]{3}\-[X\d]{2}-[X\d]{4})")
-            .alias("SSN"),
-            pl.col("AllPagesText")
-            .str.extract(r"([A-Z0-9]{11}?) State ID:")
-            .alias("SIDRAW"),
-            pl.col("AllPagesText")
-            .str.extract(r"Weight: (\d*)", group_index=1)
-            .cast(pl.Int64, strict=False)
-            .alias("Weight"),
-            pl.col("AllPagesText")
-            .str.extract(r"Height : (\d'\d{2})")
-            .alias("RAWHEIGHT"),
-            pl.col("AllPagesText")
-            .str.extract(r"Eyes/Hair: (\w{3})/(\w{3})", group_index=1)
-            .alias("Eyes"),
-            pl.col("AllPagesText")
-            .str.extract(r"Eyes/Hair: (\w{3})/(\w{3})", group_index=2)
-            .alias("Hair"),
-            pl.col("AllPagesText")
-            .str.extract(r"Country: (\w*+)")
-            .str.replace(r"(Enforcement|Party)", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("Country"),
-            pl.col("AllPagesText")
-            .str.extract(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("WarrantIssuanceDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("WarrantActionDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Warrant Issuance Status: (\w+)")
-            .str.replace(r"Description", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("WarrantIssuanceStatus"),
-            pl.col("AllPagesText")
-            .str.extract(r"Warrant Action Status: (\w+)")
-            .str.replace(r"Description", "")
-            .str.strip()
-            .alias("WarrantActionStatus"),
-            pl.col("AllPagesText")
-            .str.extract(r"Warrant Location Status: (\w+)")
-            .str.replace(r"Description", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("WarrantLocationStatus"),
-            pl.col("AllPagesText")
-            .str.extract(r"Number Of Warrants: (\d{3}\s\d{3})")
-            .str.strip()
-            .alias("NumberOfWarrants"),
-            pl.col("AllPagesText")
-            .str.extract(r"Bond Type: (\w+)")  # +
-            .str.replace(r"Bond", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("BondType"),
-            pl.col("AllPagesText")
-            .str.extract(r"Bond Type Desc: ([A-Z\s]+)")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("BondTypeDesc"),
-            pl.col("AllPagesText")
-            .str.extract(r"([\d\.]+) Bond Amount:")
-            .cast(pl.Float64, strict=False)
-            .alias("BondAmt"),
-            pl.col("AllPagesText")
-            .str.extract(r"Bond Company: ([A-Z0-9]+)")
-            .str.rstrip("S")
-            .alias("BondCompany"),
-            pl.col("AllPagesText")
-            .str.extract(r"Surety Code: ([A-Z0-9]{4})")
-            .alias("SuretyCode"),
-            pl.col("AllPagesText")
-            .str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("BondReleaseDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("FailedToAppearDate"),
-            pl.col("AllPagesText")
-            .str.extract(
-                r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:"
             )
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("BondsmanProcessIssuance"),
-            pl.col("AllPagesText")
-            .str.extract(r"Bondsman Process Return: (.*?) Number of Subponeas")
-            .str.strip()
-            .alias("BondsmanProcessReturn"),
-            pl.col("AllPagesText")
-            .str.extract(r"([\n\s/\d]*?) Appeal Court:")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("AppealDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"([A-Z\-\s]+) Appeal Case Number")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("AppealCourt"),
-            pl.col("AllPagesText")
-            .str.extract(r"Orgin Of Appeal: ([A-Z\-\s]+)")
-            .str.rstrip("L")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("OriginOfAppeal"),
-            pl.col("AllPagesText")
-            .str.extract(r"Appeal To Desc: ([A-Z\-\s]+)")
-            .str.replace(r"[\s\n]+[A-Z0-9]$", "")
-            .str.rstrip("O")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("AppealToDesc"),
-            pl.col("AllPagesText")
-            .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
-            .str.rstrip("A")
-            .str.replace_all(r"\n", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("AppealStatus"),
-            pl.col("AllPagesText")
-            .str.extract(r"Appeal To: (\w*) Appeal")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("AppealTo"),
-            pl.col("AllPagesText")
-            .str.extract(r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.replace_all(r"[\n\s:\-]", "")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("LowerCourtAppealDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.replace_all(r"[\n\s:\-]", "")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("DispositionDateOfAppeal"),
-            pl.col("AllPagesText")
-            .str.extract(r"Disposition Type Of Appeal: [^A-Za-z]+")
-            .str.replace_all(r"[\n\s:\-]", "")
-            .str.strip()
-            .alias("DispositionTypeOfAppeal"),
-            pl.col("AllPagesText")
-            .str.extract(r"Number of Subponeas: (\d{3})")
-            .str.replace_all(r"[^0-9]", "")
-            .str.strip()
-            .cast(pl.Int64, strict=False)
-            .alias("NumberOfSubpoenas"),
-            pl.col("AllPagesText")
-            .str.extract(r"Updated By: (\w{3})")
-            .str.strip()
-            .alias("AdminUpdatedBy"),
-            pl.col("AllPagesText")
-            .str.extract(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("TransferToAdminDocDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)")
-            .str.replace_all(r"(Transfer Desc:)", "")
-            .str.strip()
-            .alias("TransferDesc"),
-            pl.col("AllPagesText")
-            .str.extract(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("TBNV1"),
-            pl.col("AllPagesText")
-            .str.extract(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)")
-            .str.replace(r"Financial", "")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("TBNV2"),
-            pl.col("AllPagesText")
-            .str.extract(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("TurnOverDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"TurnOver Amt\: \$(\d+\.\d\d)")
-            .cast(pl.Float64, strict=False)
-            .alias("TurnOverAmt"),
-            pl.col("AllPagesText")
-            .str.extract(r"Frequency Amt\: \$(\d+\.\d\d)")
-            .cast(pl.Float64, strict=False)
-            .alias("FrequencyAmt"),
-            pl.col("AllPagesText")
-            .str.extract(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("DueDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("LastPaidDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Payor\: ([A-Z0-9]{4})")
-            .cast(pl.Categorical)
-            .alias("Payor"),
-            pl.col("AllPagesText")
-            .str.extract(r"Enforcement Status\: ([A-Z\:,\s]+)")
-            .str.replace_all(r"\s+", " ")
-            .str.replace(r" F$", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("EnforcementStatus"),
-            pl.col("AllPagesText")
-            .str.extract(r"Frequency\: ([W|M])")
-            .str.replace(r"Cost Paid By\:", "")
-            .str.strip()
-            .alias("Frequency"),
-            pl.col("AllPagesText")
-            .str.extract(r"Placement Status\: (.+)")
-            .str.strip()
-            .alias("PlacementStatus"),
-            pl.col("AllPagesText")
-            .str.extract(r"PreTrial\: (YES|NO)")
-            .cast(pl.Categorical)
-            .alias("PreTrial"),
-            pl.col("AllPagesText")
-            .str.extract(r"PreTrail Date\: (.+)PreTrial")
-            .str.strip()
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("PreTrialDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"PreTrial Terms\: (YES|NO)")
-            .cast(pl.Categorical)
-            .alias("PreTrialTerms"),
-            pl.col("AllPagesText")
-            .str.extract(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("PreTermsDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Delinquent\: (YES|NO)")
-            .cast(pl.Categorical)
-            .alias("Delinquent"),
-            pl.col("AllPagesText")
-            .str.extract(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("DelinquentDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"DA Mailer\: (YES|NO)")
-            .cast(pl.Categorical)
-            .alias("DAMailer"),
-            pl.col("AllPagesText")
-            .str.extract(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("DAMailerDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Warrant Mailer\: (YES|NO)")
-            .cast(pl.Categorical)
-            .alias("WarrantMailer"),
-            pl.col("AllPagesText")
-            .str.extract(r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("WarrantMailerDate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("EnforcementLastUpdate"),
-            pl.col("AllPagesText")
-            .str.extract(r"Updated By\: ([A-Z]{3})")
-            .alias("EnforcementUpdatedBy"),
-        ]
-    )
-    cases = cases.with_columns(
-        [
-            pl.when(pl.col("D999RAW").is_null())
-            .then(pl.lit(0))
-            .otherwise(pl.col("D999RAW"))
-            .alias("D999")
-        ]
-    )
-
-    dlog(cases.columns, cases.shape, "cases raw regex", cf=debug)
-
-    # clean columns, unnest totals
-    cases = cases.with_columns(
-        pl.col("RE_Phone")
-        .str.replace_all(r"[^0-9]|2050000000", "")
-        .alias("CLEAN_Phone"),
-        pl.concat_str([pl.col("Address1"), pl.lit(" "), pl.col("Address2")])
-        .str.replace_all(r"JID: \w{3} Hardship.*|Defendant Information.*", "")
-        .str.strip()
-        .alias("StreetAddress"),
-        pl.col("Name"),
-        pl.when(pl.col("PROBATIONOFFICENUMBERRAW") == "0-000000-00")
-        .then(pl.lit(""))
-        .otherwise(pl.col("PROBATIONOFFICENUMBERRAW"))
-        .alias("ProbationOfficeName"),
-        pl.when(pl.col("DLRAW") == "AL")
-        .then(pl.lit(""))
-        .otherwise(pl.col("DLRAW"))
-        .alias("DriverLicenseNo"),
-        pl.when(pl.col("SIDRAW") == "AL000000000")
-        .then(pl.lit(""))
-        .otherwise(pl.col("SIDRAW"))
-        .alias("StateID"),
-        pl.col("TOTALS")
-        .arr.get(0)
-        .str.replace_all(r"[^0-9\.]", "")
-        .cast(pl.Float64, strict=False)
-        .alias("TotalAmtDue"),
-        pl.col("TOTALS")
-        .arr.get(1)
-        .str.replace_all(r"[^0-9\.]", "")
-        .cast(pl.Float64, strict=False)
-        .alias("TotalAmtPaid"),
-        pl.col("TOTALS")
-        .arr.get(2)
-        .str.replace_all(r"[^0-9\.]", "")
-        .cast(pl.Float64, strict=False)
-        .alias("TotalBalance"),
-        pl.col("TOTALS")
-        .arr.get(3)
-        .str.replace_all(r"[^0-9\.]", "")
-        .cast(pl.Float64, strict=False)
-        .alias("TotalAmtHold"),
-    )
-    cases = cases.with_columns(
-        pl.when(pl.col("CLEAN_Phone").str.n_chars() < 7)
-        .then(None)
-        .otherwise(pl.col("CLEAN_Phone"))
-        .alias("Phone"),
-    )
-
-    dlog(cases.columns, cases.shape, cf=debug)
-
-    cases = cases.fill_null("")
-
-    cases = cases.select(
-        "Retrieved",
-        "CaseNumber",
-        "Name",
-        "Alias",
-        "DOB",
-        "Race",
-        "Sex",
-        "TotalAmtDue",
-        "TotalAmtPaid",
-        "TotalBalance",
-        "TotalAmtHold",
-        "D999",
-        "BondAmt",
-        "Phone",
-        "StreetAddress",
-        "City",
-        "State",
-        "ZipCode",
-        "County",
-        "Country",
-        "SSN",
-        "Weight",
-        "Eyes",
-        "Hair",
-        "FilingDate",
-        "CaseInitiationDate",
-        "ArrestDate",
-        "OffenseDate",
-        "IndictmentDate",
-        "JuryDemand",
-        "InpatientTreatmentOrdered",
-        "TrialType",
-        "Judge",
-        "DefendantStatus",
-        "ArrestingAgencyType",
-        "ArrestingOfficer",
-        "ProbationOfficeName",
-        "PreviousDUIConvictions",
-        "CaseInitiationType",
-        "DomesticViolence",
-        "AgencyORI",
-        "WarrantIssuanceDate",
-        "WarrantActionDate",
-        "WarrantIssuanceStatus",
-        "WarrantActionStatus",
-        "WarrantLocationStatus",
-        "NumberOfWarrants",
-        "BondType",
-        "BondTypeDesc",
-        "BondCompany",
-        "SuretyCode",
-        "BondReleaseDate",
-        "FailedToAppearDate",
-        "BondsmanProcessIssuance",
-        "AppealDate",
-        "AppealCourt",
-        "OriginOfAppeal",
-        "AppealToDesc",
-        "AppealStatus",
-        "AppealTo",
-        "NumberOfSubpoenas",
-        "AdminUpdatedBy",
-        "TransferDesc",
-        "TBNV1",
-        "TBNV2",
-        "DriverLicenseNo",
-        "StateID",
-        "TurnOverDate",
-        "TurnOverAmt",
-        "FrequencyAmt",
-        "DueDate",
-        "LastPaidDate",
-        "Payor",
-        "EnforcementStatus",
-        "Frequency",
-        "PlacementStatus",
-        "PreTrial",
-        "PreTrialDate",
-        "PreTrialTerms",
-        "PreTermsDate",
-        "Delinquent",
-        "DelinquentDate",
-        "DAMailer",
-        "DAMailerDate",
-        "WarrantMailer",
-        "WarrantMailerDate",
-        "EnforcementLastUpdate",
-        "EnforcementUpdatedBy",
-    )
-    return cases
-
-
-def _explode_split_financial_history(df, debug=False):
-    fh = df.with_columns(
-        [
-            pl.concat_str(
+            conv = charges.filter(pl.col("Disposition") & pl.col("Conviction"))
+            conv = conv.join(self._pairs, on="Name", how="outer")
+            conv = conv.groupby("AIS / Unique ID").all()
+            conv = conv.select(
                 [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                    pl.col("AIS / Unique ID"),
+                    pl.col("Conviction")
+                    .list.count_match(True)
+                    .alias("ConvictionCount"),
+                    pl.col("CERVDisqConviction")
+                    .list.count_match(True)
+                    .alias("CERVConvictionCount"),
+                    pl.col("PardonDisqConviction")
+                    .list.count_match(True)
+                    .alias("PardonToVoteConvictionCount"),
+                    pl.col("PermanentDisqConviction")
+                    .list.count_match(True)
+                    .alias("PermanentDisqConvictionCount"),
+                    pl.col("PaymentToRestore").list.mean(),
+                    pl.col("ChargesSummary").list.join(", ")
+                    .str.replace_all(r"null,?", "")
+                    .str.strip()
+                    .str.replace(r",$", "")
+                    .str.replace_all(r"\s+", " ")
+                    .alias("Convictions"),
                 ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract_all(
-                r"(\d\d/\d\d/\d\d\d\d)\s(RECEIPT|CREDIT)\s(\$\d+\.\d\d)\s(\w\d\d\d)\s(\d\d\d)\s(\w)\s(....)\s(\d{8})\s(\d{7})\s(\w{3})"
-            )
-            .alias("FinancialHistory"),
-        ]
-    )
-    fh = fh.explode("FinancialHistory")
-    fh = fh.with_columns(
-        [
-            pl.col("FinancialHistory")
-            .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("TransactionDate"),
-            pl.col("FinancialHistory")
-            .str.extract(r"(RECEIPT|CREDIT)")
-            .alias("Description"),
-            pl.col("FinancialHistory")
-            .str.extract(r"(\$\d+\.\d\d)")
-            .str.replace(r"\$", "")
-            .str.strip()
-            .cast(pl.Float64, strict=False)
-            .alias("Amount"),
-            pl.col("FinancialHistory")
-            .str.extract(r"\s(\w\d\d\d)\s")
-            .alias("FromParty"),
-            pl.col("FinancialHistory").str.extract(r"\s(\d\d\d)\s").alias("ToParty"),
-            pl.col("FinancialHistory").str.extract(r"\s(\w)\s").alias("AdminFee"),
-            pl.col("FinancialHistory")
-            .str.extract(r"\s([A-Z]{2}[A-Z0-9]{2})\s")
-            .alias("DisbursementAccount"),
-            pl.col("FinancialHistory")
-            .str.extract(r"\s([0-9]{8})\s")
-            .alias("ReceiptNumber"),
-            pl.col("FinancialHistory")
-            .str.extract(r"\s([0-9]{7})\s")
-            .alias("TransactionBatch"),
-            pl.col("FinancialHistory").str.extract(r"\s([A-Z]{3})$").alias("Operator"),
-        ]
-    )
-    fh = fh.select(
-        "CaseNumber",
-        "TransactionDate",
-        "Description",
-        "DisbursementAccount",
-        "TransactionBatch",
-        "ReceiptNumber",
-        "Amount",
-        "FromParty",
-        "ToParty",
-        "AdminFee",
-        "Operator",
-    )
-    fh = fh.drop_nulls()
-    fh = fh.fill_null("")
-    return fh
-
-
-def _split_charges(df, debug=False):
-    dlog(df.columns, df.shape, "^ split_charges input param", cf=debug)
-    charges = df.with_columns(
-        [
-            pl.col("Name"),
-            pl.col("CaseNumber"),
-            pl.col("Charges").str.slice(0, 3).alias("Num"),
-            pl.col("Charges").str.slice(4, 4).alias("Code"),
-            pl.col("Charges").str.slice(9, 1).alias("Sort"),
-            pl.col("Charges")
-            .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)", group_index=1)
-            .alias("CourtActionDate"),
-            pl.col("Charges")
-            .str.extract(
-                r"[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}\({0,1}[A-Z]{0,1}\){0,1}\.{0,1}\d{0,1}",
-                group_index=0,
-            )
-            .alias("RAWCITE"),
-            pl.col("Charges")
-            .str.extract(
-                r"(BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)",
-                group_index=1,
-            )
-            .alias("CourtAction"),
-            pl.col("Charges")
-            .apply(
-                lambda x: re.split(
-                    r"[A-Z0-9]{3}\s*?-[A-Z0-9]{3}\s*?-[A-Z0-9]{3}\(*?[A-Z]*?\)*?\(*?[A-Z0-9]*?\)*?\.*?\d*?",
-                    str(x),
-                )
-            )
-            .alias("Split"),
-        ]
-    )
-    dlog(charges, charges.shape, cf=debug)
-    charges = charges.filter(pl.col("Num").str.contains("0"))
-    charges = charges.with_columns(
-        [
-            pl.col("Charges")
-            .str.contains(r"\d\d?/\d\d?/\d\d\d\d")
-            .alias("Disposition"),
-            pl.col("Charges").str.contains(pl.lit("FELONY")).alias("Felony"),
-            pl.col("Charges").str.contains("GUILTY PLEA").alias("GUILTY_PLEA"),
-            pl.col("Charges").str.contains("CONVICTED").alias("CONVICTED"),
-        ]
-    )
-    charges = charges.with_columns(
-        [
-            pl.when(pl.col("Disposition"))
-            .then(pl.col("Split").arr.get(1))
-            .otherwise(pl.col("Split").arr.get(0).str.slice(9))
-            .str.replace(r"-   -", "", literal=True)
-            .str.replace("1STS", "1ST", literal=True)
-            .str.strip()
-            .alias("RAWDESC"),
-            pl.when(pl.col("Disposition"))
-            .then(pl.col("Split").arr.get(0).str.slice(19))
-            .otherwise(pl.col("Split").arr.get(1))
-            .str.strip()
-            .alias("SEG_2"),
-            pl.when(pl.col("Disposition") == True)
-            .then(False)
-            .otherwise(True)
-            .alias("Filing"),
-        ]
-    )
-    dlog(charges.columns, charges.shape, cf=debug)
-    charges = charges.with_columns(
-        [
-            pl.col("SEG_2")
-            .str.extract(
-                r"(TRAFFIC MISDEMEANOR|BOND|FELONY|MISDEMEANOR|OTHER|TRAFFIC|VIOLATION)",
-                group_index=1,
-            )
-            .str.replace("TRAFFIC MISDEMEANOR", "MISDEMEANOR")
-            .alias("TypeDescription"),
-            pl.col("SEG_2")
-            .str.extract(
-                r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
-                group_index=1,
-            )
-            .alias("Category"),
-            pl.col("RAWDESC")
-            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY)")
-            .is_not()
-            .alias("A_S_C_DISQ"),
-            pl.col("Code")
-            .str.contains(
-                r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
-            )
-            .alias("CERV_DISQ_MATCH"),
-            pl.col("Code")
-            .str.contains(
-                r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
-            )
-            .alias("PARDON_DISQ_MATCH"),
-            pl.col("Charges")
-            .str.contains(r"(CM\d\d|CMUR|CAPITAL)")
-            .alias("PERM_DISQ_MATCH"),
-        ]
-    )
-    charges = charges.with_columns(
-        [
-            pl.when(pl.col("A_S_C_DISQ")==None)
-            .then(True)
-            .otherwise(pl.col("A_S_C_DISQ"))
-            .alias("A_S_C_DISQ")
-        ]
-    )
-    charges = charges.filter(pl.col("TypeDescription").str.contains(r"[A-Za-z]"))
-    charges = charges.with_columns(
-        [
-            pl.when(pl.col("GUILTY_PLEA") | pl.col("CONVICTED"))
-            .then(True)
-            .otherwise(False)
-            .alias("Conviction")
-        ]
-    )
-    charges = charges.with_columns(
-        [
-            pl.when(
-                pl.col("CERV_DISQ_MATCH")
-                & pl.col("Felony")
-                & pl.col("Conviction")
-                & pl.col("A_S_C_DISQ")
-            )
-            .then(True)
-            .otherwise(False)
-            .alias("CERVDisqConviction"),
-            pl.when(pl.col("CERV_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
-            .then(True)
-            .otherwise(False)
-            .alias("CERVDisqCharge"),
-            pl.when(
-                pl.col("PARDON_DISQ_MATCH")
-                & pl.col("A_S_C_DISQ")
-                & pl.col("Conviction")
-                & pl.col("Felony")
             )
-            .then(True)
-            .otherwise(False)
-            .alias("PardonDisqConviction"),
-            pl.when(
-                pl.col("PARDON_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ")
-            )
-            .then(True)
-            .otherwise(False)
-            .alias("PardonDisqCharge"),
-            pl.when(
-                pl.col("PERM_DISQ_MATCH")
-                & pl.col("A_S_C_DISQ")
-                & pl.col("Felony")
-                & pl.col("Conviction")
-            )
-            .then(True)
-            .otherwise(False)
-            .alias("PermanentDisqConviction"),
-            pl.when(pl.col("PERM_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
-            .then(True)
-            .otherwise(False)
-            .alias("PermanentDisqCharge"),
-            pl.concat_str([pl.col("CaseNumber"), pl.lit("-"), pl.col("Num")]).alias(
-                "CASENONUM"
-            ),
-        ]
-    )
-    charges = charges.with_columns(
-        [
-            pl.col("TotalBalance"),
-            pl.when(
+            vrr = charges.filter(
                 pl.col("CERVDisqConviction")
                 | pl.col("PardonDisqConviction")
                 | pl.col("PermanentDisqConviction")
             )
-            .then((pl.col("TotalBalance") - pl.col("TotalD999")))
-            .otherwise(None)
-            .alias("PaymentToRestore"),
-            pl.col("RAWDESC").alias("Description"),
-            pl.col("RAWCITE").alias("Cite")
-        ]
-    )
-    charges = charges.fill_null("")
-    fillers = pl.DataFrame({
-        'Code': ['PFI3', 'NWNI', 'VDR1', 'UPCS', 'FRCC', 'T003', 'PMIO', 'UPCC', 'BEMV', 'HARA', 'TET3', 'T042', 'T707', 'SX12', 'TRAK', 'FCDC', 'TOD3', 'UAUV', 'T012', 'FR3D', 'HCOM', 'TP3D', 'VPCC', 'FORF', 'CECE', 'UDCS', 'PRO2', 'MCS1', 'ACHA', 'CECD', 'T627', 'FTCS', 'MCS2', 'PRO3', 'UAUM', 'T527', 'BRA3', 'FMUR', 'MURR', 'FPCC', 'PREC', 'STSA', 'T582', 'CM02', 'VDR4', 'VAPP', 'MAN1', 'VDR1', 'T755', 'TRAO', 'FORM', 'SVIA', 'TRAG', 'DSF1', 'MISC', 'BRA1', 'CEM1', 'CM04', 'IPCD', 'T005', 'T525', 'CM15', 'DUIF', 'T169', 'DUIM', 'T718', 'DVHF', 'TROP', 'CM10', 'CM17', 'CM01', 'VDRU', 'T770', 'ACAL', 'VDRY', 'TRFT', 'FNLE', 'RS3D', 'T806', 'TOS3', 'TSIB', 'T011', 'VAPD', 'T128', 'BHER', 'APPL', 'MRDI', 'UAUY', 'T019', 'T006', 'MAN2', 'CM18', 'NUSE', 'FBAP', 'VDRO', 'CM16', 'EDCO', 'T096', 'THBV', 'ASTM', 'SAVI', 'DVFC', 'T128', 'T071', 'CM07', 'TRBF', 'T813', 'CM03', 'TRMA', 'T783', 'T091', 'T072', 'TOS2', 'DV36', 'DSF2', 'CM08', 'DOG1', 'CEM3', 'PACS', 'T097', 'VDR2', 'BRA2', 'DVFC', 'TS3D', 'CODL', 'HAR2', 'T506', 'HGAR', 'TRCN', 'T773', 'PCUR', 'PPRE', 'T507', 'T081', 'PARA', 'MAAL', 'PCAB', 'DOG2', 'SFUF', 'OSUA', 'OSUA', 'EPH7', 'POBM', 'HWL2', 'FCPF', 'HNRL', 'DVAF', 'CPFP', 'VSMA', 'CM09', 'COMR', 'VDR5', 'TH3D', 'STG2', 'CM13', 'CNAR', 'VDR3', 'SCEF', 'CM06', 'T632', 'TRAA', 'CM13', "UUID", 'VIM2', 'TRSC', "OFFP", 'TRAY', 'COMF', 'SCR4', 'TRAT', 'TLT3', 'AGSF', 'EPH8', 'TER1', 'ECNF', 'DVE3', 'CM19', 'PSMF', 'TPCS', 'TRMF', 'CNVS', 'UPID', 'SCR6', 'COME', 'TRAQ', 'CM05', 'EAS1', 'FELO', 'CEM2', 'TS2D', 'DALE', 'CDMV', 'CM14', 'VAUA', 'COMM', 'AAPC', 'DVBF', 'TRAJ', 'DVMF', 'DV37', 'ASL1','BORK', 'T767', 'CNRR', 'PMDH', 'T043', 'LRAL', 'PUSF', 'SADV', 'TILU', 'T592', 'T513', 'FWPO', 'VPRA', 'FEED', 'T574', 'DOOM', 'CLCI', 'CODT', 'CRAB', 'STA2', 'NCOS', 'T731', 'BOCK', 'T031', 'PLUG', 'HLAG', 'CONT', 'T594', 'TREZ', 'T515', 'INSM', 'T802', 'SESS', 'HAMV', 'T505', 'TS4T', 'WOSO', 'T753', 'SIGN', 'T588', 'BLIC', 'T040', 'FIWO', 'VIM3', 'HUFV', 'TMOV', 'SETO', 'TMVV', 'LIFE', 'HWOL', 'T037', 'T622', 'T523', "PRFC", 'SHOW', 'VAUC', 'MAND', 'PCON', 'NBTR', 'UAUX', 'T799', 'TID1', 'T827', 'PDPM', 'CONS', 'SCFA', 'T116', 'T178', 'TRFM', 'TID2', 'FORT', 'T8LR', 'PAUL', 'DUIT', 'T309', 'TOWS', 'TZ67', 'APAA', 'BWNP', 'OFFM', 'UCR1', 'WAUB', 'TSTD', 'ASPC', 'APRE', 'SWOL', 'T082', 'MSTR', 'VSEX', 'MSDE', 'VAPR', 'TRWL', 'VLAT', 'OVES', 'TLEF', 'EPH5', 'AGSR', 'PLFV', 'STAA', 'T591', 'ROB1', 'TECH', 'PERT', 'PAGR', 'MCSD', 'EPHM', 'T590', 'EPHK'],
-        'Description':  ['POSSESS FORGED INSTRUMENT 3RD', 'NEGOTIATING WORTHLESS INST', 'USE/POSSESS DRUG PARAPHERNALIA', 'POSS. CONTR. SUBS', 'FRAUD USE CREDIT/DEBIT CARD', 'NO DRIVERS LICENSE', 'PORN POSS MATERIAL MINORS', 'POSS CONTR SUBS INTENT DISTRIB', 'BREAK/ENTER VEHICLE', 'HARASSMENT', 'THEFT OF PROPERTY 3RD DEGREE', 'OVERWEIGHT TRUCK', 'FAIL DISPLAY INSURANCE', 'SEX ABUSE-CHILD LESS 12 YOA', 'TRAFFICKING-METHAMPHETAMINE', 'FRAUD USE CREDIT/DEBIT CARD', 'THEFT/DECEPTION 3RD', 'UNAUTHORIZED USE VEHICLE', 'FAIL STOP SIGN', 'FORGERY 3RD', 'HARASSING COMMUNICATIONS', 'THEFT OF PROPERTY 3RD DEGREE', 'POSS CONTROLLED SUBST BY FRAUD', 'BOND FORF-FELONY', 'CHEM END CHILD-EXP/CTN CTR SUB', 'UNLAW DISTRIB/FURN CONT SUBST', 'PROMOTING PROSTITUTION 2ND', 'UNLAW MANF CTN SUBS 1ST DEGREE', 'AGGRAVATED CHILD ABUSE', 'CHEM END CHILD-DEATH', 'LANE CHANGE W/O PROPER SIGNAL', 'FACILITATE TRAVEL F/ CHILD SEX', 'UNLAW MANF CTN SUBS 2ND DEGREE', 'PROMOTING PROSTITUTION 3RD', 'UNAUTHORIZED USE MOTOR VEHICLE', 'DUI-CONTROLLED SUBSTANCE', 'BURGLARY 3RD (UNOCCUPIED BLDG)', 'FELONY MURDER', 'MURDER-RECKLESS', 'ILL POSSESS CREDIT/DEBIT CARD', 'POSS/SELL PRECURSOR CHEMICALS', 'SEXUAL TORTURE/ABUSE', 'EXPIRED LICENSE', 'MURDER CAPITAL-ROBBERY', 'PARAPHERNALIA - SELL/DELIVER', 'POSSESS MARIHUANA 1ST DEGREE', 'MANSLAUGHTER-RECKLESS', 'USE/POSSESS DRUG PARAPHERNALIA', 'NO/IMP TAG LIGHT', 'TRAFFICKING-HEROIN', 'BOND FORF-MISD', 'SALVIA MISDEMEANOR POSSESSION', 'TRAFFICKING-SYNTHETIC DRUGS', 'DISCHARGE GUN OCC BLDG/VEHICLE', 'MISCELLANEOUS FILING', 'BURGLARY 3RD - DWELLING', 'CHEMICAL ENDANGER MINOR', 'MURDER CAPITAL-BURGLARY', 'ILL POSSESS CREDIT/DEBIT CARD', 'UNDER INFLUENCE CONT. SUBSTANC', 'DUI: ANY SUB WHICH IMPAIRS', 'MURDER CAPITAL-UNDER 14 YEARS', 'DUI - FELONY', 'SPEED/ 70+ MPH OR 65+ MPH', 'DUI - MISD', 'DUI: UNDER INFLU ALCOHOL', 'FELONY DV 3RD HARRASSMENT', 'TRAFFICKING-OPIUM', 'MURDER CAPITAL-TWO OR MORE PER', 'MURDER CAPITAL-VEH FR OUTSIDE', 'MURDER CAPITAL-KIDNAP', 'TRAFFICKING-MORPHINE', 'INOPERABLE BRAKE LIGHTS', 'AGGRAVATED CHILD ABUSE < SIX', 'TRAFFICKING-COCAINE', 'TRAFFICKING FENTANYL', 'GIVING FALSE NAME TO OFF', 'REC STOLEN PROP 3RD', 'NO DRIVERS LICENSE', 'THEFT OF SERVICES 3RD', 'TRAFFICKING STOLEN IDENTITIES', 'DRIVING WRONG SIDE HWY', 'POSSESS MARIHUANA 1ST DEGREE', 'NO TAG REGIS IN VEHICLE', 'BOND HEARING', 'CASE APPEALED ON', 'MURDER - INTENTIONAL', 'UNAUTHORIZED USE VEHICLE', 'FAILURE TO DIM LIGHTS', 'FAIL YIELD ROW', 'MANSLAUGHTER-INTENT, PASSION', 'MURDER CAPITAL-FIRED FROM VEHI', 'NO USER PERMIT', 'FRAUD BY AUTHORIZED PERSONS', 'DRUG PARAPHERNALIA TO MINOR', 'MURDER CAPITAL-DWELL FR OUTSID', 'ENDG WELFARE CHILD-OCCUPATION', 'MOVING TRAFFIC VIO', 'HOMICIDE BY VEHICLE', 'ALCOHOL-SALE/PERMIT UNDER AGE', 'SALVIA FELONY POSSESSION', 'FELONY DV CRIM MISCHIEF 2D/3D', 'NO TAG REGIS IN VEHICLE', 'COMBINED INFLUENCE', 'MURDER CAPITAL-FOR HIRE', 'TR-FORT.', 'MOVE OVER LAW', 'MURDER CAPITAL-RAPE/SODOMY', 'TRAFFICKING-MARIJUANA', 'IMPEDING FLOW TRAFFIC', 'DUI', 'UNDER INFLU - ANY SUBSTANCE', 'THEFT OF SERVICES 2ND', 'FELONY DV CRIM MISCHIEF 2ND', 'DISCHARGE GUN UNOCC BLDG/VEH', 'MURDER CAPITAL-SEXUAL ABUSE', 'DOG/CAT CRUELTY 1ST DEGREE', 'CHEMICAL ENDANGER MINOR/DEATH', 'PROHIBITED ACTS-MAIN BLD/DWL', 'OTHER NON MOVING VIO', 'DEL/SALE DRUG PARAPHERNALIA', 'BURGLARY 3RD - OCCUPIED BLDG', 'FELONY DV CRIM MISCHIEF 2D/3D', 'THEFT OF SERVICES 3RD DEGREE', 'CONTRIBUTING TO THE DELINQUENC', 'HARASSMENT - THREAT', 'FAIL TO YIELD EMER VEHICLE', 'FAILURE TO COMPLY - GARBAGE', 'TR-CONTEMPT', 'IMP TAIL LIGHTS-TRAILER', 'FAIL CPLY REPORTS-PRECUR CHEMS', 'POSS OF PRE-CURSOR CHEMICALS', 'FAIL TO YIELD RIGHT OF WAY', 'NO HDLGTS WHEN REQUIRED', 'FAILURE COMPLY PARK CONDITIONS', 'ALCOHOL- MINOR/POSS/CONSUME', 'POSS/CONT ALCOHOL-STATE PARK', 'DOG/CAT CRUELTY 2ND DEGREE', 'SETTING FIRE-UNCL FOREST/WOOD', 'OMMISSION/MISREP SALE SECURITI', 'OMMISSION/MISREP SALE SECURITI', 'ILL PURCHASE EPHEDRINE-INDIVID', 'PORN INTENT TO DISSEMINATE', 'HUNT-W/O NONRESIDENT LICENSE', 'FIREARM-PERSONS FORBIDDEN/POSS', 'HUNT-LEND RESIDENT LICENSE', 'FELONY DV 3RD ASSAULT 3RD', 'PISTOL-CERTAIN PERSONS FORBIDD', 'UNLAWFUL DISTRIB MARIHUANA', 'MURDER CAPITAL-ARSON', 'COMM NOTIF ACT-SCHOOL/CHILD CR', 'MANUFACTURE PARAPHERN/FIREARM', 'THEFT BY DECEPTION 3RD', 'AGGRAVATED STALKING 2ND DEGREE', 'MURDER CAPITAL-20YR PRIOR CON', 'COMM NOTIFICATION-DECLARATION', 'DEL/SALE DRUG PARAPHERNALIA', 'SCHOOL EMPLOYEE SEXUAL CONTACT', 'MURDER CAPITAL-LIFE SENTENCE', 'DUI FELONY', 'TRAFF/CONTR SUBSTANCE', 'MURDER CAPITAL-20YR PRIOR CON', "UNAUTH USE ID #", 'IMITATION DRUG DIST TO MONOR', 'SCRAP METAL/FALSIFY STATEMENT',"USE POSITION-PERSONAL GAIN", 'TRAFFICKING-HYDROMORPHONE','COMM NOTIF ACT-VICTIM/VIC FAMI', 'ILLEGAL DISPOSAL/ SCRAP TIRES', 'TRAFFICKING-3,4 METHYL AMPHETA','THEFT OF LOST PROPERTY 3RD', 'AGGRAVATED SURVEILLANCE FELONY', 'ILL PURCHASE EPHEDRINE-INDIVID', 'TERRORISM', 'ERROR CORAM NOBIS - FELONY', 'FELONY DV 3RD ONE PRIOR FELONY','CAPITAL MURDER - PROTECT ORDER', 'OBSCENE MATERIAL- DIST/POSS', 'THEFT 2ND CONTROLLED SUBSTANCE', 'TRAFF CANNABIS-W/POSS FIREARM', 'COMM NOTIF-10 DAY VERIF SUBMIT', 'POSS CONTR SUBS INTENT DISTRIB', 'SCRAP METAL/FALSE INFO', 'COM NOTIF ACT-NONRESIDENT', 'TRAFFICKING-LSD', 'MURDER CAPITAL-LAW OFF/GUARD', 'EXPLOITATION OF ASSETS 1ST', 'FELONY CASE', 'CHEMICAL ENDANGER INJURY', 'THEFT OF SERVICES 2ND DEGREE', 'DISARMING LAW ENFORCEMENT', 'UNAUTH USE MTR VEH - BY FORCE', 'MURDER CAPITAL-WITNESS', 'UNEMPLOYMENT COMP-CLASS B FEL', 'COMM NOTIF ACT-MINOR RESIDENCE', 'AIDS/ABETS PERSON COMMIT OFFEN', 'FELONY DV 3RD HARRASS COMMUNIC', 'TRAFFICKING-AMPHETAMINE', 'FELONY DV 3RD MENACING', 'FELONY DV CRIM MISCHIEF 3RD', 'ASSAULT 1ST DEGREE (DUI/BUI)','BOAT-RECKLESS OPER VESSEL', 'IMPROPER LOAD-UNSECURED', 'COMM NOTIF RESIDENCE REQ', 'HUNT/FEED AREA', 'OVERWIDE TRUCK', 'PERMITTING LIVESTOCK TO RUN AT', 'POSSESSING UNDERSIZE FISH', 'BOAT-VESS W/O SAFETY DEV/LGHT', 'IMPROPER LOAD', 'ALCOHOL-CONSUM/COMM VEH', 'DRIVE THRU BARRICADE', 'FISHING W/O PERMISSION OWNER', 'VIO. PARENTAL RESPONSIBILTY AC', 'HUNT-AREA FEEDING TAKEN PLACE', 'SPILLING LOAD ON ROAD', 'DISSEMINATE OBSCENE MATERIAL', 'CHANGING LIC PLATE-CONCEAL ID', 'CONT TO TRUANCY', 'POSS UNDERSIZED BLUE CRABS', 'STALKING  2ND DEGREE', 'NO CUT OFF SWITCH LANYARD', 'HITCHHIKING', 'BOAT-CARELESS OPER VESSEL', 'ONEWAY STREET', 'ILLEGAL ARMS - TURKEY HUNTING', 'HUNT W/O LICENSE (ALL GAME)', 'CONTEMPT OF COURT', 'BOATING UNDER THE INFLUENCE', 'FAIL/YIELD EMERG VEHICLE', 'OVERSIZED LOAD LIMIT', 'OPER VEH W/O INSURANCE', 'CAUSE/ALLOW LITTER-ROADWAY', 'SOLICIT SEX ACT WITH STUDENT', 'HUNT-BY AID MOTORIZED VESSEL', 'BLUE LIGHT LAW', 'THEFT OF SERVICES 4TH DEGREE', 'NO/ATTACHED SHUT-OFF SWITCH', 'IMP LIGHT COLORING', 'BOAT-VIO. RESTRICTIVE SIGN', 'STOPPING ON HIGHWAY', 'BOATING W/O LICENSE/CERTIF', 'OVERHEIGHT TRUCK', 'FISH-WO PERMISSION', 'IMITATION DRUG POSSESSION', 'HUNT-FROM VEHICLE', 'MOVE OVER/EMERGENCY VEHICLE', 'DIST OBSCENE MATERIAL/SCHOOL', 'MOVE OVER LAW VIOLATIONS', 'BOAT-VESSEL W/O LIFE PRE.', 'HUNT-W/O LICENSE', 'MOTORCYCLE NO-HELMET', 'NO TAG - UTILITY TRAILER', 'DUI 0.08 BAC OR ABOVE', 'PT-RL F/CN', 'SHOW CAUSE DKT/HEARING', 'UNEMPLOYMENT COMP-VIOLATION', 'WIRT OF MANDAMUS', 'PISTOL-CERTAIN PERSONS FORBIDD', 'NO ANT BUCK/TURKEY HAR RECORD', 'UNAUTHORIZED USE VEHICLE', 'PEDESTRIAN-SOL EMPLY/BUSN/CONT', 'IGNITION INTERLOCK MISDEMEANOR', 'FAIL UPDATE DL NAME/ADDRESS', 'DISTRIB HARMFUL MATERIAL-MINOR', 'CONSERVATION', 'SCIRE FACI', 'CMV W/O PROPER DOCUMENTS', 'DUI .08 OR MORE', 'TRAFFIC/MISC', 'IGNITION INTERLOCK VIOLATIONS', 'FORFEITURE-TRAFFIC', 'CAUSE/ALLOW LITTER ON ROADWAY', 'ALCOHOL-POSS UNTAXED LIQ', 'DUI TRIAL DOCKET', 'FAIL TO STOP AS REQUIRED', 'BOAT-SKING W/O MIRROR\\OBSERVER', 'CZ SLOWING/STOP W/O PROPER SIG', 'ALCOHOL - ON PUBLIC ACCESS AREA', 'BURN W/OUT NECESSARY PRECAUTIO', 'USE OFF POSITION- PERSONAL GAIN', 'UNIFIED CARRIER REGISTRATION', 'WHLSE SALE ALCOHOL UNA BUYER', 'KNOWINGLY TRANSMIT EXPOSE STD', 'ASPC-OTHER', 'ALCOHOL-ON OFF PREMISES LI', 'ALCOHOL-SELL W/O LICENSE', 'FAILURE TO DIM HEADLIGHTS', 'NO MASTER PLUMBER CERTIFICATE', 'VIOLATION COMMUNITY NOT ACT', 'MISDEMEANOR', 'VIOL POSTED RULE-WILDLIFE AREA', 'WASH SHRIMP TRAWL- CLOSED AREA', 'VIOLATION', 'OPER VESSEL W/O EMERG SHUTOFF', 'INTERSTATE/LEFT LANE 1.5 MILES', 'SINGLE SALE-EPHEDRINE PRODUCT', 'AGGRAVATED SURVEILLANCE MISD', 'HUNT-POSS LOAD GUN IN VEH', 'STALKING AGGRAVATED 1ST DEGREE', 'HANDICAPPED PARKING VIOLATION', 'ROBBERY 1ST', 'TECH VIOL PROBATION', 'UNLAW SALE TOBACCO W/O PERMIT', 'ALCOHOL-POSS MORE THAN 5 GAL.', 'WRONG1MANF CTN SUBS 1ST DEGREE', 'DRUG OFFENDER EPHEDRINE MISD', 'FAIL TO STOP EXIT PARKING LOT', 'SALE EPHEDRINE 2ND CONVICTION'],
-        'Cite': ['13A-009-006.1', '13A-009-013.1', '13A-012-260(C)', '13A-012-212(A)', '13A-012-212(A)', '032-006-001(A)', '13A-012-192(B)', '013-012-192(B)', '13A-008-011(B)', '13A-011-008(A)', '13A-008-004.1', '032-009-020(4)', '032-07A-016(B)', '13A-006-069.1', '13A-012-231(11)', '13A-009-014(B)', '13A-008-004.1', '13A-008-011(A)', '032-05A-112(B)', '13A-009-003.1', '13A-011-008(B)', '13A-008-4.1', '13A-012-212(A)', '- -BOND FORT', '026-015-003.2(A)', '13A-012-211', '13A-012-112', '13A-012-218', '026-015-003.1(A)', '026-015-003.2(A)', '032-05A-133', '13A-006-125', '13A-012-217', '13A-012-113', '032-008-081', '032-05A-191(A)', '13A-007-007(A)', '13A-006-002(A)', '13A-006-002(A)', '13A-009-014(A)', '020-002-190(B)', '13A-006-065.1', '032-006-001(B)', '13A-005-040(A)', '13A-012-260(D)', '13A-012-213(A)', '13A-006-003(A)', '13A-012-260(C)', '032-005-240(C)', '13A-012-231(3)', '- -BOND FORT', '13A-012-214.1', '13A-012-231(12)', '13A-011-061(B)', '', '13A-007-007(A)', '026-015-3.2(A)', '13A-005-040(A)', '13A-009-014(A)', '032-05A-191(A)', '032-05A-191(A)', '13A-005-040(A)', '032-05A-191(A)', '032-05A-171(4)', '032-05A-191(A)', '032-05A-191(A)', '13A-006-132(D)', '13A-012-231(3)', '13A-005-040(A)', '13A-005-040(A)', '13A-005-040(A)', '13A-012-231(3)', '032-005-241(B)', '025-015-03.1(B)', '13A-012-231(2)', '13A-012-231(13)', '13A-009-018.1', '13A-008-18.1', '032-006-018(A)', '13A-008-010.3', '13A-008-193(B)', '032-05A-080(A)', '13A-012-213(A)', '040-012-260(B)', '', '', '13A-006-002(A)', '13A-008-011(A)', '032-005-242(C)', '032-05A-112(C)', '13A-006-003(A)', '13A-005-040(A)', '033-015-007(C)', '13A-009-014.1', '13A-012-260(E)', '13A-005-040(A)', '13A-013-006(A)', '', '032-05A-190.1', '028-03A-025(A)', '13A-012-214.1', '13A-006-132(D)', '040-012-260(B)', '032-05A-191(A)', '13A-005-040(A)', '', '032-05A-058.2', '13A-005-040(A)', '13A-012-231(1)', '032-05A-080(B)', '032-05A-191(A)', '032-05A-191(A)', '13A-008-010.2', '13A-006-132(D)', '13A-011-061(C)', '13A-005-040(A)', '13A-011-241(A)', '026-015-3.2(A)', '020-002-071(A)', '', '13A-012-260(E)', '13A-007-007(A)', '13A-006-132(D)', '13A-008-010.25', '012-015-111(A)', '13A-011-008(A)', '032-05A-115(A)', '022-027-003(A)', '', '032-005-240(C)', '020-002-190(A)', '020-002-181(D)', '032-05A-082(2)', '032-005-240(A)', '220-005-013(2)', '028-03A-025(A)', '220-005-016(4)', '13A-011-241(B)', '009-013-011(B)', '008-006-017(A)', '008-006-017(A)', '020-002-190(C)', '13A-012-192(A)', '009-011-051(C)', '13A-011-072(A)', '009-011-051(B)', '13A-006-132(D)', '13A-011-072(A)', '13A-012-211(A)', '13A-005-040(A)', '015-020-026(A)', '13A-012-260(D)', '13A-008-04.1', '13A-006-091.1', '13A-005-040(A)', '015-020-022(A)', '13A-012-260(E)', '13A-006-082(A)', '13A-005-040(A)', '032-05A-191(A)', '13A-012-231(12)', '13A-005-040(A)', "032-008-086(D)", '020-008-086(D)', '032-008-087(S)(2)', '036-025-005(A)','13A-012-231(5)', '015-020-026(B)', '022-40A-19(A)(4)', '13A-012-231(6)', '13A-008-008.1', '13A-011-32.1', '020-002-190(C)(4)', '13A-010-152(A)', '', '13A-006-132(E)', '13A-005-040(19)', '13A-012-200.2(1)', '13A-008-004(D)', '13A-012-231(13)', '015-020-024(B)', '13A-012-211(C)', '13A-008-031(D)', '015-020-25.1', '13A-012-231(9)', '13A-005-040(A)(5)', '038-009-007(G)', '', '026-015-3.2(A)(2)', '13A-008-010.2', '13A-010-005.1', '13A-008-011(A)(4)', '13A-005-040(A)(14)', '025-004-145(A)(1)A', '015-020-026(C)', '13A-002-023(2)', '13A-006-132(D)', '13A-012-231(10)', '13A-006-132(D)', '13A-006-132(D)', '13A-006-020(A)(5)','033-005-070(A)', '032-005-076(B)', '015-020-021(C)', '220-002-011(8', '032-009-020(1', '003-005-002(D)', '220-003-030(2', '033-005-022(A)', '032-005-076(B)', '032-006-049.1', '023-005-002(B)', '220-002-044(6', '016-028-012(A)', '220-002-011(8', '032-005-076(A)', '13A-012-200.3', '032-008-086(E)', '012-015-013(A)', '220-003-031(1', '13A-006-090.1', '033-005-051(C)', '032-05A-216(A)', '033-005-070(B)', '032-05A-087(B)', '220-002-002(3', '009-011-051(A)', '012-011-030', '032-05A-191.3', '032-05A-115(A)', '032-009-029(A)', '032-07A-016(1', '032-005-076(C)', '13A-006-082(B)', '220-002-011(1', '032-05A-115(C)', '13A-008-010.3', '033-005-072(A)', '032-005-242(G)', '220-006-019(4', '032-05A-136(A)', '033-005-052(A)', '032-009-020(2', '009-011-091(A)', '020-002-143(C)', '220-002-011(1', '032-05A-058.2', '13A-006-082.1', '032-05A-058.2', '220-006-011(1', '009-011-051(A)', '032-05A-245(A)', '040-012-252(A)', '032-05A-191(A)1','','','025-004-145(A)(1)C','','13A-011-072(B)', '220-002-146(2)', '13A-008-011(A)2', '032-05A-216(B)', '032-05A-191.4(J)', '760-X-1-07(7)', '13A-012-200.5(1)', '', '', '', '032-05A-191(A)1', '', '032-05A-191.4(L)','- -BOND FORT', '032-005-076(C)(1)', '028-04-020', '','','033-005-026(A)', '032-05A-133(C)', '220-002-037(13)', '009-013-011(B)(2)', '036-025-005(A)', 'PSC-3.2-016', '028-03A-025(A)(2)', '022-11A-021(C)', '', '028-03A-025(A)(4)', '028-03A-025(A)(14)', '032-005-242(C)(2)', '034-037-001(8)', '', '', '220-002-055(1)(BB)', '220-003-001(5)', '', '033-005-072(B)', '032-05A-080(D)(1)', '020-002-190(C)(2)', '13A-011-32.1', '220-002-055(1)(K)', '13A-006-091', '032-006-233.1', '13A-008-041', '015-022-054.1', '028-011-008', '028-004-115', '13A-012-218', '020-002-190.2(K)', '032-05A-153', '020-002-190.2(K)'] 
-        }
-    )
-    for r in fillers.rows():
-        charges = charges.with_columns(
-            [
-                pl.when(pl.col("Code")==r[0])
-                .then(r[1])
-                .otherwise(pl.col("Description"))
-                .alias("Description"),
-                pl.when(pl.col("Code")==r[0])
-                .then(r[2])
-                .otherwise(pl.col("Cite"))
-                .alias("Cite")
-            ]
-        )
-    charges = charges.with_columns(
-        [
-            pl.when((pl.col("Code")=="VIM1") & (pl.col("Description").eq("")))
-            .then("IMITATION DRUG MANUF/DIST")
-            .otherwise(pl.col("Description"))
-            .alias("Description"),
-            pl.when((pl.col("Code")=="VIM1") & (pl.col("Cite").eq("")))
-            .then("020-002-143(A)")
-            .otherwise(pl.col("Cite"))
-            .alias("Cite")
-        ]
-    )
-    charges = charges.with_columns(
-        [
-            pl.col("Charges").str.extract(r'\s(A|S|C|P)\s').alias("ID"),
-            pl.concat_str(
+            vrr = vrr.join(self._pairs, on="Name", how="outer")
+            vrr = vrr.groupby("AIS / Unique ID").all()
+            vrr = vrr.select(
                 [
-                    pl.col("CaseNumber"),
-                    pl.lit(" - "),
-                    pl.col("Num"),
-                    pl.lit(" "),
-                    pl.col("Cite"),
-                    pl.lit(" "),
-                    pl.col("Description"),
-                    pl.lit(" "),
-                    pl.col("TypeDescription"),
-                    pl.lit(" "),
-                    pl.col("CourtAction"),
-                    pl.lit(" "),
-                    pl.col("CourtActionDate"),
+                    pl.col("AIS / Unique ID"),
+                    pl.col("ChargesSummary").list.join(", ")
+                    .str.replace_all(r"null,?", "")
+                    .str.strip()
+                    .str.replace(r",$", "")
+                    .str.replace_all(r"\s+", " ")
+                    .alias("DisqualifyingConvictions")
                 ]
             )
-            .str.strip()
-            .str.replace(r",$", "")
-            .str.replace_all(r"\s+", " ")
-            .str.replace(r"\.\s\.\s", ".")
-            .str.replace(r'\s[ASC]\s'," ")
-            .alias("ChargesSummary")
-        ]
-    )
-    charges = charges.with_columns(
-        [
-            pl.when(pl.col("Charges").str.contains("ATTEMPT").is_not() & pl.col("ID").eq("A"))
-            .then("")
-            .otherwise(pl.col("ID"))
-            .alias("ID"),
-            pl.col("Description")
-            .str.replace(r'^\.\d?\s','')
-            .str.replace(r'\s[ASC]\s', " ")
-            .str.replace(r'^[ASC]\s', "")
-        ]
-    )
-    charges = charges.with_columns(
-        [
-            pl.when(pl.col("Charges").str.contains("WILLFUL FAILURE TO RETURN TO P"))
-            .then("")
-            .otherwise(pl.col("ID"))
-            .alias("ID")
-        ])
-    charges = charges.fill_null('')
-    charges = charges.with_columns(
-        [
-            pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
-            pl.col("Category").cast(pl.Categorical),
-            pl.col("TypeDescription").cast(pl.Categorical),
-            pl.col("CourtAction").cast(pl.Categorical),
-        ]
-    )
-    charges = charges.select(
-        "Name",
-        "CaseNumber",
-        "Num",
-        "Code",
-        "Cite",
-        "ID",
-        "Description",
-        "TypeDescription",
-        "Category",
-        "CourtAction",
-        "CourtActionDate",
-        "TotalBalance",
-        "PaymentToRestore",
-        "Conviction",
-        "Felony",
-        "CERVDisqCharge",
-        "CERVDisqConviction",
-        "PardonDisqCharge",
-        "PardonDisqConviction",
-        "PermanentDisqCharge",
-        "PermanentDisqConviction",
-        "Filing",
-        "Disposition",
-        "ChargesSummary"
-    )
-    dlog(charges.columns, charges.shape, cf=debug)
-    return charges
-
-
-def _split_fees(df, debug=False):
-    df = df.with_columns(
-        [
-            pl.col("CaseNumber"),
-            pl.col("Fees")
-            .str.replace(r"(?:\$\d{1,2})( )", "\2")
-            .str.split(" ")
-            .alias("SPACE_SEP"),
-            pl.col("Fees")
-            .str.strip()
-            .str.replace(" ", "")
-            .str.extract_all(r"\s\$\d+\.\d{2}")
-            .alias("FEE_SEP"),
-        ]
-    )
-    dlog(df.columns, df.shape, cf=debug)
-    df = df.with_columns(
-        [
-            pl.col("CaseNumber"),
-            pl.col("SPACE_SEP").arr.get(0).alias("FeeStatus1"),
-            pl.col("FEE_SEP").arr.get(0).str.replace(r"\$", "").alias("AmtDue"),  # good
-            pl.col("FEE_SEP")
-            .arr.get(1)
-            .str.replace(r"\$", "")
-            .alias("AmtPaid"),  # good
-            pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", "").alias("Balance1"),
-            pl.col("SPACE_SEP").arr.get(5).alias("FeeCode"),
-            pl.col("Fees").str.extract(r"(\w00\d)").alias("Payor"),
-            pl.col("Fees").str.extract(r"\s(\d\d\d)\s").alias("Payee"),
-        ]
-    )
-    out = df.with_columns(
-        [
-            pl.col("CaseNumber"),
-            pl.when(pl.col("FeeStatus1") != "ACTIVE")
-            .then(True)
-            .otherwise(False)
-            .alias("TOT"),
-            pl.when(pl.col("Balance1").is_in(["L", pl.Null]))
-            .then("$0.00")
-            .otherwise(pl.col("Balance1").str.replace_all(r"[A-Z]|\$", ""))
-            .alias("AmtHold2"),
-        ]
-    )
-    out = out.with_columns(
-        pl.col("Fees").str.extract(r'\s(Y|N)\s').alias("AdminFee"),
-        pl.when(pl.col("TOT") == True)
-        .then(pl.col("FEE_SEP").arr.get(-1).str.replace(r"\$", ""))
-        .otherwise(pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", ""))
-        .alias("AmtHold"),
-        pl.when(pl.col("TOT") == False)
-        .then(pl.col("SPACE_SEP").arr.get(0))
-        .otherwise(pl.lit(""))
-        .alias("FeeStatus"),
-        pl.when(pl.col("TOT") == True)
-        .then(pl.lit("Total:"))
-        .otherwise(pl.lit(""))
-        .alias("Total"),
-    )
-    dlog(out.columns, out.shape, cf=debug)
-    out = out.with_columns(
-        [
-            pl.col("AmtDue").str.strip().cast(pl.Float64, strict=False),
-            pl.col("AmtPaid").str.strip().cast(pl.Float64, strict=False),
-            pl.col("AmtHold").str.strip().cast(pl.Float64, strict=False),
-        ]
-    )
-    out = out.with_columns([pl.col("AmtDue").sub(pl.col("AmtPaid")).alias("Balance")])
-    out = out.select(
-        "CaseNumber",
-        "Total",
-        "FeeStatus",
-        "AdminFee",
-        "FeeCode",
-        "Payor",
-        "Payee",
-        "AmtDue",
-        "AmtPaid",
-        "Balance",
-        "AmtHold",
-    )
-    dlog(out.columns, out.shape, cf=debug)
-    out = out.fill_null("")
-    out = out.drop_nulls("AmtDue")
-    return out
-
-
-def _explode_images(df, debug=False):
-    images = df.select(
-        [
-            pl.concat_str(
+            cases = cases.join(self._pairs, on="Name", how="outer")
+            cases = cases.groupby("AIS / Unique ID").all()
+            cases = cases.join(vrr, on="AIS / Unique ID", how="outer")
+            cases = cases.join(conv, on="AIS / Unique ID", how="outer")
+            cases = cases.join(fch, on="AIS / Unique ID", how="outer")
+            cases = cases.with_columns(
                 [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                    pl.col("CaseNumber").list.join(", ")            
+                    .str.replace_all(r"null,?", "")
+                    .str.strip()
+                    .str.replace(r",$", "")
+                    .str.replace_all(r"\s+", " ")
+                    .alias("Cases")
                 ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract(
-                r"(Images\s+?Pages)([^\\n]*)(END OF THE REPORT)", group_index=2
             )
-            .str.strip()
-            .alias("ImagesChunk"),
-        ]
-    )
-    images = images.select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("ImagesChunk")
-            .str.replace_all("© Alacourt.com", "", literal=True)
-            .str.split("\n")
-            .alias("Images"),
-        ]
-    )
-    images = images.explode("Images")
-    images = images.filter(pl.col("Images").str.contains(r"[A-Za-z0-9]"))
-    images = images.select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("Images")
-            .str.replace_all(r"[A-Z][a-z]+", " ")
-            .str.replace_all(r"[\s\:]+", " ")
-            .str.strip(),
-        ]
-    )
-    images = images.select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=1).str.to_date('%-m/%-d/%Y', strict=False).alias("Date"),
-            pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=2).str.to_time('%-H %M %S %p', strict=False).alias("Time"),
-            pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').cast(pl.Int64, strict=False).alias("Doc#"),
-            pl.col("Images").str.extract(r'^\d\s(.+?)\s\d').alias("Title"),
-            pl.col("Images").str.extract(r'^\d\s.+?\s\d\s(.+?)\s\d\d?/\d\d?/\d\d\d\d').alias("Description"),
-            pl.col("Images").str.extract(r'^(\d)\s').cast(pl.Int64, strict=False).alias("Pages")
-        ])
-    images = images.fill_null('')
-    return images
-
-
-def _explode_case_action_summary(df, debug=False):
-    cas = df.select(
-        [
-            pl.concat_str(
+            cases = cases.with_columns(
                 [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                    pl.when(pl.col("CERVConvictionCount").eq(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentDisqConvictionCount").eq(0) & pl.col("Cases").str.lengths().gt(0))
+                    .then(True).otherwise(False)
+                    .alias("EligibleToVote"),
+                    pl.when(pl.col("CERVConvictionCount").gt(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentDisqConvictionCount").eq(0))
+                    .then(True).otherwise(False)
+                    .alias("NeedsCERV"),
+                    pl.when(pl.col("PardonToVoteConvictionCount") > 0 & pl.col("PermanentDisqConvictionCount").eq(0))
+                    .then(True).otherwise(False)
+                    .alias("NeedsPardon"),
+                    pl.when(pl.col("PermanentDisqConvictionCount").gt(0))
+                    .then(True).otherwise(False)
+                    .alias("PermanentlyDisqualified")
                 ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract(
-                r"(Case Action Summary)([^\\]*)(Images\s+?Pages)", group_index=2
             )
-            .str.replace_all(r"\s+", " ")
-            .alias("CASChunk"),
-        ]
-    )
-    cas = cas.select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("CASChunk")
-            .str.replace(r"© Alacourt\.com|Date: Description Doc# Title|Operator", "")
-            .str.replace(r"Date\: Time Code CommentsCase Action Summary", "")
-            .str.strip()
-            .str.rstrip()
-            .str.split("\n")
-            .alias("CaseActionSummary"),
-        ]
-    )
-    cas = cas.explode("CaseActionSummary")
-    cas = cas.filter(pl.col("CaseActionSummary").str.contains(r"[A-Za-z0-9]"))
-    return cas
-
-
-def _explode_attorneys(df, debug=False):
-    att = df.select(
-        [
-            pl.concat_str(
+            cases = cases.with_columns(
                 [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                    pl.when(pl.col("Cases").str.lengths().eq(0))
+                    .then(None).otherwise(pl.col("EligibleToVote"))
+                    .alias("EligibleToVote"),
+                    pl.when(pl.col("Cases").str.lengths().eq(0))
+                    .then(None).otherwise(pl.col("NeedsCERV"))
+                    .alias("NeedsCERV"),
+                    pl.when(pl.col("Cases").str.lengths().eq(0))
+                    .then(None).otherwise(pl.col("NeedsPardon"))
+                    .alias("NeedsPardon"),
+                    pl.when(pl.col("Cases").str.lengths().eq(0))
+                    .then(None).otherwise(pl.col("PermanentlyDisqualified"))
+                    .alias("PermanentlyDisqualified"),
                 ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesTextNoNewLine")
-            .str.extract(
-                r"(Type of Counsel Name Phone Email Attorney Code)(.+)(Warrant Issuance)",
-                group_index=2,
             )
-            .str.replace(r"Warrant.+", "")
-            .str.replace_all(r"[A-Z][a-z]+", " ")
-            .str.replace_all(r"[\s\:]+", " ")
-            .str.strip()
-            .alias("Attorneys"),
-        ]
-    )
-    return att.drop_nulls()
-
-
-def _explode_witnesses(df, debug=False):
-    wit = df.select(
-        [
-            pl.concat_str(
-                [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
-                ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesTextNoNewLine")
-            .str.extract(r"Witness(.+)Case Action Summary", group_index=1)
-            .str.replace(r"\# Date Served Service Type Attorney Issued Type", "")
-            .str.replace(r"SJIS Witness List", "")
-            .str.replace("Date Issued", "")
-            .str.replace("Subpoena", "")
-            .str.replace("List", "")
-            .str.replace("Requesting Party Name Witness", "")
-            .str.replace("Date: Time Code Comments", "")
-            .str.replace(r"© Alacourt.com \d\d?/\d\d?/\d\d\d\d", "")
-            .str.replace(r'\#','')
-            .str.replace_all(r"[A-Z][a-z]+", " ")
-            .str.replace_all(r"[\s\:]+", " ")
-            .str.strip()
-            .alias("Witnesses"),
-        ]
-    )
-    return wit.drop_nulls()
-
-
-def _explode_settings(df, debug=False):
-    settings = df.select(
-        [
-            pl.concat_str(
+            cases = cases.select(
                 [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                    pl.col("AIS / Unique ID"),
+                    pl.col("Name").list.first(),
+                    pl.col("DOB").list.first(),
+                    pl.col("Race").list.first(),
+                    pl.col("Sex").list.first(),
+                    pl.col("PaymentToRestore"),
+                    pl.col("EligibleToVote"),
+                    pl.col("NeedsCERV"),
+                    pl.col("NeedsPardon"),
+                    pl.col("PermanentlyDisqualified"),
+                    pl.col("ConvictionCount"),
+                    pl.col("CERVChargesCount"),
+                    pl.col("CERVConvictionCount"),
+                    pl.col("PardonToVoteChargesCount"),
+                    pl.col("PardonToVoteConvictionCount"),
+                    pl.col("PermanentDisqChargesCount"),
+                    pl.col("PermanentDisqConvictionCount"),
+                    pl.col("DisqualifyingConvictions"),
+                    pl.col("Convictions"),
+                    pl.col("FilingCharges"),
+                    pl.col("Cases")
                 ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesTextNoNewLine")
-            .str.extract(r"(Settings)(.+)(Court Action)", group_index=2)
-            .str.replace(r"Settings", "")
-            .str.replace(r"Date\:", "")
-            .str.replace(r"Que\:", "")
-            .str.replace(r"Time\:", "")
-            .str.replace(r"Description\:", "")
-            .str.replace(
-                r"Disposition Charges   # Code Court Action Category Cite Court Action",
-                "",
             )
-            .str.replace(r"Parties Party 1 - Plaintiff", "")
-            .str.replace(r"Court Action.+", "")
-            .str.strip()
-            .alias("SET1"),
-        ]
-    )
-    settings = settings.select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("SET1")
-            .str.replace_all(r"[A-Z][a-z]+", " ")
-            .str.replace_all(r"[\s\:]+", " ")
-            .str.strip()
-            .alias("Settings"),
-        ]
-    )
-    settings = settings.drop_nulls()
-    settings = settings.select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("Settings").str.extract(r'^(\d)\s').cast(pl.Int64, strict=False).alias("#"),
-            pl.col("Settings").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
-            pl.col("Settings").str.extract(r'\s(\d\d\d)\s').alias("Que"),
-            pl.col("Settings").str.extract(r'(\d\d \d\d [A|P]M)').str.to_time(r'%H %M %p', strict=False).alias("Time"),
-            pl.col("Settings").str.extract(r'[A|P]M (.+)').str.strip().alias("Description")
-        ])
-    return settings
-
-def _explode_split_sentences(df, debug=False):
-    sent = df.select(
-        [
-            pl.concat_str(
+            cases = cases.sort("Name")
+        self._summary = cases
+        return self._summary
+
+    def pairs_template(self):
+        if not self.is_read:
+            self.read()
+        with console.status("Creating template..."):
+            names = self.archive.with_columns(
                 [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
+                    pl.col("AllPagesText")
+                    .str.extract(
+                        r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
+                        group_index=1,
+                    )
+                    .str.replace_all("Case Number:", "", literal=True)
+                    .str.replace(r"C$", "")
+                    .str.strip()
+                    .alias("Name"),
+                    pl.col("AllPagesText")
+                    .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
+                    .str.replace_all(r"[^\d/]", "")
+                    .str.strip()
+                    .str.to_date('%m/%d/%Y', strict=False)
+                    .alias("DOB"),
+                    pl.col("AllPagesTextNoNewLine")
+                    .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
+                    .str.replace(r"(SSN)", "")
+                    .str.replace(r"Alias", "")
+                    .str.replace(r"\:", "")
+                    .str.strip()
+                    .alias("Alias"),
                 ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesTextNoNewLine")
-            .str.extract_all(r"Sentence\s\d\s.+?(Linked Cases)")
-            .alias("Sentence"),
-        ]
-    )
-    sent = sent.explode("Sentence")
-    sent = sent.select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("Sentence")
-            .str.extract(r"Sentence\s(\d)\s")
-            .cast(pl.Int64, strict=False)
-            .alias("Number"),
-            pl.col("Sentence")
-            .str.extract(
-                r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}"
-            )
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("LastUpdate"),
-            pl.col("Sentence")
-            .str.extract(
-                r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})"
-            )
-            .alias("UpdatedBy"),
-            pl.col("Sentence")
-            .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
-            .str.replace(r"Sentence.*", "")
-            .str.replace(r"License.+", "")
-            .str.strip()
-            .alias("ProbationRevoke"),
-            pl.col("Sentence")
-            .str.extract(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
-            .alias("LicenseSuspPeriod"),
-            pl.col("Sentence")
-            .str.extract(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+")
-            .alias("JailCreditPeriod"),
-            pl.col("Sentence")
-            .str.extract(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
-            .alias("ProbationPeriod"),
-            pl.col("Sentence")
-            .str.extract(r"Sentence Provisions\: ([YN])")
-            .cast(pl.Categorical)
-            .alias("Provisions"),
-            pl.col("Sentence")
-            .str.extract(r"Requrements Completed\: (YES|NO)")
-            .cast(pl.Categorical)
-            .alias("RequirementsCompleted"),
-            pl.col("Sentence")
-            .str.extract(r"Sentence Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("SentenceDate"),
-            pl.col("Sentence")
-            .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("StartDate"),
-            pl.col("Sentence")
-            .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("EndDate"),
-            pl.col("Sentence")
-            .str.extract(r"Jail Fee\:(.+?)Costs")
-            .str.replace(r"[A-Z]-\$", "")
-            .str.strip()
-            .cast(pl.Float64, strict=False)
-            .alias("JailFee"),
-            pl.col("Sentence")
-            .str.extract(r"Costs\: (.+?)Fine\:")
-            .str.replace(r"Fine.+", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("Costs"),
-            pl.col("Sentence")
-            .str.extract(r"Fine\:(.+?)Crime Victims")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("Fine"),
-            pl.col("Sentence")
-            .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
-            .str.strip()
-            .alias("CrimeVictimsFee"),
-            pl.col("Sentence")
-            .str.extract(r"Municipal Court\:(.+?)Fine Suspended")  ## NONE
-            .str.replace(r"X-\$", "")
-            .str.strip()
-            .cast(pl.Float64, strict=False)
-            .alias("MunicipalCourt"),
-            pl.col("Sentence")
-            .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
-            .str.strip()
-            .alias("FineSuspended"),
-            pl.col("Sentence")
-            .str.extract(r"Immigration Fine\: (.+?)Fine")
-            .str.replace(r"X\-\$", "")
-            .str.strip()
-            .cast(pl.Float64, strict=False)
-            .alias("ImmigrationFine"),
-            pl.col("Sentence")
-            .str.extract(r"Fine Imposed\: (.+?) Alias Warrant")
-            .str.strip()
-            .cast(pl.Float64, strict=False)
-            .alias("FineImposed"),
-            pl.col("Sentence")
-            .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing")
-            .str.replace(r"Prelim Hearing.+", "")
-            .str.strip()
-            .alias("DrugDocketFees"),
-            pl.col("Sentence")
-            .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
-            .str.replace(r"Amt.+", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("PrelimHearing"),
-            pl.col("Sentence")
-            .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
-            .str.replace_all(r"[A-Z\s]|\-|\$", "")
-            .cast(pl.Float64, strict=False)
-            .alias("AmtOverMinimumCVF"),
-            pl.col("Sentence")
-            .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
-            .str.strip()
-            .alias("WCFeeDA"),
-            pl.col("Sentence")
-            .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
-            .str.strip()
-            .alias("RemovalBill"),
-            pl.col("Sentence")
-            .str.extract(r"Crime History Fee\: (.+?) SX10")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("CrimeHistoryFee"),
-            pl.col("Sentence")
-            .str.extract(r"SX10\: (.+?)License Suspension Fee")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("SX10"),
-            pl.col("Sentence")
-            .str.extract(r"License Suspension Fee\: (.+?) WC Fee 85%")
-            .str.replace_all(r"[A-Z\s]+", "")
-            .cast(pl.Float64, strict=False)
-            .alias("LicenseSuspensionFee"),
-            pl.col("Sentence")
-            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:")
-            .str.replace(r"Demand Reduction Hearing.+", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("WCFee85"),
-            pl.col("Sentence")
-            .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee")
-            .str.replace_all(r"[A-Z]\-|\s|\$", "")
-            .str.strip()
-            .cast(pl.Float64, strict=False)
-            .alias("DemandReductionHearing"),
-            pl.col("Sentence")
-            .str.extract(r"Drug User Fee\: (.+?) Subpoena")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("DrugUserFee"),
-            pl.col("Sentence")
-            .str.extract(r"Subpoena\: (.+?) Attorney Fees")
-            .str.replace_all(r"[X\-\s\$]", "")
-            .cast(pl.Float64, strict=False)
-            .alias("Subpoena"),
-            pl.col("Sentence")
-            .str.extract(
-                r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
-            .alias("ImposedConfinementPeriod"),
-            pl.col("Sentence")
-            .str.extract(
-                r"Total Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
-            )
-            .alias("TotalConfinementPeriod"),
-            pl.col("Sentence")
-            .str.extract(
-                r"Suspended Confinement Period (\d+ Years, \d+ Months, \d+ Days\.)"
-            )
-            .alias("SuspendedConfinementPeriod"),
-            pl.col("Sentence")
-            .str.extract(r"Boot Camp\: (.+?) (Penitentiary|Life Without Parole)")
-            .str.replace(r"Penitentiary.+", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("BootCamp"),
-            pl.col("Sentence")
-            .str.extract(
-                r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1
-            )
-            .str.replace(r"Death.+", "")
-            .str.replace(r"Restitution.+", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("LifeWithoutParole"),
-            pl.col("Sentence")
-            .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1)
-            .str.strip()
-            .alias("Split"),
-            pl.col("Sentence")
-            .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
-            .str.strip()
-            .alias("ConcurrentSentence"),
-            pl.col("Sentence")
-            .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
-            .str.strip()
-            .alias("ConsecutiveSentence"),
-            pl.col("Sentence")
-            .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
-            .str.replace_all(r"[-0\s]", "")
-            .cast(pl.Categorical)
-            .alias("ElectronicMonitoring"),
-            pl.col("Sentence")
-            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
-            .str.replace_all(r"Death\: Life\:", "")
-            .str.replace(r'Life Without Parole\: ?X?','')
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("ReverseSplit"),
-            pl.col("Sentence")
-            .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
-            .alias("CoterminousSentence"),
-            pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
-            pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
-            pl.col("Sentence")
-            .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("ChainGang"),
-            pl.col("Sentence")
-            .str.extract(r"Jail\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("Jail"),
-            pl.col("Sentence")
-            .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)")
-            .alias("CommunityServiceHrs"),
-            pl.col("Sentence")
-            .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("JailDiversion"),
-            pl.col("Sentence")
-            .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
-            .cast(pl.Categorical)
-            .alias("Alcoholics Anonymous"),
-            pl.col("Sentence")
-            .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
-            .cast(pl.Categorical)
-            .alias("BadCheckSchool"),
-            pl.col("Sentence")
-            .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("InformalProbation"),
-            pl.col("Sentence")
-            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s")
-            .cast(pl.Categorical)
-            .alias("CourtReferralProgram"),
-            pl.col("Sentence")
-            .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
-            .alias("CommunityService"),
-            pl.col("Sentence")
-            .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
-            .alias("AlternativeSentencing"),
-            pl.col("Sentence")
-            .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
-            .alias("PreTrialDiversion"),
-            pl.col("Sentence")
-            .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
-            .cast(pl.Categorical)
-            .alias("DUISchool"),
-            pl.col("Sentence")
-            .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
-            .cast(pl.Categorical)
-            .alias("DefensiveDrivingSchool"),
-            pl.col("Sentence")
-            .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("DocCommunityCorrections"),
-            pl.col("Sentence")
-            .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("JailCommunityCorrections"),
-            pl.col("Sentence")
-            .str.extract(r"Mental Health\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("MentalHealth"),
-            pl.col("Sentence")
-            .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("AngerManagementProgram"),
-            pl.col("Sentence")
-            .str.extract(r"Drug Court\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("DrugCourt"),
-            pl.col("Sentence")
-            .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
-            .cast(pl.Categorical)
-            .alias("DocDrugProgram"),
-            pl.col("Sentence")
-            .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("DrugMeasureUnit"),
-            pl.col("Sentence")
-            .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("DrugNearProject"),
-            pl.col("Sentence")
-            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender")
-            .str.replace(r"Habitual Offender\:", "")
-            .str.replace(r"Sex Offender Community Notification\:", "")
-            .str.replace(r"Drug Volume\:", "")
-            .str.replace(r"Drug\:", "")
-            .str.replace(r"Drug Code\:\s?\d*", "")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("DrugsNearSchool"),
-            pl.col("Sentence")
-            .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
-            .str.strip()
-            .cast(pl.Categorical)
-            .alias("HabitualOffender"),
-            pl.col("Sentence")
-            .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
-            .str.replace_all(r"[X\s0-9]", "")
-            .str.replace(r"\.", "")
-            .cast(pl.Categorical)
-            .alias("SexOffenderCommunityNotification"),
-            pl.col("Sentence")
-            .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
-            .cast(pl.Float64, strict=False)
-            .alias("DrugVolume"),
-            pl.col("Sentence")
-            .str.extract(r"Drug Code\: (.+?)Habitual Offender Number")
-            .str.strip()
-            .cast(pl.Int64, strict=False)
-            .alias("DrugCode"),
-            pl.col("Sentence")
-            .str.extract(r"Habitual Offender Number\: (.+?)Victim")
-            .str.strip()
-            .alias("HabitualOffenderNumber"),
-            pl.col("Sentence")
-            .str.extract(r"Victim DOB\:\s+(\d?\d?/?\d?\d?/?\d?\d?\d?\d?)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("VictimDOB"),
-        ]
-    )
-    sent = sent.drop_nulls("Number")
-    sent = sent.fill_null("")
-    return sent
-
-
-#   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
-
-
-def read_query(path, window=None):
-    if isinstance(path, dict):
-        cf = path
-        path = cf["INPUTS"]
-    if os.path.splitext(path)[1] in (".xlsx", ".xls"):
-        query = pl.read_excel(
-            path,
-            xlsx2csv_options={"ignore_errors": True},
-            read_csv_options={"ignore_errors": True},
-        )
-    elif os.path.splitext(path)[1] == ".csv":
-        query = pl.read_csv(path, ignore_errors=True)
-    elif os.path.splitext(path)[1] == ".json":
-        query = pl.read_json(path)
-    elif os.path.splitext(path)[1] == ".parquet":
-        query = pl.read_parquet(path)
-    else:
-        return None
-    query = query.fill_null("")
-    if "TEMP_" in query.columns:
-        if window:
-            window.write_event_value(
-                "POPUP",
-                "Remove TEMP columns from input query spreadsheet and try again.",
-            )
-        else:
-            raise Exception(
-                "Remove TEMP columns from input query spreadsheet and try again."
-            )
-
-    found = query.shape[0]
-
-    pscols = [
-        "NAME",
-        "PARTY_TYPE",
-        "SSN",
-        "DOB",
-        "COUNTY",
-        "DIVISION",
-        "CASE_YEAR",
-        "NO_RECORDS",
-        "FILED_BEFORE",
-        "FILED_AFTER",
-    ]
-    tempcols = [
-        "TEMP_NAME",
-        "TEMP_PARTY_TYPE",
-        "TEMP_SSN",
-        "TEMP_DOB",
-        "TEMP_COUNTY",
-        "TEMP_DIVISION",
-        "TEMP_CASE_YEAR",
-        "TEMP_NO_RECORDS",
-        "TEMP_FILED_BEFORE",
-        "TEMP_FILED_AFTER",
-    ]
-
-    # add missing progress cols
-    for col in ("RETRIEVED", "CASES_FOUND", "QUERY_COMPLETE"):
-        if col not in query.columns:
-            query = query.with_columns(pl.lit("").alias(col))
-
-    # add matching temp columns for valid columns (i.e. 'Name' -> 'TEMP_NAME')
-    goodquery = False
-    for col in query.columns:
-        if col.upper().strip().replace(" ", "_") in pscols:
-            query = query.with_columns(
-                [pl.col(col).alias(f"TEMP_{col.upper().strip().replace(' ','_')}")]
+            names = (
+                names.groupby("Name")
+                .agg("CaseNumber", "Alias", "DOB")
+                .select(
+                    [
+                        pl.lit("").alias("AIS / Unique ID"),
+                        pl.col("Name"),
+                        pl.col("Alias").list.get(0),
+                        pl.col("DOB").list.get(0),
+                        pl.col("CaseNumber").list.lengths().alias("CaseCount"),
+                        pl.col("CaseNumber").list.join(", ").alias("Cases"),
+                    ]
+                )
             )
-            goodquery = True
-
-    # add other temp columns as empty
-    for col in tempcols:
-        if col not in query.columns:
-            query = query.with_columns([pl.lit("").alias(col)])
-
-    query = query.with_columns(
-        [
-            pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
-        ]
-    )
-
-    if goodquery:
-        print(f"{query.shape[0]} queries read from input query file.")
-        return query
-    else:
-        print(
-            "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
-        )
-        return None
-
-
-def fetch(
-    querypath="",
-    dirpath="",
-    cID="",
-    uID="",
-    pwd="",
-    criminal_only=False,
-    cf=None,
-    no_update=False,
-    debug=False,
-    window=None,
-):
-    """
-    Fetch case PDFs from Alacourt.com.
-    Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and download to `dirpath`.
-    Args:
-       querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
-       dirpath (str): Path to PDF output directory
-       cID (str): Customer ID on Alacourt.com
-       uID (str): User ID on Alacourt.com
-       pwd (str): Password on Alacourt.com
-       no_update (bool): Do not update query template after completion
-       debug (bool): Print detailed runtime information to console
-    """
-    if isinstance(querypath, dict):
-        cf = querypath
-    if cf != None:
-        querypath = cf["INPUTS"]
-        dirpath = cf["OUTPUT_PATH"]
-        cID = cf["ALA_CUSTOMER_ID"]
-        uID = cf["ALA_USER_ID"]
-        pwd = cf["ALA_PASSWORD"]
-        criminal_only = cf["CRIMINAL_ONLY"]
-    else:
-        cf = {
-            "INPUTS": querypath,
-            "OUTPUT_PATH": dirpath,
-            "ALA_CUSTOMER_ID": cID,
-            "ALA_USER_ID": uID,
-            "ALA_PASSWORD": pwd,
-            "CRIMINAL_ONLY": criminal_only,
+            names = names.sort("Name")
+            names = names.filter(pl.col("Name") != "")
+        self._pairs_template = names
+        return self._pairs_template
+
+    def write_tables(self, path):
+        all_tables = {
+            'cases': self._cases, 
+            'charges': self._charges, 
+            'fees': self._fees, 
+            'sentences': self._sentences, 
+            'financial-history': self._financial_history, 
+            'witnesses': self._witnesses, 
+            'attorneys': self._attorneys, 
+            'images': self._images, 
+            'case-action-summary': self._case_action_summary
         }
+        only_df_vars = {}
+        for x in all_tables:
+            if isinstance(all_tables[x], pl.dataframe.frame.DataFrame):
+                only_df_vars.update({x: all_tables[x]})
+        write(only_df_vars, path, log=True)
+        return only_df_vars
+    
+    def write_archive(self, path):
+        if not self.is_read:
+            self.read()
+        cols = [col for col in ["CaseNumber", "Path", "Timestamp", "AllPagesText"] if col in self.archive.columns]
+        out = self.archive.select(cols)
+        write({'archive': out}, path, log=True)
+        return out
 
-    query = read_query(cf["INPUTS"])
-
-    # start browser and authenticate
-    opt = webdriver.ChromeOptions()
-    opt.add_experimental_option(
-        "prefs",
-        {
-            "download.default_directory": dirpath,  # Set default directory for downloads
-            "download.prompt_for_download": False,  # To auto download the file
-            "download.directory_upgrade": True,
-            "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
-        },
-    )
-    print("Starting browser... Do not close while in progress!")
-    driver = webdriver.Chrome(options=opt)
-    login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
-
-    for i, r in enumerate(query.rows(named=True)):
-        if query[i, "QUERY_COMPLETE"] == "Y":
-            continue
-        if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
-            login(driver, cID, uID, pwd, window=window)
-        # driver.implicitly_wait(1)
-        results = party_search(
-            driver,
-            name=r["TEMP_NAME"],
-            party_type=r["TEMP_PARTY_TYPE"],
-            ssn=r["TEMP_SSN"],
-            dob=r["TEMP_DOB"],
-            county=r["TEMP_COUNTY"],
-            division=r["TEMP_DIVISION"],
-            case_year=r["TEMP_CASE_YEAR"],
-            filed_before=r["TEMP_FILED_BEFORE"],
-            filed_after=r["TEMP_FILED_AFTER"],
-            criminal_only=criminal_only,
-            window=window,
-        )
-
-        if len(results) > 0:
-            print(
-                f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']} ({len(results)} records returned)"
-            )
-            if window:
-                window.write_event_value("PROGRESS-TEXT", 0)
-                window.write_event_value("PROGRESS-TEXT-TOTAL", len(results))
-                for x, url in enumerate(results):
-                    window.write_event_value("PROGRESS-TEXT", x + 1)
-                    downloadPDF(driver, url)
-            else:
-                for x, url in enumerate(tqdm(results)):
-                    downloadPDF(driver, url)
-            query[i, "CASES_FOUND"] = len(results)
-            query[i, "RETRIEVED"] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
-            query[i, "QUERY_COMPLETE"] = "Y"
-            if not no_update:
-                qwrite = query.drop(
-                    "TEMP_NAME",
-                    "TEMP_PARTY_TYPE",
-                    "TEMP_SSN",
-                    "TEMP_DOB",
-                    "TEMP_COUNTY",
-                    "TEMP_DIVISION",
-                    "TEMP_CASE_YEAR",
-                    "TEMP_NO_RECORDS",
-                    "TEMP_FILED_BEFORE",
-                    "TEMP_FILED_AFTER",
-                )
-                write(qwrite, path=cf["INPUTS"], overwrite=True)
-        else:
-            print(f"Found no results: {query[i, 'TEMP_NAME']}")
-            query[i, "QUERY_COMPLETE"] = "Y"
-            query[i, "CASES_FOUND"] = 0
-            query[i, "RETRIEVED"] = time.time()
-            if not no_update:
-                qwrite = query.drop(
-                    "TEMP_NAME",
-                    "TEMP_PARTY_TYPE",
-                    "TEMP_SSN",
-                    "TEMP_DOB",
-                    "TEMP_COUNTY",
-                    "TEMP_DIVISION",
-                    "TEMP_CASE_YEAR",
-                    "TEMP_NO_RECORDS",
-                    "TEMP_FILED_BEFORE",
-                    "TEMP_FILED_AFTER",
-                )
-                write(qwrite, path=cf["INPUTS"], overwrite=True)
-
-    if window:
-        window.write_event_value("COMPLETE-SQ", time.time())
-    print("Completed query template.")
-    return query
-
+## COMMAND LINE INTERFACE
 
+@app.command(no_args_is_help=True)
 def party_search(
-    driver,
-    name="",
-    party_type="",
-    ssn="",
-    dob="",
-    county="",
-    division="",
-    case_year="",
-    filed_before="",
-    filed_after="",
-    debug=False,
-    cID="",
-    uID="",
-    pwd="",
-    criminal_only=False,
-    window=None,
+    queue_path: Annotated[Path, typer.Argument(help="Path to queue table with one or more columns: Name, Party Type, SSN, DOB, County, Division, Case Year, Filed Before, Filed After, No Records.", show_default=False)],
+    output_path: Annotated[Path, typer.Argument(help="Path to output results table. Will attempt to append to existing table at output path.", show_default=False)],
+    customer_ID: Annotated[str, typer.Option("--customer-id", "-c", help="Customer ID for Alacourt login.", prompt="Customer ID", show_default=False)],
+    user_ID: Annotated[str, typer.Option("--user-id", "-u", help="User ID for Alacourt login.", prompt="User ID", show_default=False)],
+    password: Annotated[str, typer.Option("--password", "-p", help="Password for Alacourt login.", prompt="Password", hide_input=True, show_default=False)],
+    criminal_only: Annotated[bool, typer.Option("--criminal-only", help="Only search criminal cases.", show_default=False)] = False,
+    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False
 ):
     """
-    Collect PDFs via SJIS Party Search Form from Alacourt.com
-    Returns list of URLs for downloadPDF() to download
-
-    Args:
-        driver (WebDriver): selenium/chrome web driver object
-        name (str, optional): Name (LAST FIRST)
-        party_type (str, optional): "Defendants" | "Plaintiffs" | "ALL"
-        ssn (str, optional): Social Security Number
-        dob (str, optional): Date of Birth
-        county (str, optional): County
-        division (str, optional): "All Divisions"
-             "Criminal Only"
-             "Civil Only"
-             "CS - CHILD SUPPORT"
-             "CV - CIRCUIT - CIVIL"
-             "CC - CIRCUIT - CRIMINAL"
-             "DV - DISTRICT - CIVIL"
-             "DC - DISTRICT - CRIMINAL"
-             "DR - DOMESTIC RELATIONS"
-             "EQ - EQUITY-CASES"
-             "MC - MUNICIPAL-CRIMINAL"
-             "TP - MUNICIPAL-PARKING"
-             "SM - SMALL CLAIMS"
-             "TR - TRAFFIC"
-        case_year (str, optional): YYYY
-        filed_before (str, optional): M/DD/YYYY
-        filed_after (str, optional): M/DD/YYYY
-        cID (str): Customer ID on Alacourt.com
-        uID (str): User ID on Alacourt.com
-        pwd (str): Password on Alacourt.com
-        criminal_only (bool, optional): Only search criminal cases
-        debug (bool, optional): Print detailed logs.
-
-    Returns:
-        List[str] of URLs to PDF
-    """
-
-    if "frmIndexSearchForm" not in driver.current_url:
-        driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
-
-    has_window = False if window == "None" else True
-
-    # connection error
-    try:
-        party_name_box = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName"
-        )
-    except selenium.common.exceptions.NoSuchElementException:
-        dlog(
-            """NoSuchElementException on `party_name_box = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")`""",
-            cf=debug,
-        )
-        if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
-            time.sleep(2)
-            login(driver, cID=cID, uID=uID, pwd=pwd)
-            driver.implicitly_wait(1)
-        driver.get("https:v2.alacourt.com/frmIndexSearchForm.aspx")
-        print("Successfully connected and logged into Alacourt!")
-
-    # field search
-
-    time.sleep(0.5)
-
-    # name
-    if name != "":
-        driver.implicitly_wait(1)
-        try:
-            party_name_box.send_keys(name)
-        except selenium.common.exceptions.StaleElementReferenceException:
-            time.sleep(2)
-            driver.implicitly_wait(2)
-            party_name_box.send_keys(name)
-    # ssn
-    if ssn != "":
-        ssn_box = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN"
-        )
-        ssn_box.send_keys(ssn)
-    # dob
-    if dob != "":
-        date_of_birth_box = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtDOB"
-        )
-        date_of_birth_box.send_keys(dob)
-    # party type
-    if party_type == "Plaintiffs":
-        driver.find_element(
-            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_0"
-        ).click()
-    if party_type == "Defendants":
-        driver.find_element(
-            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_1"
-        ).click()
-    if party_type == "ALL":
-        driver.find_element(
-            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_2"
-        ).click()
-    # division
-    if division == "" and not criminal_only:
-        division = "All Divisions"
-    if criminal_only:
-        division = "Criminal Only"
-    division_select = driver.find_element(
-        by=By.ID, value="ContentPlaceHolder1_UcddlDivisions1_ddlDivision"
-    )
-    sdivision = Select(division_select)
-    sdivision.select_by_visible_text(division)
-    if county == "":
-        county = "Statewide Search"
-    county_select = driver.find_element(
-        by=By.ID, value="ContentPlaceHolder1_ddlCounties"
-    )
-    scounty = Select(county_select)
-    scounty.select_by_visible_text(county)
-    if case_year != "" and case_year != None:
-        case_year_select = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear"
-        )
-        scase_year = Select(case_year_select)
-        scase_year.select_by_visible_text(str(case_year))
-    no_records_select = driver.find_element(
-        by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfRecords"
-    )
-    sno_records = Select(no_records_select)
-    sno_records.select_by_visible_text("1000")
-    if filed_before != "":
-        filed_before_box = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtFrom"
-        )
-        filed_before_box.send_keys(filed_before)
-    if filed_after != "":
-        filed_after_box = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$txtTo"
-        )
-        filed_after_box.send_keys(filed_after)
-
-    # submit search
-    search_button = driver.find_element(by=By.ID, value="searchButton")
-
-    time.sleep(0.25)
-
-    try:
-        search_button.click()
-    except:
-        driver.implicitly_wait(2)
-        time.sleep(2)
-
-    time.sleep(0.5)
-
-    dlog("Submitted party search form...", cf=debug)
-
-    # count pages
-    try:
-        page_counter = driver.find_element(
-            by=By.ID, value="ContentPlaceHolder1_dg_tcPageXofY"
-        ).text
-        pages = int(page_counter.strip()[-1])
-
-    except:
-        pages = 1
-
-    # count results
-    try:
-        results_indicator = driver.find_element(
-            by=By.ID, value="ContentPlaceHolder1_lblResultCount"
-        )
-        results_count = int(
-            results_indicator.text.replace("Search Results: ", "")
-            .replace(" records returned.", "")
-            .strip()
-        )
-        dlog(f"Found {results_count} results, fetching URLs and downloading PDFs...", cf=debug)
-    except:
-        results_count = 0
-
-
-    # get PDF links from each page
-    pdflinks = []
-    i = 0
-    for i in range(0, pages):
-        hovers = driver.find_elements(By.CLASS_NAME, "menuHover")
-        for x in hovers:
-            try:
-                a = x.get_attribute("href")
-                if "PDF" in a:
-                    pdflinks.append(a)
-            except:
-                pass
-        try:
-            pager_select = Select(
-                driver.find_element(
-                    by=By.NAME, value="ctl00$ContentPlaceHolder1$dg$ctl18$ddlPages"
-                )
-            )
-            next_pg = int(pager_select.text) + 1
-        except:
-            try:
-                next_button = driver.find_element(
-                    by=By.ID, value="ContentPlaceHolder1_dg_ibtnNext"
-                )
-                next_button.click()
-            except:
-                continue
-    return pdflinks
-
-
-def downloadPDF(driver, url, cID="", uID="", pwd="", window=None):
-    """
-    With selenium WebDriver `driver`, download PDF at `url`.
-
-    Args:
-        driver (WebDriver): Google Chrome selenium.WebDriver() object
-        url (str): URL to Alacourt case detail PDF download
-        cID (str, optional): Customer ID on Alacourt.com
-        uID (str, optional): User ID on Alacourt.com
-        pwd (str, optional): Password on Alacourt.com
-
-    """
-    if (
-        driver.current_url == "https://v2.alacourt.com/frmlogin.aspx"
-        and cID != ""
-        and uID != ""
-        and pwd != ""
-    ):
-        login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
-    a = driver.get(url)
-
-
-def login(driver, cID, uID="", pwd="", path="", window=None):
-    """Login to Alacourt.com using (driver) and auth (cID, username, pwd) for browser download to directory at (path)
-
-    Args:
-        driver (WebDriver): Google Chrome selenium.WebDriver() object
-        cID (str): Alacourt.com Customer ID
-        uID (str): Alacourt.com User ID
-        pwd (str): Alacourt.com Password
-        path (str, optional): Set browser download path
-
-    Returns:
-        driver (WebDriver): selenium engine
-    """
-    if driver == None:
-        options = webdriver.ChromeOptions()
-        options.add_experimental_option(
-            "prefs",
-            {
-                "download.default_directory": path,  # Change default directory for downloads
-                "download.prompt_for_download": False,  # To auto download the file
-                "download.directory_upgrade": True,
-                "plugins.always_open_pdf_externally": True,  # It will not display PDF directly in chrome
-            },
-        )
-        driver = webdriver.Chrome(options=options)
-
-    print("Connecting to Alacourt...")
-
-    login_screen = driver.get("https://v2.alacourt.com/frmlogin.aspx")
-
-    print("Logging in...")
-
-    cID_box = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder$txtCusid")
-    username_box = driver.find_element(
-        by=By.NAME, value="ctl00$ContentPlaceHolder$txtUserId"
-    )
-    pwd_box = driver.find_element(
-        by=By.NAME, value="ctl00$ContentPlaceHolder$txtPassword"
-    )
-    login_button = driver.find_element(by=By.ID, value="ContentPlaceHolder_btLogin")
-
-    cID_box.send_keys(cID)
-    username_box.send_keys(uID)
-    pwd_box.send_keys(pwd)
-
-    login_button.click()
-
-    try:
-        continueLogIn = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder$btnContinueLogin"
-        )
-        continueLogIn.click()
-    except:
-        pass
-
-    driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
-
-    print("Successfully connected and logged into Alacourt!")
-
-    return driver
-
-
-def empty_query(path):
-    """Create empty spreadsheet to fill and import as query submit search list to retrieve matching case records from Alacourt.com.
-
-    Args:
-        path (str): Desired output path (.xls, .xlsx)
-
-    """
-    success = True
-    empty = pl.DataFrame(
-        columns=[
-            "NAME",
-            "PARTY_TYPE",
-            "SSN",
-            "DOB",
-            "COUNTY",
-            "DIVISION",
-            "CASE_YEAR",
-            "NO_RECORDS",
-            "FILED_BEFORE",
-            "FILED_AFTER",
-            "RETRIEVED",
-            "CASES_FOUND",
-        ]
-    )
-    return write(empty, sheet_names="query", path=path, overwrite=True)
-
-
-#   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
-
-
-def loadgui():
-    """
-    Load PySimpleGUI tk graphical interface
-    """
-    import PySimpleGUI as sg
-    import platform
-    import threading
-
-    psys = platform.system()
-    plat = platform.platform()
-    if "Darwin" in (plat, psys) or "macOS" in (plat, psys):  # set MacOS element sizes
-        (
-            HEADER_FONT,
-            LOGO_FONT,
-            ASCII_FONT,
-            BODY_FONT,
-            TAB_FONT,
-            WINDOW_RESIZE,
-            WINDOW_SIZE,
-        ) = (
-            "Default 22",
-            "Courier 20",
-            "Courier 14",
-            "Default 12",
-            "Courier",
-            False,
-            [480, 510],
-        )
-    elif "Windows" in (plat, psys):  # set Windows element sizes
-        (
-            HEADER_FONT,
-            LOGO_FONT,
-            ASCII_FONT,
-            BODY_FONT,
-            TAB_FONT,
-            WINDOW_RESIZE,
-            WINDOW_SIZE,
-        ) = (
-            "Default 14",
-            "Courier 17",
-            "Courier 11",
-            "Default 10",
-            "Courier 11",
-            True,
-            [490, 540],
-        )
-        try:
-            from ctypes import windll
-
-            windll.shcore.SetProcessDpiAwareness(1)
-        except:
-            pass
-    else:  # set Linux, etc. element sizes
-        (
-            HEADER_FONT,
-            LOGO_FONT,
-            ASCII_FONT,
-            BODY_FONT,
-            TAB_FONT,
-            WINDOW_RESIZE,
-            WINDOW_SIZE,
-        ) = (
-            "Default 15",
-            "Courier 12",
-            "Courier 13",
-            "Default 10",
-            "Courier",
-            True,
-            [540, 540],
-        )
-    sg.theme("Black")
-    sg.set_options(font=BODY_FONT)
-    fetch_layout = [
-        [
-            sg.Text(
-                """Collect case PDFs in bulk from Alacourt.com.""",
-                font=HEADER_FONT,
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text(
-                """Requires Google Chrome. Use column headers NAME, PARTY_TYPE, SSN,\nDOB, COUNTY, DIVISION, CASE_YEAR, and/or FILED_BEFORE in an\nExcel spreadsheet to submit a list of queries for Alacorder to scrape. Each\ncolumn corresponds to a field in Alacourt's Party Search form.""",
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text("Input Path: "),
-            sg.InputText(
-                tooltip="Existing query template (.xlsx)",
-                size=[22, 10],
-                key="SQ-INPUTPATH",
-                focus=True,
-            ),
-            sg.FileBrowse(button_text="Select File", button_color=("white", "black")),
-            sg.Button(
-                button_text="New Query",
-                button_color=("white", "black"),
-                k="NEWQUERY",
-                enable_events=True,
-            ),
-        ],
-        [
-            sg.Text("Output Directory: "),
-            sg.InputText(
-                tooltip="PDF download destination folder",
-                size=[26, 10],
-                key="SQ-OUTPUTPATH",
-            ),
-            sg.FolderBrowse(
-                button_text="Select Folder", button_color=("white", "black")
-            ),
-        ],
-        [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
-        [
-            sg.Text("Customer ID: "),
-            sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
-        ],
-        [
-            sg.Text("User ID:"),
-            sg.Input(key="SQ-USERID", size=(20, 1)),
-        ],
-        [
-            sg.Text("Password: "),
-            sg.InputText(key="SQ-PASSWORD", password_char="*", size=(18, 1)),
-        ],
-        [
-            sg.Button(
-                "Start Query",
-                key="SQ",
-                button_color=("white", "black"),
-                pad=(10, 10),
-                disabled_button_color=("grey", "black"),
-                bind_return_key=True,
-            )
-        ],
-    ]
-    archive_layout = [
-        [
-            sg.Text(
-                """Create full text archives from a directory\nof PDF cases.""",
-                font=HEADER_FONT,
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text(
-                """Case text archives require a fraction of the storage capacity and\nprocessing time used to process PDF directories. Before exporting\nyour data to tables, create an archive with supported file extensions\n.parquet, .json, and .csv. Once archived, use your case text archive\nas an input for multitable or single table export.""",
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text("Input Directory: "),
-            sg.InputText(
-                tooltip="PDF directory or full text archive (.parquet, .json, .csv)",
-                size=[25, 1],
-                key="MA-INPUTPATH",
-                focus=True,
-            ),
-            sg.FolderBrowse(
-                button_text="Select Folder", button_color=("white", "black")
-            ),
-        ],
-        [
-            sg.Text("Output Path: "),
-            sg.InputText(
-                tooltip="Output archive file path (.parquet, .json, .csv)",
-                size=[39, 1],
-                key="MA-OUTPUTPATH",
-            ),
-        ],
-        [
-            sg.Text("Skip Cases From:  "),
-            sg.Input(
-                tooltip="Skip all input cases found in PDF directory or archive (.parquet, .json, .csv)",
-                key="MA-SKIP",
-                size=[36, 1],
-                pad=(0, 10),
-            ),
-        ],
-        [
-            sg.Text("Max cases: "),
-            sg.Input(key="MA-COUNT", default_text="0", size=[5, 1]),
-            sg.Checkbox("Allow Overwrite", default=True, key="MA-OVERWRITE"),
-        ],
-        [
-            sg.Button(
-                "Make Archive",
-                button_color=("white", "black"),
-                key="MA",
-                enable_events=True,
-                bind_return_key=True,
-                disabled_button_color=("grey", "black"),
-                pad=(10, 10),
-            )
-        ],
-    ]  # "MA"
-    append_layout = [
-        [
-            sg.Text(
-                """Append case text archive with the contents\nof a case directory or archive.""",
-                font=HEADER_FONT,
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text(
-                """Case text archives require a fraction of the storage capacity and\nprocessing time used to process PDF directories. Before exporting\nyour data to tables, create an archive with a supported file\nextension (.parquet, .json, .csv). Once archived, use your case text\narchive as an input for table export.""",
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text("To Append: "),
-            sg.InputText(
-                tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
-                size=[30, 10],
-                key="AA-INPUTPATH",
-                focus=True,
-            ),
-            sg.FileBrowse(button_text="Select File", button_color=("white", "black")),
-        ],
-        [
-            sg.Text("To Be Appended: "),
-            sg.InputText(
-                tooltip="Destination full text archive (.parquet, .json, .csv)",
-                size=[26, 10],
-                key="AA-OUTPUTPATH",
-            ),
-            sg.FileBrowse(button_text="Select File", button_color=("white", "black")),
-        ],
-        [
-            sg.Button(
-                "Append Archives",
-                key="AA",
-                button_color=("white", "black"),
-                pad=(10, 10),
-                disabled_button_color=("grey", "black"),
-                bind_return_key=True,
-            )
-        ],
-    ]  # "AA"
-    sum_layout = [
-        [
-            sg.Text(
-                """Pair cases by AIS number to create a\npaired voting rights summary table.""",
-                font=HEADER_FONT,
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text(
-                """To make a voting rights summary table, start by creating an AIS / Unique ID\npair template, fill the template with AIS numbers or another identifier\nto match names in common, then enter the template path and case\ninput path below.""",
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text("Input Path:  "),
-            sg.InputText(
-                tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
-                size=[31, 10],
-                key="SUM-INPUTPATH",
-                focus=True,
-            ),
-            sg.FileBrowse(button_text="Select File", button_color=("white", "black")),
-        ],
-        [
-            sg.Text("Pairs: "),
-            sg.InputText(
-                tooltip="Destination full text archive (.parquet, .json, .csv)",
-                size=[32, 10],
-                key="SUM-PAIRS",
-            ),
-            sg.Button(
-                button_text="Make Template", button_color=("white", "black"), key="MT"
-            ),
-        ],
-        [
-            sg.Text("Output Path:  "),
-            sg.InputText(
-                tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
-                size=[40, 10],
-                key="SUM-OUTPUTPATH",
-                focus=True,
-            ),
-        ],
-        [sg.Checkbox("Allow Overwrite", default=True, key="SUM-OVERWRITE")],
-        [
-            sg.Button(
-                "Create Summary",
-                key="SUM",
-                button_color=("white", "black"),
-                pad=(10, 10),
-                disabled_button_color=("grey", "black"),
-                bind_return_key=True,
-            )
-        ],
-    ]  # "SUM"
-    table_layout = [
-        [
-            sg.Text(
-                """Export data tables from a case archive\nor PDF directory.""",
-                font=HEADER_FONT,
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text(
-                """Alacorder processes case detail PDFs and case text archives into data\ntables suitable for research purposes. Enter PDF directory or case text\narchive path and output file path (.xlsx, .xls, .csv, .json) to begin. CSV\nand JSON support single table selection only.""",
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text("Input Path:  "),
-            sg.InputText(
-                tooltip="PDF directory or full text archive (.parquet, .json, .csv)",
-                size=[28, 10],
-                key="TB-INPUTPATH",
-                focus=True,
-            ),
-            sg.FolderBrowse(
-                button_text="Select Folder", button_color=("white", "black")
-            ),
-        ],
-        [
-            sg.Text("Output Path: "),
-            sg.InputText(
-                tooltip="Multitable export (.xlsx, .xls) or single-table export (.xlsx, .xls, .json, .csv)",
-                size=[39, 10],
-                key="TB-OUTPUTPATH",
-            ),
-        ],
-        [
-            sg.Radio("All Tables (.xlsx, .xls)", "TABLE", key="TB-ALL", default=True),
-            sg.Radio("Cases", "TABLE", key="TB-CASES", default=False),
-            sg.Radio("Sentences", "TABLE", key="TB-SENTENCES", default=False),
-            sg.Radio("Fees", "TABLE", key="TB-FEES", default=False),
-        ],
-        [
-            sg.Radio("Case Action Summary", "TABLE", key="TB-CAS", default=False),
-            sg.Radio("Witnesses", "TABLE", key="TB-WITNESSES", default=False),
-            sg.Radio("Images", "TABLE", key="TB-IMAGES", default=False),
-        ],
-        [
-            sg.Radio("Attorneys", "TABLE", key="TB-ATTORNEYS", default=False),
-            sg.Radio("Settings", "TABLE", key="TB-SETTINGS", default=False),
-            sg.Radio("Financial History", "TABLE", key="TB-HISTORY", default=False),
-        ],
-        [
-            sg.Radio("All Charges", "TABLE", key="TB-CHARGES", default=False),
-            sg.Radio(
-                "Disposition Charges", "TABLE", key="TB-DISPOSITION", default=False
-            ),
-            sg.Radio("Filing Charges", "TABLE", key="TB-FILING", default=False),
-        ],
-        [
-            sg.Text("Max cases: "),
-            sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
-            sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
-        ],
-        [
-            sg.Button(
-                "Export Table",
-                key="TB",
-                button_color=("white", "black"),
-                pad=(10, 10),
-                disabled_button_color=("grey", "black"),
-                bind_return_key=True,
-            )
-        ],
-    ]  # "TB"
-    rename_layout = [
-        [
-            sg.Text(
-                """Rename case PDFs in directory to\ncase numbers.""",
-                font=HEADER_FONT,
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text(
-                """To rename each PDF case in a directory to its case number, enter the\ndirectory path below and click start. Some devices may require a\nreboot or reindex to reflect updated file names. Duplicate cases will\nbe removed.""",
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text("Directory: "),
-            sg.InputText(
-                tooltip="PDF Directory",
-                size=[30, 10],
-                key="RN-INPUTPATH",
-                focus=True,
-            ),
-            sg.FolderBrowse(
-                button_text="Select Folder", button_color=("white", "black")
-            ),
-        ],
-        [
-            sg.Button(
-                "Rename Cases",
-                key="RN",
-                button_color=("white", "black"),
-                pad=(10, 10),
-                disabled_button_color=("grey", "black"),
-                bind_return_key=True,
-            )
-        ],
-    ]  # "RN"
-    about_layout = [
-        [
-            sg.Text(
-                f"""╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗\n╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ \n╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝\nversion {version}""",
-                font=ASCII_FONT,
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text(
-                "Alacorder retrieves and processes\nAlacourt case detail PDFs into\ndata tables and archives.",
-                font=HEADER_FONT,
-                pad=(5, 5),
-            )
-        ],
-        [
-            sg.Text(
-                """View documentation, source code, and latest updates at\ngithub.com/sbrobson959/alacorder.\n\n© 2023 Sam Robson""",
-                font=BODY_FONT,
-            )
-        ],
-    ]  # "ABOUT"
-    tabs = sg.TabGroup(
-        expand_x=True,
-        expand_y=False,
-        size=[0, 0],
-        font=TAB_FONT,
-        layout=[
-            [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
-            [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
-            [sg.Tab("table", layout=table_layout, pad=(2, 2))],
-            [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
-            [sg.Tab("rename", layout=rename_layout, pad=(2, 2))],
-            [sg.Tab("append", layout=append_layout, pad=(2, 2))],
-            [sg.Tab("about", layout=about_layout, pad=(2, 2))],
-        ],
-    )
-    layout = [
-        [sg.Text("ALACORDER", font=LOGO_FONT, pad=(5, 5))],
-        [tabs],
-        [
-            sg.ProgressBar(
-                100,
-                size=[5, 10],
-                expand_y=False,
-                orientation="h",
-                expand_x=True,
-                key="PROGRESS",
-                bar_color="black",
-            )
-        ],
-        [
-            sg.Multiline(
-                expand_x=True,
-                expand_y=True,
-                background_color="black",
-                reroute_stdout=True,
-                pad=(5, 5),
-                font="Courier 11",
-                write_only=True,
-                autoscroll=True,
-                no_scrollbar=True,
-                size=[None, 4],
-                border_width=0,
-            )
-        ],
-    ]
-    window = sg.Window(
-        title=name,
-        layout=layout,
-        grab_anywhere=True,
-        resizable=WINDOW_RESIZE,
-        size=WINDOW_SIZE,
-    )
-    thread = False
-    while True:
-        event, values = window.read()
-        if event in ("Exit", "Quit", sg.WIN_CLOSED):
-            window.close()
-            break
-        elif "TOTAL" in event and "PROGRESS" in event:
-            window["PROGRESS"].update(max=values[event], current_count=0)
-        elif "PROGRESS" in event and "TOTAL" not in event:
-            window["PROGRESS"].update(current_count=values[event])
-        elif "ERROR" in event:
-            window["AA"].update(disabled=False)
-            window["SQ"].update(disabled=False)
-            window["MA"].update(disabled=False)
-            window["TB"].update(disabled=False)
-            window["MA"].update(disabled=False)
-            window["SUM"].update(disabled=False)
-            window["RN"].update(disabled=False)
-        elif "COMPLETE" in event:
-            print("Alacorder completed the task.")
-            window["AA"].update(disabled=False)
-            window["SQ"].update(disabled=False)
-            window["MA"].update(disabled=False)
-            window["TB"].update(disabled=False)
-            window["MA"].update(disabled=False)
-            window["SUM"].update(disabled=False)
-            window["RN"].update(disabled=False)
-            window["PROGRESS"].update(current_count=0, max=100)
-            sg.popup("Alacorder completed the task.")
-            continue
-        elif event == "NEWQUERY":
-            if window["SQ-INPUTPATH"].get() == "":
-                sg.popup(
-                    "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
-                )
-            else:
-                if empty_query(window["SQ-INPUTPATH"].get()):
-                    sg.popup("Alacorder created query template.")
-                else:
-                    sg.popup(
-                        "Enter valid path with .xlsx extension in Input Path box and try again."
-                    )
-        elif event == "MT":
-            cf = set(
-                window["SUM-INPUTPATH"].get(),
-                window["SUM-PAIRS"].get(),
-                pairs=window["SUM-PAIRS"].get(),
-                log=True,
-                no_write=False,
-                overwrite=window["SUM-OVERWRITE"].get(),
-                window=window,
-            )
-            thread = threading.Thread(target=pairs, args=[cf], daemon=True).start()
-            print("Creating AIS / Unique ID pairs template...")
-            window["MT"].update(disabled=True)
-        elif event == "SUM":
-            cf = set(
-                window["SUM-INPUTPATH"].get(),
-                window["SUM-OUTPUTPATH"].get(),
-                pairs=window["SUM-PAIRS"].get(),
-                vrr_summary=True,
-                log=True,
-                no_write=False,
-                overwrite=window["SUM-OVERWRITE"].get(),
-                window=window,
-            )
-            thread = threading.Thread(
-                target=vrr_summary, args=[cf], daemon=True
-            ).start()
-            window["SUM"].update(disabled=True)
-        elif event == "POPUP":
-            sg.popup(values["POPUP"])
-        elif event == "TB":
-            table = ""
-            table = "all" if window["TB-ALL"].get() else table
-            table = "cases" if window["TB-CASES"].get() else table
-            table = "charges" if window["TB-CHARGES"].get() else table
-            table = "fees" if window["TB-FEES"].get() else table
-            table = "case-action-summary" if window["TB-CAS"].get() else table
-            table = "witnesses" if window["TB-WITNESSES"].get() else table
-            table = "images" if window["TB-IMAGES"].get() else table
-            table = "attorneys" if window["TB-ATTORNEYS"].get() else table
-            table = "settings" if window["TB-SETTINGS"].get() else table
-            table = "disposition" if window["TB-DISPOSITION"].get() else table
-            table = "filing" if window["TB-FILING"].get() else table
-            table = "financial-history" if window["TB-HISTORY"].get() else table
-            table = "sentences" if window["TB-SENTENCES"].get() else table
-            if (
-                window["TB-INPUTPATH"].get() == ""
-                or window["TB-OUTPUTPATH"].get() == ""
-            ):
-                sg.popup("Check configuration and try again.")
-            else:
-                cf = set(
-                    window["TB-INPUTPATH"].get(),
-                    window["TB-OUTPUTPATH"].get(),
-                    count=int(window["TB-COUNT"].get()),
-                    table=table,
-                    log=True,
-                    overwrite=window["TB-OVERWRITE"].get(),
-                    no_prompt=True,
-                    archive=False,
-                    window=window,
-                )
-                thread = threading.Thread(target=init, args=[cf], daemon=True).start()
-                window["TB"].update(disabled=True)
-                continue
-        elif event == "MA":
-            if (
-                window["MA-INPUTPATH"].get() == ""
-                or window["MA-OUTPUTPATH"].get() == ""
-            ):
-                sg.popup("Check configuration and try again.")
-                window["MA"].update(disabled=False)
-                continue
-            try:
-                count = int(window["MA-COUNT"].get().strip())
-            except:
-                count = 0
-            try:
-                cf = set(
-                    window["MA-INPUTPATH"].get(),
-                    window["MA-OUTPUTPATH"].get(),
-                    count=count,
-                    archive=True,
-                    log=True,
-                    overwrite=window["MA-OVERWRITE"].get(),
-                    no_prompt=True,
-                    window=window,
-                )
-            except:
-                sg.popup("Check configuration and try again.")
-                window["MA"].update(disabled=False)
-                continue
-            if os.path.splitext(window["MA-OUTPUTPATH"].get())[1] in (
-                ".parquet",
-                ".json",
-                ".csv",
-            ):
-                thread = threading.Thread(
-                    target=archive, args=[cf], daemon=True
-                ).start()
-                window["MA"].update(disabled=True)
-            continue
-        elif event == "SQ":
-            if (
-                window["SQ-INPUTPATH"].get() == ""
-                or window["SQ-OUTPUTPATH"].get() == ""
-            ):
-                sg.popup("Check configuration and try again.")
-                continue
-            try:
-                pwd = window["SQ-PASSWORD"].get()
-                window["SQ"].update(disabled=True)
-                thread = threading.Thread(
-                    target=fetch,
-                    args=(
-                        window["SQ-INPUTPATH"].get(),
-                        window["SQ-OUTPUTPATH"].get(),
-                        window["SQ-CUSTOMERID"].get(),
-                        window["SQ-USERID"].get(),
-                        pwd,
-                        window["SQ-CRIMINALONLY"].get(),
-                        None,
-                        False,
-                        False,
-                        window,
-                    ),
-                    daemon=True,
-                ).start()
-                continue
-            except:
-                print("Check configuration and try again.")
-                window["SQ"].update(disabled=False)
-                continue
-        elif event == "AA":
-            if (
-                window["AA-INPUTPATH"].get() == ""
-                or window["AA-OUTPUTPATH"].get() == ""
-            ):
-                sg.popup("Check configuration and try again.")
-                continue
-            try:
-                window["AA"].update(disabled=True)
-                thread = threading.Thread(
-                    target=append_archive,
-                    args=(
-                        window["AA-INPUTPATH"].get(),
-                        window["AA-OUTPUTPATH"].get(),
-                    ),
-                    kwargs={"window": window},
-                    daemon=True,
-                ).start()
-                continue
-            except:
-                print("Check configuration and try again.")
-                window["AA"].update(disabled=False)
-                continue
-        elif event == "RN":
-            if window["RN-INPUTPATH"].get() == "":
-                sg.popup("Enter directory path and try again.")
-                continue
-            else:
-                cf = set(window["RN-INPUTPATH"].get(), log=True, window=window)
-                window["RN"].update(disabled=True)
-                thread = threading.Thread(
-                    target=rename_pdfs,
-                    args=[cf],
-                    daemon=True,
-                ).start()
-                continue
-        else:
-            pass
-
-
-#   #   #   #       COMMAND LINE INTERFACE     #   #   #   #
-
-
-@click.group(
-    invoke_without_command=_autoload_graphical_user_interface,
-    context_settings=CONTEXT_SETTINGS,
-)
-@click.version_option(f"{version}", package_name=f"{name} {long_version}")
-@click.pass_context
-def main(ctx):
-    """
-    ALACORDER collects and processes case detail PDFs into data tables suitable for research purposes.
+    Collect results from Alacourt Party Search into a table at `output_path`. Input `queue_path` table from .xls(x), .csv, .json, or .parquet with columns corresponding to Alacourt Party Search fields: Name, Party Type, SSN, DOB, County, Division, Case Year, Filed Before, Filed After, No Records.
+    """ 
+    queue_path = os.path.abspath(queue_path)
+    output_path = os.path.abspath(output_path)
+    headless = not show_browser
+
+    if os.path.splitext(queue_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        raise Exception("Queue path file extension not supported. Retry with .xls, .xlsx, .csv, .json, or .parquet.")
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        raise Exception("Output path file extension not supported. Retry with .xls, .xlsx, .csv, .json, or .parquet.")
+
+    driver = AlacourtDriver(headless=headless)
+    driver.login(customer_ID, user_ID, password)
+    driver.start_party_search_queue(queue_path, output_path, criminal_only)
+
+@app.command(no_args_is_help=True)
+def fetch_cases(
+    queue_path: Annotated[Path, typer.Argument(help="Path to queue table with `CaseNumber` column.", show_default=False)],
+    output_path: Annotated[Path, typer.Argument(help="Path to output directory. PDFs will populate directory as they download.", show_default=False)],
+    customer_ID: Annotated[str, typer.Option("--customer-id", "-c", help="Customer ID for Alacourt login.", prompt="Customer ID", show_default=False)],
+    user_ID: Annotated[str, typer.Option("--user-id", "-u", help="User ID for Alacourt login.", prompt="User ID", show_default=False)],
+    password: Annotated[str, typer.Option("--password", "-p", help="Password for Alacourt login.", prompt="Password", hide_input=True, show_default=False)],
+    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False
+):
     """
-    if _autoload_graphical_user_interface and ctx.invoked_subcommand == None:
-        loadgui()
-
-
-@main.command(name="start", help="Launch graphical user interface")
-def _cli_start():
-    loadgui()
-
-
-@main.command(name="append", help="Append one case text archive to another")
-@click.option(
-    "--input-path",
-    "-in",
-    "in_path",
-    required=True,
-    prompt="Path to archive / PDF directory",
-    help="Path to input archive",
-    type=click.Path(),
-)
-@click.option(
-    "--output-path",
-    "-out",
-    "out_path",
-    required=True,
-    prompt="Path to output archive",
-    type=click.Path(),
-    help="Path to output archive",
-)
-@click.option(
-    "--no-write",
-    "-n",
-    default=False,
-    is_flag=True,
-    help="Do not export to output path",
-    hidden=True,
-)
-def _cli_append(in_path, out_path, no_write=False):
-    """Append one case text archive to another
-
-    Args:
-        in_path (Path|DataFrame): Path to input archive / PDF directory
-        out_path (Path): Path to output archive
-        no_write (bool, optional): Do not export to output path
-
-    Returns:
-        DataFrame: Appended archive
+    From a queue table with `CaseNumber` column, download case detail PDFs to directory at `output_path`.
     """
-    print("Appending archives...")
-    return append_archive(in_path, out_path)
-
-
-@main.command(name="fetch", help="Fetch cases from Alacourt.com")
-@click.option(
-    "--input-path",
-    "-in",
-    "querypath",
-    required=True,
-    prompt="Path to query table",
-    help="Path to query table/spreadsheet (.xls, .xlsx)",
-    type=click.Path(),
-)
-@click.option(
-    "--output-path",
-    "-out",
-    "path",
-    required=True,
-    prompt="PDF download path",
-    type=click.Path(),
-    help="Desired PDF output directory",
-)
-@click.option(
-    "--customer-id",
-    "-c",
-    "cID",
-    required=True,
-    prompt="Alacourt Customer ID",
-    help="Customer ID on Alacourt.com",
-)
-@click.option(
-    "--user-id",
-    "-u",
-    "uID",
-    required=True,
-    prompt="Alacourt User ID",
-    help="User ID on Alacourt.com",
-)
-@click.option(
-    "--password",
-    "-p",
-    "pwd",
-    required=True,
-    prompt="Alacourt Password",
-    help="Password on Alacourt.com",
-    hide_input=True,
-)
-@click.option(
-    "--criminal-only",
-    "-criminal",
-    is_flag=True,
-    default=False,
-    help="Only search criminal cases",
-)
-@click.option(
-    "--no-mark",
-    "-n",
-    "no_update",
-    is_flag=True,
-    default=False,
-    help="Do not update query template after completion",
-)
-@click.option(
-    "--debug",
-    is_flag=True,
-    default=False,
-    help="Print detailed runtime information to console",
-)
-def _cli_fetch(
-    querypath, path, cID, uID, pwd, no_update, criminal_only, debug
+    queue_path = os.path.abspath(queue_path)
+    output_path = os.path.abspath(output_path)
+    headless = not show_browser
+
+    if os.path.splitext(queue_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        raise Exception("Queue path file extension not supported. Retry with .xls, .xlsx, .csv, .json, or .parquet.")
+    if not os.path.isdir(output_path):
+        raise Exception("Output path must be valid directory.")
+
+    driver = AlacourtDriver(output_path, headless=headless)
+    driver.login(customer_ID, user_ID, password)
+    driver.start_case_number_queue(queue_path)
+
+@app.command(no_args_is_help=True)
+def crawl_adoc(
+    output_path: Annotated[Path, typer.Argument(help="Path to output table (.xls, .xlsx, .csv, .json, .parquet).", show_default=False)],
+    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False
 ):
     """
-    Fetch case PDFs from Alacourt.com.
-    Args:
-        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
-        path (str): Path to PDF output directory
-        cID (str): Customer ID on Alacourt.com
-        uID (str): User ID on Alacourt.com
-        pwd (str): Password on Alacourt.com
-        no_update (bool): Do not update query template after completion
-        criminal_only (bool): Only search criminal cases
-        debug (bool): Print detailed runtime information to console
+    Collect full inmates list from ADOC Inmate Search and write to table at `output_path` (.xls, .xlsx, .csv, .json, .parquet).
     """
-    fetch(
-        querypath=querypath,
-        dirpath=path,
-        cID=cID,
-        uID=uID,
-        pwd=pwd,
-        no_update=no_update,
-        criminal_only=criminal_only,
-        debug=debug,
-    )
+    output_path = os.path.abspath(output_path)
+    headless = not show_browser
 
+    driver = ADOCDriver(output_path, headless)
+    driver.crawl(output_path)
 
-@main.command(name="multi", help="Export all data tables to .xls/.xlsx")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_multi(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+@app.command(no_args_is_help=True)
+def search_adoc(
+    queue_path: Annotated[Path, typer.Argument(help="Path to queue table with \'First Name\', \'Last Name\', and \'AIS\' columns.", show_default=False)],
+    output_path: Annotated[Path, typer.Argument(help="Path to output table (.xls, .xlsx, .csv, .json, .parquet).", show_default=False)],
+    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False
 ):
     """
-    Write data tables to output path from archive or directory input.
-
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
+    Search ADOC using queue with First Name, Last Name, and AIS columns to retrieve sentencing information from ADOC. Record table to `output_path`.
     """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx"):
-        error("File extension must be .xls or .xlsx for multitable export.")
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="all",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = multi(cf)
-    return o
-
-
-@main.command(name="cases", help="Create and export case information table")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_cases(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+    queue_path = os.path.abspath(queue_path)
+    output_path = os.path.abspath(output_path)
+    headless = not show_browser
+
+    driver = ADOCDriver(output_path, headless)
+    driver.start_queue(queue_path, output_path)
+
+@app.command(no_args_is_help=True)
+def make_archive(
+    directory_path: Annotated[Path, typer.Argument(help="Path to PDF case directory.", show_default=False)],
+    output_path: Annotated[Path, typer.Argument(help="Path to output archive (recommend .parquet).", show_default=False)]
 ):
     """
-    Write `cases` table to output path from archive or directory input.
-
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
+    Create case text archive from directory of case detail PDFs.
     """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="cases",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(name="charges", help="Create and export charges table")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--filing", "-f", is_flag=True, default=False, help="Only export filing charges"
-)
-@click.option(
-    "--disposition", is_flag=True, default=False, help="Only export disposition charges"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_charges(
-    input_path,
-    output_path,
-    filing,
-    disposition,
-    count,
-    overwrite,
-    no_write,
-    no_log,
-    no_prompt,
-    debug,
-):
-    """
-    Write `cases` table to output path from archive or directory input.
+    directory_path = os.path.abspath(directory_path)
+    output_path = os.path.abspath(output_path)
 
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        filing (bool, optional): Only export filing charges
-        disposition (bool, optional): Only export disposition charges
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
-    """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    table = "charges" if not filing and not disposition else ""
-    table = "filing" if filing else table
-    table = "disposition" if disposition else table
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table=table,
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(name="fees", help="Create and export fees table")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_fees(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
-):
-    """
-    Write `cases` table to output path from archive or directory input.
+    cases = Cases(str(directory_path))
+    cases.write_archive(str(output_path))
 
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
-    """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="fees",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(name="settings", help="Create and export settings table")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_settings(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+@app.command(no_args_is_help=True)
+def make_table(
+    input_path: Annotated[Path, typer.Argument(help="Path to input case directory or archive.", show_default=False)],
+    output_path: Annotated[Path, typer.Argument(help="Path to output table (.xls, .xlsx, .csv, .json, .parquet). `All` table export must output to .xls or .xlsx.", show_default=False)],
+    table: Annotated[str, typer.Option("--table", "-t", help="Output table selection: all, cases, charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.", show_default=True)] = "all"
 ):
     """
-    Write `cases` table to output path from archive or directory input.
-
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
+    Create table at `output_path` from archive or directory at `input_path`.
     """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="settings",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(
-    name="financial-history", help="Create and export financial history table"
-)
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_finhist(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
-):
-    """
-    Write `cases` table to output path from archive or directory input.
+    input_path = os.path.abspath(input_path)
+    output_path = os.path.abspath(output_path)
 
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
-    """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="financial-history",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(name="sentences", help="Create and export sentences table")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_sentences(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
-):
-    """
-    Write `cases` table to output path from archive or directory input.
+    if table == "all" and os.path.splitext(output_path)[1] not in (".xls",".xlsx"):
+        raise Exception("Must select a table to export using --table flag. Options: cases, charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.")
 
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
-    """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="sentences",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(name="witnesses", help="Create and export witnesses table")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_witnesses(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
-):
-    """
-    Write `cases` table to output path from archive or directory input.
+    cases = Cases(str(input_path))
+    cases.read()
+
+    if table == "all":
+        output = cases.tables()
+    elif table == "cases":
+        output = cases.cases()
+    elif table == "fees":
+        output = cases.fees()
+    elif table == "charges":
+        output = cases.charges()
+    elif table == "attorneys":
+        output = cases.attorneys()
+    elif table == "case-action-summary":
+        output = cases.case_action_summary()
+    elif table == "financial-history":
+        output = cases.financial_history()
+    elif table == "images":
+        output = cases.images()
+    elif table == "sentences":
+        output = cases.sentences()
+    elif table == "settings":
+        output = cases.settings()
+    elif table == "witnesses":
+        output = cases.witnesses()
+    else:
+        raise Exception("Invalid table selection. Options: all, cases, charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.")
 
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
-    """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="witnesses",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(
-    name="case-action-summary", help="Create and export case action summaries"
-)
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_case_action_summary(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
-):
-    """
-    Write `cases` table to output path from archive or directory input.
+    write(output, output_path, log=True)
 
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
-    """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="case-action-summary",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(name="images", help="Create and export images table")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_images(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+@app.command(no_args_is_help=True)
+def make_summary(
+    input_path: Annotated[Path, typer.Argument(help="Path to input case directory or archive.", show_default=False)],
+    pairs_path: Annotated[Path, typer.Argument(help="Path to filled pairs template or party search results table.", show_default=False)],
+    output_path: Annotated[Path, typer.Argument(help="Path to output table (.xls, .xlsx, .csv, .json, .parquet).", show_default=False)]
 ):
     """
-    Write `cases` table to output path from archive or directory input.
-
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
+    Create voting rights summary grouped by person using a completed name/AIS pairing template (use make-template to create empty template). 
     """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="images",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(name="attorneys", help="Create and export attorneys table")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="Input Path",
-    show_choices=False,
-)
-@click.option(
-    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-prompt",
-    "-s",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-write", default=False, is_flag=True, help="Do not export to output path"
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print debug logs to console"
-)
-@click.version_option(
-    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
-)
-def _cli_attorneys(
-    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+    input_path = os.path.abspath(input_path)
+    pairs_path = os.path.abspath(pairs_path)
+    output_path = os.path.abspath(output_path)
+
+    cases = Cases(input_path)
+    output = cases.summary(pairs_path)
+    write({'summary': output}, output_path)
+
+@app.command(no_args_is_help=True)
+def make_template(
+    input_path: Annotated[Path, typer.Argument(help="Path to input case directory or archive.", show_default=False)],
+    output_path: Annotated[Path, typer.Argument(help="Path to output table (.xls, .xlsx, .csv, .json, .parquet). `All` table export must output to .xls or .xlsx.", show_default=False)]
 ):
     """
-    Write `cases` table to output path from archive or directory input.
-
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to table output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_log(bool): Do not print logs to console
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console
+    Create empty pairing template to be used as input for make-summary to create a voting rights summary grouped by person instead of by case.
     """
-    log = not no_log
-    if os.path.splitext(output_path)[1] not in (
-        ".xls",
-        ".xlsx",
-        ".csv",
-        ".json",
-        ".parquet",
-    ):
-        error(
-            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
-        )
-    cf = set(
-        input_path,
-        output_path,
-        count=count,
-        table="attorneys",
-        overwrite=overwrite,
-        no_write=no_write,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if cf["DEBUG"]:
-        print(cf, cf=cf)
-    o = init(cf)
-    return o
-
-
-@main.command(name="archive", help="Create full text archive from case PDFs")
-@click.option(
-    "--input-path",
-    "-in",
-    required=True,
-    type=click.Path(),
-    prompt="PDF directory or archive input",
-)
-@click.option(
-    "--output-path",
-    "-out",
-    required=True,
-    type=click.Path(),
-    prompt="Path to archive output",
-)
-@click.option(
-    "--count",
-    "-c",
-    default=0,
-    help="Total cases to pull from input",
-    show_default=False,
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--no-log",
-    default=False,
-    is_flag=True,
-    help="Do not print logs to console",
-)
-@click.option(
-    "--no-prompt",
-    default=False,
-    is_flag=True,
-    help="Skip user input / confirmation prompts",
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
-)
-@click.version_option(
-    package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
-)
-def _cli_archive(input_path, output_path, count, overwrite, no_log, no_prompt, debug):
-    """
-    Write a full text archive from a directory of case detail PDFs.
+    input_path = os.path.abspath(input_path)
+    output_path = os.path.abspath(output_path)
 
-    Args:
-        input_path (str): PDF directory or archive input
-        output_path (str): Path to archive output
-        count (int): Total cases to pull from input
-        overwrite (bool): Overwrite existing files at output path
-        no_write (bool): Do not export to output path
-        no_prompt (bool): Skip user input / confirmation prompts
-        debug (bool): Print verbose logs to console for developers
+    cases = Cases(input_path)
+    output = cases.pairs_template()
+    write({'pairs-template': output}, output_path)
+
+@app.command(no_args_is_help=True)
+def rename_cases(
+    input_directory: Annotated[Path, typer.Argument(help="Directory to rename cases within.")]
+):
     """
-    log = not no_log
-    sys.tracebacklimit = 0
-    cf = set(
-        input_path,
-        output_path,
-        archive=True,
-        count=count,
-        overwrite=overwrite,
-        no_write=False,
-        log=log,
-        no_prompt=no_prompt,
-        debug=debug,
-    )
-    if debug:
-        click.echo(cf)
-    o = archive(cf)
-    return o
-
-
-@main.command(name="rename", help="Rename cases in input directory to case numbers")
-@click.option(
-    "--input-path",
-    "-in",
-    "input_path",
-    required=True,
-    type=click.Path(),
-    prompt="PDF directory",
-)
-def _cli_rename(input_path):
-    c = cf(input_path, log=True)
-    rename_pdfs(c)
-
-
-@main.command(
-    name="pair",
-    help="Create blank AIS / unique pairing template",
-)
-@click.option(
-    "--input-path",
-    "-in",
-    "input_path",
-    required=True,
-    type=click.Path(),
-    prompt="PDF directory or archive input",
-)
-@click.option(
-    "--output-path",
-    "-out",
-    "output_path",
-    required=True,
-    type=click.Path(),
-    prompt="Path to archive output",
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
-)
-def _cli_pair(input_path, output_path, overwrite, debug):
-    conf = cf(
-        inputs=input_path,
-        outputs=output_path,
-        debug=debug,
-        overwrite=overwrite,
-        log=True,
-    )
-    p = pairs(conf)
-    print("Created pair template at output path.")
-    return p
-
-
-@main.command(
-    name="vrr-pairs", help="Create voting rights summary from input cases and pairs"
-)
-@click.option(
-    "--input-path",
-    "-in",
-    "input_path",
-    required=True,
-    type=click.Path(),
-    prompt="PDF directory or archive input",
-)
-@click.option(
-    "--pairs",
-    "-p",
-    required=True,
-    type=click.Path(),
-    prompt="Completed pairs template",
-)
-@click.option(
-    "--output-path",
-    "-out",
-    "output_path",
-    required=True,
-    type=click.Path(),
-    prompt="Path to table output",
-)
-@click.option(
-    "--overwrite",
-    "-o",
-    default=False,
-    help="Overwrite existing files at output path",
-    is_flag=True,
-    show_default=False,
-)
-@click.option(
-    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
-)
-def _cli_vrr(input_path, output_path, pairs, overwrite, debug):
-    conf = cf(
-        inputs=input_path,
-        outputs=output_path,
-        pairs=pairs,
-        vrr_summary=True,
-        debug=debug,
-        overwrite=overwrite,
-        log=True,
-    )
-    return vrr_summary(conf)
-
+    Rename all cases in a directory to full case number. Duplicates will be removed.
+    """
+    input_directory = os.path.abspath(input_directory)
+    pdfs = glob.glob(input_directory + "**/*.pdf", recursive=True)
+    with progress_bar as p:
+        for pdf in p.track(pdfs, description="Renaming PDFs..."):
+            doc = fitz.open(pdf)
+            text = " \n ".join(x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks"))
+            cnum = re.search(r'County: (\d\d)', str(text)).group(1) + "-" + re.search(r'(\w{2}\-\d{4}-\d{6}\.\d{2})', str(text)).group()
+            newpath = f"{os.path.split(pdf)[0]}/{cnum}.pdf"
+            os.rename(pdf, newpath)
+
+def version_callback(value: bool):
+    if value:
+        print(f"Alacorder {__version__}")
+        raise typer.Exit()
+
+@app.callback()
+def main(version: bool = typer.Option(None, "--version", callback=version_callback, help="Show the version and exit.")):
+    pass
 
 if __name__ == "__main__":
-    main()
-
-#   #   #   #           GETTER METHODS         #   #   #   #
-
-
-def get_paths(dirpath):
-    """
-    From path-like `dirpath`, return list of paths to pdfs in directory
-    """
-    return glob.glob(dirpath + "**/*.pdf", recursive=True)
+    app()
 
+## GETTERS
 
 def getName(text):
     try:
         return (
             re.sub(
                 r"Case Number:",
                 "",
@@ -5791,123 +3065,111 @@
             )
             .rstrip("C")
             .strip()
         )
     except:
         return ""
 
-
 def getAlias(text):
     try:
         return re.sub(
             r":", "", re.search(r"(?:SSN)(.{5,75})(?:Alias)", str(text)).group(1)
         ).strip()
     except:
         return ""
 
-
 def getDOB(text):
     try:
         return datetime.strptime(re.sub(
             r"[^\d/]",
             "",
             re.search(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", str(text)).group(1),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getPhone(text):
     try:
         text = str(text)
         text = re.sub(r"[^0-9]", "", re.search(r"(Phone: )(.+)", text).group(2)).strip()
         if len(text) < 7 or text[0:10] == "2050000000":
             return ""
         elif len(text) > 10:
             return text[0:10]
         else:
             return text
     except:
         return ""
 
-
 def getRace(text):
     try:
         return re.search(r"(B|W|H|A)/(F|M)", str(text)).group(1)
     except:
         return ""
 
-
 def getSex(text):
     try:
         return re.search(r"(B|W|H|A)/(F|M)", str(text)).group(2)
     except:
         return ""
 
-
 def getAddress1(text):
     try:
         return re.sub(
             r"Phone.+",
             "",
             re.search(r"(?:Address 1:)(.+)(?:Phone)*?", str(text)).group(1),
         ).strip()
     except:
         return ""
 
-
 def getAddress2(text):
     try:
         return re.sub(
             r"Defendant Information|JID:.+",
             "",
             re.search(r"(?:Address 2:)(.+)", str(text)).group(1).strip(),
         )
     except:
         return ""
 
-
 def getCity(text):
     try:
         return re.search(r"(?:City: )(.*)(?:State: )(.*)", str(text)).group(1)
     except:
         return ""
 
-
 def getState(text):
     try:
         return re.search(r"(?:City: )(.*)(?:State: )(.*)", str(text)).group(2)
     except:
         return ""
 
-
 def getCountry(text):
     try:
         return re.sub(
             r"Country:",
             "",
             re.sub(
                 r"(Enforcement|Party|Country)",
                 "",
                 re.search(r"Country: (\w*+)", str(text)).group(),
             ).strip(),
         )
     except:
         return ""
 
-
 def getZipCode(text):
     try:
         return re.sub(
             r"-0000$|[A-Z].+", "", re.search(r"(Zip: )(.+)", str(text)).group(2)
         ).strip()
     except:
         return ""
 
-
 def getAddress(text):
     try:
         street1 = re.sub(
             r"Phone.+",
             "",
             re.search(r"(?:Address 1:)(.+)(?:Phone)*?", str(text)).group(1),
         ).strip()
@@ -5932,1014 +3194,886 @@
     except:
         state = ""
     if len(city) > 3:
         return f"{street1} {street2} {city}, {state} {zipcode}".strip()
     else:
         return f"{street1} {street2} {city} {state} {zipcode}".strip()
 
-
 def getTotalRow(text):
     try:
         mmm = re.search(r"(Total:.+\$[^\n]*)", str(text)).group()
         mm = re.sub(r"[^0-9|\.|\s|\$]", "", str(mmm))
         m = re.findall(r"\d+\.\d{2}", str(mm))
         return m
     except:
         return ["0.00", "0.00", "0.00", "0.00"]
 
-
 def getTotalAmtDue(text):
     try:
         return float(re.sub(r"[\$\s]", "", getTotalRow(text)[0]))
     except:
         return 0.00
 
-
 def getTotalAmtPaid(text):
     try:
         return float(re.sub(r"[\$\s]", "", getTotalRow(text)[1]))
     except:
         return 0.00
 
-
 def getTotalBalance(text):
     try:
         return float(re.sub(r"[\$\s]", "", getTotalRow(text)[2]))
     except:
         return 0.00
 
-
 def getTotalAmtHold(text):
     try:
         return float(re.sub(r"[\$\s]", "", getTotalRow(text)[3]))
     except:
         return 0.00
 
-
 def getPaymentToRestore(text):
     try:
         tbal = getTotalBalance(text)
     except:
         return 0.0
     try:
         d999mm = re.search(r"(ACTIVE[^\n]+D999[^\n]+)", str(text)).group()
         d999m = re.findall(r"\$\d+\.\d{2}", str(d999mm))
         d999 = float(re.sub(r"[\$\s]", "", d999m[-1]))
     except:
         d999 = 0.0
     return float(tbal - d999)
 
-
 def getShortCaseNumber(text):
     try:
         return re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
     except:
         return ""
 
-
 def getCounty(text):
     try:
-        return re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)
+        return re.search(r"County: (\d\d)", str(text)).group(1)
     except:
         return ""
 
-
 def getCaseNumber(text):
     try:
         return (
-            re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2]
+            re.search(r"County: (\d{2})", str(text)).group(1)
             + "-"
             + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
         )
     except:
         return ""
 
-
 def getCaseYear(text):
     try:
         return int(re.search(r"\w{2}\-(\d{4})-\d{6}\.\d{2}", str(text)).group(1))
     except:
         return None
 
-
 def getLastName(text):
     try:
         return getName(text).split(" ")[0].strip()
     except:
         return ""
 
-
 def getFirstName(text):
     try:
         return getName(text).split(" ")[-1].strip()
     except:
         return ""
 
-
 def getMiddleName(text):
     try:
         if len(getName(text).split(" ")) > 2:
             return " ".join(getName(text).split(" ")[1:-2]).strip()
         else:
             return ""
     except:
         return ""
 
-
 def getRelatedCases(text):
     return re.findall(r"(\w{2}\d{12})", str(text))
 
-
 def getFilingDate(text):
     try:
         return datetime.strptime(re.sub(
             r"Filing Date: ",
             "",
             re.search(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getCaseInitiationDate(text):
     try:
-        return datetime.strptime(re.sub(
-            r"Case Initiation Date: ",
-            "",
+        return datetime.strptime(
             re.search(
                 r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)
             ).group(1),  '%m/%d/%Y')
-        )
     except:
         return None
 
-
 def getArrestDate(text):
     try:
         return datetime.strptime(re.search(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getOffenseDate(text):
     try:
         return datetime.strptime(re.search(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getIndictmentDate(text):
     try:
         return datetime.strptime(re.search(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getYouthfulDate(text):
     try:
         return datetime.strptime(re.search(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getRetrieved(text):
     try:
         return datetime.strptime(re.search(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getCourtAction(text):
     try:
         return re.search(
             r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)",
             str(text),
         ).group(1)
     except:
         return ""
 
-
 def getCourtActionDate(text):
     try:
         return datetime.strptime(re.search(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getDescription(text):
     try:
         return (
             re.search(r"Charge: ([A-Z\.0-9\-\s]+)", str(text))
             .group(1)
             .rstrip("C")
             .strip()
         )
     except:
         return ""
 
-
 def getJuryDemand(text):
     try:
         return re.search(r"Jury Demand: ([A-Z]+)", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getInpatientTreatmentOrdered(text):
     try:
         return (
             re.search(r"Inpatient Treatment Ordered: ([YES|NO]?)", str(text))
             .group(1)
             .strip()
         )
     except:
         return ""
 
-
 def getTrialType(text):
     try:
         return re.sub(
             r"[S|N]$", "", re.search(r"Trial Type: ([A-Z]+)", str(text)).group(1)
         ).strip()
     except:
         return ""
 
-
 def getJudge(text):
     try:
         return (
             re.search(r"Judge: ([A-Z\-\.\s]+)", str(text)).group(1).rstrip("T").strip()
         )
     except:
         return ""
 
-
 def getProbationOfficeNumber(text):
     try:
         return re.sub(
             r"(0-000000-00)",
             "",
             re.search(r"Probation Office \#: ([0-9\-]+)", str(text)).group(1).strip(),
         )
     except:
         return ""
 
-
 def getDefendantStatus(text):
     try:
         return (
             re.search(r"Defendant Status: ([A-Z\s]+)", str(text))
             .group(1)
             .rstrip("J")
             .strip()
         )
     except:
         return ""
 
-
-def getArrestingAgencyType(text):
-    try:
-        return re.sub(
-            r"\n",
-            "",
-            re.search(r"([^0-9]+) Arresting Agency Type:", str(text)).group(1),
-        ).strip()
-    except:
-        return ""
-
-
 def getArrestingOfficer(text):
     try:
         return (
             re.search(r"Arresting Officer: ([A-Z\s]+)", str(text))
             .group(1)
             .rstrip("S")
             .rstrip("P")
             .strip()
         )
     except:
         return ""
 
+def getArrestingAgencyType(text):
+    try:
+        out = re.search(r"([^0-9]+) Arresting Agency Type:", str(text)).group(1)
+    except:
+        return ''
+    out = re.sub(r"^\-.+", "", out)
+    out = re.sub(r"County\:", "", out)
+    out = re.sub(r"Defendant Status\:", "", out)
+    out = re.sub(r"Judge\:", "", out)
+    out = re.sub(r"Trial Type\:", "", out)
+    out = re.sub(r"Probation Office \#\:", "", out)
+    return out.strip()
 
 def getProbationOfficeName(text):
     try:
         return (
             re.search(r"Probation Office Name: ([A-Z0-9]+)", str(text)).group(1).strip()
         )
     except:
         return ""
 
-
 def getTrafficCitationNumber(text):
     try:
         return (
             re.search(r"Traffic Citation \#: ([A-Z0-9]+)", str(text)).group(1).strip()
         )
     except:
         return ""
 
-
 def getPreviousDUIConvictions(text):
     try:
         return int(
             re.search(r"Previous DUI Convictions: (\d{3})", str(text)).group(1).strip()
         )
     except:
         return ""
 
-
 def getCaseInitiationType(text):
     try:
         return (
             re.search(r"Case Initiation Type: ([A-Z\s]+)", str(text))
             .group(1)
             .rstrip("J")
             .strip()
         )
     except:
         return ""
 
-
 def getDomesticViolence(text):
     try:
         return re.search(r"Domestic Violence: ([YES|NO])", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getAgencyORI(text):
     try:
-        return (
-            re.search(r"Agency ORI: ([A-Z\s]+)", str(text)).group(1).rstrip("C").strip()
-        )
+        return re.sub(r'\s+',' ',
+            re.search(r"Agency ORI: ([A-Z\s]+)", str(text)).group(1).rstrip("C")
+        ).strip()
     except:
         return ""
 
-
 def getDriverLicenseNo(text):
     try:
         m = re.search(r"Driver License N°: ([A-Z0-9]+)", str(text)).group(1).strip()
         if m == "AL":
             return ""
         else:
             return m
     except:
         return ""
 
-
 def getSSN(text):
     try:
         return (
             re.search(r"SSN: ([X\d]{3}\-[X\d]{2}-[X\d]{4})", str(text)).group(1).strip()
         )
     except:
         return ""
 
-
 def getStateID(text):
     try:
         m = re.search(r"([A-Z0-9]{11}?) State ID:", str(text)).group(1).strip()
         if m == "AL000000000":
             return ""
         else:
             return m
     except:
         return ""
 
-
 def getWeight(text):
     try:
         return int(re.search(r"Weight: (\d+)", str(text)).group(1).strip())
     except:
         return ""
 
-
 def getHeight(text):
     try:
         return re.search(r"Height : (\d'\d{2})", str(text)).group(1).strip() + '"'
     except:
         return ""
 
-
 def getEyes(text):
     try:
         return re.search(r"Eyes/Hair: (\w{3})/(\w{3})", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getHair(text):
     try:
         return re.search(r"Eyes/Hair: (\w{3})/(\w{3})", str(text)).group(2).strip()
     except:
         return ""
 
-
-def getCountry(text):
-    try:
-        return re.sub(
-            r"(Enforcement|Party|Country:)",
-            "",
-            re.search(r"Country: (\w*+)", str(text)).group(1).strip(),
-        )
-    except:
-        return ""
-
-
 def getWarrantIssuanceDate(text):
     try:
         return datetime.strptime(
             re.search(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:", str(text))
             .group(1)
             .strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getWarrantActionDate(text):
     try:
         return datetime.strptime(
                 re.search(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1).strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getWarrantIssuanceStatus(text):
     try:
         return re.search(r"Warrant Issuance Status: (\w)", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getWarrantActionStatus(text):
     try:
         return re.search(r"Warrant Action Status: (\w)", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getWarrantLocationStatus(text):
     try:
         return re.search(r"Warrant Location Status: (\w)", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getNumberOfWarrants(text):
     try:
         return (
             re.search(r"Number Of Warrants: (\d{3}\s\d{3})", str(text)).group(1).strip()
         )
     except:
         return ""
 
-
 def getBondType(text):
     try:
         return re.search(r"Bond Type: (\w)", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getBondTypeDesc(text):
     try:
         return re.search(r"Bond Type Desc: ([A-Z\s]+)", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getBondAmt(text):
     try:
         return float(
             re.sub(
                 r"[^0-9\.\s]",
                 "",
                 re.search(r"([\d\.]+) Bond Amount:", str(text)).group(1).strip(),
             )
         )
     except:
         return ""
 
-
 def getSuretyCode(text):
     try:
         return re.search(r"Surety Code: ([A-Z0-9]{4})", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getBondReleaseDate(text):
     try:
         return datetime.strptime(
             re.search(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
             .strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getFailedToAppearDate(text):
     try:
         return datetime.strptime(
             re.search(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
             .strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getBondsmanProcessIssuance(text):
     try:
         return (
             re.search(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:",
                 str(text),
             )
             .group(1)
             .strip()
         )
     except:
         return ""
 
-
 def getBondsmanProcessReturn(text):
     try:
         return (
             re.search(r"Bondsman Process Return: (.*?) Number of Subponeas", str(text))
             .group(1)
             .strip()
         )
     except:
         return ""
 
-
 def getAppealDate(text):
     try:
         return datetime.strptime(re.sub(
             r"[\n\s]",
             "",
             re.search(r"([\n\s/\d]*?) Appeal Court:", str(text)).group(1).strip(),
         ), '%m/%d/%Y')
     except:
         return None
 
-
 def getAppealCourt(text):
     try:
         return re.search(r"([A-Z\-\s]+) Appeal Case Number", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getOriginOfAppeal(text):
     try:
         return (
             re.search(r"Orgin Of Appeal: ([A-Z\-\s]+)", str(text))
             .group(1)
             .rstrip("L")
             .strip()
         )
     except:
         return ""
 
-
 def getAppealToDesc(text):
     try:
         return (
             re.search(r"Appeal To Desc: ([A-Z\-\s]+)", str(text))
             .group(1)
             .rstrip("D")
             .rstrip("T")
             .strip()
         )
     except:
         return ""
 
-
 def getAppealStatus(text):
     try:
         return (
             re.search(r"Appeal Status: ([A-Z\-\s]+)", str(text))
             .group(1)
             .rstrip("A")
             .strip()
         )
     except:
         return ""
 
-
 def getAppealTo(text):
     try:
         return re.search(r"Appeal To: (\w?) Appeal", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getLowerCourtAppealDate(text):
     try:
         return datetime.strptime(re.sub(
             r"[\n\s:\-]",
             "",
             re.search(
                 r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)
             ).group(1),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getDispositionDateOfAppeal(text):
     try:
         return datetime.strptime(re.sub(
             r"[\n\s:\-]",
             "",
             re.search(
                 r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)", str(text)
             ).group(1),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getDispositionTypeOfAppeal(text):
     try:
         return re.sub(
             r"[\n\s:\-]",
             "",
             re.search(r"Disposition Type Of Appeal: [^A-Za-z]+", str(text)).group(1),
         ).strip()
     except:
         return ""
 
-
 def getNumberOfSubpoenas(text):
     try:
         return int(
             re.sub(
                 r"[\n\s:\-]",
                 "",
                 re.search(r"Number of Subponeas: (\d{3})", str(text)).group(1),
             ).strip()
         )
     except:
         return ""
 
-
 def getAdminUpdatedBy(text):
     try:
         return re.search(r"Updated By: (\w{3})", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getTransferToAdminDocDate(text):
     try:
         return datetime.strptime(
             re.search(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
             .strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getTransferDesc(text):
     try:
         return (
             re.search(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
             .strip()
         )
     except:
         return ""
 
-
 def getTBNV1(text):
     try:
         return datetime.strptime(
             re.search(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)", str(text))
             .group(1)
             .strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getTBNV2(text):
     try:
         return datetime.strptime(
             re.search(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)", str(text))
             .group(1)
             .strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getTurnOverDate(text):
     try:
         return datetime.strptime(re.search(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getTurnOverAmt(text):
     try:
         return float(re.search(r"TurnOver Amt\: \$(\d+\.\d\d)", str(text)).group(1))
     except:
         return ""
 
-
 def getFrequencyAmt(text):
     try:
         return float(re.search(r"Frequency Amt\: \$(\d+\.\d\d)", str(text)).group(1))
     except:
         return ""
 
-
 def getDueDate(text):
     try:
         return datetime.strptime(re.search(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getLastPaidDate(text):
     try:
         return datetime.strptime(re.search(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getPayor(text):
     try:
         return re.search(r"Payor\: ([A-Z0-9]{4})", str(text)).group(1)
     except:
         return ""
 
-
 def getEnforcementStatus(text):
     try:
         return re.sub(
             r"F$",
             "",
             re.search(r"Enforcement Status\: ([A-Z\:,\s]+)", str(text)).group(1),
         ).strip()
     except:
         return ""
 
-
 def getFrequency(text):
     try:
         return re.sub(
             r"Cost Paid By\:", "", re.search(r"Frequency\: ([W|M])", str(text)).group(1)
         )
     except:
         return ""
 
-
 def getPlacementStatus(text):
     try:
         return re.search(r"Placement Status\: (.+)", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getPreTrial(text):
     try:
         return re.search(r"PreTrial\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
-
 def getPreTrialDate(text):
     try:
         return datetime.strptime(re.search(r"PreTrail Date\: (.+)PreTrial", str(text)).group(1).strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getPreTrialTerms(text):
     try:
         return re.search(r"PreTrial Terms\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
-
 def getPreTermsDate(text):
     try:
         return datetime.strptime(re.search(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getDelinquent(text):
     try:
         return re.search(r"Delinquent\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
-
 def getDelinquentDate(text):
     try:
         return datetime.strptime(re.search(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getDAMailer(text):
     try:
         return re.search(r"DA Mailer\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
-
 def getDAMailerDate(text):
     try:
         return datetime.strptime(re.search(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getWarrantMailer(text):
     try:
         return re.search(r"Warrant Mailer\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
-
 def getWarrantMailerDate(text):
     try:
         return datetime.strptime(re.search(
             r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)
         ).group(1), '%m/%d/%Y')
     except:
         return None
 
-
 def getLastUpdate(text):
     try:
         return re.search(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
     except:
         return ""
 
-
 def getUpdatedBy(text):
     try:
         return re.search(r"Updated By\: ([A-Z]{3})", str(text)).group(1)
     except:
         return ""
 
-
 def getSentencingRequirementsCompleted(text):
     try:
         return re.sub(
             r"[\n:]|Requrements Completed",
             "",
             ", ".join(re.findall(r"(?:Requrements Completed: )([YES|NO]?)", str(text))),
         )
     except:
         return ""
 
-
 def getSentenceDate(text):
     try:
         return datetime.strptime(
             re.search(r"(Sentence Date: )(\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(2)
             .strip(), '%m/%d/%Y')
     except:
         return None 
 
-
-def getProbationPeriod(text):
-    try:
-        return "".join(
-            re.search(r"Probation Period: ([^\.]+)", str(text)).group(1).strip()
-        ).strip()
-    except:
-        return ""
-
-
-def getLicenseSuspPeriod(text):
-    try:
-        return "".join(
-            re.sub(
-                r"(License Susp Period:)",
-                "",
-                re.search(r"License Susp Period: ([^\.]+)", str(text)).group(1).strip(),
-            )
-        )
-    except:
-        return ""
-
-
 def getJailCreditPeriod(text):
     try:
         return "".join(
             re.search(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+", str(text)).group(1).strip()
         )
     except:
         return ""
 
-
 def getSentenceProvisions(text):
     try:
         return re.search(r"Sentence Provisions: ([Y|N]?)", str(text)).group(1).strip()
     except:
         return ""
 
-
 def getSentenceStartDate(text):
     try:
         return datetime.strptime(re.sub(
             r"(Sentence Start Date:)",
             "",
             ", ".join(
                 re.findall(r"Sentence Start Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getSentenceEndDate(text):
     try:
         return datetime.strptime(re.sub(
             r"(Sentence End Date:)",
             "",
             ", ".join(
                 re.findall(r"Sentence End Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
-
 def getProbationBeginDate(text):
     try:
         return datetime.strptime(re.sub(
             r"(Probation Begin Date:)",
             "",
             ", ".join(
                 re.findall(r"Probation Begin Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
         ).strip(), '%m/%d/%Y')
     except:
         return None
 
+def getProbationPeriod(text):
+    try:
+        return re.search(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)", str(text)).group(1)
+    except:
+        return ''
+
+def getLicenseSuspPeriod(text):
+    try:
+        return re.search(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)", str(text)).group(1)
+    except:
+        return ''
 
 def getProbationRevoke(text):
     try:
         return re.sub(
             r"(Probation Revoke:)",
             "",
             ", ".join(
                 re.findall(r"Probation Revoke: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
         ).strip()
     except:
         return ""
 
-
 def getAttorneys(text):
     att = re.search(
         r"(Type of Counsel Name Phone Email Attorney Code)(.+)(Warrant Issuance)",
         str(text),
         re.DOTALL,
     )
     if att:
         att = att.group(2)
         return re.sub(r"Warrant.+", "", att, re.DOTALL).strip()
     else:
         return ""
 
-
 def getCaseActionSummary(text):
     cas = re.search(
         r"(Case Action Summary)([^\\]*)(Images\s+?Pages)", str(text), re.DOTALL
     )
     if cas:
         cas = cas.group(2)
         return re.sub(
             r"© Alacourt\.com|Date: Description Doc# Title|Operator", "", cas, re.DOTALL
         ).strip()
     else:
         return ""
 
-
 def getImages(text):
     imgs = re.findall(
         r"(Images\s+?Pages)([^\\n]*)(END OF THE REPORT)", str(text), re.DOTALL
     )
     if len(imgs) > 1:
         imgs = "; ".join(imgs).strip()
     elif len(imgs) == 1:
         return imgs[0][1].strip()
     else:
         return ""
 
-
 def getWitnesses(text):
     wit = re.search(r"(Witness.+?Case Action Summary)", str(text), re.DOTALL)
     if wit:
         wit = wit.group()
         wit = re.sub(r"© Alacourt.com \d\d?/\d\d?/\d\d\d\d", "", wit, re.DOTALL)
         wit = re.sub(r"Witness", "", wit, re.DOTALL)
         wit = re.sub(r"\#Name", "", wit, re.DOTALL)
@@ -6956,20 +4090,19 @@
         wit = re.sub(r"Date Issued", "", wit, re.DOTALL)
         wit = re.sub(r"Subpoena", "", wit, re.DOTALL)
         wit = re.sub(r"Date\:", "", wit, re.DOTALL)
         wit = re.sub(r"Time", "", wit, re.DOTALL)
         wit = re.sub(r"Code", "", wit, re.DOTALL)
         wit = re.sub(r"Comments", "", wit, re.DOTALL)
         wit = re.sub(r"Case Action Summary", "", wit, re.DOTALL)
-        wit = re.sub(r"\:$", "", wit, re.DOTALL)
+        wit = re.sub(r"\:$", "", wit.strip(), re.DOTALL)
         return wit.strip()
     else:
         return ""
 
-
 def getSettings(text):
     settings = re.search(r"(Settings.+?Court Action)", str(text), re.DOTALL)
     if settings:
         out = settings.group(1)
         out = re.sub(r"Settings", "", out, re.DOTALL)
         out = re.sub(r"Date\:", "", out, re.DOTALL)
         out = re.sub(r"Que\:", "", out, re.DOTALL)
@@ -7031,7 +4164,8 @@
         if len(splr) > 0:
             bal = float(re.sub(r'\$','',splr[2]))
             tot += bal
     if len(rows) == 0:
         return None
     if len(rows) > 0:
         return tot
+
```

