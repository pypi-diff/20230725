# Comparing `tmp/eagerx_franka-0.0.3.tar.gz` & `tmp/eagerx_franka-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagerx_franka-0.0.3.tar", max compression
+gzip compressed data, was "eagerx_franka-0.0.4.tar", max compression
```

## Comparing `eagerx_franka-0.0.3.tar` & `eagerx_franka-0.0.4.tar`

### file list

```diff
@@ -1,90 +1,89 @@
--rw-r--r--   0        0        0    11357 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/LICENSE
--rw-r--r--   0        0        0      586 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/calibrations/logitech_c170.yaml
--rw-r--r--   0        0        0      684 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/calibrations/logitech_c920.yaml
--rw-r--r--   0        0        0     2222 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_description.launch
--rw-r--r--   0        0        0    10172 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_panda/LICENSE.txt
--rw-r--r--   0        0        0     7603 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/finger.obj
--rw-r--r--   0        0        0    15247 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/hand.obj
--rw-r--r--   0        0        0    14925 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link0.obj
--rw-r--r--   0        0        0    22976 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link1.obj
--rw-r--r--   0        0        0    22688 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link2.obj
--rw-r--r--   0        0        0    22870 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link3.obj
--rw-r--r--   0        0        0    68016 2023-02-09 13:24:12.759099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link4.obj
--rw-r--r--   0        0        0    67745 2023-02-09 13:24:12.763099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link5.obj
--rw-r--r--   0        0        0     3827 2023-02-09 13:24:12.763099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link6.mtl
--rw-r--r--   0        0        0   140218 2023-02-09 13:24:12.763099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link6.obj
--rw-r--r--   0        0        0    45132 2023-02-09 13:24:12.763099 eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link7.obj
--rw-r--r--   0        0        0    33337 2023-02-09 13:24:12.763099 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/colors.png
--rw-r--r--   0        0        0      481 2023-02-09 13:24:12.763099 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/finger.mtl
--rw-r--r--   0        0        0    65359 2023-02-09 13:24:12.763099 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/finger.obj
--rw-r--r--   0        0        0     1132 2023-02-09 13:24:12.763099 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/hand.mtl
--rw-r--r--   0        0        0   713204 2023-02-09 13:24:12.767099 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/hand.obj
--rw-r--r--   0        0        0      262 2023-02-09 13:24:12.767099 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link1.mtl
--rw-r--r--   0        0        0  1070650 2023-02-09 13:24:12.771099 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link1.obj
--rw-r--r--   0        0        0      261 2023-02-09 13:24:12.771099 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link2.mtl
--rw-r--r--   0        0        0  1084458 2023-02-09 13:24:12.779100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link2.obj
--rw-r--r--   0        0        0      931 2023-02-09 13:24:12.779100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link3.mtl
--rw-r--r--   0        0        0  1237175 2023-02-09 13:24:12.783100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link3.obj
--rw-r--r--   0        0        0      925 2023-02-09 13:24:12.783100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link4.mtl
--rw-r--r--   0        0        0  1272305 2023-02-09 13:24:12.791100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link4.obj
--rw-r--r--   0        0        0      676 2023-02-09 13:24:12.791100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link5.mtl
--rw-r--r--   0        0        0  1582192 2023-02-09 13:24:12.795100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link5.obj
--rw-r--r--   0        0        0     3552 2023-02-09 13:24:12.795100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link6.mtl
--rw-r--r--   0        0        0  2236857 2023-02-09 13:24:12.807100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link6.obj
--rw-r--r--   0        0        0    26999 2023-02-09 13:24:12.807100 eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/visualShapeBench.json_0.json
--rw-r--r--   0        0        0    11263 2023-02-09 13:24:12.807100 eagerx_franka-0.0.3/assets/franka_panda/panda.urdf
--rw-r--r--   0        0        0    10084 2023-02-09 13:24:12.807100 eagerx_franka-0.0.3/assets/meshes/collision/hand.stl
--rw-r--r--   0        0        0    10084 2023-02-09 13:24:12.807100 eagerx_franka-0.0.3/assets/meshes/collision/link0.stl
--rw-r--r--   0        0        0    15084 2023-02-09 13:24:12.807100 eagerx_franka-0.0.3/assets/meshes/collision/link1.stl
--rw-r--r--   0        0        0    15084 2023-02-09 13:24:12.807100 eagerx_franka-0.0.3/assets/meshes/collision/link2.stl
--rw-r--r--   0        0        0    15084 2023-02-09 13:24:12.807100 eagerx_franka-0.0.3/assets/meshes/collision/link3.stl
--rw-r--r--   0        0        0    15084 2023-02-09 13:24:12.811100 eagerx_franka-0.0.3/assets/meshes/collision/link4.stl
--rw-r--r--   0        0        0    15084 2023-02-09 13:24:12.811100 eagerx_franka-0.0.3/assets/meshes/collision/link5.stl
--rw-r--r--   0        0        0    10084 2023-02-09 13:24:12.811100 eagerx_franka-0.0.3/assets/meshes/collision/link6.stl
--rw-r--r--   0        0        0    10084 2023-02-09 13:24:12.811100 eagerx_franka-0.0.3/assets/meshes/collision/link7.stl
--rw-r--r--   0        0        0    51239 2023-02-09 13:24:12.811100 eagerx_franka-0.0.3/assets/meshes/visual/finger.dae
--rw-r--r--   0        0        0   549239 2023-02-09 13:24:12.811100 eagerx_franka-0.0.3/assets/meshes/visual/hand.dae
--rw-r--r--   0        0        0  1591592 2023-02-09 13:24:12.819100 eagerx_franka-0.0.3/assets/meshes/visual/link0.dae
--rw-r--r--   0        0        0   978473 2023-02-09 13:24:12.827101 eagerx_franka-0.0.3/assets/meshes/visual/link1.dae
--rw-r--r--   0        0        0   998544 2023-02-09 13:24:12.831101 eagerx_franka-0.0.3/assets/meshes/visual/link2.dae
--rw-r--r--   0        0        0  1099883 2023-02-09 13:24:12.835101 eagerx_franka-0.0.3/assets/meshes/visual/link3.dae
--rw-r--r--   0        0        0  1145723 2023-02-09 13:24:12.843101 eagerx_franka-0.0.3/assets/meshes/visual/link4.dae
--rw-r--r--   0        0        0  1438343 2023-02-09 13:24:12.851101 eagerx_franka-0.0.3/assets/meshes/visual/link5.dae
--rw-r--r--   0        0        0  1728753 2023-02-09 13:24:12.859101 eagerx_franka-0.0.3/assets/meshes/visual/link6.dae
--rw-r--r--   0        0        0   936416 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/meshes/visual/link7.dae
--rw-r--r--   0        0        0     6379 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/common/franka_arm.xacro
--rw-r--r--   0        0        0     4485 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/common/franka_hand.xacro
--rw-r--r--   0        0        0     5279 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/common/franka_robot.xacro
--rw-r--r--   0        0        0      305 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/common/hand.urdf.xacro
--rw-r--r--   0        0        0     2443 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/common/inertial.yaml
--rw-r--r--   0        0        0    12461 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/common/utils.xacro
--rw-r--r--   0        0        0     1561 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/dual_panda/dual_panda_example.urdf.xacro
--rw-r--r--   0        0        0      434 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/fr3/fr3.urdf.xacro
--rw-r--r--   0        0        0      736 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/fr3/joint_limits.yaml
--rw-r--r--   0        0        0      748 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/panda/joint_limits.yaml
--rw-r--r--   0        0        0      440 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/assets/robots/panda/panda.urdf.xacro
--rw-r--r--   0        0        0       22 2023-02-09 13:24:24.099361 eagerx_franka-0.0.3/eagerx_franka/__init__.py
--rw-r--r--   0        0        0     5399 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/env.py
--rw-r--r--   0        0        0        0 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/franka_arm/__init__.py
--rw-r--r--   0        0        0    10386 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/franka_arm/franka_arm.py
--rw-r--r--   0        0        0     1108 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/franka_arm/mr_descriptions.py
--rw-r--r--   0        0        0      784 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/franka_arm/processor.py
--rw-r--r--   0        0        0        0 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/franka_arm/pybullet/__init__.py
--rw-r--r--   0        0        0     2598 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/franka_arm/pybullet/enginestates.py
--rw-r--r--   0        0        0     4853 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/goal_env.py
--rw-r--r--   0        0        0        0 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/ik/__init__.py
--rw-r--r--   0        0        0     8643 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/ik/node.py
--rw-r--r--   0        0        0        0 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/solid/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/__init__.py
--rw-r--r--   0        0        0   252184 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/bolt.stl
--rw-r--r--   0        0        0      988 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/bolt.urdf
--rw-r--r--   0        0        0      924 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/box.urdf
--rw-r--r--   0        0        0      311 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/box_goal.urdf
--rw-r--r--   0        0        0      956 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/can.urdf
--rw-r--r--   0        0        0      352 2023-02-09 13:24:12.863102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/can_goal.urdf
--rw-r--r--   0        0        0   191984 2023-02-09 13:24:12.867102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/nut.stl
--rw-r--r--   0        0        0      986 2023-02-09 13:24:12.867102 eagerx_franka-0.0.3/eagerx_franka/solid/assets/nut.urdf
--rw-r--r--   0        0        0     1312 2023-02-09 13:24:12.867102 eagerx_franka-0.0.3/eagerx_franka/utils.py
--rw-r--r--   0        0        0     1195 2023-02-09 13:24:24.099361 eagerx_franka-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 eagerx_franka-0.0.3/setup.py
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 eagerx_franka-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/LICENSE
+-rw-r--r--   0        0        0      586 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/calibrations/logitech_c170.yaml
+-rw-r--r--   0        0        0      684 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/calibrations/logitech_c920.yaml
+-rw-r--r--   0        0        0     2222 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/franka_description.launch
+-rw-r--r--   0        0        0    10172 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/franka_panda/LICENSE.txt
+-rw-r--r--   0        0        0     7603 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/finger.obj
+-rw-r--r--   0        0        0    15247 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/hand.obj
+-rw-r--r--   0        0        0    14925 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link0.obj
+-rw-r--r--   0        0        0    22976 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link1.obj
+-rw-r--r--   0        0        0    22688 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link2.obj
+-rw-r--r--   0        0        0    22870 2023-07-25 09:52:49.089141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link3.obj
+-rw-r--r--   0        0        0    68016 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link4.obj
+-rw-r--r--   0        0        0    67745 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link5.obj
+-rw-r--r--   0        0        0     3827 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link6.mtl
+-rw-r--r--   0        0        0   140218 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link6.obj
+-rw-r--r--   0        0        0    45132 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link7.obj
+-rw-r--r--   0        0        0    33337 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/colors.png
+-rw-r--r--   0        0        0      481 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/finger.mtl
+-rw-r--r--   0        0        0    65359 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/finger.obj
+-rw-r--r--   0        0        0     1132 2023-07-25 09:52:49.093141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/hand.mtl
+-rw-r--r--   0        0        0   713204 2023-07-25 09:52:49.097141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/hand.obj
+-rw-r--r--   0        0        0      262 2023-07-25 09:52:49.097141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link1.mtl
+-rw-r--r--   0        0        0  1070650 2023-07-25 09:52:49.105141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link1.obj
+-rw-r--r--   0        0        0      261 2023-07-25 09:52:49.105141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link2.mtl
+-rw-r--r--   0        0        0  1084458 2023-07-25 09:52:49.109141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link2.obj
+-rw-r--r--   0        0        0      931 2023-07-25 09:52:49.109141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link3.mtl
+-rw-r--r--   0        0        0  1237175 2023-07-25 09:52:49.117141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link3.obj
+-rw-r--r--   0        0        0      925 2023-07-25 09:52:49.117141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link4.mtl
+-rw-r--r--   0        0        0  1272305 2023-07-25 09:52:49.121141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link4.obj
+-rw-r--r--   0        0        0      676 2023-07-25 09:52:49.121141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link5.mtl
+-rw-r--r--   0        0        0  1582192 2023-07-25 09:52:49.129141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link5.obj
+-rw-r--r--   0        0        0     3552 2023-07-25 09:52:49.129141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link6.mtl
+-rw-r--r--   0        0        0  2236857 2023-07-25 09:52:49.141141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link6.obj
+-rw-r--r--   0        0        0    26999 2023-07-25 09:52:49.141141 eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/visualShapeBench.json_0.json
+-rw-r--r--   0        0        0    11431 2023-07-25 09:52:49.141141 eagerx_franka-0.0.4/assets/franka_panda/panda.urdf
+-rw-r--r--   0        0        0    10084 2023-07-25 09:52:49.141141 eagerx_franka-0.0.4/assets/meshes/collision/hand.stl
+-rw-r--r--   0        0        0    10084 2023-07-25 09:52:49.141141 eagerx_franka-0.0.4/assets/meshes/collision/link0.stl
+-rw-r--r--   0        0        0    15084 2023-07-25 09:52:49.141141 eagerx_franka-0.0.4/assets/meshes/collision/link1.stl
+-rw-r--r--   0        0        0    15084 2023-07-25 09:52:49.141141 eagerx_franka-0.0.4/assets/meshes/collision/link2.stl
+-rw-r--r--   0        0        0    15084 2023-07-25 09:52:49.141141 eagerx_franka-0.0.4/assets/meshes/collision/link3.stl
+-rw-r--r--   0        0        0    15084 2023-07-25 09:52:49.145141 eagerx_franka-0.0.4/assets/meshes/collision/link4.stl
+-rw-r--r--   0        0        0    15084 2023-07-25 09:52:49.145141 eagerx_franka-0.0.4/assets/meshes/collision/link5.stl
+-rw-r--r--   0        0        0    10084 2023-07-25 09:52:49.145141 eagerx_franka-0.0.4/assets/meshes/collision/link6.stl
+-rw-r--r--   0        0        0    10084 2023-07-25 09:52:49.145141 eagerx_franka-0.0.4/assets/meshes/collision/link7.stl
+-rw-r--r--   0        0        0    51239 2023-07-25 09:52:49.145141 eagerx_franka-0.0.4/assets/meshes/visual/finger.dae
+-rw-r--r--   0        0        0   549239 2023-07-25 09:52:49.145141 eagerx_franka-0.0.4/assets/meshes/visual/hand.dae
+-rw-r--r--   0        0        0  1591592 2023-07-25 09:52:49.157141 eagerx_franka-0.0.4/assets/meshes/visual/link0.dae
+-rw-r--r--   0        0        0   978473 2023-07-25 09:52:49.161141 eagerx_franka-0.0.4/assets/meshes/visual/link1.dae
+-rw-r--r--   0        0        0   998544 2023-07-25 09:52:49.169141 eagerx_franka-0.0.4/assets/meshes/visual/link2.dae
+-rw-r--r--   0        0        0  1099883 2023-07-25 09:52:49.173141 eagerx_franka-0.0.4/assets/meshes/visual/link3.dae
+-rw-r--r--   0        0        0  1145723 2023-07-25 09:52:49.181141 eagerx_franka-0.0.4/assets/meshes/visual/link4.dae
+-rw-r--r--   0        0        0  1438343 2023-07-25 09:52:49.189141 eagerx_franka-0.0.4/assets/meshes/visual/link5.dae
+-rw-r--r--   0        0        0  1728753 2023-07-25 09:52:49.197141 eagerx_franka-0.0.4/assets/meshes/visual/link6.dae
+-rw-r--r--   0        0        0   936416 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/meshes/visual/link7.dae
+-rw-r--r--   0        0        0     6379 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/common/franka_arm.xacro
+-rw-r--r--   0        0        0     4485 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/common/franka_hand.xacro
+-rw-r--r--   0        0        0     5279 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/common/franka_robot.xacro
+-rw-r--r--   0        0        0      305 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/common/hand.urdf.xacro
+-rw-r--r--   0        0        0     2443 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/common/inertial.yaml
+-rw-r--r--   0        0        0    12461 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/common/utils.xacro
+-rw-r--r--   0        0        0     1561 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/dual_panda/dual_panda_example.urdf.xacro
+-rw-r--r--   0        0        0      434 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/fr3/fr3.urdf.xacro
+-rw-r--r--   0        0        0      736 2023-07-25 09:52:49.201140 eagerx_franka-0.0.4/assets/robots/fr3/joint_limits.yaml
+-rw-r--r--   0        0        0      748 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/assets/robots/panda/joint_limits.yaml
+-rw-r--r--   0        0        0      440 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/assets/robots/panda/panda.urdf.xacro
+-rw-r--r--   0        0        0       22 2023-07-25 09:53:00.293079 eagerx_franka-0.0.4/eagerx_franka/__init__.py
+-rw-r--r--   0        0        0     7937 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/env.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/franka_arm/__init__.py
+-rw-r--r--   0        0        0    10386 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/franka_arm/franka_arm.py
+-rw-r--r--   0        0        0     1108 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/franka_arm/mr_descriptions.py
+-rw-r--r--   0        0        0      784 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/franka_arm/processor.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/franka_arm/pybullet/__init__.py
+-rw-r--r--   0        0        0     2598 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/franka_arm/pybullet/enginestates.py
+-rw-r--r--   0        0        0     6116 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/goal_env.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/ik/__init__.py
+-rw-r--r--   0        0        0     8809 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/ik/node.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/__init__.py
+-rw-r--r--   0        0        0   252184 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/bolt.stl
+-rw-r--r--   0        0        0      988 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/bolt.urdf
+-rw-r--r--   0        0        0      924 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/box.urdf
+-rw-r--r--   0        0        0      311 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/box_goal.urdf
+-rw-r--r--   0        0        0      956 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/can.urdf
+-rw-r--r--   0        0        0      352 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/can_goal.urdf
+-rw-r--r--   0        0        0   191984 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/nut.stl
+-rw-r--r--   0        0        0      986 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/solid/assets/nut.urdf
+-rw-r--r--   0        0        0     1652 2023-07-25 09:52:49.205140 eagerx_franka-0.0.4/eagerx_franka/utils.py
+-rw-r--r--   0        0        0     1071 2023-07-25 09:53:00.293079 eagerx_franka-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 eagerx_franka-0.0.4/PKG-INFO
```

### Comparing `eagerx_franka-0.0.3/LICENSE` & `eagerx_franka-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/calibrations/logitech_c170.yaml` & `eagerx_franka-0.0.4/assets/calibrations/logitech_c170.yaml`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/calibrations/logitech_c920.yaml` & `eagerx_franka-0.0.4/assets/calibrations/logitech_c920.yaml`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_description.launch` & `eagerx_franka-0.0.4/assets/franka_description.launch`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/LICENSE.txt` & `eagerx_franka-0.0.4/assets/franka_panda/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/finger.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/finger.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/hand.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/hand.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link0.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link0.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link1.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link1.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link2.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link2.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link3.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link3.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link4.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link4.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link5.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link5.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link6.mtl` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link6.mtl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link6.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link6.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/collision/link7.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/collision/link7.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/colors.png` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/colors.png`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/finger.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/finger.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/hand.mtl` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/hand.mtl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/hand.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/hand.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link1.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link1.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link2.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link2.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link3.mtl` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link3.mtl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link3.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link3.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link4.mtl` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link4.mtl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link4.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link4.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link5.mtl` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link5.mtl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link5.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link5.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link6.mtl` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link6.mtl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/link6.obj` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/link6.obj`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/meshes/visual/visualShapeBench.json_0.json` & `eagerx_franka-0.0.4/assets/franka_panda/meshes/visual/visualShapeBench.json_0.json`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/franka_panda/panda.urdf` & `eagerx_franka-0.0.4/assets/franka_panda/panda.urdf`

 * *Files 12% similar despite different names*

#### Comparing `eagerx_franka-0.0.3/assets/franka_panda/panda.urdf` & `eagerx_franka-0.0.4/assets/franka_panda/panda.urdf`

```diff
@@ -18,15 +18,15 @@
         <color rgba="1. 1. 1. 1."/>
       </material>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/link0.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <link name="panda_link1">
     <inertial>
       <origin rpy="0 0 0" xyz="0 -0.04 -0.05"/>
       <mass value="2.7"/>
       <inertia ixx="0.1" ixy="0" ixz="0" iyy="0.1" iyz="0" izz="0.1"/>
@@ -37,15 +37,15 @@
       </geometry>
       <material name="panda_white"/>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/link1.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <joint name="panda_joint1" type="revolute">
     <safety_controller k_position="100.0" k_velocity="40.0" soft_lower_limit="-2.8973" soft_upper_limit="2.8973"/>
     <origin rpy="0 0 0" xyz="0 0 0.333"/>
     <parent link="panda_link0"/>
     <child link="panda_link1"/>
@@ -64,15 +64,15 @@
       </geometry>
       <material name="panda_white"/>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/link2.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <joint name="panda_joint2" type="revolute">
     <safety_controller k_position="100.0" k_velocity="40.0" soft_lower_limit="-1.7628" soft_upper_limit="1.7628"/>
     <origin rpy="-1.57079632679 0 0" xyz="0 0 0"/>
     <parent link="panda_link1"/>
     <child link="panda_link2"/>
@@ -119,15 +119,15 @@
       </geometry>
       <material name="panda_white"/>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/link4.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <joint name="panda_joint4" type="revolute">
     <safety_controller k_position="100.0" k_velocity="40.0" soft_lower_limit="-3.0718" soft_upper_limit="-0.0698"/>
     <origin rpy="1.57079632679 0 0" xyz="0.0825 0 0"/>
     <parent link="panda_link3"/>
     <child link="panda_link4"/>
@@ -146,15 +146,15 @@
       </geometry>
       <material name="panda_white"/>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/link5.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <joint name="panda_joint5" type="revolute">
     <safety_controller k_position="100.0" k_velocity="40.0" soft_lower_limit="-2.8973" soft_upper_limit="2.8973"/>
     <origin rpy="-1.57079632679 0 0" xyz="-0.0825 0.384 0"/>
     <parent link="panda_link4"/>
     <child link="panda_link5"/>
@@ -173,15 +173,15 @@
       </geometry>
       <material name="panda_white"/>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/link6.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <joint name="panda_joint6" type="revolute">
     <safety_controller k_position="100.0" k_velocity="40.0" soft_lower_limit="-0.0175" soft_upper_limit="3.7525"/>
     <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
     <parent link="panda_link5"/>
     <child link="panda_link6"/>
@@ -200,15 +200,15 @@
       </geometry>
       <material name="panda_white"/>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/link7.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <joint name="panda_joint7" type="revolute">
     <safety_controller k_position="100.0" k_velocity="40.0" soft_lower_limit="-2.8973" soft_upper_limit="2.8973"/>
     <origin rpy="1.57079632679 0 0" xyz="0.088 0 0"/>
     <parent link="panda_link6"/>
     <child link="panda_link7"/>
@@ -245,25 +245,25 @@
       </geometry>
       <material name="panda_white"/>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/hand.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <link name="panda_leftfinger">
-    <contact>
-      <friction_anchor/>
-      <stiffness value="30000.0"/>
-      <damping value="1000.0"/>
-      <spinning_friction value="0.1"/>
-      <lateral_friction value="1.0"/>
-    </contact>
+    <!--       <contact>-->
+    <!--      <friction_anchor/>-->
+    <!--      <stiffness value="30000.0"/>-->
+    <!--      <damping value="1000.0"/>-->
+    <!--      <spinning_friction value="0.1"/>-->
+    <!--      <lateral_friction value="1.0"/>-->
+    <!--    </contact>-->
     <inertial>
       <origin rpy="0 0 0" xyz="0 0.01 0.02"/>
       <mass value="0.1"/>
       <inertia ixx="0.1" ixy="0" ixz="0" iyy="0.1" iyz="0" izz="0.1"/>
     </inertial>
     <visual>
       <geometry>
@@ -271,25 +271,25 @@
       </geometry>
       <material name="panda_white"/>
     </visual>
     <collision>
       <geometry>
         <mesh filename="package://meshes/collision/finger.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <link name="panda_rightfinger">
-    <contact>
-      <friction_anchor/>
-      <stiffness value="30000.0"/>
-      <damping value="1000.0"/>
-      <spinning_friction value="0.1"/>
-      <lateral_friction value="1.0"/>
-    </contact>
+    <!--        <contact>-->
+    <!--      <friction_anchor/>-->
+    <!--      <stiffness value="30000.0"/>-->
+    <!--      <damping value="1000.0"/>-->
+    <!--      <spinning_friction value="0.1"/>-->
+    <!--      <lateral_friction value="1.0"/>-->
+    <!--    </contact>-->
     <inertial>
       <origin rpy="0 0 0" xyz="0 -0.01 0.02"/>
       <mass value="0.1"/>
       <inertia ixx="0.1" ixy="0" ixz="0" iyy="0.1" iyz="0" izz="0.1"/>
     </inertial>
     <visual>
       <origin rpy="0 0 3.14159265359" xyz="0 0 0"/>
@@ -299,15 +299,15 @@
       <material name="panda_white"/>
     </visual>
     <collision>
       <origin rpy="0 0 3.14159265359" xyz="0 0 0"/>
       <geometry>
         <mesh filename="package://meshes/collision/finger.obj"/>
       </geometry>
-      <material name="panda_white"/>
+      <!--      <material name="panda_white"/>-->
     </collision>
   </link>
   <joint name="panda_finger_joint1" type="prismatic">
     <parent link="panda_hand"/>
     <child link="panda_leftfinger"/>
     <origin rpy="0 0 0" xyz="0 0 0.0584"/>
     <axis xyz="0 1 0"/>
```

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/hand.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/hand.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/link0.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/link0.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/link1.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/link1.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/link2.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/link2.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/link3.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/link3.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/link4.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/link4.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/link5.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/link5.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/link6.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/link6.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/collision/link7.stl` & `eagerx_franka-0.0.4/assets/meshes/collision/link7.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/finger.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/finger.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/hand.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/hand.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/link0.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/link0.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/link1.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/link1.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/link2.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/link2.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/link3.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/link3.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/link4.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/link4.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/link5.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/link5.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/link6.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/link6.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/meshes/visual/link7.dae` & `eagerx_franka-0.0.4/assets/meshes/visual/link7.dae`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/robots/common/franka_arm.xacro` & `eagerx_franka-0.0.4/assets/robots/common/franka_arm.xacro`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/robots/common/franka_hand.xacro` & `eagerx_franka-0.0.4/assets/robots/common/franka_hand.xacro`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/robots/common/franka_robot.xacro` & `eagerx_franka-0.0.4/assets/robots/common/franka_robot.xacro`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/robots/common/inertial.yaml` & `eagerx_franka-0.0.4/assets/robots/common/inertial.yaml`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/robots/common/utils.xacro` & `eagerx_franka-0.0.4/assets/robots/common/utils.xacro`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/robots/dual_panda/dual_panda_example.urdf.xacro` & `eagerx_franka-0.0.4/assets/robots/dual_panda/dual_panda_example.urdf.xacro`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/robots/fr3/joint_limits.yaml` & `eagerx_franka-0.0.4/assets/robots/fr3/joint_limits.yaml`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/assets/robots/panda/joint_limits.yaml` & `eagerx_franka-0.0.4/assets/robots/panda/joint_limits.yaml`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/franka_arm/franka_arm.py` & `eagerx_franka-0.0.4/eagerx_franka/franka_arm/franka_arm.py`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/franka_arm/mr_descriptions.py` & `eagerx_franka-0.0.4/eagerx_franka/franka_arm/mr_descriptions.py`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/franka_arm/processor.py` & `eagerx_franka-0.0.4/eagerx_franka/franka_arm/processor.py`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/franka_arm/pybullet/enginestates.py` & `eagerx_franka-0.0.4/eagerx_franka/franka_arm/pybullet/enginestates.py`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/ik/node.py` & `eagerx_franka-0.0.4/eagerx_franka/ik/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import typing as t
 import numpy as np
 import eagerx
 from eagerx import Space
 from eagerx.core.specs import NodeSpec
 import eagerx.core.register as register
 from eagerx.utils.utils import Msg
-import roboticstoolbox as rtb
-from spatialmath import SE3
+
+# import roboticstoolbox as rtb
+# from spatialmath import SE3
 from scipy.spatial.transform import Rotation as R
 import modern_robotics as mr
 
 
 class EndEffectorDownward(eagerx.Node):
     @classmethod
     def make(
@@ -129,91 +130,93 @@
         else:
             # self.backend.logwarn("no solution")
             target = current
             dtarget = current * 0
         return dict(target=target, dtarget=dtarget)
 
 
-class PandaEndEffectorDownward(eagerx.Node):
-    @classmethod
-    def make(
-        cls,
-        name: str,
-        rate: float,
-        max_dxyz: t.List[float],
-        max_dyaw: float,
-        min_z: float = 0.03,
-        process: int = eagerx.NEW_PROCESS,
-    ) -> NodeSpec:
-        """
-        Calculate desired joint positions based on delta pose of the end effector in task space using inverse kinematics.
-
-        :param name: Node name.
-        :param rate: Rate at which callback is called.
-        :param max_dxyz: Maximum delta position in xyz [m/s].
-        :param max_dyaw: Maximum delta rotation in yaw [rad/s].
-        :param min_z: Minimum z position of the end-effector's link (cog?) [m].
-        :param process: {0: NEW_PROCESS, 1: ENVIRONMENT, 2: ENGINE, 3: EXTERNAL}.
-        :return: Parameter specification of the node.
-        """
-        spec = cls.get_specification()
-
-        # Modify default node params
-        spec.config.name = name
-        spec.config.rate = rate
-        spec.config.process = process
-        spec.config.inputs = ["dxyz", "dyaw", "current", "xyz", "orn"]
-        spec.config.outputs = ["target", "dtarget"]
-
-        # Modify custom node params
-        spec.config.max_dxyz = max_dxyz
-        spec.config.max_dyaw = max_dyaw
-        spec.config.min_z = min_z
-
-        # Add converter & space
-        spec.inputs.dxyz.space.update(low=[-i for i in max_dxyz], high=max_dxyz)
-        spec.inputs.dyaw.space.update(low=-max_dyaw, high=max_dyaw)
-        return spec
-
-    def initialize(self, spec: NodeSpec):
-        np.set_printoptions(precision=2, suppress=True)
-        self.max_dxyz = np.array(spec.config.max_dxyz, dtype="float32")
-        self.max_dyaw = np.array(spec.config.max_dyaw, dtype="float32")
-        self.min_z = spec.config.min_z
-        self.robot = rtb.models.Panda()
-
-    @register.states()
-    def reset(self):
-        pass
-
-    @register.inputs(
-        dxyz=Space(shape=(3,), dtype="float32"),
-        xyz=Space(shape=(3,), dtype="float32"),
-        orn=Space(shape=(4,), dtype="float32"),
-        dyaw=Space(shape=(), dtype="float32"),
-        current=Space(dtype="float32"),
-    )
-    @register.outputs(target=Space(dtype="float32"), dtarget=Space(dtype="float32"))
-    def callback(self, t_n: float, dxyz: Msg, xyz: Msg, orn: Msg, dyaw: Msg, current: Msg):
-        dxyz = dxyz.msgs[-1]
-        xyz = xyz.msgs[-1]
-        orn = orn.msgs[-1]
-        dyaw = dyaw.msgs[-1]
-        current = current.msgs[-1]
-
-        # Limit dz
-        dz = dxyz[-1]
-        z = xyz[-1]
-        dxyz[-1] = max(dz, self.max_dxyz[-1] * (-1 + 1 / np.exp(max(0, 10 * (z - self.min_z)))))
-
-        # Calculate the target pose
-        rot_ee2b = R.from_quat(orn).as_matrix()
-        yaw = np.arctan2(rot_ee2b[0, 1], rot_ee2b[0, 0])
-        yaw_target = (yaw + dyaw / self.rate) % (2 * np.pi)
-
-        trans = xyz + dxyz / self.rate  # Scale delta position with rate
-
-        tep = SE3.Trans(trans) * SE3.RPY(yaw_target, np.pi, 0, order="zyx")
-        sol = self.robot.ik_lm_chan(tep)
-        target = np.asarray(sol[0], dtype="float32")
-        dtarget = (target - current) * self.rate  # [rad/sec]
-        return dict(target=target, dtarget=dtarget)
+#
+#
+# class PandaEndEffectorDownward(eagerx.Node):
+#     @classmethod
+#     def make(
+#         cls,
+#         name: str,
+#         rate: float,
+#         max_dxyz: t.List[float],
+#         max_dyaw: float,
+#         min_z: float = 0.03,
+#         process: int = eagerx.NEW_PROCESS,
+#     ) -> NodeSpec:
+#         """
+#         Calculate desired joint positions based on delta pose of the end effector in task space using inverse kinematics.
+#
+#         :param name: Node name.
+#         :param rate: Rate at which callback is called.
+#         :param max_dxyz: Maximum delta position in xyz [m/s].
+#         :param max_dyaw: Maximum delta rotation in yaw [rad/s].
+#         :param min_z: Minimum z position of the end-effector's link (cog?) [m].
+#         :param process: {0: NEW_PROCESS, 1: ENVIRONMENT, 2: ENGINE, 3: EXTERNAL}.
+#         :return: Parameter specification of the node.
+#         """
+#         spec = cls.get_specification()
+#
+#         # Modify default node params
+#         spec.config.name = name
+#         spec.config.rate = rate
+#         spec.config.process = process
+#         spec.config.inputs = ["dxyz", "dyaw", "current", "xyz", "orn"]
+#         spec.config.outputs = ["target", "dtarget"]
+#
+#         # Modify custom node params
+#         spec.config.max_dxyz = max_dxyz
+#         spec.config.max_dyaw = max_dyaw
+#         spec.config.min_z = min_z
+#
+#         # Add converter & space
+#         spec.inputs.dxyz.space.update(low=[-i for i in max_dxyz], high=max_dxyz)
+#         spec.inputs.dyaw.space.update(low=-max_dyaw, high=max_dyaw)
+#         return spec
+#
+#     def initialize(self, spec: NodeSpec):
+#         np.set_printoptions(precision=2, suppress=True)
+#         self.max_dxyz = np.array(spec.config.max_dxyz, dtype="float32")
+#         self.max_dyaw = np.array(spec.config.max_dyaw, dtype="float32")
+#         self.min_z = spec.config.min_z
+#         self.robot = rtb.models.Panda()
+#
+#     @register.states()
+#     def reset(self):
+#         pass
+#
+#     @register.inputs(
+#         dxyz=Space(shape=(3,), dtype="float32"),
+#         xyz=Space(shape=(3,), dtype="float32"),
+#         orn=Space(shape=(4,), dtype="float32"),
+#         dyaw=Space(shape=(), dtype="float32"),
+#         current=Space(dtype="float32"),
+#     )
+#     @register.outputs(target=Space(dtype="float32"), dtarget=Space(dtype="float32"))
+#     def callback(self, t_n: float, dxyz: Msg, xyz: Msg, orn: Msg, dyaw: Msg, current: Msg):
+#         dxyz = dxyz.msgs[-1]
+#         xyz = xyz.msgs[-1]
+#         orn = orn.msgs[-1]
+#         dyaw = dyaw.msgs[-1]
+#         current = current.msgs[-1]
+#
+#         # Limit dz
+#         dz = dxyz[-1]
+#         z = xyz[-1]
+#         dxyz[-1] = max(dz, self.max_dxyz[-1] * (-1 + 1 / np.exp(max(0, 10 * (z - self.min_z)))))
+#
+#         # Calculate the target pose
+#         rot_ee2b = R.from_quat(orn).as_matrix()
+#         yaw = np.arctan2(rot_ee2b[0, 1], rot_ee2b[0, 0])
+#         yaw_target = (yaw + dyaw / self.rate) % (2 * np.pi)
+#
+#         trans = xyz + dxyz / self.rate  # Scale delta position with rate
+#
+#         tep = SE3.Trans(trans) * SE3.RPY(yaw_target, np.pi, 0, order="zyx")
+#         sol = self.robot.ik_lm_chan(tep)
+#         target = np.asarray(sol[0], dtype="float32")
+#         dtarget = (target - current) * self.rate  # [rad/sec]
+#         return dict(target=target, dtarget=dtarget)
```

### Comparing `eagerx_franka-0.0.3/eagerx_franka/solid/assets/bolt.stl` & `eagerx_franka-0.0.4/eagerx_franka/solid/assets/bolt.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/solid/assets/bolt.urdf` & `eagerx_franka-0.0.4/eagerx_franka/solid/assets/bolt.urdf`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/solid/assets/box.urdf` & `eagerx_franka-0.0.4/eagerx_franka/solid/assets/box.urdf`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/solid/assets/can.urdf` & `eagerx_franka-0.0.4/eagerx_franka/solid/assets/can.urdf`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/solid/assets/nut.stl` & `eagerx_franka-0.0.4/eagerx_franka/solid/assets/nut.stl`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/eagerx_franka/solid/assets/nut.urdf` & `eagerx_franka-0.0.4/eagerx_franka/solid/assets/nut.urdf`

 * *Files identical despite different names*

### Comparing `eagerx_franka-0.0.3/pyproject.toml` & `eagerx_franka-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 [tool.poetry]
 name = "eagerx_franka"
-version = "0.0.3"
+version = "0.0.4"
 license = "Apache2.0"
 description = "EAGERx interface to franka robot arms."
 authors = ["Jelle Luijkx <j.d.luijkx@tudelft.nl>", "Bas van der Heijden <d.s.vanderheijden@tudelft.nl>"]
 homepage = "https://github.com/eager-dev/eagerx_franka"
 repository = "https://github.com/eager-dev/eagerx_franka"
 documentation = "https://eagerx.readthedocs.io/en/master/"
 include = ["assets"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-eagerx = "^0.1.33"
+eagerx = "^0.1.38"
 eagerx-pybullet = "^0.1.11"
-eagerx-utility = "^0.0.2"
+eagerx-utility = "^0.0.3"
 modern-robotics = "^1.1.0"
-stable-baselines3 = "^1.6.2"
-tensorboard = "^2.11.0"
 urdf-parser-py = "^0.0.4"
-moviepy = "^1.0.3"
-numpy = "<1.20.0"
-roboticstoolbox-python = "^1.0.3"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
 flake8 = ">=3"
 flake8-bugbear = "^22.3.23"
```

