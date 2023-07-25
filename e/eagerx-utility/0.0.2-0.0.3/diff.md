# Comparing `tmp/eagerx_utility-0.0.2.tar.gz` & `tmp/eagerx_utility-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagerx_utility-0.0.2.tar", max compression
+gzip compressed data, was "eagerx_utility-0.0.3.tar", max compression
```

## Comparing `eagerx_utility-0.0.2.tar` & `eagerx_utility-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/LICENSE
--rw-r--r--   0        0        0       22 2023-01-04 10:55:21.933493 eagerx_utility-0.0.2/eagerx_utility/__init__.py
--rw-r--r--   0        0        0     3336 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/aruco_detector.py
--rw-r--r--   0        0        0        0 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/camera/__init__.py
--rw-r--r--   0        0        0     6255 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/camera/assets/realsense2_d435.urdf
--rw-r--r--   0        0        0     6156 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/camera/calibration.py
--rw-r--r--   0        0        0      324 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/camera/enginestates.py
--rw-r--r--   0        0        0     8896 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/camera/objects.py
--rw-r--r--   0        0        0    11039 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/camera/pybullet/enginenodes.py
--rw-r--r--   0        0        0        0 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/ik/__init__.py
--rw-r--r--   0        0        0     5679 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/ik/node.py
--rw-r--r--   0        0        0        0 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/overlay/__init__.py
--rw-r--r--   0        0        0     3910 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/overlay/node.py
--rw-r--r--   0        0        0        0 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/reset/__init__.py
--rw-r--r--   0        0        0     4117 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/reset/node.py
--rw-r--r--   0        0        0        0 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/safety/__init__.py
--rw-r--r--   0        0        0     8894 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/safety/collision.py
--rw-r--r--   0        0        0    18209 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/safety/node.py
--rw-r--r--   0        0        0     2383 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/safety/workspaces.py
--rw-r--r--   0        0        0        0 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/__init__.py
--rw-r--r--   0        0        0      924 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/assets/box.urdf
--rw-r--r--   0        0        0      311 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/assets/box_goal.urdf
--rw-r--r--   0        0        0      956 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/assets/can.urdf
--rw-r--r--   0        0        0      352 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/assets/can_goal.urdf
--rw-r--r--   0        0        0      304 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/assets/surface.urdf
--rw-r--r--   0        0        0     4726 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/goal.py
--rw-r--r--   0        0        0        0 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/real/__init__.py
--rw-r--r--   0        0        0     8963 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/real/enginenodes.py
--rw-r--r--   0        0        0     1907 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/real/enginestates.py
--rw-r--r--   0        0        0     8256 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/solid.py
--rw-r--r--   0        0        0     3544 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/solid/yaw_node.py
--rw-r--r--   0        0        0     3372 2023-01-04 10:55:12.793297 eagerx_utility-0.0.2/eagerx_utility/utils.py
--rw-r--r--   0        0        0      942 2023-01-04 10:55:21.933493 eagerx_utility-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 eagerx_utility-0.0.2/setup.py
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 eagerx_utility-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/LICENSE
+-rw-r--r--   0        0        0       22 2023-07-25 09:33:33.860363 eagerx_utility-0.0.3/eagerx_utility/__init__.py
+-rw-r--r--   0        0        0     3336 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/aruco_detector.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/camera/__init__.py
+-rw-r--r--   0        0        0     6255 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/camera/assets/realsense2_d435.urdf
+-rw-r--r--   0        0        0     6156 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/camera/calibration.py
+-rw-r--r--   0        0        0      324 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/camera/enginestates.py
+-rw-r--r--   0        0        0     8896 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/camera/objects.py
+-rw-r--r--   0        0        0    11039 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/camera/pybullet/enginenodes.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/ik/__init__.py
+-rw-r--r--   0        0        0     5679 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/ik/node.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/overlay/__init__.py
+-rw-r--r--   0        0        0     3910 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/overlay/node.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/reset/__init__.py
+-rw-r--r--   0        0        0     4117 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/reset/node.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/safety/__init__.py
+-rw-r--r--   0        0        0     8894 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/safety/collision.py
+-rw-r--r--   0        0        0    18209 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/safety/node.py
+-rw-r--r--   0        0        0     2383 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/safety/workspaces.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/__init__.py
+-rw-r--r--   0        0        0      924 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/assets/box.urdf
+-rw-r--r--   0        0        0      311 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/assets/box_goal.urdf
+-rw-r--r--   0        0        0      956 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/assets/can.urdf
+-rw-r--r--   0        0        0      352 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/assets/can_goal.urdf
+-rw-r--r--   0        0        0      304 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/assets/surface.urdf
+-rw-r--r--   0        0        0     4726 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/goal.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/real/__init__.py
+-rw-r--r--   0        0        0     8963 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/real/enginenodes.py
+-rw-r--r--   0        0        0     1907 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/real/enginestates.py
+-rw-r--r--   0        0        0     8256 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/solid.py
+-rw-r--r--   0        0        0     3544 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/solid/yaw_node.py
+-rw-r--r--   0        0        0     3372 2023-07-25 09:33:22.856440 eagerx_utility-0.0.3/eagerx_utility/utils.py
+-rw-r--r--   0        0        0      940 2023-07-25 09:33:33.860363 eagerx_utility-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 eagerx_utility-0.0.3/PKG-INFO
```

### Comparing `eagerx_utility-0.0.2/LICENSE` & `eagerx_utility-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/aruco_detector.py` & `eagerx_utility-0.0.3/eagerx_utility/aruco_detector.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/camera/assets/realsense2_d435.urdf` & `eagerx_utility-0.0.3/eagerx_utility/camera/assets/realsense2_d435.urdf`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/camera/calibration.py` & `eagerx_utility-0.0.3/eagerx_utility/camera/calibration.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/camera/objects.py` & `eagerx_utility-0.0.3/eagerx_utility/camera/objects.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/camera/pybullet/enginenodes.py` & `eagerx_utility-0.0.3/eagerx_utility/camera/pybullet/enginenodes.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/ik/node.py` & `eagerx_utility-0.0.3/eagerx_utility/ik/node.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/overlay/node.py` & `eagerx_utility-0.0.3/eagerx_utility/overlay/node.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/reset/node.py` & `eagerx_utility-0.0.3/eagerx_utility/reset/node.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/safety/collision.py` & `eagerx_utility-0.0.3/eagerx_utility/safety/collision.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/safety/node.py` & `eagerx_utility-0.0.3/eagerx_utility/safety/node.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/safety/workspaces.py` & `eagerx_utility-0.0.3/eagerx_utility/safety/workspaces.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/solid/assets/box.urdf` & `eagerx_utility-0.0.3/eagerx_utility/solid/assets/box.urdf`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/solid/assets/can.urdf` & `eagerx_utility-0.0.3/eagerx_utility/solid/assets/can.urdf`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/solid/goal.py` & `eagerx_utility-0.0.3/eagerx_utility/solid/goal.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/solid/real/enginenodes.py` & `eagerx_utility-0.0.3/eagerx_utility/solid/real/enginenodes.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/solid/real/enginestates.py` & `eagerx_utility-0.0.3/eagerx_utility/solid/real/enginestates.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/solid/solid.py` & `eagerx_utility-0.0.3/eagerx_utility/solid/solid.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/solid/yaw_node.py` & `eagerx_utility-0.0.3/eagerx_utility/solid/yaw_node.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/eagerx_utility/utils.py` & `eagerx_utility-0.0.3/eagerx_utility/utils.py`

 * *Files identical despite different names*

### Comparing `eagerx_utility-0.0.2/pyproject.toml` & `eagerx_utility-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "eagerx_utility"
-version = "0.0.2"
+version = "0.0.3"
 license = "Apache2.0"
 description = "Template for creating EAGERx packages."
 authors = ["Jelle Luijkx <j.d.luijkx@tudelft.nl>", "Bas van der Heijden <d.s.vanderheijden@tudelft.nl>"]
 homepage = "https://github.com/eager-dev/eagerx_utility"
 repository = "https://github.com/eager-dev/eagerx_utility"
 documentation = "https://eagerx.readthedocs.io/en/master/"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
-eagerx = "^0.1.13"
+python = "^3.8"
+eagerx = "^0.1.38"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pytest = "^7.0"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 flake8 = ">=3"
 flake8-bugbear = "^22.3.23"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eagerx_utility-0.0.2/PKG-INFO` & `eagerx_utility-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: eagerx-utility
-Version: 0.0.2
+Version: 0.0.3
 Summary: Template for creating EAGERx packages.
 Home-page: https://github.com/eager-dev/eagerx_utility
 License: Apache2.0
 Author: Jelle Luijkx
 Author-email: j.d.luijkx@tudelft.nl
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: eagerx (>=0.1.13,<0.2.0)
+Requires-Dist: eagerx (>=0.1.38,<0.2.0)
 Project-URL: Documentation, https://eagerx.readthedocs.io/en/master/
 Project-URL: Repository, https://github.com/eager-dev/eagerx_utility
```

