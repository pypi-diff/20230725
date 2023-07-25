# Comparing `tmp/tiktokapipy-0.2.1.tar.gz` & `tmp/tiktokapipy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktokapipy-0.2.1.tar", last modified: Mon Jul 17 20:27:13 2023, max compression
+gzip compressed data, was "tiktokapipy-0.2.2.tar", last modified: Tue Jul 25 17:25:21 2023, max compression
```

## Comparing `tiktokapipy-0.2.1.tar` & `tiktokapipy-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.210665 tiktokapipy-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.214665 tiktokapipy-0.2.1/src/tiktokapipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/async_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.214665 tiktokapipy-0.2.1/src/tiktokapipy/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/models/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/src/tiktokapipy/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/util/deferred_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/util/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/src/tiktokapipy/util/signing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.214665 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 20:27:13.000000 tiktokapipy-0.2.1/src/tiktokapipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:27:13.218665 tiktokapipy-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_slideshow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 20:27:00.000000 tiktokapipy-0.2.1/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.379190 tiktokapipy-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-25 17:25:21.379190 tiktokapipy-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:25:21.379190 tiktokapipy-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.371191 tiktokapipy-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.371191 tiktokapipy-0.2.2/src/tiktokapipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/async_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.375191 tiktokapipy-0.2.2/src/tiktokapipy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.375191 tiktokapipy-0.2.2/src/tiktokapipy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/util/deferred_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/util/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/util/signing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.375191 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.379190 tiktokapipy-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_slideshow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_video.py
```

### Comparing `tiktokapipy-0.2.1/LICENSE` & `tiktokapipy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/PKG-INFO` & `tiktokapipy-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.1 Summary: Asyncio TikTok
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.2 Summary: Asyncio TikTok
 data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
```

### Comparing `tiktokapipy-0.2.1/README.md` & `tiktokapipy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/pyproject.toml` & `tiktokapipy-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tiktokapipy"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name="Russell Newton", email="russell.newton01@gmail.com" },
 ]
 description = "Asyncio TikTok data scraping tool"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/__init__.py` & `tiktokapipy-0.2.2/src/tiktokapipy/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/api.py` & `tiktokapipy-0.2.2/src/tiktokapipy/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ChallengePage,
     PrimaryResponseType,
     SentToLoginResponse,
     UserResponse,
     VideoPage,
 )
 from tiktokapipy.models.user import User, user_link
-from tiktokapipy.models.video import Video
+from tiktokapipy.models.video import Video, is_mobile_share_link
 from tiktokapipy.util.queries import get_challenge_detail_sync, get_video_detail_sync
 
 _DataModelT = TypeVar("_DataModelT", bound=PrimaryResponseType, covariant=True)
 """
 Generic used for data scraping.
 """
 
@@ -157,14 +157,42 @@
         set to ``True`` at API initialization or this method will raise a :exc:`TikTokAPIError`.
 
         :param link_or_id: The link to the video or its unique ID.
         :return: A :class:`.Video` object containing the scraped data
         :rtype: :class:`.Video`
         """
         if isinstance(link_or_id, str):
+            if is_mobile_share_link(link_or_id):
+                self.context.clear_cookies()
+                page: Page = self.context.new_page()
+                page.add_init_script(
+                    """
+    if (navigator.webdriver === false) {
+        // Post Chrome 89.0.4339.0 and already good
+    } else if (navigator.webdriver === undefined) {
+        // Pre Chrome 89.0.4339.0 and already good
+    } else {
+        // Pre Chrome 88.0.4291.0 and needs patching
+        delete Object.getPrototypeOf(navigator).webdriver
+    }
+                """
+                )
+
+                def ignore_scripts(route: Route):
+                    if route.request.resource_type == "script":
+                        return route.abort()
+                    return route.continue_()
+
+                page.route("**/*", ignore_scripts)
+                page.goto(link_or_id, wait_until=None)
+                page.wait_for_selector("#SIGI_STATE", state="attached")
+
+                link_or_id = page.url
+
+                page.close()
             video_id = link_or_id.split("/")[-1].split("?")[0]
         else:
             video_id = link_or_id
 
         response = VideoPage.model_validate(
             get_video_detail_sync(video_id, self.context)
         )
```

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/async_api.py` & `tiktokapipy-0.2.2/src/tiktokapipy/async_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ChallengePage,
     PrimaryResponseType,
     SentToLoginResponse,
     UserResponse,
     VideoPage,
 )
 from tiktokapipy.models.user import User, user_link
-from tiktokapipy.models.video import Video
+from tiktokapipy.models.video import Video, is_mobile_share_link
 from tiktokapipy.util.queries import get_challenge_detail_async, get_video_detail_async
 
 _DataModelT = TypeVar("_DataModelT", bound=PrimaryResponseType, covariant=True)
 """
 Generic used for data scraping.
 """
 
@@ -152,14 +152,42 @@
         return user
 
     async def video(
         self,
         link_or_id: Union[int, str],
     ) -> Video:
         if isinstance(link_or_id, str):
+            if is_mobile_share_link(link_or_id):
+                await self.context.clear_cookies()
+                page: Page = await self.context.new_page()
+                await page.add_init_script(
+                    """
+    if (navigator.webdriver === false) {
+        // Post Chrome 89.0.4339.0 and already good
+    } else if (navigator.webdriver === undefined) {
+        // Pre Chrome 89.0.4339.0 and already good
+    } else {
+        // Pre Chrome 88.0.4291.0 and needs patching
+        delete Object.getPrototypeOf(navigator).webdriver
+    }
+                """
+                )
+
+                async def ignore_scripts(route: Route):
+                    if route.request.resource_type == "script":
+                        return await route.abort()
+                    return await route.continue_()
+
+                await page.route("**/*", ignore_scripts)
+                await page.goto(link_or_id, wait_until=None)
+                await page.wait_for_selector("#SIGI_STATE", state="attached")
+
+                link_or_id = page.url
+
+                await page.close()
             video_id = link_or_id.split("/")[-1].split("?")[0]
         else:
             video_id = link_or_id
 
         response = VideoPage.model_validate(
             await get_video_detail_async(video_id, self.context)
         )
```

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/models/__init__.py` & `tiktokapipy-0.2.2/src/tiktokapipy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/models/challenge.py` & `tiktokapipy-0.2.2/src/tiktokapipy/models/challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/models/comment.py` & `tiktokapipy-0.2.2/src/tiktokapipy/models/comment.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/models/raw_data.py` & `tiktokapipy-0.2.2/src/tiktokapipy/models/raw_data.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/models/user.py` & `tiktokapipy-0.2.2/src/tiktokapipy/models/user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/models/video.py` & `tiktokapipy-0.2.2/src/tiktokapipy/models/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,7 +270,13 @@
 
 Video.model_rebuild()
 
 
 def video_link(video_id: int) -> str:
     """Get a working link to a TikTok video from the video's unique id."""
     return f"https://m.tiktok.com/v/{video_id}"
+
+
+def is_mobile_share_link(link: str) -> bool:
+    import re
+
+    return re.match(r"https://vm\.tiktok\.com/[0-9A-Za-z]*", link) is not None
```

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/util/deferred_collectors.py` & `tiktokapipy-0.2.2/src/tiktokapipy/util/deferred_collectors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import abc
 import time
 import warnings
+from datetime import datetime
+from json import JSONDecodeError
 from typing import AsyncIterator, ForwardRef, Iterator, List, Literal, TypeVar, Union
 
 from playwright.async_api import BrowserContext as AsyncBrowserContext
 from playwright.sync_api import BrowserContext as SyncBrowserContext
 from tiktokapipy import TikTokAPIError, TikTokAPIWarning
 from tiktokapipy.util.queries import (
     get_challenge_detail_async,
@@ -171,28 +173,42 @@
         if self.from_type == "post":
             self._cursor = int(time.time()) * 1000
 
     def _fetch_sync(self):
         from tiktokapipy.models.raw_data import APIResponse
 
         # noinspection PyTypeChecker
-        raw = make_request_sync(
-            f"{self.from_type}/item_list/",
-            self._cursor,
-            self._target_id,
-            self._api.context,
-            **self._extra_params,
-        )
+        try:
+            raw = make_request_sync(
+                f"{self.from_type}/item_list/",
+                self._cursor,
+                self._target_id,
+                self._api.context,
+                **self._extra_params,
+            )
+        except JSONDecodeError:
+            readable_cursor = (
+                f"video #{self._cursor}"
+                if self.from_type == "challenge"
+                else datetime.fromtimestamp(self._cursor // 1000).strftime("%c")
+            )
+            warnings.warn(
+                f"Unable to grab videos beyond {readable_cursor} (JSONDecodeError), stopping iteration early."
+                f"Try again if you think this is a mistake.",
+                category=TikTokAPIWarning,
+                stacklevel=2,
+            )
+            self._has_more = False
+            raise StopIteration
         converted = APIResponse.model_validate(raw)
-        for item in converted.item_list:
-            item._api = self._api
+        if not converted.item_list:
+            self._has_more = False
+            raise StopIteration
         self._has_more = converted.has_more
         self._cursor = converted.cursor
-        if not converted.item_list:
-            return
 
         for video in converted.item_list:
             try:
                 self._collected_values.append(self._api.video(video.id))
             except TikTokAPIError:
                 warnings.warn(
                     f"Unable to grab video with id {video.id}",
@@ -200,28 +216,42 @@
                     stacklevel=2,
                 )
 
     async def _fetch_async(self):
         from tiktokapipy.models.raw_data import APIResponse
 
         # noinspection PyTypeChecker
-        raw = await make_request_async(
-            f"{self.from_type}/item_list/",
-            self._cursor,
-            self._target_id,
-            self._api.context,
-            **self._extra_params,
-        )
+        try:
+            raw = await make_request_async(
+                f"{self.from_type}/item_list/",
+                self._cursor,
+                self._target_id,
+                self._api.context,
+                **self._extra_params,
+            )
+        except JSONDecodeError:
+            readable_cursor = (
+                f"video #{self._cursor}"
+                if self.from_type == "challenge"
+                else datetime.fromtimestamp(self._cursor).strftime("%c")
+            )
+            warnings.warn(
+                f"Unable to grab videos beyond {readable_cursor}, stopping iteration early."
+                f"Try again if you think this is a mistake.",
+                category=TikTokAPIWarning,
+                stacklevel=2,
+            )
+            self._has_more = False
+            raise StopAsyncIteration
         converted = APIResponse.model_validate(raw)
-        for item in converted.item_list:
-            item._api = self._api
+        if not converted.item_list:
+            self._has_more = False
+            raise StopAsyncIteration
         self._has_more = converted.has_more
         self._cursor = converted.cursor
-        if not converted.item_list:
-            return
         for video in converted.item_list:
             try:
                 self._collected_values.append(await self._api.video(video.id))
             except TikTokAPIError:
                 warnings.warn(
                     f"Unable to grab video with id {video.id}",
                     category=TikTokAPIWarning,
```

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/util/queries.py` & `tiktokapipy-0.2.2/src/tiktokapipy/util/queries.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy/util/signing.py` & `tiktokapipy-0.2.2/src/tiktokapipy/util/signing.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy.egg-info/PKG-INFO` & `tiktokapipy-0.2.2/src/tiktokapipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.1 Summary: Asyncio TikTok
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.2 Summary: Asyncio TikTok
 data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
```

### Comparing `tiktokapipy-0.2.1/src/tiktokapipy.egg-info/SOURCES.txt` & `tiktokapipy-0.2.2/src/tiktokapipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/tests/test_challenge.py` & `tiktokapipy-0.2.2/tests/test_challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/tests/test_slideshow.py` & `tiktokapipy-0.2.2/tests/test_slideshow.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/tests/test_user.py` & `tiktokapipy-0.2.2/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.1/tests/test_video.py` & `tiktokapipy-0.2.2/tests/test_video.py`

 * *Files identical despite different names*

