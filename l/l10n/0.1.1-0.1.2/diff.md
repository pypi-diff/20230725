# Comparing `tmp/l10n-0.1.1.tar.gz` & `tmp/l10n-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l10n-0.1.1.tar", last modified: Fri Mar 31 11:52:16 2023, max compression
+gzip compressed data, was "l10n-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `l10n-0.1.1.tar` & `l10n-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      710 2023-03-31 11:51:22.965953 l10n-0.1.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.1/.gitignore
--rw-r--r--   0        0        0      325 2023-03-31 11:51:22.965953 l10n-0.1.1/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2023-03-31 07:51:09.539905 l10n-0.1.1/LICENSE
--rw-r--r--   0        0        0     3338 2023-03-31 11:51:52.001555 l10n-0.1.1/README.md
--rw-r--r--   0        0        0     3358 2023-03-31 11:41:21.762235 l10n-0.1.1/Taskfile.yml
--rw-r--r--   0        0        0     9237 2023-03-31 11:51:22.965953 l10n-0.1.1/docs/advanced.md
--rw-r--r--   0        0        0      110 2023-03-31 11:41:21.762235 l10n-0.1.1/docs/api.md
--rw-r--r--   0        0        0      317 2023-03-31 11:41:21.762235 l10n-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      879 2023-03-31 11:51:02.630233 l10n-0.1.1/docs/index.md
--rw-r--r--   0        0        0     6540 2023-03-31 07:51:09.539905 l10n-0.1.1/docs/intro.md
--rw-r--r--   0        0        0     1070 2023-03-31 07:51:09.539905 l10n-0.1.1/docs/more.md
--rw-r--r--   0        0        0       77 2023-03-31 11:41:21.762235 l10n-0.1.1/docs/quickstart.md
--rw-r--r--   0        0        0     1355 2023-03-31 07:51:09.539905 l10n-0.1.1/docs/removed.md
--rw-r--r--   0        0        0       26 2023-03-31 07:51:09.539905 l10n-0.1.1/example-project/.gitignore
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.539905 l10n-0.1.1/example-project/example_project/__init__.py
--rw-r--r--   0        0        0       35 2023-03-31 11:41:21.762235 l10n-0.1.1/example-project/example_project/__main__.py
--rw-r--r--   0        0        0      461 2023-03-31 11:41:21.762235 l10n-0.1.1/example-project/example_project/example.py
--rw-r--r--   0        0        0      522 2023-03-31 07:51:09.539905 l10n-0.1.1/example-project/locales/en.po
--rw-r--r--   0        0        0      590 2023-03-31 07:51:09.539905 l10n-0.1.1/example-project/locales/ru.po
--rw-r--r--   0        0        0      262 2023-03-31 07:51:09.539905 l10n-0.1.1/example-project/pyproject.toml
--rw-r--r--   0        0        0      190 2023-03-31 11:52:02.101416 l10n-0.1.1/l10n/__init__.py
--rw-r--r--   0        0        0       44 2023-03-31 11:41:21.762235 l10n-0.1.1/l10n/__main__.py
--rw-r--r--   0        0        0      942 2023-03-31 07:51:09.539905 l10n-0.1.1/l10n/_cli.py
--rw-r--r--   0        0        0      335 2023-03-31 11:41:21.762235 l10n-0.1.1/l10n/_commands/__init__.py
--rw-r--r--   0        0        0      420 2023-03-31 11:41:21.762235 l10n-0.1.1/l10n/_commands/_base.py
--rw-r--r--   0        0        0     1920 2023-03-31 11:41:21.762235 l10n-0.1.1/l10n/_commands/_compile.py
--rw-r--r--   0        0        0     4258 2023-03-31 11:41:21.762235 l10n-0.1.1/l10n/_commands/_extract.py
--rw-r--r--   0        0        0     1775 2023-03-31 07:51:09.539905 l10n-0.1.1/l10n/_commands/_translate.py
--rw-r--r--   0        0        0     2686 2023-03-31 11:41:21.762235 l10n-0.1.1/l10n/_extractor.py
--rw-r--r--   0        0        0    12795 2023-03-31 11:41:21.762235 l10n-0.1.1/l10n/_locale.py
--rw-r--r--   0        0        0     3839 2023-03-31 07:51:09.539905 l10n-0.1.1/l10n/_locales.py
--rw-r--r--   0        0        0     3370 2023-03-31 10:58:20.498487 l10n-0.1.1/l10n/_plurals.py
--rw-r--r--   0        0        0     5170 2023-03-31 11:41:21.762235 l10n-0.1.1/l10n/_project.py
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.1/l10n/py.typed
--rw-r--r--   0        0        0      693 2023-03-31 07:51:09.543905 l10n-0.1.1/messages.po
--rwxr-xr-x   0        0        0      128 2023-03-31 11:51:22.965953 l10n-0.1.1/netlify.sh
--rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.1/netlify.toml
--rw-r--r--   0        0        0     2117 2023-03-31 11:41:21.762235 l10n-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       72 2023-03-31 11:41:21.762235 l10n-0.1.1/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      468 2023-03-31 11:41:21.762235 l10n-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.1/tests/test_commands/__init__.py
--rw-r--r--   0        0        0     1104 2023-03-31 11:41:21.762235 l10n-0.1.1/tests/test_commands/test_compile.py
--rw-r--r--   0        0        0     2724 2023-03-31 11:41:21.762235 l10n-0.1.1/tests/test_commands/test_extract.py
--rw-r--r--   0        0        0      854 2023-03-31 11:41:21.762235 l10n-0.1.1/tests/test_commands/test_translate.py
--rw-r--r--   0        0        0      309 2023-03-31 11:41:21.762235 l10n-0.1.1/tests/test_extractor.py
--rw-r--r--   0        0        0     6329 2023-03-31 11:41:21.762235 l10n-0.1.1/tests/test_locale.py
--rw-r--r--   0        0        0      708 2023-03-31 11:41:21.762235 l10n-0.1.1/tests/test_locales.py
--rw-r--r--   0        0        0     4912 1970-01-01 00:00:00.000000 l10n-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      710 2023-07-25 07:04:19.275434 l10n-0.1.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.2/.gitignore
+-rw-r--r--   0        0        0      325 2023-03-31 11:51:22.965953 l10n-0.1.2/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2023-03-31 07:51:09.539905 l10n-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3338 2023-03-31 11:51:52.001555 l10n-0.1.2/README.md
+-rw-r--r--   0        0        0     3358 2023-03-31 11:41:21.762235 l10n-0.1.2/Taskfile.yml
+-rw-r--r--   0        0        0     9237 2023-03-31 11:51:22.965953 l10n-0.1.2/docs/advanced.md
+-rw-r--r--   0        0        0      110 2023-03-31 11:41:21.762235 l10n-0.1.2/docs/api.md
+-rw-r--r--   0        0        0      317 2023-03-31 11:41:21.762235 l10n-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0      879 2023-03-31 11:51:02.630233 l10n-0.1.2/docs/index.md
+-rw-r--r--   0        0        0     6540 2023-03-31 07:51:09.539905 l10n-0.1.2/docs/intro.md
+-rw-r--r--   0        0        0     1070 2023-03-31 07:51:09.539905 l10n-0.1.2/docs/more.md
+-rw-r--r--   0        0        0       77 2023-03-31 11:41:21.762235 l10n-0.1.2/docs/quickstart.md
+-rw-r--r--   0        0        0     1355 2023-03-31 07:51:09.539905 l10n-0.1.2/docs/removed.md
+-rw-r--r--   0        0        0       26 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/.gitignore
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/example_project/__init__.py
+-rw-r--r--   0        0        0       35 2023-03-31 11:41:21.762235 l10n-0.1.2/example-project/example_project/__main__.py
+-rw-r--r--   0        0        0      461 2023-03-31 11:41:21.762235 l10n-0.1.2/example-project/example_project/example.py
+-rw-r--r--   0        0        0      522 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/locales/en.po
+-rw-r--r--   0        0        0      590 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/locales/ru.po
+-rw-r--r--   0        0        0      262 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-07-25 07:29:34.910563 l10n-0.1.2/l10n/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/__main__.py
+-rw-r--r--   0        0        0      942 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_cli.py
+-rw-r--r--   0        0        0      335 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_commands/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_commands/_base.py
+-rw-r--r--   0        0        0     1920 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_commands/_compile.py
+-rw-r--r--   0        0        0     4258 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_commands/_extract.py
+-rw-r--r--   0        0        0     1943 2023-07-25 07:29:34.910563 l10n-0.1.2/l10n/_commands/_translate.py
+-rw-r--r--   0        0        0     2686 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_extractor.py
+-rw-r--r--   0        0        0    12795 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_locale.py
+-rw-r--r--   0        0        0     3839 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_locales.py
+-rw-r--r--   0        0        0     3370 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_plurals.py
+-rw-r--r--   0        0        0     5170 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_project.py
+-rw-r--r--   0        0        0        0 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/py.typed
+-rw-r--r--   0        0        0      693 2023-03-31 07:51:09.543905 l10n-0.1.2/messages.po
+-rwxr-xr-x   0        0        0      128 2023-03-31 11:51:22.965953 l10n-0.1.2/netlify.sh
+-rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.2/netlify.toml
+-rw-r--r--   0        0        0     2117 2023-07-25 07:29:34.910563 l10n-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-03-31 11:41:21.762235 l10n-0.1.2/setup.cfg
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      468 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.2/tests/test_commands/__init__.py
+-rw-r--r--   0        0        0     1104 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_commands/test_compile.py
+-rw-r--r--   0        0        0     2724 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_commands/test_extract.py
+-rw-r--r--   0        0        0      854 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_commands/test_translate.py
+-rw-r--r--   0        0        0      309 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_extractor.py
+-rw-r--r--   0        0        0     6329 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_locale.py
+-rw-r--r--   0        0        0      708 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_locales.py
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 l10n-0.1.2/PKG-INFO
```

### Comparing `l10n-0.1.1/.github/workflows/main.yml` & `l10n-0.1.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/LICENSE` & `l10n-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/README.md` & `l10n-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/Taskfile.yml` & `l10n-0.1.2/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/docs/advanced.md` & `l10n-0.1.2/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/docs/index.md` & `l10n-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/docs/intro.md` & `l10n-0.1.2/docs/intro.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/docs/more.md` & `l10n-0.1.2/docs/more.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/docs/removed.md` & `l10n-0.1.2/docs/removed.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/example-project/locales/en.po` & `l10n-0.1.2/example-project/locales/en.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/example-project/locales/ru.po` & `l10n-0.1.2/example-project/locales/ru.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/l10n/_cli.py` & `l10n-0.1.2/l10n/_cli.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/l10n/_commands/_compile.py` & `l10n-0.1.2/l10n/_commands/_compile.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/l10n/_commands/_extract.py` & `l10n-0.1.2/l10n/_commands/_extract.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/l10n/_commands/_translate.py` & `l10n-0.1.2/l10n/_commands/_translate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from argparse import ArgumentParser
 from pathlib import Path
 
 import polib
-from googletrans import Translator
 
 from .._project import Project, find_project_root
 from ._base import Command
 
 
 class Translate(Command):
     """Translate all text without translation using Google Translate.
@@ -19,14 +18,20 @@
         )
         parser.add_argument(
             '--src-lang', default='en',
             help='the language used for messages (msgid)',
         )
 
     def run(self) -> int:
+        try:
+            from googletrans import Translator
+        except ImportError:
+            msg = 'Please, run `python3 -m pip install googletrans==4.0.0rc1`'
+            raise ImportError(msg)
+
         project_root = find_project_root(self.args.path)
         project = Project(project_root)
         translator = Translator()
         for po_path in project.po_root.iterdir():
             if po_path.suffix != '.po':
                 continue
             self.print(po_path.stem)
```

### Comparing `l10n-0.1.1/l10n/_extractor.py` & `l10n-0.1.2/l10n/_extractor.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/l10n/_locale.py` & `l10n-0.1.2/l10n/_locale.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/l10n/_locales.py` & `l10n-0.1.2/l10n/_locales.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/l10n/_plurals.py` & `l10n-0.1.2/l10n/_plurals.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/l10n/_project.py` & `l10n-0.1.2/l10n/_project.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/messages.po` & `l10n-0.1.2/messages.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/pyproject.toml` & `l10n-0.1.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 dependencies = []
 
 [project.optional-dependencies]
 cli = [
     "mypy",
     "tomli",
     "polib",
-    "googletrans==4.0.0rc1",
 ]
 test = [
-    "pytest",
+    "googletrans==4.0.0rc1",
     "pytest-cov",
     "pytest-xdist",
+    "pytest",
 ]
 lint = [
     "flake8-length",
     "flake8",
     "isort",
     "mypy",
     "types-polib",
```

### Comparing `l10n-0.1.1/tests/test_commands/test_compile.py` & `l10n-0.1.2/tests/test_commands/test_compile.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/tests/test_commands/test_extract.py` & `l10n-0.1.2/tests/test_commands/test_extract.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/tests/test_commands/test_translate.py` & `l10n-0.1.2/tests/test_commands/test_translate.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/tests/test_locale.py` & `l10n-0.1.2/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/tests/test_locales.py` & `l10n-0.1.2/tests/test_locales.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.1/PKG-INFO` & `l10n-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l10n
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library and CLI for translating Python applications and libraries.
 Keywords: localization,internationalization,l10n,i18n,locale,locales,translation,gettext
 Author-email: Gram <gram@orsinium.dev>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,27 +14,27 @@
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Typing :: Typed
 Requires-Dist: mypy ; extra == "cli"
 Requires-Dist: tomli ; extra == "cli"
 Requires-Dist: polib ; extra == "cli"
-Requires-Dist: googletrans==4.0.0rc1 ; extra == "cli"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: flake8-length ; extra == "lint"
 Requires-Dist: flake8 ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: types-polib ; extra == "lint"
 Requires-Dist: types-toml ; extra == "lint"
 Requires-Dist: unify ; extra == "lint"
-Requires-Dist: pytest ; extra == "test"
+Requires-Dist: googletrans==4.0.0rc1 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-xdist ; extra == "test"
+Requires-Dist: pytest ; extra == "test"
 Project-URL: Source, https://github.com/orsinium-labs/l10n
 Provides-Extra: cli
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: test
 
 # l10n
```

