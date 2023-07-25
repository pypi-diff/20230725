# Comparing `tmp/wf_video_io-3.4.2.tar.gz` & `tmp/wf_video_io-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.4.2.tar", max compression
+gzip compressed data, was "wf_video_io-3.4.3.tar", max compression
```

## Comparing `wf_video_io-3.4.2.tar` & `wf_video_io-3.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.4.2/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.4.2/README.md
--rw-r--r--   0        0        0     1181 2023-07-17 21:27:08.226766 wf_video_io-3.4.2/pyproject.toml
--rwxr-xr-x   0        0        0       50 2023-07-17 21:27:13.213170 wf_video_io-3.4.2/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.4.2/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    18738 2023-06-29 21:12:27.242562 wf_video_io-3.4.2/video_io/client/core.py
--rw-r--r--   0        0        0      265 2023-06-29 21:08:51.793888 wf_video_io-3.4.2/video_io/client/errors.py
--rw-r--r--   0        0        0     3412 2023-06-29 21:08:51.794977 wf_video_io-3.4.2/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.4.2/video_io/config.py
--rwxr-xr-x   0        0        0    49247 2023-06-29 21:14:15.999435 wf_video_io-3.4.2/video_io/core.py
--rw-r--r--   0        0        0       41 2023-06-29 21:08:51.797796 wf_video_io-3.4.2/video_io/errors.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.4.2/video_io/log_retry.py
--rw-r--r--   0        0        0    11180 2023-07-17 21:26:49.064078 wf_video_io-3.4.2/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.4.2/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.4.2/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.4.3/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.4.3/README.md
+-rw-r--r--   0        0        0     1181 2023-07-25 21:30:29.940748 wf_video_io-3.4.3/pyproject.toml
+-rwxr-xr-x   0        0        0       50 2023-07-25 21:30:29.944820 wf_video_io-3.4.3/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.4.3/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    18738 2023-06-29 21:12:27.242562 wf_video_io-3.4.3/video_io/client/core.py
+-rw-r--r--   0        0        0      265 2023-06-29 21:08:51.793888 wf_video_io-3.4.3/video_io/client/errors.py
+-rw-r--r--   0        0        0     3412 2023-06-29 21:08:51.794977 wf_video_io-3.4.3/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.4.3/video_io/config.py
+-rwxr-xr-x   0        0        0    49400 2023-07-25 21:30:14.271638 wf_video_io-3.4.3/video_io/core.py
+-rw-r--r--   0        0        0       41 2023-06-29 21:08:51.797796 wf_video_io-3.4.3/video_io/errors.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.4.3/video_io/log_retry.py
+-rw-r--r--   0        0        0    11180 2023-07-17 21:26:49.064078 wf_video_io-3.4.3/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.4.3/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.4.3/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.4.3/PKG-INFO
```

### Comparing `wf_video_io-3.4.2/LICENSE` & `wf_video_io-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.2/pyproject.toml` & `wf_video_io-3.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "wf-video-io"
 #dynamic = ["version"]
-version = "3.4.2"
+version = "3.4.3"
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.4.2"
+version = "3.4.3"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.4.2/video_io/client/core.py` & `wf_video_io-3.4.3/video_io/client/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.2/video_io/client/utils.py` & `wf_video_io-3.4.3/video_io/client/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.2/video_io/config.py` & `wf_video_io-3.4.3/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.2/video_io/core.py` & `wf_video_io-3.4.3/video_io/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
         end_utc = video_timestamp_max_utc + video_io.config.VIDEO_DURATION
     else:
         video_timestamps_utc = None
         start_utc = start.astimezone(datetime.timezone.utc)
         end_utc = end.astimezone(datetime.timezone.utc)
         video_timestamp_min_utc = video_timestamp_min(start_utc)
         video_timestamp_max_utc = video_timestamp_max(end_utc)
-    if environment_name is not None:
+    if environment_id is None and environment_name is not None:
         environment_id = honeycomb_io.fetch_environment_id(
             environment_name=environment_name,
             client=client,
             uri=uri,
             token_uri=token_uri,
             audience=audience,
             client_id=client_id,
@@ -923,32 +923,34 @@
         ).astimezone(original_tzinfo)
     else:
         timestamp_max = timestamp_max_naive
     return timestamp_max
 
 
 def fetch_concatenated_video(
-    environment_name: str,
+    environment_id: str,
     start: datetime,
     end: datetime,
     output_directory: str,
+    environment_name: str = None,
     camera_names: Optional[List[str]] = None,
     workers: int = cpu_count() - 1,
     video_snippet_directory: str = None,
     overwrite_video_snippets: bool = False,
     overwrite_concatenated_video: bool = False,
     video_client: video_io.client.VideoStorageClient = None,
 ) -> Optional[pd.DataFrame]:
     """
     Create concatenated video files for each camera in a particular environment given a provided start and end time.
 
     Function will download individual video snippets across each camera, concatenate those snippets, and trim the videos
     to exactly match the provided start and end time.
 
     Args:
+        environment_id (str): Honeycomb environment ID
         environment_name (str): Honeycomb environment name
         start (datetime): Start of time period
         end (datetime): End of time period
         output_directory (str): Directory to write concatenated video files to. Video file names are written as "{environment_id}_{camera_device_id}_{start.strftime('%m%d%YT%H%M%S%f%z')}_{end.strftime('%m%d%YT%H%M%S%f%z')}.mp4"
         camera_names (List[str]): Filter cameras to a specific subset (default value is None which means to filter and concatenated video will be generated for all cameras)
         workers (int): Number of processes to be used to download video files
         video_snippet_directory (str): Directory to store video snippets. If no directory is provided, videos will be downloaded to the operating systems temp directory and destroyed once the function finishes
@@ -961,14 +963,15 @@
 
     """
     os.makedirs(output_directory, exist_ok=True)
 
     video_metadata = fetch_video_metadata(
         start=start,
         end=end,
+        environment_id=environment_id,
         environment_name=environment_name,
         camera_names=camera_names,
         video_client=video_client,
     )
     if video_metadata is None or len(video_metadata) == 0:
         logger.warning(
             f"Found 0 videos for {environment_name} between {start} and {end}"
```

### Comparing `wf_video_io-3.4.2/video_io/utils.py` & `wf_video_io-3.4.3/video_io/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.2/video_io/video_reader.py` & `wf_video_io-3.4.3/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.4.2/setup.py` & `wf_video_io-3.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.4.2',
+    'version': '3.4.3',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.4.2/PKG-INFO` & `wf_video_io-3.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.4.2
+Version: 3.4.3
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```

