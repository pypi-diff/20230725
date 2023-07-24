# Comparing `tmp/axe_playwright_python-0.1.1.tar.gz` & `tmp/axe_playwright_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axe_playwright_python-0.1.1.tar", max compression
+gzip compressed data, was "axe_playwright_python-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `axe_playwright_python-0.1.1.tar` & `axe_playwright_python-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,28 @@
--rw-r--r--   0        0        0     1081 2023-07-20 18:37:43.617118 axe_playwright_python-0.1.1/LICENSE
--rw-r--r--   0        0        0     1108 2023-07-20 20:46:37.115996 axe_playwright_python-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-04-03 13:02:19.820719 axe_playwright_python-0.1.1/axe_playwright_python/__init__.py
--rw-r--r--   0        0        0     1243 2023-07-20 18:37:43.618990 axe_playwright_python-0.1.1/axe_playwright_python/async_playwright.py
--rw-r--r--   0        0        0   436082 2023-04-03 13:02:19.822321 axe_playwright_python-0.1.1/axe_playwright_python/axe.min.js
--rw-r--r--   0        0        0     4343 2023-07-20 18:37:43.619790 axe_playwright_python-0.1.1/axe_playwright_python/base.py
--rw-r--r--   0        0        0     1222 2023-07-20 18:37:43.621985 axe_playwright_python-0.1.1/axe_playwright_python/sync_playwright.py
--rw-r--r--   0        0        0      131 2023-07-20 18:37:43.622614 axe_playwright_python-0.1.1/axe_playwright_python/violations.txt
--rw-r--r--   0        0        0     1226 2023-07-20 20:47:23.505775 axe_playwright_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 axe_playwright_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      922 2023-07-24 22:02:57.751373 axe_playwright_python-0.1.2/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2023-04-03 13:02:19.819263 axe_playwright_python-0.1.2/.gitignore
+-rw-r--r--   0        0        0      405 2023-07-24 22:01:27.106479 axe_playwright_python-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       80 2023-04-03 13:02:19.819796 axe_playwright_python-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      502 2023-07-24 22:01:27.107296 axe_playwright_python-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1081 2023-07-20 18:37:43.617118 axe_playwright_python-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1360 2023-07-23 19:33:50.981062 axe_playwright_python-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-23 23:53:48.558073 axe_playwright_python-0.1.2/axe_playwright_python/__init__.py
+-rw-r--r--   0        0        0     1279 2023-07-24 22:07:26.775328 axe_playwright_python-0.1.2/axe_playwright_python/async_playwright.py
+-rw-r--r--   0        0        0   436082 2023-04-03 13:02:19.822321 axe_playwright_python-0.1.2/axe_playwright_python/axe.min.js
+-rw-r--r--   0        0        0     4356 2023-07-24 21:57:47.671531 axe_playwright_python-0.1.2/axe_playwright_python/base.py
+-rw-r--r--   0        0        0     1257 2023-07-24 22:07:15.194045 axe_playwright_python-0.1.2/axe_playwright_python/sync_playwright.py
+-rw-r--r--   0        0        0      116 2023-07-23 19:30:24.470962 axe_playwright_python-0.1.2/axe_playwright_python/violations.txt
+-rw-r--r--   0        0        0      101 2023-07-20 18:37:43.623671 axe_playwright_python-0.1.2/docs/api.md
+-rw-r--r--   0        0        0      693 2023-07-20 21:02:33.627100 axe_playwright_python-0.1.2/docs/index.md
+-rw-r--r--   0        0        0     2383 2023-07-20 18:37:43.624812 axe_playwright_python-0.1.2/docs/usage.md
+-rw-r--r--   0        0        0      309 2023-07-23 19:41:06.816546 axe_playwright_python-0.1.2/examples/usage.py
+-rw-r--r--   0        0        0      840 2023-07-20 18:38:30.351452 axe_playwright_python-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0     1675 2023-07-24 21:59:37.138277 axe_playwright_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 13:02:19.828070 axe_playwright_python-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2198 2023-07-23 19:40:35.377787 axe_playwright_python-0.1.2/tests/test_axe_async_playwright.py
+-rw-r--r--   0        0        0     1945 2023-07-23 19:40:35.377772 axe_playwright_python-0.1.2/tests/test_axe_sync_playwright.py
+-rw-r--r--   0        0        0      379 2023-04-03 13:02:19.829198 axe_playwright_python-0.1.2/tests/test_page.html
+-rw-r--r--   0        0        0    32280 2023-07-23 19:31:34.275874 axe_playwright_python-0.1.2/tests/test_report.txt
+-rw-r--r--   0        0        0     9220 2023-07-23 19:31:27.259500 axe_playwright_python-0.1.2/tests/test_report_color.txt
+-rw-r--r--   0        0        0     2212 2023-07-23 19:41:06.826891 axe_playwright_python-0.1.2/tests/test_report_save.py
+-rw-r--r--   0        0        0   412591 2023-07-20 18:37:43.632179 axe_playwright_python-0.1.2/tests/test_result.json
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 axe_playwright_python-0.1.2/PKG-INFO
```

### Comparing `axe_playwright_python-0.1.1/LICENSE` & `axe_playwright_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.1/README.md` & `axe_playwright_python-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# axe-python-playwright
+# axe-playwright-python
 
 Automated web accessibility testing using [axe-core](https://github.com/dequelabs/axe-core) engine
 and [Playwright](https://playwright.dev/python/docs/intro).
 
 ## Documentation
 
 - [Full documentation](https://pamelafox.github.io/axe-playwright-python/).
 
-## Requirements
+## Dependencies
 
 - Python >= 3.10
 - [playwright](https://github.com/microsoft/playwright-python) >= 1.25.0
 
 ## Installation
 
 ```console
@@ -38,8 +38,12 @@
 print(f"Full axe-core response: {results.response}")
 ```
 
 For more examples see [documentation](https://pamelafox.github.io/axe-playwright-python/).
 
 ## Contributing
 
-See [guide on contributing](CONTRIBUTING.md).
+See [guide on contributing](CONTRIBUTING.md).
+
+## Acknowledgments
+
+This project is based on [axe-core-python](https://github.com/ruslan-rv-ua/axe-core-python) by @ruslan-rv-ua and also takes inspiration from [axe-selenium-python](https://pypi.org/project/axe-selenium-python/) for output formats.
```

### Comparing `axe_playwright_python-0.1.1/axe_playwright_python/async_playwright.py` & `axe_playwright_python-0.1.2/axe_playwright_python/async_playwright.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from .base import AxeBase, AxeResults
 
 DEFAULT_OPTIONS = {"resultTypes": ["violations"]}
 
 
 class Axe(AxeBase):
     async def run(
```

### Comparing `axe_playwright_python-0.1.1/axe_playwright_python/axe.min.js` & `axe_playwright_python-0.1.2/axe_playwright_python/axe.min.js`

 * *Files identical despite different names*

### Comparing `axe_playwright_python-0.1.1/axe_playwright_python/base.py` & `axe_playwright_python-0.1.2/axe_playwright_python/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
+
+import json
+import os
 from abc import ABC, abstractmethod
 from pathlib import Path
-import os
-import json
 from string import Template
 
-
 AXE_FILE_NAME = "axe.min.js"
 AXE_FILE_PATH = Path(__file__).parent / AXE_FILE_NAME
 
 AXE_SCRIPT = AXE_FILE_PATH.read_text()
 
 
 class AxeBase(ABC):
@@ -39,62 +40,61 @@
         return args
 
     @abstractmethod
     def run(self):
         pass
 
     @classmethod
-    def from_file(cls, axe_min_js_path: str | Path) -> "AxeBase":
+    def from_file(cls, axe_min_js_path: str | Path) -> AxeBase:
         """Load axe script from file and create Axe instance.
 
         Args:
             axe_min_js_path (str | Path): path to `axe.js` or `axe.min.js`
 
         Returns:
             AxeBase: Axe instance
         """
         axe_script = Path(axe_min_js_path).read_text(encoding="UTF-8")
         return cls(axe_script=axe_script)
 
 
-class AxeResults():
-
+class AxeResults:
     def __init__(self, response: dict):
         self.response = response
 
     @property
     def violations_count(self) -> int:
         """
         Number of violations found.
         """
-        return len(self.response['violations'])
+        return len(self.response["violations"])
 
     def generate_snapshot(self):
         """
         Return snapshot of violations, for use in snapshot testing.
         Format:
         <violation-id> (impact) : <number-of-nodes>
         """
         snapshot_lines = []
-        for v in self.response['violations']:
+        for v in self.response["violations"]:
             snapshot_lines.append(f"{v['id']} ({v['impact']}) : {len(v['nodes'])}")
-        return '\n'.join(snapshot_lines)
+        return "\n".join(snapshot_lines)
 
     def __violation_report(self, violation: dict, template: Template) -> str:
         nodes_str = ""
         for num, node in enumerate(violation["nodes"], start=1):
-            targets = ', '.join(node["target"])
+            targets = ", ".join(node["target"])
             nodes_str += f"\n\n\t{num})\tTarget: {targets}"
-            snippet = node.get('html').replace('\n', '')
+            snippet = node.get("html").replace("\n", "")
             nodes_str += f"\n\t\tSnippet: {snippet}"
             nodes_str += "\n\t\tMessages:"
             for item in node.get("all", []) + node.get("any", []) + node.get("none", []):
                 nodes_str += "\n\t\t* " + item["message"]
         return template.substitute(violation, elements=nodes_str)
-    
+
     def generate_report(self, violation_id: str | None = None) -> str:
         """
         Return readable report of accessibility violations found.
         Defaults to all violations, but can be filtered by violation ID.
         @param violation_id: Violation ID to report on
         """
         violations = self.response["violations"]
@@ -105,26 +105,25 @@
         template = Template(tmpl_f.read())
         tmpl_f.close()
         for violation in violations:
             if violation_id is not None and violation_id != violation["id"]:
                 continue
             report_str += self.__violation_report(violation, template)
         return report_str
-    
-    def save_to_file(self, file_path: str | Path | None = None,
-                     violations_only: bool = False) -> None:
+
+    def save_to_file(
+        self, file_path: str | Path | None = None, violations_only: bool = False
+    ) -> None:
         """Save results to file.
         @param results: Results from Axe analysis
         @param file_path: File path for saving results file
         """
         # create a copy of the dict
         response = self.response.copy()
         if violations_only:
             del response["inapplicable"]
             del response["incomplete"]
             del response["passes"]
         if file_path is None:
             cwd = Path.cwd()
             file_path = cwd / "results.json"
         Path(file_path).write_text(json.dumps(response, indent=4))
-
-
```

### Comparing `axe_playwright_python-0.1.1/axe_playwright_python/sync_playwright.py` & `axe_playwright_python-0.1.2/axe_playwright_python/sync_playwright.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from .base import AxeBase, AxeResults
 
 DEFAULT_OPTIONS = {"resultTypes": ["violations"]}
 
 
 class Axe(AxeBase):
     def run(
@@ -15,15 +17,15 @@
         Args:
             page (playwright.sync_api._generated.Page): Page object
             context (str | list | dict | None, optional): context.
                 Defaults to None.
             options (dict | None, optional): options.
                 Defaults to {"resultTypes": ["violations"]}.
 
-        For more information on `context` and `options`, 
+        For more information on `context` and `options`,
             view the [axe-core documentation]().
 
         Returns:
             dict: test result
         """
 
         # inject `Axe` into document
```

