# Comparing `tmp/medit-0.0.7.tar.gz` & `tmp/medit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medit-0.0.7.tar", max compression
+gzip compressed data, was "medit-0.0.8.tar", max compression
```

## Comparing `medit-0.0.7.tar` & `medit-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,58 @@
--rw-r--r--   0        0        0     3231 2023-07-25 14:15:03.192269 medit-0.0.7/Readme.md
--rw-r--r--   0        0        0        0 2023-06-16 07:35:55.912297 medit-0.0.7/medit/__init__.py
--rwxr-xr-x   0        0        0     2192 2023-07-03 06:21:56.302488 medit-0.0.7/medit/cli.py
--rw-r--r--   0        0        0     2362 2023-07-03 06:51:24.784057 medit-0.0.7/medit/medit.ui
--rw-r--r--   0        0        0     5067 2023-07-04 06:15:16.074437 medit-0.0.7/medit/meditor.py
--rw-r--r--   0        0        0     7879 2023-07-25 14:12:18.736105 medit-0.0.7/medit/mview.py
--rw-r--r--   0        0        0        0 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/__init__.py
--rw-r--r--   0        0        0    18966 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/github-markdown-dark.css
--rw-r--r--   0        0        0    18979 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/github-markdown-light.css
--rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/pygments-solarized-style/solarized-dark.css
--rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/pygments-solarized-style/solarized-light.css
--rw-r--r--   0        0        0    36899 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/solarized-dark-all-sites.css
--rw-r--r--   0        0        0    36890 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/solarized-light-all-sites.css
--rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/thomasf-solarized-css/solarized-dark.css
--rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.7/medit/styles/external/thomasf-solarized-css/solarized-light.css
--rwxr-xr-x   0        0        0     9172 2023-07-25 14:12:18.772105 medit-0.0.7/medit/ui.py
--rw-r--r--   0        0        0     5361 2023-07-04 06:15:16.098475 medit-0.0.7/medit/utils.py
--rwxr-xr-x   0        0        0     6266 2023-06-29 19:10:09.897127 medit-0.0.7/medit/yatl.py
--rw-r--r--   0        0        0     2393 2023-07-25 14:15:29.872306 medit-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 medit-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3399 2023-07-25 17:45:28.116423 medit-0.0.8/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-01 03:43:26.302528 medit-0.0.8/medit/__init__.py
+-rwxr-xr-x   0        0        0     2192 2023-07-25 16:55:11.883381 medit-0.0.8/medit/cli.py
+-rw-r--r--   0        0        0     2340 2023-07-25 17:49:29.441015 medit-0.0.8/medit/medit.ui
+-rw-r--r--   0        0        0     5067 2023-07-25 16:55:11.883381 medit-0.0.8/medit/meditor.py
+-rw-r--r--   0        0        0     7873 2023-07-25 16:55:11.884381 medit-0.0.8/medit/mview.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:04:58.958106 medit-0.0.8/medit/styles/__init__.py
+-rw-r--r--   0        0        0    18966 2023-07-02 11:28:30.508468 medit-0.0.8/medit/styles/external/github-markdown-dark.css
+-rw-r--r--   0        0        0    18979 2023-07-02 11:28:30.508468 medit-0.0.8/medit/styles/external/github-markdown-light.css
+-rw-r--r--   0        0        0    23562 2022-09-24 11:57:23.000000 medit-0.0.8/medit/styles/external/github-markdown.css
+-rw-r--r--   0        0        0     5061 2023-07-02 11:28:30.508468 medit-0.0.8/medit/styles/external/pygments-solarized-style/solarized-dark.css
+-rw-r--r--   0        0        0     5061 2023-07-02 11:28:30.508468 medit-0.0.8/medit/styles/external/pygments-solarized-style/solarized-light.css
+-rw-r--r--   0        0        0     2247 2023-07-02 08:09:35.126975 medit-0.0.8/medit/styles/external/retro.css
+-rw-r--r--   0        0        0    36899 2023-07-02 11:28:30.509468 medit-0.0.8/medit/styles/external/solarized-dark-all-sites.css
+-rw-r--r--   0        0        0    36890 2023-07-02 11:28:30.509468 medit-0.0.8/medit/styles/external/solarized-light-all-sites.css
+-rw-r--r--   0        0        0     4282 2023-07-02 11:28:30.509468 medit-0.0.8/medit/styles/external/thomasf-solarized-css/solarized-dark.css
+-rw-r--r--   0        0        0     4282 2023-07-02 11:28:30.509468 medit-0.0.8/medit/styles/external/thomasf-solarized-css/solarized-light.css
+-rw-r--r--   0        0        0     2831 2023-07-02 10:24:56.448801 medit-0.0.8/medit/styles/markdown.min.css
+-rw-r--r--   0        0        0     4046 2023-07-02 08:45:15.342414 medit-0.0.8/medit/styles/pygments/abap.css
+-rw-r--r--   0        0        0     4106 2023-07-02 08:45:15.978432 medit-0.0.8/medit/styles/pygments/algol.css
+-rw-r--r--   0        0        0     3910 2023-07-02 08:45:15.664423 medit-0.0.8/medit/styles/pygments/algol_nu.css
+-rw-r--r--   0        0        0     3955 2023-07-02 08:45:16.299441 medit-0.0.8/medit/styles/pygments/arduino.css
+-rw-r--r--   0        0        0     4556 2023-07-02 08:45:16.618450 medit-0.0.8/medit/styles/pygments/autumn.css
+-rw-r--r--   0        0        0     3826 2023-07-02 08:45:16.940460 medit-0.0.8/medit/styles/pygments/borland.css
+-rw-r--r--   0        0        0     2865 2023-07-02 08:45:17.260469 medit-0.0.8/medit/styles/pygments/bw.css
+-rw-r--r--   0        0        0     5200 2023-07-02 08:45:17.583478 medit-0.0.8/medit/styles/pygments/colorful.css
+-rw-r--r--   0        0        0     4889 2023-07-02 08:45:17.900487 medit-0.0.8/medit/styles/pygments/default.css
+-rw-r--r--   0        0        0     5159 2023-07-02 08:45:18.220497 medit-0.0.8/medit/styles/pygments/dracula.css
+-rw-r--r--   0        0        0     4888 2023-07-02 08:45:18.538506 medit-0.0.8/medit/styles/pygments/emacs.css
+-rw-r--r--   0        0        0     4916 2023-07-02 08:45:19.181524 medit-0.0.8/medit/styles/pygments/friendly.css
+-rw-r--r--   0        0        0     4916 2023-07-02 08:45:18.860515 medit-0.0.8/medit/styles/pygments/friendly_grayscale.css
+-rw-r--r--   0        0        0     5687 2023-07-02 08:45:19.500533 medit-0.0.8/medit/styles/pygments/fruity.css
+-rw-r--r--   0        0        0     2565 2023-07-02 08:45:20.520563 medit-0.0.8/medit/styles/pygments/igor.css
+-rw-r--r--   0        0        0     5248 2023-07-02 08:45:21.192582 medit-0.0.8/medit/styles/pygments/inkpot.css
+-rw-r--r--   0        0        0     4458 2023-07-02 08:45:21.513591 medit-0.0.8/medit/styles/pygments/lilypond.css
+-rw-r--r--   0        0        0     4805 2023-07-02 08:45:21.835600 medit-0.0.8/medit/styles/pygments/lovelace.css
+-rw-r--r--   0        0        0     5000 2023-07-02 08:45:22.153610 medit-0.0.8/medit/styles/pygments/manni.css
+-rw-r--r--   0        0        0     5097 2023-07-02 08:45:22.474619 medit-0.0.8/medit/styles/pygments/material.css
+-rw-r--r--   0        0        0     5036 2023-07-02 08:45:22.790628 medit-0.0.8/medit/styles/pygments/monokai.css
+-rw-r--r--   0        0        0     5282 2023-07-02 08:45:23.113637 medit-0.0.8/medit/styles/pygments/murphy.css
+-rw-r--r--   0        0        0     5437 2023-07-02 08:45:23.440647 medit-0.0.8/medit/styles/pygments/native.css
+-rw-r--r--   0        0        0     5312 2023-07-02 08:45:23.766656 medit-0.0.8/medit/styles/pygments/nord.css
+-rw-r--r--   0        0        0     5330 2023-07-02 08:45:25.136695 medit-0.0.8/medit/styles/pygments/pastie.css
+-rw-r--r--   0        0        0     4602 2023-07-02 08:45:25.457705 medit-0.0.8/medit/styles/pygments/perldoc.css
+-rw-r--r--   0        0        0     4845 2023-07-02 08:45:25.778714 medit-0.0.8/medit/styles/pygments/rainbow_dash.css
+-rw-r--r--   0        0        0     4951 2023-07-02 08:45:26.102723 medit-0.0.8/medit/styles/pygments/rrt.css
+-rw-r--r--   0        0        0     4421 2023-07-02 08:45:26.421733 medit-0.0.8/medit/styles/pygments/sas.css
+-rw-r--r--   0        0        0     4951 2023-07-02 08:45:27.095752 medit-0.0.8/medit/styles/pygments/staroffice.css
+-rw-r--r--   0        0        0     5589 2023-07-02 08:45:28.112781 medit-0.0.8/medit/styles/pygments/tango.css
+-rw-r--r--   0        0        0     4684 2023-07-02 08:45:28.434790 medit-0.0.8/medit/styles/pygments/trac.css
+-rw-r--r--   0        0        0     5112 2023-07-02 08:45:28.758800 medit-0.0.8/medit/styles/pygments/vim.css
+-rw-r--r--   0        0        0     2666 2023-07-02 08:45:29.079809 medit-0.0.8/medit/styles/pygments/vs.css
+-rw-r--r--   0        0        0     4057 2023-07-02 08:45:29.402818 medit-0.0.8/medit/styles/pygments/xcode.css
+-rw-r--r--   0        0        0     5506 2023-07-02 08:45:29.728828 medit-0.0.8/medit/styles/pygments/zenburn.css
+-rwxr-xr-x   0        0        0     9923 2023-07-25 19:18:23.170479 medit-0.0.8/medit/ui.py
+-rw-r--r--   0        0        0     5361 2023-07-25 16:55:11.884381 medit-0.0.8/medit/utils.py
+-rw-r--r--   0        0        0     2393 2023-07-25 17:15:38.969466 medit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 medit-0.0.8/PKG-INFO
```

### Comparing `medit-0.0.7/Readme.md` & `medit-0.0.8/Readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,19 +48,24 @@
 
 ## My personal MLP (v1.0) goals
 
 * [x] File to title
 * [x] File viewer for Plain, Python, YAML, JSON, ..
 * [x] Autosave
 * [x] Manage word wrap in editor
+* [x] include files
+* [ ] spell check
+* [ ] sort files by modification
+* [ ] add / remove / rename files
+* [ ] support sequence diagrams mermaid
+* [ ] Workdir/file history / Recent files
 * [ ] Autoload
 * [ ] Multi-File Undo/Redo
 * [ ] Change into / step up current directory
 * [ ] Zen mode
-* [ ] Recent files
 * [ ] Search/open files
 * [ ] Search in files
 * [ ] Preview for previewable only
 * [ ] Hightlight todo.txt
 * [ ] Notify external file changes
 * [ ] (Re-)store zoom and fullscreen
 * [ ] File ignore filter
```

### Comparing `medit-0.0.7/medit/cli.py` & `medit-0.0.8/medit/cli.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/medit.ui` & `medit-0.0.8/medit/medit.ui`

 * *Files 10% similar despite different names*

#### Comparing `medit-0.0.7/medit/medit.ui` & `medit-0.0.8/medit/medit.ui`

```diff
@@ -38,25 +38,23 @@
             <property name="orientation">
               <enum>Qt::Horizontal</enum>
             </property>
             <widget class="QSplitter" name="gb_left_splitter">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
-              <layout class="QVBoxLayout" name="verticalLayout">
-                <item>
-                  <widget class="QTreeView" name="tv_files"/>
-                </item>
-                <item>
-                  <widget class="QListWidget" name="lst_recent"/>
-                </item>
-                <item>
-                  <widget class="QPlainTextEdit" name="txt_log"/>
-                </item>
-              </layout>
+              <widget class="QTreeView" name="tv_files">
+                <property name="font">
+                  <font>
+                    <family>Source Code Pro Semibold</family>
+                  </font>
+                </property>
+              </widget>
+              <widget class="QListWidget" name="lst_recent"/>
+              <widget class="QPlainTextEdit" name="txt_log"/>
             </widget>
             <widget class="MEditor" name="txt_editor"/>
             <widget class="MView" name="wv_rendered" native="true">
               <property name="minimumSize">
                 <size>
                   <width>100</width>
                   <height>0</height>
```

### Comparing `medit-0.0.7/medit/meditor.py` & `medit-0.0.8/medit/meditor.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/mview.py` & `medit-0.0.8/medit/mview.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,28 +95,28 @@
                 # "styles/pygments/vim.css",  #                |
                 # "styles/pygments/vs.css",  #                 | light, transparent, decent
                 # "styles/pygments/xcode.css",  #              | light, transparent, decent
                 # "styles/pygments/zenburn.css",  #            | dark
             )
         )
 
-    def show(self, content, highlight_mode):
+    def show(self, content, highlight_mode, base_dir: Path):
 
         if highlight_mode == ".md":
             html, style = (
                 markdown(
                     content,
                     extensions=[
                         "extra",
                         "codehilite",
                         "markdown_checklist.extension",
                         "md_mermaid",
                         MarkdownInclude(
                             configs={
-                                "base_path": "/home/frafue/_SHARED/logbook",
+                                "base_path": base_dir,
                                 "encoding": "iso-8859-1",
                             }
                         ),
                     ],
                 ),
                 self.css_content_markdown,
             )
```

### Comparing `medit-0.0.7/medit/styles/external/github-markdown-dark.css` & `medit-0.0.8/medit/styles/external/github-markdown-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/styles/external/github-markdown-light.css` & `medit-0.0.8/medit/styles/external/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/styles/external/pygments-solarized-style/solarized-dark.css` & `medit-0.0.8/medit/styles/external/pygments-solarized-style/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/styles/external/pygments-solarized-style/solarized-light.css` & `medit-0.0.8/medit/styles/external/pygments-solarized-style/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/styles/external/solarized-dark-all-sites.css` & `medit-0.0.8/medit/styles/external/solarized-dark-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/styles/external/solarized-light-all-sites.css` & `medit-0.0.8/medit/styles/external/solarized-light-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/styles/external/thomasf-solarized-css/solarized-dark.css` & `medit-0.0.8/medit/styles/external/thomasf-solarized-css/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/styles/external/thomasf-solarized-css/solarized-light.css` & `medit-0.0.8/medit/styles/external/thomasf-solarized-css/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/medit/ui.py` & `medit-0.0.8/medit/ui.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,31 @@
 
 def load_default(filename, default):
     with suppress(FileNotFoundError, json.JSONDecodeError):
         return json.load(open(os.path.expanduser(filename)))
     return default
 
 
+# class FileFilterProxyModel(QtCore.QSortFilterProxyModel):
+# def __init__(self, *args, **kwargs):
+# super(FileFilterProxyModel, self).__init__(*args, **kwargs)
+# self.excluded_files = []
+
+# def setExcludedFiles(self, files):
+# self.excluded_files = files
+# self.invalidateFilter()
+
+# def filterAcceptsRow(self, source_row, source_parent):
+# source_model = self.sourceModel()
+# index0 = source_model.index(source_row, 0, source_parent)
+# filename = source_model.data(index0, QtCore.Qt.DisplayRole)
+
+# return not filename in self.excluded_files
+
+
 class MEditWindow(QtWidgets.QMainWindow):
     """The one and only application window"""
 
     @impatient
     def __init__(self, path: Path | None) -> None:
         super().__init__()
         uic.loadUi(Path(__file__).parent / "medit.ui", self)
@@ -72,15 +89,16 @@
         # self.fs_watcher.fileChanged.connect(self.on_file_changed_externally)
         # self.fs_watcher.directoryChanged.connect(self.on_file_changed_externally)
         # self.fs_watcher.addPaths([self.base_dir.as_posix()])
         # print(self.fs_watcher.files())
 
         self.fs_model = QtGui.QFileSystemModel()
         self.fs_model.setRootPath(Path.home().as_posix())
-
+        # self.fs_model.setNameFilters()
+        self.fs_model.setNameFilters(["*.txt", "*.md"])
         self.open_file = None
 
         def extract_paths():
             if path:
                 if not path.exists():
                     log().warning("%s does not exist", path)
                     return Path("."), None
@@ -102,14 +120,17 @@
         self.tv_files.hideColumn(1)
         self.tv_files.hideColumn(2)
         self.tv_files.hideColumn(3)
         self.tv_files.setHeaderHidden(True)
 
         self.tv_files.setRootIndex(self.fs_model.index(self.base_dir.as_posix()))
         self.tv_files.expand(self.fs_model.index(self.base_dir.as_posix()))
+
+        self.fs_model.sort(3, QtCore.Qt.SortOrder.DescendingOrder)
+
         if self.open_file:
             self.tv_files.setCurrentIndex(self.fs_model.index(self.open_file.absolute().as_posix()))
         else:
             self.tv_files.setCurrentIndex(self.fs_model.index(self.base_dir.absolute().as_posix()))
 
         self.show()
 
@@ -138,15 +159,17 @@
     def reset_timer(self):
         logging.debug("reset modification timer")
         self.autosave_timer.start(300)
 
     @impatient
     def render_content(self):
         self.wv_rendered.show(
-            self.txt_editor.text(), self.open_file and self.open_file.suffix.strip("~")
+            self.txt_editor.text(),
+            self.open_file and self.open_file.suffix.strip("~"),
+            self.base_dir,
         )
 
     @impatient
     def on_autosave_timer_timeout(self):
         """"""
         self.autosave_timer.stop()
         self.render_content()
```

### Comparing `medit-0.0.7/medit/utils.py` & `medit-0.0.8/medit/utils.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.7/pyproject.toml` & `medit-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medit"
-version = "0.0.7"
+version = "0.0.8"
 description = "Markup Editor"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/medit.git"
 readme = "Readme.md"
 packages = [
   {include = "medit/**/*.py"},
   {include = "medit/**/*.ui"},
```

### Comparing `medit-0.0.7/PKG-INFO` & `medit-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medit
-Version: 0.0.7
+Version: 0.0.8
 Summary: Markup Editor
 Home-page: https://projects.om-office.de/frans/medit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -74,19 +74,24 @@
 
 ## My personal MLP (v1.0) goals
 
 * [x] File to title
 * [x] File viewer for Plain, Python, YAML, JSON, ..
 * [x] Autosave
 * [x] Manage word wrap in editor
+* [x] include files
+* [ ] spell check
+* [ ] sort files by modification
+* [ ] add / remove / rename files
+* [ ] support sequence diagrams mermaid
+* [ ] Workdir/file history / Recent files
 * [ ] Autoload
 * [ ] Multi-File Undo/Redo
 * [ ] Change into / step up current directory
 * [ ] Zen mode
-* [ ] Recent files
 * [ ] Search/open files
 * [ ] Search in files
 * [ ] Preview for previewable only
 * [ ] Hightlight todo.txt
 * [ ] Notify external file changes
 * [ ] (Re-)store zoom and fullscreen
 * [ ] File ignore filter
```

