# Comparing `tmp/rsplan-1.0.3.tar.gz` & `tmp/rsplan-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsplan-1.0.3.tar", last modified: Tue Jul 25 02:12:57 2023, max compression
+gzip compressed data, was "rsplan-1.0.4.tar", last modified: Tue Jul 25 19:48:43 2023, max compression
```

## Comparing `rsplan-1.0.3.tar` & `rsplan-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 02:12:57.762412 rsplan-1.0.3/
--rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.3/LICENSE
--rw-rw-r--   0 built     (1000) built     (1000)     5490 2023-07-25 02:12:57.762412 rsplan-1.0.3/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)     3833 2023-07-25 02:06:53.000000 rsplan-1.0.3/README.md
--rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-25 02:12:06.000000 rsplan-1.0.3/pyproject.toml
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 02:12:57.762412 rsplan-1.0.3/rsplan/
--rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-19 03:21:47.000000 rsplan-1.0.3/rsplan/__init__.py
--rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-24 00:19:10.000000 rsplan-1.0.3/rsplan/curves.py
--rw-rw-r--   0 built     (1000) built     (1000)     2582 2023-07-25 01:59:29.000000 rsplan-1.0.3/rsplan/demo.py
--rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.3/rsplan/helpers.py
--rw-rw-r--   0 built     (1000) built     (1000)     6505 2023-07-25 02:01:50.000000 rsplan-1.0.3/rsplan/planner.py
--rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-07-25 01:56:11.000000 rsplan-1.0.3/rsplan/primitives.py
--rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.3/rsplan/unit_tests.py
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 02:12:57.762412 rsplan-1.0.3/rsplan.egg-info/
--rw-rw-r--   0 built     (1000) built     (1000)     5490 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)      319 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/SOURCES.txt
--rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/dependency_links.txt
--rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/requires.txt
--rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-25 02:12:57.000000 rsplan-1.0.3/rsplan.egg-info/top_level.txt
--rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-25 02:12:57.762412 rsplan-1.0.3/setup.cfg
--rw-rw-r--   0 built     (1000) built     (1000)      643 2023-07-25 02:12:08.000000 rsplan-1.0.3/setup.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 19:48:43.930349 rsplan-1.0.4/
+-rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.4/LICENSE
+-rw-rw-r--   0 built     (1000) built     (1000)     5490 2023-07-25 19:48:43.930349 rsplan-1.0.4/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)     3833 2023-07-25 02:06:53.000000 rsplan-1.0.4/README.md
+-rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-25 19:48:33.000000 rsplan-1.0.4/pyproject.toml
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 19:48:43.930349 rsplan-1.0.4/rsplan/
+-rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-19 03:21:47.000000 rsplan-1.0.4/rsplan/__init__.py
+-rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-24 00:19:10.000000 rsplan-1.0.4/rsplan/curves.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2582 2023-07-25 01:59:29.000000 rsplan-1.0.4/rsplan/demo.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.4/rsplan/helpers.py
+-rw-rw-r--   0 built     (1000) built     (1000)     6597 2023-07-25 02:48:24.000000 rsplan-1.0.4/rsplan/planner.py
+-rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-07-25 01:56:11.000000 rsplan-1.0.4/rsplan/primitives.py
+-rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-25 19:46:23.000000 rsplan-1.0.4/rsplan/py.typed
+-rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.4/rsplan/unit_tests.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 19:48:43.930349 rsplan-1.0.4/rsplan.egg-info/
+-rw-rw-r--   0 built     (1000) built     (1000)     5490 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)      335 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/SOURCES.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/dependency_links.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/requires.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/top_level.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-25 19:48:43.930349 rsplan-1.0.4/setup.cfg
+-rw-rw-r--   0 built     (1000) built     (1000)      686 2023-07-25 19:48:23.000000 rsplan-1.0.4/setup.py
```

### Comparing `rsplan-1.0.3/LICENSE` & `rsplan-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.3/PKG-INFO` & `rsplan-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.3
+Version: 1.0.4
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
```

### Comparing `rsplan-1.0.3/README.md` & `rsplan-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.3/pyproject.toml` & `rsplan-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsplan"
-version = "1.0.3"
+version = "1.0.4"
 description = "Reeds-Shepp algorithm implementation in Python"
 readme = "README.md"
 authors = [{ name = "Built Robotics", email = "tarakapoor9@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rsplan-1.0.3/rsplan/curves.py` & `rsplan-1.0.4/rsplan/curves.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.3/rsplan/demo.py` & `rsplan-1.0.4/rsplan/demo.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.3/rsplan/helpers.py` & `rsplan-1.0.4/rsplan/helpers.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.3/rsplan/planner.py` & `rsplan-1.0.4/rsplan/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,36 +31,40 @@
     start_pose: Tuple[float, float, float],
     end_pose: Tuple[float, float, float],
     turn_radius: float,
     runway_length: float,
     step_size: float,
     length_tolerance: float = 2.0,
 ) -> primitives.Path:
-    """Generates a Reeds-Shepp path given start and end poses (represented as
-    [x, y, yaw]), turn radius, and step size. If the path has no runway, the runway
-    length must be 0.0. If the path has a runway, calculates the runway start pose,
-    creates a Reeds-Shepp path from the given start pose to the runway start pose, and
-    adds a straight Segment to the end of the list of segments in the Path. The runway
-    segment is a straightaway intended to improve the final position accuracy of
-    navigation. The runway can either be driven in forward or reverse depending on the
-    sign of the runway length specified and can have a variable length.
+    """Generates a Reeds-Shepp path given start and end points (represented as
+    [x, y, yaw]), turn radius, and step size. The step size is the distance between each
+    point in the list of points (e.g. 0.05m).
+    
+    If the path has no runway, the runway length must be 0.0.
+    
+    If the path has a runway, calculates the runway start pose, creates a Reeds-Shepp
+    path from the given start pose to the runway start pose, and adds a straight Segment
+    to the end of the list of Segments in the Path. The runway Segment is a straightaway
+    intended to improve the final position accuracy of navigation. The runway can either
+    be driven in forward or reverse depending on the sign of the runway length specified
+    and can have a variable length.
     """
     if runway_length != 0:  # Path has a runway
         runway_direction: Literal[-1, 1] = -1 if runway_length < 0.0 else 1
-        runway_length = abs(runway_length)
+        abs_runway_length = abs(runway_length)
 
         runway_start_pose = _calc_runway_start_pose(
-            end_pose, runway_direction, runway_length
+            end_pose, runway_direction, abs_runway_length
         )
 
         # Find all Reeds-Shepp paths and choose optimal one
         all_paths = _solve_path(start_pose, runway_start_pose, turn_radius, step_size)
         path_rs = _get_optimal_path(all_paths, length_tolerance)
 
-        # Add runway segment to Path segments list
+        # Add runway Segment to Path list of Segments
         runway_segment = _calc_runway_segment(
             runway_start_pose, end_pose, runway_direction, turn_radius
         )
         segments = path_rs.segments + [runway_segment]
     else:
         # Find all Reeds-Shepp paths and choose optimal one
         all_paths = _solve_path(start_pose, end_pose, turn_radius, step_size)
@@ -85,16 +89,14 @@
     start: Tuple[float, float, float],
     end: Tuple[float, float, float],
     turn_rad: float,
     step_size: float,
 ) -> List[primitives.Path]:
     """Calls all 6 curve functions and returns a list of all valid Reeds-Shepp paths."""
     # If start is not origin, get end w.r.t. start instead of w.r.t. origin
-    
-    # Change base
     x, y, phi = helpers.change_base(start, end)
 
     # Create list of all Reeds-Shepp paths
     paths: List[primitives.Path] = []
     paths.extend(curves.csc(start, end, step_size, x, y, phi, turn_rad))
     paths.extend(curves.ccc(start, end, step_size, x, y, phi, turn_rad))
     paths.extend(curves.cccc(start, end, step_size, x, y, phi, turn_rad))
```

### Comparing `rsplan-1.0.3/rsplan/primitives.py` & `rsplan-1.0.4/rsplan/primitives.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.3/rsplan/unit_tests.py` & `rsplan-1.0.4/rsplan/unit_tests.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.3/rsplan.egg-info/PKG-INFO` & `rsplan-1.0.4/rsplan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.3
+Version: 1.0.4
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
```

