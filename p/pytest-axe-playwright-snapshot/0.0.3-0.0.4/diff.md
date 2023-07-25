# Comparing `tmp/pytest_axe_playwright_snapshot-0.0.3.tar.gz` & `tmp/pytest_axe_playwright_snapshot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_axe_playwright_snapshot-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_axe_playwright_snapshot-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_axe_playwright_snapshot-0.0.3.tar` & `pytest_axe_playwright_snapshot-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      922 2023-07-24 23:40:31.061282 pytest_axe_playwright_snapshot-0.0.3/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.3/.gitignore
--rw-r--r--   0        0        0      361 2023-07-24 23:04:01.124134 pytest_axe_playwright_snapshot-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      279 2023-07-24 23:42:03.276912 pytest_axe_playwright_snapshot-0.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.3/LICENSE
--rw-r--r--   0        0        0     1205 2023-07-24 23:16:44.216289 pytest_axe_playwright_snapshot-0.0.3/README.md
--rw-r--r--   0        0        0     1576 2023-07-25 17:41:14.784176 pytest_axe_playwright_snapshot-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2973 2023-07-25 17:41:10.934853 pytest_axe_playwright_snapshot-0.0.3/pytest_axe_playwright_snapshot.py
--rw-r--r--   0        0        0        0 2023-07-23 14:54:08.677073 pytest_axe_playwright_snapshot-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0       82 2023-07-24 22:45:49.729690 pytest_axe_playwright_snapshot-0.0.3/tests/snapshots/test_snapshot/test_violations_fewer_instances/chromium/snapshot.txt
--rw-r--r--   0        0        0      112 2023-07-24 22:46:59.355286 pytest_axe_playwright_snapshot-0.0.3/tests/snapshots/test_snapshot/test_violations_fixed/chromium/snapshot.txt
--rw-r--r--   0        0        0       82 2023-07-24 22:45:39.356302 pytest_axe_playwright_snapshot-0.0.3/tests/snapshots/test_snapshot/test_violations_more_instances/chromium/snapshot.txt
--rw-r--r--   0        0        0       54 2023-07-24 22:44:48.422339 pytest_axe_playwright_snapshot-0.0.3/tests/snapshots/test_snapshot/test_violations_new/chromium/snapshot.txt
--rw-r--r--   0        0        0       82 2023-07-24 22:44:12.677433 pytest_axe_playwright_snapshot-0.0.3/tests/snapshots/test_snapshot/test_violations_same/chromium/snapshot.txt
--rw-r--r--   0        0        0     2533 2023-07-24 23:20:46.992596 pytest_axe_playwright_snapshot-0.0.3/tests/test_snapshot.py
--rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 pytest_axe_playwright_snapshot-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      922 2023-07-24 23:40:31.061282 pytest_axe_playwright_snapshot-0.0.4/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.4/.gitignore
+-rw-r--r--   0        0        0      361 2023-07-24 23:04:01.124134 pytest_axe_playwright_snapshot-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      279 2023-07-24 23:42:03.276912 pytest_axe_playwright_snapshot-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1205 2023-07-24 23:16:44.216289 pytest_axe_playwright_snapshot-0.0.4/README.md
+-rw-r--r--   0        0        0     1576 2023-07-25 18:05:38.429097 pytest_axe_playwright_snapshot-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2993 2023-07-25 18:05:21.176265 pytest_axe_playwright_snapshot-0.0.4/pytest_axe_playwright_snapshot.py
+-rw-r--r--   0        0        0        0 2023-07-23 14:54:08.677073 pytest_axe_playwright_snapshot-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0       82 2023-07-24 22:45:49.729690 pytest_axe_playwright_snapshot-0.0.4/tests/snapshots/test_snapshot/test_violations_fewer_instances/chromium/snapshot.txt
+-rw-r--r--   0        0        0      112 2023-07-24 22:46:59.355286 pytest_axe_playwright_snapshot-0.0.4/tests/snapshots/test_snapshot/test_violations_fixed/chromium/snapshot.txt
+-rw-r--r--   0        0        0       82 2023-07-24 22:45:39.356302 pytest_axe_playwright_snapshot-0.0.4/tests/snapshots/test_snapshot/test_violations_more_instances/chromium/snapshot.txt
+-rw-r--r--   0        0        0       54 2023-07-24 22:44:48.422339 pytest_axe_playwright_snapshot-0.0.4/tests/snapshots/test_snapshot/test_violations_new/chromium/snapshot.txt
+-rw-r--r--   0        0        0       82 2023-07-24 22:44:12.677433 pytest_axe_playwright_snapshot-0.0.4/tests/snapshots/test_snapshot/test_violations_same/chromium/snapshot.txt
+-rw-r--r--   0        0        0     2533 2023-07-24 23:20:46.992596 pytest_axe_playwright_snapshot-0.0.4/tests/test_snapshot.py
+-rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 pytest_axe_playwright_snapshot-0.0.4/PKG-INFO
```

### Comparing `pytest_axe_playwright_snapshot-0.0.3/.github/workflows/python.yaml` & `pytest_axe_playwright_snapshot-0.0.4/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.3/.gitignore` & `pytest_axe_playwright_snapshot-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.3/LICENSE` & `pytest_axe_playwright_snapshot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.3/README.md` & `pytest_axe_playwright_snapshot-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.3/pyproject.toml` & `pytest_axe_playwright_snapshot-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pytest-axe-playwright-snapshot"
 description = "A pytest plugin that runs Axe-core on Playwright pages and takes snapshots of the results."
-version = "0.0.3"
+version = "0.0.4"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "pytest",
     "pytest-cov",
```

### Comparing `pytest_axe_playwright_snapshot-0.0.3/pytest_axe_playwright_snapshot.py` & `pytest_axe_playwright_snapshot-0.0.4/pytest_axe_playwright_snapshot.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 @pytest.fixture
 def axe_pytest_snapshot(request, snapshot):
     print_reports = request.config.getoption("print_reports")
 
     def run_assert(page: Page):
         results = Axe().run(page)
         if print_reports:
-            print(f"Violations found for {page.title()}:")
+            print(f"\n\n** {request.node.name} report from axe-playwright **")
             print(results.generate_report())
         snapshot.assert_match(
             results.generate_snapshot(), message_generator=functools.partial(compare_violations, new_results=results)
         )
 
     return run_assert
```

### Comparing `pytest_axe_playwright_snapshot-0.0.3/tests/test_snapshot.py` & `pytest_axe_playwright_snapshot-0.0.4/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.3/PKG-INFO` & `pytest_axe_playwright_snapshot-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-axe-playwright-snapshot
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pytest plugin that runs Axe-core on Playwright pages and takes snapshots of the results.
 Author: Pamela Fox
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

