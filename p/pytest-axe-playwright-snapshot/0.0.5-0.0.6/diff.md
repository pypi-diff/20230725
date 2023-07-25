# Comparing `tmp/pytest_axe_playwright_snapshot-0.0.5.tar.gz` & `tmp/pytest_axe_playwright_snapshot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_axe_playwright_snapshot-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_axe_playwright_snapshot-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_axe_playwright_snapshot-0.0.5.tar` & `pytest_axe_playwright_snapshot-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      922 2023-07-24 23:40:31.061282 pytest_axe_playwright_snapshot-0.0.5/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.5/.gitignore
--rw-r--r--   0        0        0      361 2023-07-24 23:04:01.124134 pytest_axe_playwright_snapshot-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      279 2023-07-24 23:42:03.276912 pytest_axe_playwright_snapshot-0.0.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.5/LICENSE
--rw-r--r--   0        0        0     1205 2023-07-24 23:16:44.216289 pytest_axe_playwright_snapshot-0.0.5/README.md
--rw-r--r--   0        0        0     1550 2023-07-25 19:00:36.024703 pytest_axe_playwright_snapshot-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3134 2023-07-25 19:00:36.025464 pytest_axe_playwright_snapshot-0.0.5/pytest_axe_playwright_snapshot.py
--rw-r--r--   0        0        0        0 2023-07-23 14:54:08.677073 pytest_axe_playwright_snapshot-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0       82 2023-07-25 18:54:48.759660 pytest_axe_playwright_snapshot-0.0.5/tests/snapshots/test_snapshot/test_violations_fewer_instances/chromium/snapshot.txt
--rw-r--r--   0        0        0      112 2023-07-25 18:54:50.596298 pytest_axe_playwright_snapshot-0.0.5/tests/snapshots/test_snapshot/test_violations_fixed/chromium/snapshot.txt
--rw-r--r--   0        0        0       82 2023-07-25 18:54:52.459883 pytest_axe_playwright_snapshot-0.0.5/tests/snapshots/test_snapshot/test_violations_more_instances/chromium/snapshot.txt
--rw-r--r--   0        0        0       54 2023-07-25 18:54:54.751234 pytest_axe_playwright_snapshot-0.0.5/tests/snapshots/test_snapshot/test_violations_new/chromium/snapshot.txt
--rw-r--r--   0        0        0        0 2023-07-25 19:00:36.026411 pytest_axe_playwright_snapshot-0.0.5/tests/snapshots/test_snapshot/test_violations_new_from_empty/chromium/snapshot.txt
--rw-r--r--   0        0        0       82 2023-07-24 22:44:12.677433 pytest_axe_playwright_snapshot-0.0.5/tests/snapshots/test_snapshot/test_violations_same/chromium/snapshot.txt
--rw-r--r--   0        0        0     4303 2023-07-25 19:00:36.030467 pytest_axe_playwright_snapshot-0.0.5/tests/test_snapshot.py
--rw-r--r--   0        0        0      452 2023-07-25 19:00:36.031048 pytest_axe_playwright_snapshot-0.0.5/tests/test_snapshot_to_dict.py
--rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 pytest_axe_playwright_snapshot-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      922 2023-07-24 23:40:31.061282 pytest_axe_playwright_snapshot-0.0.6/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.6/.gitignore
+-rw-r--r--   0        0        0      361 2023-07-24 23:04:01.124134 pytest_axe_playwright_snapshot-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      279 2023-07-24 23:42:03.276912 pytest_axe_playwright_snapshot-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2023-03-19 14:55:34.000000 pytest_axe_playwright_snapshot-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1205 2023-07-24 23:16:44.216289 pytest_axe_playwright_snapshot-0.0.6/README.md
+-rw-r--r--   0        0        0     1550 2023-07-25 19:08:07.111731 pytest_axe_playwright_snapshot-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3132 2023-07-25 19:08:07.112194 pytest_axe_playwright_snapshot-0.0.6/pytest_axe_playwright_snapshot.py
+-rw-r--r--   0        0        0        0 2023-07-23 14:54:08.677073 pytest_axe_playwright_snapshot-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0       82 2023-07-25 18:54:48.759660 pytest_axe_playwright_snapshot-0.0.6/tests/snapshots/test_snapshot/test_violations_fewer_instances/chromium/snapshot.txt
+-rw-r--r--   0        0        0      112 2023-07-25 18:54:50.596298 pytest_axe_playwright_snapshot-0.0.6/tests/snapshots/test_snapshot/test_violations_fixed/chromium/snapshot.txt
+-rw-r--r--   0        0        0       82 2023-07-25 18:54:52.459883 pytest_axe_playwright_snapshot-0.0.6/tests/snapshots/test_snapshot/test_violations_more_instances/chromium/snapshot.txt
+-rw-r--r--   0        0        0       54 2023-07-25 18:54:54.751234 pytest_axe_playwright_snapshot-0.0.6/tests/snapshots/test_snapshot/test_violations_new/chromium/snapshot.txt
+-rw-r--r--   0        0        0        0 2023-07-25 19:00:36.026411 pytest_axe_playwright_snapshot-0.0.6/tests/snapshots/test_snapshot/test_violations_new_from_empty/chromium/snapshot.txt
+-rw-r--r--   0        0        0       82 2023-07-24 22:44:12.677433 pytest_axe_playwright_snapshot-0.0.6/tests/snapshots/test_snapshot/test_violations_same/chromium/snapshot.txt
+-rw-r--r--   0        0        0     4298 2023-07-25 19:08:07.112650 pytest_axe_playwright_snapshot-0.0.6/tests/test_snapshot.py
+-rw-r--r--   0        0        0      452 2023-07-25 19:00:36.031048 pytest_axe_playwright_snapshot-0.0.6/tests/test_snapshot_to_dict.py
+-rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 pytest_axe_playwright_snapshot-0.0.6/PKG-INFO
```

### Comparing `pytest_axe_playwright_snapshot-0.0.5/.github/workflows/python.yaml` & `pytest_axe_playwright_snapshot-0.0.6/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.5/.gitignore` & `pytest_axe_playwright_snapshot-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.5/LICENSE` & `pytest_axe_playwright_snapshot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.5/README.md` & `pytest_axe_playwright_snapshot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pytest_axe_playwright_snapshot-0.0.5/pyproject.toml` & `pytest_axe_playwright_snapshot-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pytest-axe-playwright-snapshot"
 description = "A pytest plugin that runs Axe-core on Playwright pages and takes snapshots of the results."
-version = "0.0.5"
+version = "0.0.6"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "pytest",
     "pytest-cov",
```

### Comparing `pytest_axe_playwright_snapshot-0.0.5/pytest_axe_playwright_snapshot.py` & `pytest_axe_playwright_snapshot-0.0.6/pytest_axe_playwright_snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             keys_diff["increased"].add(key)
         seen_keys.add(key)
     for key in new_counts:
         if key not in seen_keys:
             keys_diff["added"].add(key)
     good_msg = "That's good news! 🎉 Run `pytest --snapshot-update` to update the snapshots.\n"
     bad_msg = "That's bad news! 😱 Either fix the issue or run `pytest --snapshot-update` to update the snapshots.\n"
-    message = "\n"
+    message = ""
     for keys_name in keys_diff:
         keys_diff[keys_name] = sorted(keys_diff[keys_name])
     if len(keys_diff["added"]) > 0:
         message += f"New violations found: {', '.join(keys_diff['added'])}\n{bad_msg}"
         for violation in keys_diff["added"]:
             violation_id = violation.split(" (")[0]
             message += new_results.generate_report(violation_id=violation_id)
```

### Comparing `pytest_axe_playwright_snapshot-0.0.5/tests/test_snapshot.py` & `pytest_axe_playwright_snapshot-0.0.6/tests/test_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     page.goto("https://www.example.com")
     try:
         axe_pytest_snapshot(page)
     except AssertionError as err:
         assert (
             str(err)
             == """\
-
 New violations found: html-has-lang (serious), landmark-one-main (moderate), region (moderate)
 That's bad news! 😱 Either fix the issue or run `pytest --snapshot-update` to update the snapshots.
 Rule Violated:
 html-has-lang - Ensures every HTML document has a lang attribute
 	URL: https://dequeuniversity.com/rules/axe/4.4/html-has-lang?application=axeAPI
 	Impact Level: serious
 	Tags: ['cat.language', 'wcag2a', 'wcag311', 'ACT']
@@ -61,15 +60,14 @@
     page.goto("https://www.example.com")
     try:
         axe_pytest_snapshot(page)
     except AssertionError as err:
         assert (
             str(err)
             == """\
-
 New violations found: html-has-lang (serious)
 That's bad news! 😱 Either fix the issue or run `pytest --snapshot-update` to update the snapshots.
 Rule Violated:
 html-has-lang - Ensures every HTML document has a lang attribute
 	URL: https://dequeuniversity.com/rules/axe/4.4/html-has-lang?application=axeAPI
 	Impact Level: serious
 	Tags: ['cat.language', 'wcag2a', 'wcag311', 'ACT']
@@ -88,30 +86,28 @@
     page.goto("https://www.example.com")
     try:
         axe_pytest_snapshot(page)
     except AssertionError as err:
         assert (
             str(err)
             == """\
-
 Old violations no longer found: color-contrast (moderate).
 That's good news! 🎉 Run `pytest --snapshot-update` to update the snapshots.
 """
         )
 
 
 def test_violations_more_instances(page: Page, axe_pytest_snapshot):
     page.goto("https://www.example.com")
     try:
         axe_pytest_snapshot(page)
     except AssertionError as err:
         assert (
             str(err)
             == """\
-
 Additional instances of existing violations were found: html-has-lang (serious)
 That's bad news! 😱 Either fix the issue or run `pytest --snapshot-update` to update the snapshots.
 Rule Violated:
 html-has-lang - Ensures every HTML document has a lang attribute
 	URL: https://dequeuniversity.com/rules/axe/4.4/html-has-lang?application=axeAPI
 	Impact Level: serious
 	Tags: ['cat.language', 'wcag2a', 'wcag311', 'ACT']
@@ -130,12 +126,11 @@
     page.goto("https://www.example.com")
     try:
         axe_pytest_snapshot(page)
     except AssertionError as err:
         assert (
             str(err)
             == """\
-
 Fewer instances of existing violations were found: region (moderate).
 That's good news! 🎉 Run `pytest --snapshot-update` to update the snapshots.
 """
         )
```

### Comparing `pytest_axe_playwright_snapshot-0.0.5/PKG-INFO` & `pytest_axe_playwright_snapshot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-axe-playwright-snapshot
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pytest plugin that runs Axe-core on Playwright pages and takes snapshots of the results.
 Author: Pamela Fox
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

