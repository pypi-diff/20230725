# Comparing `tmp/parsagon-0.7.5.tar.gz` & `tmp/parsagon-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.7.5.tar", last modified: Fri Jul  7 07:06:03 2023, max compression
+gzip compressed data, was "parsagon-0.8.0.tar", last modified: Tue Jul 25 03:46:31 2023, max compression
```

## Comparing `parsagon-0.7.5.tar` & `parsagon-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.930888 parsagon-0.7.5/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-07 07:06:03.930194 parsagon-0.7.5/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.7.5/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1048 2023-07-07 07:03:35.000000 parsagon-0.7.5/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-07-07 07:06:03.931098 parsagon-0.7.5/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.913092 parsagon-0.7.5/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.5/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.918980 parsagon-0.7.5/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     4632 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.5/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    11215 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     9044 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     2883 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.929247 parsagon-0.7.5/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.5/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/test_invalid_args.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.924101 parsagon-0.7.5/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      646 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      263 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.386427 parsagon-0.8.0/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-25 03:46:31.385857 parsagon-0.8.0/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.8.0/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1048 2023-07-25 03:41:52.000000 parsagon-0.8.0/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-07-25 03:46:31.386567 parsagon-0.8.0/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.369940 parsagon-0.8.0/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.8.0/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.375966 parsagon-0.8.0/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     4632 2023-07-25 03:32:53.000000 parsagon-0.8.0/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.8.0/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    11458 2023-07-25 03:32:56.000000 parsagon-0.8.0/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     9044 2023-07-25 03:32:53.000000 parsagon-0.8.0/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.8.0/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.384700 parsagon-0.8.0/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.8.0/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/test_invalid_args.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.8.0/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-25 03:46:31.380817 parsagon-0.8.0/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      646 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      263 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-07-25 03:46:31.000000 parsagon-0.8.0/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.7.5/PKG-INFO` & `parsagon-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.5
+Version: 0.8.0
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.7.5/README.md` & `parsagon-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.5/pyproject.toml` & `parsagon-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.7.5"
+version = "0.8.0"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.7.5/src/parsagon/api.py` & `parsagon-0.8.0/src/parsagon/api.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.5/src/parsagon/custom_function.py` & `parsagon-0.8.0/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.5/src/parsagon/exceptions.py` & `parsagon-0.8.0/src/parsagon/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.5/src/parsagon/executor.py` & `parsagon-0.8.0/src/parsagon/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             self.display = Display(visible=False, size=(1280, 1050)).start()
         chrome_options = uc.ChromeOptions()
         chrome_options.add_argument("--start-maximized")
         seleniumwire_options = {"disable_capture": True}
         self.driver = uc.Chrome(options=chrome_options, seleniumwire_options=seleniumwire_options)
         self.max_elem_id = 0
         self.execution_context = {
+            "custom_assert": self.custom_assert,
             "goto": self.goto,
             "click_elem": self.click_elem,
             "fill_input": self.fill_input,
             "select_option": self.select_option,
             "scroll": self.scroll,
             "wait": self.wait,
             "scrape_data": self.scrape_data,
@@ -123,28 +124,33 @@
         return lxml.html.tostring(root).decode()
 
     def get_elem_by_description(self, elem_type, description):
         logger.info(f'Looking for {elem_type.lower()}: "{description}"')
         visible_html = self.get_visible_html()
         elem_id = get_interaction_element_id(visible_html, elem_type, description)
         if elem_id is None:
-            raise ParsagonException(f'Could not find an element matching "{description}". Perhaps try rephrasing your prompt.')
+            raise ParsagonException(
+                f'Could not find an element matching "{description}". Perhaps try rephrasing your prompt.'
+            )
         return elem_id
 
     def _get_elem(self, elem_id):
         """
         Gets a selenium element by Parsagon ID (psgn-id).
         """
         assert elem_id is not None
         result = self.driver.find_element(By.XPATH, f'//*[@data-psgn-id="{elem_id}"]')
         elem_text = result.text
         log_suffix = f' with text "{elem_text}"' if elem_text else ""
         logger.info(f"Found element" + log_suffix)
         return result
 
+    def custom_assert(self, v):
+        assert v, "Web page interaction failed."
+
     def goto(self, url, window_id=None):
         if window_id in self.driver.window_handles:
             self.driver.switch_to.window(window_id)
         else:
             self.driver.switch_to.new_window("tab")
 
         # Go to website
@@ -260,15 +266,17 @@
         )
         self.add_custom_function(call_id, custom_function)
         return True
 
     def scroll(self, x, y, window_id):
         self.driver.switch_to.window(window_id)
         logger.info(f"Scrolling {x * 100}% to the left and {y * 100}% down")
-        self.driver.execute_script(f"window.scrollTo({{top: document.documentElement.scrollHeight * {y}, left: document.documentElement.scrollWidth * {x}, behavior: 'smooth'}});")
+        self.driver.execute_script(
+            f"window.scrollTo({{top: document.documentElement.scrollHeight * {y}, left: document.documentElement.scrollWidth * {x}, behavior: 'smooth'}});"
+        )
         time.sleep(1)
 
     def wait(self, seconds):
         logger.info(f"Waiting {seconds} seconds...")
         time.sleep(seconds)
         self.mark_html()
 
@@ -279,17 +287,21 @@
         self.driver.switch_to.window(window_id)
         logger.info("Scraping data...")
         html = self.get_scrape_html()
         result = scrape_page(html, schema)
         scraped_data = result["data"]
         nodes = result["nodes"]
         if not scraped_data and not nodes:
-            raise ParsagonException(f"Parsagon could not find any data on the page that would fit the format {schema}. Perhaps try rephrasing your prompt.")
+            raise ParsagonException(
+                f"Parsagon could not find any data on the page that would fit the format {schema}. Perhaps try rephrasing your prompt."
+            )
         elif not nodes:
-            raise ParsagonException(f"Parsagon found the following data on the page for the format {schema}:\n\n{scraped_data}\n\nHowever, it could not find a plausible program to scrape this data. If the data above is incorrect, perhaps try rephrasing your prompt.")
+            raise ParsagonException(
+                f"Parsagon found the following data on the page for the format {schema}:\n\n{scraped_data}\n\nHowever, it could not find a plausible program to scrape this data. If the data above is incorrect, perhaps try rephrasing your prompt."
+            )
         logger.info(f"Scraped data:\n{scraped_data}")
         custom_function = CustomFunction(
             "scrape_data",
             arguments={
                 "schema": schema,
             },
             examples=[
```

### Comparing `parsagon-0.7.5/src/parsagon/main.py` & `parsagon-0.8.0/src/parsagon/main.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.5/src/parsagon/settings.py` & `parsagon-0.8.0/src/parsagon/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 from os import environ
 from pathlib import Path
 
 from parsagon.exceptions import ParsagonException
 
 __API_BASE = environ.get("API_BASE", "https://parsagon.io").rstrip("/")
+__SETTINGS_FILE = environ.get("SETTINGS_FILE", ".parsagon_profile")
 
 
 logger = logging.getLogger(__name__)
 
 
 def pytest_is_running():
     return "pytest" in sys.modules
@@ -68,15 +69,15 @@
     return get_settings().get(key)
 
 
 def get_settings_file_path():
     """
     Return settings file path, which is a hidden file in the user's home directory
     """
-    return Path().home() / ".parsagon_profile"
+    return Path().home() / __SETTINGS_FILE
 
 
 def get_api_base():
     """
     Return API base, preventing tests from talking to the real backend
     """
     if pytest_is_running():
```

### Comparing `parsagon-0.7.5/src/parsagon/tests/api_mocks.py` & `parsagon-0.8.0/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.5/src/parsagon/tests/test_invalid_args.py` & `parsagon-0.8.0/src/parsagon/tests/test_invalid_args.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.5/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.8.0/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.5/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.8.0/src/parsagon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.5
+Version: 0.8.0
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.7.5/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.8.0/src/parsagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

