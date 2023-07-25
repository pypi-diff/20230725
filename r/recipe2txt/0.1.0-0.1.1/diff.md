# Comparing `tmp/recipe2txt-0.1.0.tar.gz` & `tmp/recipe2txt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recipe2txt-0.1.0.tar", last modified: Tue Jul 25 20:46:59 2023, max compression
+gzip compressed data, was "recipe2txt-0.1.1.tar", last modified: Tue Jul 25 21:05:38 2023, max compression
```

## Comparing `recipe2txt-0.1.0.tar` & `recipe2txt-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 20:46:59.418472 recipe2txt-0.1.0/
--rw-rw-r--   0 pc        (1000) pc        (1000)    35149 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/LICENSE
--rw-rw-r--   0 pc        (1000) pc        (1000)     5359 2023-07-25 20:46:59.418472 recipe2txt-0.1.0/PKG-INFO
--rw-rw-r--   0 pc        (1000) pc        (1000)     4239 2023-07-25 20:13:34.000000 recipe2txt-0.1.0/README.md
--rw-rw-r--   0 pc        (1000) pc        (1000)     1622 2023-07-25 20:42:43.000000 recipe2txt-0.1.0/pyproject.toml
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 20:46:59.410472 recipe2txt-0.1.0/recipe2txt/
--rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-07-11 12:26:00.000000 recipe2txt-0.1.0/recipe2txt/__init__.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     9047 2023-07-25 20:13:34.000000 recipe2txt-0.1.0/recipe2txt/argparse.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3736 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/recipe2txt/fetcher_abstract.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3057 2023-07-25 20:13:00.000000 recipe2txt-0.1.0/recipe2txt/fetcher_async.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     2164 2023-07-25 20:13:00.000000 recipe2txt-0.1.0/recipe2txt/fetcher_serial.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     7580 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/recipe2txt/file_setup.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    13153 2023-07-25 20:13:00.000000 recipe2txt-0.1.0/recipe2txt/html2recipe.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     1300 2023-07-25 20:13:00.000000 recipe2txt-0.1.0/recipe2txt/re2txt.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    10373 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/recipe2txt/sql.py
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 20:46:59.414472 recipe2txt-0.1.0/recipe2txt/utils/
--rw-rw-r--   0 pc        (1000) pc        (1000)    11382 2023-07-25 19:34:56.000000 recipe2txt-0.1.0/recipe2txt/utils/ContextLogger.py
--rw-rw-r--   0 pc        (1000) pc        (1000)        2 2023-03-10 12:21:19.000000 recipe2txt-0.1.0/recipe2txt/utils/__init__.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     1069 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/recipe2txt/utils/conditional_imports.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4255 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/recipe2txt/utils/markdown.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     7316 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/recipe2txt/utils/misc.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     2347 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/recipe2txt/utils/timer.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3203 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/recipe2txt/utils/traceback_utils.py
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 20:46:59.410472 recipe2txt-0.1.0/recipe2txt.egg-info/
--rw-rw-r--   0 pc        (1000) pc        (1000)     5359 2023-07-25 20:46:59.000000 recipe2txt-0.1.0/recipe2txt.egg-info/PKG-INFO
--rw-rw-r--   0 pc        (1000) pc        (1000)      882 2023-07-25 20:46:59.000000 recipe2txt-0.1.0/recipe2txt.egg-info/SOURCES.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)        1 2023-07-25 20:46:59.000000 recipe2txt-0.1.0/recipe2txt.egg-info/dependency_links.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       86 2023-07-25 20:46:59.000000 recipe2txt-0.1.0/recipe2txt.egg-info/entry_points.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)      199 2023-07-25 20:46:59.000000 recipe2txt-0.1.0/recipe2txt.egg-info/requires.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       11 2023-07-25 20:46:59.000000 recipe2txt-0.1.0/recipe2txt.egg-info/top_level.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       38 2023-07-25 20:46:59.418472 recipe2txt-0.1.0/setup.cfg
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 20:46:59.418472 recipe2txt-0.1.0/test/
--rw-rw-r--   0 pc        (1000) pc        (1000)    14635 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/test/test_contextlogger.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3484 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/test/test_fetcher.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     5694 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/test/test_file_setup.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     5155 2023-07-25 20:03:06.000000 recipe2txt-0.1.0/test/test_helpers.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4477 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/test/test_html2recipe.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     6332 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/test/test_misc.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     8542 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/test/test_sql.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     1458 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/test/test_timer.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3197 2023-07-25 13:15:25.000000 recipe2txt-0.1.0/test/test_traceback_utils.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.320814 recipe2txt-0.1.1/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    35149 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/LICENSE
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5359 2023-07-25 21:05:38.320814 recipe2txt-0.1.1/PKG-INFO
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4239 2023-07-25 20:13:34.000000 recipe2txt-0.1.1/README.md
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1622 2023-07-25 21:03:53.000000 recipe2txt-0.1.1/pyproject.toml
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.312814 recipe2txt-0.1.1/recipe2txt/
+-rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-07-11 12:26:00.000000 recipe2txt-0.1.1/recipe2txt/__init__.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     9047 2023-07-25 20:13:34.000000 recipe2txt-0.1.1/recipe2txt/argparse.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3736 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/fetcher_abstract.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3057 2023-07-25 20:13:00.000000 recipe2txt-0.1.1/recipe2txt/fetcher_async.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     2164 2023-07-25 20:13:00.000000 recipe2txt-0.1.1/recipe2txt/fetcher_serial.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     7580 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/file_setup.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    13148 2023-07-25 21:02:27.000000 recipe2txt-0.1.1/recipe2txt/html2recipe.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1300 2023-07-25 20:13:00.000000 recipe2txt-0.1.1/recipe2txt/re2txt.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    10373 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/sql.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.316814 recipe2txt-0.1.1/recipe2txt/utils/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    11382 2023-07-25 19:34:56.000000 recipe2txt-0.1.1/recipe2txt/utils/ContextLogger.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)        2 2023-03-10 12:21:19.000000 recipe2txt-0.1.1/recipe2txt/utils/__init__.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1069 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/conditional_imports.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4255 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/markdown.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     7316 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/misc.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     2347 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/timer.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3203 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/recipe2txt/utils/traceback_utils.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.316814 recipe2txt-0.1.1/recipe2txt.egg-info/
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5359 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/PKG-INFO
+-rw-rw-r--   0 pc        (1000) pc        (1000)      882 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/SOURCES.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)        1 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/dependency_links.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       86 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/entry_points.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)      199 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/requires.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       11 2023-07-25 21:05:38.000000 recipe2txt-0.1.1/recipe2txt.egg-info/top_level.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       38 2023-07-25 21:05:38.320814 recipe2txt-0.1.1/setup.cfg
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2023-07-25 21:05:38.320814 recipe2txt-0.1.1/test/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    14635 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_contextlogger.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3484 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_fetcher.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5694 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_file_setup.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5155 2023-07-25 20:03:06.000000 recipe2txt-0.1.1/test/test_helpers.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4477 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_html2recipe.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     6332 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_misc.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     8542 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_sql.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1458 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_timer.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3197 2023-07-25 13:15:25.000000 recipe2txt-0.1.1/test/test_traceback_utils.py
```

### Comparing `recipe2txt-0.1.0/LICENSE` & `recipe2txt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/PKG-INFO` & `recipe2txt-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe2txt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Scrapes recipes and converts them to txt or markdown
 Author-email: Jan Philipp Berg <git.7ksst@aleeas.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/jp-berg/recipe2txt
 Project-URL: Bug Tracker, https://github.com/jp-berg/recipe2txt/issues
 Keywords: recipes,cooking,scraping,website
 Classifier: Programming Language :: Python :: 3
```

### Comparing `recipe2txt-0.1.0/README.md` & `recipe2txt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/pyproject.toml` & `recipe2txt-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "recipe2txt"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Jan Philipp Berg", email="git.7ksst@aleeas.com" },
 ]
 description = "Scrapes recipes and converts them to txt or markdown"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
```

### Comparing `recipe2txt-0.1.0/recipe2txt/argparse.py` & `recipe2txt-0.1.1/recipe2txt/argparse.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/fetcher_abstract.py` & `recipe2txt-0.1.1/recipe2txt/fetcher_abstract.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/fetcher_async.py` & `recipe2txt-0.1.1/recipe2txt/fetcher_async.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/fetcher_serial.py` & `recipe2txt-0.1.1/recipe2txt/fetcher_serial.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/file_setup.py` & `recipe2txt-0.1.1/recipe2txt/file_setup.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/html2recipe.py` & `recipe2txt-0.1.1/recipe2txt/html2recipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
 
 
 def html2parsed(url: URL, content: str) -> Optional[Parsed]:
     try:
         parsed: Parsed = Parsed(recipe_scrapers.scrape_html(html=content, org_url=url))
     except (WebsiteNotImplementedError,
             NoSchemaFoundInWildMode):
-        logger.error("Unknown Website. Extraction not supported", url)
+        logger.error("Unknown Website. Extraction not supported")
         return None
     except (AttributeError, TypeError) as e:
         handle_parsing_error(url, e)
         return None
     except Exception as e:
         if type(e) in (KeyboardInterrupt, SystemExit, MemoryError):
             raise e
```

### Comparing `recipe2txt-0.1.0/recipe2txt/re2txt.py` & `recipe2txt-0.1.1/recipe2txt/re2txt.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/sql.py` & `recipe2txt-0.1.1/recipe2txt/sql.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/utils/ContextLogger.py` & `recipe2txt-0.1.1/recipe2txt/utils/ContextLogger.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/utils/conditional_imports.py` & `recipe2txt-0.1.1/recipe2txt/utils/conditional_imports.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/utils/markdown.py` & `recipe2txt-0.1.1/recipe2txt/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/utils/misc.py` & `recipe2txt-0.1.1/recipe2txt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/utils/timer.py` & `recipe2txt-0.1.1/recipe2txt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt/utils/traceback_utils.py` & `recipe2txt-0.1.1/recipe2txt/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/recipe2txt.egg-info/PKG-INFO` & `recipe2txt-0.1.1/recipe2txt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe2txt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Scrapes recipes and converts them to txt or markdown
 Author-email: Jan Philipp Berg <git.7ksst@aleeas.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/jp-berg/recipe2txt
 Project-URL: Bug Tracker, https://github.com/jp-berg/recipe2txt/issues
 Keywords: recipes,cooking,scraping,website
 Classifier: Programming Language :: Python :: 3
```

### Comparing `recipe2txt-0.1.0/recipe2txt.egg-info/SOURCES.txt` & `recipe2txt-0.1.1/recipe2txt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_contextlogger.py` & `recipe2txt-0.1.1/test/test_contextlogger.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_fetcher.py` & `recipe2txt-0.1.1/test/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_file_setup.py` & `recipe2txt-0.1.1/test/test_file_setup.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_helpers.py` & `recipe2txt-0.1.1/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_html2recipe.py` & `recipe2txt-0.1.1/test/test_html2recipe.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_misc.py` & `recipe2txt-0.1.1/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_sql.py` & `recipe2txt-0.1.1/test/test_sql.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_timer.py` & `recipe2txt-0.1.1/test/test_timer.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.1.0/test/test_traceback_utils.py` & `recipe2txt-0.1.1/test/test_traceback_utils.py`

 * *Files identical despite different names*

