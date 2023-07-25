# Comparing `tmp/scanpydoc-0.9.3.tar.gz` & `tmp/scanpydoc-0.9.4.tar.gz`

## Comparing `scanpydoc-0.9.3.tar` & `scanpydoc-0.9.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.editorconfig
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.prettierrc.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.readthedocs.yml
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.vscode/settings.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/docs/conf.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/docs/index.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/_version.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/autosummary_generate_imported.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/definition_list_typed_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/py.typed
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/autodoc_patch.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/example.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/formatting.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/return_tuple.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/static/typehints.css
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/rtd_github_links/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/rtd_github_links/_linkcode.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/theme/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/theme/layout.html
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/theme/theme.conf
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/theme/static/styles/scanpy.css
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/conftest.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/test_base.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/test_definition_list_typed_field.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/test_elegant_typehints.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/test_rtd_github_links.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.gitignore
--rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/LICENSE
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/README.rst
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/.editorconfig
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/.prettierrc.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/.readthedocs.yml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/.vscode/settings.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/docs/conf.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/docs/index.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/_version.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/autosummary_generate_imported.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/definition_list_typed_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/py.typed
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/__init__.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/autodoc_patch.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/example.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/formatting.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/return_tuple.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/static/typehints.css
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/rtd_github_links/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/rtd_github_links/_linkcode.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/theme/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/theme/layout.html
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/theme/theme.conf
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/src/scanpydoc/theme/static/styles/scanpy.css
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/tests/test_base.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/tests/test_definition_list_typed_field.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/tests/test_elegant_typehints.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/tests/test_rtd_github_links.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/.gitignore
+-rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/README.rst
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 scanpydoc-0.9.4/PKG-INFO
```

### Comparing `scanpydoc-0.9.3/.pre-commit-config.yaml` & `scanpydoc-0.9.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       - id: trailing-whitespace
   - repo: https://github.com/psf/black
     rev: "23.7.0"
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.278
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: ["--fix"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0
     hooks:
       - id: prettier
```

### Comparing `scanpydoc-0.9.3/.github/workflows/ci.yml` & `scanpydoc-0.9.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/.github/workflows/publish.yml` & `scanpydoc-0.9.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/docs/conf.py` & `scanpydoc-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/docs/_templates/autosummary/module.rst` & `scanpydoc-0.9.4/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/__init__.py` & `scanpydoc-0.9.4/src/scanpydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/autosummary_generate_imported.py` & `scanpydoc-0.9.4/src/scanpydoc/autosummary_generate_imported.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/definition_list_typed_field.py` & `scanpydoc-0.9.4/src/scanpydoc/definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/__init__.py` & `scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/autodoc_patch.py` & `scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/autodoc_patch.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/formatting.py` & `scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/formatting.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/return_tuple.py` & `scanpydoc-0.9.4/src/scanpydoc/elegant_typehints/return_tuple.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/rtd_github_links/__init__.py` & `scanpydoc-0.9.4/src/scanpydoc/rtd_github_links/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/rtd_github_links/_linkcode.py` & `scanpydoc-0.9.4/src/scanpydoc/rtd_github_links/_linkcode.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/theme/__init__.py` & `scanpydoc-0.9.4/src/scanpydoc/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/theme/layout.html` & `scanpydoc-0.9.4/src/scanpydoc/theme/layout.html`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/src/scanpydoc/theme/theme.conf` & `scanpydoc-0.9.4/src/scanpydoc/theme/theme.conf`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/tests/conftest.py` & `scanpydoc-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/tests/test_base.py` & `scanpydoc-0.9.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/tests/test_definition_list_typed_field.py` & `scanpydoc-0.9.4/tests/test_definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/tests/test_elegant_typehints.py` & `scanpydoc-0.9.4/tests/test_elegant_typehints.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/tests/test_rtd_github_links.py` & `scanpydoc-0.9.4/tests/test_rtd_github_links.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/LICENSE` & `scanpydoc-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/README.rst` & `scanpydoc-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.3/pyproject.toml` & `scanpydoc-0.9.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,18 @@
     'pytest-cov',
 ]
 doc = [
     'scanpydoc[typehints,theme]',
     'sphinx',
 ]
 typehints = ['sphinx-autodoc-typehints>=1.15.2']
-theme = ['sphinx-book-theme>=1.0.1']
+theme = [
+    'sphinx-book-theme>=1.0.1',
+    'docutils>=0.8,!=0.18.*,!=0.19.*',
+]
 
 [project.entry-points.'sphinx.html_themes']
 scanpydoc = 'scanpydoc.theme'
 
 [tool.ruff]
 select = [
     'E', 'W', # Pycodestyle
```

### Comparing `scanpydoc-0.9.3/PKG-INFO` & `scanpydoc-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanpydoc
-Version: 0.9.3
+Version: 0.9.4
 Summary: A series of Sphinx extensions to get maintainable numpydoc style documentation.
 Project-URL: Source, https://github.com/theislab/scanpydoc/
 Project-URL: Documentation, https://icb-scanpydoc.readthedocs-hosted.com/
 Author-email: Philipp Angerer <phil.angerer@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Sphinx :: Extension
@@ -19,14 +19,15 @@
 Provides-Extra: doc
 Requires-Dist: scanpydoc[theme,typehints]; extra == 'doc'
 Requires-Dist: sphinx; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Provides-Extra: theme
+Requires-Dist: docutils!=0.18.*,!=0.19.*,>=0.8; extra == 'theme'
 Requires-Dist: sphinx-book-theme>=1.0.1; extra == 'theme'
 Provides-Extra: typehints
 Requires-Dist: sphinx-autodoc-typehints>=1.15.2; extra == 'typehints'
 Description-Content-Type: text/x-rst
 
 scanpydoc |pypi| |docs| |tests| |checks| |cov|
 ==============================================
```

