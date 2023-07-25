# Comparing `tmp/kohlrahbi-0.0.7.tar.gz` & `tmp/kohlrahbi-0.0.8.tar.gz`

## Comparing `kohlrahbi-0.0.7.tar` & `kohlrahbi-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/README.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/requirements.in
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/requirements.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.github/workflows/black.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/ahbfilefinder.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/all_known_pruefis.toml
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/collect_pruefis.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/ahb/ahbsubtable.py
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/ahb/ahbtable.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/ahb/ahbtablerow.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/temp/test-fobar.docx
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/LICENSE
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 kohlrahbi-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/README.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/requirements.in
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/requirements.txt
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/black.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0     9052 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahbfilefinder.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/all_known_pruefis.toml
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/collect_pruefis.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbsubtable.py
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbtable.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbtablerow.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/temp/test-fobar.docx
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/PKG-INFO
```

### Comparing `kohlrahbi-0.0.7/.pre-commit-config.yaml` & `kohlrahbi-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/README.md` & `kohlrahbi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/requirements.txt` & `kohlrahbi-0.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/tox.ini` & `kohlrahbi-0.0.8/tox.ini`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/.github/dependabot.yml` & `kohlrahbi-0.0.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/.github/workflows/black.yml` & `kohlrahbi-0.0.8/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/.github/workflows/coverage.yml` & `kohlrahbi-0.0.8/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/.github/workflows/packaging_test.yml` & `kohlrahbi-0.0.8/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/.github/workflows/python-publish.yml` & `kohlrahbi-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/.github/workflows/pythonlint.yml` & `kohlrahbi-0.0.8/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/.github/workflows/unittests.yml` & `kohlrahbi-0.0.8/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/__init__.py` & `kohlrahbi-0.0.8/src/kohlrahbi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 """
 kohlrahbi is a package to scrape AHBs (in docx format)
 """
+import fnmatch
 import gc
 import re
 import sys
 from pathlib import Path
-from typing import Any
+from typing import Any, Optional
 
 import click
 import docx  # type:ignore[import]
 import tomlkit
 
 from kohlrahbi.ahb.ahbtable import AhbTable
 from kohlrahbi.ahbfilefinder import AhbFileFinder
 from kohlrahbi.logger import logger
 from kohlrahbi.read_functions import get_ahb_table
 from kohlrahbi.unfoldedahb.unfoldedahbtable import UnfoldedAhb
 
 _pruefi_pattern = re.compile(r"^[1-9]\d{4}$")
 
 
-def get_valid_pruefis(list_of_pruefis: list[str]) -> list[str]:
+# pylint:disable=anomalous-backslash-in-string
+def get_valid_pruefis(list_of_pruefis: list[str], all_known_pruefis: Optional[list[str]] = None) -> list[str]:
     """
-    This function returns a new list with only those pruefis which match the pruefi_pattern.
-    """
-    valid_pruefis: list[str] = [pruefi for pruefi in list_of_pruefis if _pruefi_pattern.match(pruefi)]
-    return valid_pruefis
+    This function returns a new list with only those pruefis which match the pruefi_pattern r"^[1-9]\d{4}$".
+    It also supports unix wildcards like '*' and '?' iff a list of known pruefis is given.
+    E.g. '11*' for all pruefis starting with '11' or '*01' for all pruefis ending with '01'.
+    """
+    result: set[str] = set()
+
+    for pruefi in list_of_pruefis:
+        if ("*" in pruefi or "?" in pruefi) and all_known_pruefis:
+            filtered_pruefis = fnmatch.filter(all_known_pruefis, pruefi)
+            result = result.union(filtered_pruefis)
+        elif _pruefi_pattern.match(pruefi):
+            result.add(pruefi)
+
+    return sorted(list(result))
 
 
 def check_python_version():
     """
     Check if the Python interpreter is greater or equal to 3.11
     """
     if sys.version_info.major != 3 or sys.version_info.minor < 11:
@@ -91,15 +103,15 @@
 
 @click.command()
 @click.option(
     "-p",
     "--pruefis",
     default=[],
     required=False,
-    help="Five digit number like 11042.",
+    help="Five digit number like 11042 or use wildcards like 110* or *042 or 11?42.",
     multiple=True,
 )
 @click.option(
     "-i",
     "--input_path",
     type=click.Path(exists=True, dir_okay=True, file_okay=False, path_type=Path),
     prompt="Input directory",
```

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/all_known_pruefis.toml` & `kohlrahbi-0.0.8/src/kohlrahbi/all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/collect_pruefis.py` & `kohlrahbi-0.0.8/src/kohlrahbi/collect_pruefis.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/read_functions.py` & `kohlrahbi-0.0.8/src/kohlrahbi/read_functions.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-0.0.8/src/kohlrahbi/row_type_checker.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/seed.py` & `kohlrahbi-0.0.8/src/kohlrahbi/seed.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/ahb/ahbsubtable.py` & `kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbsubtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/ahb/ahbtable.py` & `kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/ahb/ahbtablerow.py` & `kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbtablerow.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-0.0.8/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/temp/test-fobar.docx` & `kohlrahbi-0.0.8/temp/test-fobar.docx`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/.gitignore` & `kohlrahbi-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/LICENSE` & `kohlrahbi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/pyproject.toml` & `kohlrahbi-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.7/PKG-INFO` & `kohlrahbi-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kohlrahbi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
```

