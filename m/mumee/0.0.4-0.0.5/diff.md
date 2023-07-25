# Comparing `tmp/mumee-0.0.4.tar.gz` & `tmp/mumee-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mumee-0.0.4.tar", max compression
+gzip compressed data, was "mumee-0.0.5.tar", max compression
```

## Comparing `mumee-0.0.4.tar` & `mumee-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,36 @@
--rw-r--r--   0        0        0     1063 2023-07-19 09:03:39.990929 mumee-0.0.4/LICENSE
--rw-r--r--   0        0        0     2311 2023-07-19 09:03:39.990929 mumee-0.0.4/README.md
--rw-r--r--   0        0        0      520 2023-07-19 09:03:39.990929 mumee-0.0.4/mumee/__init__.py
--rw-r--r--   0        0        0      328 2023-07-19 09:03:39.990929 mumee-0.0.4/mumee/classes/__init__.py
--rw-r--r--   0        0        0      180 2023-07-19 09:03:39.990929 mumee-0.0.4/mumee/classes/clients/__init__.py
--rw-r--r--   0        0        0     5715 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/clients/spotify_metadata_client.py
--rw-r--r--   0        0        0     5439 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/clients/ytmusic_metadata_client.py
--rw-r--r--   0        0        0       74 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/config/__init__.py
--rw-r--r--   0        0        0      419 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/config/spotify_options.py
--rw-r--r--   0        0        0      532 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/__init__.py
--rw-r--r--   0        0        0      705 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/spotify_playlist_handler.py
--rw-r--r--   0        0        0      652 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/spotify_search_handler.py
--rw-r--r--   0        0        0      693 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/spotify_track_handler.py
--rw-r--r--   0        0        0      711 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/ytmusic_playlist_handler.py
--rw-r--r--   0        0        0      652 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/ytmusic_search_handler.py
--rw-r--r--   0        0        0      696 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/handlers/ytmusic_track_handler.py
--rw-r--r--   0        0        0      249 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/playlist_metadata.py
--rw-r--r--   0        0        0      557 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/classes/song_metadata.py
--rw-r--r--   0        0        0       68 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/di/__init__.py
--rw-r--r--   0        0        0      800 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/di/dependency_injector.py
--rw-r--r--   0        0        0       90 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/errors/__init__.py
--rw-r--r--   0        0        0       83 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/errors/metadata_client_error.py
--rw-r--r--   0        0        0       87 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/interfaces/__init__.py
--rw-r--r--   0        0        0      231 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/interfaces/base_metadata_client.py
--rw-r--r--   0        0        0      904 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/main.py
--rw-r--r--   0        0        0        0 2023-07-19 09:03:39.994929 mumee-0.0.4/mumee/py.typed
--rw-r--r--   0        0        0     1324 2023-07-19 09:03:39.994929 mumee-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3440 1970-01-01 00:00:00.000000 mumee-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-25 19:05:10.630209 mumee-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3347 2023-07-25 19:05:10.630209 mumee-0.0.5/README.md
+-rw-r--r--   0        0        0      677 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/clients/__init__.py
+-rw-r--r--   0        0        0     5710 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/clients/spotify_metadata_client.py
+-rw-r--r--   0        0        0     5570 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/clients/ytmusic_metadata_client.py
+-rw-r--r--   0        0        0       74 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/config/__init__.py
+-rw-r--r--   0        0        0      419 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/config/spotify_options.py
+-rw-r--r--   0        0        0      493 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/fetch/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/fetch/spotify_playlist_handler.py
+-rw-r--r--   0        0        0      676 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/fetch/spotify_search_handler.py
+-rw-r--r--   0        0        0      711 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/fetch/spotify_track_handler.py
+-rw-r--r--   0        0        0      729 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/fetch/ytmusic_playlist_handler.py
+-rw-r--r--   0        0        0      676 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/fetch/ytmusic_search_handler.py
+-rw-r--r--   0        0        0      714 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/fetch/ytmusic_track_handler.py
+-rw-r--r--   0        0        0      186 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/search/__init__.py
+-rw-r--r--   0        0        0     1271 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/search/spotify_explorer_handler.py
+-rw-r--r--   0        0        0     1279 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/classes/handlers/search/ytmusic_explorer_handler.py
+-rw-r--r--   0        0        0      311 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/data/__init__.py
+-rw-r--r--   0        0        0      134 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/data/metadata_clients.py
+-rw-r--r--   0        0        0      246 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/data/playlist_metadata.py
+-rw-r--r--   0        0        0      318 2023-07-25 19:05:10.630209 mumee-0.0.5/mumee/data/search_metadata_command.py
+-rw-r--r--   0        0        0      557 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/data/song_metadata.py
+-rw-r--r--   0        0        0       68 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/di/__init__.py
+-rw-r--r--   0        0        0      963 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/di/dependency_injector.py
+-rw-r--r--   0        0        0       90 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/errors/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/errors/metadata_client_error.py
+-rw-r--r--   0        0        0      168 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/interfaces/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/interfaces/base_metadata_client.py
+-rw-r--r--   0        0        0      235 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/interfaces/base_metadata_explorer.py
+-rw-r--r--   0        0        0     1376 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/main.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:05:10.634209 mumee-0.0.5/mumee/py.typed
+-rw-r--r--   0        0        0     1324 2023-07-25 19:05:10.634209 mumee-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4476 1970-01-01 00:00:00.000000 mumee-0.0.5/PKG-INFO
```

### Comparing `mumee-0.0.4/LICENSE` & `mumee-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mumee-0.0.4/README.md` & `mumee-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -30,49 +30,80 @@
 
 ## Usage
 
 There are 2 ways to use this library : using the `SongMetadataClient` object or via the DI.
 
 ### Using SongMetadataClient
 
-The library exposes the `SongMetadataClient` class. This class has 1 methods : `search`.
+The library exposes the `SongMetadataClient` class. This class has 2 methods : `fetch` and `search`.
 
-This method fetches the metadata corresponding to the request you give it, whether it is an URL or a query. It returns the result as a `SongMetadata` object or a `PlaylistMetadata` object.
+The `fetch` method fetches the metadata corresponding to the request you give it, whether it is an URL or a query. It returns the result as a `SongMetadata` object or a `PlaylistMetadata` object.
 
 **Example :**
 
 ```python
 from mumee import SongMetadataClient
 
 client = SongMetadataClient()
-result = client.search("in the end - linkin park")
+result = client.fetch("https://open.spotify.com/track/7AB0cUXnzuSlAnyHOqmrZr")
 
-title = result.title # In The End
+title = result.title # Faint
+artists = result.artists # ['Linkin Park']
+```
+
+The `search` method expects a query (e.g.: {title} - {artists}) and a limit corresponding to the number of results you want. It returns a list of `SongMetadata` objects that fit closest to the query that was given. This list is sorted by closest fit per client.
+
+**Example :**
+
+```python
+from mumee import SongMetadataClient
+
+client = SongMetadataClient()
+results = client.search("in the end - linkin park")
+
+title = results[0].title # In The End
+artists = results[0].artists # ['Linkin Park']
 ```
 
 ### Using DI
 
-The library also exposes a `BaseMetadataClient` interface and a `add_mumee` function for [Taipan-DI](https://github.com/Billuc/Taipan-DI).
+The library also exposes the `BaseMetadataClient` and `BaseMetadataExplorer` interfaces and a `add_mumee` function for [Taipan-DI](https://github.com/Billuc/Taipan-DI).
 
-In this function, the clients are registered as a Pipeline. All you need to do is to resolve the pipeline and execute it.
+In this function, the clients and explorers are registered as a Pipeline. All you need to do is to resolve the pipelines and execute it.
 
-**Example :**
+**Example 1 :**
 
 ```python
 from mumee import BaseMetadataClient, add_mumee
 from taipan_di import DependencyCollection
 
 services = DependencyCollection()
 add_mumee(services)
 
 provider = services.build()
 client = provider.resolve(BaseMetadataClient)
 
-result = client.exec("in the end - linkin park")
-title = result.title # In The End
+result = client.exec("https://open.spotify.com/track/7AB0cUXnzuSlAnyHOqmrZr")
+title = result.title # Faint
+```
+
+**Example 2 :**
+
+```python
+from mumee import BaseMetadataExplorer, add_mumee
+from taipan_di import DependencyCollection
+
+services = DependencyCollection()
+add_mumee(services)
+
+provider = services.build()
+explorer = provider.resolve(BaseMetadataExplorer)
+
+results = explorer.exec("in the end - linkin park")
+title = results[0].title # In The End
 ```
 
 ## Inspirations
 
 This library is partially based on spotDL's [spotify-downloader](https://github.com/spotDL/spotify-downloader).
 
 ## TODO
@@ -80,8 +111,9 @@
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
 - Support for Amazon Music
 - More metadata in the SongMetadata class
-- Allow return of multiple results
+- Handle edge case in explorer_handler
+- Re-sort explorer results
```

### Comparing `mumee-0.0.4/mumee/__init__.py` & `mumee-0.0.5/mumee/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .classes import (
-    SongMetadata,
-    PlaylistMetadata,
     SpotifyOptions,
     SpotifyMetadataClient,
     YTMusicMetadataClient,
 )
+from .data import SearchMetadataCommand, SongMetadata, MetadataClientEnum, PlaylistMetadata
 from .di import add_mumee
 from .errors import MetadataClientError
-from .interfaces import BaseMetadataClient
+from .interfaces import BaseMetadataClient, BaseMetadataExplorer
 from .main import SongMetadataClient
 
 __all__ = [
     "add_mumee",
     "SongMetadataClient",
     "BaseMetadataClient",
+    "BaseMetadataExplorer",
     "MetadataClientError",
     "SongMetadata",
     "PlaylistMetadata",
+    "SearchMetadataCommand",
+    "MetadataClientEnum",
     "SpotifyOptions",
     "SpotifyMetadataClient",
     "YTMusicMetadataClient",
 ]
```

### Comparing `mumee-0.0.4/mumee/classes/clients/spotify_metadata_client.py` & `mumee-0.0.5/mumee/classes/clients/ytmusic_metadata_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,160 +1,139 @@
 from typing import Any, Dict, List, Tuple
-from spotipy import (
-    Spotify,
-    CacheFileHandler,
-    MemoryCacheHandler,
-    SpotifyOAuth,
-    SpotifyClientCredentials,
-)
+from ytmusicapi import YTMusic
 from rapidfuzz import fuzz
 from slugify import slugify
 
-from mumee.classes import SongMetadata, SpotifyOptions, PlaylistMetadata
+from mumee.data import SongMetadata, PlaylistMetadata
 from mumee.errors import MetadataClientError
 
-__all__ = ["SpotifyMetadataClient"]
+__all__ = ["YTMusicMetadataClient"]
 
 
-class SpotifyMetadataClient:
-    def __init__(self, options: SpotifyOptions) -> None:
-        cache_handler = (
-            CacheFileHandler(options.cache_path)
-            if options.use_cache
-            else MemoryCacheHandler()
-        )
-
-        if options.auth_token is not None:
-            credentials_manager = None
-        elif options.use_auth:
-            credentials_manager = SpotifyOAuth(
-                client_id=options.client_id,
-                client_secret=options.client_secret,
-                redirect_uri="http://127.0.0.1:8080/",
-                scope="user-library-read",
-                cache_handler=cache_handler,
-                open_browser=not options.headless,
-            )
-        else:
-            credentials_manager = SpotifyClientCredentials(
-                client_id=options.client_id,
-                client_secret=options.client_secret,
-                cache_handler=cache_handler,
-            )
-
-        self._client = Spotify(
-            auth=options.auth_token,
-            auth_manager=credentials_manager,
-            status_forcelist=(429, 500, 502, 503, 504, 404),
-        )
+class YTMusicMetadataClient:
+    def __init__(self) -> None:
+        self._client = YTMusic()
 
     def get_track(self, url: str) -> SongMetadata:
-        if "open.spotify.com" not in url or "track" not in url:
-            raise MetadataClientError(f"Invalid Spotify track URL: {url}")
+        if "music.youtube.com" not in url or "watch?v" not in url:
+            raise MetadataClientError(f"Invalid Youtube Music track URL: {url}")
 
-        track_info = self._client.track(url)
+        start_index = url.find("?v=") + len("?v=")
+        end_index = url.find("&", start_index) if url.find("&", start_index) >= 0 else None
+        track_info = self._client.get_song(url[start_index:end_index])
 
-        if track_info is None:
+        if not track_info or track_info["playabilityStatus"]["status"] == "ERROR":
             raise MetadataClientError(
                 f"Couldn't get metadata associated with this URL: {url}"
             )
 
-        if track_info["duration_ms"] == 0 or track_info["name"].strip() == "":
-            raise MetadataClientError(f"Track no longer exists: {url}")
-
-        return self._to_song_metadata(track_info)
-
-    def _to_song_metadata(self, track_info: Dict[str, Any]) -> SongMetadata:
-        artist_names = [artist["name"] for artist in track_info["artists"]]
-        album_info = self._client.album(track_info["album"]["id"]) or {}
-
-        thumbnails = [
-            (tn["width"] * tn["height"], tn["url"]) for tn in album_info["images"]
-        ]
-
-        result = SongMetadata(
-            name=track_info["name"],
-            artists=artist_names,
-            artist=artist_names[0],
-            album_name=album_info["name"],
-            album_artist=album_info["artists"][0]["name"],
-            disc_number=track_info["disc_number"],
-            disc_count=int(album_info["tracks"]["items"][-1]["disc_number"]),
-            track_number=track_info["track_number"],
-            track_count=album_info["total_tracks"],
-            genres=album_info["genres"],
-            duration=int(track_info["duration_ms"] / 1000),
-            date=album_info["release_date"],
-            year=int(album_info["release_date"][:4]),
-            is_song=True,
-            id=track_info["id"],
-            explicit=track_info["explicit"],
-            cover_url=max(thumbnails)[1],
-            url=track_info["external_urls"]["spotify"],
+        track_data = self.search(
+            f"{track_info['videoDetails']['title']} - {track_info['videoDetails']['author']}",
+            1,
         )
-
-        return result
+        return track_data[0]
 
     def get_playlist(self, url: str) -> PlaylistMetadata:
-        if "open.spotify.com" not in url or "playlist" not in url:
-            raise MetadataClientError(f"Invalid Spotify playlist URL: {url}")
+        if "music.youtube.com" not in url or "playlist?list" not in url:
+            raise MetadataClientError(f"Invalid Youtube Music playlist URL: {url}")
 
-        track_info = self._client.playlist(url)
+        start_index = url.find("?list=") + len("?list=")
+        end_index = url.find("&", start_index) if url.find("&", start_index) >= 0 else None
+        playlist_info = self._client.get_playlist(url[start_index:end_index], None)  # type: ignore
 
-        if track_info is None:
+        if not playlist_info:
             raise MetadataClientError(
                 f"Couldn't get metadata associated with this URL: {url}"
             )
 
         result = PlaylistMetadata(
-            name=track_info["name"],
-            description=track_info["description"],
-            author=track_info["owner"]["display_name"],
+            name=playlist_info["title"],
+            description=playlist_info["description"],
+            author=playlist_info["author"]["name"],
             tracks=[
-                self._to_song_metadata(track["track"])
-                for track in track_info["tracks"]["items"]
+                self.search(
+                    f"{track['title']} - {', '.join([artist['name'] for artist in track['artists']])}",
+                    1,
+                )[0]
+                for track in playlist_info["tracks"]
             ],
         )
         return result
 
-    def search(self, query: str) -> SongMetadata:
-        search_results = self._client.search(query)
+    def search(self, query: str, limit: int) -> List[SongMetadata]:
+        search_results = self._client.search(query, "songs", limit=limit)
 
-        if search_results is None or len(search_results["tracks"]["items"]) == 0:
-            raise MetadataClientError("No result found for '{query}'")
+        if search_results is None or len(search_results) == 0:
+            raise MetadataClientError(f"No result found for '{query}'")
 
-        best_result = self._get_best_result(query, search_results["tracks"]["items"])
+        best_results = self._get_best_results(query, search_results, limit)
 
-        if best_result[2] < 55:
+        if not best_results or best_results[0][2] < 55:
             raise MetadataClientError(
                 "Best match found isn't close enough to your query. "
-                f"Best match : {best_result[1]}, query: {query}"
+                f"Best match : {best_results[0][1]}, query: {query}"
             )
 
-        song_url = "http://open.spotify.com/track/" + best_result[0]
-        return self.get_track(song_url)
+        results = [self._dict_to_song(track[0]) for track in best_results]
+        return results
 
-    def _get_best_result(
-        self, query: str, tracks_info: List[Dict[str, Any]]
-    ) -> Tuple[str, str, float]:
-        best_score = 0
-        best_id = ""
-        best_query = ""
-        best_popularity = 0
+    def _get_best_results(
+        self, query: str, tracks_info: List[Dict[str, Any]], limit: int
+    ) -> List[Tuple[Dict[str, Any], str, float, bool]]:
+        track_infos: List[Tuple[Dict[str, Any], str, float, bool]] = []
 
         for track in tracks_info:
-            track_name = track["name"]
+            track_name = track["title"]
             track_artists = [artist["name"] for artist in track["artists"]]
             track_query = f"{track_name} - {', '.join(track_artists)}"
-            track_popularity = track["popularity"]
+            track_has_album = (
+                track["album"] is not None and track["album"]["id"] is not None
+            )
 
             score = fuzz.ratio(slugify(track_query), slugify(query))
 
-            if score > best_score or (
-                score == best_score and track_popularity > best_popularity
-            ):
-                best_score = score
-                best_id = track["id"]
-                best_query = track_query
-                best_popularity = track_popularity
+            track_infos.append((track, track_query, score, track_has_album))
+
+        track_infos = sorted(track_infos, key=lambda t: (t[2], t[3]), reverse=True)
+
+        return track_infos[:limit]
+
+    def _dict_to_song(self, track_info: Dict[str, Any]) -> SongMetadata:
+        if track_info.get("album", {}).get("id") is not None:
+            album_info = self._client.get_album(track_info["album"]["id"])
+        else:
+            album_info = None
+
+        thumbnails = [
+            (tn["width"] * tn["height"], tn["url"])
+            for tn in (album_info if album_info else track_info)["thumbnails"]
+        ]
 
-        return best_id, best_query, best_score
+        result = SongMetadata(
+            name=track_info["title"],
+            artists=[artist["name"] for artist in track_info["artists"]],
+            artist=track_info["artists"][0]["name"],
+            album_name=album_info["title"] if album_info is not None else None,
+            album_artist=album_info["artists"][0]["name"]
+            if album_info is not None
+            else None,
+            disc_number=None,
+            disc_count=None,
+            track_number=[
+                idx
+                for idx, track in enumerate(album_info["tracks"])
+                if fuzz.ratio(track["title"], track_info["title"]) > 80
+            ][0]
+            if album_info is not None
+            else None,
+            track_count=album_info["trackCount"] if album_info is not None else None,
+            genres=[],
+            duration=track_info["duration_seconds"],
+            date=None,
+            year=int(album_info["year"]) if album_info is not None else None,
+            explicit=track_info["isExplicit"],
+            cover_url=max(thumbnails)[1],
+            is_song=track_info["resultType"] == "song",
+            id=track_info["videoId"],
+            url=f"https://{'music' if track_info['resultType'] == 'song' else 'www'}.youtube.com/watch?v={track_info['videoId']}",
+        )
+        return result
```

### Comparing `mumee-0.0.4/mumee/classes/clients/ytmusic_metadata_client.py` & `mumee-0.0.5/mumee/classes/clients/spotify_metadata_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,141 +1,158 @@
 from typing import Any, Dict, List, Tuple
-from ytmusicapi import YTMusic
+from spotipy import (
+    Spotify,
+    CacheFileHandler,
+    MemoryCacheHandler,
+    SpotifyOAuth,
+    SpotifyClientCredentials,
+)
 from rapidfuzz import fuzz
 from slugify import slugify
 
-from mumee.classes import SongMetadata, PlaylistMetadata
+from mumee.classes import SpotifyOptions
+from mumee.data import SongMetadata, PlaylistMetadata
 from mumee.errors import MetadataClientError
 
-__all__ = ["YTMusicMetadataClient"]
+__all__ = ["SpotifyMetadataClient"]
 
 
-class YTMusicMetadataClient:
-    def __init__(self) -> None:
-        self._client = YTMusic()
+class SpotifyMetadataClient:
+    def __init__(self, options: SpotifyOptions) -> None:
+        cache_handler = (
+            CacheFileHandler(options.cache_path)
+            if options.use_cache
+            else MemoryCacheHandler()
+        )
+
+        if options.auth_token is not None:
+            credentials_manager = None
+        elif options.use_auth:
+            credentials_manager = SpotifyOAuth(
+                client_id=options.client_id,
+                client_secret=options.client_secret,
+                redirect_uri="http://127.0.0.1:8080/",
+                scope="user-library-read",
+                cache_handler=cache_handler,
+                open_browser=not options.headless,
+            )
+        else:
+            credentials_manager = SpotifyClientCredentials(
+                client_id=options.client_id,
+                client_secret=options.client_secret,
+                cache_handler=cache_handler,
+            )
+
+        self._client = Spotify(
+            auth=options.auth_token,
+            auth_manager=credentials_manager,
+            status_forcelist=(429, 500, 502, 503, 504, 404),
+        )
 
     def get_track(self, url: str) -> SongMetadata:
-        if "music.youtube.com" not in url or "watch?v" not in url:
-            raise MetadataClientError(f"Invalid Youtube Music track URL: {url}")
+        if "open.spotify.com" not in url or "track" not in url:
+            raise MetadataClientError(f"Invalid Spotify track URL: {url}")
 
-        start_index = url.find("?v=") + len("?v=")
-        end_index = url.find("&", start_index) if url.find("&", start_index) >= 0 else None
-        track_info = self._client.get_song(url[start_index:end_index])
+        track_info = self._client.track(url)
 
-        if not track_info or track_info["playabilityStatus"]["status"] == "ERROR":
+        if track_info is None:
             raise MetadataClientError(
                 f"Couldn't get metadata associated with this URL: {url}"
             )
 
-        return self.search(
-            f"{track_info['videoDetails']['title']} - {track_info['videoDetails']['author']}"
+        if track_info["duration_ms"] == 0 or track_info["name"].strip() == "":
+            raise MetadataClientError(f"Track no longer exists: {url}")
+
+        return self._to_song_metadata(track_info)
+
+    def _to_song_metadata(self, track_info: Dict[str, Any]) -> SongMetadata:
+        artist_names = [artist["name"] for artist in track_info["artists"]]
+        album_info = self._client.album(track_info["album"]["id"]) or {}
+
+        thumbnails = [
+            (tn["width"] * tn["height"], tn["url"]) for tn in album_info["images"]
+        ]
+
+        result = SongMetadata(
+            name=track_info["name"],
+            artists=artist_names,
+            artist=artist_names[0],
+            album_name=album_info["name"],
+            album_artist=album_info["artists"][0]["name"],
+            disc_number=track_info["disc_number"],
+            disc_count=int(album_info["tracks"]["items"][-1]["disc_number"]),
+            track_number=track_info["track_number"],
+            track_count=album_info["total_tracks"],
+            genres=album_info["genres"],
+            duration=int(track_info["duration_ms"] / 1000),
+            date=album_info["release_date"],
+            year=int(album_info["release_date"][:4]),
+            is_song=True,
+            id=track_info["id"],
+            explicit=track_info["explicit"],
+            cover_url=max(thumbnails)[1],
+            url=track_info["external_urls"]["spotify"],
         )
 
+        return result
+
     def get_playlist(self, url: str) -> PlaylistMetadata:
-        if "music.youtube.com" not in url or "playlist?list" not in url:
-            raise MetadataClientError(f"Invalid Youtube Music playlist URL: {url}")
+        if "open.spotify.com" not in url or "playlist" not in url:
+            raise MetadataClientError(f"Invalid Spotify playlist URL: {url}")
 
-        start_index = url.find("?list=") + len("?list=")
-        end_index = url.find("&", start_index) if url.find("&", start_index) >= 0 else None
-        playlist_info = self._client.get_playlist(url[start_index:end_index], None)  # type: ignore
+        track_info = self._client.playlist(url)
 
-        if not playlist_info:
+        if track_info is None:
             raise MetadataClientError(
                 f"Couldn't get metadata associated with this URL: {url}"
             )
 
         result = PlaylistMetadata(
-            name=playlist_info["title"],
-            description=playlist_info["description"],
-            author=playlist_info["author"]["name"],
+            name=track_info["name"],
+            description=track_info["description"],
+            author=track_info["owner"]["display_name"],
             tracks=[
-                self.search(
-                    f"{track['title']} - {', '.join([artist['name'] for artist in track['artists']])}"
-                )
-                for track in playlist_info["tracks"]
+                self._to_song_metadata(track["track"])
+                for track in track_info["tracks"]["items"]
             ],
         )
         return result
 
-    def search(self, query: str) -> SongMetadata:
-        search_results = self._client.search(query, "songs")
+    def search(self, query: str, limit: int) -> List[SongMetadata]:
+        search_results = self._client.search(query)
 
-        if search_results is None or len(search_results) == 0:
-            raise MetadataClientError(f"No result found for '{query}'")
+        if search_results is None or len(search_results["tracks"]["items"]) == 0:
+            raise MetadataClientError("No result found for '{query}'")
 
-        best_result = self._get_best_result(query, search_results)
+        best_results = self._get_best_results(
+            query, search_results["tracks"]["items"], limit
+        )
 
-        if best_result[2] < 55:
+        if not best_results or best_results[0][2] < 55:
             raise MetadataClientError(
                 "Best match found isn't close enough to your query. "
-                f"Best match : {best_result[1]}, query: {query}"
+                f"Best match : {best_results[0][1]}, query: {query}"
             )
 
-        track_info = best_result[0]
-        if track_info.get("album", {}).get("id") is not None:
-            album_info = self._client.get_album(track_info["album"]["id"])
-        else:
-            album_info = None
-
-        thumbnails = [
-            (tn["width"] * tn["height"], tn["url"])
-            for tn in (album_info if album_info else track_info)["thumbnails"]
+        track_infos = [
+            self.get_track("http://open.spotify.com/track/" + track[0])
+            for track in best_results
         ]
+        return track_infos
 
-        result = SongMetadata(
-            name=track_info["title"],
-            artists=[artist["name"] for artist in track_info["artists"]],
-            artist=track_info["artists"][0]["name"],
-            album_name=album_info["title"] if album_info is not None else None,
-            album_artist=album_info["artists"][0]["name"]
-            if album_info is not None
-            else None,
-            disc_number=None,
-            disc_count=None,
-            track_number=[
-                idx
-                for idx, track in enumerate(album_info["tracks"])
-                if fuzz.ratio(track["title"], track_info["title"]) > 80
-            ][0]
-            if album_info is not None
-            else None,
-            track_count=album_info["trackCount"] if album_info is not None else None,
-            genres=[],
-            duration=track_info["duration_seconds"],
-            date=None,
-            year=int(album_info["year"]) if album_info is not None else None,
-            explicit=track_info["isExplicit"],
-            cover_url=max(thumbnails)[1],
-            is_song=track_info["resultType"] == "song",
-            id=track_info["videoId"],
-            url=f"https://{'music' if track_info['resultType'] == 'song' else 'www'}.youtube.com/watch?v={track_info['videoId']}",
-        )
-
-        return result
-
-    def _get_best_result(
-        self, query: str, tracks_info: List[Dict[str, Any]]
-    ) -> Tuple[Dict[str, Any], str, float]:
-        best_score = 0
-        best_result = None
-        best_query = ""
-        has_album = False
+    def _get_best_results(
+        self, query: str, tracks_info: List[Dict[str, Any]], limit: int
+    ) -> List[Tuple[str, str, float, float]]:
+        results: List[Tuple[str, str, float, float]] = []
 
         for track in tracks_info:
-            track_name = track["title"]
+            track_name = track["name"]
             track_artists = [artist["name"] for artist in track["artists"]]
             track_query = f"{track_name} - {', '.join(track_artists)}"
-            track_has_album = (
-                track["album"] is not None and track["album"]["id"] is not None
-            )
+            track_popularity = track["popularity"]
 
             score = fuzz.ratio(slugify(track_query), slugify(query))
 
-            if score > best_score or (
-                score == best_score and track_has_album and not has_album
-            ):
-                best_score = score
-                best_result = track
-                best_query = track_query
-                has_album = track_has_album
+            results.append((track["id"], track_query, score, track_popularity))
 
-        return best_result or {}, best_query, best_score
+        results = sorted(results, key=lambda t: (t[2], t[3]), reverse=True)
+        return results[:limit]
```

### Comparing `mumee-0.0.4/mumee/classes/handlers/__init__.py` & `mumee-0.0.5/mumee/classes/handlers/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.4/mumee/classes/handlers/spotify_playlist_handler.py` & `mumee-0.0.5/mumee/classes/handlers/fetch/spotify_playlist_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from mumee.interfaces import BaseMetadataClient
-from mumee.classes import (
-    SpotifyMetadataClient,
+from mumee.classes import SpotifyMetadataClient
+from mumee.data import (
     SongMetadata,
     PlaylistMetadata,
 )
 
 __all__ = ["SpotifyPlaylistHandler"]
```

### Comparing `mumee-0.0.4/mumee/classes/handlers/spotify_search_handler.py` & `mumee-0.0.5/mumee/classes/handlers/fetch/spotify_search_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from mumee.interfaces import BaseMetadataClient
-from mumee.classes import (
-    SpotifyMetadataClient,
+from mumee.classes import SpotifyMetadataClient
+from mumee.data import (
     SongMetadata,
     PlaylistMetadata,
 )
 
 __all__ = ["SpotifySearchHandler"]
 
 
@@ -15,10 +15,10 @@
         super().__init__()
         self._client = client
 
     def _handle(
         self, request: str, next: Callable[[str], Union[SongMetadata, PlaylistMetadata]]
     ) -> Union[SongMetadata, PlaylistMetadata]:
         try:
-            return self._client.search(request)
+            return self._client.search(request, 1)[0]
         except:
             return next(request)
```

### Comparing `mumee-0.0.4/mumee/classes/handlers/spotify_track_handler.py` & `mumee-0.0.5/mumee/classes/handlers/fetch/spotify_track_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from mumee.interfaces import BaseMetadataClient
-from mumee.classes import (
-    SpotifyMetadataClient,
+from mumee.classes import SpotifyMetadataClient
+from mumee.data import (
     SongMetadata,
     PlaylistMetadata,
 )
 
 __all__ = ["SpotifyTrackHandler"]
```

### Comparing `mumee-0.0.4/mumee/classes/handlers/ytmusic_playlist_handler.py` & `mumee-0.0.5/mumee/classes/handlers/fetch/ytmusic_playlist_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from mumee.interfaces import BaseMetadataClient
-from mumee.classes import (
-    YTMusicMetadataClient,
+from mumee.classes import YTMusicMetadataClient
+from mumee.data import (
     SongMetadata,
     PlaylistMetadata,
 )
 
 __all__ = ["YTMusicPlaylistHandler"]
```

### Comparing `mumee-0.0.4/mumee/classes/handlers/ytmusic_search_handler.py` & `mumee-0.0.5/mumee/classes/handlers/fetch/ytmusic_search_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from mumee.interfaces import BaseMetadataClient
-from mumee.classes import (
-    YTMusicMetadataClient,
+from mumee.classes import YTMusicMetadataClient
+from mumee.data import (
     SongMetadata,
     PlaylistMetadata,
 )
 
 __all__ = ["YTMusicSearchHandler"]
 
 
@@ -15,10 +15,10 @@
         super().__init__()
         self._client = client
 
     def _handle(
         self, request: str, next: Callable[[str], Union[SongMetadata, PlaylistMetadata]]
     ) -> Union[SongMetadata, PlaylistMetadata]:
         try:
-            return self._client.search(request)
+            return self._client.search(request, 1)[0]
         except:
             return next(request)
```

### Comparing `mumee-0.0.4/mumee/classes/handlers/ytmusic_track_handler.py` & `mumee-0.0.5/mumee/classes/handlers/fetch/ytmusic_track_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union
 
 from mumee.interfaces import BaseMetadataClient
-from mumee.classes import (
-    YTMusicMetadataClient,
+from mumee.classes import YTMusicMetadataClient
+from mumee.data import (
     SongMetadata,
     PlaylistMetadata,
 )
 
 __all__ = ["YTMusicTrackHandler"]
```

### Comparing `mumee-0.0.4/mumee/classes/song_metadata.py` & `mumee-0.0.5/mumee/data/song_metadata.py`

 * *Files identical despite different names*

### Comparing `mumee-0.0.4/mumee/di/dependency_injector.py` & `mumee-0.0.5/mumee/di/dependency_injector.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 
 from mumee.classes import (
     SpotifyOptions,
     SpotifyMetadataClient,
     YTMusicMetadataClient,
 )
 from mumee.classes.handlers import *
-from mumee.interfaces import BaseMetadataClient
+from mumee.interfaces import BaseMetadataClient, BaseMetadataExplorer
 
 __all__ = ["add_mumee"]
 
 
 def add_mumee(services: ServiceCollection) -> ServiceCollection:
     services.register(SpotifyOptions).as_singleton().with_self()
 
-    services.register(SpotifyMetadataClient).as_factory().with_self()
-    services.register(YTMusicMetadataClient).as_factory().with_self()
+    services.register(SpotifyMetadataClient).as_singleton().with_self()
+    services.register(YTMusicMetadataClient).as_singleton().with_self()
 
     services.register_pipeline(BaseMetadataClient).add(SpotifyTrackHandler).add(
         SpotifyPlaylistHandler
     ).add(YTMusicTrackHandler).add(YTMusicPlaylistHandler).add(SpotifySearchHandler).add(
         YTMusicSearchHandler
     ).as_factory()
 
+    services.register_pipeline(BaseMetadataExplorer).add(SpotifyExplorerHandler).add(
+        YTMusicExplorerHandler
+    ).as_factory()
+
     return services
```

### Comparing `mumee-0.0.4/mumee/main.py` & `mumee-0.0.5/mumee/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,38 @@
-from typing import Optional, Union
+from typing import List, Optional, Union
 from taipan_di import ServiceCollection
 
-from mumee.classes import SongMetadata, PlaylistMetadata, SpotifyOptions
+from mumee.classes import SpotifyOptions
+from mumee.data import SongMetadata, PlaylistMetadata, SearchMetadataCommand, MetadataClientEnum
 from mumee.di import add_mumee
-from mumee.interfaces import BaseMetadataClient
+from mumee.interfaces import BaseMetadataClient, BaseMetadataExplorer
 from mumee.errors import MetadataClientError
 
 
 class SongMetadataClient:
     def __init__(self, spotify_options: Optional[SpotifyOptions] = None):
         services = ServiceCollection()
         add_mumee(services)
 
         if spotify_options is not None:
             services.register(SpotifyOptions).as_singleton().with_instance(spotify_options)
 
-        self._client = services.build().resolve(BaseMetadataClient)
+        provider = services.build()
 
-    def search(self, url_or_query: str) -> Union[SongMetadata, PlaylistMetadata]:
-        result = self._client.exec(url_or_query)
+        self._fetcher = provider.resolve(BaseMetadataClient)
+        self._explorer = provider.resolve(BaseMetadataExplorer)
+
+    def fetch(self, url_or_query: str) -> Union[SongMetadata, PlaylistMetadata]:
+        result = self._fetcher.exec(url_or_query)
 
         if result is None:
             raise MetadataClientError(f"No result for query {url_or_query}")
 
         return result
+
+    def search(
+        self, query: str, limit: int, clients: List[MetadataClientEnum] = [MetadataClientEnum.ALL]
+    ) -> List[SongMetadata]:
+        command = SearchMetadataCommand(query, clients, limit)
+        results = self._explorer.exec(command)
+
+        return results or []
```

### Comparing `mumee-0.0.4/pyproject.toml` & `mumee-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Mumee"
-version = "0.0.4"
+version = "0.0.5"
 description = "MUsic MEtadata Explorer"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mumee"}]
 
 keywords = ["mumee", "metadata", "python", "song metadata", "spotify", "youtube", "youtube music", "music", "song"]
```

### Comparing `mumee-0.0.4/PKG-INFO` & `mumee-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mumee
-Version: 0.0.4
+Version: 0.0.5
 Summary: MUsic MEtadata Explorer
 Home-page: https://github.com/Billuc/Mumee
 License: MIT
 Keywords: mumee,metadata,python,song metadata,spotify,youtube,youtube music,music,song
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -59,49 +59,80 @@
 
 ## Usage
 
 There are 2 ways to use this library : using the `SongMetadataClient` object or via the DI.
 
 ### Using SongMetadataClient
 
-The library exposes the `SongMetadataClient` class. This class has 1 methods : `search`.
+The library exposes the `SongMetadataClient` class. This class has 2 methods : `fetch` and `search`.
 
-This method fetches the metadata corresponding to the request you give it, whether it is an URL or a query. It returns the result as a `SongMetadata` object or a `PlaylistMetadata` object.
+The `fetch` method fetches the metadata corresponding to the request you give it, whether it is an URL or a query. It returns the result as a `SongMetadata` object or a `PlaylistMetadata` object.
 
 **Example :**
 
 ```python
 from mumee import SongMetadataClient
 
 client = SongMetadataClient()
-result = client.search("in the end - linkin park")
+result = client.fetch("https://open.spotify.com/track/7AB0cUXnzuSlAnyHOqmrZr")
 
-title = result.title # In The End
+title = result.title # Faint
+artists = result.artists # ['Linkin Park']
+```
+
+The `search` method expects a query (e.g.: {title} - {artists}) and a limit corresponding to the number of results you want. It returns a list of `SongMetadata` objects that fit closest to the query that was given. This list is sorted by closest fit per client.
+
+**Example :**
+
+```python
+from mumee import SongMetadataClient
+
+client = SongMetadataClient()
+results = client.search("in the end - linkin park")
+
+title = results[0].title # In The End
+artists = results[0].artists # ['Linkin Park']
 ```
 
 ### Using DI
 
-The library also exposes a `BaseMetadataClient` interface and a `add_mumee` function for [Taipan-DI](https://github.com/Billuc/Taipan-DI).
+The library also exposes the `BaseMetadataClient` and `BaseMetadataExplorer` interfaces and a `add_mumee` function for [Taipan-DI](https://github.com/Billuc/Taipan-DI).
 
-In this function, the clients are registered as a Pipeline. All you need to do is to resolve the pipeline and execute it.
+In this function, the clients and explorers are registered as a Pipeline. All you need to do is to resolve the pipelines and execute it.
 
-**Example :**
+**Example 1 :**
 
 ```python
 from mumee import BaseMetadataClient, add_mumee
 from taipan_di import DependencyCollection
 
 services = DependencyCollection()
 add_mumee(services)
 
 provider = services.build()
 client = provider.resolve(BaseMetadataClient)
 
-result = client.exec("in the end - linkin park")
-title = result.title # In The End
+result = client.exec("https://open.spotify.com/track/7AB0cUXnzuSlAnyHOqmrZr")
+title = result.title # Faint
+```
+
+**Example 2 :**
+
+```python
+from mumee import BaseMetadataExplorer, add_mumee
+from taipan_di import DependencyCollection
+
+services = DependencyCollection()
+add_mumee(services)
+
+provider = services.build()
+explorer = provider.resolve(BaseMetadataExplorer)
+
+results = explorer.exec("in the end - linkin park")
+title = results[0].title # In The End
 ```
 
 ## Inspirations
 
 This library is partially based on spotDL's [spotify-downloader](https://github.com/spotDL/spotify-downloader).
 
 ## TODO
@@ -109,9 +140,10 @@
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
 - Support for Amazon Music
 - More metadata in the SongMetadata class
-- Allow return of multiple results
+- Handle edge case in explorer_handler
+- Re-sort explorer results
```

