# Comparing `tmp/PyFlyt-0.8.3.tar.gz` & `tmp/PyFlyt-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.8.3.tar", last modified: Tue Jul 25 11:05:25 2023, max compression
+gzip compressed data, was "PyFlyt-0.8.4.tar", last modified: Tue Jul 25 14:43:24 2023, max compression
```

## Comparing `PyFlyt-0.8.3.tar` & `PyFlyt-0.8.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.901300 PyFlyt-0.8.3/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.8.3/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-25 11:05:25.901300 PyFlyt-0.8.3/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)      508 2023-07-25 11:03:32.000000 PyFlyt-0.8.3/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.8.3/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-12 22:54:11.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/base_wind_field.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12160 2023-07-19 16:05:50.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7560 2023-07-25 11:03:23.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-06-07 19:10:09.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-06-07 19:14:24.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-06-07 19:08:30.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.8.3/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-07-25 10:38:46.000000 PyFlyt-0.8.3/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.8.3/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-07-25 10:38:45.000000 PyFlyt-0.8.3/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-14 18:31:25.000000 PyFlyt-0.8.3/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/core/wind/
--rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.8.3/PyFlyt/core/wind/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9097 2023-07-25 10:48:05.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8831 2023-07-25 10:47:00.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3977 2023-07-19 17:39:31.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-05-29 18:39:28.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11470 2023-07-25 10:48:09.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-07-19 16:01:20.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.8.3/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.8.3/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.8.3/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.8.3/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1959 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-25 11:05:25.000000 PyFlyt-0.8.3/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1236 2023-07-25 11:05:18.000000 PyFlyt-0.8.3/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2421 2023-07-19 13:24:00.000000 PyFlyt-0.8.3/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-25 11:05:25.901300 PyFlyt-0.8.3/setup.cfg
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 11:05:25.897300 PyFlyt-0.8.3/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9520 2023-07-25 10:58:02.000000 PyFlyt-0.8.3/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5258 2023-07-25 10:51:05.000000 PyFlyt-0.8.3/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-06-30 13:35:00.000000 PyFlyt-0.8.4/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.848314 PyFlyt-0.8.4/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      592 2023-07-25 14:26:37.000000 PyFlyt-0.8.4/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.848314 PyFlyt-0.8.4/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-07 16:22:47.000000 PyFlyt-0.8.4/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-27 15:02:04.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-16 17:24:04.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12160 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-16 17:21:09.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7939 2023-07-25 14:21:42.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-02 11:06:46.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-05-16 17:31:41.000000 PyFlyt-0.8.4/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-11 16:33:17.000000 PyFlyt-0.8.4/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-16 17:13:33.000000 PyFlyt-0.8.4/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-16 17:12:54.000000 PyFlyt-0.8.4/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-16 17:14:09.000000 PyFlyt-0.8.4/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-02 11:06:46.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9224 2023-07-25 14:21:42.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8958 2023-07-25 14:23:04.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-21 13:48:00.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3977 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11598 2023-07-25 14:23:00.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-05-25 12:51:02.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-07 18:11:27.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-28 12:51:18.000000 PyFlyt-0.8.4/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-06-30 13:35:00.000000 PyFlyt-0.8.4/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-28 12:51:18.000000 PyFlyt-0.8.4/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.844314 PyFlyt-0.8.4/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-22 14:06:54.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-21 13:48:00.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-02 11:06:46.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-07 01:25:05.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-07 01:25:05.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-07 18:11:27.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-07 18:11:27.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.848314 PyFlyt-0.8.4/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1959 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1236 2023-07-25 14:43:12.000000 PyFlyt-0.8.4/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2421 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/setup.cfg
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9638 2023-07-25 14:35:24.000000 PyFlyt-0.8.4/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5304 2023-07-25 14:35:42.000000 PyFlyt-0.8.4/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.8.3/LICENSE.txt` & `PyFlyt-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PKG-INFO` & `PyFlyt-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.8.3
+Version: 0.8.4
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/camera.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,8 +158,18 @@
         _, _, rgbaImg, depthImg, segImg = self.p.getCameraImage(
             height=self.camera_resolution[0],
             width=self.camera_resolution[1],
             viewMatrix=self.view_mat,
             projectionMatrix=self.proj_mat,
         )
 
+        rgbaImg = np.asarray(rgbaImg).reshape(
+            self.camera_resolution[0], self.camera_resolution[1], -1
+        )
+        depthImg = np.asarray(depthImg).reshape(
+            self.camera_resolution[0], self.camera_resolution[1], -1
+        )
+        segImg = np.asarray(segImg).reshape(
+            self.camera_resolution[0], self.camera_resolution[1], -1
+        )
+
         return rgbaImg, depthImg, segImg
```

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.8.4/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/aviary.py` & `PyFlyt-0.8.4/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.8.4/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.8.4/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.8.4/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/core/load_objs.py` & `PyFlyt-0.8.4/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,8 +273,12 @@
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
             width=self.render_resolution[1],
             height=self.render_resolution[0],
             viewMatrix=self.env.drones[0].camera.view_mat,
             projectionMatrix=self.env.drones[0].camera.proj_mat,
         )
 
+        rgbaImg = np.asarray(rgbaImg).reshape(
+            self.render_resolution[0], self.render_resolution[1], -1
+        )
+
         return rgbaImg
```

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,8 +267,12 @@
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
             width=self.render_resolution[1],
             height=self.render_resolution[0],
             viewMatrix=self.camera_parameters[2],
             projectionMatrix=self.camera_parameters[3],
         )
 
+        rgbaImg = np.asarray(rgbaImg).reshape(
+            self.render_resolution[0], self.render_resolution[1], -1
+        )
+
         return rgbaImg
```

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,8 +328,13 @@
 
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
             width=self.render_resolution[1],
             height=self.render_resolution[0],
             viewMatrix=self.env.drones[0].camera.view_mat,
             projectionMatrix=self.env.drones[0].camera.proj_mat,
         )
+
+        rgbaImg = np.asarray(rgbaImg).reshape(
+            self.render_resolution[0], self.render_resolution[1], -1
+        )
+
         return rgbaImg
```

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.8.4/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.8.4/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.8.4/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.8.4/PyFlyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.8.3
+Version: 0.8.4
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.8.3/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.8.4/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/pyproject.toml` & `PyFlyt-0.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.8.3/readme.md` & `PyFlyt-0.8.4/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.3/tests/test_core.py` & `PyFlyt-0.8.4/tests/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,20 +111,32 @@
     env.set_mode(6)
 
     # simulate for 1000 steps (1000/120 ~= 8 seconds)
     for i in range(100):
         env.step()
 
         # check the camera image
-        assert isinstance(env.drones[0].rgbaImg, np.ndarray), f"Expected camera image to be of type `np.ndarray`, got {type(env.drones[0].rgbaImg)}."
-        assert isinstance(env.drones[0].depthImg, np.ndarray), f"Expected depth image to be of type `np.ndarray`, got {type(env.drones[0].depthImg)}."
-        assert isinstance(env.drones[0].segImg, np.ndarray), f"Expected segmented image to be of type `np.ndarray`, got {type(env.drones[0].segImg)}."
-        assert env.drones[0].rgbaImg.shape[-1] == 4, f"Expected 4 channels in the rendered image, got {env.drones[0].rgbaImg.shape[-1]}."
-        assert len(env.drones[0].depthImg.shape) == 2, f"Expected depth image to only have 2 dimensions, got {len(env.drones[0].depthImg.shape)}."
-        assert len(env.drones[0].segImg.shape) == 2, f"Expected segmented image to have only 2 dimensions, got {len(env.drones[0].segImg.shape)}"
+        assert isinstance(
+            env.drones[0].rgbaImg, np.ndarray
+        ), f"Expected camera image to be of type `np.ndarray`, got {type(env.drones[0].rgbaImg)}."
+        assert isinstance(
+            env.drones[0].depthImg, np.ndarray
+        ), f"Expected depth image to be of type `np.ndarray`, got {type(env.drones[0].depthImg)}."
+        assert isinstance(
+            env.drones[0].segImg, np.ndarray
+        ), f"Expected segmented image to be of type `np.ndarray`, got {type(env.drones[0].segImg)}."
+        assert (
+            env.drones[0].rgbaImg.shape[-1] == 4
+        ), f"Expected 4 channels in the rendered image, got {env.drones[0].rgbaImg.shape[-1]}."
+        assert (
+            env.drones[0].depthImg.shape[-1] == 1
+        ), f"Expected 1 channel in the depth image, got {env.drones[0].depthImg.shape[-1]}."
+        assert (
+            env.drones[0].segImg.shape[-1] == 1
+        ), f"Expected 1 channel in the segmentated image, got {env.drones[0].segImg.shape[-1]}"
 
     env.disconnect()
 
 
 def test_custom_controller():
     """Tests implementing a custom controller"""
```

### Comparing `PyFlyt-0.8.3/tests/test_gym_envs.py` & `PyFlyt-0.8.4/tests/test_gym_envs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests the API compatibility of all PyFlyt Envs."""
 import warnings
 
 import gymnasium as gym
+import numpy as np
 import pytest
 from gymnasium.error import Error
 from gymnasium.utils.env_checker import check_env, data_equivalence
-import numpy as np
 
 import PyFlyt.gym_envs
 
 _ALL_ENV_CONFIGS = []
 # quadx envs
 _ALL_ENV_CONFIGS.append(("PyFlyt/QuadX-Hover-v0", dict(angle_representation="euler")))
 _ALL_ENV_CONFIGS.append(
@@ -159,11 +159,15 @@
     env.reset()
     frames = []
     for _ in range(10):
         frames.append(env.render())
         env.step(env.action_space.sample())
 
     for frame in frames:
-        assert isinstance(frame, np.ndarray), f"Expected render frames to be of type `np.ndarray`, got {type(frame)}."
-        assert frame.shape[-1] == 4, f"Expected 4 channels in the rendered image, got {frame.shape[-1]}."
+        assert isinstance(
+            frame, np.ndarray
+        ), f"Expected render frames to be of type `np.ndarray`, got {type(frame)}."
+        assert (
+            frame.shape[-1] == 4
+        ), f"Expected 4 channels in the rendered image, got {frame.shape[-1]}."
 
     env.close()
```

