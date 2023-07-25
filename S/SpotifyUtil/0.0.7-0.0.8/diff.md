# Comparing `tmp/SpotifyUtil-0.0.7.tar.gz` & `tmp/SpotifyUtil-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpotifyUtil-0.0.7.tar", last modified: Tue Jul 25 10:47:11 2023, max compression
+gzip compressed data, was "SpotifyUtil-0.0.8.tar", last modified: Tue Jul 25 17:20:19 2023, max compression
```

## Comparing `SpotifyUtil-0.0.7.tar` & `SpotifyUtil-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 10:47:11.315080 SpotifyUtil-0.0.7/
--rw-rw-rw-   0        0        0    35823 2023-07-13 08:37:27.000000 SpotifyUtil-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2006 2023-07-25 10:47:11.314078 SpotifyUtil-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1284 2023-07-17 13:09:57.000000 SpotifyUtil-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 10:47:11.289281 SpotifyUtil-0.0.7/SpotifyUtil/
--rw-rw-rw-   0        0        0    16334 2023-07-25 10:46:27.000000 SpotifyUtil-0.0.7/SpotifyUtil/SpotifyUtil.py
--rw-rw-rw-   0        0        0      139 2023-07-18 16:53:30.000000 SpotifyUtil-0.0.7/SpotifyUtil/__init__.py
--rw-rw-rw-   0        0        0     1387 2023-07-17 18:50:45.000000 SpotifyUtil-0.0.7/SpotifyUtil/config.py
--rw-rw-rw-   0        0        0      262 2023-07-16 14:31:36.000000 SpotifyUtil-0.0.7/SpotifyUtil/file_reader.py
--rw-rw-rw-   0        0        0      177 2023-07-24 17:02:35.000000 SpotifyUtil-0.0.7/SpotifyUtil/secret.py
--rw-rw-rw-   0        0        0     1594 2023-07-22 17:47:21.000000 SpotifyUtil-0.0.7/SpotifyUtil/utilityTest.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:47:11.312082 SpotifyUtil-0.0.7/SpotifyUtil.egg-info/
--rw-rw-rw-   0        0        0     2006 2023-07-25 10:47:11.000000 SpotifyUtil-0.0.7/SpotifyUtil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-07-25 10:47:11.000000 SpotifyUtil-0.0.7/SpotifyUtil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 10:47:11.000000 SpotifyUtil-0.0.7/SpotifyUtil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 10:47:11.000000 SpotifyUtil-0.0.7/SpotifyUtil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-25 10:47:11.000000 SpotifyUtil-0.0.7/SpotifyUtil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      795 2023-07-25 10:46:38.000000 SpotifyUtil-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 10:47:11.315080 SpotifyUtil-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-07-25 10:46:42.000000 SpotifyUtil-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:20:19.519571 SpotifyUtil-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-07-13 08:37:27.000000 SpotifyUtil-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2006 2023-07-25 17:20:19.515419 SpotifyUtil-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1284 2023-07-17 13:09:57.000000 SpotifyUtil-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 17:20:19.461282 SpotifyUtil-0.0.8/SpotifyUtil/
+-rw-rw-rw-   0        0        0    16424 2023-07-25 17:19:29.000000 SpotifyUtil-0.0.8/SpotifyUtil/SpotifyUtil.py
+-rw-rw-rw-   0        0        0      139 2023-07-18 16:53:30.000000 SpotifyUtil-0.0.8/SpotifyUtil/__init__.py
+-rw-rw-rw-   0        0        0     1387 2023-07-17 18:50:45.000000 SpotifyUtil-0.0.8/SpotifyUtil/config.py
+-rw-rw-rw-   0        0        0      262 2023-07-16 14:31:36.000000 SpotifyUtil-0.0.8/SpotifyUtil/file_reader.py
+-rw-rw-rw-   0        0        0      177 2023-07-24 17:02:35.000000 SpotifyUtil-0.0.8/SpotifyUtil/secret.py
+-rw-rw-rw-   0        0        0     1594 2023-07-22 17:47:21.000000 SpotifyUtil-0.0.8/SpotifyUtil/utilityTest.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:20:19.510411 SpotifyUtil-0.0.8/SpotifyUtil.egg-info/
+-rw-rw-rw-   0        0        0     2006 2023-07-25 17:20:19.000000 SpotifyUtil-0.0.8/SpotifyUtil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-07-25 17:20:19.000000 SpotifyUtil-0.0.8/SpotifyUtil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 17:20:19.000000 SpotifyUtil-0.0.8/SpotifyUtil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 17:20:19.000000 SpotifyUtil-0.0.8/SpotifyUtil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-25 17:20:19.000000 SpotifyUtil-0.0.8/SpotifyUtil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      795 2023-07-25 17:19:49.000000 SpotifyUtil-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 17:20:19.520532 SpotifyUtil-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-07-25 17:19:53.000000 SpotifyUtil-0.0.8/setup.py
```

### Comparing `SpotifyUtil-0.0.7/LICENSE` & `SpotifyUtil-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.7/PKG-INFO` & `SpotifyUtil-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpotifyUtil
-Version: 0.0.7
+Version: 0.0.8
 Summary: SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.
 Home-page: https://github.com/Arg0naut18/SpotifyUtil
 Author: Arg0naut18
 Author-email: Arg0naut18 <gaming.genos1729@gmail.com>
 Project-URL: Homepage, https://github.com/Arg0naut18/SpotifyUtil
 Keywords: Spotify,Spotipy,SpotifyUtil,SpotifyUtils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SpotifyUtil-0.0.7/README.md` & `SpotifyUtil-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.7/SpotifyUtil/SpotifyUtil.py` & `SpotifyUtil-0.0.8/SpotifyUtil/SpotifyUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from spotipy import Spotify
-from spotipy.oauth2 import SpotifyOAuth
+from spotipy.oauth2 import SpotifyOAuth, CacheFileHandler
 from SpotifyUtil.config import Config
 import os
 import logging
 from SpotifyUtil.file_reader import FileReader
 
 
 log = logging.getLogger(__name__)
@@ -16,17 +16,17 @@
         self.unplayable_uris = unplayable_list
 
 
 class SpotifyUtil(Config):
     """
     A utility that aims to create and modify spotify playlists and albums for you using a single function.
     """
-    def __init__(self, spotify_client_id=None, spotify_client_secret=None, spotify_redirect_uri=None):
+    def __init__(self, spotify_client_id=None, spotify_client_secret=None, spotify_redirect_uri=None, cache_path=None):
         super().__init__(client_id=spotify_client_id, client_secret=spotify_client_secret, redirect_uri=spotify_redirect_uri)
-        self.auth_manager = SpotifyOAuth(client_id=self._client_id, client_secret=self._client_secret, redirect_uri=self._redirect_uri, scope=self._scope_str)
+        self.auth_manager = SpotifyOAuth(client_id=self._client_id, client_secret=self._client_secret, redirect_uri=self._redirect_uri, scope=self._scope_str, cache_handler=CacheFileHandler(cache_path=cache_path))
         self.spotify = Spotify(auth_manager=self.auth_manager)
         self.user = self.spotify.current_user()
         self.user_id = self.user['id']
         log.debug(msg=self.user_id)
 
     def get_track_details(self, url: str):
         song = self.spotify.track(url)
```

### Comparing `SpotifyUtil-0.0.7/SpotifyUtil/config.py` & `SpotifyUtil-0.0.8/SpotifyUtil/config.py`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.7/SpotifyUtil/utilityTest.py` & `SpotifyUtil-0.0.8/SpotifyUtil/utilityTest.py`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.7/SpotifyUtil.egg-info/PKG-INFO` & `SpotifyUtil-0.0.8/SpotifyUtil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpotifyUtil
-Version: 0.0.7
+Version: 0.0.8
 Summary: SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.
 Home-page: https://github.com/Arg0naut18/SpotifyUtil
 Author: Arg0naut18
 Author-email: Arg0naut18 <gaming.genos1729@gmail.com>
 Project-URL: Homepage, https://github.com/Arg0naut18/SpotifyUtil
 Keywords: Spotify,Spotipy,SpotifyUtil,SpotifyUtils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SpotifyUtil-0.0.7/pyproject.toml` & `SpotifyUtil-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SpotifyUtil"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name="Arg0naut18", email="gaming.genos1729@gmail.com" },
 ]
 description = "SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `SpotifyUtil-0.0.7/setup.py` & `SpotifyUtil-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SpotifyUtil",
-    version="0.0.7",
+    version="0.0.8",
     author="Arg0naut18",
     description="SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Arg0naut18/SpotifyUtil",
     packages=setuptools.find_packages(),
     classifiers=[
```

