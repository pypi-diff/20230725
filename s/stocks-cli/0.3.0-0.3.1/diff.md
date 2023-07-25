# Comparing `tmp/stocks-cli-0.3.0.tar.gz` & `tmp/stocks-cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stocks-cli-0.3.0.tar", last modified: Tue Jul 25 14:11:56 2023, max compression
+gzip compressed data, was "stocks-cli-0.3.1.tar", last modified: Tue Jul 25 14:32:26 2023, max compression
```

## Comparing `stocks-cli-0.3.0.tar` & `stocks-cli-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.714431 stocks-cli-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-25 14:11:56.714431 stocks-cli-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4988 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.712431 stocks-cli-0.3.0/cli/
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     8914 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    60509 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/export.py
--rw-rw-rw-   0 root         (0) root         (0)     8634 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/export_eln_website_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    64936 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/export_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12896 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/fetch.py
--rw-rw-rw-   0 root         (0) root         (0)    37310 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/register.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/stockscli.ini
--rw-rw-rw-   0 root         (0) root         (0)     7311 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4729 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/cli/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     2529 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/pypi_description.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 14:11:56.714431 stocks-cli-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.712431 stocks-cli-0.3.0/stocks/
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.713431 stocks-cli-0.3.0/stocks/assaysniffer/
--rw-rw-rw-   0 root         (0) root         (0)     4129 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/assaysniffer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3624 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/assaysniffer/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    40236 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/assaysniffer/sniffers.py
--rw-rw-rw-   0 root         (0) root         (0)    30518 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocks/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.713431 stocks-cli-0.3.0/stocks_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      695 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 14:11:56.000000 stocks-cli-0.3.0/stocks_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:11:56.714431 stocks-cli-0.3.0/stocksapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10865 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2607 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    81438 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    28467 2023-07-25 14:11:48.000000 stocks-cli-0.3.0/stocksapi/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:32:26.896939 stocks-cli-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-25 14:32:26.896939 stocks-cli-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4988 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:32:26.894939 stocks-cli-0.3.1/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8914 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    60509 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     8634 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/export_eln_website_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    64936 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/export_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12896 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)    37310 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/register.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/stockscli.ini
+-rw-rw-rw-   0 root         (0) root         (0)     7311 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4729 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/cli/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/pypi_description.md
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 14:32:26.896939 stocks-cli-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:32:26.894939 stocks-cli-0.3.1/stocks/
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:32:26.894939 stocks-cli-0.3.1/stocks/assaysniffer/
+-rw-rw-rw-   0 root         (0) root         (0)     4129 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocks/assaysniffer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3624 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocks/assaysniffer/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    40236 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocks/assaysniffer/sniffers.py
+-rw-rw-rw-   0 root         (0) root         (0)    30518 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocks/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:32:26.895939 stocks-cli-0.3.1/stocks_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-25 14:32:26.000000 stocks-cli-0.3.1/stocks_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 14:32:26.000000 stocks-cli-0.3.1/stocks_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:32:26.000000 stocks-cli-0.3.1/stocks_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-25 14:32:26.000000 stocks-cli-0.3.1/stocks_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-25 14:32:26.000000 stocks-cli-0.3.1/stocks_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 14:32:26.000000 stocks-cli-0.3.1/stocks_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:32:26.895939 stocks-cli-0.3.1/stocksapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocksapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10865 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocksapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocksapi/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    81438 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocksapi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    28467 2023-07-25 14:32:19.000000 stocks-cli-0.3.1/stocksapi/models.py
```

### Comparing `stocks-cli-0.3.0/LICENSE.txt` & `stocks-cli-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/PKG-INFO` & `stocks-cli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocks-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: Command Line Interface to the STOCKS server
 Home-page: https://www.embl.org/research/units/genome-biology/genome-biology-computational-support/
 Author: GBCS
 Author-email: gbcs@embl.de
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `stocks-cli-0.3.0/README.md` & `stocks-cli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/__init__.py` & `stocks-cli-0.3.1/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/__main__.py` & `stocks-cli-0.3.1/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/config.py` & `stocks-cli-0.3.1/cli/config.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/export.py` & `stocks-cli-0.3.1/cli/export.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/export_eln_website_utils.py` & `stocks-cli-0.3.1/cli/export_eln_website_utils.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/export_utils.py` & `stocks-cli-0.3.1/cli/export_utils.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/fetch.py` & `stocks-cli-0.3.1/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/register.py` & `stocks-cli-0.3.1/cli/register.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/utils.py` & `stocks-cli-0.3.1/cli/utils.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/cli/validate.py` & `stocks-cli-0.3.1/cli/validate.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/pypi_description.md` & `stocks-cli-0.3.1/pypi_description.md`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/setup.py` & `stocks-cli-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="stocks-cli",
-    version="0.3.0",
+    version="0.3.1",
     author="GBCS",
     author_email="gbcs@embl.de",
     packages=["cli", "stocks", "stocks.assaysniffer", "stocksapi"],
     data_files=[('cli', ['cli/stockscli.ini'])],
     include_package_data=True,
     install_requires=requirements,
     extras_require={
```

### Comparing `stocks-cli-0.3.0/stocks/__init__.py` & `stocks-cli-0.3.1/stocks/__init__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/stocks/assaysniffer/__init__.py` & `stocks-cli-0.3.1/stocks/assaysniffer/__init__.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/stocks/assaysniffer/registry.py` & `stocks-cli-0.3.1/stocks/assaysniffer/registry.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/stocks/assaysniffer/sniffers.py` & `stocks-cli-0.3.1/stocks/assaysniffer/sniffers.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/stocks/models.py` & `stocks-cli-0.3.1/stocks/models.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/stocks_cli.egg-info/PKG-INFO` & `stocks-cli-0.3.1/stocks_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stocks-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: Command Line Interface to the STOCKS server
 Home-page: https://www.embl.org/research/units/genome-biology/genome-biology-computational-support/
 Author: GBCS
 Author-email: gbcs@embl.de
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `stocks-cli-0.3.0/stocks_cli.egg-info/SOURCES.txt` & `stocks-cli-0.3.1/stocks_cli.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pypi_description.md
+requirements.txt
 setup.py
 cli/__init__.py
 cli/__main__.py
 cli/config.py
 cli/export.py
 cli/export_eln_website_utils.py
 cli/export_utils.py
```

### Comparing `stocks-cli-0.3.0/stocksapi/client.py` & `stocks-cli-0.3.1/stocksapi/client.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/stocksapi/exceptions.py` & `stocks-cli-0.3.1/stocksapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/stocksapi/manager.py` & `stocks-cli-0.3.1/stocksapi/manager.py`

 * *Files identical despite different names*

### Comparing `stocks-cli-0.3.0/stocksapi/models.py` & `stocks-cli-0.3.1/stocksapi/models.py`

 * *Files identical despite different names*

