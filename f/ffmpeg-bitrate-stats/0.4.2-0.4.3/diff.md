# Comparing `tmp/ffmpeg_bitrate_stats-0.4.2.tar.gz` & `tmp/ffmpeg_bitrate_stats-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_bitrate_stats-0.4.2.tar", last modified: Tue Jul 25 11:14:46 2023, max compression
+gzip compressed data, was "ffmpeg_bitrate_stats-0.4.3.tar", last modified: Tue Jul 25 11:30:54 2023, max compression
```

## Comparing `ffmpeg_bitrate_stats-0.4.2.tar` & `ffmpeg_bitrate_stats-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:14:46.381673 ffmpeg_bitrate_stats-0.4.2/
--rw-r--r--   0 werner     (501) staff       (20)     1085 2023-02-21 07:33:13.000000 ffmpeg_bitrate_stats-0.4.2/LICENSE.md
--rw-r--r--   0 werner     (501) staff       (20)     9622 2023-07-25 11:14:46.381769 ffmpeg_bitrate_stats-0.4.2/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     8857 2023-02-21 07:32:48.000000 ffmpeg_bitrate_stats-0.4.2/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:14:46.380802 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/
--rw-r--r--   0 werner     (501) staff       (20)      163 2023-07-25 11:14:44.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     2337 2023-02-05 15:42:43.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)    14154 2023-07-25 11:12:23.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/bitrate_stats.py
--rw-r--r--   0 werner     (501) staff       (20)      890 2023-02-05 15:44:36.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/log.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2023-01-01 19:28:03.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:14:46.381410 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)     9622 2023-07-25 11:14:46.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      437 2023-07-25 11:14:46.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-25 11:14:46.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       76 2023-07-25 11:14:46.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)       21 2023-07-25 11:14:46.000000 ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      720 2023-07-25 11:14:46.382113 ffmpeg_bitrate_stats-0.4.2/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1695 2023-01-02 12:10:15.000000 ffmpeg_bitrate_stats-0.4.2/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:14:46.381553 ffmpeg_bitrate_stats-0.4.2/test/
--rwxr-xr-x   0 werner     (501) staff       (20)     1677 2023-02-05 15:44:42.000000 ffmpeg_bitrate_stats-0.4.2/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:30:54.065703 ffmpeg_bitrate_stats-0.4.3/
+-rw-r--r--   0 werner     (501) staff       (20)     1085 2023-02-21 07:33:13.000000 ffmpeg_bitrate_stats-0.4.3/LICENSE.md
+-rw-r--r--   0 werner     (501) staff       (20)     9622 2023-07-25 11:30:54.065795 ffmpeg_bitrate_stats-0.4.3/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)     8857 2023-02-21 07:32:48.000000 ffmpeg_bitrate_stats-0.4.3/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:30:54.064861 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/
+-rw-r--r--   0 werner     (501) staff       (20)      163 2023-07-25 11:30:51.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     2337 2023-02-05 15:42:43.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)    14270 2023-07-25 11:22:52.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/bitrate_stats.py
+-rw-r--r--   0 werner     (501) staff       (20)      890 2023-02-05 15:44:36.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/log.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2023-01-01 19:28:03.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:30:54.065464 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)     9622 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      437 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       76 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)       21 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      720 2023-07-25 11:30:54.066141 ffmpeg_bitrate_stats-0.4.3/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1695 2023-01-02 12:10:15.000000 ffmpeg_bitrate_stats-0.4.3/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:30:54.065584 ffmpeg_bitrate_stats-0.4.3/test/
+-rwxr-xr-x   0 werner     (501) staff       (20)     2564 2023-07-25 11:30:03.000000 ffmpeg_bitrate_stats-0.4.3/test/test.py
```

### Comparing `ffmpeg_bitrate_stats-0.4.2/LICENSE.md` & `ffmpeg_bitrate_stats-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-0.4.2/PKG-INFO` & `ffmpeg_bitrate_stats-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg_bitrate_stats
-Version: 0.4.2
+Version: 0.4.3
 Summary: Calculate bitrate statistics using FFmpeg
 Home-page: https://github.com/slhck/ffmpeg-bitrate-stats
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ffmpeg_bitrate_stats-0.4.2/README.md` & `ffmpeg_bitrate_stats-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/__main__.py` & `ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/__main__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/bitrate_stats.py` & `ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/bitrate_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,18 @@
 
         default_duration = next(
             (x["duration_time"] for x in info if "duration_time" in x.keys()), "NaN"
         )
 
         for packet_info in info:
             frame_type: Literal["I", "Non-I"] = (
-                "I" if packet_info["flags"] == "K_" else "Non-I"
+                # key frames are marked with a capital K (K_ or K__) in packet flags
+                "I"
+                if "K" in packet_info["flags"]
+                else "Non-I"
             )
 
             pts: float | Literal["NaN"] = (
                 float(packet_info["pts_time"])
                 if "pts_time" in packet_info.keys()
                 else "NaN"
             )
```

### Comparing `ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats/log.py` & `ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/log.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-0.4.2/ffmpeg_bitrate_stats.egg-info/PKG-INFO` & `ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-bitrate-stats
-Version: 0.4.2
+Version: 0.4.3
 Summary: Calculate bitrate statistics using FFmpeg
 Home-page: https://github.com/slhck/ffmpeg-bitrate-stats
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ffmpeg_bitrate_stats-0.4.2/setup.cfg` & `ffmpeg_bitrate_stats-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-0.4.2/setup.py` & `ffmpeg_bitrate_stats-0.4.3/setup.py`

 * *Files identical despite different names*

