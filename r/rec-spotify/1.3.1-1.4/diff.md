# Comparing `tmp/rec_spotify-1.3.1.tar.gz` & `tmp/rec_spotify-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rec_spotify-1.3.1.tar", max compression
+gzip compressed data, was "rec_spotify-1.4.tar", max compression
```

## Comparing `rec_spotify-1.3.1.tar` & `rec_spotify-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.3.1/etc/screen.png
--rw-r--r--   0        0        0     1291 2023-07-24 16:18:18.928798 rec_spotify-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2407 2023-07-24 16:16:52.249892 rec_spotify-1.3.1/README.md
--rw-r--r--   0        0        0       23 2023-07-24 16:18:12.934635 rec_spotify-1.3.1/rec_spotify/__init__.py
--rw-r--r--   0        0        0     1735 2023-07-24 09:38:53.871492 rec_spotify-1.3.1/rec_spotify/cli.py
--rw-r--r--   0        0        0     4278 2023-07-24 16:17:06.052316 rec_spotify-1.3.1/rec_spotify/config.py
--rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.3.1/rec_spotify/console.py
--rw-r--r--   0        0        0     7310 2023-07-23 19:42:31.072891 rec_spotify-1.3.1/rec_spotify/database.py
--rw-r--r--   0        0        0     6427 2023-07-23 15:53:09.981754 rec_spotify-1.3.1/rec_spotify/items.py
--rw-r--r--   0        0        0     2195 2023-07-23 16:28:40.968471 rec_spotify-1.3.1/rec_spotify/lyrics.py
--rw-r--r--   0        0        0     6507 2023-07-24 16:04:26.469628 rec_spotify-1.3.1/rec_spotify/manager.py
--rw-r--r--   0        0        0     1968 2023-07-23 16:07:01.827794 rec_spotify-1.3.1/rec_spotify/messages.py
--rw-r--r--   0        0        0     3317 2023-07-23 18:16:28.832707 rec_spotify-1.3.1/rec_spotify/recorder.py
--rw-r--r--   0        0        0     5548 2023-07-24 16:20:37.555003 rec_spotify-1.3.1/rec_spotify/spotify.py
--rw-r--r--   0        0        0     2207 2023-07-24 14:59:10.819037 rec_spotify-1.3.1/rec_spotify/utils.py
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 rec_spotify-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.4/etc/screen.png
+-rw-r--r--   0        0        0     1289 2023-07-25 08:31:43.317279 rec_spotify-1.4/pyproject.toml
+-rw-r--r--   0        0        0     2407 2023-07-24 16:16:52.249892 rec_spotify-1.4/README.md
+-rw-r--r--   0        0        0       21 2023-07-25 08:31:22.204023 rec_spotify-1.4/rec_spotify/__init__.py
+-rw-r--r--   0        0        0     1735 2023-07-24 09:38:53.871492 rec_spotify-1.4/rec_spotify/cli.py
+-rw-r--r--   0        0        0     4278 2023-07-24 16:17:06.052316 rec_spotify-1.4/rec_spotify/config.py
+-rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.4/rec_spotify/console.py
+-rw-r--r--   0        0        0     7310 2023-07-23 19:42:31.072891 rec_spotify-1.4/rec_spotify/database.py
+-rw-r--r--   0        0        0     6427 2023-07-23 15:53:09.981754 rec_spotify-1.4/rec_spotify/items.py
+-rw-r--r--   0        0        0     2195 2023-07-23 16:28:40.968471 rec_spotify-1.4/rec_spotify/lyrics.py
+-rw-r--r--   0        0        0     6507 2023-07-24 16:37:50.030511 rec_spotify-1.4/rec_spotify/manager.py
+-rw-r--r--   0        0        0     1968 2023-07-23 16:07:01.827794 rec_spotify-1.4/rec_spotify/messages.py
+-rw-r--r--   0        0        0     3317 2023-07-23 18:16:28.832707 rec_spotify-1.4/rec_spotify/recorder.py
+-rw-r--r--   0        0        0     6079 2023-07-24 16:58:47.535112 rec_spotify-1.4/rec_spotify/spotify.py
+-rw-r--r--   0        0        0     2207 2023-07-24 14:59:10.819037 rec_spotify-1.4/rec_spotify/utils.py
+-rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 rec_spotify-1.4/PKG-INFO
```

### Comparing `rec_spotify-1.3.1/etc/screen.png` & `rec_spotify-1.4/etc/screen.png`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/pyproject.toml` & `rec_spotify-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rec-spotify"
-version = "1.3.1"
+version = "1.4"
 description = "📻 Record and sync Spotify tracks, albums, and playlists."
 repository = "https://github.com/oSeeLight/rec-spotify"
 authors = ["Jacov Rainz <oSeeLight@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rec_spotify"}]
 include = ["README.md", "etc"]
```

### Comparing `rec_spotify-1.3.1/README.md` & `rec_spotify-1.4/README.md`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/cli.py` & `rec_spotify-1.4/rec_spotify/cli.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/config.py` & `rec_spotify-1.4/rec_spotify/config.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/console.py` & `rec_spotify-1.4/rec_spotify/console.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/database.py` & `rec_spotify-1.4/rec_spotify/database.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/items.py` & `rec_spotify-1.4/rec_spotify/items.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/lyrics.py` & `rec_spotify-1.4/rec_spotify/lyrics.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/manager.py` & `rec_spotify-1.4/rec_spotify/manager.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/messages.py` & `rec_spotify-1.4/rec_spotify/messages.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/recorder.py` & `rec_spotify-1.4/rec_spotify/recorder.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/rec_spotify/spotify.py` & `rec_spotify-1.4/rec_spotify/spotify.py`

 * *Files 20% similar despite different names*

```diff
@@ -106,17 +106,29 @@
             "title": track.name,
             "artist": track.artist,
             "album": song["album"]["name"],
             "date": song["album"]["release_date"],
             "track": song["track_number"],
             "cover_url": song["album"]["images"][0]["url"],
         }
+        genres = cls._get_song_genre(song)
+        if genres:
+            data["genre"] = genres
         return data
 
     @classmethod
+    def _get_song_genre(cls, data: dict) -> str:
+        artist_ids = [artist["id"] for artist in data["artists"]]
+        artists = cls._make_request(cls._client.artists, artist_ids)
+        artists = artists["artists"]
+        genres = [artist["genres"] for artist in artists if artist["genres"]]
+        genres_str = "; ".join(x.title() for artist in genres for x in artist)
+        return genres_str
+
+    @classmethod
     def _extract_artist(cls, track_artists: dict) -> str:
         if len(track_artists) > 1:
             artists = ""
             for artist in track_artists:
                 artists += f"{artist['name']}, "
             return artists.strip()[0:-1]
         else:
```

### Comparing `rec_spotify-1.3.1/rec_spotify/utils.py` & `rec_spotify-1.4/rec_spotify/utils.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.3.1/PKG-INFO` & `rec_spotify-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rec-spotify
-Version: 1.3.1
+Version: 1.4
 Summary: 📻 Record and sync Spotify tracks, albums, and playlists.
 Home-page: https://github.com/oSeeLight/rec-spotify
 License: MIT
 Keywords: spotify,record
 Author: Jacov Rainz
 Author-email: oSeeLight@proton.me
 Requires-Python: >=3.11,<4.0
```

