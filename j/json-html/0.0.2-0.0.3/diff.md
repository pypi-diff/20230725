# Comparing `tmp/json-html-0.0.2.tar.gz` & `tmp/json-html-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-html-0.0.2.tar", last modified: Tue Jul 25 13:39:23 2023, max compression
+gzip compressed data, was "json-html-0.0.3.tar", last modified: Tue Jul 25 13:53:10 2023, max compression
```

## Comparing `json-html-0.0.2.tar` & `json-html-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 13:39:23.058018 json-html-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-25 12:21:49.000000 json-html-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       26 2023-07-25 12:24:39.000000 json-html-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      232 2023-07-25 13:39:23.057005 json-html-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      792 2023-07-25 13:02:39.000000 json-html-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 13:39:23.048286 json-html-0.0.2/json_html/
--rw-rw-rw-   0        0        0       70 2023-07-25 13:39:17.000000 json-html-0.0.2/json_html/__init__.py
--rw-rw-rw-   0        0        0     1843 2023-07-25 12:59:45.000000 json-html-0.0.2/json_html/cmd.py
--rw-rw-rw-   0        0        0     1520 2023-07-25 13:33:49.000000 json-html-0.0.2/json_html/lists.py
--rw-rw-rw-   0        0        0     2668 2023-07-25 13:38:01.000000 json-html-0.0.2/json_html/parser.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:39:23.057005 json-html-0.0.2/json_html.egg-info/
--rw-rw-rw-   0        0        0      232 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 12:23:09.000000 json-html-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 13:39:23.058018 json-html-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-07-25 13:02:51.000000 json-html-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:53:10.604458 json-html-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-25 12:21:49.000000 json-html-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-07-25 12:24:39.000000 json-html-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      232 2023-07-25 13:53:10.604458 json-html-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      792 2023-07-25 13:02:39.000000 json-html-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 13:53:10.595253 json-html-0.0.3/json_html/
+-rw-rw-rw-   0        0        0       70 2023-07-25 13:42:16.000000 json-html-0.0.3/json_html/__init__.py
+-rw-rw-rw-   0        0        0     1843 2023-07-25 12:59:45.000000 json-html-0.0.3/json_html/cmd.py
+-rw-rw-rw-   0        0        0     1520 2023-07-25 13:33:49.000000 json-html-0.0.3/json_html/lists.py
+-rw-rw-rw-   0        0        0     2638 2023-07-25 13:52:28.000000 json-html-0.0.3/json_html/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:53:10.603440 json-html-0.0.3/json_html.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-07-25 13:53:10.000000 json-html-0.0.3/json_html.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-25 13:53:10.000000 json-html-0.0.3/json_html.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 13:53:10.000000 json-html-0.0.3/json_html.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-25 13:53:10.000000 json-html-0.0.3/json_html.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-07-25 13:53:10.000000 json-html-0.0.3/json_html.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 13:53:10.000000 json-html-0.0.3/json_html.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        5 2023-07-25 12:23:09.000000 json-html-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 13:53:10.604458 json-html-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-07-25 13:02:51.000000 json-html-0.0.3/setup.py
```

### Comparing `json-html-0.0.2/LICENSE` & `json-html-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `json-html-0.0.2/README.md` & `json-html-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `json-html-0.0.2/json_html/cmd.py` & `json-html-0.0.3/json_html/cmd.py`

 * *Files identical despite different names*

### Comparing `json-html-0.0.2/json_html/lists.py` & `json-html-0.0.3/json_html/lists.py`

 * *Files identical despite different names*

### Comparing `json-html-0.0.2/json_html/parser.py` & `json-html-0.0.3/json_html/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,35 +46,36 @@
         if attrs_str:
             attrs_str = " " + attrs_str
 
         return f"<{tag}{attrs_str}>{content}"
 
     def render(self, data: dict = None) -> str:
         """ Returns a HTML string """
-        html = ""
+        html: str = ""
         data: dict = data or self._data
 
         for k, v in data.items():
             if k in ["head", "body"]:
                 self._location = k
 
             if isinstance(v, dict):
                 if k == "title" and self._location == "body":
                     continue
 
                 if k in elements:
                     html += self.element(k, v)
                     html += self.render(v)
                     html += f"</{k}>"
-            else:
+
+            elif isinstance(v, str):
                 if k not in elements:
                     continue
-                if k == "title" and self._location == "body":
-                    continue
+
                 html += self.element(k, {"content": str(v)})
+                html += f"</{k}>"
 
         return html
 
     def prettify(self, html_content, indent_width: int = 2) -> str:
         """ Returns a indented HTML string """
         soup = BeautifulSoup(html_content, "html.parser")
         pretty_html = soup.prettify(formatter=None)
```

### Comparing `json-html-0.0.2/setup.py` & `json-html-0.0.3/setup.py`

 * *Files identical despite different names*

