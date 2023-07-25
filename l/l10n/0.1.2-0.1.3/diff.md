# Comparing `tmp/l10n-0.1.2.tar.gz` & `tmp/l10n-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l10n-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "l10n-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `l10n-0.1.2.tar` & `l10n-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      710 2023-07-25 07:04:19.275434 l10n-0.1.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.2/.gitignore
--rw-r--r--   0        0        0      325 2023-03-31 11:51:22.965953 l10n-0.1.2/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2023-03-31 07:51:09.539905 l10n-0.1.2/LICENSE
--rw-r--r--   0        0        0     3338 2023-03-31 11:51:52.001555 l10n-0.1.2/README.md
--rw-r--r--   0        0        0     3358 2023-03-31 11:41:21.762235 l10n-0.1.2/Taskfile.yml
--rw-r--r--   0        0        0     9237 2023-03-31 11:51:22.965953 l10n-0.1.2/docs/advanced.md
--rw-r--r--   0        0        0      110 2023-03-31 11:41:21.762235 l10n-0.1.2/docs/api.md
--rw-r--r--   0        0        0      317 2023-03-31 11:41:21.762235 l10n-0.1.2/docs/conf.py
--rw-r--r--   0        0        0      879 2023-03-31 11:51:02.630233 l10n-0.1.2/docs/index.md
--rw-r--r--   0        0        0     6540 2023-03-31 07:51:09.539905 l10n-0.1.2/docs/intro.md
--rw-r--r--   0        0        0     1070 2023-03-31 07:51:09.539905 l10n-0.1.2/docs/more.md
--rw-r--r--   0        0        0       77 2023-03-31 11:41:21.762235 l10n-0.1.2/docs/quickstart.md
--rw-r--r--   0        0        0     1355 2023-03-31 07:51:09.539905 l10n-0.1.2/docs/removed.md
--rw-r--r--   0        0        0       26 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/.gitignore
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/example_project/__init__.py
--rw-r--r--   0        0        0       35 2023-03-31 11:41:21.762235 l10n-0.1.2/example-project/example_project/__main__.py
--rw-r--r--   0        0        0      461 2023-03-31 11:41:21.762235 l10n-0.1.2/example-project/example_project/example.py
--rw-r--r--   0        0        0      522 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/locales/en.po
--rw-r--r--   0        0        0      590 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/locales/ru.po
--rw-r--r--   0        0        0      262 2023-03-31 07:51:09.539905 l10n-0.1.2/example-project/pyproject.toml
--rw-r--r--   0        0        0      190 2023-07-25 07:29:34.910563 l10n-0.1.2/l10n/__init__.py
--rw-r--r--   0        0        0       44 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/__main__.py
--rw-r--r--   0        0        0      942 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_cli.py
--rw-r--r--   0        0        0      335 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_commands/__init__.py
--rw-r--r--   0        0        0      420 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_commands/_base.py
--rw-r--r--   0        0        0     1920 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_commands/_compile.py
--rw-r--r--   0        0        0     4258 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_commands/_extract.py
--rw-r--r--   0        0        0     1943 2023-07-25 07:29:34.910563 l10n-0.1.2/l10n/_commands/_translate.py
--rw-r--r--   0        0        0     2686 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_extractor.py
--rw-r--r--   0        0        0    12795 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_locale.py
--rw-r--r--   0        0        0     3839 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_locales.py
--rw-r--r--   0        0        0     3370 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_plurals.py
--rw-r--r--   0        0        0     5170 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/_project.py
--rw-r--r--   0        0        0        0 2023-07-25 07:24:06.837236 l10n-0.1.2/l10n/py.typed
--rw-r--r--   0        0        0      693 2023-03-31 07:51:09.543905 l10n-0.1.2/messages.po
--rwxr-xr-x   0        0        0      128 2023-03-31 11:51:22.965953 l10n-0.1.2/netlify.sh
--rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.2/netlify.toml
--rw-r--r--   0        0        0     2117 2023-07-25 07:29:34.910563 l10n-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       72 2023-03-31 11:41:21.762235 l10n-0.1.2/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      468 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.2/tests/test_commands/__init__.py
--rw-r--r--   0        0        0     1104 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_commands/test_compile.py
--rw-r--r--   0        0        0     2724 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_commands/test_extract.py
--rw-r--r--   0        0        0      854 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_commands/test_translate.py
--rw-r--r--   0        0        0      309 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_extractor.py
--rw-r--r--   0        0        0     6329 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_locale.py
--rw-r--r--   0        0        0      708 2023-03-31 11:41:21.762235 l10n-0.1.2/tests/test_locales.py
--rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 l10n-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      710 2023-07-25 07:04:19.275434 l10n-0.1.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.3/.gitignore
+-rw-r--r--   0        0        0      325 2023-03-31 11:51:22.965953 l10n-0.1.3/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2023-03-31 07:51:09.539905 l10n-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3338 2023-03-31 11:51:52.001555 l10n-0.1.3/README.md
+-rw-r--r--   0        0        0     3358 2023-03-31 11:41:21.762235 l10n-0.1.3/Taskfile.yml
+-rw-r--r--   0        0        0     9237 2023-03-31 11:51:22.965953 l10n-0.1.3/docs/advanced.md
+-rw-r--r--   0        0        0      110 2023-03-31 11:41:21.762235 l10n-0.1.3/docs/api.md
+-rw-r--r--   0        0        0      317 2023-03-31 11:41:21.762235 l10n-0.1.3/docs/conf.py
+-rw-r--r--   0        0        0      879 2023-03-31 11:51:02.630233 l10n-0.1.3/docs/index.md
+-rw-r--r--   0        0        0     6540 2023-03-31 07:51:09.539905 l10n-0.1.3/docs/intro.md
+-rw-r--r--   0        0        0     1070 2023-03-31 07:51:09.539905 l10n-0.1.3/docs/more.md
+-rw-r--r--   0        0        0       77 2023-03-31 11:41:21.762235 l10n-0.1.3/docs/quickstart.md
+-rw-r--r--   0        0        0     1355 2023-03-31 07:51:09.539905 l10n-0.1.3/docs/removed.md
+-rw-r--r--   0        0        0       26 2023-03-31 07:51:09.539905 l10n-0.1.3/example-project/.gitignore
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.539905 l10n-0.1.3/example-project/example_project/__init__.py
+-rw-r--r--   0        0        0       35 2023-03-31 11:41:21.762235 l10n-0.1.3/example-project/example_project/__main__.py
+-rw-r--r--   0        0        0      461 2023-03-31 11:41:21.762235 l10n-0.1.3/example-project/example_project/example.py
+-rw-r--r--   0        0        0      522 2023-03-31 07:51:09.539905 l10n-0.1.3/example-project/locales/en.po
+-rw-r--r--   0        0        0      590 2023-03-31 07:51:09.539905 l10n-0.1.3/example-project/locales/ru.po
+-rw-r--r--   0        0        0      262 2023-03-31 07:51:09.539905 l10n-0.1.3/example-project/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-07-25 08:09:23.545901 l10n-0.1.3/l10n/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/__main__.py
+-rw-r--r--   0        0        0      942 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/_cli.py
+-rw-r--r--   0        0        0      335 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/_commands/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/_commands/_base.py
+-rw-r--r--   0        0        0     1920 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/_commands/_compile.py
+-rw-r--r--   0        0        0     4867 2023-07-25 08:09:21.425920 l10n-0.1.3/l10n/_commands/_extract.py
+-rw-r--r--   0        0        0     1943 2023-07-25 07:29:34.910563 l10n-0.1.3/l10n/_commands/_translate.py
+-rw-r--r--   0        0        0     2824 2023-07-25 08:09:21.425920 l10n-0.1.3/l10n/_extractor.py
+-rw-r--r--   0        0        0    12795 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/_locale.py
+-rw-r--r--   0        0        0     3839 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/_locales.py
+-rw-r--r--   0        0        0     3370 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/_plurals.py
+-rw-r--r--   0        0        0     5170 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/_project.py
+-rw-r--r--   0        0        0        0 2023-07-25 07:24:06.837236 l10n-0.1.3/l10n/py.typed
+-rw-r--r--   0        0        0      693 2023-03-31 07:51:09.543905 l10n-0.1.3/messages.po
+-rwxr-xr-x   0        0        0      128 2023-03-31 11:51:22.965953 l10n-0.1.3/netlify.sh
+-rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.3/netlify.toml
+-rw-r--r--   0        0        0     2117 2023-07-25 07:29:34.910563 l10n-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-03-31 11:41:21.762235 l10n-0.1.3/setup.cfg
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      468 2023-03-31 11:41:21.762235 l10n-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.3/tests/test_commands/__init__.py
+-rw-r--r--   0        0        0     1104 2023-03-31 11:41:21.762235 l10n-0.1.3/tests/test_commands/test_compile.py
+-rw-r--r--   0        0        0     2724 2023-03-31 11:41:21.762235 l10n-0.1.3/tests/test_commands/test_extract.py
+-rw-r--r--   0        0        0      854 2023-03-31 11:41:21.762235 l10n-0.1.3/tests/test_commands/test_translate.py
+-rw-r--r--   0        0        0      309 2023-03-31 11:41:21.762235 l10n-0.1.3/tests/test_extractor.py
+-rw-r--r--   0        0        0     6329 2023-03-31 11:41:21.762235 l10n-0.1.3/tests/test_locale.py
+-rw-r--r--   0        0        0      708 2023-03-31 11:41:21.762235 l10n-0.1.3/tests/test_locales.py
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 l10n-0.1.3/PKG-INFO
```

### Comparing `l10n-0.1.2/.github/workflows/main.yml` & `l10n-0.1.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/LICENSE` & `l10n-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/README.md` & `l10n-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/Taskfile.yml` & `l10n-0.1.3/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/docs/advanced.md` & `l10n-0.1.3/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/docs/index.md` & `l10n-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/docs/intro.md` & `l10n-0.1.3/docs/intro.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/docs/more.md` & `l10n-0.1.3/docs/more.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/docs/removed.md` & `l10n-0.1.3/docs/removed.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/example-project/locales/en.po` & `l10n-0.1.3/example-project/locales/en.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/example-project/locales/ru.po` & `l10n-0.1.3/example-project/locales/ru.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/l10n/_cli.py` & `l10n-0.1.3/l10n/_cli.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/l10n/_commands/_compile.py` & `l10n-0.1.3/l10n/_commands/_compile.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/l10n/_commands/_extract.py` & `l10n-0.1.3/l10n/_commands/_extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,17 +26,25 @@
             help='path to the project root directory',
         )
         parser.add_argument(
             '--lang',
             help='language to generate a PO file for',
         )
         parser.add_argument(
+            '--wrap', default=90, type=int,
+            help='wrap msgstr longer than that many characters',
+        )
+        parser.add_argument(
             '--echo', action='store_true',
             help='set msgstr to the same value as msgid',
         )
+        parser.add_argument(
+            '--allow-duplicates', action='store_true',
+            help='do not check the file for duplicates',
+        )
         now = datetime.now(timezone.utc).astimezone()
         parser.add_argument(
             '--now', default=now.isoformat(),
             help='the current time in ISO format'
         )
 
     def run(self) -> int:
@@ -53,18 +61,25 @@
         for root, entries in files.items():
             project = Project(root)
             project.po_root.mkdir(exist_ok=True)
             for lang in self._langs_for(project):
                 self.print(lang)
                 file_path = project.po_root / f'{lang}.po'
 
-                template_file = polib.POFile()
+                template_file = polib.POFile(
+                    wrapwidth=self.args.wrap,
+                    check_for_duplicates=not self.args.allow_duplicates,
+                )
                 template_file.extend(entries)
                 if file_path.exists():
-                    target_file = polib.pofile(str(file_path))
+                    target_file = polib.pofile(
+                        str(file_path),
+                        wrapwidth=self.args.wrap,
+                        check_for_duplicates=not self.args.allow_duplicates,
+                    )
                     target_file.merge(template_file)
                 else:
                     target_file = template_file
                 self._set_meta(project, target_file, lang)
                 target_file.save(str(file_path))
                 self.print(f'  extracted: {len(entries)}')
         return 0
```

### Comparing `l10n-0.1.2/l10n/_commands/_translate.py` & `l10n-0.1.3/l10n/_commands/_translate.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/l10n/_extractor.py` & `l10n-0.1.3/l10n/_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from __future__ import annotations
 
 import json
 import subprocess
 import sys
 from pathlib import Path
 from tempfile import NamedTemporaryFile
+from textwrap import dedent
 from typing import Iterator, NamedTuple
 
 from mypy import types
 from mypy.plugin import MethodContext, Plugin
 from mypy.types import LiteralValue
 
 
 PREFIX = '__L10N__:'
+CONFIG = f"""
+    [mypy]
+    plugins = {__name__}
+    follow_imports = skip
+
+    [mypy-l10n.*]
+    follow_imports = normal
+"""
 
 
 class Message(NamedTuple):
     text: str
     line: int
     column: int
     n: int | None
@@ -27,15 +36,15 @@
 
     @property
     def path(self) -> Path:
         return Path(self.file_name)
 
 
 def extract_messages(project_path: Path) -> Iterator[Message]:
-    config = f'[mypy]\nplugins = {__name__}'
+    config = dedent(CONFIG)
     with NamedTemporaryFile() as tmp_file:
         tmp_file.write(config.encode())
         tmp_file.flush()
         cmd = [
             sys.executable, '-m', 'mypy',
             '--no-incremental',
             '--show-traceback',
```

### Comparing `l10n-0.1.2/l10n/_locale.py` & `l10n-0.1.3/l10n/_locale.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/l10n/_locales.py` & `l10n-0.1.3/l10n/_locales.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/l10n/_plurals.py` & `l10n-0.1.3/l10n/_plurals.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/l10n/_project.py` & `l10n-0.1.3/l10n/_project.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/messages.po` & `l10n-0.1.3/messages.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/pyproject.toml` & `l10n-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/tests/test_commands/test_compile.py` & `l10n-0.1.3/tests/test_commands/test_compile.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/tests/test_commands/test_extract.py` & `l10n-0.1.3/tests/test_commands/test_extract.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/tests/test_commands/test_translate.py` & `l10n-0.1.3/tests/test_commands/test_translate.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/tests/test_locale.py` & `l10n-0.1.3/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/tests/test_locales.py` & `l10n-0.1.3/tests/test_locales.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.2/PKG-INFO` & `l10n-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l10n
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library and CLI for translating Python applications and libraries.
 Keywords: localization,internationalization,l10n,i18n,locale,locales,translation,gettext
 Author-email: Gram <gram@orsinium.dev>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

