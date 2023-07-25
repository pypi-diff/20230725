# Comparing `tmp/forwardkinematics-1.1.3.tar.gz` & `tmp/forwardkinematics-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forwardkinematics-1.1.3.tar", max compression
+gzip compressed data, was "forwardkinematics-1.1.4.tar", max compression
```

## Comparing `forwardkinematics-1.1.3.tar` & `forwardkinematics-1.1.4.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0      582 2022-05-23 06:27:34.000000 forwardkinematics-1.1.3/README.md
--rw-r--r--   0        0        0        0 2021-12-23 11:38:15.000000 forwardkinematics-1.1.3/forwardkinematics/__init__.py
--rw-r--r--   0        0        0      849 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk.py
--rw-r--r--   0        0        0      741 2022-05-10 14:08:20.000000 forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk_by_name.py
--rw-r--r--   0        0        0     1760 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk_creator.py
--rw-r--r--   0        0        0     1548 2022-03-31 08:49:42.000000 forwardkinematics-1.1.3/forwardkinematics/planarFks/groundRobotFk.py
--rw-r--r--   0        0        0     1949 2022-03-31 08:49:42.000000 forwardkinematics-1.1.3/forwardkinematics/planarFks/mobileRobotFk.py
--rw-r--r--   0        0        0     1140 2023-03-01 09:04:08.669225 forwardkinematics-1.1.3/forwardkinematics/planarFks/planarArmFk.py
--rw-r--r--   0        0        0      842 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/planarFks/planar_fk.py
--rw-r--r--   0        0        0     1054 2022-05-23 06:19:44.000000 forwardkinematics-1.1.3/forwardkinematics/planarFks/pointFk.py
--rw-r--r--   0        0        0      468 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/albertFk.py
--rw-r--r--   0        0        0      343 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/boxerFk.py
--rw-r--r--   0        0        0        0 2021-12-23 10:47:55.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/__init__.py
--rw-r--r--   0        0        0        0 2021-12-23 10:47:55.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
--rw-r--r--   0        0        0     3442 2022-03-16 12:17:29.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
--rwxr-xr-x   0        0        0     6237 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
--rw-r--r--   0        0        0      380 2022-05-23 12:16:36.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/dual_arm_fk.py
--rw-r--r--   0        0        0     3544 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/urdfFks/generic_urdf_fk.py
--rw-r--r--   0        0        0      306 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/jackalFk.py
--rw-r--r--   0        0        0      436 2022-05-23 12:16:36.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/mobilePandaFk.py
--rw-r--r--   0        0        0      367 2022-05-23 12:16:36.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/pandaFk.py
--rw-r--r--   0        0        0      365 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/pointRobotUrdfFk.py
--rw-r--r--   0        0        0      841 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/tiagoFk.py
--rw-r--r--   0        0        0     7580 2023-03-01 09:56:43.501774 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/albert.urdf
--rw-r--r--   0        0        0     2031 2023-03-01 09:56:43.501774 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/boxer.urdf
--rw-r--r--   0        0        0     8160 2022-03-16 12:17:29.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/dual_arm.urdf
--rw-r--r--   0        0        0     1693 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/jackal.urdf
--rw-r--r--   0        0        0    12167 2021-12-23 11:38:39.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/mobilePanda.urdf
--rw-r--r--   0        0        0    12455 2022-03-16 12:17:29.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/panda.urdf
--rw-r--r--   0        0        0     2628 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/pointRobot.urdf
--rw-r--r--   0        0        0    33577 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/tiago.urdf
--rw-r--r--   0        0        0     3304 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdfFk.py
--rw-r--r--   0        0        0      738 2023-07-21 14:40:42.572056 forwardkinematics-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 forwardkinematics-1.1.3/setup.py
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 forwardkinematics-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      582 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/README.md
+-rw-r--r--   0        0        0       71 2023-07-25 18:39:32.736912 forwardkinematics-1.1.4/forwardkinematics/__init__.py
+-rw-r--r--   0        0        0      849 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/fksCommon/fk.py
+-rw-r--r--   0        0        0      741 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/fksCommon/fk_by_name.py
+-rw-r--r--   0        0        0     1760 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/fksCommon/fk_creator.py
+-rw-r--r--   0        0        0     1548 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/planarFks/groundRobotFk.py
+-rw-r--r--   0        0        0     1949 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/planarFks/mobileRobotFk.py
+-rw-r--r--   0        0        0     1140 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/planarFks/planarArmFk.py
+-rw-r--r--   0        0        0      842 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/planarFks/planar_fk.py
+-rw-r--r--   0        0        0     1054 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/planarFks/pointFk.py
+-rw-r--r--   0        0        0      468 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/albertFk.py
+-rw-r--r--   0        0        0      343 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/boxerFk.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:39:02.166915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/casadiConversion/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
+-rw-r--r--   0        0        0     3442 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
+-rwxr-xr-x   0        0        0     6237 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
+-rw-r--r--   0        0        0      380 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/dual_arm_fk.py
+-rw-r--r--   0        0        0     3544 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/generic_urdf_fk.py
+-rw-r--r--   0        0        0      306 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/jackalFk.py
+-rw-r--r--   0        0        0      436 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/mobilePandaFk.py
+-rw-r--r--   0        0        0      367 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/pandaFk.py
+-rw-r--r--   0        0        0      365 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/pointRobotUrdfFk.py
+-rw-r--r--   0        0        0      841 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/tiagoFk.py
+-rw-r--r--   0        0        0     7580 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/albert.urdf
+-rw-r--r--   0        0        0     2031 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/boxer.urdf
+-rw-r--r--   0        0        0     8160 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/dual_arm.urdf
+-rw-r--r--   0        0        0     1693 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/jackal.urdf
+-rw-r--r--   0        0        0    12167 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/mobilePanda.urdf
+-rw-r--r--   0        0        0    12455 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/panda.urdf
+-rw-r--r--   0        0        0     2628 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/pointRobot.urdf
+-rw-r--r--   0        0        0    33577 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/tiago.urdf
+-rw-r--r--   0        0        0     3304 2023-07-25 18:39:02.170915 forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdfFk.py
+-rw-r--r--   0        0        0      738 2023-07-25 18:39:32.736912 forwardkinematics-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 forwardkinematics-1.1.4/PKG-INFO
```

### Comparing `forwardkinematics-1.1.3/README.md` & `forwardkinematics-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk.py` & `forwardkinematics-1.1.4/forwardkinematics/fksCommon/fk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk_by_name.py` & `forwardkinematics-1.1.4/forwardkinematics/fksCommon/fk_by_name.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk_creator.py` & `forwardkinematics-1.1.4/forwardkinematics/fksCommon/fk_creator.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/planarFks/groundRobotFk.py` & `forwardkinematics-1.1.4/forwardkinematics/planarFks/groundRobotFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/planarFks/mobileRobotFk.py` & `forwardkinematics-1.1.4/forwardkinematics/planarFks/mobileRobotFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/planarFks/planarArmFk.py` & `forwardkinematics-1.1.4/forwardkinematics/planarFks/planarArmFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/planarFks/planar_fk.py` & `forwardkinematics-1.1.4/forwardkinematics/planarFks/planar_fk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/planarFks/pointFk.py` & `forwardkinematics-1.1.4/forwardkinematics/planarFks/pointFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/urdfparser.py` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/casadiConversion/urdfparser.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/generic_urdf_fk.py` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/generic_urdf_fk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/tiagoFk.py` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/tiagoFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/albert.urdf` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/albert.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/boxer.urdf` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/boxer.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/dual_arm.urdf` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/dual_arm.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/jackal.urdf` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/jackal.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/mobilePanda.urdf` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/mobilePanda.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/panda.urdf` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/panda.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/pointRobot.urdf` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/pointRobot.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/tiago.urdf` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdf/tiago.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdfFk.py` & `forwardkinematics-1.1.4/forwardkinematics/urdfFks/urdfFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.3/pyproject.toml` & `forwardkinematics-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forwardkinematics"
-version = "1.1.3"
+version = "1.1.4"
 description = "\"Light-weight implementation of forward kinematics using casadi.\""
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maxspahn/forwardKinematics.git"
 repository = "https://github.com/maxspahn/forwardKinematics.git"
```

### Comparing `forwardkinematics-1.1.3/PKG-INFO` & `forwardkinematics-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forwardkinematics
-Version: 1.1.3
+Version: 1.1.4
 Summary: "Light-weight implementation of forward kinematics using casadi."
 Home-page: https://github.com/maxspahn/forwardKinematics.git
 License: MIT
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
```

