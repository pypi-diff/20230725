# Comparing `tmp/akari-dl-1.2.0.tar.gz` & `tmp/akari-dl-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-dl-1.2.0.tar", last modified: Mon Jul 24 23:28:35 2023, max compression
+gzip compressed data, was "akari-dl-1.2.1.tar", last modified: Mon Jul 24 23:39:47 2023, max compression
```

## Comparing `akari-dl-1.2.0.tar` & `akari-dl-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 23:28:35.957230 akari-dl-1.2.0/
--rw-rw-rw-   0        0        0     1235 2023-07-18 05:22:58.000000 akari-dl-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      589 2023-07-24 23:28:35.956231 akari-dl-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4541 2023-07-24 23:25:51.000000 akari-dl-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 23:28:35.933688 akari-dl-1.2.0/akari_dl/
--rw-rw-rw-   0        0        0     2792 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/__init__.py
--rw-rw-rw-   0        0        0     1844 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 23:28:35.955232 akari-dl-1.2.0/akari_dl/src/
--rw-rw-rw-   0        0        0     3737 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/src/download_anime.py
--rw-rw-rw-   0        0        0      368 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/src/log_response.py
--rw-rw-rw-   0        0        0     1106 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/src/resolve_anime.py
--rw-rw-rw-   0        0        0     1194 2023-07-24 23:25:51.000000 akari-dl-1.2.0/akari_dl/src/website.py
-drwxrwxrwx   0        0        0        0 2023-07-24 23:28:35.951719 akari-dl-1.2.0/akari_dl.egg-info/
--rw-rw-rw-   0        0        0      589 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 23:28:35.000000 akari-dl-1.2.0/akari_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 23:28:35.957230 akari-dl-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-07-24 23:25:51.000000 akari-dl-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:39:47.852800 akari-dl-1.2.1/
+-rw-rw-rw-   0        0        0     1235 2023-07-18 05:22:58.000000 akari-dl-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      589 2023-07-24 23:39:47.851804 akari-dl-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4541 2023-07-24 23:25:51.000000 akari-dl-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 23:39:47.782778 akari-dl-1.2.1/akari_dl/
+-rw-rw-rw-   0        0        0     2792 2023-07-24 23:39:30.000000 akari-dl-1.2.1/akari_dl/__init__.py
+-rw-rw-rw-   0        0        0     1829 2023-07-24 23:32:08.000000 akari-dl-1.2.1/akari_dl/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:39:47.850801 akari-dl-1.2.1/akari_dl/src/
+-rw-rw-rw-   0        0        0     2983 2023-07-24 23:38:21.000000 akari-dl-1.2.1/akari_dl/src/download_anime.py
+-rw-rw-rw-   0        0        0      368 2023-07-24 23:25:51.000000 akari-dl-1.2.1/akari_dl/src/log_response.py
+-rw-rw-rw-   0        0        0     1106 2023-07-24 23:38:25.000000 akari-dl-1.2.1/akari_dl/src/resolve_anime.py
+-rw-rw-rw-   0        0        0     1155 2023-07-24 23:33:26.000000 akari-dl-1.2.1/akari_dl/src/website.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:39:47.847799 akari-dl-1.2.1/akari_dl.egg-info/
+-rw-rw-rw-   0        0        0      589 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 23:39:47.000000 akari-dl-1.2.1/akari_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 23:39:47.852800 akari-dl-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-07-24 23:39:39.000000 akari-dl-1.2.1/setup.py
```

### Comparing `akari-dl-1.2.0/LICENSE` & `akari-dl-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.0/PKG-INFO` & `akari-dl-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-dl
-Version: 1.2.0
+Version: 1.2.1
 Summary: A lightweight and open-source anime downloading CLI.
 Home-page: https://github.com/keisanng/akari-dl
 Author: keisan
 Author-email: <keisan@skiff.com>
 Project-URL: Documentation, https://github.com/keisanng/akari-dl#readme
 Project-URL: Tracker, https://github.com/users/keisanng/projects/3
 Requires-Python: >=3.10
```

### Comparing `akari-dl-1.2.0/README.md` & `akari-dl-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.0/akari_dl/__init__.py` & `akari-dl-1.2.1/akari_dl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,10 +57,10 @@
 
 arg_parser.add_argument("website", type=str, help="Specify the name of what website to direct-download anime from (see supported websites: https://github.com/keisanng/akari-dl#supported-websites.)", nargs="?")
 arg_parser.add_argument("anime", type=str, help="Specify what anime to download by title (in Romaji {https://en.wikipedia.org/wiki/Romanization_of_Japanese}.)")
 arg_parser.add_argument("output", type=str, help="Specify path to output downloaded video files to.", nargs="?")
 arg_parser.add_argument("-e", "--episodes", type=int, help="Specify the amount of episodes to download (downloads all if not specified) [NOT YET IMPLEMENTED.]")
 arg_parser.add_argument("-s", "--specials", action="store_true", help="Enable downloading of special episodes (only works with websites that list the specials on the same page as the episodes.)")
 arg_parser.add_argument("-d", "--debug", action="store_true", help="Run akari-dl in debug mode; log each connections html body and http headers and prints logging messages.")
-arg_parser.add_argument("-v", "--version", action="version", version="1.1.1", help="Print the current version of akari-dl.")
+arg_parser.add_argument("-v", "--version", action="version", version="1.2.1", help="Print the current version of akari-dl.")
 
 logger = logging
```

### Comparing `akari-dl-1.2.0/akari_dl/__main__.py` & `akari-dl-1.2.1/akari_dl/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from akari_dl import conf_parser, arg_parser, logger
-from akari_dl.src.website import Website
+from . import conf_parser, arg_parser, logger
+from .src.website import Website
 
 def main():
   args = arg_parser.parse_args()
 
   if args.debug or conf_parser["debug"]:
     logger.basicConfig(level=logger.NOTSET)
```

### Comparing `akari-dl-1.2.0/akari_dl/src/download_anime.py` & `akari-dl-1.2.1/akari_dl/src/download_anime.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,66 @@
 """
   Download an anime based on user-configuration given desired anime is found on desired website.
 """
 
 import os
 import requests.exceptions
 
-from akari_dl import conf_parser
-from akari_dl.src.log_response import log_response
-
 def download_episodes(self, folder_path=os.PathLike, episodes=list):
   """
     Download all (unless specified otherwise) episodes of an anime
     into a folder of the anime's name inside the user-provided output path.
   """
   ep_count = 0
 
   for episode in episodes:
     ep_count += 1
 
-    self.endpoint = episode.attrs["href"]
-
-    if self.name == "chauthanh":
-      self.response = self.session.get(f"{self.url}/anime/{self.endpoint[3:]}", timeout=30)
-    else:
-      if self.endpoint.startswith("https"):
-        self.response = self.session.get(self.endpoint, timeout=30)
+    try:
+      if self.name == "chauthanh":
+        self.response = self.session.get(f"{self.url}/anime/{episode.attrs['href'][3:]}", timeout=30)
       else:
-        self.response = self.session.get(f"{self.url}{self.endpoint}", timeout=30)
+        self.response = self.session.get(f"{self.url}{episode.attrs['href']}", timeout=30)
+      anchor = self.response.html.find(self.anchors[2], first=True)
+      self.endpoint = anchor.attrs["href"]
+    except AttributeError:
+      print("Video file not found - skipping episode.")
+      continue
 
-    anchors = self.response.html.find(self.anchors[2])
+    file_format = self.endpoint[-3:]
 
-    connected = False
+    if not os.path.exists(folder_path):
+      os.makedirs(folder_path)
 
     try:
-      for anchor in anchors:
-        try:
-          while not connected:
-            self.endpoint = anchor.attrs["href"]
-
-            if self.name == "chauthanh":
-              self.endpoint = f"{self.url}/anime/download/{self.endpoint[3:]}"
-
-            print(f"Querying {self.endpoint}")
-
-            file_format = self.endpoint[-3:]
-
-            self.response = self.session.get(self.endpoint, timeout=30)
-
-            if self.response.status_code == 200:
-              connected = True
-        except requests.exceptions.MissingSchema:
-          print("Video file not found.")
-    except Exception:
-      print("Unable to find video file; skipping episode.")
+      if self.name == "chauthanh":
+        self.response = self.session.get(f"{self.url}/anime/download/{self.endpoint[3:]}", timeout=30)
+      else:
+        self.response = self.session.get(self.endpoint, timeout=30)
+    except requests.exceptions.MissingSchema:
+      print("Video file not found - skipping episode.")
       continue
 
-    try:
-      print(f"Downloading episode {ep_count} from {self.endpoint}")
-      file_path = os.path.join(folder_path, f"Episode {ep_count}.{file_format}")
-      with open(file_path, "wb") as video_file:
-        for chunk in self.response.iter_content(1024):
-          video_file.write(chunk)
-      print(f"Episode {ep_count} downloaded to {file_path}")
-    except Exception as error:
-      print(f"Failed to download episode: {error}.")
+    print(f"Downloading episode {ep_count} from {self.endpoint}")
+    file_path = os.path.join(folder_path, f"Episode {ep_count}.{file_format}")
+    with open(file_path, "wb") as video_file:
+      for chunk in self.response.iter_content(1024):
+        video_file.write(chunk)
+    print(f"Episode {ep_count} downloaded to {file_path}")
 
 
 def download_anime(self):
   """
     Download user specified anime by scraping links until reaching a video file source.
   """
-  if self.endpoint.startswith("https"):
-    self.response = self.session.get(self.endpoint)
-  else:
-    self.response = self.session.get(f"{self.url}{self.endpoint}")
+  self.response = self.session.get(f"{self.url}{self.endpoint}")
   episodes = self.response.html.find(self.anchors[1]) # Episodes anchors
 
-  if conf_parser["debug"]:
-    log_response(self.response)
-
   episodes_regular, episodes_special = [], []
-
-  if self.name != "enime":
-    episodes.reverse()
+  episodes.reverse()
 
   if self.name == "tokyoinsider":
     for episode in episodes:
       match episode.find("em", first=True).text:
         case "episode":
           episodes_regular.append(episode)
         case _:
@@ -96,25 +70,20 @@
 
   anime_slug = self.anime
   for char in "/><\"\:|?*":
     anime_slug = anime_slug.replace(char, "")
 
   folder_path = os.path.join(self.output_path, anime_slug)
 
-  if not os.path.exists(folder_path):
-    os.makedirs(folder_path)
-
   download_episodes(self, folder_path, episodes_regular)
 
-  if self.specials_enabled:
+  if self.specials_enabled is True:
     folder_path = os.path.join(self.output_path, anime_slug, "Specials")
 
-    if conf_parser["debug"]:
-      download_episodes(self, folder_path, episodes_special)
-    else:
-      try:
-        download_episodes(self, folder_path, episodes_special)
-      except Exception as error:
-        print(f"Download failed: {error}")
-        exit()
+    download_episodes(self, folder_path, episodes_special)
+    # try:
+      # download_episodes(self, folder_path, episodes_special)
+    # except Exception as error:
+      # print(f"Download failed: {error}")
+      # exit()
 
   return f"Finished downloading {self.anime}."
```

### Comparing `akari-dl-1.2.0/akari_dl/src/resolve_anime.py` & `akari-dl-1.2.1/akari_dl/src/resolve_anime.py`

 * *Files identical despite different names*

### Comparing `akari-dl-1.2.0/akari_dl/src/website.py` & `akari-dl-1.2.1/akari_dl/src/website.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=missing-module-docstring, missing-class-docstring, missing-function-docstring, not-callable
 
 from os import PathLike
 import requests_html
 
-from akari_dl.src.resolve_website import resolve_website
-from akari_dl.src.resolve_anime import resolve_anime
-from akari_dl.src.download_anime import download_anime
+from resolve_website import resolve_website
+from resolve_anime import resolve_anime
+from download_anime import download_anime
 
 class Website:
   def __init__(self, name=str, anime=str, output=PathLike, episodes=int, specials=bool, domains=str|tuple, search=str, anchors=tuple):
 
     self.name = name
     self.anime = anime
     self.output_path = output
```

### Comparing `akari-dl-1.2.0/akari_dl.egg-info/PKG-INFO` & `akari-dl-1.2.1/akari_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-dl
-Version: 1.2.0
+Version: 1.2.1
 Summary: A lightweight and open-source anime downloading CLI.
 Home-page: https://github.com/keisanng/akari-dl
 Author: keisan
 Author-email: <keisan@skiff.com>
 Project-URL: Documentation, https://github.com/keisanng/akari-dl#readme
 Project-URL: Tracker, https://github.com/users/keisanng/projects/3
 Requires-Python: >=3.10
```

