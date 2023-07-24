# Comparing `tmp/akari-dl-1.1.0.tar.gz` & `tmp/akari-dl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-dl-1.1.0.tar", last modified: Wed Jul 19 00:18:38 2023, max compression
+gzip compressed data, was "akari-dl-1.2.0.tar", last modified: Mon Jul 24 23:28:35 2023, max compression
```

## Comparing `akari-dl-1.1.0.tar` & `akari-dl-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 00:18:38.037960 akari-dl-1.1.0/
--rw-rw-rw-   0        0        0     1235 2023-07-18 05:22:58.000000 akari-dl-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      589 2023-07-19 00:18:38.036955 akari-dl-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3565 2023-07-18 23:34:24.000000 akari-dl-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 00:18:38.004390 akari-dl-1.1.0/akari_dl/
--rw-rw-rw-   0        0        0     1413 2023-07-18 21:05:22.000000 akari-dl-1.1.0/akari_dl/__init__.py
--rw-rw-rw-   0        0        0      978 2023-07-18 23:56:34.000000 akari-dl-1.1.0/akari_dl/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:18:38.035955 akari-dl-1.1.0/akari_dl/src/
--rw-rw-rw-   0        0        0      124 2023-07-18 01:49:00.000000 akari-dl-1.1.0/akari_dl/src/__init__.py
--rw-rw-rw-   0        0        0     3037 2023-07-18 23:59:10.000000 akari-dl-1.1.0/akari_dl/src/download_anime.py
--rw-rw-rw-   0        0        0      366 2023-07-18 21:02:44.000000 akari-dl-1.1.0/akari_dl/src/log_response.py
--rw-rw-rw-   0        0        0     1186 2023-07-19 00:05:45.000000 akari-dl-1.1.0/akari_dl/src/resolve_anime.py
--rw-rw-rw-   0        0        0      936 2023-07-17 06:32:32.000000 akari-dl-1.1.0/akari_dl/src/resolve_url.py
--rw-rw-rw-   0        0        0     1184 2023-07-17 06:23:26.000000 akari-dl-1.1.0/akari_dl/src/website.py
-drwxrwxrwx   0        0        0        0 2023-07-19 00:18:38.019389 akari-dl-1.1.0/akari_dl.egg-info/
--rw-rw-rw-   0        0        0      589 2023-07-19 00:18:37.000000 akari-dl-1.1.0/akari_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-07-19 00:18:37.000000 akari-dl-1.1.0/akari_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 00:18:37.000000 akari-dl-1.1.0/akari_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-19 00:18:37.000000 akari-dl-1.1.0/akari_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-19 00:18:37.000000 akari-dl-1.1.0/akari_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-19 00:18:37.000000 akari-dl-1.1.0/akari_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 00:18:38.037960 akari-dl-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-07-18 21:00:51.000000 akari-dl-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:28:35.957230 akari-dl-1.2.0/
+-rw-rw-rw-   0        0        0     1235 2023-07-18 05:22:58.000000 akari-dl-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      589 2023-07-24 23:28:35.956231 akari-dl-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4541 2023-07-24 23:25:51.000000 akari-dl-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 23:28:35.933688 akari-dl-1.2.0/akari_dl/
+-rw-rw-rw-   0        0        0     2792 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/__init__.py
+-rw-rw-rw-   0        0        0     1844 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:28:35.955232 akari-dl-1.2.0/akari_dl/src/
+-rw-rw-rw-   0        0        0     3737 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/src/download_anime.py
+-rw-rw-rw-   0        0        0      368 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/src/log_response.py
+-rw-rw-rw-   0        0        0     1106 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/src/resolve_anime.py
+-rw-rw-rw-   0        0        0     1194 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/src/website.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:28:35.951719 akari-dl-1.2.0/akari_dl.egg-info/
+-rw-rw-rw-   0        0        0      589 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 23:28:35.957230 akari-dl-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-07-24 23:25:51.000000 akari-dl-1.2.0/setup.py
```

### Comparing `akari-dl-1.1.0/LICENSE` & `akari-dl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `akari-dl-1.1.0/PKG-INFO` & `akari-dl-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-dl
-Version: 1.1.0
+Version: 1.2.0
 Summary: A lightweight and open-source anime downloading CLI.
 Home-page: https://github.com/keisanng/akari-dl
 Author: keisan
 Author-email: <keisan@skiff.com>
 Project-URL: Documentation, https://github.com/keisanng/akari-dl#readme
 Project-URL: Tracker, https://github.com/users/keisanng/projects/3
 Requires-Python: >=3.10
```

### Comparing `akari-dl-1.1.0/akari_dl/src/resolve_anime.py` & `akari-dl-1.2.0/akari_dl/src/resolve_anime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,29 @@
+from akari_dl import conf_parser
+from akari_dl.src.log_response import log_response
+
 def resolve_anime(self):
   """
     Verify user-specified anime exists on user-specified website via resolved url
     and return the link of the first entry of the anime's name on the website.
   """
   print(f"Searching for \"{self.anime}\"...")
 
-  match self.name:
-    case "tokyoinsider":
-      self.response = self.session.get(f"{self.url}/anime/search?k={self.anime}", timeout=30)
-    case "chauthanh":
-      self.response = self.session.get(f"{self.url}/search/?s={self.anime}", timeout=30)
+  self.response = self.session.get(f"{self.url}/{self.search}{self.anime}", timeout=30)
+  if conf_parser["debug"]:
+    log_response(self.response)
 
   try:
     anchors = self.response.html.find(self.anchors[0])
     if self.name == "tokyoinsider":
       anchors += self.response.html.find("table > tr > .c_h2b > a")
   except Exception:
     print("Anime not found.")
     exit()
 
-  if not anchors:
-    print("Anime not found.")
-    exit()
-
   for i, anchor in enumerate(anchors):
     if self.name == "tokyoinsider":
       print(f"{i+1}. {anchor.attrs['href']}")
     else:
       print(f"{i+1}. {anchor.text}")
 
   while True:
```

### Comparing `akari-dl-1.1.0/akari_dl/src/website.py` & `akari-dl-1.2.0/akari_dl/src/website.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # pylint: disable=missing-module-docstring, missing-class-docstring, missing-function-docstring, not-callable
 
 from os import PathLike
 import requests_html
 
-from akari_dl import src
+from akari_dl.src.resolve_website import resolve_website
+from akari_dl.src.resolve_anime import resolve_anime
+from akari_dl.src.download_anime import download_anime
 
 class Website:
-  def __init__(self, name=str, anime=str, output=PathLike, episodes=int, specials=bool, urls=str|tuple, anchors=tuple):
+  def __init__(self, name=str, anime=str, output=PathLike, episodes=int, specials=bool, domains=str|tuple, search=str, anchors=tuple):
 
     self.name = name
     self.anime = anime
     self.output_path = output
 
     self.episodes_count = episodes
     self.specials_enabled = specials
 
-    self.urls = urls # Available URLs to try to connect to requested site
+    self.domains = domains # Available URLs to try to connect to requested site.
+    self.search = search
     self.anchors = anchors # Expected anchor elements to scrape href from to go from the search page to the anime page to the video file link.
 
     self.url = str
     self.endpoint = None
     self.session  = requests_html.HTMLSession()
 
-    # options.add_argument("User-Agent=Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Mobile Safari/537.36")
 
-
-  def resolve_url(self):
-    self.url = src.resolve_url(self)
+  def resolve_website(self):
+    self.url = resolve_website(self)
 
 
   def resolve_anime(self):
-    self.endpoint = src.resolve_anime(self)
+    self.endpoint = resolve_anime(self)
 
 
   def download_anime(self):
-    src.download_anime(self)
+    download_anime(self)
```

### Comparing `akari-dl-1.1.0/akari_dl.egg-info/PKG-INFO` & `akari-dl-1.2.0/akari_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-dl
-Version: 1.1.0
+Version: 1.2.0
 Summary: A lightweight and open-source anime downloading CLI.
 Home-page: https://github.com/keisanng/akari-dl
 Author: keisan
 Author-email: <keisan@skiff.com>
 Project-URL: Documentation, https://github.com/keisanng/akari-dl#readme
 Project-URL: Tracker, https://github.com/users/keisanng/projects/3
 Requires-Python: >=3.10
```

### Comparing `akari-dl-1.1.0/setup.py` & `akari-dl-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
   name="akari-dl",
-  version="1.1.0",
+  version="1.2.0",
   author="keisan",
   author_email="<keisan@skiff.com>",
   description="A lightweight and open-source anime downloading CLI.",
   long_description="akari-dl downloads anime video files from direct download websites based on user configuration to avoid more annoying downloading methods like torrenting and manually downloading.",
   url="https://github.com/keisanng/akari-dl",
   project_urls={
     "Documentation": "https://github.com/keisanng/akari-dl#readme",
```

