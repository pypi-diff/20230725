# Comparing `tmp/ffmpeg_bitrate_stats-0.4.3.tar.gz` & `tmp/ffmpeg_bitrate_stats-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_bitrate_stats-0.4.3.tar", last modified: Tue Jul 25 11:30:54 2023, max compression
+gzip compressed data, was "ffmpeg_bitrate_stats-1.0.0.tar", last modified: Tue Jul 25 12:15:52 2023, max compression
```

## Comparing `ffmpeg_bitrate_stats-0.4.3.tar` & `ffmpeg_bitrate_stats-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:30:54.065703 ffmpeg_bitrate_stats-0.4.3/
--rw-r--r--   0 werner     (501) staff       (20)     1085 2023-02-21 07:33:13.000000 ffmpeg_bitrate_stats-0.4.3/LICENSE.md
--rw-r--r--   0 werner     (501) staff       (20)     9622 2023-07-25 11:30:54.065795 ffmpeg_bitrate_stats-0.4.3/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     8857 2023-02-21 07:32:48.000000 ffmpeg_bitrate_stats-0.4.3/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:30:54.064861 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/
--rw-r--r--   0 werner     (501) staff       (20)      163 2023-07-25 11:30:51.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     2337 2023-02-05 15:42:43.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)    14270 2023-07-25 11:22:52.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/bitrate_stats.py
--rw-r--r--   0 werner     (501) staff       (20)      890 2023-02-05 15:44:36.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/log.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2023-01-01 19:28:03.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:30:54.065464 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)     9622 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      437 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       76 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)       21 2023-07-25 11:30:54.000000 ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      720 2023-07-25 11:30:54.066141 ffmpeg_bitrate_stats-0.4.3/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1695 2023-01-02 12:10:15.000000 ffmpeg_bitrate_stats-0.4.3/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 11:30:54.065584 ffmpeg_bitrate_stats-0.4.3/test/
--rwxr-xr-x   0 werner     (501) staff       (20)     2564 2023-07-25 11:30:03.000000 ffmpeg_bitrate_stats-0.4.3/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:15:52.042539 ffmpeg_bitrate_stats-1.0.0/
+-rw-r--r--   0 werner     (501) staff       (20)     1085 2023-02-21 07:33:13.000000 ffmpeg_bitrate_stats-1.0.0/LICENSE.md
+-rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:15:52.042722 ffmpeg_bitrate_stats-1.0.0/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)    13595 2023-07-25 12:14:18.000000 ffmpeg_bitrate_stats-1.0.0/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:15:52.040831 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/
+-rw-r--r--   0 werner     (501) staff       (20)      163 2023-07-25 12:15:49.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     3227 2023-07-25 12:13:04.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)    15601 2023-07-25 12:14:58.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/bitrate_stats.py
+-rw-r--r--   0 werner     (501) staff       (20)      890 2023-02-05 15:44:36.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/log.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2023-01-01 19:28:03.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:15:52.042095 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    14360 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      480 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       76 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/requires.txt
+-rw-r--r--   0 werner     (501) staff       (20)       21 2023-07-25 12:15:52.000000 ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      720 2023-07-25 12:15:52.043215 ffmpeg_bitrate_stats-1.0.0/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1749 2023-07-25 11:35:21.000000 ffmpeg_bitrate_stats-1.0.0/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-25 12:15:52.042318 ffmpeg_bitrate_stats-1.0.0/test/
+-rwxr-xr-x   0 werner     (501) staff       (20)     2564 2023-07-25 11:30:03.000000 ffmpeg_bitrate_stats-1.0.0/test/test.py
```

### Comparing `ffmpeg_bitrate_stats-0.4.3/LICENSE.md` & `ffmpeg_bitrate_stats-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/__main__.py` & `ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,23 +5,33 @@
 # Output is in kilobit per second unless specified otherwise.
 #
 # Author: Werner Robitza
 # License: MIT
 
 import argparse
 import logging
+import os
 import sys
+from typing import Tuple
 
 from .__init__ import __version__ as version
 from .bitrate_stats import BitrateStats
 from .log import CustomLogFormatter
 
 logger = logging.getLogger("ffmpeg-bitrate-stats")
 
 
+def get_terminal_size() -> Tuple[int, int]:
+    try:
+        term_size = os.get_terminal_size()
+        return (term_size.columns, term_size.lines)
+    except OSError:
+        return (80, 24)
+
+
 def setup_logger(level: int = logging.INFO) -> logging.Logger:
     logger = logging.getLogger("ffmpeg-bitrate-stats")
     logger.setLevel(level)
 
     ch = logging.StreamHandler(sys.stderr)
     ch.setLevel(level)
 
@@ -79,24 +89,52 @@
         "--output-format",
         type=str,
         default="json",
         choices=["json", "csv"],
         help="output in which format",
     )
 
+    parser.add_argument(
+        "-p",
+        "--plot",
+        action="store_true",
+        help="Plot the bitrate over time (to STDERR)",
+    )
+
+    parser.add_argument(
+        "-pw",
+        "--plot-width",
+        type=int,
+        default=max(get_terminal_size()[0] - 10, 10),
+        help="Plot width",
+    )
+    parser.add_argument(
+        "-ph",
+        "--plot-height",
+        type=int,
+        default=max(get_terminal_size()[1] - 6, 10),
+        help="Plot height",
+    )
+
     cli_args = parser.parse_args()
 
     setup_logger(logging.DEBUG if cli_args.verbose else logging.INFO)
 
     br = BitrateStats(
         cli_args.input,
-        cli_args.stream_type,
-        cli_args.aggregation,
-        cli_args.chunk_size,
-        cli_args.dry_run,
+        stream_type=cli_args.stream_type,
+        aggregation=cli_args.aggregation,
+        chunk_size=cli_args.chunk_size,
+        dry_run=cli_args.dry_run,
     )
     br.calculate_statistics()
     br.print_statistics(cli_args.output_format)
 
+    if cli_args.plot:
+        br.plot(
+            width=cli_args.plot_width,
+            height=cli_args.plot_height,
+        )
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/bitrate_stats.py` & `ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/bitrate_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import json
 import logging
 import math
 import subprocess
 import sys
-from typing import List, Literal, TypedDict, cast
+from typing import Any, List, Literal, TypedDict, cast
 
 import numpy as np
 import pandas as pd
+import plotille
 
 logger = logging.getLogger("ffmpeg-bitrate-stats")
 
 
 def run_command(
     cmd: List[str], dry_run: bool = False, verbose: bool = False
 ) -> tuple[str, str] | tuple[None, None]:
@@ -467,7 +468,47 @@
         Returns:
             str: The bitrate statistics as a JSON string
         """
         if not self.bitrate_stats:
             raise RuntimeError("No bitrate stats available")
 
         return json.dumps(self.bitrate_stats, indent=4)
+
+    def plot(self, width: int = 80, height: int = 30) -> None:
+        """
+        Plot the bitrate over time to STDERR.
+
+        Args:
+            width (int, optional): Width of the plot. Defaults to 80.
+            height (int, optional): Height of the plot. Defaults to 30.
+        """
+        chunks = self._collect_chunks()
+
+        if self.aggregation == "gop":
+            x_values = [i for i in range(len(chunks))]
+        else:
+            # x values are time-based
+            x_values = [i * self.chunk_size for i in range(len(chunks))]
+        y_values = chunks
+
+        def _num_formatter(
+            val: Any, chars: int, delta: float, left: bool = False
+        ) -> str:
+            align = "<" if left else ""
+            return f"{val:{align}{chars}.{self.rounding_factor}f}"
+
+        fig = plotille.Figure()
+        fig.width = width
+        fig.height = height
+        fig.set_x_limits(min_=0, max_=self.duration)
+        fig.set_y_limits(min_=0, max_=math.ceil(max(y_values)))
+        fig.register_label_formatter(float, _num_formatter)
+        fig.register_label_formatter(int, _num_formatter)
+        fig.x_label = "Time (s)"
+        fig.y_label = "Bitrate (kbit/s)"
+
+        fig.plot(
+            x_values,
+            y_values,
+        )
+
+        print(fig.show(), file=sys.stderr)
```

### Comparing `ffmpeg_bitrate_stats-0.4.3/ffmpeg_bitrate_stats/log.py` & `ffmpeg_bitrate_stats-1.0.0/ffmpeg_bitrate_stats/log.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-0.4.3/setup.cfg` & `ffmpeg_bitrate_stats-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ffmpeg_bitrate_stats-0.4.3/setup.py` & `ffmpeg_bitrate_stats-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.8",
     packages=["ffmpeg_bitrate_stats"],
+    install_requires=["numpy", "pandas", "plotille"],
     include_package_data=True,
     package_data={
         "ffmpeg_bitrate_stats": ["py.typed"],
     },
     entry_points={
         "console_scripts": [
             "ffmpeg-bitrate-stats=ffmpeg_bitrate_stats.__main__:main",
```

### Comparing `ffmpeg_bitrate_stats-0.4.3/test/test.py` & `ffmpeg_bitrate_stats-1.0.0/test/test.py`

 * *Files identical despite different names*

