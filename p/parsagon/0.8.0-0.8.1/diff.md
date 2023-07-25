# Comparing `tmp/parsagon-0.8.0.tar.gz` & `tmp/parsagon-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.8.0.tar", last modified: Tue Jul 25 03:46:31 2023, max compression
+gzip compressed data, was "parsagon-0.8.1.tar", last modified: Tue Jul 25 06:04:52 2023, max compression
```

## Comparing `parsagon-0.8.0.tar` & `parsagon-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.386427 parsagon-0.8.0/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-25 03:46:31.385857 parsagon-0.8.0/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.8.0/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1048 2023-07-25 03:41:52.000000 parsagon-0.8.0/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-07-25 03:46:31.386567 parsagon-0.8.0/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.369940 parsagon-0.8.0/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.8.0/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.375966 parsagon-0.8.0/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     4632 2023-07-25 03:32:53.000000 parsagon-0.8.0/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.8.0/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    11458 2023-07-25 03:32:56.000000 parsagon-0.8.0/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     9044 2023-07-25 03:32:53.000000 parsagon-0.8.0/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.8.0/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.384700 parsagon-0.8.0/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.8.0/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/test_invalid_args.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.380817 parsagon-0.8.0/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      646 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      263 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.838197 parsagon-0.8.1/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-25 06:04:52.837869 parsagon-0.8.1/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.8.1/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1048 2023-07-25 06:04:15.000000 parsagon-0.8.1/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-07-25 06:04:52.838300 parsagon-0.8.1/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.823145 parsagon-0.8.1/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.8.1/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.830641 parsagon-0.8.1/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     4677 2023-07-25 05:41:45.000000 parsagon-0.8.1/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.8.1/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    11483 2023-07-25 05:49:16.000000 parsagon-0.8.1/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     9044 2023-07-25 03:32:53.000000 parsagon-0.8.1/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.8.1/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.837192 parsagon-0.8.1/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.8.1/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/test_invalid_args.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.8.1/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 06:04:52.833742 parsagon-0.8.1/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      646 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      263 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-07-25 06:04:52.000000 parsagon-0.8.1/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.8.0/PKG-INFO` & `parsagon-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.8.0
+Version: 0.8.1
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.8.0/README.md` & `parsagon-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.0/pyproject.toml` & `parsagon-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.8.0"
+version = "0.8.1"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.8.0/src/parsagon/api.py` & `parsagon-0.8.1/src/parsagon/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,22 +76,23 @@
         httpx.post,
         "/transformers/get-nav-elem/",
         json={"html": marked_html, "elem_type": elem_type, "description": description},
     )["id"]
     return result
 
 
-def scrape_page(html, schema):
+def scrape_page(url, html, schema):
     """
     Scrapes data from the provided page HTML - data will be returned in the schema provided.
+    :param url: url of the page to scrape.
     :param html: HTML of the page to scrape.
-    :param schema: Schema of the data to scrape, in the format
+    :param schema: Schema of the data to scrape
     :return: Scraped data, with lists truncated.
     """
-    return _api_call(httpx.post, "/transformers/get-custom-data/", json={"html": html, "schema": schema})
+    return _api_call(httpx.post, "/transformers/get-custom-data/", json={"url": url, "html": html, "schema": schema})
 
 
 def create_pipeline(name, description, program_sketch):
     return _api_call(
         httpx.post, "/pipelines/", json={"name": name, "description": description, "program_sketch": program_sketch}
     )
```

### Comparing `parsagon-0.8.0/src/parsagon/custom_function.py` & `parsagon-0.8.1/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.0/src/parsagon/exceptions.py` & `parsagon-0.8.1/src/parsagon/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.0/src/parsagon/executor.py` & `parsagon-0.8.1/src/parsagon/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
     def scrape_data(self, schema, window_id, call_id):
         """
         Scrapes data from the current page.
         """
         self.driver.switch_to.window(window_id)
         logger.info("Scraping data...")
         html = self.get_scrape_html()
-        result = scrape_page(html, schema)
+        result = scrape_page(self.driver.current_url, html, schema)
         scraped_data = result["data"]
         nodes = result["nodes"]
         if not scraped_data and not nodes:
             raise ParsagonException(
                 f"Parsagon could not find any data on the page that would fit the format {schema}. Perhaps try rephrasing your prompt."
             )
         elif not nodes:
```

### Comparing `parsagon-0.8.0/src/parsagon/main.py` & `parsagon-0.8.1/src/parsagon/main.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.0/src/parsagon/settings.py` & `parsagon-0.8.1/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.0/src/parsagon/tests/api_mocks.py` & `parsagon-0.8.1/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.0/src/parsagon/tests/test_invalid_args.py` & `parsagon-0.8.1/src/parsagon/tests/test_invalid_args.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.0/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.8.1/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.8.0/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.8.1/src/parsagon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.8.0
+Version: 0.8.1
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.8.0/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.8.1/src/parsagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

