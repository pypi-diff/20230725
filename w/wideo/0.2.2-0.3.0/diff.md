# Comparing `tmp/wideo-0.2.2.tar.gz` & `tmp/wideo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wideo-0.2.2.tar", max compression
+gzip compressed data, was "wideo-0.3.0.tar", max compression
```

## Comparing `wideo-0.2.2.tar` & `wideo-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      674 2023-07-18 16:33:24.723037 wideo-0.2.2/README.md
--rw-r--r--   0        0        0      469 2023-07-18 16:33:24.731038 wideo-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1584 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/__init__.py
--rw-r--r--   0        0        0      767 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/admin_urls.py
--rw-r--r--   0        0        0      174 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/apps.py
--rw-r--r--   0        0        0      376 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/blocks.py
--rw-r--r--   0        0        0     2494 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/codecs.py
--rw-r--r--   0        0        0       92 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/exceptions.py
--rw-r--r--   0        0        0     7167 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/ffmpeg.py
--rw-r--r--   0        0        0      329 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/fields.py
--rw-r--r--   0        0        0      334 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/forms.py
--rw-r--r--   0        0        0        0 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/management/commands/__init__.py
--rw-r--r--   0        0        0      321 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/management/commands/delete_orphan_uploaded_videos.py
--rw-r--r--   0        0        0      557 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/management/commands/encode_videos.py
--rw-r--r--   0        0        0     9737 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/migrations/0001_initial.py
--rw-r--r--   0        0        0      676 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/migrations/0002_lock.py
--rw-r--r--   0        0        0     2955 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/migrations/0003_uploadedvideochunk.py
--rw-r--r--   0        0        0        0 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/migrations/__init__.py
--rw-r--r--   0        0        0     6373 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/models.py
--rw-r--r--   0        0        0      777 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/permissions.py
--rw-r--r--   0        0        0     1544 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/signals.py
--rw-r--r--   0        0        0     1301 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/storage.py
--rw-r--r--   0        0        0      655 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/tasks.py
--rw-r--r--   0        0        0      179 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/blocks/video.html
--rw-r--r--   0        0        0     4210 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/forms/file.html
--rw-r--r--   0        0        0      190 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/forms/file_edit.html
--rw-r--r--   0        0        0      179 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/icons/video.svg
--rw-r--r--   0        0        0      457 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/preview/plyr_styles.html
--rw-r--r--   0        0        0     1757 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/preview/video_source.html
--rw-r--r--   0        0        0      124 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/video.html
--rw-r--r--   0        0        0     3303 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/videos/add.html
--rw-r--r--   0        0        0     1621 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/videos/confirm_delete.html
--rw-r--r--   0        0        0     2690 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/videos/edit.html
--rw-r--r--   0        0        0     4455 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/videos/index.html
--rw-r--r--   0        0        0     2586 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/videos/results.html
--rw-r--r--   0        0        0        0 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templates/wideo/videos/results_video.html
--rw-r--r--   0        0        0        0 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templatetags/__init__.py
--rw-r--r--   0        0        0      231 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/templatetags/settings.py
--rw-r--r--   0        0        0    14570 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/views.py
--rw-r--r--   0        0        0      612 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/wagtail_hooks.py
--rw-r--r--   0        0        0      126 2023-07-18 16:33:24.731038 wideo-0.2.2/src/wideo/widgets.py
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 wideo-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      674 2023-07-25 10:26:57.854470 wideo-0.3.0/README.md
+-rw-r--r--   0        0        0      469 2023-07-25 10:26:57.858470 wideo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1584 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/__init__.py
+-rw-r--r--   0        0        0      767 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/admin_urls.py
+-rw-r--r--   0        0        0      174 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/apps.py
+-rw-r--r--   0        0        0      376 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/blocks.py
+-rw-r--r--   0        0        0     2494 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/codecs.py
+-rw-r--r--   0        0        0       92 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/exceptions.py
+-rw-r--r--   0        0        0     7726 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/ffmpeg.py
+-rw-r--r--   0        0        0      329 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/fields.py
+-rw-r--r--   0        0        0      334 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/forms.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/management/commands/__init__.py
+-rw-r--r--   0        0        0      321 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/management/commands/delete_orphan_uploaded_videos.py
+-rw-r--r--   0        0        0      557 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/management/commands/encode_videos.py
+-rw-r--r--   0        0        0     9737 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/migrations/0001_initial.py
+-rw-r--r--   0        0        0      676 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/migrations/0002_lock.py
+-rw-r--r--   0        0        0     2955 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/migrations/0003_uploadedvideochunk.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/migrations/__init__.py
+-rw-r--r--   0        0        0     6373 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/models.py
+-rw-r--r--   0        0        0      777 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/permissions.py
+-rw-r--r--   0        0        0     1544 2023-07-25 10:26:57.858470 wideo-0.3.0/src/wideo/signals.py
+-rw-r--r--   0        0        0     1301 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/storage.py
+-rw-r--r--   0        0        0      655 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/tasks.py
+-rw-r--r--   0        0        0      179 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/blocks/video.html
+-rw-r--r--   0        0        0     4210 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/forms/file.html
+-rw-r--r--   0        0        0      190 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/forms/file_edit.html
+-rw-r--r--   0        0        0      179 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/icons/video.svg
+-rw-r--r--   0        0        0      457 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/preview/plyr_styles.html
+-rw-r--r--   0        0        0     1757 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/preview/video_source.html
+-rw-r--r--   0        0        0      124 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/video.html
+-rw-r--r--   0        0        0     3303 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/videos/add.html
+-rw-r--r--   0        0        0     1621 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/videos/confirm_delete.html
+-rw-r--r--   0        0        0     2690 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/videos/edit.html
+-rw-r--r--   0        0        0     4455 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/videos/index.html
+-rw-r--r--   0        0        0     2586 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/videos/results.html
+-rw-r--r--   0        0        0        0 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templates/wideo/videos/results_video.html
+-rw-r--r--   0        0        0        0 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templatetags/__init__.py
+-rw-r--r--   0        0        0      231 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/templatetags/settings.py
+-rw-r--r--   0        0        0    14570 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/views.py
+-rw-r--r--   0        0        0      612 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/wagtail_hooks.py
+-rw-r--r--   0        0        0      126 2023-07-25 10:26:57.862470 wideo-0.3.0/src/wideo/widgets.py
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 wideo-0.3.0/PKG-INFO
```

### Comparing `wideo-0.2.2/README.md` & `wideo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/__init__.py` & `wideo-0.3.0/src/wideo/__init__.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/admin_urls.py` & `wideo-0.3.0/src/wideo/admin_urls.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/codecs.py` & `wideo-0.3.0/src/wideo/codecs.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/ffmpeg.py` & `wideo-0.3.0/src/wideo/ffmpeg.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import join
 from shutil import rmtree
 from subprocess import run
 from typing import BinaryIO, Optional
 
 import magic
 from django.conf import settings
-from django.core.files.base import ContentFile
+from django.core.files.base import File
 from django.core.files.uploadedfile import InMemoryUploadedFile, TemporaryUploadedFile
 from django.db.transaction import atomic
 
 from . import get_render_model, get_video_model
 from .codecs import get_presets
 from .exceptions import ConfigurationError, InvalidVideoFile
 from .models import AbstractRender, AbstractVideo, RemoteVideoFile, lock
@@ -139,14 +139,25 @@
     encoding went down as intended, or `False` if something went wrong.
     """
 
     presets_map = get_presets()
     renders = {}
     ffmpegs = []
 
+    def abort_everything():
+        """
+        If something goes wrong during processing (invalid file...), stop everything and
+        ensure we don't keep any unused Render objects.
+        """
+        for f in ffmpegs:
+            f.kill()
+
+        for r in renders.values():
+            r.delete()
+
     def get_render_temp_file(r: AbstractRender) -> str:
         """
         Creates a simple unique path to a temporary file, used for storing outputs of
         ffmpeg.
         """
         return join(working_dir, str(r.id))
 
@@ -171,46 +182,45 @@
             height=0,
             frames_per_second=0,
             frame_count=0,
         )
         renders[preset_label] = render
         flags = preset["ffmpeg_flags"]
         command = f"ffmpeg -y -i {input_file_path} -f {preset['extension']} {' '.join(flags)} {get_render_temp_file(render)}"
-        ffmpegs.append(subprocess.Popen(command, shell=True))
-
-    def abort_everything():
-        """
-        If something goes wrong during processing (invalid file...), stop everything and
-        ensure we don't keep any unused Render objects.
-        """
-        for f in ffmpegs:
-            f.kill()
+        ffmpeg = subprocess.Popen(command, shell=True)
 
-        for r in renders.values():
-            r.delete()
+        # If parallel work is disabled, wait for each ffmpeg process synchronously to
+        # avoid having more than one running at once, and panic if any of them fails.
+        # If parallel work is enabled, store the processes to check for their result
+        # later on.
+        if getattr(settings, "WIDEO_PARALLEL_WORK", False):
+            ffmpegs.append(ffmpeg)
+        elif ffmpeg.wait():
+            abort_everything()
+            return False
 
-    # Wait for all ffmpeg processes to successfully finish their job (otherwise, panic
-    # and abort everything immediately)
+    # When parallel work is enabled, `ffmpegs` will contain a list with all ffmpeg
+    # process that we should wait for. As for when parallel work is disabled, if any of
+    # them has failed, panic and abort everything.
     for ffmpeg in ffmpegs:
         if ffmpeg.wait():
             abort_everything()
             return False
 
     # After all videos have been correctly generated, we just need to write them into
     # their respective Render objects
     for preset_label, preset in presets_map.items():
         render = renders[preset_label]
 
         with open(get_render_temp_file(render), "rb") as file:
             name = f"{render.video.title}_{preset_label}.{preset['extension']}"
-            render.file = ContentFile(b"", name=name)
-
-            with render.file.open("wb") as target:
-                while buf := file.read(1024**2):
-                    target.write(buf)
+            uploaded_file = File(file)
+            # Saving the file this way is necessary; `render.file = File(file, name)`
+            # does not work
+            render.file.save(name, uploaded_file, save=True)
 
             # Don't forget to get info from the generated videos, and to store it in the
             # previously created Render objects
             video_info = get_video_info(file)
 
         for field in RemoteVideoFile.INFORMATION_FIELDS:
             setattr(render, field, video_info[field])
```

### Comparing `wideo-0.2.2/src/wideo/management/commands/encode_videos.py` & `wideo-0.3.0/src/wideo/management/commands/encode_videos.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/migrations/0001_initial.py` & `wideo-0.3.0/src/wideo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/migrations/0002_lock.py` & `wideo-0.3.0/src/wideo/migrations/0002_lock.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/migrations/0003_uploadedvideochunk.py` & `wideo-0.3.0/src/wideo/migrations/0003_uploadedvideochunk.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/models.py` & `wideo-0.3.0/src/wideo/models.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/permissions.py` & `wideo-0.3.0/src/wideo/permissions.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/signals.py` & `wideo-0.3.0/src/wideo/signals.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/storage.py` & `wideo-0.3.0/src/wideo/storage.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/tasks.py` & `wideo-0.3.0/src/wideo/tasks.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/templates/wideo/forms/file.html` & `wideo-0.3.0/src/wideo/templates/wideo/forms/file.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/templates/wideo/preview/video_source.html` & `wideo-0.3.0/src/wideo/templates/wideo/preview/video_source.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/templates/wideo/videos/add.html` & `wideo-0.3.0/src/wideo/templates/wideo/videos/add.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/templates/wideo/videos/confirm_delete.html` & `wideo-0.3.0/src/wideo/templates/wideo/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/templates/wideo/videos/edit.html` & `wideo-0.3.0/src/wideo/templates/wideo/videos/edit.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/templates/wideo/videos/index.html` & `wideo-0.3.0/src/wideo/templates/wideo/videos/index.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/templates/wideo/videos/results.html` & `wideo-0.3.0/src/wideo/templates/wideo/videos/results.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/views.py` & `wideo-0.3.0/src/wideo/views.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/src/wideo/wagtail_hooks.py` & `wideo-0.3.0/src/wideo/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.2/PKG-INFO` & `wideo-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wideo
-Version: 0.2.2
+Version: 0.3.0
 Summary: Add video goodness to your Wagtail website
 License: WTFPL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

