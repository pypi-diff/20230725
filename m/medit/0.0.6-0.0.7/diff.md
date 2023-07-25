# Comparing `tmp/medit-0.0.6.tar.gz` & `tmp/medit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medit-0.0.6.tar", max compression
+gzip compressed data, was "medit-0.0.7.tar", max compression
```

## Comparing `medit-0.0.6.tar` & `medit-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3100 2023-07-03 07:44:20.904244 medit-0.0.6/Readme.md
--rw-r--r--   0        0        0        0 2023-06-16 07:35:55.912297 medit-0.0.6/medit/__init__.py
--rwxr-xr-x   0        0        0     2192 2023-07-03 06:21:56.302488 medit-0.0.6/medit/cli.py
--rw-r--r--   0        0        0     2362 2023-07-03 06:51:24.784057 medit-0.0.6/medit/medit.ui
--rw-r--r--   0        0        0     5067 2023-07-04 06:15:16.074437 medit-0.0.6/medit/meditor.py
--rw-r--r--   0        0        0     7517 2023-07-03 06:21:56.302488 medit-0.0.6/medit/mview.py
--rw-r--r--   0        0        0        0 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/__init__.py
--rw-r--r--   0        0        0    18966 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/github-markdown-dark.css
--rw-r--r--   0        0        0    18979 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/github-markdown-light.css
--rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/pygments-solarized-style/solarized-dark.css
--rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/pygments-solarized-style/solarized-light.css
--rw-r--r--   0        0        0    36899 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/solarized-dark-all-sites.css
--rw-r--r--   0        0        0    36890 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/solarized-light-all-sites.css
--rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/thomasf-solarized-css/solarized-dark.css
--rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/thomasf-solarized-css/solarized-light.css
--rwxr-xr-x   0        0        0     8700 2023-07-04 06:36:24.786456 medit-0.0.6/medit/ui.py
--rw-r--r--   0        0        0     5361 2023-07-04 06:15:16.098475 medit-0.0.6/medit/utils.py
--rwxr-xr-x   0        0        0     6266 2023-06-29 19:10:09.897127 medit-0.0.6/medit/yatl.py
--rw-r--r--   0        0        0     2315 2023-07-04 06:37:03.356763 medit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 medit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3231 2023-07-25 14:15:03.192269 medit-0.0.7/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-16 07:35:55.912297 medit-0.0.7/medit/__init__.py
+-rwxr-xr-x   0        0        0     2192 2023-07-03 06:21:56.302488 medit-0.0.7/medit/cli.py
+-rw-r--r--   0        0        0     2362 2023-07-03 06:51:24.784057 medit-0.0.7/medit/medit.ui
+-rw-r--r--   0        0        0     5067 2023-07-04 06:15:16.074437 medit-0.0.7/medit/meditor.py
+-rw-r--r--   0        0        0     7879 2023-07-25 14:12:18.736105 medit-0.0.7/medit/mview.py
+-rw-r--r--   0        0        0        0 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/__init__.py
+-rw-r--r--   0        0        0    18966 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/github-markdown-dark.css
+-rw-r--r--   0        0        0    18979 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/github-markdown-light.css
+-rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/pygments-solarized-style/solarized-dark.css
+-rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/pygments-solarized-style/solarized-light.css
+-rw-r--r--   0        0        0    36899 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/solarized-dark-all-sites.css
+-rw-r--r--   0        0        0    36890 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/solarized-light-all-sites.css
+-rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/thomasf-solarized-css/solarized-dark.css
+-rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/thomasf-solarized-css/solarized-light.css
+-rwxr-xr-x   0        0        0     9172 2023-07-25 14:12:18.772105 medit-0.0.7/medit/ui.py
+-rw-r--r--   0        0        0     5361 2023-07-04 06:15:16.098475 medit-0.0.7/medit/utils.py
+-rwxr-xr-x   0        0        0     6266 2023-06-29 19:10:09.897127 medit-0.0.7/medit/yatl.py
+-rw-r--r--   0        0        0     2393 2023-07-25 14:15:29.872306 medit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 medit-0.0.7/PKG-INFO
```

### Comparing `medit-0.0.6/Readme.md` & `medit-0.0.7/Readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -83,14 +83,17 @@
 * [ ] Spell checker
 * [ ] Script console with preview
 * [ ] Preview rules (markdown->HTML, xml/json/yaml -> xml/json/yaml ..)
 
 
 ## Read
 
+* https://pypi.org/project/markdown-include/
+* https://unpkg.com/browse/mermaid@8.1.0/dist/
+* https://pypi.org/project/md-mermaid/
 * https://web.archive.org/web/20190604145031/https://qscintilla.com/prepare-image-hack/
 
 * https://github.com/sindresorhus/github-markdown-css
 * https://python-markdown.github.io/extensions/code_hilite/#step-1-download-and-install-pygments
 * https://github.com/richleland/pygments-css
 * https://github.com/OzakIOne/markdown-github-dark
 * https://github.com/jamiemcg/remarkable
```

### Comparing `medit-0.0.6/medit/cli.py` & `medit-0.0.7/medit/cli.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/medit.ui` & `medit-0.0.7/medit/medit.ui`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/meditor.py` & `medit-0.0.7/medit/meditor.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/mview.py` & `medit-0.0.7/medit/mview.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 
 import pygments.lexers
 from markdown import markdown
+from markdown_include.include import MarkdownInclude
 from pygments import highlight
 from pygments.formatters import HtmlFormatter
 from PyQt6.QtWebEngineWidgets import QWebEngineView
 
 
 class MView(QWebEngineView):
     def __init__(self, parent):
@@ -104,14 +105,21 @@
             html, style = (
                 markdown(
                     content,
                     extensions=[
                         "extra",
                         "codehilite",
                         "markdown_checklist.extension",
+                        "md_mermaid",
+                        MarkdownInclude(
+                            configs={
+                                "base_path": "/home/frafue/_SHARED/logbook",
+                                "encoding": "iso-8859-1",
+                            }
+                        ),
                     ],
                 ),
                 self.css_content_markdown,
             )
         else:
             formatter = HtmlFormatter(linenos="table", cssclass="codehilite")
             lexer = (
```

### Comparing `medit-0.0.6/medit/styles/external/github-markdown-dark.css` & `medit-0.0.7/medit/styles/external/github-markdown-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/styles/external/github-markdown-light.css` & `medit-0.0.7/medit/styles/external/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/styles/external/pygments-solarized-style/solarized-dark.css` & `medit-0.0.7/medit/styles/external/pygments-solarized-style/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/styles/external/pygments-solarized-style/solarized-light.css` & `medit-0.0.7/medit/styles/external/pygments-solarized-style/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/styles/external/solarized-dark-all-sites.css` & `medit-0.0.7/medit/styles/external/solarized-dark-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/styles/external/solarized-light-all-sites.css` & `medit-0.0.7/medit/styles/external/solarized-light-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/styles/external/thomasf-solarized-css/solarized-dark.css` & `medit-0.0.7/medit/styles/external/thomasf-solarized-css/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/styles/external/thomasf-solarized-css/solarized-light.css` & `medit-0.0.7/medit/styles/external/thomasf-solarized-css/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/ui.py` & `medit-0.0.7/medit/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
         self.autosave_timer = QtCore.QTimer(self)
         self.autosave_timer.timeout.connect(self.on_autosave_timer_timeout)
 
         self.setGeometry(*config.get("window_geometry", (50, 50, 1000, 500)))
         self.base_dir = (
             path
+            and path.exists()
             and (path if path.is_dir else path.parent)
             or Path(config.get("base_dir") or ".").absolute()
         )
         self.autoload_thread = QtCore.QThread(self)
         self.autoload_thread.run = lambda: self.async_stuff()
         self.autoload_thread.start()
 
@@ -74,15 +75,27 @@
         # print(self.fs_watcher.files())
 
         self.fs_model = QtGui.QFileSystemModel()
         self.fs_model.setRootPath(Path.home().as_posix())
 
         self.open_file = None
 
-        self.set_open_file(path if path and path.is_file() else config.get("open_file"))
+        def extract_paths():
+            if path:
+                if not path.exists():
+                    log().warning("%s does not exist", path)
+                    return Path("."), None
+                if path.is_dir():
+                    return path, None
+                return path.parent, path
+            return Path(config.get("base_dir") or "."), config.get("open_file")
+
+        self.base_dir, file_path = extract_paths()
+
+        self.set_open_file(file_path)
 
         self.gb_splitter.setSizes(config.get("split_sizes", [1, 1, 1]))
 
         self.tv_files.setModel(self.fs_model)
 
         self.tv_files.selectionModel().selectionChanged.connect(self.on_tv_files_selectionChanged)
 
@@ -162,15 +175,17 @@
             self.txt_editor.openFile(selected_file)
             self.open_file = selected_file
         except UnicodeDecodeError:
             self.txt_editor.setText("")
         finally:
             self.txt_editor.blockSignals(block_state)
             self.setWindowTitle(str(self.open_file))
-            QtWidgets.QApplication.instance().setApplicationName(f"medit - {self.open_file.name}")
+            QtWidgets.QApplication.instance().setApplicationName(
+                f"medit - {self.open_file and self.open_file.name or ''}"
+            )
 
         self.render_content()
 
     @impatient
     def on_tv_files_selectionChanged(self, selection1, selection2) -> None:
         # print(Path(self.fs_model.filePath(selection.indexes()[0])))
         try:
```

### Comparing `medit-0.0.6/medit/utils.py` & `medit-0.0.7/medit/utils.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/medit/yatl.py` & `medit-0.0.7/medit/yatl.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.6/pyproject.toml` & `medit-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medit"
-version = "0.0.6"
+version = "0.0.7"
 description = "Markup Editor"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/medit.git"
 readme = "Readme.md"
 packages = [
   {include = "medit/**/*.py"},
   {include = "medit/**/*.ui"},
@@ -17,19 +17,22 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 asyncinotify = "^4.0.1"
 toml = "^0.10.2"
 pyqt6 = "^6.5.1"
 pyqt6-qscintilla = "^2.14.0"
 pyqt6-webengine = "^6.5.0"
-markdown = "^3.4.3"
+markdown = "<3.2"
 markdown-checklist = "^0.4.4"
 # pygments-solarized-style = "^0.1"
 pyqtdarktheme = "^2.1.0"
 pygments = "^2.15.1"
+#plantuml-markdown = "^3.9.2"
+md-mermaid = "^0.1.1"
+markdown-include = "^0.8.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
```

### Comparing `medit-0.0.6/PKG-INFO` & `medit-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: medit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Markup Editor
 Home-page: https://projects.om-office.de/frans/medit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncinotify (>=4.0.1,<5.0.0)
-Requires-Dist: markdown (>=3.4.3,<4.0.0)
+Requires-Dist: markdown (<3.2)
 Requires-Dist: markdown-checklist (>=0.4.4,<0.5.0)
+Requires-Dist: markdown-include (>=0.8.1,<0.9.0)
+Requires-Dist: md-mermaid (>=0.1.1,<0.2.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: pyqt6 (>=6.5.1,<7.0.0)
 Requires-Dist: pyqt6-qscintilla (>=2.14.0,<3.0.0)
 Requires-Dist: pyqt6-webengine (>=6.5.0,<7.0.0)
 Requires-Dist: pyqtdarktheme (>=2.1.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://projects.om-office.de/frans/medit.git
@@ -107,14 +109,17 @@
 * [ ] Spell checker
 * [ ] Script console with preview
 * [ ] Preview rules (markdown->HTML, xml/json/yaml -> xml/json/yaml ..)
 
 
 ## Read
 
+* https://pypi.org/project/markdown-include/
+* https://unpkg.com/browse/mermaid@8.1.0/dist/
+* https://pypi.org/project/md-mermaid/
 * https://web.archive.org/web/20190604145031/https://qscintilla.com/prepare-image-hack/
 
 * https://github.com/sindresorhus/github-markdown-css
 * https://python-markdown.github.io/extensions/code_hilite/#step-1-download-and-install-pygments
 * https://github.com/richleland/pygments-css
 * https://github.com/OzakIOne/markdown-github-dark
 * https://github.com/jamiemcg/remarkable
```

