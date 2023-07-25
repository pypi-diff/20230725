# Comparing `tmp/json_html-0.0.1.tar.gz` & `tmp/json-html-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_html-0.0.1.tar", last modified: Tue Jul 25 13:02:02 2023, max compression
+gzip compressed data, was "json-html-0.0.2.tar", last modified: Tue Jul 25 13:39:23 2023, max compression
```

## Comparing `json_html-0.0.1.tar` & `json-html-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 13:02:02.762991 json_html-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-25 12:21:49.000000 json_html-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       26 2023-07-25 12:24:39.000000 json_html-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      232 2023-07-25 13:02:02.762991 json_html-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      792 2023-07-25 13:01:48.000000 json_html-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 13:02:02.754339 json_html-0.0.1/json_html/
--rw-rw-rw-   0        0        0       70 2023-07-25 13:00:52.000000 json_html-0.0.1/json_html/__init__.py
--rw-rw-rw-   0        0        0     1843 2023-07-25 12:59:45.000000 json_html-0.0.1/json_html/cmd.py
--rw-rw-rw-   0        0        0     2753 2023-07-25 12:35:52.000000 json_html-0.0.1/json_html/parser.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:02:02.761954 json_html-0.0.1/json_html.egg-info/
--rw-rw-rw-   0        0        0      232 2023-07-25 13:02:02.000000 json_html-0.0.1/json_html.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-25 13:02:02.000000 json_html-0.0.1/json_html.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:02:02.000000 json_html-0.0.1/json_html.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-25 13:02:02.000000 json_html-0.0.1/json_html.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-07-25 13:02:02.000000 json_html-0.0.1/json_html.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 13:02:02.000000 json_html-0.0.1/json_html.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 12:23:09.000000 json_html-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 13:02:02.762991 json_html-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-07-25 12:32:21.000000 json_html-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:39:23.058018 json-html-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-25 12:21:49.000000 json-html-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-07-25 12:24:39.000000 json-html-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      232 2023-07-25 13:39:23.057005 json-html-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      792 2023-07-25 13:02:39.000000 json-html-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 13:39:23.048286 json-html-0.0.2/json_html/
+-rw-rw-rw-   0        0        0       70 2023-07-25 13:39:17.000000 json-html-0.0.2/json_html/__init__.py
+-rw-rw-rw-   0        0        0     1843 2023-07-25 12:59:45.000000 json-html-0.0.2/json_html/cmd.py
+-rw-rw-rw-   0        0        0     1520 2023-07-25 13:33:49.000000 json-html-0.0.2/json_html/lists.py
+-rw-rw-rw-   0        0        0     2668 2023-07-25 13:38:01.000000 json-html-0.0.2/json_html/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:39:23.057005 json-html-0.0.2/json_html.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 13:39:22.000000 json-html-0.0.2/json_html.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        5 2023-07-25 12:23:09.000000 json-html-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 13:39:23.058018 json-html-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-07-25 13:02:51.000000 json-html-0.0.2/setup.py
```

### Comparing `json_html-0.0.1/LICENSE` & `json-html-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `json_html-0.0.1/README.md` & `json-html-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # json_html.py
 Python code that translates JSON template to HTML
 
 ## Requirements
 - Python >=3.10
 
 ## Install
-Simply use the command `pip install json_html` to install the package.
+Simply use the command `pip install json-html` to install the package.
 
 ## Usage (Python)
 ```py
 import json
 from json_html import JSONHTML
 
 with open("./FILENAME.json", "r", encoding="utf-8") as f:
```

### Comparing `json_html-0.0.1/json_html/cmd.py` & `json-html-0.0.2/json_html/cmd.py`

 * *Files identical despite different names*

### Comparing `json_html-0.0.1/json_html/parser.py` & `json-html-0.0.2/json_html/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 import re
 import json
 
 from bs4 import BeautifulSoup
 
+from .lists import elements
+
 __all__ = (
     "JSONHTML",
 )
 
 
 class JSONHTML:
     def __init__(self, data: dict):
         if not isinstance(data, dict):
             raise TypeError("data must be a dict")
 
         self._data = data
+        self._location = None
         self.re_space = re.compile(r"^\s+")
 
-        self._elements = [
-            "html", "head", "body", "title",
-            "h1", "h2", "h3", "h4", "h5", "h6",
-            "div", "span", "p", "a", "img",
-            "ul", "ol", "li", "table", "tr"
-        ]
-
-        self._attrs = [
-            "id", "class", "style", "src", "href", "alt", "content"
-        ]
-
     @classmethod
     def from_file(cls, filename: str) -> "JSONHTML":
         """ Attempts to load a JSON file and return the class """
         with open(filename, "r", encoding="utf-8") as f:
             data = json.load(f)
         return cls(data)
 
@@ -42,15 +34,15 @@
     def element(self, tag: str, data: dict) -> str:
         """ Returns a HTML element with attributes and content """
         attrs = []
 
         content = data.get("content", "")
 
         for k, v in data.items():
-            if k != "content" and k not in self._elements:
+            if k != "content" and k not in elements:
                 attrs.append(f'{k}="{v}"')
 
         attrs_str = " ".join(attrs)
 
         if attrs_str:
             attrs_str = " " + attrs_str
 
@@ -58,23 +50,29 @@
 
     def render(self, data: dict = None) -> str:
         """ Returns a HTML string """
         html = ""
         data: dict = data or self._data
 
         for k, v in data.items():
+            if k in ["head", "body"]:
+                self._location = k
+
             if isinstance(v, dict):
-                if k in self._attrs:
+                if k == "title" and self._location == "body":
                     continue
-                if k in self._elements:
+
+                if k in elements:
                     html += self.element(k, v)
                     html += self.render(v)
                     html += f"</{k}>"
             else:
-                if k in self._attrs:
+                if k not in elements:
+                    continue
+                if k == "title" and self._location == "body":
                     continue
                 html += self.element(k, {"content": str(v)})
 
         return html
 
     def prettify(self, html_content, indent_width: int = 2) -> str:
         """ Returns a indented HTML string """
```

### Comparing `json_html-0.0.1/setup.py` & `json-html-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
 
 if not version:
     raise RuntimeError('version is not set')
 
 
 setup(
-    name='json_html',
+    name='json-html',
     author='AlexFlipnote',
     url='https://github.com/AlexFlipnote/json_html.py',
     version=version,
     packages=['json_html'],
     license='MIT',
     description='Python code that translates JSON template to HTML',
     include_package_data=True,
```

