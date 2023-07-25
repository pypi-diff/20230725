# Comparing `tmp/youtubeaio-1.1.4.tar.gz` & `tmp/youtubeaio-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubeaio-1.1.4.tar", max compression
+gzip compressed data, was "youtubeaio-1.1.5.tar", max compression
```

## Comparing `youtubeaio-1.1.4.tar` & `youtubeaio-1.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/LICENSE.md
--rw-r--r--   0        0        0     4864 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/README.md
--rw-r--r--   0        0        0     3873 2023-07-23 22:58:53.330885 youtubeaio-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       57 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/src/youtubeaio/__init__.py
--rw-r--r--   0        0        0      831 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/src/youtubeaio/const.py
--rw-r--r--   0        0        0     3149 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/src/youtubeaio/helper.py
--rw-r--r--   0        0        0     7429 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/models.py
--rw-r--r--   0        0        0     1772 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/oauth.py
--rw-r--r--   0        0        0        0 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/py.typed
--rw-r--r--   0        0        0     2139 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/types.py
--rw-r--r--   0        0        0     9711 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/youtube.py
--rw-r--r--   0        0        0     6115 1970-01-01 00:00:00.000000 youtubeaio-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-25 19:51:43.081213 youtubeaio-1.1.5/LICENSE.md
+-rw-r--r--   0        0        0     4864 2023-07-25 19:51:43.081213 youtubeaio-1.1.5/README.md
+-rw-r--r--   0        0        0     3892 2023-07-25 19:52:02.496849 youtubeaio-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-07-25 19:51:43.085211 youtubeaio-1.1.5/src/youtubeaio/__init__.py
+-rw-r--r--   0        0        0     1217 2023-07-25 19:51:43.085211 youtubeaio-1.1.5/src/youtubeaio/const.py
+-rw-r--r--   0        0        0     3721 2023-07-25 19:51:43.085211 youtubeaio-1.1.5/src/youtubeaio/helper.py
+-rw-r--r--   0        0        0     8597 2023-07-25 19:51:43.085211 youtubeaio-1.1.5/src/youtubeaio/models.py
+-rw-r--r--   0        0        0     1772 2023-07-25 19:51:43.085211 youtubeaio-1.1.5/src/youtubeaio/oauth.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:51:43.085211 youtubeaio-1.1.5/src/youtubeaio/py.typed
+-rw-r--r--   0        0        0     2139 2023-07-25 19:51:43.085211 youtubeaio-1.1.5/src/youtubeaio/types.py
+-rw-r--r--   0        0        0     9715 2023-07-25 19:51:43.085211 youtubeaio-1.1.5/src/youtubeaio/youtube.py
+-rw-r--r--   0        0        0     6115 1970-01-01 00:00:00.000000 youtubeaio-1.1.5/PKG-INFO
```

### Comparing `youtubeaio-1.1.4/LICENSE.md` & `youtubeaio-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.4/README.md` & `youtubeaio-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.4/pyproject.toml` & `youtubeaio-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "youtubeaio"
-version = "1.1.4"
+version = "1.1.5"
 description = "Asynchronous Python client for YouTube V3 API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-youtube"
 repository = "https://github.com/joostlek/python-youtube"
@@ -43,14 +43,15 @@
 pylint = "2.17.4"
 pytest = "7.4.0"
 pytest-asyncio = "0.21.1"
 pytest-cov = "4.1.0"
 ruff = "0.0.280"
 safety = "2.4.0b1"
 yamllint = "1.32.0"
+syrupy = "^4.0.8"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/joostlek/python-youtube/issues"
 Changelog = "https://github.com/joostlek/python-youtube/releases"
 
 [tool.coverage.report]
 show_missing = true
@@ -77,15 +78,15 @@
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_decorators = true
 disallow_untyped_defs = true
 no_implicit_optional = true
-no_implicit_reexport = true
+#no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
```

### Comparing `youtubeaio-1.1.4/src/youtubeaio/const.py` & `youtubeaio-1.1.5/src/youtubeaio/const.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,13 +22,34 @@
     SNIPPET = "snippet"
     STATISTICS = "statistics"
     STATUS = "status"
     SUGGESTIONS = "suggestions"
     TOPIC_DETAILS = "topicDetails"
 
 
+class VideoDimension(str, Enum):
+    """Enum holding the possible video dimensions."""
+
+    D3 = "3d"
+    D2 = "2d"
+
+
+class VideoDefinition(str, Enum):
+    """Enum holding the possible video definitions."""
+
+    HD = "hd"
+    SD = "sd"
+
+
+class VideoProjection(str, Enum):
+    """Enum holding the possible video projections."""
+
+    THREE_SIXTY = "360"
+    RECTANGULAR = "rectangular"
+
+
 class LiveBroadcastContent(str, Enum):
     """Enum holding the liveBroadcastContent values."""
 
     NONE = "none"
     LIVE = "live"
     UPCOMING = "upcoming"
```

### Comparing `youtubeaio-1.1.4/src/youtubeaio/helper.py` & `youtubeaio-1.1.5/src/youtubeaio/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Helper functions for the YouTube API."""
+import re
 import urllib.parse
 from collections.abc import AsyncGenerator, Generator
+from datetime import timedelta
 from enum import Enum
 from typing import Any, TypeVar
 
 from youtubeaio.types import AuthScope
 
 __all__ = [
     "YOUTUBE_AUTH_BASE_URL",
@@ -102,7 +104,27 @@
         raise ValueError(msg)
     count = 0
     async for item in generator:
         count += 1
         if count > total:
             break
         yield item
+
+
+def get_duration(duration: str) -> timedelta:
+    """Return timedelta for ISO8601 duration string."""
+    attributes = {
+        "S": 0,
+        "M": 0,
+        "H": 0,
+        "D": 0,
+    }
+    for match in re.compile(r"(\d+[DHMS])").finditer(duration):
+        part = match.group(1)
+        time_value = int(part[:-1])
+        attributes[part[len(part) - 1]] = time_value
+    return timedelta(
+        days=attributes["D"],
+        hours=attributes["H"],
+        minutes=attributes["M"],
+        seconds=attributes["S"],
+    )
```

### Comparing `youtubeaio-1.1.4/src/youtubeaio/models.py` & `youtubeaio-1.1.5/src/youtubeaio/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """Models for YouTube API."""
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import TypeVar
 
 from pydantic import BaseModel, Field
 
-from youtubeaio.const import LiveBroadcastContent
+from youtubeaio.const import (
+    LiveBroadcastContent,
+    VideoDefinition,
+    VideoDimension,
+    VideoProjection,
+)
 
 __all__ = [
     "YouTubeThumbnail",
     "YouTubeVideoThumbnails",
     "YouTubeVideoSnippet",
     "YouTubeVideo",
     "YouTubeChannelThumbnails",
     "YouTubeChannelRelatedPlaylists",
     "YouTubeChannelContentDetails",
     "YouTubeChannelSnippet",
     "YouTubeChannel",
 ]
 
+from youtubeaio.helper import get_duration
 from youtubeaio.types import PartMissingError
 
 T = TypeVar("T")
 
 
 class YouTubeThumbnail(BaseModel):
     """Model representing a video thumbnail."""
@@ -62,27 +68,59 @@
         ...,
         alias="liveBroadcastContent",
     )
     default_language: str | None = Field(None, alias="defaultLanguage")
     default_audio_language: str | None = Field(None, alias="defaultAudioLanguage")
 
 
+class YouTubeVideoContentDetails(BaseModel):
+    """Model representing video content details."""
+
+    raw_duration: str = Field(..., alias="duration")
+    dimension: VideoDimension = Field(...)
+    definition: VideoDefinition = Field(...)
+    raw_caption: str = Field(..., alias="caption")
+    licensed_content: bool = Field(..., alias="licensedContent")
+    projection: VideoProjection = Field(...)
+
+    @property
+    def caption(self) -> bool:
+        """Return if video has caption."""
+        return self.raw_caption == "true"
+
+    @property
+    def duration(self) -> timedelta:
+        """Return length of the video."""
+        return get_duration(self.raw_duration)
+
+
 class YouTubeVideo(BaseModel):
     """Model representing a video."""
 
     video_id: str = Field(..., alias="id")
     nullable_snippet: YouTubeVideoSnippet | None = Field(None, alias="snippet")
+    nullable_content_details: YouTubeVideoContentDetails | None = Field(
+        None,
+        alias="contentDetails",
+    )
 
     @property
     def snippet(self) -> YouTubeVideoSnippet:
         """Return snippet."""
         if self.nullable_snippet is None:
             raise PartMissingError
         return self.nullable_snippet
 
+    @property
+    def content_details(self) -> YouTubeVideoContentDetails:
+        """Return content details."""
+        if self.nullable_content_details is None:
+            raise PartMissingError
+        return self.nullable_content_details
+
 
 class YouTubeChannelThumbnails(BaseModel):
     """Model representing channel thumbnails."""
 
     default: YouTubeThumbnail = Field(...)
     medium: YouTubeThumbnail | None = Field(None)
     high: YouTubeThumbnail | None = Field(None)
```

### Comparing `youtubeaio-1.1.4/src/youtubeaio/oauth.py` & `youtubeaio-1.1.5/src/youtubeaio/oauth.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.4/src/youtubeaio/types.py` & `youtubeaio-1.1.5/src/youtubeaio/types.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.4/src/youtubeaio/youtube.py` & `youtubeaio-1.1.5/src/youtubeaio/youtube.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                 data = await response.json()
                 for entry in data.get("items", []):
                     yield return_type(**entry)  # type: ignore[operator]
                 _after = data.get("nextPageToken")
                 _first = False
         except asyncio.TimeoutError as exc:
             msg = "Timeout occurred"
-            raise YouTubeAPIError(msg) from exc
+            raise YouTubeBackendError(msg) from exc
 
     async def set_user_authentication(
         self,
         token: str,
         scopes: list[AuthScope],
         refresh_token: str | None = None,
     ) -> None:
```

### Comparing `youtubeaio-1.1.4/PKG-INFO` & `youtubeaio-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtubeaio
-Version: 1.1.4
+Version: 1.1.5
 Summary: Asynchronous Python client for YouTube V3 API.
 Home-page: https://github.com/joostlek/python-youtube
 License: MIT
 Keywords: youtube,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
```

