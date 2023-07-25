# Comparing `tmp/blendersynth-0.0.4.tar.gz` & `tmp/blendersynth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendersynth-0.0.4.tar", last modified: Thu Jul 13 08:17:49 2023, max compression
+gzip compressed data, was "blendersynth-0.0.5.tar", last modified: Tue Jul 25 13:12:19 2023, max compression
```

## Comparing `blendersynth-0.0.4.tar` & `blendersynth-0.0.5.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.907982 blendersynth-0.0.4/
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.891185 blendersynth-0.0.4/BlenderSynth.egg-info/
--rw-r--r--   0 ollie      (501) staff       (20)     2034 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1835 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/SOURCES.txt
--rw-r--r--   0 ollie      (501) staff       (20)        1 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/dependency_links.txt
--rw-r--r--   0 ollie      (501) staff       (20)       40 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/requires.txt
--rw-r--r--   0 ollie      (501) staff       (20)       13 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/top_level.txt
--rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.4/LICENSE
--rw-r--r--   0 ollie      (501) staff       (20)     2034 2023-07-13 08:17:49.907807 blendersynth-0.0.4/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1759 2023-07-12 13:02:47.000000 blendersynth-0.0.4/README.md
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.890748 blendersynth-0.0.4/blendersynth/
--rw-r--r--   0 ollie      (501) staff       (20)     1650 2023-07-10 19:24:35.000000 blendersynth-0.0.4/blendersynth/__init__.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.894613 blendersynth-0.0.4/blendersynth/annotations/
--rw-r--r--   0 ollie      (501) staff       (20)      133 2023-07-10 22:37:06.000000 blendersynth-0.0.4/blendersynth/annotations/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     2066 2023-07-10 22:37:46.000000 blendersynth-0.0.4/blendersynth/annotations/axes.py
--rw-r--r--   0 ollie      (501) staff       (20)     2440 2023-07-09 12:11:14.000000 blendersynth-0.0.4/blendersynth/annotations/bbox.py
--rw-r--r--   0 ollie      (501) staff       (20)      656 2023-07-09 12:11:14.000000 blendersynth-0.0.4/blendersynth/annotations/keypoints.py
--rw-r--r--   0 ollie      (501) staff       (20)     1387 2023-07-09 12:13:20.000000 blendersynth-0.0.4/blendersynth/annotations/utils.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.899966 blendersynth-0.0.4/blendersynth/blender/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-07-05 14:54:19.000000 blendersynth-0.0.4/blendersynth/blender/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     8664 2023-07-05 14:37:51.000000 blendersynth-0.0.4/blendersynth/blender/aov.py
--rw-r--r--   0 ollie      (501) staff       (20)     1525 2023-07-07 11:07:54.000000 blendersynth-0.0.4/blendersynth/blender/bsyn_object.py
--rw-r--r--   0 ollie      (501) staff       (20)     6288 2023-07-07 12:50:10.000000 blendersynth-0.0.4/blendersynth/blender/camera.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.902098 blendersynth-0.0.4/blendersynth/blender/compositor/
--rw-r--r--   0 ollie      (501) staff       (20)       34 2023-07-05 13:24:45.000000 blendersynth-0.0.4/blendersynth/blender/compositor/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)    11373 2023-07-10 22:37:06.000000 blendersynth-0.0.4/blendersynth/blender/compositor/compositor.py
--rw-r--r--   0 ollie      (501) staff       (20)     6574 2023-07-10 22:39:48.000000 blendersynth-0.0.4/blendersynth/blender/compositor/image_overlay.py
--rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.4/blendersynth/blender/compositor/mask_overlay.py
--rw-r--r--   0 ollie      (501) staff       (20)      887 2023-07-10 22:40:32.000000 blendersynth-0.0.4/blendersynth/blender/compositor/node_group.py
--rw-r--r--   0 ollie      (501) staff       (20)     1103 2023-07-05 12:25:55.000000 blendersynth-0.0.4/blendersynth/blender/compositor/visuals.py
--rw-r--r--   0 ollie      (501) staff       (20)     1218 2023-07-05 12:25:55.000000 blendersynth-0.0.4/blendersynth/blender/curve.py
--rw-r--r--   0 ollie      (501) staff       (20)     1843 2023-07-05 15:30:58.000000 blendersynth-0.0.4/blendersynth/blender/light.py
--rw-r--r--   0 ollie      (501) staff       (20)    17430 2023-07-12 14:35:28.000000 blendersynth-0.0.4/blendersynth/blender/mesh.py
--rw-r--r--   0 ollie      (501) staff       (20)     1491 2023-07-05 15:36:05.000000 blendersynth-0.0.4/blendersynth/blender/render.py
--rw-r--r--   0 ollie      (501) staff       (20)     3191 2023-07-12 14:28:48.000000 blendersynth-0.0.4/blendersynth/blender/utils.py
--rw-r--r--   0 ollie      (501) staff       (20)     2444 2023-07-10 21:23:07.000000 blendersynth-0.0.4/blendersynth/blender/world.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.904062 blendersynth-0.0.4/blendersynth/file/
--rw-r--r--   0 ollie      (501) staff       (20)      152 2023-07-07 19:23:23.000000 blendersynth-0.0.4/blendersynth/file/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     1005 2023-07-05 13:57:01.000000 blendersynth-0.0.4/blendersynth/file/dataset_inputs.py
--rw-r--r--   0 ollie      (501) staff       (20)      318 2023-07-09 12:14:45.000000 blendersynth-0.0.4/blendersynth/file/dataset_outputs.py
--rw-r--r--   0 ollie      (501) staff       (20)      497 2023-07-07 19:24:14.000000 blendersynth-0.0.4/blendersynth/file/ffmpeg_utils.py
--rw-r--r--   0 ollie      (501) staff       (20)     3001 2023-07-07 10:33:19.000000 blendersynth-0.0.4/blendersynth/file/frames_to_video.py
--rw-r--r--   0 ollie      (501) staff       (20)      618 2023-07-05 13:54:50.000000 blendersynth-0.0.4/blendersynth/file/tempfiles.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.905496 blendersynth-0.0.4/blendersynth/run/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.4/blendersynth/run/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.4/blendersynth/run/blender_interface.py
--rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.4/blendersynth/run/blender_threading.py
--rw-r--r--   0 ollie      (501) staff       (20)     3278 2023-07-09 12:37:15.000000 blendersynth-0.0.4/blendersynth/run/run.py
--rw-r--r--   0 ollie      (501) staff       (20)      859 2023-07-12 13:54:07.000000 blendersynth-0.0.4/blendersynth/run/run_this_script.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.906266 blendersynth-0.0.4/blendersynth/utils/
--rw-r--r--   0 ollie      (501) staff       (20)       43 2023-07-07 10:33:19.000000 blendersynth-0.0.4/blendersynth/utils/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      713 2023-07-07 10:33:19.000000 blendersynth-0.0.4/blendersynth/utils/blender_importer.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.907446 blendersynth-0.0.4/blendersynth/utils/blender_setup/
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.4/blendersynth/utils/blender_setup/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     4475 2023-07-07 10:33:19.000000 blendersynth-0.0.4/blendersynth/utils/blender_setup/blender_locator.py
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.4/blendersynth/utils/blender_setup/blender_python_path.py
--rw-r--r--   0 ollie      (501) staff       (20)     2956 2023-07-12 13:58:45.000000 blendersynth-0.0.4/blendersynth/utils/blender_setup/check_blender_install.py
--rw-r--r--   0 ollie      (501) staff       (20)     3604 2023-07-09 12:37:15.000000 blendersynth-0.0.4/blendersynth/utils/node_arranger.py
--rw-r--r--   0 ollie      (501) staff       (20)      409 2023-07-13 08:17:27.000000 blendersynth-0.0.4/pyproject.toml
--rw-r--r--   0 ollie      (501) staff       (20)       38 2023-07-13 08:17:49.908049 blendersynth-0.0.4/setup.cfg
--rw-r--r--   0 ollie      (501) staff       (20)      245 2023-07-13 08:17:27.000000 blendersynth-0.0.4/setup.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.699272 blendersynth-0.0.5/
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.686253 blendersynth-0.0.5/BlenderSynth.egg-info/
+-rw-r--r--   0 ollie      (501) staff       (20)     2129 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1896 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/SOURCES.txt
+-rw-r--r--   0 ollie      (501) staff       (20)        1 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/dependency_links.txt
+-rw-r--r--   0 ollie      (501) staff       (20)       40 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/requires.txt
+-rw-r--r--   0 ollie      (501) staff       (20)       13 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/top_level.txt
+-rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.5/LICENSE
+-rw-r--r--   0 ollie      (501) staff       (20)     2129 2023-07-25 13:12:19.699118 blendersynth-0.0.5/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1854 2023-07-24 10:03:26.000000 blendersynth-0.0.5/README.md
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.685681 blendersynth-0.0.5/blendersynth/
+-rw-r--r--   0 ollie      (501) staff       (20)     1807 2023-07-24 20:40:32.000000 blendersynth-0.0.5/blendersynth/__init__.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.687777 blendersynth-0.0.5/blendersynth/annotations/
+-rw-r--r--   0 ollie      (501) staff       (20)      133 2023-07-10 22:37:06.000000 blendersynth-0.0.5/blendersynth/annotations/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2066 2023-07-10 22:37:46.000000 blendersynth-0.0.5/blendersynth/annotations/axes.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2440 2023-07-09 12:11:14.000000 blendersynth-0.0.5/blendersynth/annotations/bbox.py
+-rw-r--r--   0 ollie      (501) staff       (20)      656 2023-07-09 12:11:14.000000 blendersynth-0.0.5/blendersynth/annotations/keypoints.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1387 2023-07-09 12:13:20.000000 blendersynth-0.0.5/blendersynth/annotations/utils.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.691050 blendersynth-0.0.5/blendersynth/blender/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-07-05 14:54:19.000000 blendersynth-0.0.5/blendersynth/blender/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     8763 2023-07-13 15:44:48.000000 blendersynth-0.0.5/blendersynth/blender/aov.py
+-rw-r--r--   0 ollie      (501) staff       (20)     6498 2023-07-25 12:59:05.000000 blendersynth-0.0.5/blendersynth/blender/bsyn_object.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3571 2023-07-25 12:19:49.000000 blendersynth-0.0.5/blendersynth/blender/camera.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.692617 blendersynth-0.0.5/blendersynth/blender/compositor/
+-rw-r--r--   0 ollie      (501) staff       (20)       34 2023-07-05 13:24:45.000000 blendersynth-0.0.5/blendersynth/blender/compositor/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)    14112 2023-07-24 12:32:58.000000 blendersynth-0.0.5/blendersynth/blender/compositor/compositor.py
+-rw-r--r--   0 ollie      (501) staff       (20)     6574 2023-07-10 22:39:48.000000 blendersynth-0.0.5/blendersynth/blender/compositor/image_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.5/blendersynth/blender/compositor/mask_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)      887 2023-07-10 22:40:32.000000 blendersynth-0.0.5/blendersynth/blender/compositor/node_group.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1103 2023-07-05 12:25:55.000000 blendersynth-0.0.5/blendersynth/blender/compositor/visuals.py
+-rw-r--r--   0 ollie      (501) staff       (20)      726 2023-07-25 10:21:51.000000 blendersynth-0.0.5/blendersynth/blender/curve.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2261 2023-07-25 13:11:41.000000 blendersynth-0.0.5/blendersynth/blender/light.py
+-rw-r--r--   0 ollie      (501) staff       (20)     4779 2023-07-25 08:10:33.000000 blendersynth-0.0.5/blendersynth/blender/material.py
+-rw-r--r--   0 ollie      (501) staff       (20)    15416 2023-07-25 13:11:41.000000 blendersynth-0.0.5/blendersynth/blender/mesh.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1491 2023-07-05 15:36:05.000000 blendersynth-0.0.5/blendersynth/blender/render.py
+-rw-r--r--   0 ollie      (501) staff       (20)     7380 2023-07-25 12:57:52.000000 blendersynth-0.0.5/blendersynth/blender/utils.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3170 2023-07-24 14:32:46.000000 blendersynth-0.0.5/blendersynth/blender/world.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.694598 blendersynth-0.0.5/blendersynth/file/
+-rw-r--r--   0 ollie      (501) staff       (20)      152 2023-07-24 12:27:08.000000 blendersynth-0.0.5/blendersynth/file/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1165 2023-07-24 12:27:08.000000 blendersynth-0.0.5/blendersynth/file/dataset_inputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)      318 2023-07-09 12:14:45.000000 blendersynth-0.0.5/blendersynth/file/dataset_outputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)      497 2023-07-07 19:24:14.000000 blendersynth-0.0.5/blendersynth/file/ffmpeg_utils.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3001 2023-07-07 10:33:19.000000 blendersynth-0.0.5/blendersynth/file/frames_to_video.py
+-rw-r--r--   0 ollie      (501) staff       (20)      618 2023-07-05 13:54:50.000000 blendersynth-0.0.5/blendersynth/file/tempfiles.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.696211 blendersynth-0.0.5/blendersynth/run/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.5/blendersynth/run/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.5/blendersynth/run/blender_interface.py
+-rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.5/blendersynth/run/blender_threading.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3278 2023-07-09 12:37:15.000000 blendersynth-0.0.5/blendersynth/run/run.py
+-rw-r--r--   0 ollie      (501) staff       (20)      859 2023-07-12 13:54:07.000000 blendersynth-0.0.5/blendersynth/run/run_this_script.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.697611 blendersynth-0.0.5/blendersynth/utils/
+-rw-r--r--   0 ollie      (501) staff       (20)       43 2023-07-07 10:33:19.000000 blendersynth-0.0.5/blendersynth/utils/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      713 2023-07-07 10:33:19.000000 blendersynth-0.0.5/blendersynth/utils/blender_importer.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.698670 blendersynth-0.0.5/blendersynth/utils/blender_setup/
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.5/blendersynth/utils/blender_setup/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     4475 2023-07-07 10:33:19.000000 blendersynth-0.0.5/blendersynth/utils/blender_setup/blender_locator.py
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.5/blendersynth/utils/blender_setup/blender_python_path.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3000 2023-07-24 09:59:41.000000 blendersynth-0.0.5/blendersynth/utils/blender_setup/check_blender_install.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3604 2023-07-09 12:37:15.000000 blendersynth-0.0.5/blendersynth/utils/node_arranger.py
+-rw-r--r--   0 ollie      (501) staff       (20)      619 2023-07-25 13:01:55.000000 blendersynth-0.0.5/blendersynth/utils/types.py
+-rw-r--r--   0 ollie      (501) staff       (20)      409 2023-07-25 13:12:11.000000 blendersynth-0.0.5/pyproject.toml
+-rw-r--r--   0 ollie      (501) staff       (20)       38 2023-07-25 13:12:19.699322 blendersynth-0.0.5/setup.cfg
+-rw-r--r--   0 ollie      (501) staff       (20)      245 2023-07-25 13:12:11.000000 blendersynth-0.0.5/setup.py
```

### Comparing `blendersynth-0.0.4/BlenderSynth.egg-info/PKG-INFO` & `blendersynth-0.0.5/BlenderSynth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.4
+Version: 0.0.5
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
@@ -56,12 +56,12 @@
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
 
 ## Troubleshooting
 
-If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
+If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both. If you are making changes to the local clone, use `editable=True` to install in editable mode.
 
 ## Benchmarking
 
 ![](docs/benchmark-1.png)
```

### Comparing `blendersynth-0.0.4/BlenderSynth.egg-info/SOURCES.txt` & `blendersynth-0.0.5/BlenderSynth.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 blendersynth/annotations/utils.py
 blendersynth/blender/__init__.py
 blendersynth/blender/aov.py
 blendersynth/blender/bsyn_object.py
 blendersynth/blender/camera.py
 blendersynth/blender/curve.py
 blendersynth/blender/light.py
+blendersynth/blender/material.py
 blendersynth/blender/mesh.py
 blendersynth/blender/render.py
 blendersynth/blender/utils.py
 blendersynth/blender/world.py
 blendersynth/blender/compositor/__init__.py
 blendersynth/blender/compositor/compositor.py
 blendersynth/blender/compositor/image_overlay.py
@@ -43,11 +44,12 @@
 blendersynth/run/blender_interface.py
 blendersynth/run/blender_threading.py
 blendersynth/run/run.py
 blendersynth/run/run_this_script.py
 blendersynth/utils/__init__.py
 blendersynth/utils/blender_importer.py
 blendersynth/utils/node_arranger.py
+blendersynth/utils/types.py
 blendersynth/utils/blender_setup/__init__.py
 blendersynth/utils/blender_setup/blender_locator.py
 blendersynth/utils/blender_setup/blender_python_path.py
 blendersynth/utils/blender_setup/check_blender_install.py
```

### Comparing `blendersynth-0.0.4/LICENSE` & `blendersynth-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/PKG-INFO` & `blendersynth-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.4
+Version: 0.0.5
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
@@ -56,12 +56,12 @@
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
 
 ## Troubleshooting
 
-If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
+If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both. If you are making changes to the local clone, use `editable=True` to install in editable mode.
 
 ## Benchmarking
 
 ![](docs/benchmark-1.png)
```

### Comparing `blendersynth-0.0.4/README.md` & `blendersynth-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
 
 ## Troubleshooting
 
-If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
+If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both. If you are making changes to the local clone, use `editable=True` to install in editable mode.
 
 ## Benchmarking
 
 ![](docs/benchmark-1.png)
```

### Comparing `blendersynth-0.0.4/blendersynth/__init__.py` & `blendersynth-0.0.5/blendersynth/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 from .utils.blender_setup import check_blender_install
 
 building_docs = 'sphinx' in sys.modules
 
 if not building_docs:
 	check_blender_install(blendersynth_from_local='--local' in sys.argv) # check install here
 
-def fix_blender_install(local=False):
-	check_blender_install(force_all=True, blendersynth_from_local=local)
+def fix_blender_install(local=False, editable=False):
+	check_blender_install(force_all=True, blendersynth_from_local=local, blendersynth_editable=editable)
 
-def fix_blender_modules(local=False):
-	check_blender_install(force_install_dependencies=True, blendersynth_from_local=local)
+def fix_blender_modules(local=False, editable=False):
+	check_blender_install(force_install_dependencies=True, blendersynth_from_local=local,
+						  blendersynth_editable=editable)
 
 from .run.run_this_script import run_this_script
 
 import sys
 from .utils.blender_setup.blender_locator import get_blender_path
 
 if building_docs or get_blender_path() == sys.argv[0]:  # if blender is running this script, or if building docs
 	import bpy
 	from bpy import *
 	from .blender.mesh import Mesh
+	from .blender.material import Material
 	from .blender.curve import Curve
 	from .blender import render
 	from .blender.compositor.compositor import Compositor
 	from .blender import aov
-	from .file.dataset_inputs import INPUTS
+	from .file.dataset_inputs import Inputs, DebugInputs
 	from . import file
 	from .run.blender_interface import log_event
 	from .blender.world import world
 	from .blender.light import Light
 	from .blender.camera import Camera
 	from . import annotations
 	from .file.tempfiles import cleanup_temp_files as cleanup
```

### Comparing `blendersynth-0.0.4/blendersynth/annotations/axes.py` & `blendersynth-0.0.5/blendersynth/annotations/axes.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/annotations/bbox.py` & `blendersynth-0.0.5/blendersynth/annotations/bbox.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/annotations/keypoints.py` & `blendersynth-0.0.5/blendersynth/annotations/keypoints.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/annotations/utils.py` & `blendersynth-0.0.5/blendersynth/annotations/utils.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/blender/aov.py` & `blendersynth-0.0.5/blendersynth/blender/aov.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 """Shader AOV manager"""
 
 import bpy
 from ..utils.node_arranger import tidy_tree
 
 ref_frames = ['CAMERA', 'WORLD', 'OBJECT']
 
+# Acceptable socket types for AOV colors & nodes
+_socket_color_types = (bpy.types.NodeSocketVector, bpy.types.NodeSocketColor)
+_socket_value_types = (bpy.types.NodeSocketFloat, bpy.types.NodeSocketInt)
+
 class AOV:
 	"""A generic Arbitrary Output Value.
 	An AOV is a float or color value that can be output from a shader to the renderer.
 	See `Blender docs <https://docs.blender.org/manual/en/latest/render/shader_nodes/output/aov.html>`_ for more info.
 	"""
 
 	AOV_TYPE = 'COLOR'
 	def __init__(self, name=None, **kwargs):
 		if name is None:
 			name = self.__class__.__name__
 
 		self.name = name
+		self._aov = None
 		self._add_to_view_layer()
 
 	def _add_to_view_layer(self, view_layer=None):
 		"""Add aov to view layer if not already there"""
 		if view_layer is None:
 			view_layer = bpy.context.view_layer
 
 		for aov in view_layer.aovs:
 			if aov.name == self.name:
 				return
 
 		aov = view_layer.aovs.add()
 		aov.name = self.name
-		aov.type = self.AOV_TYPE
+		self._aov = aov
+
 
 	def add_to_shader(self, shader_node_tree):
 		"""Add AOV to shader node tree"""
-		self._add_to_shader(shader_node_tree)
+		# add_to_shader must return output socket to connect to node
+		out_socket = self._add_to_shader(shader_node_tree)
+
+		# check node socket is correct type
+		AOV_TYPE = None
+		if isinstance(out_socket, _socket_color_types):
+			AOV_TYPE = 'COLOR'
+		elif isinstance(out_socket, _socket_value_types):
+			AOV_TYPE = 'VALUE'
+		else:
+			raise ValueError(f"Output of _add_to_layer must be in {_socket_color_types} if Color or {_socket_value_types} if value. Got: `{type(out_socket)}`")
+
+		shader_aov_node = shader_node_tree.nodes.new('ShaderNodeOutputAOV')
+		shader_aov_node.name = self.name
+		shader_node_tree.links.new(out_socket, shader_aov_node.inputs[AOV_TYPE.title()])
+
+		self._aov.type = self.AOV_TYPE
 		tidy_tree(shader_node_tree)
 
-	def _add_to_shader(self, shader_node_tree):
+	def _add_to_shader(self, shader_node_tree) -> bpy.types.NodeSocket:
 		raise NotImplementedError
 
 	def update(self):
 		"""Some AOVs need an update before rendering (to change certain node properties)"""
 		return
 
 	def __str__(self):
@@ -67,16 +89,14 @@
 		self.polarity = polarity
 
 	def _add_to_shader(self, shader_node_tree):
 
 		geom_node = shader_node_tree.nodes.new('ShaderNodeNewGeometry')
 		vec_transform = shader_node_tree.nodes.new('ShaderNodeVectorTransform')
 		map_range_node = shader_node_tree.nodes.new('ShaderNodeMapRange')
-		shader_aov_node = shader_node_tree.nodes.new('ShaderNodeOutputAOV')
-		shader_aov_node.name = self.name
 
 		vec_transform.vector_type = 'NORMAL'
 		vec_transform.convert_to = self.ref_frame
 
 		# Set up mapping - with polarity
 		map_range_node.data_type = 'FLOAT_VECTOR'
 		for i in range(3):
@@ -89,57 +109,47 @@
 		for i in range(3):
 			shader_node_tree.links.new(sep_xyz_node.outputs[self.order[i]], comb_xyz_node.inputs['XYZ'[i]])
 
 		# Make necessary connections for shader graph
 		shader_node_tree.links.new(geom_node.outputs['True Normal'], vec_transform.inputs['Vector'])
 		shader_node_tree.links.new(vec_transform.outputs['Vector'], map_range_node.inputs['Vector'])
 		shader_node_tree.links.new(map_range_node.outputs['Vector'], sep_xyz_node.inputs['Vector'])
-		shader_node_tree.links.new(comb_xyz_node.outputs['Vector'], shader_aov_node.inputs['Color'])
+
+		return comb_xyz_node.outputs['Vector']
 
 	def update(self, scene=None):
 		"""Some AOVs may need render_time updates from scene context, hence this method"""
 		pass
 
 class NOCAOV(AOV):
 	"""Normalised object coordinates - Gives the position of the object in object space,
 	normalised to the object's bounding box."""
 
 	def _add_to_shader(self, shader_node_tree):
 		texcon_node = shader_node_tree.nodes.new('ShaderNodeTexCoord')
-		shader_aov_node = shader_node_tree.nodes.new('ShaderNodeOutputAOV')
-		shader_aov_node.name = self.name
-
-		shader_node_tree.links.new(texcon_node.outputs['Generated'], shader_aov_node.inputs['Color'])
-
+		return texcon_node.outputs['Generated']
 
 class UVAOV(AOV):
 	"""UV coordinates"""
 
 	def _add_to_shader(self, shader_node_tree):
 		texcon_node = shader_node_tree.nodes.new('ShaderNodeTexCoord')
-		shader_aov_node = shader_node_tree.nodes.new('ShaderNodeOutputAOV')
-		shader_aov_node.name = self.name
-
-		shader_node_tree.links.new(texcon_node.outputs['UV'], shader_aov_node.inputs['Color'])
+		return texcon_node.outputs['UV']
 
 
 class AttrAOV(AOV):
 	"""Take an object attribute, and output it as an AOV"""
 	attribute_type = None
 	attribute_name = None
 
 	def _add_to_shader(self, shader_node_tree):
 		attr_node = shader_node_tree.nodes.new('ShaderNodeAttribute')
 		attr_node.attribute_type = self.attribute_type
 		attr_node.attribute_name = self.attribute_name
-
-		shader_aov_node = shader_node_tree.nodes.new('ShaderNodeOutputAOV')
-		shader_aov_node.name = self.name
-
-		shader_node_tree.links.new(attr_node.outputs['Instance Index'], shader_aov_node.inputs['Value'])
+		return attr_node.outputs['Instance Index']
 
 class InstanceIDAOV(AttrAOV):
 	"""Instance ID - given to each object on creation.
 	Output is an integer corresponding to the object's instance ID (0-indexed)
 	"""
 	attribute_type = 'OBJECT'
 	attribute_name = 'instance_id'
@@ -195,19 +205,16 @@
 		attr_node.attribute_type = self.attribute_type
 		attr_node.attribute_name = self.attribute_name
 
 		# Create a group node for the Int Index -> HSV conversion
 		group_node = shader_node_tree.nodes.new('ShaderNodeGroup')
 		group_node.node_tree = self.group
 
-		shader_aov_node = shader_node_tree.nodes.new('ShaderNodeOutputAOV')
-		shader_aov_node.name = self.name
-
 		shader_node_tree.links.new(attr_node.outputs['Fac'], group_node.inputs['Index'])
-		shader_node_tree.links.new(group_node.outputs['Color'], shader_aov_node.inputs['Color'])
+		return group_node.outputs['Color']
 
 	def update(self):
 		self.div_node.inputs[1].default_value = self.N
 
 	@property
 	def N(self):
 		return 0
```

### Comparing `blendersynth-0.0.4/blendersynth/blender/camera.py` & `blendersynth-0.0.5/blendersynth/blender/bsyn_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,202 +1,201 @@
-import bpy
+"""Base class for all BlenderSynth objects."""
+from .utils import handle_vec, SelectObjects, _euler_add, _euler_from, animatable_property
+from mathutils import Vector, Euler
 import numpy as np
-import mathutils
-from .utils import handle_vec, SelectObjects
-from .bsyn_object import BsynObject, animatable_property
+import bpy
 from typing import Union
-from .mesh import Mesh
-from .curve import Curve
-
-
-def look_at_rotation(obj_camera: bpy.types.Object,
-					 at: mathutils.Vector = mathutils.Vector((0, 0, 0)),
-					 up: mathutils.Vector = mathutils.Vector((0, 1, 0))) -> mathutils.Euler:
-	"""	Rotate camera to look at 'at', with 'up' maintained.
+from ..utils import types
 
-	:param obj_camera: Camera object
-	:param at: Point to look at
-	:param up: Up vector"""
+class BsynObject:
+	"""Generic class for BlenderSynth objects."""
+	_object = None # corresponding blender object
 
-	camera_position = obj_camera.location
-
-	z_axis = - (at - camera_position).normalized()  # Blender forwards is '-z', so use -ve here
-	x_axis = up.cross(z_axis)
-	y_axis = z_axis.cross(x_axis).normalized()
-	is_close = all(abs(i) < 5e-3 for i in x_axis)
-
-	if is_close:
-		replacement = y_axis.cross(z_axis).normalized()
-		x_axis = replacement
-
-	R = mathutils.Matrix([x_axis, y_axis, z_axis]).transposed()
-	euler = R.to_euler()
-	return euler
+	@property
+	def obj(self):
+		if self._object is None:
+			raise ValueError("self._object not set. Ensure it is set in the Object's __init__ function.")
 
+		return self._object
 
-class Camera(BsynObject):
-	"""Camera object, to handle movement, tracking, etc."""
+	@property
+	def object(self):
+		return self.obj
 
-	def __init__(self, camera: bpy.types.Object = None):
-		if camera is None:
-			camera = bpy.context.scene.camera
+	@property
+	def data(self):
+		return self.object.data
 
-		self.camera = camera
-		self._object = camera
+	# def update(self):
+	#   ---> not currently needed, may be needed in the future
+	# 	"""On any update, run this. For most objects, this is a no-op, but for some objects,
+	# 	this is necessary to update the object's state. e.g. Camera"""
+	# 	return
 
-	@classmethod
-	def create(cls, name: str = 'Camera',
-			   location: Union[list, tuple, np.ndarray] = None,
-			   rotation: Union[list, tuple, np.ndarray] = None) -> 'Camera':
-		"""Create a new camera object.
+	def _keyframe_delete(self, *args, **kwargs):
+		self._object.keyframe_delete(*args, **kwargs)
 
-		:param name: Name of camera
-		:param location: Location of camera
-		:param rotation_euler: Rotation of camera in euler angles"""
+	def _keyframe_insert(self, *args, **kwargs):
+		self._object.keyframe_insert(*args, **kwargs)
 
-		with SelectObjects():  # revert selection after creating camera
-			bpy.ops.object.camera_add(enter_editmode=False, align='VIEW')
-			camera = bpy.context.object
-			camera.name = name
+	@property
+	def _all_objects(self):
+		"""List of all objects associated with this object."""
+		return [self.object]
 
-		cam = cls(camera)
+	@property
+	def location(self) -> Vector:
+		"""Location of object"""
+		return self.obj.location
 
-		if location is not None:
-			cam.set_location(location)
+	@location.setter
+	def location(self, value):
+		self.set_location(value)
 
-		if rotation is not None:
-			cam.set_rotation_euler(rotation)
+	@property
+	def rotation_euler(self) -> Euler:
+		"""Rotation in euler XYZ angles"""
+		return self.obj.rotation_euler
 
-		return cam
+	@rotation_euler.setter
+	def rotation_euler(self, value):
+		self.set_rotation_euler(value)
 
-	@classmethod
-	def from_scene(cls, name: str = 'Camera') -> 'Camera':
-		"""Create from a named camera in scene
 
-		:param name: Name of camera"""
-		assert name in bpy.data.objects, f'Camera {name} does not exist'
-		return cls(bpy.data.objects[name])
+	@property
+	def scale(self):
+		return self.obj.scale
 
-	def update(self):
-		"""Update view layer and depsgraph"""
-		bpy.context.view_layer.update()
-		bpy.context.evaluated_depsgraph_get()
+	@scale.setter
+	def scale(self, scale):
+		self.set_scale(scale)
 
-	@property
-	def fov(self):
-		"""Field of view in degrees"""
-		return self.camera.data.angle * 180 / np.pi
 
-	@fov.setter
-	def fov(self, fov):
-		self.set_fov(fov)
+	@animatable_property('location')
+	def set_location(self, location: types.VectorLikeAlias):
+		"""Set location of object.
 
-	@animatable_property('lens', use_data_object=True)  # FOV is not animatable, so keyframe focal length instead
-	def set_fov(self, fov):
-		self.camera.data.angle = fov * np.pi / 180
-		self.update()
+		:param location: Location vector to set"""
+		location = handle_vec(location, 3)
 
-	@property
-	def location(self):
-		return self.camera.location
+		translation = location - self.location
+		with SelectObjects(self._all_objects):
+			bpy.ops.transform.translate(value=translation)
 
-	@location.setter
-	def location(self, pos):
-		self.set_location(pos)
 
-	@property
-	def rotation_euler(self):
-		return self.camera.rotation_euler
+	@animatable_property('rotation_euler')
+	def set_rotation_euler(self, rotation: types.VectorLikeAlias):
+		"""Set euler rotation of object.
 
-	@rotation_euler.setter
-	def rotation_euler(self, euler):
-		self.set_rotation_euler(euler)
+		:param rotation: Rotation vector"""
 
-	@animatable_property('location')
-	def set_location(self, pos):
-		self.camera.location = mathutils.Vector(pos)
-		self.update()
+		assert len(rotation) == 3, f"Rotation must be a tuple of length 3, got {len(rotation)}"
+		rotation = Euler(rotation, 'XYZ')
+		diff = _euler_from(self.rotation_euler, rotation)
+
+		with SelectObjects(self._all_objects):
+			for ax, val in zip('XYZ', diff):
+				if val != 0:
+					bpy.ops.transform.rotate(value=val, orient_axis=ax)
+
+	@animatable_property('scale')
+	def set_scale(self, scale: types.VectorLikeOrScalarAlias):
+		"""Set scale of object.
+
+		:param scale: Scale to set. Either single value or 3 long vector"""
+		if isinstance(scale, (int, float)):
+			scale = (scale, scale, scale)
+
+		resize_fac = np.array(scale) / np.array(self.scale)
+
+		with SelectObjects(self._all_objects):
+			bpy.ops.transform.resize(value=resize_fac)
+
+	def translate(self, translation):
+		"""Translate object"""
+		translation = handle_vec(translation, 3)
+		self.location = self.location + translation
+
+	def rotate_by(self, rotation):
+		"""Add a rotation to the object. Must be in XYZ order, euler angles, radians."""
+		rotation = handle_vec(rotation, 3)
+		new_rotation = _euler_add(self.rotation_euler, Euler(rotation, 'XYZ'))
+		self.rotation_euler = new_rotation
+
+	def scale_by(self, scale):
+		"""Scale object"""
+		if isinstance(scale, (int, float)):
+			scale = (scale, scale, scale)
 
-	@animatable_property('rotation_euler')
-	def set_rotation_euler(self, euler):
-		self.camera.rotation_euler = euler
-		self.update()
+		scale = handle_vec(scale, 3)
+		self.scale *= scale
 
 	@property
 	def matrix_world(self):
-		return self.camera.matrix_world
+		"""Return world matrix of object(s)."""
+		bpy.context.evaluated_depsgraph_get()  # required to update object matrix
+		return self.object.matrix_world
 
 	@property
-	def data(self):
-		return self.camera.data
+	def axes(self) -> np.ndarray:
+		"""Return 3x3 rotation matrix (normalized) to represent axes"""
+		mat = np.array(self.matrix_world)[:3, :3]
+		mat = mat / np.linalg.norm(mat, axis=0)
+		return mat
+
+	def track_to(self, obj: Union['BsynObject', bpy.types.Object]):
+		"""Track to object.
 
-	def look_at(self, at=mathutils.Vector((0, 0, 0)), up=mathutils.Vector((0, 1, 0))):
-		self.euler = look_at_rotation(self.camera, at, up)
+		:param obj: BsynObject or Blender Object to track to
+		"""
 
-	def place_and_rotate(self, pos, euler):
-		self.location = pos
-		self.euler = euler
-
-	def place_and_look_at(self, pos, at, up=mathutils.Vector((0, 1, 0))):
-		pos = handle_vec(pos)
-		at = handle_vec(at)
-		up = handle_vec(up)
-
-		self.location = pos
-		self.look_at(at, up)
-
-	def track_to(self, obj: Union[Mesh, bpy.types.Object]):
-		"""Track camera to object"""
-		if isinstance(obj, Mesh):
+		if isinstance(obj, BsynObject):
 			obj = obj.obj
 
-		constraint = self.camera.constraints.new('TRACK_TO')
+		constraint = self.object.constraints.new('TRACK_TO')
 		constraint.target = obj
 		constraint.track_axis = 'TRACK_NEGATIVE_Z'
 		constraint.up_axis = 'UP_Y'
-		self.update()
 
 	def untrack(self):
-		"""Remove track to constraint"""
-		constraint = self.camera.constraints.get('Track To')
-		self.camera.constraints.remove(constraint)
-		self.update()
+		"""Remove track to constraint from object"""
+		constraint = self.object.constraints.get('Track To')
+		self.object.constraints.remove(constraint)
 
-	def follow_path(self, path: Curve, zero: bool = True,
+	def follow_path(self, path: 'Curve', zero: bool = True,
 					animate: bool = True, frames: tuple = (0, 250), fracs: tuple = (0, 1)):
 		"""Follow path, with optional animation setting.
 
 		:param path: Curve object
 		:param zero: If True, set camera location to (0, 0, 0) [aligns camera with path]
 		:param animate: If True, animate camera along path
 		:param frames: tuple of keyframes to animate at - length N
 		:param fracs: tuple of fractions along path to animate at - length N
 		"""
-		constraint = self.camera.constraints.new('FOLLOW_PATH')
+
+		constraint = self.object.constraints.new('FOLLOW_PATH')
 		constraint.target = path.path
 		constraint.forward_axis = 'TRACK_NEGATIVE_Z'
 		constraint.up_axis = 'UP_Y'
 		constraint.use_fixed_location = True  # ensures that offset factor is in 0-1 range
 
 		if zero:
 			self.location = (0, 0, 0)
 
 		if animate:
 			self.animate_path(frames, fracs)
 
-		# if there is are any track constraints, place this constraint first
-		# so that the camera is not rotated by the track constraint
-		track_constraint_idx = self.camera.constraints.find('Track To')
+		# if there are any track constraints, place this constraint first
+		# so that the object is not rotated by the track constraint
+		track_constraint_idx = self.object.constraints.find('Track To')
 		if track_constraint_idx > -1:
-			self.camera.constraints.move(track_constraint_idx, track_constraint_idx + 1)
-
-		self.update()
+			self.object.constraints.move(track_constraint_idx, track_constraint_idx + 1)
 
 	def animate_path(self, frames: tuple = (0, 250), fracs: tuple = (0, 1)):
-		"""Animate camera along path.
+		"""Animate object along path.
 
 		:param frames: tuple of keyframes to animate at - length N
 		:param fracs: tuple of fractions along path to animate at - length N
 		"""
 
 		assert len(frames) == len(fracs), f"frames and fracs must be same length - got {len(frames)} and {len(fracs)}"
 
@@ -205,15 +204,13 @@
 
 	def path_keyframe(self, frame: int, offset: float):
 		"""Set keyframe for camera path offset
 
 		:param frame: Frame number
 		:param offset: Offset fraction (0-1)
 		"""
-		constraint = self.camera.constraints.get('Follow Path')
+		constraint = self.object.constraints.get('Follow Path')
 		if constraint is None:
-			raise ValueError("Camera does not have a 'Follow Path' constraint")
+			raise ValueError(f"Object `{self.__class__}` does not have a 'Follow Path' constraint")
 
 		constraint.offset_factor = offset
-		constraint.keyframe_insert(data_path='offset_factor', frame=frame)
-
-		self.update()
+		constraint.keyframe_insert(data_path='offset_factor', frame=frame)
```

### Comparing `blendersynth-0.0.4/blendersynth/blender/compositor/compositor.py` & `blendersynth-0.0.5/blendersynth/blender/compositor/compositor.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from .visuals import DepthVis
 from .image_overlay import KeypointsOverlay, BoundingBoxOverlay, AlphaImageOverlay, AxesOverlay
 
 
 from typing import Union, List
 from ...utils.node_arranger import tidy_tree
 
+from ..world import world
+
 # Mapping of file formats to extensions
 format_to_extension = {
 	'BMP': '.bmp',
 	'IRIS': '.rgb',
 	'PNG': '.png',
 	'JPEG': '.jpg',
 	'JPEG2000': '.jp2',
@@ -52,58 +54,80 @@
 def remove_ext(fname):
 	return os.path.splitext(fname)[0]  # remove extension if given
 
 
 class Compositor:
 	"""Compositor output - for handling file outputs, and managing Compositor node tree"""
 
-	def __init__(self, view_layer='ViewLayer'):
+	def __init__(self, view_layer='ViewLayer', background_color:tuple=None,
+				 rgb_color_space:str='Filmic sRGB'):
+		"""
+		:param view_layer: Name of View Layer to render
+		:param background_color: If given, RGB[A] tuple in range [0-1], will overwrite World background with solid color (while retaining lighting effects).
+		:param rgb_color_space: Color transform for RGB only.
+		"""
 		# Create compositor node tree
 		bpy.context.scene.use_nodes = True
 		self.node_tree = bpy.context.scene.node_tree
 		# self.file_output_nodes = []
 
 		self.view_layer = view_layer#
 
 		self.file_output_nodes = {}  # Mapping of output name to FileOutputNode
 		self.mask_nodes = {}  # Mapping of mask pass index to CompositorNodeGroup
 		self.overlays = {}
 		self.aovs = []  # List of AOVs (used to update before rendering)
 
+		# We set view transform to 'Raw' to avoid any gamma correction to all non-Image layers
+		bpy.context.scene.view_settings.view_transform = 'Raw'
+
+		# Socket to be used as RGB input for anything. Defined separately in case of applying overlays (e.g. background colour)
+		self._rgb_socket = get_node_by_name(self.node_tree, 'Render Layers').outputs['Image']
+		self._set_rgb_color_space(rgb_color_space)
+		if background_color is not None:
+			self._set_background_color(background_color)
+
 	def tidy_tree(self):
 		"""Tidy up node tree"""
 		tidy_tree(self.node_tree)
 
 	@property
 	def render_layers_node(self):
 		return get_node_by_name(self.node_tree, 'Render Layers')
 
+	def _get_render_layer_output(self, key:str):
+		"""Get output socket from Render Layers node"""
+		if key == 'Image': # special case
+			return self._rgb_socket
+		else:
+			return self.render_layers_node.outputs[key]
+
 	def get_mask(self, index, input_rgb: Union[str, CompositorNodeGroup], anti_aliasing=False) -> CompositorNodeGroup:
 		"""Get mask node from pass index. If not found, create new mask node"""
 		bpy.context.scene.view_layers[self.view_layer].use_pass_object_index = True  # Make sure object index is enabled
 
 		if index not in self.mask_nodes:
 
 			if isinstance(input_rgb, str):
-				ip_node = self.render_layers_node.outputs[input_rgb]
+				ip_node = self._get_render_layer_output(input_rgb)
 
 			elif isinstance(input_rgb, CompositorNodeGroup):
 				ip_node = input_rgb.outputs['Image']
 
 			else:
 				raise TypeError(f"input_rgb must be str or CompositorNodeGroup, got {type(input_rgb)}")
 
 			dtype = 'Float' if isinstance(ip_node, bpy.types.NodeSocketFloat) else 'Color'
 
 			cng = MaskOverlay(f"Mask - ID: {index} - Input {input_rgb}",
 							  self.node_tree, index=index, dtype=dtype,
 							  use_antialiasing=anti_aliasing)
 
 			self.node_tree.links.new(ip_node, cng.input('Image'))
-			self.node_tree.links.new(self.render_layers_node.outputs['IndexOB'], cng.input('IndexOB'))
+			self.node_tree.links.new(self._get_render_layer_output('IndexOB'), cng.input('IndexOB'))
 			self.mask_nodes[index] = cng
 
 		self.tidy_tree()
 		return self.mask_nodes[index]
 
 	def get_bounding_box_visual(self, col=(0., 0., 255., 255.), thickness=5) -> BoundingBoxOverlay:
 		"""
@@ -111,15 +135,15 @@
 		which will render the bounding boxes of the objects
 
 		:param col: (3,) or (N, 3) Color(s) of bounding box(es) [in BGR]
 		:param thickness: (,) or (N,) Thickness(es) of bounding box(es)
 		"""
 
 		cng = BoundingBoxOverlay(f"Bounding Box Visual", self.node_tree, col=col, thickness=thickness)
-		self.node_tree.links.new(self.render_layers_node.outputs['Image'], cng.input('Image'))
+		self.node_tree.links.new(self._get_render_layer_output('Image'), cng.input('Image'))
 
 		if 'BBox' in self.overlays:
 			raise ValueError("Only allowed one BBox overlay (it can contain multiple objects).")
 
 		self.overlays['BBox'] = cng
 
 		self.tidy_tree()
@@ -134,15 +158,15 @@
 		:param size: Size of marker. Default 5
 		:param color: Color of marker, RGB or RGBA, default (0, 0, 255) (red)
 		:param thickness: Thickness of marker. Default 2
 		"""
 
 		cng = KeypointsOverlay(f"Keypoints Visual", self.node_tree, marker=marker, color=color,
 							   size=size, thickness=thickness)
-		self.node_tree.links.new(self.render_layers_node.outputs['Image'], cng.input('Image'))
+		self.node_tree.links.new(self._get_render_layer_output('Image'), cng.input('Image'))
 
 		if 'Keypoints' in self.overlays:
 			raise ValueError("Only allowed one Keypoints overlay.")
 
 		self.overlays['Keypoints'] = cng
 
 		self.tidy_tree()
@@ -154,15 +178,15 @@
 
 		:param size: Size of axes. Default 100
 		:param thickness: Thickness of axes. Default 2
 		"""
 
 		cng = AxesOverlay(f"Axes Visual", self.node_tree,
 							   size=size, thickness=thickness)
-		self.node_tree.links.new(self.render_layers_node.outputs['Image'], cng.input('Image'))
+		self.node_tree.links.new(self._get_render_layer_output('Image'), cng.input('Image'))
 
 		if 'Axes' in self.overlays:
 			raise ValueError("Only allowed one Axes overlay.")
 
 		self.overlays['Axes'] = cng
 		self.tidy_tree()
 		return cng
@@ -195,15 +219,15 @@
 		if 'Depth' not in self.render_layers_node.outputs:
 			render_depth()
 
 		# convert col to 0-1, RGBA
 		col = ([i/255 for i in col] + [1])[:4]
 
 		cng = DepthVis(self.node_tree, max_depth=max_depth, col=col)
-		self.node_tree.links.new(self.render_layers_node.outputs['Depth'], cng.input('Depth'))
+		self.node_tree.links.new(self._get_render_layer_output('Depth'), cng.input('Depth'))
 
 		self.tidy_tree()
 		return cng
 
 	def define_output(self, input_data: Union[str, CompositorNodeGroup, AOV], directory, file_name=None, mode='image',
 					  file_format='PNG', color_mode='RGBA', jpeg_quality=90,
 					  png_compression=15, color_depth='8', EXR_color_depth='32',
@@ -249,15 +273,15 @@
 		os.makedirs(directory, exist_ok=True)
 
 		# Create new 'File Output' node in compositor
 		node = self.node_tree.nodes.new('CompositorNodeOutputFile')
 		node.name = node_name
 
 		if isinstance(input_data, str):
-			self.node_tree.links.new(self.render_layers_node.outputs[input_data], node.inputs['Image'])
+			self.node_tree.links.new(self._get_render_layer_output(input_data), node.inputs['Image'])
 
 		elif isinstance(input_data, CompositorNodeGroup):  # add overlay in between
 			self.node_tree.links.new(input_data.outputs[0], node.inputs['Image'])
 
 		else:
 			raise NotImplementedError(
 				f"input_data must be either str or CompositorNodeGroup, got {type(input_data)}")
@@ -279,20 +303,31 @@
 		node.format.color_depth = color_depth if file_format != 'OPEN_EXR' else EXR_color_depth
 
 		self.file_output_nodes[name] = node
 
 		self.tidy_tree()
 		return name
 
-	def update_filename(self, key, fname):
-		"""Reassign the filename (not directory) for a given file output node"""
+	def update_filename(self, key: str, fname: str):
+		"""Reassign the filename (not directory) for a given file output node.
+
+		:param key: key of output, as given in `define_output`
+		:param fname: new filename, without extension"""
 		fname = remove_ext(fname)
 		node = self.file_output_nodes[str(key)]
 		node.file_slots[0].path = fname
 
+	def update_all_filenames(self, fname:str):
+		"""Reassign all filenames (not directories) for all file output nodes.
+
+		:param fname: new filename, without extension"""
+		fname = remove_ext(fname)
+		for node in self.file_output_nodes.values():
+			node.file_slots[0].path = fname
+
 	def update_directory(self, key, directory):
 		"""Reassign the directory for a given file output node"""
 		node = self.file_output_nodes[str(key)]
 		node.base_path = directory
 
 	def fix_namings(self):
 		"""After rendering,
@@ -343,7 +378,42 @@
 			scene.frame_start = frame_start
 			scene.frame_end = frame_end
 
 		render(animation=animation)
 
 		if not animation:
 			self.fix_namings()
+
+	def _set_rgb_color_space(self, color_space:str='Filmic sRGB'):
+		"""Color spaces are all handled manually within compositor (so that we keep
+		AOVs in raw space). So set the color space for RGB socket here."""
+
+		color_space_node = self.node_tree.nodes.new('CompositorNodeConvertColorSpace')
+		color_space_node.from_color_space = 'Linear'
+		color_space_node.to_color_space = color_space
+
+		self.node_tree.links.new(self._rgb_socket, color_space_node.inputs[0])
+		self._rgb_socket = color_space_node.outputs[0]
+
+	def _set_background_color(self, color:tuple=(0, 0, 0)):
+		"""Set a solid background color, instead of transparent.
+		Will remove the visuals of existing world background (but not the lighting effects).
+
+		:param color: RGBA color, in range [0, 1]
+		"""
+
+		world.set_transparent()
+
+		rgba = color
+		if len(rgba) == 3:
+			rgba = (*rgba, 1)
+
+		rgb_node = self.node_tree.nodes.new('CompositorNodeRGB')
+		rgb_node.outputs[0].default_value = rgba
+
+		mix_node = self.node_tree.nodes.new('CompositorNodeMixRGB')
+
+		self.node_tree.links.new(self._rgb_socket, mix_node.inputs[2])
+		self.node_tree.links.new(rgb_node.outputs[0], mix_node.inputs[1])
+
+		self.node_tree.links.new(self._get_render_layer_output('Alpha'), mix_node.inputs['Fac'])
+		self._rgb_socket = mix_node.outputs['Image']
```

### Comparing `blendersynth-0.0.4/blendersynth/blender/compositor/image_overlay.py` & `blendersynth-0.0.5/blendersynth/blender/compositor/image_overlay.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/blender/compositor/mask_overlay.py` & `blendersynth-0.0.5/blendersynth/blender/compositor/mask_overlay.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/blender/compositor/node_group.py` & `blendersynth-0.0.5/blendersynth/blender/compositor/node_group.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/blender/compositor/visuals.py` & `blendersynth-0.0.5/blendersynth/blender/compositor/visuals.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/blender/light.py` & `blendersynth-0.0.5/blendersynth/blender/light.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import copy
 
 import bpy
-from .utils import GetNewObject
-from copy import deepcopy
+from .utils import GetNewObject, animatable_property
+from .bsyn_object import BsynObject
+from ..utils import types
 
 LIGHT_TYPES = ['POINT', 'SUN', 'SPOT', 'AREA']
 
 
-class Light:
+class Light(BsynObject):
 	"""Light object, for managing lights in the scene"""
 	light_types = LIGHT_TYPES
 	"""List of available light types"""
 
 	def __init__(self, light):
-		self.obj = light
-		self.__dict__ = copy.deepcopy(light.__dict__)  # copy over attributes from light
+		self._object = light
 
 	@classmethod
 	def from_scene(cls, key):
 		"""Create object from scene key
 
 		:param key: Key of object in scene
 		:return: :class:`~blendersynth.blender.light.Light` object
 		"""
 		obj = bpy.data.objects[key]
 		return cls(obj)
 
 	@classmethod
-	def create(cls, light_type='POINT', name='Light', intensity=1.0, color=(1.0, 1.0, 1.0), location=(0, 0, 0)):
-		"""Create a new light object
+	def create(cls, light_type:str='POINT', name:str='Light', intensity:float=1.0,
+			   color:types.VectorLikeAlias=(1.0, 1.0, 1.0), location:types.VectorLikeAlias=(0, 0, 0)):
+		"""Create a new Light object
 
 		:param light_type: Type of light to create (see :attr:`~blendersynth.blender.light.Light.light_types`)
 		:param name: Name of light
 		:param intensity: Intensity of light
 		:param color: Color of light
 		:param location: Location of light
 
@@ -45,26 +46,43 @@
 		light_data.energy = intensity
 		light_data.color = color
 
 		light = bpy.data.objects.new(name=name, object_data=light_data)
 		light.location = location
 		bpy.context.collection.objects.link(light)
 
-		return light
+		return Light(light)
 
 	@property
-	def rotation_euler(self):
-		"""Rotation of light in euler XYZ angles"""
-		return self.obj.rotation_euler
-
-	@rotation_euler.setter
-	def rotation_euler(self, value):
-		self.obj.rotation_euler = value
+	def energy(self):
+		"""Energy of light source"""
+		return self.obj.data.energy
+
+	@energy.setter
+	def energy(self, value):
+		self.set_energy(value)
+
+	@animatable_property('energy', use_data_object=True)
+	def set_energy(self, value: float):
+		"""Set energy of light source
+
+		:param value: Energy of light source
+		:return:
+		"""
+		self.obj.data.energy = value
 
 	@property
-	def location(self):
-		"""Location of light"""
-		return self.obj.location
-
-	@location.setter
-	def location(self, value):
-		self.obj.location = value
+	def color(self):
+		"""Color of light source"""
+		return self.obj.data.color
+
+	@color.setter
+	def color(self, value):
+		self.set_color(value)
+
+	@animatable_property('color', use_data_object=True)
+	def set_color(self, value: types.VectorLikeAlias):
+		"""Set color of light source
+
+		:param value: RGB[A] color
+		"""
+		self.obj.data.color = value
```

### Comparing `blendersynth-0.0.4/blendersynth/blender/mesh.py` & `blendersynth-0.0.5/blendersynth/blender/mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os.path
 
 import bpy
-from .utils import GetNewObject, SelectObjects, handle_vec, SetMode
-from .bsyn_object import BsynObject, animatable_property
+from .utils import GetNewObject, SelectObjects, handle_vec, SetMode, animatable_property
+from .bsyn_object import BsynObject
+from .material import Material
 from .aov import AOV
 import numpy as np
 import mathutils
 from mathutils import Vector, Euler
 from typing import Union, List
 from copy import deepcopy
 
@@ -43,79 +44,66 @@
 			child_meshes, child_other = _get_child_meshes(child)
 			meshes += child_meshes
 			other += child_other
 
 		return meshes, other
 
 
-def _euler_from(a: mathutils.Euler, b: mathutils.Euler):
-	"""Get euler rotation from a to b"""
-	return (b.to_matrix() @ a.to_matrix().inverted()).to_euler()
-
-
-def _euler_add(a: mathutils.Euler, b: mathutils.Euler):
-	"""Compute euler rotation of a, followed by b"""
-	return (a.to_matrix() @ b.to_matrix()).to_euler()
-
 
 class Mesh(BsynObject):
 	"""A mesh object. Can be a single mesh, or a hierarchy of meshes."""
 	primitive_list = list(_primitives.keys())
 	"""List of available primitives"""
 
 	def __init__(self, obj, material=None, scene=None, class_id=None):
 		"""
 		:param obj: Receives either a single mesh, or an empty with children empty & meshes
-		:param material:
+		:param material: bpy.types.Material to assign to the mesh
 		:param scene:
 
 		If obj contains multiple meshes, they will all be assigned the same material, and must act as a single object
 		i.e. they will all be transformed together
 
 		"""
 
 		if scene is None:
 			scene = bpy.context.scene
 
 		self.scene = scene
 		self._object = obj
 		self._meshes, self._other_objects = _get_child_meshes(obj)
 
-		# Must have a material, create if not passed
-		if material is None:
-			material = bpy.data.materials.new(name='Material')
-			material.use_nodes = True
+		# Manage materials here
+		if material is not None:
+			self._material = Material.from_blender_material(material)
+		else:
+			self._material = Material('NewMaterial')
 
-			for mesh in self._meshes:
-				mesh.data.materials.append(material)
+		for mesh in self._meshes:
+			mesh.data.materials.append(self._material.object)
 
 		# INSTANCING - Define InstanceID based on number of meshes in scene
 		self._object['instance_id'] = scene.get('NUM_MESHES', 0)
 		scene['NUM_MESHES'] = scene.get('NUM_MESHES', 0) + 1  # Increment number of meshes in scene
 
 		# CLASS - Define class based on type of object (e.g. primitive)
 		# can be overriden at any point
 		self.set_class_id(class_id)
 
 		self.assigned_aovs = []
 
-		# we want to be able to manage scale, rotation and location separately from the children meshes
-		self._scale = Vector((1, 1, 1))
-		self._rotation_euler = Euler((0, 0, 0))
-		self._location = Vector((0, 0, 0))
-
 	def set_class_id(self, class_id):
 		assert isinstance(class_id, int), f"Class ID must be an integer, not {type(class_id)}"
 		assert class_id >= 0, f"Class ID must be >= 0, not {class_id}"
 
 		self._object['class_id'] = class_id
 		self.scene['MAX_CLASSES'] = max(self.scene.get('MAX_CLASSES', 0), class_id)
 
 	@classmethod
-	def from_scene(cls, key, class_id=0) -> 'Mesh':
+	def from_scene(cls, key:str, class_id:int=0) -> 'Mesh':
 		"""Create object from named object in scene.
 
 		:param key: Name of object in scene
 		:param class_id: Class ID to assign to object
 
 		:return: Mesh loaded from scene"""
 		obj = bpy.data.objects[key]
@@ -150,18 +138,24 @@
 		if scale is not None: obj.scale = scale
 		if location is not None: obj.location = location
 		if rotation_euler is not None: obj.rotation_euler = rotation_euler
 
 		return obj
 
 	@classmethod
-	def from_obj(cls, obj_loc, class_id=None,
-				 forward_axis='-Z', up_axis='Y'):
+	def from_obj(cls, obj_loc:str, class_id:int=None,
+				 forward_axis:str='-Z', up_axis:str='Y'):
 		"""Load object from .obj file.
 
+		:param obj_loc: Location of .obj file
+		:param class_id: Class ID to assign to object
+		:param forward_axis: Axis to use as forward axis
+		:param up_axis: Axis to use as up axis
+
+
 		Note: we use bpy.ops.wm.obj_import instead of bpy.ops.import_scene.obj because the latter
 		causes issues with materials & vertex ordering.
 		(Changing vertex ordering makes the use of keypoints difficult.)
 		"""
 		for axis in (forward_axis, up_axis):
 			assert axis in (
 			'X', 'Y', 'Z', '-X', '-Y', '-Z'), f"Axis `{axis}` not valid, must be one of X, Y, Z, -X, -Y, -Z"
@@ -182,36 +176,44 @@
 		if class_id is None:
 			class_id = default_ids['loaded_mesh']
 
 		obj = importer.imported_obj
 		return cls(obj, class_id=class_id)
 
 	@classmethod
-	def from_glb(cls, glb_loc, class_id=None):
-		"""Load object from .glb file"""
+	def from_glb(cls, glb_loc:str, class_id:int=None):
+		"""Load object from .glb file.
+
+		:param glb_loc: Location of .glb file
+		:param class_id: Class ID to assign to object
+		"""
 		assert os.path.isfile(glb_loc) and glb_loc.endswith(
 			('.glb', '.gtlf')), f"File `{glb_loc}` not a valid .glb file"
 
 		directory, fname = os.path.split(glb_loc)
 		importer = GetNewObject(bpy.context.scene)
 		with importer:
 			bpy.ops.import_scene.gltf(filepath=glb_loc, files=[{"name": fname}])
 
 		if class_id is None:
 			class_id = default_ids['loaded_mesh']
 
 		return cls(importer.imported_obj, class_id=class_id)
 
 	@classmethod
-	def from_gltf(cls, gltf_loc, class_id=None):
+	def from_gltf(cls, gltf_loc:str, class_id:int=None):
+		"""Alias for :meth:`~blendersynth.blender.Mesh.from_glb`"""
 		return cls.from_glb(gltf_loc, class_id=class_id)
 
 	@classmethod
-	def from_fbx(cls, fbx_loc, class_id=None):
-		"""Load object from .fbx file"""
+	def from_fbx(cls, fbx_loc:str, class_id:int=None):
+		"""Load object from .fbx file.
+
+		:param fbx_loc: Location of .fbx file
+		:param class_id: Class ID to assign to object"""
 		assert os.path.isfile(fbx_loc) and fbx_loc.endswith('.fbx'), f"File `{fbx_loc}` not a valid .fbx file"
 
 		directory, fname = os.path.split(fbx_loc)
 		importer = GetNewObject(bpy.context.scene)
 		with importer:
 			bpy.ops.import_scene.fbx(filepath=fbx_loc, files=[{"name": fname}])
 
@@ -251,28 +253,30 @@
 					vec = handle_vec(origin[i])
 					self._meshes[i].location = vec
 				except:
 					raise ValueError(
 						f"Error with setting origin. Expects a list of {len(self._meshes)} 3-long Vector. Received: {origin}")
 
 	def get_all_vertices(self, ref_frame='WORLD'):
-		verts = np.array([vert.co[:] + (1,) for mesh in self._meshes for vert in mesh.data.vertices]).T
+		if ref_frame not in {'LOCAL', 'WORLD'}:
+			raise ValueError(f"Invalid ref_frame: {ref_frame}. Must be one of ['LOCAL', 'WORLD']")
 
-		if ref_frame == 'LOCAL':
-			pass
+		verts = []
 
-		elif ref_frame == 'WORLD':
-			world_matrix = np.array(self.matrix_world)
-			verts = np.dot(world_matrix, verts)
+		for mesh in self._meshes:
+			mesh_verts = np.array([vert.co for vert in mesh.data.vertices])
 
-		else:
-			raise ValueError(f"Invalid ref_frame: {ref_frame}. Must be one of ['LOCAL', 'WORLD']")
+			if ref_frame == 'WORLD':
+				mesh_verts = np.dot(mesh.matrix_world, np.vstack((mesh_verts.T, np.ones(mesh_verts.shape[0]))))
+
+			verts.append(mesh_verts)
 
-		verts = verts[:3, :] / verts[3, :]  # convert from homogeneous coordinates
-		return verts.T
+		verts = np.concatenate(verts, axis=1)
+		verts /= verts[3]  # convert from homogeneous coordinates
+		return verts[:3].T
 
 	@property
 	def materials(self):
 		return {m for mesh in self._meshes for m in mesh.data.materials}
 
 	def assign_pass_index(self, index: int):
 		"""Assign pass index to object. This can be used when mask rendering."""
@@ -293,108 +297,14 @@
 	def set_minimum_to(self, axis='Z', pos=0):
 		"""Set minimum of object to a given position"""
 		min_pos = self.get_all_vertices('WORLD')[:, 'XYZ'.index(axis)].min()
 		trans_vec = np.zeros(3)
 		trans_vec['XYZ'.index(axis)] = pos - min_pos
 		self.translate(trans_vec)
 
-	@property
-	def matrix_world(self):
-		"""Return world matrix of object(s).
-		"""
-		bpy.context.evaluated_depsgraph_get()  # required to update object matrix
-		return self._meshes[0].matrix_world
-
-	@property
-	def axes(self) -> np.ndarray:
-		"""Return 3x3 rotation matrix (normalized) to represent axes"""
-		mat = np.array(self.matrix_world)[:3, :3]
-		mat = mat / np.linalg.norm(mat, axis=0)
-		return mat
-
-	@property
-	def location(self):
-		return self._location
-
-	@location.setter
-	def location(self, location):
-		self.set_location(location)
-
-	@property
-	def rotation_euler(self):
-		return self._rotation_euler
-
-	@rotation_euler.setter
-	def rotation_euler(self, rotation):
-		self.set_rotation_euler(rotation)
-
-	@property
-	def scale(self):
-		return self._scale
-
-	@scale.setter
-	def scale(self, scale):
-		self.set_scale(scale)
-
-	@animatable_property('location')
-	def set_location(self, location):
-		"""Set location of object"""
-		location = handle_vec(location, 3)
-
-		translation = location - self.location
-		with SelectObjects(self._meshes + self._other_objects):
-			bpy.ops.transform.translate(value=translation)
-
-		self._location = location
-
-	@animatable_property('rotation_euler')
-	def set_rotation_euler(self, rotation):
-		"""Set euler rotation of object"""
-		assert len(rotation) == 3, f"Rotation must be a tuple of length 3, got {len(rotation)}"
-		rotation = Euler(rotation, 'XYZ')
-		diff = _euler_from(self.rotation_euler, rotation)
-
-		with SelectObjects(self._meshes + self._other_objects):
-			for ax, val in zip('XYZ', diff):
-				if val != 0:
-					bpy.ops.transform.rotate(value=val, orient_axis=ax)
-
-		self._rotation_euler = rotation
-
-	@animatable_property('scale')
-	def set_scale(self, scale):
-		"""Set scale of object"""
-		if isinstance(scale, (int, float)):
-			scale = (scale, scale, scale)
-
-		resize_fac = np.array(scale) / np.array(self.scale)
-
-		with SelectObjects(self._meshes + self._other_objects):
-			bpy.ops.transform.resize(value=resize_fac)
-
-		self._scale = scale
-
-	def translate(self, translation):
-		"""Translate object"""
-		translation = handle_vec(translation, 3)
-		self.location = self.location + translation
-
-	def rotate_by(self, rotation):
-		"""Add a rotation to the object. Must be in XYZ order, euler angles, radians."""
-		rotation = handle_vec(rotation, 3)
-		new_rotation = _euler_add(self.rotation_euler, Euler(rotation, 'XYZ'))
-		self.rotation_euler = new_rotation
-
-	def scale_by(self, scale):
-		"""Scale object"""
-		if isinstance(scale, (int, float)):
-			scale = (scale, scale, scale)
-
-		scale = handle_vec(scale, 3)
-		self.scale = self._scale * scale
 
 	def delete(self, delete_materials: bool = True):
 		"""Clear mesh from scene & mesh data.
 
 		:param delete_materials: Also delete object materials from scene"""
 		mesh_names = [m.name for m in self._meshes]
 		for mesh in self._meshes:
@@ -523,30 +433,46 @@
 		armature = self.get_armature(armature_name)
 		try:
 			bone = armature.pose.bones[bone_name]
 		except KeyError:
 			raise KeyError(f"Bone `{bone_name}` not found in armature `{armature.name}`")
 		return bone
 
-	def pose_bone(self, bone_name: str, armature_name: str = None, rotation: Vector = None, location: Vector = None,
-				  frame: int = None):
+	def pose_bone(self, bone: Union[str, bpy.types.PoseBone], rotation: Vector = None, location: Vector = None,
+				  armature_name: str = None, frame: int = None):
 		"""Set the pose of a bone by giving a Euler XYZ rotation and/or location.
 
-		:param bone_name: Name of bone to pose
-		:param armature_name: Name of armature to use. If not given, will use first armature found.
+		:param bone: Name of bone to pose, or PoseBone object
 		:param rotation: Euler XYZ rotation in radians
 		:param location: Location in object space
+		:param armature_name: Name of armature to use. If not given, will use first armature found.
 		:param frame: Frame to set pose on. If given, will insert keyframe here.
 		"""
 
-		with SetMode('POSE'):
-			bone = self.get_bone(bone_name, armature_name)
-			bone.rotation_mode = 'XYZ'
-			if rotation is not None:
-				bone.rotation_euler = rotation
-				if frame is not None:
-					bone.keyframe_insert(data_path='rotation_euler', frame=frame)
-
-			if location is not None:
-				bone.location = location
-				if frame is not None:
-					bone.keyframe_insert(data_path='location', frame=frame)
+
+		with SelectObjects(self._meshes + self._other_objects):
+			armature = self.get_armature(armature_name)
+			with SetMode('POSE', object = armature):
+				if isinstance(bone, str):
+					bone = self.get_bone(bone, armature_name)
+
+				bone.rotation_mode = 'XYZ'
+				if rotation is not None:
+					bone.rotation_euler = rotation
+					if frame is not None:
+						bone.keyframe_insert(data_path='rotation_euler', frame=frame)
+
+				if location is not None:
+					bone.location = location
+					if frame is not None:
+						bone.keyframe_insert(data_path='location', frame=frame)
+
+	@property
+	def material(self):
+		return self._material
+
+	@material.setter
+	def material(self, material: Material):
+		self._material = material
+		for mesh in self._meshes:
+			mesh.data.materials.clear()
+			mesh.data.materials.append(material.object)
```

### Comparing `blendersynth-0.0.4/blendersynth/blender/render.py` & `blendersynth-0.0.5/blendersynth/blender/render.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/blender/world.py` & `blendersynth-0.0.5/blendersynth/blender/world.py`

 * *Files 23% similar despite different names*

```diff
@@ -61,41 +61,54 @@
 		# Link the nodes
 		self.hdri_link = self.node_tree.links.new(self.node_texture.outputs["Color"],
 												  self.node_background.inputs["Color"])
 		tidy_tree(self.node_tree)
 
 		self.mode = 'HDRI'
 
-	def set_color(self, color: Union[list, tuple]):
+	def set_color(self, color: Union[list, tuple], affect_scene:bool=True):
 		"""Set the world color.
 
-		:param color: RGB or RGBA color"""
+		:param color: RGB or RGBA color
+		:param affect_scene: Toggle for whether color's lighting should affect the scene (if False, functions as a solid background color)"""
 
 		self._setup_color()
 
 		assert len(color) in [3, 4], "Color must be RGB or RGBA"
 
 		if len(color) == 3:
 			color = (*color, 1.0)
 
 		self.node_background.inputs["Color"].default_value = color
+		self._lighting_from_background(affect_scene)
 
-	def set_hdri(self, pth:str):
+	def set_hdri(self, pth:str, affect_scene:bool=True, intensity:float=None):
 		"""Set the HDRI image location
 
-		:param pth: Path to the HDRI image (.hdr or .exr)"""
+		:param pth: Path to the HDRI image (.hdr or .exr)
+		:param affect_scene: Toggle for whether color's lighting should affect the scene (if False, functions as a solid background color)
+		:param intensity: [Optional] Set the intensity of the HDRI lighting"""
+
 
 		self._setup_hdri()
 		self.world_nodes['Environment Texture'].image = bpy.data.images.load(pth)
+		self._lighting_from_background(affect_scene)
+
+		if intensity:
+			self.set_intensity(intensity)
 
 	def set_intensity(self, intensity:float=1.):
 		"""Set the intensity of the color/HDRI.
 
 		:param float: The intensity value
 		"""
 		self.world_nodes["Background"].inputs[1].default_value = intensity
 
 	def set_transparent(self, transparent=True):
 		bpy.context.scene.render.film_transparent = transparent
 
+	def _lighting_from_background(self, val=True):
+		"""Change the ability for the background to influence lighting on the scene"""
+		self.world.cycles_visibility.diffuse = val
+
 
 world = World()
```

### Comparing `blendersynth-0.0.4/blendersynth/file/dataset_inputs.py` & `blendersynth-0.0.5/blendersynth/file/dataset_inputs.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import sys
 import json
 import os
 
 import logging
 
-class INPUTS:
+class Inputs:
 	"""This class is used to iterate over the JSONs passed in via `--jobs` in sys.argv."""
 	jsons = None
 	"""List of JSON files passed in via `--jobs` in sys.argv."""
 
 	def __init__(self):
 		self.jsons = sys.argv[sys.argv.index('--jobs') + 1].split(',')
 		log_loc = sys.argv[sys.argv.index('--log') + 1]
@@ -27,8 +27,14 @@
 				fname = os.path.splitext(os.path.split(j)[-1])[0]
 				yield fname, json.load(f)
 
 			# Once we get here, we've passed 'yield', so we know that JSON has been loaded & rendering has occured
 			logging.info(f"RENDERED: {n:04d}")
 
 	def __len__(self):
-		return len(self.jsons)
+		return len(self.jsons)
+
+class DebugInputs(Inputs):
+	"""Class to emulate the Inputs class, for a single JSON for testing."""
+	def __init__(self, json_loc):
+		self.jsons = [json_loc]
+
```

### Comparing `blendersynth-0.0.4/blendersynth/file/frames_to_video.py` & `blendersynth-0.0.5/blendersynth/file/frames_to_video.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/file/tempfiles.py` & `blendersynth-0.0.5/blendersynth/file/tempfiles.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/run/blender_threading.py` & `blendersynth-0.0.5/blendersynth/run/blender_threading.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/run/run.py` & `blendersynth-0.0.5/blendersynth/run/run.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/run/run_this_script.py` & `blendersynth-0.0.5/blendersynth/run/run_this_script.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/utils/blender_importer.py` & `blendersynth-0.0.5/blendersynth/utils/blender_importer.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/utils/blender_setup/blender_locator.py` & `blendersynth-0.0.5/blendersynth/utils/blender_setup/blender_locator.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.4/blendersynth/utils/blender_setup/check_blender_install.py` & `blendersynth-0.0.5/blendersynth/utils/blender_setup/check_blender_install.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,35 +9,39 @@
 		subprocess.check_call([python_executable, '-m', 'pip', 'show', module_name],
 							  stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
 		return True
 	except subprocess.CalledProcessError:
 		return False
 
 def install_module(python_executable, module_name, is_test_pypi=False,
-				   version=None, upgrade=True):
+				   version=None, upgrade=True, editable=False):
 
 	commands = [python_executable, '-m', 'pip']
 	commands += ['install']
 	if is_test_pypi:
 		commands += ['-i', 'https://test.pypi.org/simple/']
 
+	if editable:
+		commands += ['-e']
+
 	commands += [module_name + (f"=={version}" if version is not None else "")]
 	if upgrade:
 		commands += ['--upgrade']
 
 	try:
 		subprocess.check_call(commands)
 	except subprocess.CalledProcessError as e:
 		raise Exception(f"Could not install {module_name} via pip. Error: {e}")
 
 def check_blender_install(force_all=False,
 						  force_find_blender=False,
 						  force_find_blender_python=False,
 						  force_install_dependencies=False,
-						  blendersynth_from_local=False):
+						  blendersynth_from_local=False,
+						  blendersynth_editable=False):
 	"""Check if Blender is installed correctly and has all necessary packages.
 	If not, run first time setup.
 
 	On first time setup, will create a file, config.ini, in the user's config,
 	containing the necessary info.
 
 	Force: if True, will run first time setup (overwriting any existing config.ini)
@@ -63,16 +67,15 @@
 		if check_module(python_path, 'blendersynth'):
 			subprocess.check_call([python_path, '-m', 'pip', 'uninstall', '-y', 'blendersynth'])
 
 		# Install blendersynth package to blender's python
 		if blendersynth_from_local:
 			# Install from local setup.py
 			setup_py_loc = os.path.join(os.path.dirname(__file__), '..', '..', '..', 'setup.py')
-			if not os.path.isfile(setup_py_loc):
-				raise Exception(f"Could not find setup.py at {setup_py_loc}.")
-			subprocess.check_call([python_path, setup_py_loc, 'install'])
+			directory_loc = os.path.dirname(setup_py_loc)
+			install_module(python_path, directory_loc, editable=blendersynth_editable)
 
 		else:
 			# Install from pypi
 			install_module(python_path, 'blendersynth', upgrade=True)
 
 		write_to_config('DEPENDENCIES_INSTALLED', 'True')
```

### Comparing `blendersynth-0.0.4/blendersynth/utils/node_arranger.py` & `blendersynth-0.0.5/blendersynth/utils/node_arranger.py`

 * *Files identical despite different names*

