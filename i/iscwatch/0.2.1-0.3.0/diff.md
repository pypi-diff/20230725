# Comparing `tmp/iscwatch-0.2.1.tar.gz` & `tmp/iscwatch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iscwatch-0.2.1.tar", max compression
+gzip compressed data, was "iscwatch-0.3.0.tar", max compression
```

## Comparing `iscwatch-0.2.1.tar` & `iscwatch-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rwxr-xr-x   0        0        0     2300 2023-07-20 04:46:21.223136 iscwatch-0.2.1/README.md
--rwxr-xr-x   0        0        0      573 2023-07-20 04:53:06.335102 iscwatch-0.2.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-15 22:53:30.000000 iscwatch-0.2.1/src/iscwatch/__init__.py
--rw-r--r--   0        0        0      265 2023-07-19 22:54:31.754068 iscwatch-0.2.1/src/iscwatch/advisory.py
--rwxr-xr-x   0        0        0     1591 2023-07-20 02:59:25.585631 iscwatch-0.2.1/src/iscwatch/main.py
--rw-r--r--   0        0        0     2805 2023-07-19 22:54:28.494701 iscwatch-0.2.1/src/iscwatch/scrape.py
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 iscwatch-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     2571 2023-07-25 19:10:32.240679 iscwatch-0.3.0/README.md
+-rwxr-xr-x   0        0        0      573 2023-07-25 19:10:32.241345 iscwatch-0.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-06-15 22:53:30.000000 iscwatch-0.3.0/src/iscwatch/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-25 18:36:36.175858 iscwatch-0.3.0/src/iscwatch/advisory.py
+-rw-r--r--   0        0        0      519 2023-07-25 19:10:32.241567 iscwatch-0.3.0/src/iscwatch/logconfig.py
+-rwxr-xr-x   0        0        0     2074 2023-07-25 19:10:32.241861 iscwatch-0.3.0/src/iscwatch/main.py
+-rw-r--r--   0        0        0     3590 2023-07-25 19:10:32.242036 iscwatch-0.3.0/src/iscwatch/scrape.py
+-rw-r--r--   0        0        0     3038 1970-01-01 00:00:00.000000 iscwatch-0.3.0/PKG-INFO
```

### Comparing `iscwatch-0.2.1/README.md` & `iscwatch-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# iscwatch - A Tool for Monitoring Intel Security Center Product Advisories
+# iscwatch - A Command Line Application For Monitoring Intel Security Center Product Advisories
 
-![Version](https://img.shields.io/badge/version-0.2.1-blue.svg)
+![Version](https://img.shields.io/badge/version-0.3.0-blue.svg)
 ![License](https://img.shields.io/badge/license-MIT-green.svg)
 
 ## Description
 
-`iscwatch` is a command line application providing summaries of Intel's Security Center Product Advisories in CSV format. Included in the output per advisory is its title, full text url, advisory ID, updated date, and released date.
+`iscwatch` is a command line application that searches for summaries of [Intel's Security Center Product Advisories](https://www.intel.com/content/www/us/en/security-center/default.html) and outputs those summaries in CSV format. Included in the output per advisory is its title, full text url, advisory ID, updated date, and released date.
 
 ## Features
 
 - Fetches summaries of Intel's Security Center Product Advisories.
 - Outputs advisory data in CSV format to stdout.
-- Allows filtering advisories based on updated or released date using the --since option.
+- Optionally filters advisories based on date using the --since option.
 - Enables or disables CSV column headers with --headers and --no-headers options, respectively.
 
 ## Installation
 
 You can install `iscwatch` using pip:
 
 ```
@@ -48,23 +48,25 @@
 
 - Advisory Title
 - Advisory Page Link
 - Advisory ID
 - Updated Date
 - Released Date
 
+```bash
+> iscwatch --since 2023-07-01 --no-headers
+2023.2 IPU – BIOS Advisory,https://www.intel.com/content/www/us/en/security-center/advisory/intel-sa-00807.html,INTEL-SA-00807,2023-07-07,2023-05-09
+Intel® NUC Laptop Kit Advisory,https://www.intel.com/content/www/us/en/security-center/advisory/intel-sa-00712.html,INTEL-SA-00712,2023-07-07,2022-08-09
+```
+
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to create an issue or submit a pull request.
 
 ## Acknowledgments
 
 - This application relies on Intel's Security Center for fetching advisories data.
-
----
-
-*Note: This is a sample README.md file for the `iscwatch` command line application. Please modify and update the content according to the actual implementation and features of the application.*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iscwatch-0.2.1/pyproject.toml` & `iscwatch-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iscwatch"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["Roger Hurwitz <rogerhurwitz@inspirsmith.com>"]
 readme = "README.md"
 packages = [{include = "iscwatch", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `iscwatch-0.2.1/src/iscwatch/main.py` & `iscwatch-0.3.0/src/iscwatch/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 import csv
 import datetime
+import logging
+import logging.config
 import sys
 from dataclasses import asdict, fields
-from typing import Annotated, Union
+from typing import Annotated, Final
 
 import pkg_resources
 import typer
 
 from iscwatch.advisory import Advisory
+from iscwatch.logconfig import logging_config
 from iscwatch.scrape import iter_advisories
 
+logging.config.dictConfig(logging_config)
+
+PACKAGE_NAME: Final = "iscwatch"
+
 
 def cli():
     """CLI entry point executes typer-wrapped main function"""
     typer.run(main)
 
+
 def main(
     since: Annotated[
-        Union[datetime.datetime, None],
+        datetime.datetime,
         typer.Option(
             help="Output only those summaries released or updated since specified date."
         ),
-    ] = None,
-    version: Annotated[
-        bool,
-        typer.Option(help="Output product version and exit.")
-    ] = False,
+    ] = datetime.datetime.min,
+    version: Annotated[bool, typer.Option(help="Output product version and exit.")] = False,
     headers: Annotated[
-        bool,
-        typer.Option(help="Include column headers in CSV output.")
-    ] = True
+        bool, typer.Option(help="Include column headers in CSV output.")
+    ] = True,
 ):
-    """Retrieve Security Advisory summaries from Intel website and output as CSV."""
+    """Disposition command line and vector work to appropriate sub-function."""
     if version:
-        output_version()
+        print_version()
     else:
-        output_advisories(since, headers)
+        if since:
+            selected_advisories = [a for a in iter_advisories() if a.updated >= since.date()]
+        else:
+            selected_advisories = list(iter_advisories())
+        print_csv_advisories(selected_advisories, headers)
 
-def output_advisories(since: datetime.datetime | None, headers: bool):
+
+def print_csv_advisories(advisories: list[Advisory], use_headers: bool):
+    """Convert advisories into dictionaries and output in CSV format."""
     fieldnames = [field.name for field in fields(Advisory)]
     writer = csv.DictWriter(sys.stdout, fieldnames=fieldnames)
-    if headers:
+    if use_headers:
         writer.writeheader()
-    select_advisories = [
-        asdict(advisory)
-        for advisory in iter_advisories()
-        if not since or advisory.updated >= since.date()
-    ]
-    writer.writerows(select_advisories)
-
-def output_version():
-    distribution = pkg_resources.get_distribution("iscwatch")
-    print(f"{distribution.project_name} {distribution.version}")
+    writer.writerows(asdict(advisory) for advisory in advisories)
+
+
+def print_version():
+    """Output current version of the application."""
+    try:
+        distribution = pkg_resources.get_distribution(PACKAGE_NAME)
+        print(f"{distribution.project_name} {distribution.version}")
+    except pkg_resources.DistributionNotFound:
+        logging.error(f"The package ({PACKAGE_NAME}) is not installed.")
```

### Comparing `iscwatch-0.2.1/src/iscwatch/scrape.py` & `iscwatch-0.3.0/src/iscwatch/scrape.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,31 @@
+"""Implements the web scraper logic of the library.
+
+Advisories (really Advisor summaries) are listed on the home page of the Intel Security Center
+inside of an HTML table. The code in this module is responsible for retrieving the contents of
+that table then parsing the data to allow iteration over Advisory objects.
+
+"""
 import datetime
+import logging
 import re
 import unicodedata
 from typing import Final, Iterator
 
 import bs4
 import requests
 from bs4 import Tag
 
 from iscwatch.advisory import Advisory
 
 INTEL_HOME_PAGE: Final = "https://www.intel.com"
 INTEL_PAGE_NOT_FOUND: Final = "https://www.intel.com/content/www/us/en/404.html"
 ISC_HOME_PAGE: Final = "https://www.intel.com/content/www/us/en/security-center/default.html"
 
+logger = logging.getLogger(__name__)
 
 def iter_advisories() -> Iterator[Advisory]:
     """Iterate over all Intel Security Center product advisories"""
     if result := requests.get(ISC_HOME_PAGE):
         for row_data in iter_advisory_table_row_data(result.text):
             yield Advisory(
                 title=text_from_tag(row_data[0]),
@@ -24,35 +33,43 @@
                 id=text_from_tag(row_data[1]),
                 updated=date_from_tag(row_data[2]),
                 released=date_from_tag(row_data[3]),
             )
 
 
 def text_from_tag(tag: Tag):
-    """Extract text from tag and remove unicode special characters."""
-    return strip_unicode(tag.text)
+    """Extract text from tag and remove unicode special characters and whitespace."""
+    return strip_unicode(tag.text).strip()
 
 
 def link_from_tag(tag: Tag) -> str:
     """Convert relative path HREF from anchor tag into absolute path page link."""
     if (anchor := tag.find("a")) and isinstance(anchor, Tag):
         return f"{INTEL_HOME_PAGE}{anchor['href']}"
     return INTEL_PAGE_NOT_FOUND
 
 
 def date_from_tag(tag: Tag) -> datetime.date:
-    """Convert advisory table date format to datetime.date."""
+    """Convert advisory table date format to datetime.datetime.
+    
+    The regular expression pattern in this function was arrived through trial and error.
+    Unfortunately, the way that dates are entered in the HTML table cells is not completely
+    consistent (e.g, "Jan" in some cases, "January" in others).  The &nbsp versus a "real"
+    space was particularly challenging.
+    
+    """
     date_pattern = (
         r"(?P<month>(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec))\w*"
         r"(\s|&nbsp;)(?P<day>0?[1-9]|[12][0-9]|3[01]), (?P<year>[0-9]{4})"
     )
     if m := re.search(date_pattern, tag.text):
         return datetime.datetime.strptime(
             f"{m['month']} {m['day']}, {m['year']}", "%b %d, %Y"
         ).date()
+    logger.warning(f"Unable to parse date: {tag.text}")
     return datetime.datetime.min.date()
 
 
 def strip_unicode(text: str):
     """Magic internet code that removes special characters from unicode strings."""
     return "".join(
         char for char in unicodedata.normalize("NFKD", text) if not unicodedata.combining(char)
```

### Comparing `iscwatch-0.2.1/PKG-INFO` & `iscwatch-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: iscwatch
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: Roger Hurwitz
 Author-email: rogerhurwitz@inspirsmith.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-# iscwatch - A Tool for Monitoring Intel Security Center Product Advisories
+# iscwatch - A Command Line Application For Monitoring Intel Security Center Product Advisories
 
-![Version](https://img.shields.io/badge/version-0.2.1-blue.svg)
+![Version](https://img.shields.io/badge/version-0.3.0-blue.svg)
 ![License](https://img.shields.io/badge/license-MIT-green.svg)
 
 ## Description
 
-`iscwatch` is a command line application providing summaries of Intel's Security Center Product Advisories in CSV format. Included in the output per advisory is its title, full text url, advisory ID, updated date, and released date.
+`iscwatch` is a command line application that searches for summaries of [Intel's Security Center Product Advisories](https://www.intel.com/content/www/us/en/security-center/default.html) and outputs those summaries in CSV format. Included in the output per advisory is its title, full text url, advisory ID, updated date, and released date.
 
 ## Features
 
 - Fetches summaries of Intel's Security Center Product Advisories.
 - Outputs advisory data in CSV format to stdout.
-- Allows filtering advisories based on updated or released date using the --since option.
+- Optionally filters advisories based on date using the --since option.
 - Enables or disables CSV column headers with --headers and --no-headers options, respectively.
 
 ## Installation
 
 You can install `iscwatch` using pip:
 
 ```
@@ -63,24 +63,26 @@
 
 - Advisory Title
 - Advisory Page Link
 - Advisory ID
 - Updated Date
 - Released Date
 
+```bash
+> iscwatch --since 2023-07-01 --no-headers
+2023.2 IPU – BIOS Advisory,https://www.intel.com/content/www/us/en/security-center/advisory/intel-sa-00807.html,INTEL-SA-00807,2023-07-07,2023-05-09
+Intel® NUC Laptop Kit Advisory,https://www.intel.com/content/www/us/en/security-center/advisory/intel-sa-00712.html,INTEL-SA-00712,2023-07-07,2022-08-09
+```
+
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to create an issue or submit a pull request.
 
 ## Acknowledgments
 
 - This application relies on Intel's Security Center for fetching advisories data.
 
----
-
-*Note: This is a sample README.md file for the `iscwatch` command line application. Please modify and update the content according to the actual implementation and features of the application.*
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

