# Comparing `tmp/axe_playwright_python-0.1.3.tar.gz` & `tmp/axe_playwright_python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axe_playwright_python-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "axe_playwright_python-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `axe_playwright_python-0.1.3.tar` & `axe_playwright_python-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      922 2023-07-24 22:02:57.751373 axe_playwright_python-0.1.3/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2023-04-03 13:02:19.819263 axe_playwright_python-0.1.3/.gitignore
--rw-r--r--   0        0        0      405 2023-07-24 22:01:27.106479 axe_playwright_python-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       80 2023-04-03 13:02:19.819796 axe_playwright_python-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0      380 2023-07-24 22:15:42.488285 axe_playwright_python-0.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1081 2023-07-20 18:37:43.617118 axe_playwright_python-0.1.3/LICENSE
--rw-r--r--   0        0        0     1360 2023-07-23 19:33:50.981062 axe_playwright_python-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-07-24 22:39:16.087979 axe_playwright_python-0.1.3/axe_playwright_python/__init__.py
--rw-r--r--   0        0        0     1279 2023-07-24 22:07:26.775328 axe_playwright_python-0.1.3/axe_playwright_python/async_playwright.py
--rw-r--r--   0        0        0   436082 2023-04-03 13:02:19.822321 axe_playwright_python-0.1.3/axe_playwright_python/axe.min.js
--rw-r--r--   0        0        0     4356 2023-07-24 21:57:47.671531 axe_playwright_python-0.1.3/axe_playwright_python/base.py
--rw-r--r--   0        0        0     1257 2023-07-24 22:07:15.194045 axe_playwright_python-0.1.3/axe_playwright_python/sync_playwright.py
--rw-r--r--   0        0        0      115 2023-07-24 22:32:25.676875 axe_playwright_python-0.1.3/axe_playwright_python/violations.txt
--rw-r--r--   0        0        0      101 2023-07-20 18:37:43.623671 axe_playwright_python-0.1.3/docs/api.md
--rw-r--r--   0        0        0      693 2023-07-20 21:02:33.627100 axe_playwright_python-0.1.3/docs/index.md
--rw-r--r--   0        0        0     2383 2023-07-20 18:37:43.624812 axe_playwright_python-0.1.3/docs/usage.md
--rw-r--r--   0        0        0      309 2023-07-23 19:41:06.816546 axe_playwright_python-0.1.3/examples/usage.py
--rw-r--r--   0        0        0      840 2023-07-20 18:38:30.351452 axe_playwright_python-0.1.3/mkdocs.yml
--rw-r--r--   0        0        0     1675 2023-07-24 22:39:03.040543 axe_playwright_python-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 13:02:19.828070 axe_playwright_python-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2198 2023-07-23 19:40:35.377787 axe_playwright_python-0.1.3/tests/test_axe_async_playwright.py
--rw-r--r--   0        0        0     1945 2023-07-23 19:40:35.377772 axe_playwright_python-0.1.3/tests/test_axe_sync_playwright.py
--rw-r--r--   0        0        0      379 2023-04-03 13:02:19.829198 axe_playwright_python-0.1.3/tests/test_page.html
--rw-r--r--   0        0        0    32278 2023-07-24 22:33:06.155615 axe_playwright_python-0.1.3/tests/test_report.txt
--rw-r--r--   0        0        0     9219 2023-07-24 22:32:55.948542 axe_playwright_python-0.1.3/tests/test_report_color.txt
--rw-r--r--   0        0        0     2212 2023-07-23 19:41:06.826891 axe_playwright_python-0.1.3/tests/test_report_save.py
--rw-r--r--   0        0        0   412591 2023-07-20 18:37:43.632179 axe_playwright_python-0.1.3/tests/test_result.json
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 axe_playwright_python-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      922 2023-07-25 13:07:14.252681 axe_playwright_python-0.1.4/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2023-04-03 13:02:19.819263 axe_playwright_python-0.1.4/.gitignore
+-rw-r--r--   0        0        0      405 2023-07-25 13:07:14.254580 axe_playwright_python-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       80 2023-04-03 13:02:19.819796 axe_playwright_python-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0      380 2023-07-25 13:07:14.255255 axe_playwright_python-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1081 2023-07-20 18:37:43.617118 axe_playwright_python-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1360 2023-07-25 13:07:14.255720 axe_playwright_python-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 13:07:18.583052 axe_playwright_python-0.1.4/axe_playwright_python/__init__.py
+-rw-r--r--   0        0        0     1279 2023-07-25 13:07:14.258012 axe_playwright_python-0.1.4/axe_playwright_python/async_playwright.py
+-rw-r--r--   0        0        0   436082 2023-04-03 13:02:19.822321 axe_playwright_python-0.1.4/axe_playwright_python/axe.min.js
+-rw-r--r--   0        0        0     4356 2023-07-25 13:07:14.259268 axe_playwright_python-0.1.4/axe_playwright_python/base.py
+-rw-r--r--   0        0        0     1257 2023-07-25 13:07:14.260414 axe_playwright_python-0.1.4/axe_playwright_python/sync_playwright.py
+-rw-r--r--   0        0        0      115 2023-07-25 13:07:14.260974 axe_playwright_python-0.1.4/axe_playwright_python/violations.txt
+-rw-r--r--   0        0        0      101 2023-07-20 18:37:43.623671 axe_playwright_python-0.1.4/docs/api.md
+-rw-r--r--   0        0        0      693 2023-07-20 21:02:33.627100 axe_playwright_python-0.1.4/docs/index.md
+-rw-r--r--   0        0        0     2383 2023-07-20 18:37:43.624812 axe_playwright_python-0.1.4/docs/usage.md
+-rw-r--r--   0        0        0      309 2023-07-25 13:07:14.263113 axe_playwright_python-0.1.4/examples/usage.py
+-rw-r--r--   0        0        0      840 2023-07-20 18:38:30.351452 axe_playwright_python-0.1.4/mkdocs.yml
+-rw-r--r--   0        0        0     1675 2023-07-25 13:07:39.957226 axe_playwright_python-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 13:02:19.828070 axe_playwright_python-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2198 2023-07-25 13:07:14.266305 axe_playwright_python-0.1.4/tests/test_axe_async_playwright.py
+-rw-r--r--   0        0        0     1945 2023-07-25 13:07:14.268190 axe_playwright_python-0.1.4/tests/test_axe_sync_playwright.py
+-rw-r--r--   0        0        0      379 2023-04-03 13:02:19.829198 axe_playwright_python-0.1.4/tests/test_page.html
+-rw-r--r--   0        0        0    32278 2023-07-25 13:07:14.268698 axe_playwright_python-0.1.4/tests/test_report.txt
+-rw-r--r--   0        0        0     9219 2023-07-25 13:07:14.269318 axe_playwright_python-0.1.4/tests/test_report_color.txt
+-rw-r--r--   0        0        0     2212 2023-07-25 13:07:14.269774 axe_playwright_python-0.1.4/tests/test_report_save.py
+-rw-r--r--   0        0        0   412591 2023-07-20 18:37:43.632179 axe_playwright_python-0.1.4/tests/test_result.json
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 axe_playwright_python-0.1.4/PKG-INFO
```

### Comparing `axe_playwright_python-0.1.3/.github/workflows/python.yaml` & `axe_playwright_python-0.1.4/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/.gitignore` & `axe_playwright_python-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/LICENSE` & `axe_playwright_python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/README.md` & `axe_playwright_python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/axe_playwright_python/async_playwright.py` & `axe_playwright_python-0.1.4/axe_playwright_python/async_playwright.py`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/axe_playwright_python/axe.min.js` & `axe_playwright_python-0.1.4/axe_playwright_python/axe.min.js`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/axe_playwright_python/base.py` & `axe_playwright_python-0.1.4/axe_playwright_python/base.py`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/axe_playwright_python/sync_playwright.py` & `axe_playwright_python-0.1.4/axe_playwright_python/sync_playwright.py`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/docs/index.md` & `axe_playwright_python-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/docs/usage.md` & `axe_playwright_python-0.1.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/mkdocs.yml` & `axe_playwright_python-0.1.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/pyproject.toml` & `axe_playwright_python-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "axe-playwright-python"
 description = "Automated web accessibility testing using axe-core engine and Playwright."
-version = "0.1.3"
+version = "0.1.4"
 authors = [{name = "Pamela Fox", "email" = "pamela.fox@gmail.com"}]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "playwright >= 1.36.0"
     ]
@@ -54,8 +54,8 @@
 target-version = "py38"
 select = ["E", "F", "I", "UP"]
 ignore = ["D203"]
 show-source = true
 
 [tool.black]
 line-length = 100
-target-version = ["py39"]
+target-version = ["py38"]
```

### Comparing `axe_playwright_python-0.1.3/tests/test_axe_async_playwright.py` & `axe_playwright_python-0.1.4/tests/test_axe_async_playwright.py`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/tests/test_axe_sync_playwright.py` & `axe_playwright_python-0.1.4/tests/test_axe_sync_playwright.py`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/tests/test_report.txt` & `axe_playwright_python-0.1.4/tests/test_report.txt`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/tests/test_report_color.txt` & `axe_playwright_python-0.1.4/tests/test_report_color.txt`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/tests/test_report_save.py` & `axe_playwright_python-0.1.4/tests/test_report_save.py`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/tests/test_result.json` & `axe_playwright_python-0.1.4/tests/test_result.json`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.3/PKG-INFO` & `axe_playwright_python-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axe-playwright-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automated web accessibility testing using axe-core engine and Playwright.
 Keywords: accessibility,axe,axe-core,playwright
 Author-email: Pamela Fox <pamela.fox@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

