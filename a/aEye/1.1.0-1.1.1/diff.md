# Comparing `tmp/aEye-1.1.0.tar.gz` & `tmp/aEye-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aEye-1.1.0.tar", last modified: Thu Jul 20 16:17:52 2023, max compression
+gzip compressed data, was "aEye-1.1.1.tar", last modified: Tue Jul 25 20:07:47 2023, max compression
```

## Comparing `aEye-1.1.0.tar` & `aEye-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:52.090942 aEye-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 16:17:38.000000 aEye-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-20 16:17:52.090942 aEye-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-20 16:17:38.000000 aEye-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:52.090942 aEye-1.1.0/aEye/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-20 16:17:38.000000 aEye-1.1.0/aEye/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:52.090942 aEye-1.1.0/aEye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 16:17:52.000000 aEye-1.1.0/aEye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:17:52.090942 aEye-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 16:17:38.000000 aEye-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:52.090942 aEye-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-20 16:17:38.000000 aEye-1.1.0/tests/test_extract_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:47.497064 aEye-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 20:07:33.000000 aEye-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-07-25 20:07:47.497064 aEye-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-25 20:07:33.000000 aEye-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:47.497064 aEye-1.1.1/aEye/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:47.497064 aEye-1.1.1/aEye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:07:47.497064 aEye-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 20:07:33.000000 aEye-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:47.497064 aEye-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-25 20:07:33.000000 aEye-1.1.1/tests/test_extract_metadata.py
```

### Comparing `aEye-1.1.0/LICENSE` & `aEye-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aEye-1.1.0/PKG-INFO` & `aEye-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -128,21 +128,21 @@
 The framework allows frames to be extracted at any point while processing, but if there are pending processor modifications, a warning will be raised, and the resulting images will come from the original source. 
 The execution order affects frame capture.
 
 Example:
 
 
 ```console
-to_process = process.add_label_change_resolution(video_list_s3, "720p")
-process.cv_extract_specific_frame(to_process, 42)  # These screenshots will NOT be in 720p
-aux.execute_label_and_write_local(to_process)
+label.change_resolution(video_list_s3, "720p")
+extract.specific_frame_extractor(aux, video_list_s3, 42)  # These screenshots will NOT be in 720p
+aux.execute_label_and_write_local(video_list_s3)
 
 # Because the video modifications have not been executed, the images will come from the original video.
 
-to_process = process.add_label_change_resolution(video_list_s3, "720p")
+label.change_resolution(video_list_s3, "720p")
 output_list = aux.execute_label_and_write_local(to_process)
 process.cv_extract_specific_frame(output_list, 42)  # These screenshots WILL be in 720p!
 
 # Because the rescale was executed, the resulting screenshot is in 720p!
 ```
 
 All Label Utility:
@@ -172,19 +172,19 @@
 bitrate in comparison to the original will result in a loss of some i/b frames, but the output duration will remain the same. 
 
 grayscale(video_list) -> Applies a grayscale filter to all videos in video_list.
 ```
 
 All Extract Utility:
 ```console
-frame_at_time_extractor(video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
+frame_at_time_extractor(aux, video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
 
-specific_frame_extractor(video_list, frame) -> Extract the exact frame you pass as a PNG
+specific_frame_extractor(aux, video_list, frame) -> Extract the exact frame you pass as a PNG
 
-multiple_frame_extractor(video_list, start_frame, num_frames) -> Beginning at start_frame, extract the next num_frames
+multiple_frame_extractor(aux, video_list, start_frame, num_frames) -> Beginning at start_frame, extract the next num_frames
 ```
 
 Limitations:
 
 Please note the following limitations of the framework:
 
 Frames cannot be extracted from a source that has been previously executed in the processor pipeline.
```

### Comparing `aEye-1.1.0/README.md` & `aEye-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,21 +118,21 @@
 The framework allows frames to be extracted at any point while processing, but if there are pending processor modifications, a warning will be raised, and the resulting images will come from the original source. 
 The execution order affects frame capture.
 
 Example:
 
 
 ```console
-to_process = process.add_label_change_resolution(video_list_s3, "720p")
-process.cv_extract_specific_frame(to_process, 42)  # These screenshots will NOT be in 720p
-aux.execute_label_and_write_local(to_process)
+label.change_resolution(video_list_s3, "720p")
+extract.specific_frame_extractor(aux, video_list_s3, 42)  # These screenshots will NOT be in 720p
+aux.execute_label_and_write_local(video_list_s3)
 
 # Because the video modifications have not been executed, the images will come from the original video.
 
-to_process = process.add_label_change_resolution(video_list_s3, "720p")
+label.change_resolution(video_list_s3, "720p")
 output_list = aux.execute_label_and_write_local(to_process)
 process.cv_extract_specific_frame(output_list, 42)  # These screenshots WILL be in 720p!
 
 # Because the rescale was executed, the resulting screenshot is in 720p!
 ```
 
 All Label Utility:
@@ -162,19 +162,19 @@
 bitrate in comparison to the original will result in a loss of some i/b frames, but the output duration will remain the same. 
 
 grayscale(video_list) -> Applies a grayscale filter to all videos in video_list.
 ```
 
 All Extract Utility:
 ```console
-frame_at_time_extractor(video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
+frame_at_time_extractor(aux, video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
 
-specific_frame_extractor(video_list, frame) -> Extract the exact frame you pass as a PNG
+specific_frame_extractor(aux, video_list, frame) -> Extract the exact frame you pass as a PNG
 
-multiple_frame_extractor(video_list, start_frame, num_frames) -> Beginning at start_frame, extract the next num_frames
+multiple_frame_extractor(aux, video_list, start_frame, num_frames) -> Beginning at start_frame, extract the next num_frames
 ```
 
 Limitations:
 
 Please note the following limitations of the framework:
 
 Frames cannot be extracted from a source that has been previously executed in the processor pipeline.
```

### Comparing `aEye-1.1.0/aEye/auxiliary.py` & `aEye-1.1.1/aEye/auxiliary.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from aEye.video import Video
 import boto3
 import tempfile
 import os
 import subprocess
 import logging
-import static_ffmpeg
+from static_ffmpeg import run
 
 
 class Aux:
     """
     Aux is the class that works as a pipeline to load, write, and upload all video from S3 bucket.
 
     Attributes
@@ -189,38 +189,39 @@
                 The path to write the output videos to.
 
         """
 
         # If the user prompts this method with a specific path, then this will save it into the internal variable.
         # This will check if there exists an local path internal. If there exists, then we will write video files there.
         if path is None:
-            if self._local_path:
+            if self._local_path is not None:
                 path = self._local_path
             else:
                 self._temp_folder = tempfile.mkdtemp(dir="")
                 path = self._temp_folder
         else:
             self.set_local_path(path)
 
         list_video = []
-
+        ffmpeg, probe_path = run.get_or_fetch_platform_executables_else_raise()
         for video in video_list:
             if video.out == '':
                 source = video.get_presigned_url()
             else:
                 source = video.out
             if len(video.complex_filter) > 0:
                 video.create_complex_filter(video)
-            command = f"static_ffmpeg -y -i {source} {video.get_label()} {path}/{video.get_output_title()}"
+            command = f"{ffmpeg} -y -i {source} {video.get_label()} {path}/{video.get_output_title()}"
             subprocess.run(command, shell=True)
             logging.info(command)
-            # print(command)  # REALLY useful for debug
+            print(command)  # REALLY useful for debug
             new_path = video.get_output_title()
             video.reset_label()
             new_video = Video(f'{path}/{video.get_output_title()}', title=f'{video.get_output_title()}')
+            new_video.path = path
             new_video.set_output(f"'{path}/{new_path}'")
             list_video.append(new_video)
 
         logging.info(f"successfully write the output video files to path: {path}")
 
         return list_video
```

### Comparing `aEye-1.1.0/aEye/extractor.py` & `aEye-1.1.1/aEye/extractor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 import cv2
 import logging
 import os
-
+import tempfile
+from aEye.auxiliary import Aux
 
 class Extractor:
     """
     The Extractor class is used for frame extractions using openCV. Any time the methods
     within the Extractor are run, they will instantly execute. To get frames from processed
     videos, use Aux.execute_label_and_write_local and pass the resulting list to the extractor.
 
     Methods
     --------
 
-    frame_at_time_extractor(video_list, time) -> List[Video]
+    frame_at_time_extractor(aux, video_list, time) -> List[Video]
         Given a time as a float, extract the frame at that point and put it in the temp output folder
 
-    specific_frame_extractor(video_list, frame) -> List[Video]
+    specific_frame_extractor(aux, video_list, frame) -> List[Video]
         Will extract the frame # that is passed in and store it as a PNG in the temp folder
 
-    multiple_frame_extractor(video_list, start_frame, num_frames) -> List[Video]
+    multiple_frame_extractor(aux, video_list, start_frame, num_frames) -> List[Video]
         Extract the next num_frames after start_frame and send ALL the images to the output folder. This has the
         capacity to create a HUGE amount of images per video, use with caution!
 
     Examples
     --------
 
-    frame_at_time_extractor(s3_videos, 10) -> Output images come from timestamp 10s
+    frame_at_time_extractor(aux, s3_videos, 10) -> Output images come from timestamp 10s
 
-    specific_frame_extractor(s3_videos, 320) -> Output image comes from frame 320
+    specific_frame_extractor(aux, s3_videos, 320) -> Output image comes from frame 320
 
-    multiple_frame_extractor(s3_videos, 634, 10) -> Extract 10 contiguous frames starting from 634
+    multiple_frame_extractor(aux, s3_videos, 634, 10) -> Extract 10 contiguous frames starting from 634
     """
 
-    def frame_at_time_extractor(self, video_list, time):
+    def frame_at_time_extractor(self, aux, video_list, time):
         """
         Given a time in seconds, this will extract the closest frame.
         Img extraction that takes less than half as long as the FFMpeg version.
 
         Parameters
         -------
+        aux         : Auxiliary Loader
+            Sets the output path and creates tmp folder
 
         video_list : List[Video]
             List of all video objects loaded for processing.
 
         time       : Float
             Time in seconds to extract frame. Can be a float for higher degree of specificity
 
@@ -64,32 +67,42 @@
                 cv_video = cv2.VideoCapture(file_path)
                 fps = cv_video.get(cv2.CAP_PROP_FPS)
                 frame_id = int(fps * time)
                 cv_video.set(cv2.CAP_PROP_POS_FRAMES, frame_id)
                 ret, frame = cv_video.read()
                 actual_title = os.path.splitext(video.title)[0]
                 if video.path is None:
-                    path = file_path.split('/')[0]
-                else:
+                    video.path = tempfile.mkdtemp(dir="")
                     path = video.path
+                    aux._local_path = path
+                    aux._temp_folder = path
+                else:
+                    path = file_path.split('/')[0]
+                # if video.path is None:
+                #     path = file_path.split('/')[0]
+                # else:
+                #     path = video.path
                 cv2.imwrite(f"{path}/output_cv_extract_frame_at_time_{time}_{actual_title}.png", frame)
                 cv_video.release()
                 logging.info(f"Extracted frame at time {time}")
             except:
                 logging.error(f" Cannot extract frame at time {time} for video {video}")
         return video_list
 
-    def specific_frame_extractor(self, video_list, frame):
+    def specific_frame_extractor(self, aux, video_list, frame):
         """
         OpenCv method to grab a single frame as a PNG. Passed argument frame is the frame that
         will be extracted. (No decimals please)
 
         Parameters
         -------
 
+        aux         : Auxiliary Loader
+            Sets the output path and creates tmp folder
+
         video_list : List[Video]
             List of all video objects loaded for processing.
 
         frame      : Integer
             The frame number to be saved as a PNG
 
         Returns
@@ -108,34 +121,44 @@
                 else:
                     file_path = video.out.strip("'")
                 cv_video = cv2.VideoCapture(file_path)
                 cv_video.set(cv2.CAP_PROP_POS_FRAMES, frame)
                 ret, output = cv_video.read()
                 actual_title = os.path.splitext(video.title)[0]
                 if video.path is None:
-                    path = file_path.split('/')[0]
-                else:
+                    video.path = tempfile.mkdtemp(dir="")
                     path = video.path
+                    aux._local_path = path
+                    aux._temp_folder = path
+                else:
+                    path = file_path.split('/')[0]
+                # if video.path is None:
+                #     path = file_path.split('/')[0]
+                # else:
+                #     path = video.path
                 cv2.imwrite(f"{path}/output_cv_extract_specific_frame_{frame}_{actual_title}.png", output)
                 logging.info(f"Frame #{frame} extracted ")
                 cv_video.release()
             except:
                 logging.error(f" Cannot extract frame {frame} for video {video}")
         return video_list
 
-    def multiple_frame_extractor(self, video_list, start_frame, num_frames):
+    def multiple_frame_extractor(self, aux, video_list, start_frame, num_frames):
         """
         Given a start_frame, extract the next num_frames from the video, and store the resulting
         collection of frames in the output folder. num_Frames is the number of frames to be returned
         Has the potential to create like a million images, only use this when you REALLY need a lot
         of frames or a specific set of frames.
 
         Parameters
         -------
 
+        aux         : Auxiliary Loader
+            Sets the output path and creates tmp folder
+
         video_list  : List[Video]
             List of all video objects loaded for processing.
 
         start_frame : Integer
             Number of the frame at which to start all the frame grabs.
 
         num_frames  : Integer
@@ -145,33 +168,39 @@
         Returns
         -------
 
         Returns a list of Videos, and many frames are output as PNG's
         """
         for video in video_list:
             try:
-                assert 0 <= start_frame < int(video.get_num_frames()) and int(
-                    start_frame + num_frames) <= int(video.get_num_frames())
                 if video.label != '':
                     logging.error(
                         f"WARNING: Video {video} has processing to execute still! Resulting images will NOT have these modifications applied!")
                 if video.out == '':
                     file_path = video.get_presigned_url().strip("'")
                 else:
                     file_path = video.out.strip("'")
                 vid_obj = cv2.VideoCapture(file_path)
                 actual_title = os.path.splitext(video.title)[0]
                 if video.path is None:
-                    path = file_path.split('/')[0]
-                else:
+                    video.path = tempfile.mkdtemp(dir="")
                     path = video.path
+                    aux._local_path = path
+                    aux._temp_folder = path
+                else:
+                    path = file_path.split('/')[0]
+                # if video.path is None:
+                #     path = file_path.split('/')[0]
+                # else:
+                #     path = video.path
                 #  Sets the relative file location
                 for x in range(num_frames):
                     vid_obj.set(cv2.CAP_PROP_POS_FRAMES, start_frame + x)
                     ret, frame = vid_obj.read()
                     fn = f"{path}/output_extract_many_frames_{start_frame}_{num_frames}_{actual_title}_{x}.png"
+                    #fn = f"images/output_extract_many_frames_{start_frame}_{num_frames}_{actual_title}_{x}.png"
                     cv2.imwrite(fn, frame)
                 vid_obj.release()
                 logging.info(f"Extracted {num_frames} from video, saved as PNG's")
             except:
                 logging.error(f" Cannot extract {num_frames} starting from frame {start_frame}!")
         return video_list
```

### Comparing `aEye-1.1.0/aEye/labeler.py` & `aEye-1.1.1/aEye/labeler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import math
-
+import subprocess
 
 
 class Labeler:
     """
     The Labler class works by applying "labels" to a Video object. These labels are
     FFmpeg commands that will be executed upon the Aux.execute_label_and_write_local command.
     If two simple labels of the same type (trim for example) are applied, only the most recent
@@ -380,15 +380,15 @@
         -------
 
         List of videos with the blur label applied
         """
         for video in video_list:
             try:
                 assert blur_level in range(0, 52) and blur_steps in range(1, 6)
-                video.complex_filter.append(f"gblur=sigma={blur_level}:steps={blur_steps} ")
+                video.complex_filter.append(f"gblur=sigma={blur_level}:steps={blur_steps}")
                 video.add_output_title(f"blurred_{blur_level}x{blur_steps}_")
                 logging.info(f"Created a blur of strength {blur_level} and applied it {blur_steps} times")
             except:
                 logging.error(
                     f" Cannot create a blur with level {blur_level} (max 51) and {blur_steps} steps (max 5) for video {video}")
         return video_list
 
@@ -457,31 +457,31 @@
             try:
                 video.complex_filter.append(f"fps={new_framerate}")
                 video.add_output_title(f"framerate_{new_framerate}_")
             except:
                 logging.error(f" Cannot adjust video {video} framerate to {new_framerate}!")
         return video_list
 
-    def grayscale(self, video_list):
+    def greyscale(self, video_list):
         """
-        Applies grayscale to all videos in the queue
+        Applies greyscale to all videos in the queue
 
         Parameters
         ----------
 
         video_list : List[Video]
-            List of all videos to apply grayscale to
+            List of all videos to apply greyscale to
 
         Returns
         ----------
 
         List of all videos with complex filter applied
         """
         for video in video_list:
             try:
                 video.complex_filter.append(f"format=gray")
-                video.add_output_title(f"grayscale_")
+                video.add_output_title(f"greyscale_")
             except:
-                logging.error(f"Cannot apply grayscale to video {video}")
+                logging.error(f"Cannot apply greyscale to video {video}")
         return video_list
```

### Comparing `aEye-1.1.0/aEye/video.py` & `aEye-1.1.1/aEye/video.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.0/aEye.egg-info/PKG-INFO` & `aEye-1.1.1/aEye.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -128,21 +128,21 @@
 The framework allows frames to be extracted at any point while processing, but if there are pending processor modifications, a warning will be raised, and the resulting images will come from the original source. 
 The execution order affects frame capture.
 
 Example:
 
 
 ```console
-to_process = process.add_label_change_resolution(video_list_s3, "720p")
-process.cv_extract_specific_frame(to_process, 42)  # These screenshots will NOT be in 720p
-aux.execute_label_and_write_local(to_process)
+label.change_resolution(video_list_s3, "720p")
+extract.specific_frame_extractor(aux, video_list_s3, 42)  # These screenshots will NOT be in 720p
+aux.execute_label_and_write_local(video_list_s3)
 
 # Because the video modifications have not been executed, the images will come from the original video.
 
-to_process = process.add_label_change_resolution(video_list_s3, "720p")
+label.change_resolution(video_list_s3, "720p")
 output_list = aux.execute_label_and_write_local(to_process)
 process.cv_extract_specific_frame(output_list, 42)  # These screenshots WILL be in 720p!
 
 # Because the rescale was executed, the resulting screenshot is in 720p!
 ```
 
 All Label Utility:
@@ -172,19 +172,19 @@
 bitrate in comparison to the original will result in a loss of some i/b frames, but the output duration will remain the same. 
 
 grayscale(video_list) -> Applies a grayscale filter to all videos in video_list.
 ```
 
 All Extract Utility:
 ```console
-frame_at_time_extractor(video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
+frame_at_time_extractor(aux, video_list, time) -> Given a time (can be a float), find the closest B-Frame and extract it
 
-specific_frame_extractor(video_list, frame) -> Extract the exact frame you pass as a PNG
+specific_frame_extractor(aux, video_list, frame) -> Extract the exact frame you pass as a PNG
 
-multiple_frame_extractor(video_list, start_frame, num_frames) -> Beginning at start_frame, extract the next num_frames
+multiple_frame_extractor(aux, video_list, start_frame, num_frames) -> Beginning at start_frame, extract the next num_frames
 ```
 
 Limitations:
 
 Please note the following limitations of the framework:
 
 Frames cannot be extracted from a source that has been previously executed in the processor pipeline.
```

### Comparing `aEye-1.1.0/setup.py` & `aEye-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 def get_version():
     """
     Checks commandline arguments for a user specified Version number.
     If the --version flag is not given at run time, then the version number is defaulted to
-    v1.1.0, which will later be replaced with a git tag when performing
+    v1.1.1, which will later be replaced with a git tag when performing
     version releases.
 
     Returns
     -------
     when the bdist_wheel command is given a version flag and version number, such as:
 
     --version 1.x.x
@@ -36,15 +36,15 @@
     If the --version flag is given, but no version number is supplied, such as:
 
     --version
 
     then an IndexError will be thrown and the build will exit with exit status 1.
 
     """
-    version = 'v1.1.0'
+    version = 'v1.1.1'
     if "--version" in sys.argv:
         try:
             version = sys.argv[3]
             sys.argv.remove(sys.argv[3])
         except IndexError as e:
             print("error:  " + str(e))
             print("supply a version number i.e. --version 1.x.x")
```

### Comparing `aEye-1.1.0/tests/test_extract_metadata.py` & `aEye-1.1.1/tests/test_extract_metadata.py`

 * *Files identical despite different names*

