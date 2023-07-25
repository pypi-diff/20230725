# Comparing `tmp/tkvue-2.1.2-py3-none-any.whl.zip` & `tmp/tkvue-2.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 196218 bytes, number of entries: 10
--rw-r--r--  2.0 unx    32060 b- defN 23-Jul-13 17:53 tkvue/__init__.py
--rw-rw-rw-  2.0 unx   170486 b- defN 22-Nov-09 20:26 tkvue/tests/preloader.gif
--rw-rw-rw-  2.0 unx      814 b- defN 22-Nov-09 20:26 tkvue/tests/python_icon.png
--rw-rw-rw-  2.0 unx    23217 b- defN 23-Jul-12 18:21 tkvue/tests/test_tkvue.py
--rw-rw-rw-  2.0 unx    26523 b- defN 23-Jul-13 18:02 tkvue-2.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6250 b- defN 23-Jul-13 18:02 tkvue-2.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 18:02 tkvue-2.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-13 18:02 tkvue-2.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-13 18:02 tkvue-2.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      794 b- defN 23-Jul-13 18:02 tkvue-2.1.2.dist-info/RECORD
-10 files, 260289 bytes uncompressed, 194874 bytes compressed:  25.1%
+Zip file size: 196322 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    32214 b- defN 23-Jul-25 12:19 tkvue/__init__.py
+-rw-rw-rw-  2.0 unx   170486 b- defN 23-Jul-12 18:03 tkvue/tests/preloader.gif
+-rw-rw-rw-  2.0 unx      814 b- defN 23-Jul-12 18:03 tkvue/tests/python_icon.png
+-rw-rw-rw-  2.0 unx    23217 b- defN 23-Jul-12 18:18 tkvue/tests/test_tkvue.py
+-rw-rw-rw-  2.0 unx    26523 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6478 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jul-25 12:39 tkvue-2.1.3.dist-info/RECORD
+10 files, 260671 bytes uncompressed, 194978 bytes compressed:  25.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tkvue/tests/python_icon.png
 Comment: 
 
 Filename: tkvue/tests/test_tkvue.py
 Comment: 
 
-Filename: tkvue-2.1.2.dist-info/LICENSE
+Filename: tkvue-2.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: tkvue-2.1.2.dist-info/METADATA
+Filename: tkvue-2.1.3.dist-info/METADATA
 Comment: 
 
-Filename: tkvue-2.1.2.dist-info/WHEEL
+Filename: tkvue-2.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: tkvue-2.1.2.dist-info/entry_points.txt
+Filename: tkvue-2.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: tkvue-2.1.2.dist-info/top_level.txt
+Filename: tkvue-2.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: tkvue-2.1.2.dist-info/RECORD
+Filename: tkvue-2.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tkvue/__init__.py

```diff
@@ -589,15 +589,22 @@
     """
 
     def __init__(self, master, *args, **kw):
         ttk.Frame.__init__(self, master, *args, **kw)
 
         # create a canvas object and a vertical scrollbar for scrolling it
         self.vscrollbar = ttk.Scrollbar(self, orient=tkinter.VERTICAL)
-        self.canvas = tkinter.Canvas(self, bd=0, highlightthickness=0, yscrollcommand=self.vscrollbar.set)
+        min_height = self.vscrollbar.winfo_reqheight()
+        self.canvas = tkinter.Canvas(
+            self,
+            borderwidth=0,
+            highlightthickness=0,
+            yscrollcommand=self.vscrollbar.set,
+            height=min_height,
+        )
         self.canvas.pack(side=tkinter.LEFT, fill=tkinter.BOTH, expand=tkinter.TRUE)
         self.vscrollbar.config(command=self.canvas.yview)
 
         # reset the view
         self.canvas.xview_moveto(0)
         self.canvas.yview_moveto(0)
```

## Comparing `tkvue-2.1.2.dist-info/LICENSE` & `tkvue-2.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tkvue-2.1.2.dist-info/METADATA` & `tkvue-2.1.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkvue
-Version: 2.1.2
+Version: 2.1.3
 Summary: Declarative Tkinter UI using makup language with reactive data binding
 Home-page: https://gitlab.com/ikus-soft/tkvue
 Author: IKUS Software inc.
 Author-email: support@ikus-soft.com
 Maintainer: Patrik Dufresne
 Maintainer-email: patrik@ikus-soft.com
 License: LGPLv3
@@ -113,14 +113,26 @@
 Other Tkinter-related projects worth mentioning:
 
 * [witkets](https://www.leandromattioli.com.br/witkets): Create Tkinter interface using XML similar to TKVue
 * [ttkbootstrap](https://ttkbootstrap.readthedocs.io/): Theme extension for tkinter inspire by Bootstrap
 
 ## Changelog
 
+## 2.1.3 (2023-07-25)
+
+* Define minimum height for ScrolledFrame.
+
+## 2.1.2 (2023-07-13)
+
+* Fix display of scrollbar in ScrolledFrame when resize on Y axis.
+
+## 2.1.1 (2023-07-12)
+
+* Fix display of scrollbar on initialization.
+
 ## 2.1.0 (2023-04-20)
 
 * Add many examples for self documentation
 * Provide the `@tkvue.widget` annotation to register a new widget.
 * Provide the `@tkvue.attr` annotation to register the custom attributes of the widget.
 
 ## 2.0.3 (2023-02-26)
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tkvue Version: 2.1.2 Summary: Declarative Tkinter
+Metadata-Version: 2.1 Name: tkvue Version: 2.1.3 Summary: Declarative Tkinter
 UI using makup language with reactive data binding Home-page: https://
 gitlab.com/ikus-soft/tkvue Author: IKUS Software inc. Author-email:
 support@ikus-soft.com Maintainer: Patrik Dufresne Maintainer-email:
 patrik@ikus-soft.com License: LGPLv3 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications Classifier: Environment :: Win32
 (MS Windows) Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: License :: OSI Approved :: GNU Lesser
@@ -38,16 +38,19 @@
 right plugin to extract the values from the templates. babel.cfg: ```ini
 [tkvue: **/templates/**.tkml] ``` Then You may use babel and other gettext
 tools to complete the translation using the `.po` file. ```sh python setup.py
 extract_messages ``` ## See Also Other Tkinter-related projects worth
 mentioning: * [witkets](https://www.leandromattioli.com.br/witkets): Create
 Tkinter interface using XML similar to TKVue * [ttkbootstrap](https://
 ttkbootstrap.readthedocs.io/): Theme extension for tkinter inspire by Bootstrap
-## Changelog ## 2.1.0 (2023-04-20) * Add many examples for self documentation *
-Provide the `@tkvue.widget` annotation to register a new widget. * Provide the
+## Changelog ## 2.1.3 (2023-07-25) * Define minimum height for ScrolledFrame.
+## 2.1.2 (2023-07-13) * Fix display of scrollbar in ScrolledFrame when resize
+on Y axis. ## 2.1.1 (2023-07-12) * Fix display of scrollbar on initialization.
+## 2.1.0 (2023-04-20) * Add many examples for self documentation * Provide the
+`@tkvue.widget` annotation to register a new widget. * Provide the
 `@tkvue.attr` annotation to register the custom attributes of the widget. ##
 2.0.3 (2023-02-26) * Support `resizable` attribute on TopLevel
 [not_resizable.py](https://gitlab.com/ikus-soft/tkvue/-/blob/master/src/tkvue/
 examples/not_resizable.py) * Support `theme` attribute on TopLevel [theme.py]
 (https://gitlab.com/ikus-soft/tkvue/-/blob/master/src/tkvue/examples/theme.py)
 ## 2.0.2 (2023-02-08) * Add example to demonstrate usage of variables
 [dynamic.py](https://gitlab.com/ikus-soft/tkvue/-/blob/master/src/tkvue/
```

## Comparing `tkvue-2.1.2.dist-info/RECORD` & `tkvue-2.1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tkvue/__init__.py,sha256=m4KRLUDA-LdHq0Ch4kUsuG3sZXi4oLzFKAIl9RVJG3Y,32060
+tkvue/__init__.py,sha256=Gwdj9kQkco-465TtfVpDrt--ZnbtFc86jBtDYjO4Kto,32214
 tkvue/tests/preloader.gif,sha256=4WubudKMAoutzmKtq4PR70A8DoCy5GC_fdVn08FRItc,170486
 tkvue/tests/python_icon.png,sha256=TNB4Jv9uPJYDC9CxCVUv6q5Fu6mlSx2Skuk68ckAcqQ,814
 tkvue/tests/test_tkvue.py,sha256=ou_M6PUEyTeVlPOA0UfTAaW4OyZigxjcXX7m86Cnv7A,23217
-tkvue-2.1.2.dist-info/LICENSE,sha256=wOyDtdXHKbVMd0kW1v8xZvyrYk9MeGP2-70glJMR9nc,26523
-tkvue-2.1.2.dist-info/METADATA,sha256=oZTJCoRsMC_AZmWvN5QeTMaUwRo7HYgQYp5qbETth9Q,6250
-tkvue-2.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tkvue-2.1.2.dist-info/entry_points.txt,sha256=8VY5M0e9X8hXWRDu4nXU60waEEcTmLS5mRgxCmcVE88,47
-tkvue-2.1.2.dist-info/top_level.txt,sha256=anZORAc3YItPGY-GYRZ9zA_9cHsS-bhOtuYTL0R6ffU,6
-tkvue-2.1.2.dist-info/RECORD,,
+tkvue-2.1.3.dist-info/LICENSE,sha256=wOyDtdXHKbVMd0kW1v8xZvyrYk9MeGP2-70glJMR9nc,26523
+tkvue-2.1.3.dist-info/METADATA,sha256=6aZVSjlx6QXjfTM8DnuAbphKBIIRwwLcrkqjuKlhbhk,6478
+tkvue-2.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tkvue-2.1.3.dist-info/entry_points.txt,sha256=8VY5M0e9X8hXWRDu4nXU60waEEcTmLS5mRgxCmcVE88,47
+tkvue-2.1.3.dist-info/top_level.txt,sha256=anZORAc3YItPGY-GYRZ9zA_9cHsS-bhOtuYTL0R6ffU,6
+tkvue-2.1.3.dist-info/RECORD,,
```

