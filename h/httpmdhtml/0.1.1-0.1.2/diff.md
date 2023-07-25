# Comparing `tmp/httpmdhtml-0.1.1.tar.gz` & `tmp/httpmdhtml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpmdhtml-0.1.1.tar", last modified: Fri Jul 21 16:44:22 2023, max compression
+gzip compressed data, was "httpmdhtml-0.1.2.tar", last modified: Tue Jul 25 20:01:14 2023, max compression
```

## Comparing `httpmdhtml-0.1.1.tar` & `httpmdhtml-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-21 16:44:22.945489 httpmdhtml-0.1.1/
--rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-04-04 17:12:07.000000 httpmdhtml-0.1.1/LICENSE.txt
--rwxrwxrwx   0 john      (1000) john      (1000)     3574 2023-07-21 16:44:22.947500 httpmdhtml-0.1.1/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)     3139 2023-05-03 16:16:27.000000 httpmdhtml-0.1.1/README.md
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-21 16:44:22.560410 httpmdhtml-0.1.1/httpmdhtml/
--rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-04 17:12:07.000000 httpmdhtml-0.1.1/httpmdhtml/__init__.py
--rwxrwxrwx   0 john      (1000) john      (1000)     3957 2023-07-21 16:37:51.000000 httpmdhtml-0.1.1/httpmdhtml/md_to_html.py
--rwxrwxrwx   0 john      (1000) john      (1000)     4532 2023-05-03 16:03:35.000000 httpmdhtml-0.1.1/httpmdhtml/server.py
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-21 16:44:22.850361 httpmdhtml-0.1.1/httpmdhtml.egg-info/
--rwxrwxrwx   0 john      (1000) john      (1000)     3574 2023-07-21 16:44:21.000000 httpmdhtml-0.1.1/httpmdhtml.egg-info/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)      293 2023-07-21 16:44:22.000000 httpmdhtml-0.1.1/httpmdhtml.egg-info/SOURCES.txt
--rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-07-21 16:44:21.000000 httpmdhtml-0.1.1/httpmdhtml.egg-info/dependency_links.txt
--rwxrwxrwx   0 john      (1000) john      (1000)       39 2023-07-21 16:44:21.000000 httpmdhtml-0.1.1/httpmdhtml.egg-info/requires.txt
--rwxrwxrwx   0 john      (1000) john      (1000)       11 2023-07-21 16:44:21.000000 httpmdhtml-0.1.1/httpmdhtml.egg-info/top_level.txt
--rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-05-03 14:31:06.000000 httpmdhtml-0.1.1/pyproject.toml
--rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-07-21 16:44:22.961130 httpmdhtml-0.1.1/setup.cfg
--rwxrwxrwx   0 john      (1000) john      (1000)      923 2023-07-21 16:42:38.000000 httpmdhtml-0.1.1/setup.py
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-25 20:01:14.757909 httpmdhtml-0.1.2/
+-rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-04-04 17:12:07.000000 httpmdhtml-0.1.2/LICENSE.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)     3574 2023-07-25 20:01:14.760617 httpmdhtml-0.1.2/PKG-INFO
+-rwxrwxrwx   0 john      (1000) john      (1000)     3139 2023-05-03 16:16:27.000000 httpmdhtml-0.1.2/README.md
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-25 20:01:14.370373 httpmdhtml-0.1.2/httpmdhtml/
+-rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-04 17:12:07.000000 httpmdhtml-0.1.2/httpmdhtml/__init__.py
+-rwxrwxrwx   0 john      (1000) john      (1000)     3930 2023-07-25 19:59:35.000000 httpmdhtml-0.1.2/httpmdhtml/md_to_html.py
+-rwxrwxrwx   0 john      (1000) john      (1000)     4532 2023-05-03 16:03:35.000000 httpmdhtml-0.1.2/httpmdhtml/server.py
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-07-25 20:01:14.679153 httpmdhtml-0.1.2/httpmdhtml.egg-info/
+-rwxrwxrwx   0 john      (1000) john      (1000)     3574 2023-07-25 20:01:13.000000 httpmdhtml-0.1.2/httpmdhtml.egg-info/PKG-INFO
+-rwxrwxrwx   0 john      (1000) john      (1000)      293 2023-07-25 20:01:13.000000 httpmdhtml-0.1.2/httpmdhtml.egg-info/SOURCES.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-07-25 20:01:13.000000 httpmdhtml-0.1.2/httpmdhtml.egg-info/dependency_links.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)       39 2023-07-25 20:01:13.000000 httpmdhtml-0.1.2/httpmdhtml.egg-info/requires.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)       11 2023-07-25 20:01:13.000000 httpmdhtml-0.1.2/httpmdhtml.egg-info/top_level.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-05-03 14:31:06.000000 httpmdhtml-0.1.2/pyproject.toml
+-rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-07-25 20:01:14.779338 httpmdhtml-0.1.2/setup.cfg
+-rwxrwxrwx   0 john      (1000) john      (1000)      923 2023-07-25 20:00:15.000000 httpmdhtml-0.1.2/setup.py
```

### Comparing `httpmdhtml-0.1.1/LICENSE.txt` & `httpmdhtml-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `httpmdhtml-0.1.1/PKG-INFO` & `httpmdhtml-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: httpmdhtml
-Version: 0.1.1
+Version: 0.1.2
 Summary: HTTP server that converts markdown to HTML
 Home-page: https://github.com/treatmesubj/python-md-to-html-server
-Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.1.2.tar.gz
 Author: John Hupperts
 Author-email: jrock4503@hotmail.com
 License: gpl-3.0
 Project-URL: Source, https://github.com/treatmesubj/python-md-to-html-server
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_b4y61qs0_/tmp31zo4vdg_TarContainer/0/2", line 73, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_b4y61qs0_/tmp31zo4vdg_TarContainer/0/2", line 73, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: httpmdhtml Version: 0.1.1 Summary: HTTP server that
+Metadata-Version: 2.1 Name: httpmdhtml Version: 0.1.2 Summary: HTTP server that
 converts markdown to HTML Home-page: https://github.com/treatmesubj/python-md-
 to-html-server Download-URL: https://github.com/treatmesubj/python-md-to-html-
-server/archive/refs/tags/v0.1.1.tar.gz Author: John Hupperts Author-email:
+server/archive/refs/tags/v0.1.2.tar.gz Author: John Hupperts Author-email:
 jrock4503@hotmail.com License: gpl-3.0 Project-URL: Source, https://github.com/
 treatmesubj/python-md-to-html-server Description-Content-Type: text/markdown
 License-File: LICENSE.txt # Python Markdown-to-HTML Server It's the standard
 Python [http.server module](https://docs.python.org/3/library/http.server.html)
 but via [markdown-it-py](https://github.com/executablebooks/markdown-it-py),
 requested Markdown files are rendered and served as HTML The `http.server`
 module's `SimpleHTTPRequestHandler` class is inherited by a new class with its
```

### Comparing `httpmdhtml-0.1.1/README.md` & `httpmdhtml-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `httpmdhtml-0.1.1/httpmdhtml/md_to_html.py` & `httpmdhtml-0.1.2/httpmdhtml/md_to_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         else:
             with open(css_file, "r") as f:
                 css = f.read()
     else:
         css = """
 body { background-color: #272822; color: #e6edf3; font-family: -apple-system,BlinkMacSystemFont,"Segoe UI","Noto Sans",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji"; position: relative; max-width: 960px; margin: auto; line-height: 1.5; }
 a[href] { color: #66d9ef; }
-code { color: #e6edf3; background-color: #343941; font-family: monospace; white-space: break-spaces; padding: .2em .4em; border-radius: 6px; }
+code { color: #e6edf3; background-color: #343941; font-family: monospace; padding: .2em .4em; border-radius: 6px; }
 pre { padding: 1em; border-radius: 6px; background-color: #161b22; }
 pre code { background-color: #161b22; }
 table, th, td { border: 1px solid; border-collapse: collapse; padding-left: 4px; padding-right: 4px; }
 img { max-width: 100%; }
 """
     soup.select_one("style").string = css
     if live_md_rr:
```

### Comparing `httpmdhtml-0.1.1/httpmdhtml/server.py` & `httpmdhtml-0.1.2/httpmdhtml/server.py`

 * *Files identical despite different names*

### Comparing `httpmdhtml-0.1.1/httpmdhtml.egg-info/PKG-INFO` & `httpmdhtml-0.1.2/httpmdhtml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: httpmdhtml
-Version: 0.1.1
+Version: 0.1.2
 Summary: HTTP server that converts markdown to HTML
 Home-page: https://github.com/treatmesubj/python-md-to-html-server
-Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.1.2.tar.gz
 Author: John Hupperts
 Author-email: jrock4503@hotmail.com
 License: gpl-3.0
 Project-URL: Source, https://github.com/treatmesubj/python-md-to-html-server
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_b4y61qs0_/tmp31zo4vdg_TarContainer/0/9", line 73, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_b4y61qs0_/tmp31zo4vdg_TarContainer/0/9", line 73, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: httpmdhtml Version: 0.1.1 Summary: HTTP server that
+Metadata-Version: 2.1 Name: httpmdhtml Version: 0.1.2 Summary: HTTP server that
 converts markdown to HTML Home-page: https://github.com/treatmesubj/python-md-
 to-html-server Download-URL: https://github.com/treatmesubj/python-md-to-html-
-server/archive/refs/tags/v0.1.1.tar.gz Author: John Hupperts Author-email:
+server/archive/refs/tags/v0.1.2.tar.gz Author: John Hupperts Author-email:
 jrock4503@hotmail.com License: gpl-3.0 Project-URL: Source, https://github.com/
 treatmesubj/python-md-to-html-server Description-Content-Type: text/markdown
 License-File: LICENSE.txt # Python Markdown-to-HTML Server It's the standard
 Python [http.server module](https://docs.python.org/3/library/http.server.html)
 but via [markdown-it-py](https://github.com/executablebooks/markdown-it-py),
 requested Markdown files are rendered and served as HTML The `http.server`
 module's `SimpleHTTPRequestHandler` class is inherited by a new class with its
```

### Comparing `httpmdhtml-0.1.1/setup.py` & `httpmdhtml-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="httpmdhtml",
-    version="0.1.1",
+    version="0.1.2",
     license="gpl-3.0",
     author="John Hupperts",
     author_email="jrock4503@hotmail.com",
     description="HTTP server that converts markdown to HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/treatmesubj/python-md-to-html-server",
-    download_url="https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.1.1.tar.gz",
+    download_url="https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.1.2.tar.gz",
     packages=["httpmdhtml"],
     package_dir={"python-md-to-html-server": "httpmdhtml"},
     project_urls={
         "Source": "https://github.com/treatmesubj/python-md-to-html-server",
     },
     install_requires=[
         "markdown-it-py",
```

