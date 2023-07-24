# Comparing `tmp/wikiscrape-0.2.1.tar.gz` & `tmp/wikiscrape-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikiscrape-0.2.1.tar", max compression
+gzip compressed data, was "wikiscrape-0.2.2.tar", max compression
```

## Comparing `wikiscrape-0.2.1.tar` & `wikiscrape-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      661 2023-05-20 15:53:34.608059 wikiscrape-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       58 2023-05-19 22:15:26.142574 wikiscrape-0.2.1/README.md
--rw-r--r--   0        0        0      102 2023-05-19 22:41:43.658345 wikiscrape-0.2.1/wikiscrape/__init__.py
--rw-r--r--   0        0        0      772 2023-05-19 22:41:43.658345 wikiscrape-0.2.1/wikiscrape/markdown.py
--rw-r--r--   0        0        0     1132 2023-05-20 15:41:09.549133 wikiscrape-0.2.1/wikiscrape/wikipage.py
--rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 wikiscrape-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      737 2023-07-24 22:53:55.141745 wikiscrape-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-05-19 22:15:26.142574 wikiscrape-0.2.2/README.md
+-rw-r--r--   0        0        0      102 2023-05-19 22:41:43.658345 wikiscrape-0.2.2/wikiscrape/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-19 22:41:43.658345 wikiscrape-0.2.2/wikiscrape/markdown.py
+-rw-r--r--   0        0        0     1132 2023-05-20 15:56:10.716816 wikiscrape-0.2.2/wikiscrape/wikipage.py
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 wikiscrape-0.2.2/PKG-INFO
```

### Comparing `wikiscrape-0.2.1/pyproject.toml` & `wikiscrape-0.2.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wikiscrape"
-version = "0.2.1"
+version = "0.2.2"
 description = "A tool for scraping info from Wikipedia"
 authors = ["peaky76 <robertjamespeacock@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -14,15 +14,17 @@
 [tool.poetry.group.dev.dependencies]
 auto-changelog = "^0.6.0"
 black = "^23.3.0"
 coverage = "^7.2.5"
 mypy = "^1.3.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.269"
+requests-mock = "^1.10.0"
+ruff = ">=0.0.269,<0.0.281"
 sphinx = "^6.2.1"
 sphinx-rtd-theme = "^1.2.0"
-requests-mock = "^1.10.0"
+types-requests = "^2.31.0.2"
+types-beautifulsoup4 = "^4.12.0.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wikiscrape-0.2.1/wikiscrape/markdown.py` & `wikiscrape-0.2.2/wikiscrape/markdown.py`

 * *Files identical despite different names*

### Comparing `wikiscrape-0.2.1/wikiscrape/wikipage.py` & `wikiscrape-0.2.2/wikiscrape/wikipage.py`

 * *Files identical despite different names*

### Comparing `wikiscrape-0.2.1/PKG-INFO` & `wikiscrape-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikiscrape
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool for scraping info from Wikipedia
 License: GPL-3.0-only
 Author: peaky76
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

