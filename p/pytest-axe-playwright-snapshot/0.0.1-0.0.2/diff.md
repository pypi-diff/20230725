# Comparing `tmp/pytest_axe_playwright_snapshot-0.0.1.tar.gz` & `tmp/pytest_axe_playwright_snapshot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_axe_playwright_snapshot-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_axe_playwright_snapshot-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_axe_playwright_snapshot-0.0.1.tar` & `pytest_axe_playwright_snapshot-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0      922 2023-07-24 23:40:31.061282 pytest_axe_playwright_snapshot-0.0.1/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.1/.gitignore
--rw-r--r--   0        0        0      361 2023-07-24 23:04:01.124134 pytest_axe_playwright_snapshot-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      279 2023-07-24 23:42:03.276912 pytest_axe_playwright_snapshot-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.1/LICENSE
--rw-r--r--   0        0        0     1205 2023-07-24 23:16:44.216289 pytest_axe_playwright_snapshot-0.0.1/README.md
--rw-r--r--   0        0        0     1509 2023-07-25 14:59:58.763955 pytest_axe_playwright_snapshot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2543 2023-07-23 14:01:41.721086 pytest_axe_playwright_snapshot-0.0.1/pytest_axe_playwright_snapshot.py
--rw-r--r--   0        0        0        0 2023-07-23 14:54:08.677073 pytest_axe_playwright_snapshot-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0       54 2023-07-23 14:57:17.989973 pytest_axe_playwright_snapshot-0.0.1/tests/snapshots/test_snapshot/test_fail/chromium/snapshot.txt
--rw-r--r--   0        0        0       82 2023-07-23 14:56:41.913291 pytest_axe_playwright_snapshot-0.0.1/tests/snapshots/test_snapshot/test_pass/chromium/snapshot.txt
--rw-r--r--   0        0        0       82 2023-07-24 22:45:49.729690 pytest_axe_playwright_snapshot-0.0.1/tests/snapshots/test_snapshot/test_violations_fewer_instances/chromium/snapshot.txt
--rw-r--r--   0        0        0      112 2023-07-24 22:46:59.355286 pytest_axe_playwright_snapshot-0.0.1/tests/snapshots/test_snapshot/test_violations_fixed/chromium/snapshot.txt
--rw-r--r--   0        0        0       82 2023-07-24 22:45:39.356302 pytest_axe_playwright_snapshot-0.0.1/tests/snapshots/test_snapshot/test_violations_more_instances/chromium/snapshot.txt
--rw-r--r--   0        0        0       54 2023-07-24 22:44:48.422339 pytest_axe_playwright_snapshot-0.0.1/tests/snapshots/test_snapshot/test_violations_new/chromium/snapshot.txt
--rw-r--r--   0        0        0       82 2023-07-24 22:44:12.677433 pytest_axe_playwright_snapshot-0.0.1/tests/snapshots/test_snapshot/test_violations_same/chromium/snapshot.txt
--rw-r--r--   0        0        0     2533 2023-07-24 23:20:46.992596 pytest_axe_playwright_snapshot-0.0.1/tests/test_snapshot.py
--rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 pytest_axe_playwright_snapshot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      922 2023-07-24 23:40:31.061282 pytest_axe_playwright_snapshot-0.0.2/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.2/.gitignore
+-rw-r--r--   0        0        0      361 2023-07-24 23:04:01.124134 pytest_axe_playwright_snapshot-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      279 2023-07-24 23:42:03.276912 pytest_axe_playwright_snapshot-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1205 2023-07-24 23:16:44.216289 pytest_axe_playwright_snapshot-0.0.2/README.md
+-rw-r--r--   0        0        0     1576 2023-07-25 17:16:26.821282 pytest_axe_playwright_snapshot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2971 2023-07-25 17:15:55.047108 pytest_axe_playwright_snapshot-0.0.2/pytest_axe_playwright_snapshot.py
+-rw-r--r--   0        0        0        0 2023-07-23 14:54:08.677073 pytest_axe_playwright_snapshot-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0       82 2023-07-24 22:45:49.729690 pytest_axe_playwright_snapshot-0.0.2/tests/snapshots/test_snapshot/test_violations_fewer_instances/chromium/snapshot.txt
+-rw-r--r--   0        0        0      112 2023-07-24 22:46:59.355286 pytest_axe_playwright_snapshot-0.0.2/tests/snapshots/test_snapshot/test_violations_fixed/chromium/snapshot.txt
+-rw-r--r--   0        0        0       82 2023-07-24 22:45:39.356302 pytest_axe_playwright_snapshot-0.0.2/tests/snapshots/test_snapshot/test_violations_more_instances/chromium/snapshot.txt
+-rw-r--r--   0        0        0       54 2023-07-24 22:44:48.422339 pytest_axe_playwright_snapshot-0.0.2/tests/snapshots/test_snapshot/test_violations_new/chromium/snapshot.txt
+-rw-r--r--   0        0        0       82 2023-07-24 22:44:12.677433 pytest_axe_playwright_snapshot-0.0.2/tests/snapshots/test_snapshot/test_violations_same/chromium/snapshot.txt
+-rw-r--r--   0        0        0     2533 2023-07-24 23:20:46.992596 pytest_axe_playwright_snapshot-0.0.2/tests/test_snapshot.py
+-rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 pytest_axe_playwright_snapshot-0.0.2/PKG-INFO
```

### Comparing `pytest_axe_playwright_snapshot-0.0.1/.github/workflows/python.yaml` & `pytest_axe_playwright_snapshot-0.0.2/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.1/.gitignore` & `pytest_axe_playwright_snapshot-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.1/LICENSE` & `pytest_axe_playwright_snapshot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.1/README.md` & `pytest_axe_playwright_snapshot-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.1/pyproject.toml` & `pytest_axe_playwright_snapshot-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "pytest-axe-playwright-snapshot"
 description = "A pytest plugin that runs Axe-core on Playwright pages and takes snapshots of the results."
-version = "0.0.1"
+version = "0.0.2"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "pytest",
+    "pytest-cov",
     "playwright",
     "axe-playwright-python",
     "pytest-snapshot-with-message-generator"
     ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -54,12 +55,15 @@
 ignore = ["D203"]
 show-source = true
 
 [tool.black]
 line-length = 120
 target-version = ["py38"]
 
+[tool.pytest.ini_options]
+addopts = "-ra --cov"
+
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `pytest_axe_playwright_snapshot-0.0.1/pytest_axe_playwright_snapshot.py` & `pytest_axe_playwright_snapshot-0.0.2/pytest_axe_playwright_snapshot.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,16 +47,28 @@
             violation_id = violation.split(" (")[0]
             message += new_results.generate_report(violation_id=violation_id)
     if len(keys_diff["decreased"]) > 0:
         message += f"Fewer instances of existing violations were found: {','.join(keys_diff['decreased'])}.\n{good_msg}"
     return message
 
 
+def pytest_addoption(parser):
+    group = parser.getgroup("axe_playwright_snapshot")
+    group.addoption(
+        "--print-reports", action="store_true", default=False, help="Print full reports for violations to stdout"
+    )
+
+
 @pytest.fixture
-def axe_pytest_snapshot(snapshot):
+def axe_pytest_snapshot(request, snapshot):
+    print_reports = request.config.getoption("print_reports")
+
     def run_assert(page: Page):
         results = Axe().run(page)
+        if print_reports:
+            print(f"Violations found for {page.title()}:")
+            print(results.generate_report)
         snapshot.assert_match(
             results.generate_snapshot(), message_generator=functools.partial(compare_violations, new_results=results)
         )
 
     return run_assert
```

### Comparing `pytest_axe_playwright_snapshot-0.0.1/tests/test_snapshot.py` & `pytest_axe_playwright_snapshot-0.0.2/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.1/PKG-INFO` & `pytest_axe_playwright_snapshot-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-axe-playwright-snapshot
-Version: 0.0.1
+Version: 0.0.2
 Summary: A pytest plugin that runs Axe-core on Playwright pages and takes snapshots of the results.
 Author: Pamela Fox
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Pytest
 Requires-Dist: pytest
+Requires-Dist: pytest-cov
 Requires-Dist: playwright
 Requires-Dist: axe-playwright-python
 Requires-Dist: pytest-snapshot-with-message-generator
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-playwright ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
```

