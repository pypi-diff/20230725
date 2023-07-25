# Comparing `tmp/pomdp-py-1.3.1.tar.gz` & `tmp/pomdp-py-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomdp-py-1.3.1.tar", last modified: Wed Nov  3 19:43:28 2021, max compression
+gzip compressed data, was "dist/pomdp-py-1.3.2.tar", last modified: Sun Apr  3 19:18:24 2022, max compression
```

## Comparing `pomdp-py-1.3.1.tar` & `pomdp-py-1.3.2.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.692956 pomdp-py-1.3.1/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1073 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/LICENSE
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      623 2021-09-30 03:46:48.000000 pomdp-py-1.3.1/MANIFEST.in
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1573 2021-11-03 19:43:28.692956 pomdp-py-1.3.1/PKG-INFO
--rw-r--r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1112 2021-02-14 18:11:56.000000 pomdp-py-1.3.1/README.rst
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       33 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/lasertag/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/lasertag/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/light_dark/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      424 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/light_dark/agent/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/agent/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3048 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/agent/belief.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/light_dark/domain/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/domain/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1136 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/domain/action.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1433 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/domain/observation.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1015 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/domain/state.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/light_dark/env/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/env/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1456 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/env/env.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5825 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/env/visual.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/light_dark/models/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/models/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4057 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/models/observation_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2630 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/models/transition_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       67 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/problem_discrete.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     8047 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/light_dark/test.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/load_unload/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/load_unload/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    10477 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/load_unload/load_unload.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/maze/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      895 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_problems/maze/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/maze/domain/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/maze/domain/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      271 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/maze/domain/action.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      898 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/maze/domain/observation.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1000 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/maze/domain/state.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/maze/env/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/maze/env/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      111 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/maze/env/env.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/maze/models/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/maze/models/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/maze/models/components/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/maze/models/components/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      860 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/maze/models/components/map.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/multi_object_search/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/multi_object_search/agent/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/agent/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3087 2020-09-07 11:43:14.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/agent/agent.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     8632 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/agent/belief.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/multi_object_search/domain/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       48 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/domain/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5188 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/domain/action.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3044 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/domain/observation.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2724 2020-02-27 23:34:11.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/domain/state.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/multi_object_search/env/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/env/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     9129 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/env/env.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    12879 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/env/visual.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2273 2020-04-27 20:02:18.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/example_worlds.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.684955 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      152 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/components/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/components/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2458 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/components/grid_map.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     8330 2021-03-22 14:54:05.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/components/sensor.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    10196 2021-03-22 14:54:05.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/observation_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1910 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/policy_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2923 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/reward_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     7805 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/transition_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    15178 2021-08-26 19:46:56.000000 pomdp-py-1.3.1/pomdp_problems/multi_object_search/problem.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/rocksample/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/rocksample/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/rocksample/cythonize/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/rocksample/cythonize/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    18706 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/rocksample/cythonize/rocksample_problem.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       75 2020-09-11 18:07:18.000000 pomdp-py-1.3.1/pomdp_problems/rocksample/cythonize/run_rocksample.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    18368 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/rocksample/rocksample_problem.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/tag/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/tag/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/tag/agent/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/tag/agent/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4593 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/agent/agent.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       15 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/constants.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/tag/domain/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/tag/domain/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      583 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/domain/action.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      758 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/domain/observation.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1376 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/domain/state.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/tag/env/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/tag/env/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2101 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/env/env.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     8999 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/tag/env/visual.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      128 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/example_worlds.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1404 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/experiment.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/tag/models/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/tag/models/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/tag/models/components/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/tag/models/components/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1632 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/models/components/grid_map.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4306 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/tag/models/components/motion_policy.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1374 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/models/observation_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      917 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/models/policy_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      949 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_problems/tag/models/reward_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3918 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/tag/models/transition_model.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6268 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/tag/problem.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/tiger/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       54 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/tiger/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_problems/tiger/cythonize/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.1/pomdp_problems/tiger/cythonize/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       70 2020-09-11 18:07:18.000000 pomdp-py-1.3.1/pomdp_problems/tiger/cythonize/run_tiger.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    14901 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/tiger/cythonize/tiger_problem.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    11608 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_problems/tiger/tiger_problem.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_py/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1318 2021-09-30 03:14:00.000000 pomdp-py-1.3.1/pomdp_py/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1290 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/__main__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_py/algorithms/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.1/pomdp_py/algorithms/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_py/algorithms/bsp/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_py/algorithms/bsp/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    11551 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_py/algorithms/bsp/blqr.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      659 2020-09-07 11:36:06.000000 pomdp-py-1.3.1/pomdp_py/algorithms/po_rollout.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5316 2020-09-11 17:04:13.000000 pomdp-py-1.3.1/pomdp_py/algorithms/po_rollout.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1557 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/algorithms/po_uct.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    18057 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/algorithms/po_uct.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      272 2019-12-27 19:39:57.000000 pomdp-py-1.3.1/pomdp_py/algorithms/pomcp.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6925 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/algorithms/pomcp.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6068 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/algorithms/value_function.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.1/pomdp_py/algorithms/value_iteration.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6197 2020-12-23 21:54:51.000000 pomdp-py-1.3.1/pomdp_py/algorithms/value_iteration.pyx
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_py/framework/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2019-12-16 14:16:00.000000 pomdp-py-1.3.1/pomdp_py/framework/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1290 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/framework/basics.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    24822 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/framework/basics.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      699 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/framework/oopomdp.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    14758 2021-10-18 11:06:34.000000 pomdp-py-1.3.1/pomdp_py/framework/oopomdp.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      234 2020-01-07 19:09:46.000000 pomdp-py-1.3.1/pomdp_py/framework/planner.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1584 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/framework/planner.pyx
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_py/representations/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.1/pomdp_py/representations/__init__.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_py/representations/belief/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.1/pomdp_py/representations/belief/__init__.py
--rw-r--r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4074 2021-01-11 10:30:47.000000 pomdp-py-1.3.1/pomdp_py/representations/belief/histogram.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      535 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_py/representations/belief/particles.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4230 2020-09-26 18:00:05.000000 pomdp-py-1.3.1/pomdp_py/representations/belief/particles.pyx
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_py/representations/distribution/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.1/pomdp_py/representations/distribution/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      147 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_py/representations/distribution/gaussian.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2476 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_py/representations/distribution/gaussian.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      134 2020-07-30 18:59:24.000000 pomdp-py-1.3.1/pomdp_py/representations/distribution/histogram.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3100 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/representations/distribution/histogram.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      379 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/representations/distribution/particles.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     7058 2021-11-03 19:09:44.000000 pomdp-py-1.3.1/pomdp_py/representations/distribution/particles.pyx
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.692956 pomdp-py-1.3.1/pomdp_py/utils/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      622 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2118 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/colors.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       33 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/cython_utils.pxd
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      287 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/cython_utils.pyx
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    25835 2021-09-30 12:54:45.000000 pomdp-py-1.3.1/pomdp_py/utils/debugging.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.692956 pomdp-py-1.3.1/pomdp_py/utils/interfaces/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       56 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/interfaces/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    15391 2021-03-22 14:54:05.000000 pomdp-py-1.3.1/pomdp_py/utils/interfaces/conversion.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3283 2020-02-18 16:38:46.000000 pomdp-py-1.3.1/pomdp_py/utils/interfaces/simple_rl.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5662 2021-09-29 19:20:32.000000 pomdp-py-1.3.1/pomdp_py/utils/interfaces/solvers.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1888 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/math.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1588 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/misc.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2393 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/plotting.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     7344 2021-11-03 19:20:02.000000 pomdp-py-1.3.1/pomdp_py/utils/templates.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      694 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/test_utils.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1974 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/utils/typ.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.692956 pomdp-py-1.3.1/pomdp_py/visual/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-09-30 03:14:03.000000 pomdp-py-1.3.1/pomdp_py/visual/__init__.py
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6480 2021-09-30 02:29:30.000000 pomdp-py-1.3.1/pomdp_py/visual/search_tree.py
-drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-11-03 19:43:28.688956 pomdp-py-1.3.1/pomdp_py.egg-info/
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1573 2021-11-03 19:43:28.000000 pomdp-py-1.3.1/pomdp_py.egg-info/PKG-INFO
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5644 2021-11-03 19:43:28.000000 pomdp-py-1.3.1/pomdp_py.egg-info/SOURCES.txt
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-11-03 19:43:28.000000 pomdp-py-1.3.1/pomdp_py.egg-info/dependency_links.txt
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-07-06 22:15:35.000000 pomdp-py-1.3.1/pomdp_py.egg-info/not-zip-safe
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       56 2021-11-03 19:43:28.000000 pomdp-py-1.3.1/pomdp_py.egg-info/requires.txt
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       24 2021-11-03 19:43:28.000000 pomdp-py-1.3.1/pomdp_py.egg-info/top_level.txt
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       38 2021-11-03 19:43:28.692956 pomdp-py-1.3.1/setup.cfg
--rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2233 2021-11-03 19:28:25.000000 pomdp-py-1.3.1/setup.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1073 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/LICENSE
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      623 2021-09-30 03:46:48.000000 pomdp-py-1.3.2/MANIFEST.in
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1573 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/PKG-INFO
+-rw-r--r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1112 2021-02-14 18:11:56.000000 pomdp-py-1.3.2/README.rst
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       33 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/lasertag/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/lasertag/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      424 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/agent/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/agent/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3048 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/agent/belief.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/domain/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/domain/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1136 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/domain/action.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1433 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/domain/observation.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1015 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/domain/state.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/env/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/env/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1456 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/env/env.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5825 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/env/visual.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/models/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/models/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4057 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/models/observation_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2630 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/models/transition_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       67 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/problem_discrete.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     8047 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/light_dark/test.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/load_unload/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/load_unload/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    10477 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/load_unload/load_unload.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/maze/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      895 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_problems/maze/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/maze/domain/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/maze/domain/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      271 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/maze/domain/action.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      898 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/maze/domain/observation.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1000 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/maze/domain/state.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/maze/env/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/maze/env/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      111 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/maze/env/env.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/maze/models/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/maze/models/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/maze/models/components/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/maze/models/components/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      860 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/maze/models/components/map.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/agent/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/agent/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3087 2020-09-07 11:43:14.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/agent/agent.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     8632 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/agent/belief.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/domain/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       48 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/domain/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5188 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/domain/action.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3044 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/domain/observation.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2724 2020-02-27 23:34:11.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/domain/state.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/env/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/env/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     9129 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/env/env.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    12879 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/env/visual.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2273 2020-04-27 20:02:18.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/example_worlds.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      152 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/components/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/components/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2458 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/components/grid_map.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     8330 2021-03-22 14:54:05.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/components/sensor.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    10196 2021-03-22 14:54:05.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/observation_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1910 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/policy_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2923 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/reward_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     7805 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/transition_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    15178 2021-08-26 19:46:56.000000 pomdp-py-1.3.2/pomdp_problems/multi_object_search/problem.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/rocksample/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/rocksample/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/rocksample/cythonize/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/rocksample/cythonize/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    18706 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/rocksample/cythonize/rocksample_problem.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       75 2020-09-11 18:07:18.000000 pomdp-py-1.3.2/pomdp_problems/rocksample/cythonize/run_rocksample.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    18368 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/rocksample/rocksample_problem.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/tag/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/tag/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/tag/agent/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/tag/agent/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4593 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/agent/agent.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       15 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/constants.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/tag/domain/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/tag/domain/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      583 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/domain/action.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      758 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/domain/observation.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1376 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/domain/state.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/tag/env/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/tag/env/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2101 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/env/env.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     8999 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/tag/env/visual.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      128 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/example_worlds.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1404 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/experiment.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/components/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/components/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1632 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/components/grid_map.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4306 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/components/motion_policy.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1374 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/observation_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      917 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/policy_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      949 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/reward_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3918 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/tag/models/transition_model.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6268 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/tag/problem.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/tiger/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       54 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/tiger/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_problems/tiger/cythonize/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2021-06-01 18:09:19.000000 pomdp-py-1.3.2/pomdp_problems/tiger/cythonize/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       70 2020-09-11 18:07:18.000000 pomdp-py-1.3.2/pomdp_problems/tiger/cythonize/run_tiger.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    14901 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_problems/tiger/cythonize/tiger_problem.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    12632 2022-04-03 18:52:09.000000 pomdp-py-1.3.2/pomdp_problems/tiger/tiger_problem.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1318 2021-09-30 03:14:00.000000 pomdp-py-1.3.2/pomdp_py/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1290 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/__main__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/algorithms/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.2/pomdp_py/algorithms/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/algorithms/bsp/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_py/algorithms/bsp/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    11551 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_py/algorithms/bsp/blqr.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      659 2020-09-07 11:36:06.000000 pomdp-py-1.3.2/pomdp_py/algorithms/po_rollout.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5316 2020-09-11 17:04:13.000000 pomdp-py-1.3.2/pomdp_py/algorithms/po_rollout.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1557 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/algorithms/po_uct.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    18057 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/algorithms/po_uct.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      272 2019-12-27 19:39:57.000000 pomdp-py-1.3.2/pomdp_py/algorithms/pomcp.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6925 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/algorithms/pomcp.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6068 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/algorithms/value_function.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.2/pomdp_py/algorithms/value_iteration.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6197 2020-12-23 21:54:51.000000 pomdp-py-1.3.2/pomdp_py/algorithms/value_iteration.pyx
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/framework/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2019-12-16 14:16:00.000000 pomdp-py-1.3.2/pomdp_py/framework/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1290 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/framework/basics.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    24822 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/framework/basics.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      699 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/framework/oopomdp.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    14758 2021-10-18 11:06:34.000000 pomdp-py-1.3.2/pomdp_py/framework/oopomdp.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      234 2020-01-07 19:09:46.000000 pomdp-py-1.3.2/pomdp_py/framework/planner.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1584 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/framework/planner.pyx
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/representations/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.2/pomdp_py/representations/__init__.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/representations/belief/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.2/pomdp_py/representations/belief/__init__.py
+-rw-r--r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4074 2021-01-11 10:30:47.000000 pomdp-py-1.3.2/pomdp_py/representations/belief/histogram.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      535 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_py/representations/belief/particles.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     4230 2020-09-26 18:00:05.000000 pomdp-py-1.3.2/pomdp_py/representations/belief/particles.pyx
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/representations/distribution/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2019-12-27 19:39:57.000000 pomdp-py-1.3.2/pomdp_py/representations/distribution/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      147 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_py/representations/distribution/gaussian.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2476 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_py/representations/distribution/gaussian.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      134 2020-07-30 18:59:24.000000 pomdp-py-1.3.2/pomdp_py/representations/distribution/histogram.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2885 2022-04-03 16:09:03.000000 pomdp-py-1.3.2/pomdp_py/representations/distribution/histogram.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      379 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/representations/distribution/particles.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     7058 2021-11-03 19:09:44.000000 pomdp-py-1.3.2/pomdp_py/representations/distribution/particles.pyx
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/utils/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      622 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2118 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/colors.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       33 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/cython_utils.pxd
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      287 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/cython_utils.pyx
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    25835 2021-09-30 12:54:45.000000 pomdp-py-1.3.2/pomdp_py/utils/debugging.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/utils/interfaces/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       56 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/interfaces/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)    15391 2021-03-22 14:54:05.000000 pomdp-py-1.3.2/pomdp_py/utils/interfaces/conversion.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     3283 2020-02-18 16:38:46.000000 pomdp-py-1.3.2/pomdp_py/utils/interfaces/simple_rl.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5662 2021-09-29 19:20:32.000000 pomdp-py-1.3.2/pomdp_py/utils/interfaces/solvers.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1888 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/math.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1588 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/misc.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2393 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/plotting.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     7344 2021-11-03 19:20:02.000000 pomdp-py-1.3.2/pomdp_py/utils/templates.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)      694 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/test_utils.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1974 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/utils/typ.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py/visual/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-09-30 03:14:03.000000 pomdp-py-1.3.2/pomdp_py/visual/__init__.py
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     6480 2021-09-30 02:29:30.000000 pomdp-py-1.3.2/pomdp_py/visual/search_tree.py
+drwxrwxr-x   0 kaiyuzh   (1000) kaiyuzh   (1000)        0 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/pomdp_py.egg-info/
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     1573 2022-04-03 19:18:23.000000 pomdp-py-1.3.2/pomdp_py.egg-info/PKG-INFO
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     5644 2022-04-03 19:18:23.000000 pomdp-py-1.3.2/pomdp_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2022-04-03 19:18:23.000000 pomdp-py-1.3.2/pomdp_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)        1 2021-07-06 22:15:35.000000 pomdp-py-1.3.2/pomdp_py.egg-info/not-zip-safe
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       56 2022-04-03 19:18:23.000000 pomdp-py-1.3.2/pomdp_py.egg-info/requires.txt
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       24 2022-04-03 19:18:23.000000 pomdp-py-1.3.2/pomdp_py.egg-info/top_level.txt
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)       38 2022-04-03 19:18:24.000000 pomdp-py-1.3.2/setup.cfg
+-rw-rw-r--   0 kaiyuzh   (1000) kaiyuzh   (1000)     2233 2022-04-03 19:02:12.000000 pomdp-py-1.3.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pomdp-py-1.3.1/LICENSE` & `pomdp-py-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/MANIFEST.in` & `pomdp-py-1.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/PKG-INFO` & `pomdp-py-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomdp-py
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python POMDP Library.
 Home-page: UNKNOWN
 Author: Kaiyu Zheng
 Author-email: kzheng10@cs.brown.edu
 License: MIT
 Description: pomdp_py
         ========
```

### Comparing `pomdp-py-1.3.1/README.rst` & `pomdp-py-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/agent/belief.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/agent/belief.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/domain/action.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/domain/action.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/domain/observation.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/domain/observation.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/domain/state.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/domain/state.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/env/env.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/env/env.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/env/visual.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/env/visual.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/models/observation_model.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/models/observation_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/models/transition_model.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/models/transition_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/light_dark/test.py` & `pomdp-py-1.3.2/pomdp_problems/light_dark/test.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/load_unload/load_unload.py` & `pomdp-py-1.3.2/pomdp_problems/load_unload/load_unload.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/maze/__init__.py` & `pomdp-py-1.3.2/pomdp_problems/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/maze/domain/observation.py` & `pomdp-py-1.3.2/pomdp_problems/maze/domain/observation.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/maze/domain/state.py` & `pomdp-py-1.3.2/pomdp_problems/maze/domain/state.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/maze/models/components/map.py` & `pomdp-py-1.3.2/pomdp_problems/maze/models/components/map.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/agent/agent.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/agent/agent.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/agent/belief.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/agent/belief.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/domain/action.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/domain/action.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/domain/observation.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/domain/observation.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/domain/state.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/domain/state.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/env/env.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/env/env.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/env/visual.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/env/visual.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/example_worlds.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/example_worlds.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/components/grid_map.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/components/grid_map.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/components/sensor.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/components/sensor.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/observation_model.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/observation_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/policy_model.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/policy_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/reward_model.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/reward_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/models/transition_model.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/models/transition_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/multi_object_search/problem.py` & `pomdp-py-1.3.2/pomdp_problems/multi_object_search/problem.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/rocksample/cythonize/rocksample_problem.pyx` & `pomdp-py-1.3.2/pomdp_problems/rocksample/cythonize/rocksample_problem.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/rocksample/rocksample_problem.py` & `pomdp-py-1.3.2/pomdp_problems/rocksample/rocksample_problem.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/agent/agent.py` & `pomdp-py-1.3.2/pomdp_problems/tag/agent/agent.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/domain/action.py` & `pomdp-py-1.3.2/pomdp_problems/tag/domain/action.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/domain/observation.py` & `pomdp-py-1.3.2/pomdp_problems/tag/domain/observation.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/domain/state.py` & `pomdp-py-1.3.2/pomdp_problems/tag/domain/state.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/env/env.py` & `pomdp-py-1.3.2/pomdp_problems/tag/env/env.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/env/visual.py` & `pomdp-py-1.3.2/pomdp_problems/tag/env/visual.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/experiment.py` & `pomdp-py-1.3.2/pomdp_problems/tag/experiment.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/models/components/grid_map.py` & `pomdp-py-1.3.2/pomdp_problems/tag/models/components/grid_map.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/models/components/motion_policy.py` & `pomdp-py-1.3.2/pomdp_problems/tag/models/components/motion_policy.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/models/observation_model.py` & `pomdp-py-1.3.2/pomdp_problems/tag/models/observation_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/models/policy_model.py` & `pomdp-py-1.3.2/pomdp_problems/tag/models/policy_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/models/reward_model.py` & `pomdp-py-1.3.2/pomdp_problems/tag/models/reward_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/models/transition_model.py` & `pomdp-py-1.3.2/pomdp_problems/tag/models/transition_model.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tag/problem.py` & `pomdp-py-1.3.2/pomdp_problems/tag/problem.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tiger/cythonize/tiger_problem.pyx` & `pomdp-py-1.3.2/pomdp_problems/tiger/cythonize/tiger_problem.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_problems/tiger/tiger_problem.py` & `pomdp-py-1.3.2/pomdp_problems/tiger/tiger_problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The classic Tiger problem.
 
 This is a POMDP problem; Namely, it specifies both
 the POMDP (i.e. state, action, observation space)
 and the T/O/R for the agent as well as the environment.
 
-The description of the tiger problem is as follows: (Quote from `POMDP:
-Introduction to Partially Observable Markov Decision Processes
+The description of the tiger problem is as follows: (Quote from
+`POMDP: Introduction to Partially Observable Markov Decision Processes
 <https://cran.r-project.org/web/packages/pomdp/vignettes/POMDP.pdf>`_ by
 Kamalzadeh and Hahsler )
 
 A tiger is put with equal probability behind one
 of two doors, while treasure is put behind the other one.
 You are standing in front of the two closed doors and
 need to decide which one to open. If you open the door
@@ -26,17 +26,16 @@
 Rewards:
     +10 for opening treasure door. -100 for opening tiger door.
     -1 for listening.
 Observations: You can hear either "tiger-left", or "tiger-right".
 
 Note that in this example, the TigerProblem is a POMDP that
 also contains the agent and the environment as its fields. In
-general this doesn't need to be the case. (Refer to more complicated
-examples.)
-
+general this doesn't need to be the case. (Refer to more
+complicated examples.)
 """
 
 import pomdp_py
 from pomdp_py.utils import TreeDebugger
 import random
 import numpy as np
 import sys
@@ -91,15 +90,16 @@
 # Observation model
 class ObservationModel(pomdp_py.ObservationModel):
     def __init__(self, noise=0.15):
         self.noise = noise
 
     def probability(self, observation, next_state, action):
         if action.name == "listen":
-            if observation.name == next_state.name: # heard the correct growl
+            # heard the correct growl
+            if observation.name == next_state.name:
                 return 1.0 - self.noise
             else:
                 return self.noise
         else:
             return 0.5
 
     def sample(self, next_state, action):
@@ -111,16 +111,18 @@
         if random.uniform(0,1) < thresh:
             return TigerObservation(next_state.name)
         else:
             return TigerObservation(next_state.other().name)
 
     def get_all_observations(self):
         """Only need to implement this if you're using
-        a solver that needs to enumerate over the observation space (e.g. value iteration)"""
-        return [TigerObservation(s) for s in {"tiger-left", "tiger-right"}]
+        a solver that needs to enumerate over the observation space
+        (e.g. value iteration)"""
+        return [TigerObservation(s)
+                for s in {"tiger-left", "tiger-right"}]
 
 # Transition Model
 class TransitionModel(pomdp_py.TransitionModel):
     def probability(self, next_state, state, action):
         """According to problem spec, the world resets once
         action is open-left/open-right. Otherwise, stays the same"""
         if action.name.startswith("open"):
@@ -138,16 +140,14 @@
             return TigerState(state.name)
 
     def get_all_states(self):
         """Only need to implement this if you're using
         a solver that needs to enumerate over the observation space (e.g. value iteration)"""
         return [TigerState(s) for s in {"tiger-left", "tiger-right"}]
 
-
-
 # Reward Model
 class RewardModel(pomdp_py.RewardModel):
     def _reward_func(self, state, action):
         if action.name == "open-left":
             if state.name == "tiger-right":
                 return 10
             else:
@@ -161,25 +161,28 @@
             return -1
 
     def sample(self, state, action, next_state):
         # deterministic
         return self._reward_func(state, action)
 
 # Policy Model
-class PolicyModel(pomdp_py.RandomRollout):
-    """This is an extremely dumb policy model; To keep consistent
-    with the framework."""
-    # A stay action can be added to test that POMDP solver is
-    # able to differentiate information gathering actions.
-    ACTIONS = {TigerAction(s) for s in {"open-left", "open-right", "listen"}}
+class PolicyModel(pomdp_py.RolloutPolicy):
+    """A simple policy model with uniform prior over a
+       small, finite action space"""
+    ACTIONS = {TigerAction(s)
+              for s in {"open-left", "open-right", "listen"}}
 
-    def sample(self, state, **kwargs):
+    def sample(self, state):
         return random.sample(self.get_all_actions(), 1)[0]
 
-    def get_all_actions(self, **kwargs):
+    def rollout(self, state, history=None):
+        """Treating this PolicyModel as a rollout policy"""
+        return self.sample(state)
+
+    def get_all_actions(self, state=None, history=None):
         return PolicyModel.ACTIONS
 
 
 class TigerProblem(pomdp_py.POMDP):
     """
     In fact, creating a TigerProblem class is entirely optional
     to simulate and solve POMDPs. But this is just an example
@@ -198,73 +201,104 @@
                                    RewardModel())
         super().__init__(agent, env, name="TigerProblem")
 
     @staticmethod
     def create(state="tiger-left", belief=0.5, obs_noise=0.15):
         """
         Args:
-            state (str): could be 'tiger-left' or 'tiger-right'; True state of the environment
-            belief (float): Initial belief that the target is on the left; Between 0-1.
-            obs_noise (float): Noise for the observation model (default 0.15)
+            state (str): could be 'tiger-left' or 'tiger-right';
+                         True state of the environment
+            belief (float): Initial belief that the target is
+                            on the left; Between 0-1.
+            obs_noise (float): Noise for the observation
+                               model (default 0.15)
         """
         init_true_state = TigerState(state)
-        init_belief = pomdp_py.Histogram({TigerState("tiger-left"): belief,
-                                          TigerState("tiger-right"): 1.0 - belief})
-        tiger_problem = TigerProblem(obs_noise,  # observation noise
+        init_belief = pomdp_py.Histogram({
+            TigerState("tiger-left"): belief,
+            TigerState("tiger-right"): 1.0 - belief
+        })
+        tiger_problem = TigerProblem(obs_noise,
                                      init_true_state, init_belief)
         tiger_problem.agent.set_belief(init_belief, prior=True)
         return tiger_problem
 
 
 
 
-def test_planner(tiger_problem, planner, nsteps=3, debug_tree=False):
+def test_planner(tiger_problem, planner, nsteps=3,
+                 debug_tree=False):
     """
     Runs the action-feedback loop of Tiger problem POMDP
 
     Args:
-        tiger_problem (TigerProblem): an instance of the tiger problem.
+        tiger_problem (TigerProblem): a problem instance
         planner (Planner): a planner
         nsteps (int): Maximum number of steps to run this loop.
+        debug_tree (bool): True if get into the pdb with a
+                           TreeDebugger created as 'dd' variable.
     """
     for i in range(nsteps):
         action = planner.plan(tiger_problem.agent)
         if debug_tree:
             from pomdp_py.utils import TreeDebugger
             dd = TreeDebugger(tiger_problem.agent.tree)
             import pdb; pdb.set_trace()
 
         print("==== Step %d ====" % (i+1))
-        print("True state: %s" % tiger_problem.env.state)
-        print("Belief: %s" % str(tiger_problem.agent.cur_belief))
-        print("Action: %s" % str(action))
-        print("Reward: %s" % str(tiger_problem.env.reward_model.sample(tiger_problem.env.state, action, None)))
-
-        # Let's create some simulated real observation; Update the belief
-        # Creating true observation for sanity checking solver behavior.
-        # In general, this observation should be sampled from agent's observation model.
+        print("True state:", tiger_problem.env.state)
+        print("Belief:", tiger_problem.agent.cur_belief)
+        print("Action:", action)
+        # There is no state transition for the tiger domain.
+        # In general, the ennvironment state can be transitioned
+        # using
+        #
+        #   reward = tiger_problem.env.state_transition(action, execute=True)
+        #
+        # Or, it is possible that you don't have control
+        # over the environment change (e.g. robot acting
+        # in real world); In that case, you could skip
+        # the state transition and re-estimate the state
+        # (e.g. through the perception stack on the robot).
+        reward = tiger_problem.env.reward_model.sample(tiger_problem.env.state, action, None)
+        print("Reward:", reward)
+
+        # Let's create some simulated real observation;
+        # Update the belief Creating true observation for
+        # sanity checking solver behavior. In general, this
+        # observation should be sampled from agent's observation
+        # model, as
+        #
+        #    real_observation = tiger_problem.agent.observation_model.sample(tiger_problem.env.state, action)
+        #
+        # or coming from an external source (e.g. robot sensor
+        # reading). Note that tiger_problem.env.state stores the
+        # environment state after action execution.
         real_observation = TigerObservation(tiger_problem.env.state.name)
-        print(">> Observation: %s" % real_observation)
+        print(">> Observation:",  real_observation)
         tiger_problem.agent.update_history(action, real_observation)
 
         # If the planner is POMCP, planner.update also updates agent belief.
         planner.update(tiger_problem.agent, action, real_observation)
         if isinstance(planner, pomdp_py.POUCT):
-            print("Num sims: %d" % planner.last_num_sims)
+            print("Num sims:", planner.last_num_sims)
             print("Plan time: %.5f" % planner.last_planning_time)
 
-        if isinstance(tiger_problem.agent.cur_belief, pomdp_py.Histogram):
-            new_belief = pomdp_py.update_histogram_belief(tiger_problem.agent.cur_belief,
-                                                          action, real_observation,
-                                                          tiger_problem.agent.observation_model,
-                                                          tiger_problem.agent.transition_model)
+        if isinstance(tiger_problem.agent.cur_belief,
+                      pomdp_py.Histogram):
+            new_belief = pomdp_py.update_histogram_belief(
+                tiger_problem.agent.cur_belief,
+                action, real_observation,
+                tiger_problem.agent.observation_model,
+                tiger_problem.agent.transition_model)
             tiger_problem.agent.set_belief(new_belief)
 
         if action.name.startswith("open"):
-            # Make it clearer to see what actions are taken until every time door is opened.
+            # Make it clearer to see what actions are taken
+            # until every time door is opened.
             print("\n")
 
 def main():
     init_true_state = random.choice([TigerState("tiger-left"),
                                      TigerState("tiger-right")])
     init_belief = pomdp_py.Histogram({TigerState("tiger-left"): 0.5,
                                       TigerState("tiger-right"): 0.5})
```

### Comparing `pomdp-py-1.3.1/pomdp_py/__init__.py` & `pomdp-py-1.3.2/pomdp_py/__init__.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/__main__.py` & `pomdp-py-1.3.2/pomdp_py/__main__.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/algorithms/bsp/blqr.py` & `pomdp-py-1.3.2/pomdp_py/algorithms/bsp/blqr.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/algorithms/po_rollout.pxd` & `pomdp-py-1.3.2/pomdp_py/algorithms/po_rollout.pxd`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/algorithms/po_rollout.pyx` & `pomdp-py-1.3.2/pomdp_py/algorithms/po_rollout.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/algorithms/po_uct.pxd` & `pomdp-py-1.3.2/pomdp_py/algorithms/po_uct.pxd`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/algorithms/po_uct.pyx` & `pomdp-py-1.3.2/pomdp_py/algorithms/po_uct.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/algorithms/pomcp.pyx` & `pomdp-py-1.3.2/pomdp_py/algorithms/pomcp.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/algorithms/value_function.py` & `pomdp-py-1.3.2/pomdp_py/algorithms/value_function.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/algorithms/value_iteration.pyx` & `pomdp-py-1.3.2/pomdp_py/algorithms/value_iteration.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/framework/basics.pxd` & `pomdp-py-1.3.2/pomdp_py/framework/basics.pxd`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/framework/basics.pyx` & `pomdp-py-1.3.2/pomdp_py/framework/basics.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/framework/oopomdp.pxd` & `pomdp-py-1.3.2/pomdp_py/framework/oopomdp.pxd`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/framework/oopomdp.pyx` & `pomdp-py-1.3.2/pomdp_py/framework/oopomdp.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/framework/planner.pyx` & `pomdp-py-1.3.2/pomdp_py/framework/planner.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/representations/belief/histogram.py` & `pomdp-py-1.3.2/pomdp_py/representations/belief/histogram.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/representations/belief/particles.pxd` & `pomdp-py-1.3.2/pomdp_py/representations/belief/particles.pxd`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/representations/belief/particles.pyx` & `pomdp-py-1.3.2/pomdp_py/representations/belief/particles.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/representations/distribution/gaussian.pyx` & `pomdp-py-1.3.2/pomdp_py/representations/distribution/gaussian.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/representations/distribution/histogram.pyx` & `pomdp-py-1.3.2/pomdp_py/representations/distribution/histogram.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,15 @@
 
     @property
     def histogram(self):
         """histogram(self)"""
         return self._histogram
 
     def __str__(self):
-        if isinstance(self._histogram, dict):
-            return str([(k,self._histogram[k])
-                        for k in list(reversed(sorted(self._histogram,
-                                                      key=self._histogram.get)))[:5]])
+        return str(self._histogram)
 
     def __len__(self):
         return len(self._histogram)
 
     def __getitem__(self, value):
         """__getitem__(self, value)
         Returns the probability of `value`."""
```

### Comparing `pomdp-py-1.3.1/pomdp_py/representations/distribution/particles.pyx` & `pomdp-py-1.3.2/pomdp_py/representations/distribution/particles.pyx`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/__init__.py` & `pomdp-py-1.3.2/pomdp_py/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/colors.py` & `pomdp-py-1.3.2/pomdp_py/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/debugging.py` & `pomdp-py-1.3.2/pomdp_py/utils/debugging.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/interfaces/conversion.py` & `pomdp-py-1.3.2/pomdp_py/utils/interfaces/conversion.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/interfaces/simple_rl.py` & `pomdp-py-1.3.2/pomdp_py/utils/interfaces/simple_rl.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/interfaces/solvers.py` & `pomdp-py-1.3.2/pomdp_py/utils/interfaces/solvers.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/math.py` & `pomdp-py-1.3.2/pomdp_py/utils/math.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/misc.py` & `pomdp-py-1.3.2/pomdp_py/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/plotting.py` & `pomdp-py-1.3.2/pomdp_py/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/templates.py` & `pomdp-py-1.3.2/pomdp_py/utils/templates.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/test_utils.py` & `pomdp-py-1.3.2/pomdp_py/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/utils/typ.py` & `pomdp-py-1.3.2/pomdp_py/utils/typ.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py/visual/search_tree.py` & `pomdp-py-1.3.2/pomdp_py/visual/search_tree.py`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/pomdp_py.egg-info/PKG-INFO` & `pomdp-py-1.3.2/pomdp_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomdp-py
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python POMDP Library.
 Home-page: UNKNOWN
 Author: Kaiyu Zheng
 Author-email: kzheng10@cs.brown.edu
 License: MIT
 Description: pomdp_py
         ========
```

### Comparing `pomdp-py-1.3.1/pomdp_py.egg-info/SOURCES.txt` & `pomdp-py-1.3.2/pomdp_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pomdp-py-1.3.1/setup.py` & `pomdp-py-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 extensions += [
     Extension("pomdp_problems.tiger.cythonize", ["pomdp_problems/tiger/cythonize/tiger_problem.pyx"]),
     Extension("pomdp_problems.rocksample.cythonize", ["pomdp_problems/rocksample/cythonize/rocksample_problem.pyx"])
 ]
 
 setup(name='pomdp-py',
       packages=find_packages(),
-      version='1.3.1',
+      version='1.3.2',
       description='Python POMDP Library.',
       long_description=long_description,
       long_description_content_type="text/x-rst",
       install_requires=[
           'Cython',
           'numpy',
           'scipy',
```

