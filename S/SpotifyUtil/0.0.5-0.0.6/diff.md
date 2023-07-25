# Comparing `tmp/SpotifyUtil-0.0.5.tar.gz` & `tmp/SpotifyUtil-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpotifyUtil-0.0.5.tar", last modified: Sun Jul 23 07:29:21 2023, max compression
+gzip compressed data, was "SpotifyUtil-0.0.6.tar", last modified: Tue Jul 25 10:32:45 2023, max compression
```

## Comparing `SpotifyUtil-0.0.5.tar` & `SpotifyUtil-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 07:29:21.912008 SpotifyUtil-0.0.5/
--rw-rw-rw-   0        0        0    35823 2023-07-13 08:37:27.000000 SpotifyUtil-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2006 2023-07-23 07:29:21.906014 SpotifyUtil-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1284 2023-07-17 13:09:57.000000 SpotifyUtil-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 07:29:21.854483 SpotifyUtil-0.0.5/SpotifyUtil/
--rw-rw-rw-   0        0        0    16390 2023-07-23 07:29:00.000000 SpotifyUtil-0.0.5/SpotifyUtil/SpotifyUtil.py
--rw-rw-rw-   0        0        0      139 2023-07-18 16:53:30.000000 SpotifyUtil-0.0.5/SpotifyUtil/__init__.py
--rw-rw-rw-   0        0        0     1387 2023-07-17 18:50:45.000000 SpotifyUtil-0.0.5/SpotifyUtil/config.py
--rw-rw-rw-   0        0        0      262 2023-07-16 14:31:36.000000 SpotifyUtil-0.0.5/SpotifyUtil/file_reader.py
--rw-rw-rw-   0        0        0      157 2023-07-17 14:31:47.000000 SpotifyUtil-0.0.5/SpotifyUtil/secret.py
--rw-rw-rw-   0        0        0     1594 2023-07-22 17:47:21.000000 SpotifyUtil-0.0.5/SpotifyUtil/utilityTest.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:29:21.902007 SpotifyUtil-0.0.5/SpotifyUtil.egg-info/
--rw-rw-rw-   0        0        0     2006 2023-07-23 07:29:21.000000 SpotifyUtil-0.0.5/SpotifyUtil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-07-23 07:29:21.000000 SpotifyUtil-0.0.5/SpotifyUtil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 07:29:21.000000 SpotifyUtil-0.0.5/SpotifyUtil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-23 07:29:21.000000 SpotifyUtil-0.0.5/SpotifyUtil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-23 07:29:21.000000 SpotifyUtil-0.0.5/SpotifyUtil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      768 2023-07-23 07:28:44.000000 SpotifyUtil-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-23 07:29:21.912008 SpotifyUtil-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      962 2023-07-23 07:28:51.000000 SpotifyUtil-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:32:45.806416 SpotifyUtil-0.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-07-13 08:37:27.000000 SpotifyUtil-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2006 2023-07-25 10:32:45.804905 SpotifyUtil-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1284 2023-07-17 13:09:57.000000 SpotifyUtil-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 10:32:45.727977 SpotifyUtil-0.0.6/SpotifyUtil/
+-rw-rw-rw-   0        0        0    16372 2023-07-24 16:54:36.000000 SpotifyUtil-0.0.6/SpotifyUtil/SpotifyUtil.py
+-rw-rw-rw-   0        0        0      139 2023-07-18 16:53:30.000000 SpotifyUtil-0.0.6/SpotifyUtil/__init__.py
+-rw-rw-rw-   0        0        0     1387 2023-07-17 18:50:45.000000 SpotifyUtil-0.0.6/SpotifyUtil/config.py
+-rw-rw-rw-   0        0        0      262 2023-07-16 14:31:36.000000 SpotifyUtil-0.0.6/SpotifyUtil/file_reader.py
+-rw-rw-rw-   0        0        0      177 2023-07-24 17:02:35.000000 SpotifyUtil-0.0.6/SpotifyUtil/secret.py
+-rw-rw-rw-   0        0        0     1594 2023-07-22 17:47:21.000000 SpotifyUtil-0.0.6/SpotifyUtil/utilityTest.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:32:45.802384 SpotifyUtil-0.0.6/SpotifyUtil.egg-info/
+-rw-rw-rw-   0        0        0     2006 2023-07-25 10:32:45.000000 SpotifyUtil-0.0.6/SpotifyUtil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-07-25 10:32:45.000000 SpotifyUtil-0.0.6/SpotifyUtil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 10:32:45.000000 SpotifyUtil-0.0.6/SpotifyUtil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 10:32:45.000000 SpotifyUtil-0.0.6/SpotifyUtil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-25 10:32:45.000000 SpotifyUtil-0.0.6/SpotifyUtil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      795 2023-07-25 10:32:01.000000 SpotifyUtil-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 10:32:45.807427 SpotifyUtil-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-07-25 10:32:05.000000 SpotifyUtil-0.0.6/setup.py
```

### Comparing `SpotifyUtil-0.0.5/LICENSE` & `SpotifyUtil-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.5/PKG-INFO` & `SpotifyUtil-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpotifyUtil
-Version: 0.0.5
+Version: 0.0.6
 Summary: SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.
 Home-page: https://github.com/Arg0naut18/SpotifyUtil
 Author: Arg0naut18
 Author-email: Arg0naut18 <gaming.genos1729@gmail.com>
 Project-URL: Homepage, https://github.com/Arg0naut18/SpotifyUtil
 Keywords: Spotify,Spotipy,SpotifyUtil,SpotifyUtils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SpotifyUtil-0.0.5/README.md` & `SpotifyUtil-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.5/SpotifyUtil/SpotifyUtil.py` & `SpotifyUtil-0.0.6/SpotifyUtil/SpotifyUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 from SpotifyUtil.file_reader import FileReader
 
 
 log = logging.getLogger(__name__)
 
 class TrackSetDetails:
-    def __init__(self, total_size: int, playable_size: int, detailed_list: list[dict], unplayable_list:list):
+    def __init__(self, total_size: int, playable_size: int, detailed_list: list, unplayable_list:list):
         self.total_size = total_size
         self.playable_size = playable_size
         self.detailed_list = detailed_list
         self.unplayable_uris = unplayable_list
 
 
 class SpotifyUtil(Config):
@@ -42,23 +42,23 @@
         id = self.get_id(url=url, type=type)
         return f'spotify:{type}:{id}'
     
     def get_playlist_name_from_id(self, playlist_id):
         playlist = self.spotify.user_playlist(user=None, playlist_id=playlist_id, fields="name")
         return playlist['name']
     
-    def get_playlist_tracks(self, playlist_id, market=None) -> list[dict]:
+    def get_playlist_tracks(self, playlist_id, market=None) -> list:
         results = self.spotify.user_playlist_tracks(self.user_id, playlist_id, market=market)
         tracks = results['items']
         while results['next']:
             results = self.spotify.next(results)
             tracks.extend(results['items'])
         return tracks
     
-    def get_liked_songs(self, limit, offset) -> list[dict]:
+    def get_liked_songs(self, limit, offset) -> list:
         results = self.spotify.current_user_saved_tracks(limit=limit, offset=offset)
         tracks = results['items']
         while results['next']:
             results = self.spotify.next(results)
             tracks.extend(results['items'])
         return tracks
```

### Comparing `SpotifyUtil-0.0.5/SpotifyUtil/config.py` & `SpotifyUtil-0.0.6/SpotifyUtil/config.py`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.5/SpotifyUtil/utilityTest.py` & `SpotifyUtil-0.0.6/SpotifyUtil/utilityTest.py`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.5/SpotifyUtil.egg-info/PKG-INFO` & `SpotifyUtil-0.0.6/SpotifyUtil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpotifyUtil
-Version: 0.0.5
+Version: 0.0.6
 Summary: SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.
 Home-page: https://github.com/Arg0naut18/SpotifyUtil
 Author: Arg0naut18
 Author-email: Arg0naut18 <gaming.genos1729@gmail.com>
 Project-URL: Homepage, https://github.com/Arg0naut18/SpotifyUtil
 Keywords: Spotify,Spotipy,SpotifyUtil,SpotifyUtils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SpotifyUtil-0.0.5/pyproject.toml` & `SpotifyUtil-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SpotifyUtil"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="Arg0naut18", email="gaming.genos1729@gmail.com" },
 ]
 description = "SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -13,16 +13,17 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 keywords = [
     "Spotify",
     "Spotipy",
     "SpotifyUtil",
-    "SpotifyUtils",
+    "SpotifyUtils"
 ]
+dependencies = ["spotipy"]
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
 "Homepage" = "https://github.com/Arg0naut18/SpotifyUtil"
```

### Comparing `SpotifyUtil-0.0.5/setup.py` & `SpotifyUtil-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SpotifyUtil",
-    version="0.0.5",
+    version="0.0.6",
     author="Arg0naut18",
     description="SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Arg0naut18/SpotifyUtil",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     keywords = [
-    "Spotify",
-    "Spotipy",
-    "SpotifyUtil",
-    "SpotifyUtils",
+        "Spotify",
+        "Spotipy",
+        "SpotifyUtil",
+        "SpotifyUtils",
     ],
     python_requires=">= 3.8",
     include_package_data=True,
     install_requires=["spotipy"]
 )
```

