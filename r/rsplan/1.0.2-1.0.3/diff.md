# Comparing `tmp/rsplan-1.0.2.tar.gz` & `tmp/rsplan-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsplan-1.0.2.tar", last modified: Mon Jul 24 00:07:22 2023, max compression
+gzip compressed data, was "rsplan-1.0.3.tar", last modified: Tue Jul 25 02:12:57 2023, max compression
```

## Comparing `rsplan-1.0.2.tar` & `rsplan-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-24 00:07:22.968987 rsplan-1.0.2/
--rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.2/LICENSE
--rw-rw-r--   0 built     (1000) built     (1000)     5412 2023-07-24 00:07:22.968987 rsplan-1.0.2/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)     3755 2023-07-21 21:43:28.000000 rsplan-1.0.2/README.md
--rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-24 00:07:13.000000 rsplan-1.0.2/pyproject.toml
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-24 00:07:22.968987 rsplan-1.0.2/rsplan/
--rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-19 03:21:47.000000 rsplan-1.0.2/rsplan/__init__.py
--rw-rw-r--   0 built     (1000) built     (1000)    28383 2023-07-23 20:09:00.000000 rsplan-1.0.2/rsplan/curves.py
--rw-rw-r--   0 built     (1000) built     (1000)     2614 2023-07-23 20:09:06.000000 rsplan-1.0.2/rsplan/demo.py
--rw-rw-r--   0 built     (1000) built     (1000)     3082 2023-07-19 19:07:31.000000 rsplan-1.0.2/rsplan/helpers.py
--rw-rw-r--   0 built     (1000) built     (1000)     6527 2023-07-23 20:08:41.000000 rsplan-1.0.2/rsplan/planner.py
--rw-rw-r--   0 built     (1000) built     (1000)    11989 2023-07-24 00:04:40.000000 rsplan-1.0.2/rsplan/primitives.py
--rw-rw-r--   0 built     (1000) built     (1000)     5109 2023-07-23 20:08:55.000000 rsplan-1.0.2/rsplan/unit_tests.py
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-24 00:07:22.968987 rsplan-1.0.2/rsplan.egg-info/
--rw-rw-r--   0 built     (1000) built     (1000)     5412 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)      319 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/SOURCES.txt
--rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/dependency_links.txt
--rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/requires.txt
--rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/top_level.txt
--rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-24 00:07:22.968987 rsplan-1.0.2/setup.cfg
--rw-rw-r--   0 built     (1000) built     (1000)      643 2023-07-24 00:07:00.000000 rsplan-1.0.2/setup.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 02:12:57.762412 rsplan-1.0.3/
+-rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.3/LICENSE
+-rw-rw-r--   0 built     (1000) built     (1000)     5490 2023-07-25 02:12:57.762412 rsplan-1.0.3/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)     3833 2023-07-25 02:06:53.000000 rsplan-1.0.3/README.md
+-rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-25 02:12:06.000000 rsplan-1.0.3/pyproject.toml
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 02:12:57.762412 rsplan-1.0.3/rsplan/
+-rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-19 03:21:47.000000 rsplan-1.0.3/rsplan/__init__.py
+-rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-24 00:19:10.000000 rsplan-1.0.3/rsplan/curves.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2582 2023-07-25 01:59:29.000000 rsplan-1.0.3/rsplan/demo.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.3/rsplan/helpers.py
+-rw-rw-r--   0 built     (1000) built     (1000)     6505 2023-07-25 02:01:50.000000 rsplan-1.0.3/rsplan/planner.py
+-rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-07-25 01:56:11.000000 rsplan-1.0.3/rsplan/primitives.py
+-rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.3/rsplan/unit_tests.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 02:12:57.762412 rsplan-1.0.3/rsplan.egg-info/
+-rw-rw-r--   0 built     (1000) built     (1000)     5490 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)      319 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/SOURCES.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/dependency_links.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/requires.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/top_level.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-25 02:12:57.762412 rsplan-1.0.3/setup.cfg
+-rw-rw-r--   0 built     (1000) built     (1000)      643 2023-07-25 02:12:08.000000 rsplan-1.0.3/setup.py
```

### Comparing `rsplan-1.0.2/LICENSE` & `rsplan-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.2/PKG-INFO` & `rsplan-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.2
+Version: 1.0.3
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
@@ -31,41 +31,43 @@
   - [Running](#running)
   - [Demo](#demo)
 - [FAQ](#faq)
 - [Exhibits](#exhibits)
 - [References](#references)
 
 ## Overview
-This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions including 3.11.
+This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions >= 3.9, including 3.11.
 
 Contains the following files:
   - `planner`: Path planning code. `path` function outputs the optimal Reeds-Shepp path with or without a runway.
   - `curves`: Curve formulas for all of the curve types in the Reeds-Shepp paper.
-  - `primitives`: Three class architectures (path, waypoint, and segment).
-    - Waypoint class (stores x, y, yaw, as well as the curvature and angle/length of the segment the waypoint is on)
-    - Segment class (stores left/right/straight type, forward/backward direction, magnitude (arc angle or straight length), and turn radius of the segment)
+  - `primitives`: Three class architectures (Waypoint, Segment, and Path).
+    - Waypoint class (stores x, y, yaw of the waypoint and the curvature and length of the segment the waypoint is on as well as if the segment is a runway)
+    - Segment class (stores left/right/straight type, forward/backward direction, length, and turn radius of the segment)
     - Path class (stores start and end points, turn radius, step size, and list of Segments. Also contains a cached waypoints function to get a list of Waypoints for the path)
   - `helpers`: Helper functions for planner, primitives, and curves files.
   - `demo`: Demo/visualization of paths.
 
 
 
 ## Usage
 
-### Running
+### Installation
+You can install this software using pip:
+
+`pip install -U rsplan`
 
-See demo.py for example usage
 
-path(start_pt, end_pt, turn_radius, runway_length, step_size, length_tolerance (optional))
-- return a Reeds-Shepp path from start_pt to end_pt with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
-- start_pt and end_pt are in the format `Tuple[float, float, float]` of x, y, yaw values.
+### Running
 
-### Demo
+See demo.py for example usage
 
-$ python demos/demo.py
+path(start_pose, end_pose, turn_radius, runway_length, step_size, length_tolerance (optional))
+- return a Reeds-Shepp path from start_pose to end_pose with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
+- start_pose and end_pose are in the format `Tuple[float, float, float]` of x, y, yaw values.
 
 
 ## FAQ
 
 What are t, u, and v parameters?
 - As a whole, t, u, v are segment parameters generated in each of the curve helper functions that represent the distance (angular distance for curved segments, linear distance for straight segments) of their respective segments.
 - If there are 3 segments (ccc or csc), t is for segment 1, u is for segment 2, and v is for segment 3.
@@ -78,14 +80,15 @@
 
 
 ### Exhibits
 
 From demo.py:
 
 Paths start from origin
+
 Format: (end x, end y, yaw, turn radius, runway length)
 1. (5, 6, np.pi, 1, 0)
 2. (15, 3, np.pi / 2.0, 2, 6)
 3. (-2, -4, np.pi, 4, 3)
 4. (-7, 2, np.pi, 4, 0)
 5. (-7, -7, 0.0, 6, 1)
 6. (0.7, 1.8, 1, 1, 1)
```

### Comparing `rsplan-1.0.2/README.md` & `rsplan-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,41 +6,43 @@
   - [Running](#running)
   - [Demo](#demo)
 - [FAQ](#faq)
 - [Exhibits](#exhibits)
 - [References](#references)
 
 ## Overview
-This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions including 3.11.
+This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions >= 3.9, including 3.11.
 
 Contains the following files:
   - `planner`: Path planning code. `path` function outputs the optimal Reeds-Shepp path with or without a runway.
   - `curves`: Curve formulas for all of the curve types in the Reeds-Shepp paper.
-  - `primitives`: Three class architectures (path, waypoint, and segment).
-    - Waypoint class (stores x, y, yaw, as well as the curvature and angle/length of the segment the waypoint is on)
-    - Segment class (stores left/right/straight type, forward/backward direction, magnitude (arc angle or straight length), and turn radius of the segment)
+  - `primitives`: Three class architectures (Waypoint, Segment, and Path).
+    - Waypoint class (stores x, y, yaw of the waypoint and the curvature and length of the segment the waypoint is on as well as if the segment is a runway)
+    - Segment class (stores left/right/straight type, forward/backward direction, length, and turn radius of the segment)
     - Path class (stores start and end points, turn radius, step size, and list of Segments. Also contains a cached waypoints function to get a list of Waypoints for the path)
   - `helpers`: Helper functions for planner, primitives, and curves files.
   - `demo`: Demo/visualization of paths.
 
 
 
 ## Usage
 
-### Running
+### Installation
+You can install this software using pip:
+
+`pip install -U rsplan`
 
-See demo.py for example usage
 
-path(start_pt, end_pt, turn_radius, runway_length, step_size, length_tolerance (optional))
-- return a Reeds-Shepp path from start_pt to end_pt with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
-- start_pt and end_pt are in the format `Tuple[float, float, float]` of x, y, yaw values.
+### Running
 
-### Demo
+See demo.py for example usage
 
-$ python demos/demo.py
+path(start_pose, end_pose, turn_radius, runway_length, step_size, length_tolerance (optional))
+- return a Reeds-Shepp path from start_pose to end_pose with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
+- start_pose and end_pose are in the format `Tuple[float, float, float]` of x, y, yaw values.
 
 
 ## FAQ
 
 What are t, u, and v parameters?
 - As a whole, t, u, v are segment parameters generated in each of the curve helper functions that represent the distance (angular distance for curved segments, linear distance for straight segments) of their respective segments.
 - If there are 3 segments (ccc or csc), t is for segment 1, u is for segment 2, and v is for segment 3.
@@ -53,14 +55,15 @@
 
 
 ### Exhibits
 
 From demo.py:
 
 Paths start from origin
+
 Format: (end x, end y, yaw, turn radius, runway length)
 1. (5, 6, np.pi, 1, 0)
 2. (15, 3, np.pi / 2.0, 2, 6)
 3. (-2, -4, np.pi, 4, 3)
 4. (-7, 2, np.pi, 4, 0)
 5. (-7, -7, 0.0, 6, 1)
 6. (0.7, 1.8, 1, 1, 1)
```

### Comparing `rsplan-1.0.2/pyproject.toml` & `rsplan-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsplan"
-version = "1.0.2"
+version = "1.0.3"
 description = "Reeds-Shepp algorithm implementation in Python"
 readme = "README.md"
 authors = [{ name = "Built Robotics", email = "tarakapoor9@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rsplan-1.0.2/rsplan/curves.py` & `rsplan-1.0.3/rsplan/curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,16 +451,16 @@
     Path.
     """
     path_segments = []
     for segment_param, segment_type in zip(segment_params, path_segment_types):
         path_segments.append(_create_segment(segment_param, segment_type, turn_radius))
 
     return primitives.Path(
-        start_pt=start,
-        end_pt=end,
+        start_pose=start,
+        end_pose=end,
         segments=path_segments,
         turn_radius=turn_radius,
         step_size=step_size,
     )
 
 
 def _create_segment(
```

### Comparing `rsplan-1.0.2/rsplan/demo.py` & `rsplan-1.0.3/rsplan/demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Tuple
 
 import matplotlib.pyplot as plt  # type: ignore[import]
 import numpy as np
 
 from rsplan import planner, primitives
 
-# List of path endpoints to visualize Reeds-Shepp paths for with matplotlib.
+# List of path end poses to visualize Reeds-Shepp paths for with matplotlib.
 # Format: (end x, end y, end yaw, turn radius, runway length)
 _END_POSES: List[Tuple[float, float, float, int, float]] = [
     (5, 6, np.pi, 1, 0),
     (15, 3, np.pi / 2.0, 2, 6),
     (-2, -4, np.pi, 4, 3),
     (-7, 2, np.pi, 4, 0),
     (-7, -7, 0.0, 6, 1),
@@ -75,17 +75,15 @@
     start = (0.0, 0.0, 0.0)
 
     for i in range(len(_END_POSES)):
         end_coords = _END_POSES[i]
         x, y, yaw, turn_radius, runway_length = end_coords
         step_size = 0.05
 
-        _plot_arrow(
-            *start
-        )  # Start of path arrow (same for all paths starting at origin)
+        _plot_arrow(*start)  # Start arrow same for all paths starting at origin
 
         # Passing in yaw angles in radians
         rs_path = planner.path(
             start, (x, y, yaw), turn_radius, runway_length, step_size
         )
         _viz_path(rs_path, i + 1)
         _plot_arrow(x, y, yaw)  # End of path arrow to show direction
```

### Comparing `rsplan-1.0.2/rsplan/helpers.py` & `rsplan-1.0.3/rsplan/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 
 ########################################################################################
 # GENERAL HELPER FUNCTIONS #############################################################
 ########################################################################################
 
 
 def change_base(
-    new_base: Tuple[float, float, float], end_pose2d: Tuple[float, float, float]
+    start_pose: Tuple[float, float, float], end_pose: Tuple[float, float, float]
 ) -> Tuple[float, float, float]:
-    """Given new_base = (x1, y1, theta1) and end_pose2d = (x2, y2, theta2) represented
+    """Given start_pose = (x1, y1, theta1) and end_pose = (x2, y2, theta2) represented
     in a coordinate system with origin (0, 0) and rotation 0 (in radians), return the
-    position and rotation of end_pose2d in the coordinate system with origin (x1, y1)
+    position and rotation of end_pose in the coordinate system with origin (x1, y1)
     and rotation theta1.
     """
-    dx = end_pose2d[0] - new_base[0]
-    dy = end_pose2d[1] - new_base[1]
-    xb, yb = rotate(dx, dy, -new_base[2])
+    dx = end_pose[0] - start_pose[0]
+    dy = end_pose[1] - start_pose[1]
+    xb, yb = rotate(dx, dy, -start_pose[2])
 
-    dtheta = end_pose2d[2] - new_base[2]
+    dtheta = end_pose[2] - start_pose[2]
 
     return xb, yb, dtheta
 
-    return *(helpers.rotate(end[0] - start[0], end[1] - start[1], -start[2])), (end[2] - start[2])
-
 
 def rotate(
     x: Union[float, np.ndarray[Any, np.dtype[np.floating[Any]]]],
     y: Union[float, np.ndarray[Any, np.dtype[np.floating[Any]]]],
     psi: float,
 ) -> Tuple[Any, Any]:
     """Rotate all coordinates in the x and y lists counterclockwise by the angle psi (in
@@ -52,15 +50,15 @@
     else:
         return 0
 
 
 def euclidean_distance(
     p1: Tuple[float, float, float], p2: Tuple[float, float, float]
 ) -> float:
-    """Helper method that returns the Euclidean distance between points p1 and p2, each
+    """Helper method that returns the Euclidean distance between poses p1 and p2, each
     in form (x, y, yaw).
     """
     return ((p1[0] - p2[0]) ** 2.0 + (p1[1] - p2[1]) ** 2.0) ** 0.5
 
 
 def wrap_to_pi(angle: float) -> float:
     """Wraps the given angle to its equivalent angle within the range -pi to pi."""
```

### Comparing `rsplan-1.0.2/rsplan/planner.py` & `rsplan-1.0.3/rsplan/planner.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,69 +11,69 @@
 and backwards. https://msp.org/pjm/1990/145-2/pjm-v145-n2-p06-s.pdf
 Curve formulas can be found on page 390-391.
 
 Inspiration for this Python implementation of the Reeds-Shepp algorithm:
 https://github.com/boyali/reeds_and_shepp_curves/tree/master
 
 Our implementation adds the option for a runway (straightaway segment at the end of the
-path) to improve precision in reaching the given end point. We also prioritize a path
+path) to improve precision in reaching the given end pose. We also prioritize a path
 with fewer segments over a path with a shorter overall length as long as the two paths
 have a total length within 2 meters of each others.
 """
 
 from typing import List, Literal, Tuple
 
 import numpy as np
 
 from rsplan import curves, helpers, primitives
 
 
 def path(
-    start_pt: Tuple[float, float, float],
-    end_pt: Tuple[float, float, float],
+    start_pose: Tuple[float, float, float],
+    end_pose: Tuple[float, float, float],
     turn_radius: float,
     runway_length: float,
     step_size: float,
     length_tolerance: float = 2.0,
 ) -> primitives.Path:
-    """Generates a Reeds-Shepp path given start and end points (represented as
+    """Generates a Reeds-Shepp path given start and end poses (represented as
     [x, y, yaw]), turn radius, and step size. If the path has no runway, the runway
-    length must be 0.0. If the path has a runway, calculates the runway start point,
-    creates a Reeds-Shepp path from the given start point to the runway start point, and
+    length must be 0.0. If the path has a runway, calculates the runway start pose,
+    creates a Reeds-Shepp path from the given start pose to the runway start pose, and
     adds a straight Segment to the end of the list of segments in the Path. The runway
     segment is a straightaway intended to improve the final position accuracy of
     navigation. The runway can either be driven in forward or reverse depending on the
     sign of the runway length specified and can have a variable length.
     """
     if runway_length != 0:  # Path has a runway
         runway_direction: Literal[-1, 1] = -1 if runway_length < 0.0 else 1
         runway_length = abs(runway_length)
 
-        runway_start_pt = _calc_runway_start_point(
-            end_pt, runway_direction, runway_length
+        runway_start_pose = _calc_runway_start_pose(
+            end_pose, runway_direction, runway_length
         )
 
         # Find all Reeds-Shepp paths and choose optimal one
-        all_paths = _solve_path(start_pt, runway_start_pt, turn_radius, step_size)
+        all_paths = _solve_path(start_pose, runway_start_pose, turn_radius, step_size)
         path_rs = _get_optimal_path(all_paths, length_tolerance)
 
         # Add runway segment to Path segments list
         runway_segment = _calc_runway_segment(
-            runway_start_pt, end_pt, runway_direction, turn_radius
+            runway_start_pose, end_pose, runway_direction, turn_radius
         )
         segments = path_rs.segments + [runway_segment]
     else:
         # Find all Reeds-Shepp paths and choose optimal one
-        all_paths = _solve_path(start_pt, end_pt, turn_radius, step_size)
+        all_paths = _solve_path(start_pose, end_pose, turn_radius, step_size)
         path_rs = _get_optimal_path(all_paths, length_tolerance)
         segments = path_rs.segments
 
     return primitives.Path(
-        start_pt=start_pt,
-        end_pt=end_pt,
+        start_pose=start_pose,
+        end_pose=end_pose,
         segments=segments,
         turn_radius=turn_radius,
         step_size=step_size,
     )
 
 
 ########################################################################################
@@ -87,16 +87,15 @@
     turn_rad: float,
     step_size: float,
 ) -> List[primitives.Path]:
     """Calls all 6 curve functions and returns a list of all valid Reeds-Shepp paths."""
     # If start is not origin, get end w.r.t. start instead of w.r.t. origin
     
     # Change base
-    x, y = helpers.rotate(end[0] - start[0], end[1] - start[1], -start[2])
-    phi = end[2] - start[2]
+    x, y, phi = helpers.change_base(start, end)
 
     # Create list of all Reeds-Shepp paths
     paths: List[primitives.Path] = []
     paths.extend(curves.csc(start, end, step_size, x, y, phi, turn_rad))
     paths.extend(curves.ccc(start, end, step_size, x, y, phi, turn_rad))
     paths.extend(curves.cccc(start, end, step_size, x, y, phi, turn_rad))
     paths.extend(curves.ccsc(start, end, step_size, x, y, phi, turn_rad))
@@ -124,37 +123,37 @@
         best_path = paths[1]  # Choose second shortest path because it has less segments
     else:
         best_path = paths[0]  # Choose shortest path (> length tolerance shorter than other paths)
 
     return best_path
 
 
-def _calc_runway_start_point(
-    end_pt: Tuple[float, float, float],
+def _calc_runway_start_pose(
+    end_pose: Tuple[float, float, float],
     driving_direction: Literal[1, -1],
     runway_length: float,
 ) -> Tuple[float, float, float]:
     """The start of the runway. Driving direction indicates whether the robot is
     travelling in forward or reverse along the runway.
     """
-    end_x, end_y, yaw = end_pt  # Yaw is in radians
+    end_x, end_y, yaw = end_pose  # Yaw is in radians
     x = end_x - (driving_direction * abs(runway_length) * np.cos(yaw))
     y = end_y - (driving_direction * abs(runway_length) * np.sin(yaw))
 
     return x, y, yaw
 
 
 def _calc_runway_segment(
-    start_pt: Tuple[float, float, float],
-    end_pt: Tuple[float, float, float],
+    start_pose: Tuple[float, float, float],
+    end_pose: Tuple[float, float, float],
     direction: Literal[1, -1],
     turn_radius: float,
 ) -> primitives.Segment:
     """Creates a straight Segment representing a path's runway."""
-    path_length = round(helpers.euclidean_distance(start_pt, end_pt), 3)
+    path_length = round(helpers.euclidean_distance(start_pose, end_pose), 3)
 
     return primitives.Segment(
         type="straight",
         direction=direction,
         length=path_length,
         turn_radius=turn_radius,
     )
```

### Comparing `rsplan-1.0.2/rsplan/primitives.py` & `rsplan-1.0.3/rsplan/primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 import numpy as np
 
 from rsplan import helpers
 
 
 @dataclasses.dataclass
 class Path:
-    """Reeds-Shepp path represented as its start/end points, turn radius (in meters),
+    """Reeds-Shepp path represented as its start/end poses, turn radius (in meters),
     and a list of Segments. Additionally contains a step size value (in meters) used to
     calculate the Waypoint representation of the path.
     """
 
-    start_pt: Tuple[float, float, float]
-    end_pt: Tuple[float, float, float]
+    start_pose: Tuple[float, float, float]
+    end_pose: Tuple[float, float, float]
     segments: List[Segment]
     turn_radius: float
     step_size: float
 
     @property
     def start(self) -> Waypoint:
         return self.waypoints()[0]
@@ -55,15 +55,15 @@
     def prune(self, increment: int) -> List[Waypoint]:
         """Returns a pruned list of waypoints that occur at regularly spaced distances."""
         return [
             self.waypoints()[ix] for ix in range(0, len(self.waypoints()), increment)
         ]
 
     def coordinates_tuple(self) -> Tuple[List[float], List[float], List[float]]:
-        """Convenience function for decomposing the path points into their components
+        """Convenience function for decomposing the path waypoints into their components
         (x, y, yaw).
         """
         x_coords, y_coords, yaw_coords = [], [], []
 
         for pt in self.waypoints():
             x_coords.append(pt.x)
             y_coords.append(pt.y)
@@ -74,22 +74,22 @@
     @functools.lru_cache
     def waypoints(self) -> List[Waypoint]:
         """Interpolate the path's segments into a list of Waypoints. First compute the
         pure segment points, then stitch to path list of points. For negative segments,
         we find the segment motion in positive discretization, then we adjust the sign
         of the motion in the equations.
         """
-        x0, y0, yaw0 = self.start_pt
+        x0, y0, yaw0 = self.start_pose
         path_points: List[Tuple[float, float, float, float, Literal[-1, 1], bool]] = []
 
         # Calculate list of Waypoint parameter tuples for non-runway segments
         for ix, segment in enumerate(self.segments):
             if self._has_runway and ix == len(self.segments) - 1:  # Runway segment
                 seg_points = segment.calc_waypoints(
-                    (x0, y0, yaw0), self.step_size, True, end_pt=self.end_pt
+                    (x0, y0, yaw0), self.step_size, True, end_pose=self.end_pose
                 )
                 # Remove duplicated runway starting point
                 if Waypoint(*path_points[-1]).is_close(Waypoint(*seg_points[0])):
                     seg_points.pop(0)
             else:  # Non-runway segment
                 seg_points = segment.calc_waypoints(
                     (x0, y0, yaw0), self.step_size, False
@@ -98,42 +98,42 @@
             path_points.extend(seg_points)  # Add segment pts to list of path pts
 
             # For next segment, set first point to last pt of this segment
             x0, y0, yaw0 = seg_points[-1][0], seg_points[-1][1], seg_points[-1][2]
 
         # Ensures that the path's last pt equals the provided end pt by appending end pt
         # to the list of path pts if the last pt in the path is not the end pt
-        end_pt_to_add = self._end_pt_to_add(path_points[-1])
-        path_points.append(end_pt_to_add) if end_pt_to_add is not None else ()
+        end_pose_to_add = self._end_pose_to_add(path_points[-1])
+        path_points.append(end_pose_to_add) if end_pose_to_add is not None else ()
 
         return [Waypoint(*point) for point in path_points]
 
-    def _end_pt_to_add(
+    def _end_pose_to_add(
         self, last_path_pt: Tuple[float, float, float, float, Literal[-1, 1], bool]
     ) -> Optional[Tuple[float, float, float, float, Literal[-1, 1], bool]]:
         """Checks if the last path point equals the provided Path end point. It's
         possible for end points to be slightly off the target end pose due to path
         discretization with a non-ideal step size.
         """
-        end_pt_with_params = (*self.end_pt, *last_path_pt[3:])
-        if not Waypoint(*last_path_pt).is_close(Waypoint(*end_pt_with_params)):
+        end_pose_with_params = (*self.end_pose, *last_path_pt[3:])
+        if not Waypoint(*last_path_pt).is_close(Waypoint(*end_pose_with_params)):
             # Point to append is end point with last 3 parameters from final path point
-            return end_pt_with_params
+            return end_pose_with_params
 
         return None
 
     def __hash__(self) -> int:
         segment_tuple = tuple(
             (segment.type, segment.direction, segment.length)
             for segment in self.segments
         )
         return hash(
             (
-                self.start_pt,
-                self.end_pt,
+                self.start_pose,
+                self.end_pose,
                 self.turn_radius,
                 self.step_size,
                 segment_tuple,
             )
         )
 
 
@@ -156,24 +156,24 @@
         """The direction to turn at the Waypoint defined by the right hand rule.
         Turns either left (negative), right (positive) or straight (zero).
         """
         return helpers.sign(self.curvature)
 
     @property
     def pose_2d_tuple(self) -> Tuple[float, float, float]:
-        """The X, Y, and yaw of the RSNavPoint as a Tuple."""
+        """The X, Y, and yaw of the Waypoint as a Tuple."""
         return (self.x, self.y, self.yaw)
 
     def transform_to(self, end: Waypoint) -> Tuple[float, float, float]:
         """Calculates the X and Y translation and the yaw rotation values needed to
         transform the current point to the end point.
         """
         x_translation = end.x - self.x
         y_translation = end.y - self.y
-        yaw_rotation = np.rad2deg(end.yaw - self.yaw)
+        yaw_rotation = (end.yaw - self.yaw) * 180 / np.pi
         return x_translation, y_translation, yaw_rotation
 
     def is_close(self, p2: Waypoint) -> bool:
         return [round(a, 5) for a in (self.x, self.y, self.yaw)] == [
             round(b, 5) for b in (p2.x, p2.y, p2.yaw)
         ]
 
@@ -207,30 +207,30 @@
 
     @property
     def is_straight(self) -> bool:
         return self.type == "straight"
 
     def calc_waypoints(
         self,
-        start_pt: Tuple[float, float, float],
+        start_pose: Tuple[float, float, float],
         step_size: float,
         is_runway: bool,
-        end_pt: Tuple[float, float, float] = (0.0, 0.0, 0.0),
+        end_pose: Tuple[float, float, float] = (0.0, 0.0, 0.0),
     ) -> List[Tuple[float, float, float, float, Literal[-1, 1], bool]]:
         """Calculate the parameters needed (x, y, yaw coordinates, and list of segment
         length and curvature) to calculate the list of points used to represent this
         segment.
         """
-        if self.is_straight and end_pt != (0.0, 0.0, 0.0):
+        if self.is_straight and end_pose != (0.0, 0.0, 0.0):
             # Runway segment with end point passed in for accuracy
-            xs, ys, yaws = self._straight_runway_pts(start_pt, end_pt, step_size)
+            xs, ys, yaws = self._straight_runway_pts(start_pose, end_pose, step_size)
         else:
             # Non-runway segment
             segment_points = self._interpolated(step_size)
-            xs, ys, yaws = self._get_segment_coords(start_pt, segment_points)
+            xs, ys, yaws = self._get_segment_coords(start_pose, segment_points)
 
         return [
             (xs[i], ys[i], yaws[i], self._curvature(), self.direction, is_runway)
             for i in range(len(xs))
         ]
 
     def _curvature(self) -> float:
@@ -245,47 +245,47 @@
 
     def _straight_runway_pts(
         self,
         start: Tuple[float, float, float],
         end: Tuple[float, float, float],
         step_size: float,
     ) -> Tuple[list[float], list[float], list[float]]:
-        """Calculate a straight line of coordinates from the runway start point to the
-        runway end point using the yaw angle of the runway end point to ensure the
+        """Calculate a straight line of coordinates from the runway start pose to the
+        runway end pose using the yaw angle of the runway end pose to ensure the
         runway coordinates are accurate.
         """
         num_coords = int((self.length / step_size) + 2)
         x_coords = (np.linspace(start[0], end[0], num=num_coords, dtype=float)).tolist()
         y_coords = (np.linspace(start[1], end[1], num=num_coords, dtype=float)).tolist()
         yaw_coords = (np.ones(num_coords) * end[2]).tolist()
 
         return x_coords, y_coords, yaw_coords
 
     def _get_segment_coords(
         self,
-        start: Tuple[float, float, float],
+        start_pose: Tuple[float, float, float],
         segment_points: np.ndarray[Any, np.dtype[np.floating[Any]]],
     ) -> Tuple[List[float], List[float], List[float]]:
         """Generates the segment's x, y, yaw coordinate lists for each point in the
-        interpolated list) using the segment type, turn radius, and start point.
+        interpolated list) using the segment type, turn radius, and start pose.
         """
         if self.type == "left":
             xs = self.direction * self.turn_radius * np.sin(segment_points)
             ys = self.turn_radius * (1 - np.cos(segment_points))
             yaws = self.direction * segment_points
         elif self.type == "right":
             xs = self.direction * self.turn_radius * np.sin(segment_points)
             ys = -self.turn_radius * (1 - np.cos(segment_points))
             yaws = -self.direction * segment_points
         elif self.type == "straight":
             xs = self.direction * segment_points
             ys = np.zeros(xs.shape[0])
             yaws = np.zeros(xs.shape[0])
 
-        x0, y0, yaw0 = start
+        x0, y0, yaw0 = start_pose
         # Rotate generic coordinates w.r.t segment start orientation
         yaw_coords = (yaws + yaw0).tolist()
         xs, ys = helpers.rotate(xs, ys, yaw0) if yaw0 != 0 else (xs, ys)
 
         # Add segment start position (x0 and y0) values to x and y coordinates
         x_coords = (xs + x0).tolist()
         y_coords = (ys + y0).tolist()
```

### Comparing `rsplan-1.0.2/rsplan/unit_tests.py` & `rsplan-1.0.3/rsplan/unit_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,16 +76,16 @@
 def test_straight_path(
     start: Tuple[float, float, float], end: Tuple[float, float, float]
 ) -> None:
 
     nav_path = _nav_path(start, end, has_runway=False)
     assert nav_path is not None
 
-    assert start == nav_path.start_pt
-    assert end == nav_path.end_pt
+    assert start == nav_path.start_pose
+    assert end == nav_path.end_pose
 
     assert round(nav_path.total_length, 5) == round(
         helpers.euclidean_distance(start, end), 5
     )
 
     for wp1, wp2 in zip(nav_path.waypoints()[:-1], nav_path.waypoints()[1:]):
         assert wp1 != wp2
@@ -121,16 +121,16 @@
 def test_path_no_runway(
     start: Tuple[float, float, float], end: Tuple[float, float, float]
 ) -> None:
 
     nav_path = _nav_path(start, end, has_runway=False)
 
     assert nav_path.total_length >= helpers.euclidean_distance(start, end)
-    assert start == nav_path.start_pt
-    assert end == nav_path.end_pt
+    assert start == nav_path.start_pose
+    assert end == nav_path.end_pose
 
     assert all(waypoint.is_runway is False for waypoint in nav_path.waypoints())
 
     for wp1, wp2 in zip(nav_path.waypoints()[:-1], nav_path.waypoints()[1:]):
         assert wp1 != wp2
 
 
@@ -151,16 +151,16 @@
     y = _RANDOM_PATH_DISTANCE_RANGE * rng.uniform(-1, 1)
     yaw = _RANDOM_PATH_ANGLE_RANGE * rng.random()
     end = (x, y, yaw)
 
     nav_path = _nav_path(start, end)
 
     assert nav_path.total_length >= helpers.euclidean_distance(start, end)
-    assert nav_path.start_pt == start
-    assert nav_path.end_pt == end
+    assert nav_path.start_pose == start
+    assert nav_path.end_pose == end
 
     for wp1, wp2 in zip(nav_path.waypoints()[:-1], nav_path.waypoints()[1:]):
         assert wp1 != wp2
 
 
 def main() -> None:
     test_random_path()
```

### Comparing `rsplan-1.0.2/rsplan.egg-info/PKG-INFO` & `rsplan-1.0.3/rsplan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.2
+Version: 1.0.3
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
@@ -31,41 +31,43 @@
   - [Running](#running)
   - [Demo](#demo)
 - [FAQ](#faq)
 - [Exhibits](#exhibits)
 - [References](#references)
 
 ## Overview
-This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions including 3.11.
+This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions >= 3.9, including 3.11.
 
 Contains the following files:
   - `planner`: Path planning code. `path` function outputs the optimal Reeds-Shepp path with or without a runway.
   - `curves`: Curve formulas for all of the curve types in the Reeds-Shepp paper.
-  - `primitives`: Three class architectures (path, waypoint, and segment).
-    - Waypoint class (stores x, y, yaw, as well as the curvature and angle/length of the segment the waypoint is on)
-    - Segment class (stores left/right/straight type, forward/backward direction, magnitude (arc angle or straight length), and turn radius of the segment)
+  - `primitives`: Three class architectures (Waypoint, Segment, and Path).
+    - Waypoint class (stores x, y, yaw of the waypoint and the curvature and length of the segment the waypoint is on as well as if the segment is a runway)
+    - Segment class (stores left/right/straight type, forward/backward direction, length, and turn radius of the segment)
     - Path class (stores start and end points, turn radius, step size, and list of Segments. Also contains a cached waypoints function to get a list of Waypoints for the path)
   - `helpers`: Helper functions for planner, primitives, and curves files.
   - `demo`: Demo/visualization of paths.
 
 
 
 ## Usage
 
-### Running
+### Installation
+You can install this software using pip:
+
+`pip install -U rsplan`
 
-See demo.py for example usage
 
-path(start_pt, end_pt, turn_radius, runway_length, step_size, length_tolerance (optional))
-- return a Reeds-Shepp path from start_pt to end_pt with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
-- start_pt and end_pt are in the format `Tuple[float, float, float]` of x, y, yaw values.
+### Running
 
-### Demo
+See demo.py for example usage
 
-$ python demos/demo.py
+path(start_pose, end_pose, turn_radius, runway_length, step_size, length_tolerance (optional))
+- return a Reeds-Shepp path from start_pose to end_pose with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
+- start_pose and end_pose are in the format `Tuple[float, float, float]` of x, y, yaw values.
 
 
 ## FAQ
 
 What are t, u, and v parameters?
 - As a whole, t, u, v are segment parameters generated in each of the curve helper functions that represent the distance (angular distance for curved segments, linear distance for straight segments) of their respective segments.
 - If there are 3 segments (ccc or csc), t is for segment 1, u is for segment 2, and v is for segment 3.
@@ -78,14 +80,15 @@
 
 
 ### Exhibits
 
 From demo.py:
 
 Paths start from origin
+
 Format: (end x, end y, yaw, turn radius, runway length)
 1. (5, 6, np.pi, 1, 0)
 2. (15, 3, np.pi / 2.0, 2, 6)
 3. (-2, -4, np.pi, 4, 3)
 4. (-7, 2, np.pi, 4, 0)
 5. (-7, -7, 0.0, 6, 1)
 6. (0.7, 1.8, 1, 1, 1)
```

### Comparing `rsplan-1.0.2/setup.py` & `rsplan-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "rsplan",
-    version = "1.0.2",
+    version = "1.0.3",
     author = "Built Robotics",
     author_email = "tarakapoor9@gmail.com",
     description = ("Reeds-Shepp algorithm implementation in Python."),
     license = "MIT",
     keywords = "reeds-shepp path planning",
     url = "https://github.com/builtrobotics/rs",
     packages=['rsplan'],
```

