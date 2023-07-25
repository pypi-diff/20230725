# Comparing `tmp/ffmpeg_bitrate_stats-1.0.1.tar.gz` & `tmp/ffmpeg_bitrate_stats-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_bitrate_stats-1.0.1.tar", last modified: Tue Jul 25 12:24:07 2023, max compression
+gzip compressed data, was "ffmpeg_bitrate_stats-1.0.2.tar", last modified: Tue Jul 25 12:39:38 2023, max compression
```

## Comparing `ffmpeg_bitrate_stats-1.0.1.tar` & `ffmpeg_bitrate_stats-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:24:07.470250 ffmpeg_bitrate_stats-1.0.1/
--rw-r--r--   0 werner     (501) staff       (20)     1085 2023-02-21 07:33:13.000000 ffmpeg_bitrate_stats-1.0.1/LICENSE.md
--rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:24:07.470371 ffmpeg_bitrate_stats-1.0.1/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)    13595 2023-07-25 12:14:18.000000 ffmpeg_bitrate_stats-1.0.1/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:24:07.469189 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/
--rw-r--r--   0 werner     (501) staff       (20)      163 2023-07-25 12:24:05.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     3227 2023-07-25 12:13:04.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)    15852 2023-07-25 12:23:49.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/bitrate_stats.py
--rw-r--r--   0 werner     (501) staff       (20)      890 2023-02-05 15:44:36.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/log.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2023-01-01 19:28:03.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:24:07.469997 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      480 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       76 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)       22 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/requires.txt
--rw-r--r--   0 werner     (501) staff       (20)       21 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      720 2023-07-25 12:24:07.470797 ffmpeg_bitrate_stats-1.0.1/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1749 2023-07-25 11:35:21.000000 ffmpeg_bitrate_stats-1.0.1/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:24:07.470124 ffmpeg_bitrate_stats-1.0.1/test/
--rwxr-xr-x   0 werner     (501) staff       (20)     2564 2023-07-25 11:30:03.000000 ffmpeg_bitrate_stats-1.0.1/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:39:38.146558 ffmpeg_bitrate_stats-1.0.2/
+-rw-r--r--   0 werner     (501) staff       (20)     1085 2023-02-21 07:33:13.000000 ffmpeg_bitrate_stats-1.0.2/LICENSE.md
+-rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:39:38.146687 ffmpeg_bitrate_stats-1.0.2/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)    13595 2023-07-25 12:14:18.000000 ffmpeg_bitrate_stats-1.0.2/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:39:38.145201 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/
+-rw-r--r--   0 werner     (501) staff       (20)      163 2023-07-25 12:39:35.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     3227 2023-07-25 12:13:04.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)    15727 2023-07-25 12:38:35.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/bitrate_stats.py
+-rw-r--r--   0 werner     (501) staff       (20)      890 2023-02-05 15:44:36.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/log.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2023-01-01 19:28:03.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:39:38.146309 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:39:38.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      480 2023-07-25 12:39:38.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-25 12:39:38.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       76 2023-07-25 12:39:38.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-07-25 12:39:38.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats.egg-info/requires.txt
+-rw-r--r--   0 werner     (501) staff       (20)       21 2023-07-25 12:39:38.000000 ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      720 2023-07-25 12:39:38.147116 ffmpeg_bitrate_stats-1.0.2/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1749 2023-07-25 11:35:21.000000 ffmpeg_bitrate_stats-1.0.2/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:39:38.146432 ffmpeg_bitrate_stats-1.0.2/test/
+-rwxr-xr-x   0 werner     (501) staff       (20)     2564 2023-07-25 11:30:03.000000 ffmpeg_bitrate_stats-1.0.2/test/test.py
```

### Comparing `ffmpeg_bitrate_stats-1.0.1/LICENSE.md` & `ffmpeg_bitrate_stats-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.1/PKG-INFO` & `ffmpeg_bitrate_stats-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg_bitrate_stats
-Version: 1.0.1
+Version: 1.0.2
 Summary: Calculate bitrate statistics using FFmpeg
 Home-page: https://github.com/slhck/ffmpeg-bitrate-stats
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ffmpeg_bitrate_stats-1.0.1/README.md` & `ffmpeg_bitrate_stats-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/__main__.py` & `ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/__main__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/bitrate_stats.py` & `ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/bitrate_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import json
 import logging
 import math
 import subprocess
 import sys
-from typing import Any, List, Literal, TypedDict, cast
+from typing import Any, List, Literal, Optional, TypedDict, cast
 
 import numpy as np
 import pandas as pd
 import plotille
 
 logger = logging.getLogger("ffmpeg-bitrate-stats")
 
@@ -89,15 +89,15 @@
     """
     The bitrate per chunk in kbit/s.
     """
     aggregation: Aggregation
     """
     The aggregation type (time/chunks).
     """
-    chunk_size: int
+    chunk_size: Optional[int]
     """
     The chunk size in seconds.
     """
     duration: float
     """
     The duration in seconds.
     """
@@ -147,14 +147,15 @@
         self.min_bitrate: float = 0
         self.moving_avg_bitrate: list[float] = []
         self.frames: list[FrameEntry] = []
         self.bitrate_stats: BitrateStatsSummary | None = None
 
         self.rounding_factor: int = 3
 
+        self._gop_start_times: Optional[list[float]] = None
         self._chunks: list[float] = []
 
     def calculate_statistics(self) -> BitrateStatsSummary:
         """
         Calculate the bitrate statistics.
 
         Raises:
@@ -308,23 +309,26 @@
 
         logger.debug("Collecting chunks for bitrate calculation")
 
         # this is where we will store the stats in buckets
         aggregation_chunks: list[list[FrameEntry]] = []
         curr_list: list[FrameEntry] = []
 
+        self._gop_start_times = []
+
         if self.aggregation == "gop":
             # collect group of pictures, each one containing all frames belonging to it
             for frame in self.frames:
                 if frame["frame_type"] != "I":
                     curr_list.append(frame)
                 if frame["frame_type"] == "I":
                     if curr_list:
                         aggregation_chunks.append(curr_list)
                     curr_list = [frame]
+                    self._gop_start_times.append(float(frame["pts"]))
             # flush the last one
             aggregation_chunks.append(curr_list)
 
         else:
             # per-time aggregation
             agg_time: float = 0
             for frame in self.frames:
@@ -409,15 +413,15 @@
             "max_bitrate": round(self.max_bitrate, self.rounding_factor),
             "min_bitrate": round(self.min_bitrate, self.rounding_factor),
             "max_bitrate_factor": round(self.max_bitrate_factor, self.rounding_factor),
             "bitrate_per_chunk": [
                 round(b, self.rounding_factor) for b in self._collect_chunks()
             ],
             "aggregation": self.aggregation,
-            "chunk_size": self.chunk_size,
+            "chunk_size": self.chunk_size if self.aggregation == "time" else None,
             "duration": round(self.duration, self.rounding_factor),
         }
 
         self.bitrate_stats = ret
         return self.bitrate_stats
 
     def print_statistics(self, output_format: Literal["csv", "json"]) -> None:
@@ -489,33 +493,25 @@
 
         def _round_decimals(
             val: Any, chars: int, delta: float, left: bool = False
         ) -> str:
             align = "<" if left else ""
             return f"{val:{align}{chars}.{self.rounding_factor}f}"
 
-        # def _float_to_int(
-        #     val: Any, chars: int, delta: float, left: bool = False
-        # ) -> str:
-        #     align = "<" if left else ""
-        #     return f"{int(val):{align}{chars}}"
-
-        if self.aggregation == "gop":
-            x_values = [i for i in range(len(chunks))]
-            fig.set_x_limits(min_=0, max_=len(chunks))
-            fig.x_label = "GOP"
-        else:
-            # x values are time-based
-            x_values = [i * self.chunk_size for i in range(len(chunks))]
-            fig.set_x_limits(min_=0, max_=self.duration)
-            fig.x_label = "Time (s)"
+        x_values = (
+            self._gop_start_times
+            if self.aggregation == "gop"
+            else [i * self.chunk_size for i in range(len(chunks))]
+        )
 
         fig.register_label_formatter(int, _round_decimals)
         fig.register_label_formatter(float, _round_decimals)
+        fig.set_x_limits(min_=0, max_=self.duration)
         fig.set_y_limits(min_=0)
+        fig.x_label = "Time (s)"
         fig.y_label = "Bitrate (kbit/s)"
 
         fig.plot(
             x_values,
             chunks,
         )
```

### Comparing `ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/log.py` & `ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats/log.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/PKG-INFO` & `ffmpeg_bitrate_stats-1.0.2/ffmpeg_bitrate_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-bitrate-stats
-Version: 1.0.1
+Version: 1.0.2
 Summary: Calculate bitrate statistics using FFmpeg
 Home-page: https://github.com/slhck/ffmpeg-bitrate-stats
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ffmpeg_bitrate_stats-1.0.1/setup.cfg` & `ffmpeg_bitrate_stats-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.1/setup.py` & `ffmpeg_bitrate_stats-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.1/test/test.py` & `ffmpeg_bitrate_stats-1.0.2/test/test.py`

 * *Files identical despite different names*

