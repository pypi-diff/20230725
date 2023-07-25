# Comparing `tmp/PyFlyt-0.8.2.tar.gz` & `tmp/PyFlyt-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.8.2.tar", last modified: Wed Jul 19 16:07:45 2023, max compression
+gzip compressed data, was "PyFlyt-0.8.3.tar", last modified: Tue Jul 25 11:05:25 2023, max compression
```

## Comparing `PyFlyt-0.8.2.tar` & `PyFlyt-0.8.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.8.2/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1514 2023-07-19 12:21:37.000000 PyFlyt-0.8.2/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.8.2/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-12 22:54:11.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/base_wind_field.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12160 2023-07-19 16:05:50.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-29 18:39:28.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7560 2023-07-17 12:29:32.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-06-07 19:10:09.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-06-07 19:14:24.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-06-07 19:08:30.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.8.2/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-07-19 16:06:15.000000 PyFlyt-0.8.2/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.8.2/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-29 18:39:28.000000 PyFlyt-0.8.2/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-29 18:39:28.000000 PyFlyt-0.8.2/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-29 18:39:28.000000 PyFlyt-0.8.2/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-14 18:31:25.000000 PyFlyt-0.8.2/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt/core/wind/
--rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.8.2/PyFlyt/core/wind/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-05-29 18:39:28.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-05-29 18:39:28.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-07-19 16:01:20.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.8.2/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.8.2/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.8.2/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.8.2/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.8.2/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.835173 PyFlyt-0.8.2/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-19 16:07:45.000000 PyFlyt-0.8.2/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1959 2023-07-19 16:07:45.000000 PyFlyt-0.8.2/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-19 16:07:45.000000 PyFlyt-0.8.2/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-07-19 16:07:45.000000 PyFlyt-0.8.2/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-19 16:07:45.000000 PyFlyt-0.8.2/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1236 2023-07-19 16:07:36.000000 PyFlyt-0.8.2/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2421 2023-07-19 13:24:00.000000 PyFlyt-0.8.2/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/setup.cfg
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-19 16:07:45.839173 PyFlyt-0.8.2/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8603 2023-05-12 23:01:51.000000 PyFlyt-0.8.2/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4779 2023-07-19 16:07:18.000000 PyFlyt-0.8.2/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.901300 PyFlyt-0.8.3/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.8.3/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-25 11:05:25.901300 PyFlyt-0.8.3/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      508 2023-07-25 11:03:32.000000 PyFlyt-0.8.3/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.8.3/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-12 22:54:11.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12160 2023-07-19 16:05:50.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7560 2023-07-25 11:03:23.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-06-07 19:10:09.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-06-07 19:14:24.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-06-07 19:08:30.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-07-25 10:38:46.000000 PyFlyt-0.8.3/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.8.3/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-07-25 10:38:45.000000 PyFlyt-0.8.3/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-14 18:31:25.000000 PyFlyt-0.8.3/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.8.3/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9097 2023-07-25 10:48:05.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8831 2023-07-25 10:47:00.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3977 2023-07-19 17:39:31.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11470 2023-07-25 10:48:09.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-07-19 16:01:20.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.8.3/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.8.3/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.8.3/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1959 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1236 2023-07-25 11:05:18.000000 PyFlyt-0.8.3/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2421 2023-07-19 13:24:00.000000 PyFlyt-0.8.3/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-25 11:05:25.901300 PyFlyt-0.8.3/setup.cfg
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9520 2023-07-25 10:58:02.000000 PyFlyt-0.8.3/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5258 2023-07-25 10:51:05.000000 PyFlyt-0.8.3/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.8.2/LICENSE.txt` & `PyFlyt-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PKG-INFO` & `PyFlyt-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.8.2
+Version: 0.8.3
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.8.3/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/aviary.py` & `PyFlyt-0.8.3/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.8.3/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.8.3/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.8.3/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/core/load_objs.py` & `PyFlyt-0.8.3/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,14 @@
     def render(self):
         """render."""
         assert (
             self.render_mode is not None
         ), "Please set `render_mode='human'` or `render_mode='rgb_array'` to use this function."
 
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
-            width=self.render_resolution[0],
-            height=self.render_resolution[1],
+            width=self.render_resolution[1],
+            height=self.render_resolution[0],
             viewMatrix=self.env.drones[0].camera.view_mat,
             projectionMatrix=self.env.drones[0].camera.proj_mat,
         )
 
-        return np.array(rgbaImg, dtype=np.uint8).reshape(
-            self.render_resolution[1], self.render_resolution[0], -1
-        )
+        return rgbaImg
```

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,16 +261,14 @@
     def render(self):
         """render."""
         assert (
             self.render_mode is not None
         ), "Please set `render_mode='human'` or `render_mode='rgb_array'` to use this function."
 
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
-            width=self.render_resolution[0],
-            height=self.render_resolution[1],
+            width=self.render_resolution[1],
+            height=self.render_resolution[0],
             viewMatrix=self.camera_parameters[2],
             projectionMatrix=self.camera_parameters[3],
         )
 
-        return np.array(rgbaImg, dtype=np.uint8).reshape(
-            self.render_resolution[1], self.render_resolution[0], -1
-        )
+        return rgbaImg
```

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 [*ang_vel, *quarternion, *lin_vel, *lin_pos, *self.action, *aux_state]
             )
 
     def compute_term_trunc_reward(self):
         """Computes the termination, truncation, and reward of the current timestep."""
         super().compute_base_term_trunc_reward()
 
-        if self.sparse_reward:
+        if not self.sparse_reward:
             # distance from 0, 0, 1 hover point
             linear_distance = np.linalg.norm(
                 self.env.state(0)[-1] - np.array([0.0, 0.0, 1.0])
             )
 
             # how far are we from 0 roll pitch
             angular_distance = np.linalg.norm(self.env.state(0)[1][:2])
```

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,16 +323,13 @@
     def render(self):
         """render."""
         assert (
             self.render_mode is not None
         ), "Please set `render_mode='human'` or `render_mode='rgb_array'` to use this function."
 
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
-            width=self.render_resolution[0],
-            height=self.render_resolution[1],
+            width=self.render_resolution[1],
+            height=self.render_resolution[0],
             viewMatrix=self.env.drones[0].camera.view_mat,
             projectionMatrix=self.env.drones[0].camera.proj_mat,
         )
-
-        return np.array(rgbaImg, dtype=np.uint8).reshape(
-            self.render_resolution[1], self.render_resolution[0], -1
-        )
+        return rgbaImg
```

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.8.3/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.8.3/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.8.3/PyFlyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.8.2
+Version: 0.8.3
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.8.2/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.8.3/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/pyproject.toml` & `PyFlyt-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.8.2/readme.md` & `PyFlyt-0.8.3/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.2/tests/test_core.py` & `PyFlyt-0.8.3/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,14 +110,22 @@
     # set to velocity control
     env.set_mode(6)
 
     # simulate for 1000 steps (1000/120 ~= 8 seconds)
     for i in range(100):
         env.step()
 
+        # check the camera image
+        assert isinstance(env.drones[0].rgbaImg, np.ndarray), f"Expected camera image to be of type `np.ndarray`, got {type(env.drones[0].rgbaImg)}."
+        assert isinstance(env.drones[0].depthImg, np.ndarray), f"Expected depth image to be of type `np.ndarray`, got {type(env.drones[0].depthImg)}."
+        assert isinstance(env.drones[0].segImg, np.ndarray), f"Expected segmented image to be of type `np.ndarray`, got {type(env.drones[0].segImg)}."
+        assert env.drones[0].rgbaImg.shape[-1] == 4, f"Expected 4 channels in the rendered image, got {env.drones[0].rgbaImg.shape[-1]}."
+        assert len(env.drones[0].depthImg.shape) == 2, f"Expected depth image to only have 2 dimensions, got {len(env.drones[0].depthImg.shape)}."
+        assert len(env.drones[0].segImg.shape) == 2, f"Expected segmented image to have only 2 dimensions, got {len(env.drones[0].segImg.shape)}"
+
     env.disconnect()
 
 
 def test_custom_controller():
     """Tests implementing a custom controller"""
 
     class CustomController(ControlClass):
```

### Comparing `PyFlyt-0.8.2/tests/test_gym_envs.py` & `PyFlyt-0.8.3/tests/test_gym_envs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests the API compatibility of all PyFlyt Envs."""
 import warnings
 
 import gymnasium as gym
 import pytest
 from gymnasium.error import Error
 from gymnasium.utils.env_checker import check_env, data_equivalence
+import numpy as np
 
 import PyFlyt.gym_envs
 
 _ALL_ENV_CONFIGS = []
 # quadx envs
 _ALL_ENV_CONFIGS.append(("PyFlyt/QuadX-Hover-v0", dict(angle_representation="euler")))
 _ALL_ENV_CONFIGS.append(
@@ -95,14 +96,15 @@
     ("PyFlyt/Rocket-Landing-v0", dict(angle_representation="quaternion"))
 )
 _ALL_ENV_CONFIGS.append(("PyFlyt/Rocket-Landing-v0", dict(sparse_reward=True)))
 
 CHECK_ENV_IGNORE_WARNINGS = [
     f"\x1b[33mWARN: {message}\x1b[0m"
     for message in [
+        "For Box action spaces, we recommend using a symmetric and normalized space (range=[-1, 1] or [0, 1]). See https://stable-baselines3.readthedocs.io/en/master/guide/rl_tips.html for more information.",
         "A Box observation space minimum value is -infinity. This is probably too low.",
         "A Box observation space maximum value is -infinity. This is probably too high.",
         "Human rendering should return `None`, got <class 'numpy.ndarray'>",
         "RGB-array rendering should return a numpy array in which the last axis has three dimensions, got 4",
     ]
 ]
 
@@ -156,8 +158,12 @@
     )
     env.reset()
     frames = []
     for _ in range(10):
         frames.append(env.render())
         env.step(env.action_space.sample())
 
+    for frame in frames:
+        assert isinstance(frame, np.ndarray), f"Expected render frames to be of type `np.ndarray`, got {type(frame)}."
+        assert frame.shape[-1] == 4, f"Expected 4 channels in the rendered image, got {frame.shape[-1]}."
+
     env.close()
```

