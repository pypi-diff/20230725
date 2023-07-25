# Comparing `tmp/ffmpeg_bitrate_stats-1.0.0.tar.gz` & `tmp/ffmpeg_bitrate_stats-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_bitrate_stats-1.0.0.tar", last modified: Tue Jul 25 12:15:52 2023, max compression
+gzip compressed data, was "ffmpeg_bitrate_stats-1.0.1.tar", last modified: Tue Jul 25 12:24:07 2023, max compression
```

## Comparing `ffmpeg_bitrate_stats-1.0.0.tar` & `ffmpeg_bitrate_stats-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:15:52.042539 ffmpeg_bitrate_stats-1.0.0/
--rw-r--r--   0 werner     (501) staff       (20)     1085 2023-02-21 07:33:13.000000 ffmpeg_bitrate_stats-1.0.0/LICENSE.md
--rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:15:52.042722 ffmpeg_bitrate_stats-1.0.0/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)    13595 2023-07-25 12:14:18.000000 ffmpeg_bitrate_stats-1.0.0/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:15:52.040831 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/
--rw-r--r--   0 werner     (501) staff       (20)      163 2023-07-25 12:15:49.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     3227 2023-07-25 12:13:04.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)    15601 2023-07-25 12:14:58.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/bitrate_stats.py
--rw-r--r--   0 werner     (501) staff       (20)      890 2023-02-05 15:44:36.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/log.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2023-01-01 19:28:03.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:15:52.042095 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      480 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       76 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)       22 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/requires.txt
--rw-r--r--   0 werner     (501) staff       (20)       21 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      720 2023-07-25 12:15:52.043215 ffmpeg_bitrate_stats-1.0.0/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1749 2023-07-25 11:35:21.000000 ffmpeg_bitrate_stats-1.0.0/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:15:52.042318 ffmpeg_bitrate_stats-1.0.0/test/
--rwxr-xr-x   0 werner     (501) staff       (20)     2564 2023-07-25 11:30:03.000000 ffmpeg_bitrate_stats-1.0.0/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:24:07.470250 ffmpeg_bitrate_stats-1.0.1/
+-rw-r--r--   0 werner     (501) staff       (20)     1085 2023-02-21 07:33:13.000000 ffmpeg_bitrate_stats-1.0.1/LICENSE.md
+-rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:24:07.470371 ffmpeg_bitrate_stats-1.0.1/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)    13595 2023-07-25 12:14:18.000000 ffmpeg_bitrate_stats-1.0.1/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:24:07.469189 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/
+-rw-r--r--   0 werner     (501) staff       (20)      163 2023-07-25 12:24:05.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     3227 2023-07-25 12:13:04.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)    15852 2023-07-25 12:23:49.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/bitrate_stats.py
+-rw-r--r--   0 werner     (501) staff       (20)      890 2023-02-05 15:44:36.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/log.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2023-01-01 19:28:03.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:24:07.469997 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      480 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       76 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/requires.txt
+-rw-r--r--   0 werner     (501) staff       (20)       21 2023-07-25 12:24:07.000000 ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      720 2023-07-25 12:24:07.470797 ffmpeg_bitrate_stats-1.0.1/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1749 2023-07-25 11:35:21.000000 ffmpeg_bitrate_stats-1.0.1/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:24:07.470124 ffmpeg_bitrate_stats-1.0.1/test/
+-rwxr-xr-x   0 werner     (501) staff       (20)     2564 2023-07-25 11:30:03.000000 ffmpeg_bitrate_stats-1.0.1/test/test.py
```

### Comparing `ffmpeg_bitrate_stats-1.0.0/LICENSE.md` & `ffmpeg_bitrate_stats-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.0/PKG-INFO` & `ffmpeg_bitrate_stats-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg_bitrate_stats
-Version: 1.0.0
+Version: 1.0.1
 Summary: Calculate bitrate statistics using FFmpeg
 Home-page: https://github.com/slhck/ffmpeg-bitrate-stats
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ffmpeg_bitrate_stats-1.0.0/README.md` & `ffmpeg_bitrate_stats-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/__main__.py` & `ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/__main__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/bitrate_stats.py` & `ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/bitrate_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -479,36 +479,44 @@
 
         Args:
             width (int, optional): Width of the plot. Defaults to 80.
             height (int, optional): Height of the plot. Defaults to 30.
         """
         chunks = self._collect_chunks()
 
-        if self.aggregation == "gop":
-            x_values = [i for i in range(len(chunks))]
-        else:
-            # x values are time-based
-            x_values = [i * self.chunk_size for i in range(len(chunks))]
-        y_values = chunks
+        fig = plotille.Figure()
+        fig.width = width
+        fig.height = height
 
-        def _num_formatter(
+        def _round_decimals(
             val: Any, chars: int, delta: float, left: bool = False
         ) -> str:
             align = "<" if left else ""
             return f"{val:{align}{chars}.{self.rounding_factor}f}"
 
-        fig = plotille.Figure()
-        fig.width = width
-        fig.height = height
-        fig.set_x_limits(min_=0, max_=self.duration)
-        fig.set_y_limits(min_=0, max_=math.ceil(max(y_values)))
-        fig.register_label_formatter(float, _num_formatter)
-        fig.register_label_formatter(int, _num_formatter)
-        fig.x_label = "Time (s)"
+        # def _float_to_int(
+        #     val: Any, chars: int, delta: float, left: bool = False
+        # ) -> str:
+        #     align = "<" if left else ""
+        #     return f"{int(val):{align}{chars}}"
+
+        if self.aggregation == "gop":
+            x_values = [i for i in range(len(chunks))]
+            fig.set_x_limits(min_=0, max_=len(chunks))
+            fig.x_label = "GOP"
+        else:
+            # x values are time-based
+            x_values = [i * self.chunk_size for i in range(len(chunks))]
+            fig.set_x_limits(min_=0, max_=self.duration)
+            fig.x_label = "Time (s)"
+
+        fig.register_label_formatter(int, _round_decimals)
+        fig.register_label_formatter(float, _round_decimals)
+        fig.set_y_limits(min_=0)
         fig.y_label = "Bitrate (kbit/s)"
 
         fig.plot(
             x_values,
-            y_values,
+            chunks,
         )
 
         print(fig.show(), file=sys.stderr)
```

### Comparing `ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/log.py` & `ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats/log.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/PKG-INFO` & `ffmpeg_bitrate_stats-1.0.1/ffmpeg_bitrate_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-bitrate-stats
-Version: 1.0.0
+Version: 1.0.1
 Summary: Calculate bitrate statistics using FFmpeg
 Home-page: https://github.com/slhck/ffmpeg-bitrate-stats
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ffmpeg_bitrate_stats-1.0.0/setup.cfg` & `ffmpeg_bitrate_stats-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.0/setup.py` & `ffmpeg_bitrate_stats-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-1.0.0/test/test.py` & `ffmpeg_bitrate_stats-1.0.1/test/test.py`

 * *Files identical despite different names*

