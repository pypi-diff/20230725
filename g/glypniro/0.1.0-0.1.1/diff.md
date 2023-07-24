# Comparing `tmp/glypniro-0.1.0.tar.gz` & `tmp/glypniro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glypniro-0.1.0.tar", max compression
+gzip compressed data, was "glypniro-0.1.1.tar", max compression
```

## Comparing `glypniro-0.1.0.tar` & `glypniro-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.0/glypniro/__init__.py
--rw-r--r--   0        0        0    14001 2023-07-21 20:06:56.672928 glypniro-0.1.0/glypniro/cli.py
--rw-r--r--   0        0        0    49474 2023-07-21 19:37:02.551163 glypniro-0.1.0/glypniro/common.py
--rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.0/glypniro/reformat.py
--rw-r--r--   0        0        0     2597 2023-07-21 20:17:32.217490 glypniro-0.1.0/glypniro/reformat_skyline.py
--rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.0/LICENSE
--rw-r--r--   0        0        0      672 2023-07-21 20:24:09.657923 glypniro-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.0/README.md
--rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.1/glypniro/__init__.py
+-rw-r--r--   0        0        0    14001 2023-07-21 20:06:56.672928 glypniro-0.1.1/glypniro/cli.py
+-rw-r--r--   0        0        0    49477 2023-07-24 23:51:40.093127 glypniro-0.1.1/glypniro/common.py
+-rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.1/glypniro/reformat.py
+-rw-r--r--   0        0        0     2599 2023-07-22 07:18:03.874051 glypniro-0.1.1/glypniro/reformat_skyline.py
+-rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.1/LICENSE
+-rw-r--r--   0        0        0      672 2023-07-24 23:51:48.273671 glypniro-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.1/README.md
+-rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.1/PKG-INFO
```

### Comparing `glypniro-0.1.0/glypniro/cli.py` & `glypniro-0.1.1/glypniro/cli.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.0/glypniro/common.py` & `glypniro-0.1.1/glypniro/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,15 +676,15 @@
                 if r["area_filename"].endswith("xlsx"):
                     file_with_area = pd.read_excel(r["area_filename"])
                 else:
                     file_with_area = pd.read_csv(r["area_filename"], sep="\t")
 
                 for index, g in data.groupby([protein_id_column]):
 
-                    u = index
+                    u = index[0]
                     if not u.startswith(">Reverse") and not u.endswith("(Common contaminant protein)"):
                         # merging of byonic and pd data for appropriate protein
                         comp = GlypnirOComponent(g, file_with_area, r["replicate_id"],
                                                  condition_id=r["condition_id"], protein_name=u,
                                                  minimum_score=minimum_score, trust_byonic=self.trust_byonic, legacy=legacy)
                         if not comp.empty:
```

### Comparing `glypniro-0.1.0/glypniro/reformat.py` & `glypniro-0.1.1/glypniro/reformat.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.0/glypniro/reformat_skyline.py` & `glypniro-0.1.1/glypniro/reformat_skyline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 import pandas as pd
 import pathlib
 import click
 
 glycan_column = "Glycans\nNHFAGNa"
 peptide_column = "Peptide\n< ProteinMetrics Confidential >"
-scan_number_regex = re.compile("id=(\d+)")
-replicate_regex = re.compile("(\w+)(\d+)$")
+scan_number_regex = re.compile(r"id=(\d+)")
+replicate_regex = re.compile(r"(\w+)(\d+)$")
 
 
 @click.command()
 @click.option("-b", "-byonic", type=click.Path(exists=True), help="Filepath to Byonic output xlsx file.")
 @click.option("-s", "-skyline", type=click.Path(exists=True), help="Filepath to Skyline peptide output in xlsx format")
 @click.option("-o", "-output", type=click.Path(exists=False), help="Filepath to output folder")
 def main(b, s, o):
```

### Comparing `glypniro-0.1.0/LICENSE` & `glypniro-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.0/pyproject.toml` & `glypniro-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glypniro"
-version = "0.1.0"
+version = "0.1.1"
 description = "A automated script for processing and combining Byonic and PD standard output."
 authors = ["Toan Phung <toan.phungkhoiquoctoan@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 scipy = "^1.11.1"
```

### Comparing `glypniro-0.1.0/README.md` & `glypniro-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.0/PKG-INFO` & `glypniro-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glypniro
-Version: 0.1.0
+Version: 0.1.1
 Summary: A automated script for processing and combining Byonic and PD standard output.
 Author: Toan Phung
 Author-email: toan.phungkhoiquoctoan@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

