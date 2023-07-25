# Comparing `tmp/skrl-0.9.1.tar.gz` & `tmp/skrl-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/skrl/skrl/dist/.tmp-4_xcyjbv/skrl-0.9.1.tar", last modified: Tue Jan 17 14:08:19 2023, max compression
+gzip compressed data, was "/home/runner/work/skrl/skrl/dist/.tmp-2_bsfy1x/skrl-1.0.0rc1.tar", last modified: Tue Jul 25 09:17:01 2023, max compression
```

## Comparing `skrl-0.9.1.tar` & `skrl-1.0.0rc1.tar`

### file list

```diff
@@ -1,112 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-17 14:08:08.000000 skrl-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-01-17 14:08:19.000000 skrl-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-01-17 14:08:08.000000 skrl-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:08:19.000000 skrl-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-01-17 14:08:08.000000 skrl-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/a2c/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/a2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23343 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/a2c/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/amp/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31024 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/amp/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)    33359 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/cem/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/cem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/cem/cem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/ddpg/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/ddpg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/ddpg/ddpg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/dqn/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/dqn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14711 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/dqn/ddqn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/dqn/dqn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/ppo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25338 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/ppo/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/q_learning/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/q_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/q_learning/q_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/sac/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/sac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21449 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/sac/sac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/sarsa/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/sarsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/sarsa/sarsa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/td3/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/td3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/td3/td3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/agents/torch/trpo/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/trpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/agents/torch/trpo/trpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/envs/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/envs/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/envs/torch/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    39214 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/envs/torch/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/memories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/memories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/memories/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/memories/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/memories/torch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/memories/torch/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/models/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/models/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36202 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/models/torch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/models/torch/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/models/torch/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/models/torch/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/models/torch/multivariate_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/models/torch/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/resources/noises/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/noises/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/resources/noises/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/noises/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/noises/torch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/noises/torch/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/noises/torch/ornstein_uhlenbeck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/resources/preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/resources/preprocessors/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/preprocessors/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/preprocessors/torch/running_standard_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/resources/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/resources/schedulers/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/schedulers/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/resources/schedulers/torch/kl_adaptive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/trainers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/trainers/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/trainers/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/trainers/torch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/trainers/torch/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/trainers/torch/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/trainers/torch/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/utils/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/utils/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20572 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/utils/isaacgym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24634 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/utils/model_instantiators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/utils/omniverse_isaacgym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/utils/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-17 14:08:08.000000 skrl-0.9.1/skrl/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-17 14:08:19.000000 skrl-0.9.1/skrl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/a2c/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/a2c/a2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21860 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/cem/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/cem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/cem/cem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/ddpg/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/ddpg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21720 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/ddpg/ddpg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/dqn/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/dqn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/dqn/ddqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/dqn/dqn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/ppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25645 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/ppo/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/rpo/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/rpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26109 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/rpo/rpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/sac/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/sac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25218 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/sac/sac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/jax/td3/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/td3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26715 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/jax/td3/td3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/a2c/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/a2c/a2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23414 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/a2c/a2c_rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31040 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/amp/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33314 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/cem/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/cem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/cem/cem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/ddpg/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/ddpg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/ddpg/ddpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/ddpg/ddpg_rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/dqn/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/dqn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14711 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/dqn/ddqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/dqn/dqn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/ppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21024 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/ppo/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/ppo/ppo_rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/q_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/q_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/q_learning/q_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/rpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/rpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/rpo/rpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25671 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/rpo/rpo_rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/sac/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/sac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/sac/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21519 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/sac/sac_rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/sarsa/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/sarsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/sarsa/sarsa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/td3/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/td3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21390 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/td3/td3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23679 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/td3/td3_rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/agents/torch/trpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/trpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25930 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/trpo/trpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30788 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/agents/torch/trpo/trpo_rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/envs/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/envs/jax/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/loaders/bidexhands_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/loaders/isaac_orbit_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/loaders/isaacgym_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/loaders/omniverse_isaacgym_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/bidexhands_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/gym_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/gymnasium_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/isaac_orbit_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/isaacgym_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/omniverse_isaacgym_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/jax/wrappers/pettingzoo_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/envs/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/envs/torch/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/loaders/bidexhands_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/loaders/isaac_orbit_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/loaders/isaacgym_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/loaders/omniverse_isaacgym_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/bidexhands_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/deepmind_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/gym_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/gymnasium_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/isaac_orbit_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/isaacgym_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/omniverse_isaacgym_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/pettingzoo_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/envs/torch/wrappers/robosuite_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/memories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/memories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/memories/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/memories/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23656 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/memories/jax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/memories/jax/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/memories/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/memories/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/memories/torch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/memories/torch/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/models/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25940 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/jax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/jax/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/jax/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/jax/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/models/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36029 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/torch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/torch/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/torch/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/torch/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/torch/multivariate_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/models/torch/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/multi_agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24232 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/ippo/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/ippo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/ippo/ippo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/mappo/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/mappo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29998 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/jax/mappo/mappo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/ippo/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/ippo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23244 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/ippo/ippo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/mappo/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/mappo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/multi_agents/torch/mappo/mappo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/noises/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/noises/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/jax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/jax/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/jax/ornstein_uhlenbeck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/noises/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/torch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/torch/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/noises/torch/ornstein_uhlenbeck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/optimizers/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/optimizers/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/optimizers/jax/adam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/preprocessors/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/preprocessors/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/preprocessors/jax/running_standard_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/preprocessors/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/preprocessors/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/preprocessors/torch/running_standard_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/schedulers/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/schedulers/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/schedulers/jax/kl_adaptive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/resources/schedulers/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/schedulers/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/resources/schedulers/torch/kl_adaptive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/trainers/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/jax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/jax/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/jax/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/trainers/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/torch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/torch/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/torch/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/trainers/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/utils/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/utils/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/utils/isaacgym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30201 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/utils/model_instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/utils/omniverse_isaacgym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/skrl/utils/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/skrl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:17:01.000000 skrl-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_deepmind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_gymnasium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_isaac_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_isaacgym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_isaacsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_omniisaacgym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_robosuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-25 09:16:49.000000 skrl-1.0.0rc1/tests/test_examples_shimmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-25 09:16:50.000000 skrl-1.0.0rc1/tests/test_jax_memories_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-25 09:16:50.000000 skrl-1.0.0rc1/tests/test_memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-25 09:16:50.000000 skrl-1.0.0rc1/tests/test_model_instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-25 09:16:50.000000 skrl-1.0.0rc1/tests/test_resources_noises.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-25 09:16:50.000000 skrl-1.0.0rc1/tests/test_resources_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-25 09:16:50.000000 skrl-1.0.0rc1/tests/test_resources_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-25 09:16:50.000000 skrl-1.0.0rc1/tests/test_trainers.py
```

### Comparing `skrl-0.9.1/LICENSE` & `skrl-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `skrl-0.9.1/PKG-INFO` & `skrl-1.0.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 Metadata-Version: 2.1
 Name: skrl
-Version: 0.9.1
-Summary: Modular and flexible library for Reinforcement Learning
-Home-page: https://github.com/Toni-SM/skrl
+Version: 1.0.0rc1
+Summary: Modular and flexible library for reinforcement learning on PyTorch and JAX
 Author: Toni-SM
-License: MIT
+Maintainer: Toni-SM
+License: MIT License
+Project-URL: Homepage, https://github.com/Toni-SM/skrl
 Project-URL: Documentation, https://skrl.readthedocs.io
-Project-URL: Repository, https://github.com/Toni-SM/skrl
-Project-URL: Bug Tracker, https://github.com/Toni-SM/skrl/issues
 Project-URL: Discussions, https://github.com/Toni-SM/skrl/discussions
-Keywords: reinforcement,machine,learning,rl
+Project-URL: Bug Reports, https://github.com/Toni-SM/skrl/issues
+Project-URL: Say Thanks!, https://github.com/Toni-SM
+Project-URL: Source, https://github.com/Toni-SM/skrl
+Keywords: reinforcement-learning,machine-learning,reinforcement,machine,learning,rl
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6.*
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: torch
+Provides-Extra: jax
+Provides-Extra: all
 License-File: LICENSE
 
 [![pypi](https://img.shields.io/pypi/v/skrl)](https://pypi.org/project/skrl)
-[<img src="https://img.shields.io/badge/%F0%9F%A4%97%20Models-Huggingface-F8D521">](https://huggingface.co/skrl)
+[<img src="https://img.shields.io/badge/%F0%9F%A4%97%20models-hugging%20face-F8D521">](https://huggingface.co/skrl)
 ![discussions](https://img.shields.io/github/discussions/Toni-SM/skrl)
 <br>
 [![license](https://img.shields.io/github/license/Toni-SM/skrl)](https://github.com/Toni-SM/skrl)
 <span>&nbsp;&nbsp;&nbsp;&nbsp;</span>
 [![docs](https://readthedocs.org/projects/skrl/badge/?version=latest)](https://skrl.readthedocs.io/en/latest/?badge=latest)
 [![pytest](https://github.com/Toni-SM/skrl/actions/workflows/python-test.yml/badge.svg)](https://github.com/Toni-SM/skrl/actions/workflows/python-test.yml)
 [![pre-commit](https://github.com/Toni-SM/skrl/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/Toni-SM/skrl/actions/workflows/pre-commit.yml)
 
 <br>
 <p align="center">
-  <img width="300rem" src="https://raw.githubusercontent.com/Toni-SM/skrl/main/docs/source/_static/data/skrl-up-transparent.png">
+  <img width="300rem" src="https://raw.githubusercontent.com/Toni-SM/skrl/main/docs/source/_static/data/logo-light-mode.png">
 </p>
 <h2 align="center" style="border-bottom: 0 !important;">SKRL - Reinforcement Learning library</h2>
 <br>
 
-**skrl** is an open-source modular library for Reinforcement Learning written in Python (using [PyTorch](https://pytorch.org/)) and designed with a focus on readability, simplicity, and transparency of algorithm implementation. In addition to supporting the OpenAI [Gym](https://www.gymlibrary.dev) / Farama [Gymnasium](https://gymnasium.farama.org) and [DeepMind](https://github.com/deepmind/dm_env) environment interfaces, it allows loading and configuring [NVIDIA Isaac Gym](https://developer.nvidia.com/isaac-gym/) and [NVIDIA Omniverse Isaac Gym](https://docs.omniverse.nvidia.com/app_isaacsim/app_isaacsim/tutorial_gym_isaac_gym.html) environments, enabling agents' simultaneous training by scopes (subsets of environments among all available environments), which may or may not share resources, in the same run
+**skrl** is an open-source modular library for Reinforcement Learning written in Python (on top of [PyTorch](https://pytorch.org/) and [JAX](https://jax.readthedocs.io) and designed with a focus on modularity, readability, simplicity, and transparency of algorithm implementation. In addition to supporting the OpenAI [Gym](https://www.gymlibrary.dev) / Farama [Gymnasium](https://gymnasium.farama.org) and [DeepMind](https://github.com/deepmind/dm_env) and other environment interfaces, it allows loading and configuring [NVIDIA Isaac Gym](https://developer.nvidia.com/isaac-gym/), [NVIDIA Isaac Orbit](https://isaac-orbit.github.io/orbit/index.html) and [NVIDIA Omniverse Isaac Gym](https://docs.omniverse.nvidia.com/app_isaacsim/app_isaacsim/tutorial_gym_isaac_gym.html) environments, enabling agents' simultaneous training by scopes (subsets of environments among all available environments), which may or may not share resources, in the same run.
 
 <br>
 
 ### Please, visit the documentation for usage details and examples
 
 https://skrl.readthedocs.io/en/latest/
```

### Comparing `skrl-0.9.1/skrl/agents/torch/a2c/a2c.py` & `skrl-1.0.0rc1/skrl/agents/torch/a2c/a2c_rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
 import itertools
+import gym
+import gymnasium
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
-from skrl.resources.schedulers.torch import KLAdaptiveRL
-
-from skrl.agents.torch import Agent
+from skrl.resources.schedulers.torch import KLAdaptiveLR
 
 
 A2C_DEFAULT_CONFIG = {
     "rollouts": 16,                 # number of rollouts before updating
     "mini_batches": 1,              # number of mini batches to use for updating
 
     "discount_factor": 0.99,        # discount factor (gamma)
@@ -50,38 +50,38 @@
 
         "wandb": False,             # whether to use Weights & Biases
         "wandb_kwargs": {}          # wandb kwargs (see https://docs.wandb.ai/ref/python/init)
     }
 }
 
 
-class A2C(Agent):
+class A2C_RNN(Agent):
     def __init__(self,
                  models: Dict[str, Model],
                  memory: Optional[Union[Memory, Tuple[Memory]]] = None,
                  observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  device: Optional[Union[str, torch.device]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """Advantage Actor Critic (A2C)
+        """Advantage Actor Critic (A2C) with support for Recurrent Neural Networks (RNN, GRU, LSTM, etc.)
 
         https://arxiv.org/abs/1602.01783
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(A2C_DEFAULT_CONFIG)
@@ -427,15 +427,15 @@
                     rnn_value = {"rnn": [s.transpose(0, 1) for s, n in zip(sampled_rnn_batches[i], self._rnn_tensors_names) if "value" in n], "terminated": sampled_dones}
 
             sampled_states = self._state_preprocessor(sampled_states, train=True)
 
             _, next_log_prob, _ = self.policy.act({"states": sampled_states, "taken_actions": sampled_actions, **rnn_policy}, role="policy")
 
             # compute aproximate KL divergence for KLAdaptive learning rate scheduler
-            if isinstance(self.scheduler, KLAdaptiveRL):
+            if isinstance(self.scheduler, KLAdaptiveLR):
                 with torch.no_grad():
                     ratio = next_log_prob - sampled_log_prob
                     kl_divergence = ((torch.exp(ratio) - 1) - ratio).mean()
                     kl_divergences.append(kl_divergence)
 
             # compute entropy loss
             if self._entropy_loss_scale:
@@ -465,15 +465,15 @@
             cumulative_policy_loss += policy_loss.item()
             cumulative_value_loss += value_loss.item()
             if self._entropy_loss_scale:
                 cumulative_entropy_loss += entropy_loss.item()
 
         # update learning rate
         if self._learning_rate_scheduler:
-            if isinstance(self.scheduler, KLAdaptiveRL):
+            if isinstance(self.scheduler, KLAdaptiveLR):
                 self.scheduler.step(torch.tensor(kl_divergences).mean())
             else:
                 self.scheduler.step()
 
         # record data
         self.track_data("Loss / Policy loss", cumulative_policy_loss / len(sampled_batches))
         self.track_data("Loss / Value loss", cumulative_value_loss / len(sampled_batches))
```

### Comparing `skrl-0.9.1/skrl/agents/torch/amp/amp.py` & `skrl-1.0.0rc1/skrl/agents/torch/amp/amp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Callable, Union, Tuple, Dict, Any, Optional
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
-import math
 import copy
 import itertools
+import math
+import gym
+import gymnasium
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
 AMP_DEFAULT_CONFIG = {
     "rollouts": 16,                 # number of rollouts before updating
     "learning_epochs": 6,           # number of learning epochs during each update
     "mini_batches": 2,              # number of mini batches during each learning epoch
 
     "discount_factor": 0.99,        # discount factor (gamma)
@@ -93,32 +93,32 @@
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
-        :param amp_observation_space: AMP observation/state space or shape (default: None)
-        :type amp_observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None
-        :param motion_dataset: Reference motion dataset: M (default: None)
+        :param amp_observation_space: AMP observation/state space or shape (default: ``None``)
+        :type amp_observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None
+        :param motion_dataset: Reference motion dataset: M (default: ``None``)
         :type motion_dataset: skrl.memory.torch.Memory or None
-        :param reply_buffer: Reply buffer for preventing discriminator overfitting: B (default: None)
+        :param reply_buffer: Reply buffer for preventing discriminator overfitting: B (default: ``None``)
         :type reply_buffer: skrl.memory.torch.Memory or None
-        :param collect_reference_motions: Callable to collect reference motions (default: None)
+        :param collect_reference_motions: Callable to collect reference motions (default: ``None``)
         :type collect_reference_motions: Callable[[int], torch.Tensor] or None
-        :param collect_observation: Callable to collect observation (default: None)
+        :param collect_observation: Callable to collect observation (default: ``None``)
         :type collect_observation: Callable[[], torch.Tensor] or None
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(AMP_DEFAULT_CONFIG)
         _cfg.update(cfg if cfg is not None else {})
         super().__init__(models=models,
```

### Comparing `skrl-0.9.1/skrl/agents/torch/base.py` & `skrl-1.0.0rc1/skrl/agents/torch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import Union, Mapping, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Mapping, Optional, Tuple, Union
 
-import os
-import gym, gymnasium
+import collections
 import copy
 import datetime
-import collections
-import numpy as np
+import os
+import gym
+import gymnasium
 
+import numpy as np
 import torch
 from torch.utils.tensorboard import SummaryWriter
 
 from skrl import logger
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
@@ -27,20 +28,20 @@
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
         """
         self.models = models
         self.observation_space = observation_space
         self.action_space = action_space
@@ -86,22 +87,22 @@
 
     def __str__(self) -> str:
         """Generate a representation of the agent as string
 
         :return: Representation of the agent as string
         :rtype: str
         """
-        string = "Agent: {}".format(repr(self))
+        string = f"Agent: {repr(self)}"
         for k, v in self.cfg.items():
             if type(v) is dict:
-                string += "\n  |-- {}".format(k)
+                string += f"\n  |-- {k}"
                 for k1, v1 in v.items():
-                    string += "\n  |     |-- {}: {}".format(k1, v1)
+                    string += f"\n  |     |-- {k1}: {v1}"
             else:
-                string += "\n  |-- {}: {}".format(k, v)
+                string += f"\n  |-- {k}: {v}"
         return string
 
     def _empty_preprocessor(self, _input: Any, *args, **kwargs) -> Any:
         """Empty preprocess method
 
         This method is defined because PyTorch multiprocessing can't pickle lambdas
 
@@ -149,15 +150,16 @@
             wandb_kwargs.setdefault("config", {})
             wandb_kwargs["config"].update(config)
             # init Weights & Biases
             import wandb
             wandb.init(**wandb_kwargs)
 
         # main entry to log data for consumption and visualization by TensorBoard
-        self.writer = SummaryWriter(log_dir=self.experiment_dir)
+        if self.write_interval > 0:
+            self.writer = SummaryWriter(log_dir=self.experiment_dir)
 
         if self.checkpoint_interval > 0:
             os.makedirs(os.path.join(self.experiment_dir, "checkpoints"), exist_ok=True)
 
     def track_data(self, tag: str, value: float) -> None:
         """Track data to TensorBoard
 
@@ -201,35 +203,36 @@
         :param timesteps: Number of timesteps
         :type timesteps: int
         """
         tag = str(timestep if timestep is not None else datetime.datetime.now().strftime("%y-%m-%d_%H-%M-%S-%f"))
         # separated modules
         if self.checkpoint_store_separately:
             for name, module in self.checkpoint_modules.items():
-                torch.save(self._get_internal_value(module), os.path.join(self.experiment_dir, "checkpoints", "{}_{}.pt".format(name, tag)))
+                torch.save(self._get_internal_value(module),
+                           os.path.join(self.experiment_dir, "checkpoints", f"{name}_{tag}.pt"))
         # whole agent
         else:
             modules = {}
             for name, module in self.checkpoint_modules.items():
                 modules[name] = self._get_internal_value(module)
-            torch.save(modules, os.path.join(self.experiment_dir, "checkpoints", "{}_{}.pt".format("agent", tag)))
+            torch.save(modules, os.path.join(self.experiment_dir, "checkpoints", f"agent_{tag}.pt"))
 
         # best modules
         if self.checkpoint_best_modules["modules"] and not self.checkpoint_best_modules["saved"]:
             # separated modules
             if self.checkpoint_store_separately:
                 for name, module in self.checkpoint_modules.items():
                     torch.save(self.checkpoint_best_modules["modules"][name],
-                               os.path.join(self.experiment_dir, "checkpoints", "best_{}.pt".format(name)))
+                               os.path.join(self.experiment_dir, "checkpoints", f"best_{name}.pt"))
             # whole agent
             else:
                 modules = {}
                 for name, module in self.checkpoint_modules.items():
                     modules[name] = self.checkpoint_best_modules["modules"][name]
-                torch.save(modules, os.path.join(self.experiment_dir, "checkpoints", "best_{}.pt".format("agent")))
+                torch.save(modules, os.path.join(self.experiment_dir, "checkpoints", "best_agent.pt"))
             self.checkpoint_best_modules["saved"] = True
 
     def act(self,
             states: torch.Tensor,
             timestep: int,
             timesteps: int) -> torch.Tensor:
         """Process the environment's states to make a decision (actions) using the main policy
@@ -278,36 +281,36 @@
         :param infos: Additional information about the environment
         :type infos: Any type supported by the environment
         :param timestep: Current timestep
         :type timestep: int
         :param timesteps: Number of timesteps
         :type timesteps: int
         """
-        # compute the cumulative sum of the rewards and timesteps
-        if self._cumulative_rewards is None:
-            self._cumulative_rewards = torch.zeros_like(rewards, dtype=torch.float32)
-            self._cumulative_timesteps = torch.zeros_like(rewards, dtype=torch.int32)
-
-        self._cumulative_rewards.add_(rewards)
-        self._cumulative_timesteps.add_(1)
-
-        # check ended episodes
-        finished_episodes = (terminated + truncated).nonzero(as_tuple=False)
-        if finished_episodes.numel():
-
-            # storage cumulative rewards and timesteps
-            self._track_rewards.extend(self._cumulative_rewards[finished_episodes][:, 0].reshape(-1).tolist())
-            self._track_timesteps.extend(self._cumulative_timesteps[finished_episodes][:, 0].reshape(-1).tolist())
-
-            # reset the cumulative rewards and timesteps
-            self._cumulative_rewards[finished_episodes] = 0
-            self._cumulative_timesteps[finished_episodes] = 0
-
-        # record data
         if self.write_interval > 0:
+            # compute the cumulative sum of the rewards and timesteps
+            if self._cumulative_rewards is None:
+                self._cumulative_rewards = torch.zeros_like(rewards, dtype=torch.float32)
+                self._cumulative_timesteps = torch.zeros_like(rewards, dtype=torch.int32)
+
+            self._cumulative_rewards.add_(rewards)
+            self._cumulative_timesteps.add_(1)
+
+            # check ended episodes
+            finished_episodes = (terminated + truncated).nonzero(as_tuple=False)
+            if finished_episodes.numel():
+
+                # storage cumulative rewards and timesteps
+                self._track_rewards.extend(self._cumulative_rewards[finished_episodes][:, 0].reshape(-1).tolist())
+                self._track_timesteps.extend(self._cumulative_timesteps[finished_episodes][:, 0].reshape(-1).tolist())
+
+                # reset the cumulative rewards and timesteps
+                self._cumulative_rewards[finished_episodes] = 0
+                self._cumulative_timesteps[finished_episodes] = 0
+
+            # record data
             self.tracking_data["Reward / Instantaneous reward (max)"].append(torch.max(rewards).item())
             self.tracking_data["Reward / Instantaneous reward (min)"].append(torch.min(rewards).item())
             self.tracking_data["Reward / Instantaneous reward (mean)"].append(torch.mean(rewards).item())
 
             if len(self._track_rewards):
                 track_rewards = np.array(self._track_rewards)
                 track_timesteps = np.array(self._track_timesteps)
@@ -368,15 +371,15 @@
                     if hasattr(module, "load_state_dict"):
                         module.load_state_dict(data)
                         if hasattr(module, "eval"):
                             module.eval()
                     else:
                         raise NotImplementedError
                 else:
-                    logger.warning("Cannot load the {} module. The agent doesn't have such an instance".format(name))
+                    logger.warning(f"Cannot load the {name} module. The agent doesn't have such an instance")
 
     def migrate(self,
                 path: str,
                 name_map: Mapping[str, Mapping[str, str]] = {},
                 auto_mapping: bool = True,
                 verbose: bool = False) -> bool:
         """Migrate the specified extrernal checkpoint to the current agent
@@ -545,34 +548,34 @@
                 raise ValueError("Cannot identify file type")
 
         # show modules
         if verbose:
             logger.info("Modules")
             logger.info("  |-- current")
             for name, module in self.checkpoint_modules.items():
-                logger.info("  |    |-- {} ({})".format(name, type(module).__name__))
+                logger.info(f"  |    |-- {name} ({type(module).__name__})")
                 if hasattr(module, "state_dict"):
                     for k, v in module.state_dict().items():
                         if hasattr(v, "shape"):
-                            logger.info("  |    |    |-- {} : {}".format(k, list(v.shape)))
+                            logger.info(f"  |    |    |-- {k} : {list(v.shape)}")
                         else:
-                            logger.info("  |    |    |-- {} ({})".format(k, type(v).__name__))
+                            logger.info(f"  |    |    |-- {k} ({type(v).__name__})")
             logger.info("  |-- source")
             for name, module in checkpoint.items():
-                logger.info("  |    |-- {} ({})".format(name, type(module).__name__))
+                logger.info(f"  |    |-- {name} ({type(module).__name__})")
                 if name == "model":
                     for k, v in module.items():
-                        logger.info("  |    |    |-- {} : {}".format(k, list(v.shape)))
+                        logger.info(f"  |    |    |-- {k} : {list(v.shape)}")
                 else:
                     if hasattr(module, "state_dict"):
                         for k, v in module.state_dict().items():
                             if hasattr(v, "shape"):
-                                logger.info("  |    |    |-- {} : {}".format(k, list(v.shape)))
+                                logger.info(f"  |    |    |-- {k} : {list(v.shape)}")
                             else:
-                                logger.info("  |    |    |-- {} ({})".format(k, type(v).__name__))
+                                logger.info(f"  |    |    |-- {k} ({type(v).__name__})")
             logger.info("Migration")
 
         if "optimizer" in self.checkpoint_modules:
             # loaded state dict contains a parameter group that doesn't match the size of optimizer's group
             # self.checkpoint_modules["optimizer"].load_state_dict(checkpoint["optimizer"])
             pass
         # state_preprocessor
@@ -599,15 +602,15 @@
                 del checkpoint["model"]["value_mean_std.count"]
         # TODO: AMP state preprocessor
         # model
         status = True
         for name, module in self.checkpoint_modules.items():
             if module not in ["state_preprocessor", "value_preprocessor", "optimizer"] and hasattr(module, "migrate"):
                 if verbose:
-                    logger.info("Model: {} ({})".format(name, type(module).__name__))
+                    logger.info(f"Model: {name} ({type(module).__name__})")
                 status *= module.migrate(state_dict=checkpoint["model"],
                                             name_map=name_map.get(name, {}),
                                             auto_mapping=auto_mapping,
                                             verbose=verbose)
 
         self.set_mode("eval")
         return bool(status)
@@ -628,31 +631,30 @@
         :param timestep: Current timestep
         :type timestep: int
         :param timesteps: Number of timesteps
         :type timesteps: int
         """
         timestep += 1
 
-        # update best models and write data to tensorboard
-        if timestep > 1 and self.write_interval > 0 and not timestep % self.write_interval:
+        # update best models and write checkpoints
+        if timestep > 1 and self.checkpoint_interval > 0 and not timestep % self.checkpoint_interval:
             # update best models
             reward = np.mean(self.tracking_data.get("Reward / Total reward (mean)", -2 ** 31))
             if reward > self.checkpoint_best_modules["reward"]:
                 self.checkpoint_best_modules["timestep"] = timestep
                 self.checkpoint_best_modules["reward"] = reward
                 self.checkpoint_best_modules["saved"] = False
                 self.checkpoint_best_modules["modules"] = {k: copy.deepcopy(self._get_internal_value(v)) for k, v in self.checkpoint_modules.items()}
+            # write checkpoints
+            self.write_checkpoint(timestep, timesteps)
 
-            # write to tensorboard
+        # write to tensorboard
+        if timestep > 1 and self.write_interval > 0 and not timestep % self.write_interval:
             self.write_tracking_data(timestep, timesteps)
 
-        # write checkpoints
-        if timestep > 1 and self.checkpoint_interval > 0 and not timestep % self.checkpoint_interval:
-            self.write_checkpoint(timestep, timesteps)
-
     def _update(self, timestep: int, timesteps: int) -> None:
         """Algorithm's main update step
 
         :param timestep: Current timestep
         :type timestep: int
         :param timesteps: Number of timesteps
         :type timesteps: int
```

### Comparing `skrl-0.9.1/skrl/agents/torch/cem/cem.py` & `skrl-1.0.0rc1/skrl/agents/torch/cem/cem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
+import gym
+import gymnasium
 
 import torch
 import torch.nn.functional as F
 
+from skrl import logger
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
 CEM_DEFAULT_CONFIG = {
     "rollouts": 16,                 # number of rollouts before updating
     "percentile": 0.70,             # percentile to compute the reward bound [0, 1]
 
     "discount_factor": 0.99,        # discount factor (gamma)
 
@@ -58,20 +59,20 @@
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(CEM_DEFAULT_CONFIG)
@@ -261,15 +262,15 @@
                 for i, j in zip(self._episode_tracking[e][:-1], self._episode_tracking[e][1:]):
                     limits.append([e + i, e + j])
                     rewards = sampled_rewards[e + i: e + j]
                     returns.append(torch.sum(rewards * self._discount_factor ** \
                         torch.arange(rewards.size(0), device=rewards.device).flip(-1).view(rewards.size())))
 
             if not len(returns):
-                print("[WARNING] No returns to update. Consider increasing the number of rollouts")
+                logger.warning("No returns to update. Consider increasing the number of rollouts")
                 return
 
             returns = torch.tensor(returns)
             return_threshold = torch.quantile(returns, self._percentile, dim=-1)
 
             # get elite states and actions
             indexes = torch.nonzero(returns >= return_threshold)
```

### Comparing `skrl-0.9.1/skrl/agents/torch/ddpg/ddpg.py` & `skrl-1.0.0rc1/skrl/agents/torch/ddpg/ddpg_rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
+import gym
+import gymnasium
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
 DDPG_DEFAULT_CONFIG = {
     "gradient_steps": 1,            # gradient steps
     "batch_size": 64,               # training batch size
 
     "discount_factor": 0.99,        # discount factor (gamma)
     "polyak": 0.005,                # soft update hyperparameter (tau)
@@ -52,38 +52,38 @@
 
         "wandb": False,             # whether to use Weights & Biases
         "wandb_kwargs": {}          # wandb kwargs (see https://docs.wandb.ai/ref/python/init)
     }
 }
 
 
-class DDPG(Agent):
+class DDPG_RNN(Agent):
     def __init__(self,
                  models: Dict[str, Model],
                  memory: Optional[Union[Memory, Tuple[Memory]]] = None,
                  observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  device: Optional[Union[str, torch.device]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """Deep Deterministic Policy Gradient (DDPG)
+        """Deep Deterministic Policy Gradient (DDPG) with support for Recurrent Neural Networks (RNN, GRU, LSTM, etc.)
 
         https://arxiv.org/abs/1509.02971
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(DDPG_DEFAULT_CONFIG)
@@ -364,16 +364,16 @@
         if self._rnn:
             sampled_rnn = self.memory.sample_by_index(names=self._rnn_tensors_names, indexes=self.memory.get_sampling_indexes())[0]
             rnn_policy = {"rnn": [s.transpose(0, 1) for s in sampled_rnn], "terminated": sampled_dones}
 
         # gradient steps
         for gradient_step in range(self._gradient_steps):
 
-            sampled_states = self._state_preprocessor(sampled_states, train=not gradient_step)
-            sampled_next_states = self._state_preprocessor(sampled_next_states)
+            sampled_states = self._state_preprocessor(sampled_states, train=True)
+            sampled_next_states = self._state_preprocessor(sampled_next_states, train=True)
 
             # compute target values
             with torch.no_grad():
                 next_actions, _, _ = self.target_policy.act({"states": sampled_next_states, **rnn_policy}, role="target_policy")
 
                 target_q_values, _, _ = self.target_critic.act({"states": sampled_next_states, "taken_actions": next_actions, **rnn_policy}, role="target_critic")
                 target_values = sampled_rewards + self._discount_factor * sampled_dones.logical_not() * target_q_values
```

### Comparing `skrl-0.9.1/skrl/agents/torch/dqn/ddqn.py` & `skrl-1.0.0rc1/skrl/agents/torch/dqn/ddqn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
 import math
+import gym
+import gymnasium
 
 import torch
 import torch.nn.functional as F
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
 DDQN_DEFAULT_CONFIG = {
     "gradient_steps": 1,            # gradient steps
     "batch_size": 64,               # training batch size
 
     "discount_factor": 0.99,        # discount factor (gamma)
     "polyak": 0.005,                # soft update hyperparameter (tau)
@@ -69,20 +69,20 @@
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(DDQN_DEFAULT_CONFIG)
@@ -278,16 +278,16 @@
         # sample a batch from memory
         sampled_states, sampled_actions, sampled_rewards, sampled_next_states, sampled_dones = \
             self.memory.sample(names=self.tensors_names, batch_size=self._batch_size)[0]
 
         # gradient steps
         for gradient_step in range(self._gradient_steps):
 
-            sampled_states = self._state_preprocessor(sampled_states, train=not gradient_step)
-            sampled_next_states = self._state_preprocessor(sampled_next_states)
+            sampled_states = self._state_preprocessor(sampled_states, train=True)
+            sampled_next_states = self._state_preprocessor(sampled_next_states, train=True)
 
             # compute target values
             with torch.no_grad():
                 next_q_values, _, _ = self.target_q_network.act({"states": sampled_next_states}, role="target_q_network")
 
                 target_q_values = torch.gather(next_q_values, dim=1, index=torch.argmax(self.q_network.act({"states": sampled_next_states}, \
                     role="q_network")[0], dim=1, keepdim=True))
```

### Comparing `skrl-0.9.1/skrl/agents/torch/dqn/dqn.py` & `skrl-1.0.0rc1/skrl/agents/torch/dqn/dqn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
 import math
+import gym
+import gymnasium
 
 import torch
 import torch.nn.functional as F
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
 DQN_DEFAULT_CONFIG = {
     "gradient_steps": 1,            # gradient steps
     "batch_size": 64,               # training batch size
 
     "discount_factor": 0.99,        # discount factor (gamma)
     "polyak": 0.005,                # soft update hyperparameter (tau)
@@ -69,20 +69,20 @@
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(DQN_DEFAULT_CONFIG)
@@ -278,16 +278,16 @@
         # sample a batch from memory
         sampled_states, sampled_actions, sampled_rewards, sampled_next_states, sampled_dones = \
             self.memory.sample(names=self.tensors_names, batch_size=self._batch_size)[0]
 
         # gradient steps
         for gradient_step in range(self._gradient_steps):
 
-            sampled_states = self._state_preprocessor(sampled_states, train=not gradient_step)
-            sampled_next_states = self._state_preprocessor(sampled_next_states)
+            sampled_states = self._state_preprocessor(sampled_states, train=True)
+            sampled_next_states = self._state_preprocessor(sampled_next_states, train=True)
 
             # compute target values
             with torch.no_grad():
                 next_q_values, _, _ = self.target_q_network.act({"states": sampled_next_states}, role="target_q_network")
 
                 target_q_values = torch.max(next_q_values, dim=-1, keepdim=True)[0]
                 target_values = sampled_rewards + self._discount_factor * sampled_dones.logical_not() * target_q_values
```

### Comparing `skrl-0.9.1/skrl/agents/torch/ppo/ppo.py` & `skrl-1.0.0rc1/skrl/agents/torch/ppo/ppo_rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
 import itertools
+import gym
+import gymnasium
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
-from skrl.resources.schedulers.torch import KLAdaptiveRL
-
-from skrl.agents.torch import Agent
+from skrl.resources.schedulers.torch import KLAdaptiveLR
 
 
 PPO_DEFAULT_CONFIG = {
     "rollouts": 16,                 # number of rollouts before updating
     "learning_epochs": 8,           # number of learning epochs during each update
     "mini_batches": 2,              # number of mini batches during each learning epoch
 
@@ -57,38 +57,38 @@
 
         "wandb": False,             # whether to use Weights & Biases
         "wandb_kwargs": {}          # wandb kwargs (see https://docs.wandb.ai/ref/python/init)
     }
 }
 
 
-class PPO(Agent):
+class PPO_RNN(Agent):
     def __init__(self,
                  models: Dict[str, Model],
                  memory: Optional[Union[Memory, Tuple[Memory]]] = None,
                  observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  device: Optional[Union[str, torch.device]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """Proximal Policy Optimization (PPO)
+        """Proximal Policy Optimization (PPO) with support for Recurrent Neural Networks (RNN, GRU, LSTM, etc.)
 
         https://arxiv.org/abs/1707.06347
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(PPO_DEFAULT_CONFIG)
@@ -493,15 +493,15 @@
                 cumulative_policy_loss += policy_loss.item()
                 cumulative_value_loss += value_loss.item()
                 if self._entropy_loss_scale:
                     cumulative_entropy_loss += entropy_loss.item()
 
             # update learning rate
             if self._learning_rate_scheduler:
-                if isinstance(self.scheduler, KLAdaptiveRL):
+                if isinstance(self.scheduler, KLAdaptiveLR):
                     self.scheduler.step(torch.tensor(kl_divergences).mean())
                 else:
                     self.scheduler.step()
 
         # record data
         self.track_data("Loss / Policy loss", cumulative_policy_loss / (self._learning_epochs * self._mini_batches))
         self.track_data("Loss / Value loss", cumulative_value_loss / (self._learning_epochs * self._mini_batches))
```

### Comparing `skrl-0.9.1/skrl/agents/torch/q_learning/q_learning.py` & `skrl-1.0.0rc1/skrl/agents/torch/sarsa/sarsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
+import gym
+import gymnasium
 
 import torch
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
-Q_LEARNING_DEFAULT_CONFIG = {
+SARSA_DEFAULT_CONFIG = {
     "discount_factor": 0.99,        # discount factor (gamma)
 
     "random_timesteps": 0,          # random exploration steps
     "learning_starts": 0,           # learning starts after this many steps
 
     "learning_rate": 0.5,           # learning rate (alpha)
 
@@ -31,45 +31,45 @@
 
         "wandb": False,             # whether to use Weights & Biases
         "wandb_kwargs": {}          # wandb kwargs (see https://docs.wandb.ai/ref/python/init)
     }
 }
 
 
-class Q_LEARNING(Agent):
+class SARSA(Agent):
     def __init__(self,
                  models: Dict[str, Model],
                  memory: Optional[Union[Memory, Tuple[Memory]]] = None,
                  observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  device: Optional[Union[str, torch.device]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """Q-learning
+        """State Action Reward State Action (SARSA)
 
-        https://www.academia.edu/3294050/Learning_from_delayed_rewards
+        https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.17.2539
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
-        _cfg = copy.deepcopy(Q_LEARNING_DEFAULT_CONFIG)
+        _cfg = copy.deepcopy(SARSA_DEFAULT_CONFIG)
         _cfg.update(cfg if cfg is not None else {})
         super().__init__(models=models,
                          memory=memory,
                          observation_space=observation_space,
                          action_space=action_space,
                          device=device,
                          cfg=_cfg)
@@ -204,14 +204,14 @@
         :param timesteps: Number of timesteps
         :type timesteps: int
         """
         q_table = self.policy.table()
         env_ids = torch.arange(self._current_rewards.shape[0]).view(-1, 1)
 
         # compute next actions
-        next_actions = torch.argmax(q_table[env_ids, self._current_next_states], dim=-1, keepdim=True).view(-1,1)
+        next_actions = self.policy.act({"states": self._current_next_states}, role="policy")[0]
 
         # update Q-table
         q_table[env_ids, self._current_states, self._current_actions] += self._learning_rate \
             * (self._current_rewards + self._discount_factor * self._current_dones.logical_not() \
                 * q_table[env_ids, self._current_next_states, next_actions] \
                     - q_table[env_ids, self._current_states, self._current_actions])
```

### Comparing `skrl-0.9.1/skrl/agents/torch/sac/sac.py` & `skrl-1.0.0rc1/skrl/agents/torch/sac/sac_rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
 import itertools
-import numpy as np
+import gym
+import gymnasium
 
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
 SAC_DEFAULT_CONFIG = {
     "gradient_steps": 1,            # gradient steps
     "batch_size": 64,               # training batch size
 
     "discount_factor": 0.99,        # discount factor (gamma)
     "polyak": 0.005,                # soft update hyperparameter (tau)
@@ -52,38 +52,38 @@
 
         "wandb": False,             # whether to use Weights & Biases
         "wandb_kwargs": {}          # wandb kwargs (see https://docs.wandb.ai/ref/python/init)
     }
 }
 
 
-class SAC(Agent):
+class SAC_RNN(Agent):
     def __init__(self,
                  models: Dict[str, Model],
                  memory: Optional[Union[Memory, Tuple[Memory]]] = None,
                  observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  device: Optional[Union[str, torch.device]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """Soft Actor-Critic (SAC)
+        """Soft Actor-Critic (SAC) with support for Recurrent Neural Networks (RNN, GRU, LSTM, etc.)
 
         https://arxiv.org/abs/1801.01290
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(SAC_DEFAULT_CONFIG)
@@ -340,16 +340,16 @@
         if self._rnn:
             sampled_rnn = self.memory.sample_by_index(names=self._rnn_tensors_names, indexes=self.memory.get_sampling_indexes())[0]
             rnn_policy = {"rnn": [s.transpose(0, 1) for s in sampled_rnn], "terminated": sampled_dones}
 
         # gradient steps
         for gradient_step in range(self._gradient_steps):
 
-            sampled_states = self._state_preprocessor(sampled_states, train=not gradient_step)
-            sampled_next_states = self._state_preprocessor(sampled_next_states)
+            sampled_states = self._state_preprocessor(sampled_states, train=True)
+            sampled_next_states = self._state_preprocessor(sampled_next_states, train=True)
 
             # compute target values
             with torch.no_grad():
                 next_actions, next_log_prob, _ = self.policy.act({"states": sampled_next_states, **rnn_policy}, role="policy")
 
                 target_q1_values, _, _ = self.target_critic_1.act({"states": sampled_next_states, "taken_actions": next_actions, **rnn_policy}, role="target_critic_1")
                 target_q2_values, _, _ = self.target_critic_2.act({"states": sampled_next_states, "taken_actions": next_actions, **rnn_policy}, role="target_critic_2")
```

### Comparing `skrl-0.9.1/skrl/agents/torch/sarsa/sarsa.py` & `skrl-1.0.0rc1/skrl/agents/torch/q_learning/q_learning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
+import gym
+import gymnasium
 
 import torch
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
-SARSA_DEFAULT_CONFIG = {
+Q_LEARNING_DEFAULT_CONFIG = {
     "discount_factor": 0.99,        # discount factor (gamma)
 
     "random_timesteps": 0,          # random exploration steps
     "learning_starts": 0,           # learning starts after this many steps
 
     "learning_rate": 0.5,           # learning rate (alpha)
 
@@ -31,45 +31,45 @@
 
         "wandb": False,             # whether to use Weights & Biases
         "wandb_kwargs": {}          # wandb kwargs (see https://docs.wandb.ai/ref/python/init)
     }
 }
 
 
-class SARSA(Agent):
+class Q_LEARNING(Agent):
     def __init__(self,
                  models: Dict[str, Model],
                  memory: Optional[Union[Memory, Tuple[Memory]]] = None,
                  observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  device: Optional[Union[str, torch.device]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """State Action Reward State Action (SARSA)
+        """Q-learning
 
-        https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.17.2539
+        https://www.academia.edu/3294050/Learning_from_delayed_rewards
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
-        _cfg = copy.deepcopy(SARSA_DEFAULT_CONFIG)
+        _cfg = copy.deepcopy(Q_LEARNING_DEFAULT_CONFIG)
         _cfg.update(cfg if cfg is not None else {})
         super().__init__(models=models,
                          memory=memory,
                          observation_space=observation_space,
                          action_space=action_space,
                          device=device,
                          cfg=_cfg)
@@ -204,14 +204,14 @@
         :param timesteps: Number of timesteps
         :type timesteps: int
         """
         q_table = self.policy.table()
         env_ids = torch.arange(self._current_rewards.shape[0]).view(-1, 1)
 
         # compute next actions
-        next_actions = self.policy.act({"states": self._current_next_states}, role="policy")[0]
+        next_actions = torch.argmax(q_table[env_ids, self._current_next_states], dim=-1, keepdim=True).view(-1,1)
 
         # update Q-table
         q_table[env_ids, self._current_states, self._current_actions] += self._learning_rate \
             * (self._current_rewards + self._discount_factor * self._current_dones.logical_not() \
                 * q_table[env_ids, self._current_next_states, next_actions] \
                     - q_table[env_ids, self._current_states, self._current_actions])
```

### Comparing `skrl-0.9.1/skrl/agents/torch/td3/td3.py` & `skrl-1.0.0rc1/skrl/agents/torch/td3/td3_rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
 import itertools
+import gym
+import gymnasium
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from skrl import logger
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
 TD3_DEFAULT_CONFIG = {
     "gradient_steps": 1,            # gradient steps
     "batch_size": 64,               # training batch size
 
     "discount_factor": 0.99,        # discount factor (gamma)
     "polyak": 0.005,                # soft update hyperparameter (tau)
@@ -57,38 +58,38 @@
 
         "wandb": False,             # whether to use Weights & Biases
         "wandb_kwargs": {}          # wandb kwargs (see https://docs.wandb.ai/ref/python/init)
     }
 }
 
 
-class TD3(Agent):
+class TD3_RNN(Agent):
     def __init__(self,
                  models: Dict[str, Model],
                  memory: Optional[Union[Memory, Tuple[Memory]]] = None,
                  observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  device: Optional[Union[str, torch.device]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """Twin Delayed DDPG (TD3)
+        """Twin Delayed DDPG (TD3) with support for Recurrent Neural Networks (RNN, GRU, LSTM, etc.)
 
         https://arxiv.org/abs/1802.09477
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(TD3_DEFAULT_CONFIG)
@@ -151,14 +152,16 @@
         self._exploration_timesteps = self.cfg["exploration"]["timesteps"]
 
         self._policy_delay = self.cfg["policy_delay"]
         self._critic_update_counter = 0
 
         self._smooth_regularization_noise = self.cfg["smooth_regularization_noise"]
         self._smooth_regularization_clip = self.cfg["smooth_regularization_clip"]
+        if self._smooth_regularization_noise is None:
+            logger.warning("agents:TD3: No smooth regularization noise specified to reduce variance during training")
 
         self._rewards_shaper = self.cfg["rewards_shaper"]
 
         # set up optimizers and learning rate schedulers
         if self.policy is not None and self.critic_1 is not None and self.critic_2 is not None:
             self.policy_optimizer = torch.optim.Adam(self.policy.parameters(), lr=self._actor_learning_rate)
             self.critic_optimizer = torch.optim.Adam(itertools.chain(self.critic_1.parameters(), self.critic_2.parameters()),
@@ -382,29 +385,30 @@
         if self._rnn:
             sampled_rnn = self.memory.sample_by_index(names=self._rnn_tensors_names, indexes=self.memory.get_sampling_indexes())[0]
             rnn_policy = {"rnn": [s.transpose(0, 1) for s in sampled_rnn], "terminated": sampled_dones}
 
         # gradient steps
         for gradient_step in range(self._gradient_steps):
 
-            sampled_states = self._state_preprocessor(sampled_states, train=not gradient_step)
-            sampled_next_states = self._state_preprocessor(sampled_next_states)
+            sampled_states = self._state_preprocessor(sampled_states, train=True)
+            sampled_next_states = self._state_preprocessor(sampled_next_states, train=True)
 
             with torch.no_grad():
                 # target policy smoothing
                 next_actions, _, _ = self.target_policy.act({"states": sampled_next_states, **rnn_policy}, role="target_policy")
-                noises = torch.clamp(self._smooth_regularization_noise.sample(next_actions.shape),
-                                     min=-self._smooth_regularization_clip,
-                                     max=self._smooth_regularization_clip)
-                next_actions.add_(noises)
-
-                if self._backward_compatibility:
-                    next_actions = torch.max(torch.min(next_actions, self.clip_actions_max), self.clip_actions_min)
-                else:
-                    next_actions.clamp_(min=self.clip_actions_min, max=self.clip_actions_max)
+                if self._smooth_regularization_noise is not None:
+                    noises = torch.clamp(self._smooth_regularization_noise.sample(next_actions.shape),
+                                        min=-self._smooth_regularization_clip,
+                                        max=self._smooth_regularization_clip)
+                    next_actions.add_(noises)
+
+                    if self._backward_compatibility:
+                        next_actions = torch.max(torch.min(next_actions, self.clip_actions_max), self.clip_actions_min)
+                    else:
+                        next_actions.clamp_(min=self.clip_actions_min, max=self.clip_actions_max)
 
                 # compute target values
                 target_q1_values, _, _ = self.target_critic_1.act({"states": sampled_next_states, "taken_actions": next_actions, **rnn_policy}, role="target_critic_1")
                 target_q2_values, _, _ = self.target_critic_2.act({"states": sampled_next_states, "taken_actions": next_actions, **rnn_policy}, role="target_critic_2")
                 target_q_values = torch.min(target_q1_values, target_q2_values)
                 target_values = sampled_rewards + self._discount_factor * sampled_dones.logical_not() * target_q_values
```

### Comparing `skrl-0.9.1/skrl/agents/torch/trpo/trpo.py` & `skrl-1.0.0rc1/skrl/agents/torch/trpo/trpo_rnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from typing import Union, Tuple, Dict, Any, Optional
+from typing import Any, Dict, Optional, Tuple, Union
 
-import gym, gymnasium
 import copy
+import gym
+import gymnasium
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from torch.nn.utils.convert_parameters import parameters_to_vector
-from torch.nn.utils.convert_parameters import vector_to_parameters
+from torch.nn.utils.convert_parameters import parameters_to_vector, vector_to_parameters
 
+from skrl.agents.torch import Agent
 from skrl.memories.torch import Memory
 from skrl.models.torch import Model
 
-from skrl.agents.torch import Agent
-
 
 TRPO_DEFAULT_CONFIG = {
     "rollouts": 16,                 # number of rollouts before updating
     "learning_epochs": 8,           # number of learning epochs during each update
     "mini_batches": 2,              # number of mini batches during each learning epoch
 
     "discount_factor": 0.99,        # discount factor (gamma)
@@ -57,38 +56,38 @@
 
         "wandb": False,             # whether to use Weights & Biases
         "wandb_kwargs": {}          # wandb kwargs (see https://docs.wandb.ai/ref/python/init)
     }
 }
 
 
-class TRPO(Agent):
+class TRPO_RNN(Agent):
     def __init__(self,
                  models: Dict[str, Model],
                  memory: Optional[Union[Memory, Tuple[Memory]]] = None,
                  observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
                  device: Optional[Union[str, torch.device]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """Trust Region Policy Optimization (TRPO)
+        """Trust Region Policy Optimization (TRPO) with support for Recurrent Neural Networks (RNN, GRU, LSTM, etc.)
 
         https://arxiv.org/abs/1502.05477
 
         :param models: Models used by the agent
         :type models: dictionary of skrl.models.torch.Model
         :param memory: Memory to storage the transitions.
                        If it is a tuple, the first element will be used for training and
                        for the rest only the environment transitions will be added
         :type memory: skrl.memory.torch.Memory, list of skrl.memory.torch.Memory or None
-        :param observation_space: Observation/state space or shape (default: None)
-        :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param action_space: Action space or shape (default: None)
-        :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param observation_space: Observation/state space or shape (default: ``None``)
+        :type observation_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param action_space: Action space or shape (default: ``None``)
+        :type action_space: int, tuple or list of int, gym.Space, gymnasium.Space or None, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         :param cfg: Configuration dictionary
         :type cfg: dict
 
         :raises KeyError: If the models dictionary is missing a required key
         """
         _cfg = copy.deepcopy(TRPO_DEFAULT_CONFIG)
@@ -430,17 +429,17 @@
 
             :param policy: Policy
             :type policy: Model
             :param states: States
             :type states: torch.Tensor
             :param b: Vector b
             :type b: torch.Tensor
-            :param num_iterations: Number of iterations (default: 10)
+            :param num_iterations: Number of iterations (default: ``10``)
             :type num_iterations: float, optional
-            :param residual_tolerance: Residual tolerance (default: 1e-10)
+            :param residual_tolerance: Residual tolerance (default: ``1e-10``)
             :type residual_tolerance: float, optional
 
             :return: Conjugate vector
             :rtype: torch.Tensor
             """
             x = torch.zeros_like(b)
             r = b.clone()
@@ -468,15 +467,15 @@
 
             :param policy: Policy
             :type policy: Model
             :param states: States
             :type states: torch.Tensor
             :param vector: Vector
             :type vector: torch.Tensor
-            :param damping: Damping (default: 0.1)
+            :param damping: Damping (default: ``0.1``)
             :type damping: float, optional
 
             :return: Hessian vector product
             :rtype: torch.Tensor
             """
             kl = kl_divergence(policy, policy, states)
             kl_gradient = torch.autograd.grad(kl, policy.parameters(), create_graph=True)
```

### Comparing `skrl-0.9.1/skrl/envs/torch/loaders.py` & `skrl-1.0.0rc1/skrl/envs/torch/loaders/isaacgym_envs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from typing import Optional, Sequence
+
 import os
 import sys
-import queue
 from contextlib import contextmanager
 
+from skrl import logger
+
+
 __all__ = ["load_isaacgym_env_preview2",
            "load_isaacgym_env_preview3",
-           "load_isaacgym_env_preview4",
-           "load_omniverse_isaacgym_env"]
+           "load_isaacgym_env_preview4"]
 
 
 @contextmanager
 def cwd(new_path: str) -> None:
     """Context manager to change the current working directory
 
     This function restores the current working directory after the context manager exits
@@ -43,35 +46,50 @@
     return d
 
 def _print_cfg(d, indent=0) -> None:
     """Print the environment configuration
 
     :param d: The dictionary to print
     :type d: dict
-    :param indent: The indentation level (default: 0)
+    :param indent: The indentation level (default: ``0``)
     :type indent: int, optional
     """
     for key, value in d.items():
         if isinstance(value, dict):
             _print_cfg(value, indent + 1)
         else:
-            print('  |   ' * indent + "  |-- {}: {}".format(key, value))
+            print("  |   " * indent + f"  |-- {key}: {value}")
 
 
-def load_isaacgym_env_preview2(task_name: str = "", isaacgymenvs_path: str = "", show_cfg: bool = True):
+def load_isaacgym_env_preview2(task_name: str = "",
+                               num_envs: Optional[int] = None,
+                               headless: Optional[bool] = None,
+                               cli_args: Sequence[str] = [],
+                               isaacgymenvs_path: str = "",
+                               show_cfg: bool = True):
     """Load an Isaac Gym environment (preview 2)
 
-    :param task_name: The name of the task (default: "").
+    :param task_name: The name of the task (default: ``""``).
                       If not specified, the task name is taken from the command line argument (``--task TASK_NAME``).
                       Command line argument has priority over function parameter if both are specified
     :type task_name: str, optional
-    :param isaacgymenvs_path: The path to the ``rlgpu`` directory (default: "").
+    :param num_envs: Number of parallel environments to create (default: ``None``).
+                     If not specified, the default number of environments defined in the task configuration is used.
+                     Command line argument has priority over function parameter if both are specified
+    :type num_envs: int, optional
+    :param headless: Whether to use headless mode (no rendering) (default: ``None``).
+                     If not specified, the default task configuration is used.
+                     Command line argument has priority over function parameter if both are specified
+    :type headless: bool, optional
+    :param cli_args: Isaac Gym environment configuration and command line arguments (default: ``[]``)
+    :type cli_args: list of str, optional
+    :param isaacgymenvs_path: The path to the ``rlgpu`` directory (default: ``""``).
                               If empty, the path will obtained from isaacgym package metadata
     :type isaacgymenvs_path: str, optional
-    :param show_cfg: Whether to print the configuration (default: True)
+    :param show_cfg: Whether to print the configuration (default: ``True``)
     :type show_cfg: bool, optional
 
     :raises ValueError: The task name has not been defined,
                         neither by the function parameter nor by the command line arguments
     :raises RuntimeError: The isaacgym package is not installed or the path is wrong
 
     :return: Isaac Gym environment (preview 2)
@@ -87,113 +105,190 @@
             break
     # get task name from command line arguments
     if defined:
         arg_index = sys.argv.index("--task") + 1
         if arg_index >= len(sys.argv):
             raise ValueError("No task name defined. Set the task_name parameter or use --task <task_name> as command line argument")
         if task_name and task_name != sys.argv[arg_index]:
-            print("[WARNING] Overriding task ({}) with command line argument ({})".format(task_name, sys.argv[arg_index]))
+            logger.warning(f"Overriding task ({task_name}) with command line argument ({sys.argv[arg_index]})")
     # get task name from function arguments
     else:
         if task_name:
             sys.argv.append("--task")
             sys.argv.append(task_name)
         else:
             raise ValueError("No task name defined. Set the task_name parameter or use --task <task_name> as command line argument")
 
+    # check num_envs from command line arguments
+    defined = False
+    for arg in sys.argv:
+        if arg.startswith("--num_envs"):
+            defined = True
+            break
+    # get num_envs from command line arguments
+    if defined:
+        if num_envs is not None:
+            logger.warning("Overriding num_envs with command line argument --num_envs")
+    # get num_envs from function arguments
+    elif num_envs is not None and num_envs > 0:
+        sys.argv.append("--num_envs")
+        sys.argv.append(str(num_envs))
+
+    # check headless from command line arguments
+    defined = False
+    for arg in sys.argv:
+        if arg.startswith("--headless"):
+            defined = True
+            break
+    # get headless from command line arguments
+    if defined:
+        if headless is not None:
+            logger.warning("Overriding headless with command line argument --headless")
+    # get headless from function arguments
+    elif headless is not None:
+        sys.argv.append("--headless")
+
+    # others command line arguments
+    sys.argv += cli_args
+
     # get isaacgym envs path from isaacgym package metadata
     if not isaacgymenvs_path:
         if not hasattr(isaacgym, "__path__"):
             raise RuntimeError("isaacgym package is not installed or could not be accessed by the current Python environment")
         path = isaacgym.__path__
         path = os.path.join(path[0], "..", "rlgpu")
     else:
         path = isaacgymenvs_path
 
     # import required packages
     sys.path.append(path)
 
     status = True
     try:
-        from utils.config import get_args, load_cfg, parse_sim_params
-        from utils.parse_task import parse_task
+        from utils.config import get_args, load_cfg, parse_sim_params  # type: ignore
+        from utils.parse_task import parse_task  # type: ignore
     except Exception as e:
         status = False
-        print("[ERROR] Failed to import required packages: {}".format(e))
+        logger.error(f"Failed to import required packages: {e}")
     if not status:
-        raise RuntimeError("The path ({}) is not valid or the isaacgym package is not installed in editable mode (pip install -e .)" \
-            .format(path))
+        raise RuntimeError(f"Path ({path}) is not valid or the isaacgym package is not installed in editable mode (pip install -e .)")
 
     args = get_args()
 
     # print config
     if show_cfg:
-        print("\nIsaac Gym environment ({})".format(args.task))
+        print(f"\nIsaac Gym environment ({args.task})")
         _print_cfg(vars(args))
 
     # update task arguments
     args.cfg_train = os.path.join(path, args.cfg_train)
     args.cfg_env = os.path.join(path, args.cfg_env)
 
     # load environment
     with cwd(path):
         cfg, cfg_train, _ = load_cfg(args)
         sim_params = parse_sim_params(args, cfg, cfg_train)
         task, env = parse_task(args, cfg, cfg_train, sim_params)
 
     return env
 
-def load_isaacgym_env_preview3(task_name: str = "", isaacgymenvs_path: str = "", show_cfg: bool = True):
+def load_isaacgym_env_preview3(task_name: str = "",
+                               num_envs: Optional[int] = None,
+                               headless: Optional[bool] = None,
+                               cli_args: Sequence[str] = [],
+                               isaacgymenvs_path: str = "",
+                               show_cfg: bool = True):
     """Load an Isaac Gym environment (preview 3)
 
     Isaac Gym benchmark environments: https://github.com/NVIDIA-Omniverse/IsaacGymEnvs
 
-    :param task_name: The name of the task (default: "").
+    :param task_name: The name of the task (default: ``""``).
                       If not specified, the task name is taken from the command line argument (``task=TASK_NAME``).
                       Command line argument has priority over function parameter if both are specified
     :type task_name: str, optional
-    :param isaacgymenvs_path: The path to the ``isaacgymenvs`` directory (default: "").
+    :param num_envs: Number of parallel environments to create (default: ``None``).
+                     If not specified, the default number of environments defined in the task configuration is used.
+                     Command line argument has priority over function parameter if both are specified
+    :type num_envs: int, optional
+    :param headless: Whether to use headless mode (no rendering) (default: ``None``).
+                     If not specified, the default task configuration is used.
+                     Command line argument has priority over function parameter if both are specified
+    :type headless: bool, optional
+    :param cli_args: IsaacGymEnvs configuration and command line arguments (default: ``[]``)
+    :type cli_args: list of str, optional
+    :param isaacgymenvs_path: The path to the ``isaacgymenvs`` directory (default: ``""``).
                               If empty, the path will obtained from isaacgymenvs package metadata
     :type isaacgymenvs_path: str, optional
-    :param show_cfg: Whether to print the configuration (default: True)
+    :param show_cfg: Whether to print the configuration (default: ``True``)
     :type show_cfg: bool, optional
 
     :raises ValueError: The task name has not been defined, neither by the function parameter nor by the command line arguments
     :raises RuntimeError: The isaacgymenvs package is not installed or the path is wrong
 
     :return: Isaac Gym environment (preview 3)
     :rtype: isaacgymenvs.tasks.base.vec_task.VecTask
     """
-    from hydra.types import RunMode
+    import isaacgym
+    import isaacgymenvs
     from hydra._internal.hydra import Hydra
     from hydra._internal.utils import create_automatic_config_search_path, get_args_parser
-
+    from hydra.types import RunMode
     from omegaconf import OmegaConf
 
-    import isaacgym
-    import isaacgymenvs
-
     # check task from command line arguments
     defined = False
     for arg in sys.argv:
         if arg.startswith("task="):
             defined = True
             break
     # get task name from command line arguments
     if defined:
         if task_name and task_name != arg.split("task=")[1].split(" ")[0]:
-            print("[WARNING] Overriding task name ({}) with command line argument ({})" \
+            logger.warning("Overriding task name ({}) with command line argument ({})" \
                 .format(task_name, arg.split("task=")[1].split(" ")[0]))
     # get task name from function arguments
     else:
         if task_name:
-            sys.argv.append("task={}".format(task_name))
+            sys.argv.append(f"task={task_name}")
         else:
             raise ValueError("No task name defined. Set task_name parameter or use task=<task_name> as command line argument")
 
+    # check num_envs from command line arguments
+    defined = False
+    for arg in sys.argv:
+        if arg.startswith("num_envs="):
+            defined = True
+            break
+    # get num_envs from command line arguments
+    if defined:
+        if num_envs is not None and num_envs != int(arg.split("num_envs=")[1].split(" ")[0]):
+            logger.warning("Overriding num_envs ({}) with command line argument (num_envs={})" \
+                .format(num_envs, arg.split("num_envs=")[1].split(" ")[0]))
+    # get num_envs from function arguments
+    elif num_envs is not None and num_envs > 0:
+        sys.argv.append(f"num_envs={num_envs}")
+
+    # check headless from command line arguments
+    defined = False
+    for arg in sys.argv:
+        if arg.startswith("headless="):
+            defined = True
+            break
+    # get headless from command line arguments
+    if defined:
+        if headless is not None and str(headless).lower() != arg.split("headless=")[1].split(" ")[0].lower():
+            logger.warning("Overriding headless ({}) with command line argument (headless={})" \
+                .format(headless, arg.split("headless=")[1].split(" ")[0]))
+    # get headless from function arguments
+    elif headless is not None:
+        sys.argv.append(f"headless={headless}")
+
+    # others command line arguments
+    sys.argv += cli_args
+
     # get isaacgymenvs path from isaacgymenvs package metadata
     if isaacgymenvs_path == "":
         if not hasattr(isaacgymenvs, "__path__"):
             raise RuntimeError("isaacgymenvs package is not installed")
         isaacgymenvs_path = list(isaacgymenvs.__path__)[0]
     config_path = os.path.join(isaacgymenvs_path, "cfg")
 
@@ -222,20 +317,20 @@
     hydra_object = Hydra.create_main_hydra2(task_name='load_isaacgymenv', config_search_path=search_path)
     config = hydra_object.compose_config(config_file, args.overrides, run_mode=RunMode.RUN)
 
     cfg = _omegaconf_to_dict(config.task)
 
     # print config
     if show_cfg:
-        print("\nIsaac Gym environment ({})".format(config.task.name))
+        print(f"\nIsaac Gym environment ({config.task.name})")
         _print_cfg(cfg)
 
     # load environment
     sys.path.append(isaacgymenvs_path)
-    from tasks import isaacgym_task_map
+    from tasks import isaacgym_task_map  # type: ignore
     try:
         env = isaacgym_task_map[config.task.name](cfg=cfg,
                                                   sim_device=config.sim_device,
                                                   graphics_device_id=config.graphics_device_id,
                                                   headless=config.headless)
     except TypeError as e:
         env = isaacgym_task_map[config.task.name](cfg=cfg,
@@ -244,210 +339,44 @@
                                                   graphics_device_id=config.graphics_device_id,
                                                   headless=config.headless,
                                                   virtual_screen_capture=config.capture_video,  # TODO: check
                                                   force_render=config.force_render)
 
     return env
 
-def load_isaacgym_env_preview4(task_name: str = "", isaacgymenvs_path: str = "", show_cfg: bool = True):
+def load_isaacgym_env_preview4(task_name: str = "",
+                               num_envs: Optional[int] = None,
+                               headless: Optional[bool] = None,
+                               cli_args: Sequence[str] = [],
+                               isaacgymenvs_path: str = "",
+                               show_cfg: bool = True):
     """Load an Isaac Gym environment (preview 4)
 
     Isaac Gym benchmark environments: https://github.com/NVIDIA-Omniverse/IsaacGymEnvs
 
-    :param task_name: The name of the task (default: "").
+    :param task_name: The name of the task (default: ``""``).
                       If not specified, the task name is taken from the command line argument (``task=TASK_NAME``).
                       Command line argument has priority over function parameter if both are specified
     :type task_name: str, optional
-    :param isaacgymenvs_path: The path to the ``isaacgymenvs`` directory (default: "").
+    :param num_envs: Number of parallel environments to create (default: ``None``).
+                     If not specified, the default number of environments defined in the task configuration is used.
+                     Command line argument has priority over function parameter if both are specified
+    :type num_envs: int, optional
+    :param headless: Whether to use headless mode (no rendering) (default: ``None``).
+                     If not specified, the default task configuration is used.
+                     Command line argument has priority over function parameter if both are specified
+    :type headless: bool, optional
+    :param cli_args: IsaacGymEnvs configuration and command line arguments (default: ``[]``)
+    :type cli_args: list of str, optional
+    :param isaacgymenvs_path: The path to the ``isaacgymenvs`` directory (default: ``""``).
                               If empty, the path will obtained from isaacgymenvs package metadata
     :type isaacgymenvs_path: str, optional
-    :param show_cfg: Whether to print the configuration (default: True)
+    :param show_cfg: Whether to print the configuration (default: ``True``)
     :type show_cfg: bool, optional
 
     :raises ValueError: The task name has not been defined, neither by the function parameter nor by the command line arguments
     :raises RuntimeError: The isaacgymenvs package is not installed or the path is wrong
 
     :return: Isaac Gym environment (preview 4)
     :rtype: isaacgymenvs.tasks.base.vec_task.VecTask
     """
-    return load_isaacgym_env_preview3(task_name, isaacgymenvs_path, show_cfg)
-
-def load_omniverse_isaacgym_env(task_name: str = "",
-                                omniisaacgymenvs_path: str = "",
-                                show_cfg: bool = True,
-                                multi_threaded: bool = False,
-                                timeout: int = 30):
-    """Load an Omniverse Isaac Gym environment
-
-    Omniverse Isaac Gym benchmark environments: https://github.com/NVIDIA-Omniverse/OmniIsaacGymEnvs
-
-    :param task_name: The name of the task (default: "").
-                      If not specified, the task name is taken from the command line argument (``task=TASK_NAME``).
-                      Command line argument has priority over function parameter if both are specified
-    :type task_name: str, optional
-    :param omniisaacgymenvs_path: The path to the ``omniisaacgymenvs`` directory (default: "").
-                              If empty, the path will obtained from omniisaacgymenvs package metadata
-    :type omniisaacgymenvs_path: str, optional
-    :param show_cfg: Whether to print the configuration (default: True)
-    :type show_cfg: bool, optional
-    :param multi_threaded: Whether to use multi-threaded environment (default: False)
-    :type multi_threaded: bool, optional
-    :param timeout: Seconds to wait for data when queue is empty in multi-threaded environment (default: 30)
-    :type timeout: int, optional
-
-    :raises ValueError: The task name has not been defined, neither by the function parameter nor by the command line arguments
-    :raises RuntimeError: The omniisaacgymenvs package is not installed or the path is wrong
-
-    :return: Omniverse Isaac Gym environment
-    :rtype: omni.isaac.gym.vec_env.vec_env_base.VecEnvBase or omni.isaac.gym.vec_env.vec_env_mt.VecEnvMT
-    """
-    import torch
-    from hydra.types import RunMode
-    from hydra._internal.hydra import Hydra
-    from hydra._internal.utils import create_automatic_config_search_path, get_args_parser
-
-    from omegaconf import OmegaConf
-
-    from omni.isaac.gym.vec_env import VecEnvBase, VecEnvMT, TaskStopException
-    from omni.isaac.gym.vec_env.vec_env_mt import TrainerMT
-
-    import omniisaacgymenvs
-
-    # check task from command line arguments
-    defined = False
-    for arg in sys.argv:
-        if arg.startswith("task="):
-            defined = True
-            break
-    # get task name from command line arguments
-    if defined:
-        if task_name and task_name != arg.split("task=")[1].split(" ")[0]:
-            print("[WARNING] Overriding task name ({}) with command line argument ({})" \
-                .format(task_name, arg.split("task=")[1].split(" ")[0]))
-    # get task name from function arguments
-    else:
-        if task_name:
-            sys.argv.append("task={}".format(task_name))
-        else:
-            raise ValueError("No task name defined. Set task_name parameter or use task=<task_name> as command line argument")
-
-    # get omniisaacgymenvs path from omniisaacgymenvs package metadata
-    if omniisaacgymenvs_path == "":
-        if not hasattr(omniisaacgymenvs, "__path__"):
-            raise RuntimeError("omniisaacgymenvs package is not installed")
-        omniisaacgymenvs_path = list(omniisaacgymenvs.__path__)[0]
-    config_path = os.path.join(omniisaacgymenvs_path, "cfg")
-
-    # set omegaconf resolvers
-    OmegaConf.register_new_resolver('eq', lambda x, y: x.lower() == y.lower())
-    OmegaConf.register_new_resolver('contains', lambda x, y: x.lower() in y.lower())
-    OmegaConf.register_new_resolver('if', lambda condition, a, b: a if condition else b)
-    OmegaConf.register_new_resolver('resolve_default', lambda default, arg: default if arg == '' else arg)
-
-    # get hydra config without use @hydra.main
-    config_file = "config"
-    args = get_args_parser().parse_args()
-    search_path = create_automatic_config_search_path(config_file, None, config_path)
-    hydra_object = Hydra.create_main_hydra2(task_name='load_omniisaacgymenv', config_search_path=search_path)
-    config = hydra_object.compose_config(config_file, args.overrides, run_mode=RunMode.RUN)
-
-    cfg = {}
-    cfg["task"] = _omegaconf_to_dict(config.task)
-    cfg["task_name"] = config.task_name
-    cfg["experiment"] = config.experiment
-    cfg["num_envs"] = config.num_envs
-    cfg["seed"] = config.seed
-    cfg["torch_deterministic"] = config.torch_deterministic
-    cfg["max_iterations"] = config.max_iterations
-    cfg["physics_engine"] = config.physics_engine
-    cfg["pipeline"] = config.pipeline
-    cfg["sim_device"] = config.sim_device
-    cfg["device_id"] = config.device_id
-    cfg["rl_device"] = config.rl_device
-    cfg["num_threads"] = config.num_threads
-    cfg["solver_type"] = config.solver_type
-    cfg["test"] = config.test
-    cfg["checkpoint"] = config.checkpoint
-    cfg["headless"] = config.headless
-
-    # print config
-    if show_cfg:
-        print("\nOmniverse Isaac Gym environment ({})".format(config.task.name))
-        _print_cfg(cfg)
-
-    # internal classes
-    class _OmniIsaacGymVecEnv(VecEnvBase):
-        def step(self, actions):
-            actions = torch.clamp(actions, -self._task.clip_actions, self._task.clip_actions).to(self._task.device).clone()
-            self._task.pre_physics_step(actions)
-
-            for _ in range(self._task.control_frequency_inv):
-                self._world.step(render=self._render)
-                self.sim_frame_count += 1
-
-            observations, rewards, dones, info = self._task.post_physics_step()
-
-            return {"obs": torch.clamp(observations, -self._task.clip_obs, self._task.clip_obs).to(self._task.rl_device).clone()}, \
-                rewards.to(self._task.rl_device).clone(), dones.to(self._task.rl_device).clone(), info.copy()
-
-        def reset(self):
-            self._task.reset()
-            actions = torch.zeros((self.num_envs, self._task.num_actions), device=self._task.device)
-            return self.step(actions)[0]
-
-    class _OmniIsaacGymTrainerMT(TrainerMT):
-        def run(self):
-            pass
-
-        def stop(self):
-            pass
-
-    class _OmniIsaacGymVecEnvMT(VecEnvMT):
-        def __init__(self, headless):
-            super().__init__(headless)
-
-            self.action_queue = queue.Queue(1)
-            self.data_queue = queue.Queue(1)
-
-        def run(self, trainer=None):
-            super().run(_OmniIsaacGymTrainerMT() if trainer is None else trainer)
-
-        def _parse_data(self, data):
-            self._observations = torch.clamp(data["obs"], -self._task.clip_obs, self._task.clip_obs).to(self._task.rl_device).clone()
-            self._rewards = data["rew"].to(self._task.rl_device).clone()
-            self._dones = data["reset"].to(self._task.rl_device).clone()
-            self._info = data["extras"].copy()
-
-        def step(self, actions):
-            if self._stop:
-                raise TaskStopException()
-
-            actions = torch.clamp(actions, -self._task.clip_actions, self._task.clip_actions).clone()
-
-            self.send_actions(actions)
-            data = self.get_data()
-
-            return {"obs": self._observations}, self._rewards, self._dones, self._info
-
-        def reset(self):
-            self._task.reset()
-            actions = torch.zeros((self.num_envs, self._task.num_actions), device=self._task.device)
-            return self.step(actions)[0]
-
-        def close(self):
-            # end stop signal to main thread
-            self.send_actions(None)
-            self.stop = True
-
-    # load environment
-    sys.path.append(omniisaacgymenvs_path)
-    from utils.task_util import initialize_task
-
-    if multi_threaded:
-        env = _OmniIsaacGymVecEnvMT(headless=config.headless)
-        task = initialize_task(cfg, env, init_sim=False)
-        env.initialize(env.action_queue, env.data_queue, timeout=timeout)
-    else:
-        env = _OmniIsaacGymVecEnv(headless=config.headless)
-        task = initialize_task(cfg, env, init_sim=True)
-
-    return env
+    return load_isaacgym_env_preview3(task_name, num_envs, headless, cli_args, isaacgymenvs_path, show_cfg)
```

### Comparing `skrl-0.9.1/skrl/memories/torch/base.py` & `skrl-1.0.0rc1/skrl/memories/torch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Optional, Union, Tuple, List
+from typing import List, Optional, Tuple, Union
 
-import os
 import csv
-import gym
-import gymnasium
-import operator
 import datetime
 import functools
-import numpy as np
+import operator
+import os
+import gym
+import gymnasium
 
+import numpy as np
 import torch
 from torch.utils.data.sampler import BatchSampler
 
 
 class Memory:
     def __init__(self,
                  memory_size: int,
@@ -24,26 +24,26 @@
         """Base class representing a memory with circular buffers
 
         Buffers are torch tensors with shape (memory size, number of environments, data size).
         Circular buffers are implemented with two integers: a memory index and an environment index
 
         :param memory_size: Maximum number of elements in the first dimension of each internal storage
         :type memory_size: int
-        :param num_envs: Number of parallel environments (default: 1)
+        :param num_envs: Number of parallel environments (default: ``1``)
         :type num_envs: int, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
-        :param export: Export the memory to a file (default: False).
+        :param export: Export the memory to a file (default: ``False``).
                        If True, the memory will be exported when the memory is filled
         :type export: bool, optional
-        :param export_format: Export format (default: "pt").
+        :param export_format: Export format (default: ``"pt"``).
                               Supported formats: torch (pt), numpy (np), comma separated values (csv)
         :type export_format: str, optional
-        :param export_directory: Directory where the memory will be exported (default: "").
+        :param export_directory: Directory where the memory will be exported (default: ``""``).
                                  If empty, the agent's experiment directory will be used
         :type export_directory: str, optional
 
         :raises ValueError: The export format is not supported
         """
         self.memory_size = memory_size
         self.num_envs = num_envs
@@ -63,15 +63,15 @@
 
         # exporting data
         self.export = export
         self.export_format = export_format
         self.export_directory = export_directory
 
         if not self.export_format in ["pt", "np", "csv"]:
-            raise ValueError("Export format not supported ({})".format(self.export_format))
+            raise ValueError(f"Export format not supported ({self.export_format})")
 
     def __len__(self) -> int:
         """Compute and return the current (valid) size of the memory
 
         The valid size is calculated as the ``memory_size * num_envs`` if the memory is full (filled).
         Otherwise, the ``memory_index * num_envs + env_index`` is returned
 
@@ -83,20 +83,20 @@
     def _get_space_size(self,
                         space: Union[int, Tuple[int], gym.Space, gymnasium.Space],
                         keep_dimensions: bool = False) -> Union[Tuple, int]:
         """Get the size (number of elements) of a space
 
         :param space: Space or shape from which to obtain the number of elements
         :type space: int, tuple or list of integers, gym.Space, or gymnasium.Space
-        :param keep_dimensions: Whether or not to keep the space dimensions (default: False)
-        :type keep_dimensions: bool
+        :param keep_dimensions: Whether or not to keep the space dimensions (default: ``False``)
+        :type keep_dimensions: bool, optional
 
         :raises ValueError: If the space is not supported
 
-        :return: Size of the space. If keep_dimensions is True, the space size will be a tuple
+        :return: Size of the space. If ``keep_dimensions`` is True, the space size will be a tuple
         :rtype: int or tuple of int
         """
         if type(space) in [int, float]:
             return (int(space),) if keep_dimensions else int(space)
         elif type(space) in [tuple, list]:
             return tuple(space) if keep_dimensions else np.prod(space)
         elif issubclass(type(space), gym.Space):
@@ -113,15 +113,15 @@
                 return (1,) if keep_dimensions else 1
             elif issubclass(type(space), gymnasium.spaces.Box):
                 return tuple(space.shape) if keep_dimensions else np.prod(space.shape)
             elif issubclass(type(space), gymnasium.spaces.Dict):
                 if keep_dimensions:
                     raise ValueError("keep_dimensions=True cannot be used with Dict spaces")
                 return sum([self._get_space_size(space.spaces[key]) for key in space.spaces])
-        raise ValueError("Space type {} not supported".format(type(space)))
+        raise ValueError(f"Space type {type(space)} not supported")
 
     def share_memory(self) -> None:
         """Share the tensors between processes
         """
         for tensor in self.tensors.values():
             if not tensor.is_cuda:
                 tensor.share_memory_()
@@ -135,15 +135,15 @@
         return sorted(self.tensors.keys())
 
     def get_tensor_by_name(self, name: str, keepdim: bool = True) -> torch.Tensor:
         """Get a tensor by its name
 
         :param name: Name of the tensor to retrieve
         :type name: str
-        :param keepdim: Keep the tensor's shape (memory size, number of environments, size) (default: True)
+        :param keepdim: Keep the tensor's shape (memory size, number of environments, size) (default: ``True``)
                         If False, the returned tensor will have a shape of (memory size * number of environments, size)
         :type keepdim: bool, optional
 
         :raises KeyError: The tensor does not exist
 
         :return: Tensor
         :rtype: torch.Tensor
@@ -174,42 +174,42 @@
         The internal representation will use _tensor_<name> as the name of the class property
 
         :param name: Tensor name (the name has to follow the python PEP 8 style)
         :type name: str
         :param size: Number of elements in the last dimension (effective data size).
                      The product of the elements will be computed for sequences or gym/gymnasium spaces
         :type size: int, tuple or list of integers, gym.Space, or gymnasium.Space
-        :param dtype: Data type (torch.dtype).
-                      If None, the global default torch data type will be used (default)
+        :param dtype: Data type (torch.dtype) (default: ``None``).
+                      If None, the global default torch data type will be used
         :type dtype: torch.dtype or None, optional
-        :param keep_dimensions: Whether or not to keep the dimensions defined through the size parameter (default: False)
-        :type keep_dimensions: bool
+        :param keep_dimensions: Whether or not to keep the dimensions defined through the size parameter (default: ``False``)
+        :type keep_dimensions: bool, optional
 
         :raises ValueError: The tensor name exists already but the size or dtype are different
 
         :return: True if the tensor was created, otherwise False
         :rtype: bool
         """
         # compute data size
         size = self._get_space_size(size, keep_dimensions)
         # check dtype and size if the tensor exists
         if name in self.tensors:
             tensor = self.tensors[name]
             if tensor.size(-1) != size:
-                raise ValueError("The size of the tensor {} ({}) doesn't match the existing one ({})".format(name, size, tensor.size(-1)))
+                raise ValueError(f"Size of tensor {name} ({size}) doesn't match the existing one ({tensor.size(-1)})")
             if dtype is not None and tensor.dtype != dtype:
-                raise ValueError("The dtype of the tensor {} ({}) doesn't match the existing one ({})".format(name, dtype, tensor.dtype))
+                raise ValueError(f"Dtype of tensor {name} ({dtype}) doesn't match the existing one ({tensor.dtype})")
             return False
         # define tensor shape
         tensor_shape = (self.memory_size, self.num_envs, *size) if keep_dimensions else (self.memory_size, self.num_envs, size)
         view_shape = (-1, *size) if keep_dimensions else (-1, size)
         # create tensor (_tensor_<name>) and add it to the internal storage
-        setattr(self, "_tensor_{}".format(name), torch.zeros(tensor_shape, device=self.device, dtype=dtype))
+        setattr(self, f"_tensor_{name}", torch.zeros(tensor_shape, device=self.device, dtype=dtype))
         # update internal variables
-        self.tensors[name] = getattr(self, "_tensor_{}".format(name))
+        self.tensors[name] = getattr(self, f"_tensor_{name}")
         self.tensors_view[name] = self.tensors[name].view(*view_shape)
         self.tensors_keep_dimensions[name] = keep_dimensions
         # fill the tensors (float tensors) with NaN
         for tensor in self.tensors.values():
             if torch.is_floating_point(tensor):
                 tensor.fill_(float("nan"))
         return True
@@ -287,15 +287,15 @@
         # single environment
         elif dim == 1:
             for name, tensor in tensors.items():
                 if name in self.tensors:
                     self.tensors[name][self.memory_index, self.env_index].copy_(tensor)
             self.env_index += 1
         else:
-            raise ValueError("Expected tensors with 2-components shape (number of environments = {}, data size), got {}".format(self.num_envs, shape))
+            raise ValueError(f"Expected shape (number of environments = {self.num_envs}, data size), got {shape}")
 
         # update indexes and flags
         if self.env_index >= self.num_envs:
             self.env_index = 0
             self.memory_index += 1
         if self.memory_index >= self.memory_size:
             self.memory_index = 0
@@ -312,17 +312,17 @@
                sequence_length: int = 1) -> List[List[torch.Tensor]]:
         """Data sampling method to be implemented by the inheriting classes
 
         :param names: Tensors names from which to obtain the samples
         :type names: tuple or list of strings
         :param batch_size: Number of element to sample
         :type batch_size: int
-        :param mini_batches: Number of mini-batches to sample (default: 1)
+        :param mini_batches: Number of mini-batches to sample (default: ``1``)
         :type mini_batches: int, optional
-        :param sequence_length: Length of each sequence (default: 1)
+        :param sequence_length: Length of each sequence (default: ``1``)
         :type sequence_length: int, optional
 
         :raises NotImplementedError: The method has not been implemented
 
         :return: Sampled data from tensors sorted according to their position in the list of names.
                  The sampled tensors will have the following shape: (batch size, data size)
         :rtype: list of torch.Tensor list
@@ -332,15 +332,15 @@
     def sample_by_index(self, names: Tuple[str], indexes: Union[tuple, np.ndarray, torch.Tensor], mini_batches: int = 1) -> List[List[torch.Tensor]]:
         """Sample data from memory according to their indexes
 
         :param names: Tensors names from which to obtain the samples
         :type names: tuple or list of strings
         :param indexes: Indexes used for sampling
         :type indexes: tuple or list, numpy.ndarray or torch.Tensor
-        :param mini_batches: Number of mini-batches to sample (default: 1)
+        :param mini_batches: Number of mini-batches to sample (default: ``1``)
         :type mini_batches: int, optional
 
         :return: Sampled data from tensors sorted according to their position in the list of names.
                  The sampled tensors will have the following shape: (number of indexes, data size)
         :rtype: list of torch.Tensor list
         """
         if mini_batches > 1:
@@ -349,17 +349,17 @@
         return [[self.tensors_view[name][indexes] for name in names]]
 
     def sample_all(self, names: Tuple[str], mini_batches: int = 1, sequence_length: int = 1) -> List[List[torch.Tensor]]:
         """Sample all data from memory
 
         :param names: Tensors names from which to obtain the samples
         :type names: tuple or list of strings
-        :param mini_batches: Number of mini-batches to sample (default: 1)
+        :param mini_batches: Number of mini-batches to sample (default: ``1``)
         :type mini_batches: int, optional
-        :param sequence_length: Length of each sequence (default: 1)
+        :param sequence_length: Length of each sequence (default: ``1``)
         :type sequence_length: int, optional
 
         :return: Sampled data from memory.
                  The sampled tensors will have the following shape: (memory size * number of environments, data size)
         :rtype: list of torch.Tensor list
         """
         # sequential order
@@ -392,15 +392,15 @@
         - PyTorch (pt)
         - NumPy (npz)
         - Comma-separated values (csv)
 
         :param directory: Path to the folder where the memory will be saved.
                           If not provided, the directory defined in the constructor will be used
         :type directory: str
-        :param format: Format of the file where the memory will be saved (default: "pt")
+        :param format: Format of the file where the memory will be saved (default: ``"pt"``)
         :type format: str, optional
 
         :raises ValueError: If the format is not supported
         """
         if not directory:
             directory = self.export_directory
         os.makedirs(os.path.join(directory, "memories"), exist_ok=True)
@@ -416,22 +416,22 @@
         # comma-separated values
         elif format == "csv":
             # open csv writer # TODO: support keeping the dimensions
             with open(memory_path, "a") as file:
                 writer = csv.writer(file)
                 names = self.get_tensor_names()
                 # write headers
-                headers = [["{}.{}".format(name, i) for i in range(self.tensors_view[name].shape[-1])] for name in names]
+                headers = [[f"{name}.{i}" for i in range(self.tensors_view[name].shape[-1])] for name in names]
                 writer.writerow([item for sublist in headers for item in sublist])
                 # write rows
                 for i in range(len(self)):
                     writer.writerow(functools.reduce(operator.iconcat, [self.tensors_view[name][i].tolist() for name in names], []))
         # unsupported format
         else:
-            raise ValueError("Unsupported format: {}. Available formats: pt, csv, npz".format(format))
+            raise ValueError(f"Unsupported format: {format}. Available formats: pt, csv, npz")
 
     def load(self, path: str) -> None:
         """Load the memory from a file
 
         Supported formats:
         - PyTorch (pt)
         - NumPy (npz)
@@ -442,23 +442,23 @@
 
         :raises ValueError: If the format is not supported
         """
         # torch
         if path.endswith(".pt"):
             data = torch.load(path)
             for name in self.get_tensor_names():
-                setattr(self, "_tensor_{}".format(name), data[name])
+                setattr(self, f"_tensor_{name}", data[name])
 
         # numpy
         elif path.endswith(".npz"):
             data = np.load(path)
             for name in data:
-                setattr(self, "_tensor_{}".format(name), torch.tensor(data[name]))
+                setattr(self, f"_tensor_{name}", torch.tensor(data[name]))
 
         # comma-separated values
         elif path.endswith(".csv"):
             # TODO: load the memory from a csv
             pass
 
         # unsupported format
         else:
-            raise ValueError("Unsupported format: {}".format(path))
+            raise ValueError(f"Unsupported format: {path}")
```

### Comparing `skrl-0.9.1/skrl/memories/torch/random.py` & `skrl-1.0.0rc1/skrl/memories/torch/random.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, Tuple, List
+from typing import List, Optional, Tuple, Union
 
 import torch
 
 from skrl.memories.torch import Memory
 
 
 class RandomMemory(Memory):
@@ -16,29 +16,29 @@
                  replacement=True) -> None:
         """Random sampling memory
 
         Sample a batch from memory randomly
 
         :param memory_size: Maximum number of elements in the first dimension of each internal storage
         :type memory_size: int
-        :param num_envs: Number of parallel environments (default: 1)
+        :param num_envs: Number of parallel environments (default: ``1``)
         :type num_envs: int, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
-        :param export: Export the memory to a file (default: False).
+        :param export: Export the memory to a file (default: ``False``).
                        If True, the memory will be exported when the memory is filled
         :type export: bool, optional
-        :param export_format: Export format (default: "pt").
+        :param export_format: Export format (default: ``"pt"``).
                               Supported formats: torch (pt), numpy (np), comma separated values (csv)
         :type export_format: str, optional
-        :param export_directory: Directory where the memory will be exported (default: "").
+        :param export_directory: Directory where the memory will be exported (default: ``""``).
                                  If empty, the agent's experiment directory will be used
         :type export_directory: str, optional
-        :param replacement: Flag to indicate whether the sample is with or without replacement (default: True).
+        :param replacement: Flag to indicate whether the sample is with or without replacement (default: ``True``).
                             Replacement implies that a value can be selected multiple times (the batch size is always guaranteed).
                             Sampling without replacement will return a batch of maximum memory size if the memory size is less than the requested batch size
         :type replacement: bool, optional
 
         :raises ValueError: The export format is not supported
         """
         super().__init__(memory_size, num_envs, device, export, export_format, export_directory)
@@ -52,17 +52,17 @@
                sequence_length: int = 1) -> List[List[torch.Tensor]]:
         """Sample a batch from memory randomly
 
         :param names: Tensors names from which to obtain the samples
         :type names: tuple or list of strings
         :param batch_size: Number of element to sample
         :type batch_size: int
-        :param mini_batches: Number of mini-batches to sample (default: 1)
+        :param mini_batches: Number of mini-batches to sample (default: ``1``)
         :type mini_batches: int, optional
-        :param sequence_length: Length of each sequence (default: 1)
+        :param sequence_length: Length of each sequence (default: ``1``)
         :type sequence_length: int, optional
 
         :return: Sampled data from tensors sorted according to their position in the list of names.
                  The sampled tensors will have the following shape: (batch size, data size)
         :rtype: list of torch.Tensor list
         """
         # compute valid memory sizes
```

### Comparing `skrl-0.9.1/skrl/models/torch/base.py` & `skrl-1.0.0rc1/skrl/models/torch/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Optional, Union, Mapping, Sequence, Tuple, Any
+from typing import Any, Mapping, Optional, Sequence, Tuple, Union
 
+import collections
 import gym
 import gymnasium
-import collections
-import numpy as np
 
+import numpy as np
 import torch
 
 from skrl import logger
 
 
 class Model(torch.nn.Module):
     def __init__(self,
@@ -27,16 +27,16 @@
 
         :param observation_space: Observation/state space or shape.
                                   The ``num_observations`` property will contain the size of that space
         :type observation_space: int, sequence of int, gym.Space, gymnasium.Space
         :param action_space: Action space or shape.
                              The ``num_actions`` property will contain the size of that space
         :type action_space: int, sequence of int, gym.Space, gymnasium.Space
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
 
         Custom models should override the ``act`` method::
 
             import torch
             from skrl.models.torch import Model
 
@@ -131,15 +131,15 @@
                 else:
                     size = 1
             elif issubclass(type(space), gymnasium.spaces.Box):
                 size = np.prod(space.shape)
             elif issubclass(type(space), gymnasium.spaces.Dict):
                 size = sum([self._get_space_size(space.spaces[key], number_of_elements) for key in space.spaces])
         if size is None:
-            raise ValueError("Space type {} not supported".format(type(space)))
+            raise ValueError(f"Space type {type(space)} not supported")
         return int(size)
 
     def tensor_to_space(self,
                         tensor: torch.Tensor,
                         space: Union[gym.Space, gymnasium.Space],
                         start: int = 0) -> Union[torch.Tensor, dict]:
         """Map a flat tensor to a Gym/Gymnasium space
@@ -194,15 +194,15 @@
             elif issubclass(type(space), gymnasium.spaces.Dict):
                 output = {}
                 for k in sorted(space.keys()):
                     end = start + self._get_space_size(space[k], number_of_elements=False)
                     output[k] = self.tensor_to_space(tensor[:, start:end], space[k], end)
                     start = end
                 return output
-        raise ValueError("Space type {} not supported".format(type(space)))
+        raise ValueError(f"Space type {type(space)} not supported")
 
     def random_act(self,
                    inputs: Mapping[str, Union[torch.Tensor, Any]],
                    role: str = "") -> Tuple[torch.Tensor, None, Mapping[str, Union[torch.Tensor, Any]]]:
         """Act randomly according to the action space
 
         :param inputs: Model inputs. The most common keys are:
@@ -212,29 +212,29 @@
         :type inputs: dict where the values are typically torch.Tensor
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
 
         :raises NotImplementedError: Unsupported action space
 
         :return: Model output. The first component is the action to be taken by the agent
-        :rtype: tuple of torch.Tensor, None, and dictionary
+        :rtype: tuple of torch.Tensor, None, and dict
         """
         # discrete action space (Discrete)
         if issubclass(type(self.action_space), gym.spaces.Discrete) or issubclass(type(self.action_space), gymnasium.spaces.Discrete):
-             return torch.randint(self.action_space.n, (inputs["states"].shape[0], 1), device=self.device), None, {}
+            return torch.randint(self.action_space.n, (inputs["states"].shape[0], 1), device=self.device), None, {}
         # continuous action space (Box)
         elif issubclass(type(self.action_space), gym.spaces.Box) or issubclass(type(self.action_space), gymnasium.spaces.Box):
             if self._random_distribution is None:
                 self._random_distribution = torch.distributions.uniform.Uniform(
                     low=torch.tensor(self.action_space.low[0], device=self.device, dtype=torch.float32),
                     high=torch.tensor(self.action_space.high[0], device=self.device, dtype=torch.float32))
 
             return self._random_distribution.sample(sample_shape=(inputs["states"].shape[0], self.num_actions)), None, {}
         else:
-            raise NotImplementedError("Action space type ({}) not supported".format(type(self.action_space)))
+            raise NotImplementedError(f"Action space type ({type(self.action_space)}) not supported")
 
     def init_parameters(self, method_name: str = "normal_", *args, **kwargs) -> None:
         """Initialize the model parameters according to the specified method name
 
         Method names are from the `torch.nn.init <https://pytorch.org/docs/stable/nn.init.html>`_ module.
         Allowed method names are *uniform_*, *normal_*, *constant_*, etc.
 
@@ -250,15 +250,15 @@
             # initialize all parameters with an orthogonal distribution with a gain of 0.5
             >>> model.init_parameters("orthogonal_", gain=0.5)
 
             # initialize all parameters as a sparse matrix with a sparsity of 0.1
             >>> model.init_parameters("sparse_", sparsity=0.1)
         """
         for parameters in self.parameters():
-            exec("torch.nn.init.{}(parameters, *args, **kwargs)".format(method_name))
+            exec(f"torch.nn.init.{method_name}(parameters, *args, **kwargs)")
 
     def init_weights(self, method_name: str = "orthogonal_", *args, **kwargs) -> None:
         """Initialize the model weights according to the specified method name
 
         Method names are from the `torch.nn.init <https://pytorch.org/docs/stable/nn.init.html>`_ module.
         Allowed method names are *uniform_*, *normal_*, *constant_*, etc.
 
@@ -281,15 +281,15 @@
             >>> model.init_weights(method_name="normal_", mean=0.0, std=0.25)
         """
         def _update_weights(module, method_name, args, kwargs):
             for layer in module:
                 if isinstance(layer, torch.nn.Sequential):
                     _update_weights(layer, method_name, args, kwargs)
                 elif isinstance(layer, torch.nn.Linear):
-                    exec("torch.nn.init.{}(layer.weight, *args, **kwargs)".format(method_name))
+                    exec(f"torch.nn.init.{method_name}(layer.weight, *args, **kwargs)")
 
         _update_weights(self.children(), method_name, args, kwargs)
 
     def init_biases(self, method_name: str = "constant_", *args, **kwargs) -> None:
         """Initialize the model biases according to the specified method name
 
         Method names are from the `torch.nn.init <https://pytorch.org/docs/stable/nn.init.html>`_ module.
@@ -314,15 +314,15 @@
             >>> model.init_biases(method_name="normal_", mean=0.0, std=0.25)
         """
         def _update_biases(module, method_name, args, kwargs):
             for layer in module:
                 if isinstance(layer, torch.nn.Sequential):
                     _update_biases(layer, method_name, args, kwargs)
                 elif isinstance(layer, torch.nn.Linear):
-                    exec("torch.nn.init.{}(layer.bias, *args, **kwargs)".format(method_name))
+                    exec(f"torch.nn.init.{method_name}(layer.bias, *args, **kwargs)")
 
         _update_biases(self.children(), method_name, args, kwargs)
 
     def get_specification(self) -> Mapping[str, Any]:
         """Returns the specification of the model
 
         The following keys are used by the agents for initialization:
@@ -360,15 +360,15 @@
         :type inputs: dict where the values are typically torch.Tensor
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
 
         :return: Model output. The first component is the action to be taken by the agent.
                  The second component is the log of the probability density function for stochastic models
                  or None for deterministic models. The third component is a dictionary containing extra output values
-        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dictionary
+        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dict
         """
         return self.act(inputs, role)
 
     def compute(self,
                 inputs: Mapping[str, Union[torch.Tensor, Any]],
                 role: str = "") -> Tuple[Union[torch.Tensor, Mapping[str, Union[torch.Tensor, Any]]]]:
         """Define the computation performed (to be implemented by the inheriting classes) by the models
@@ -380,15 +380,15 @@
         :type inputs: dict where the values are typically torch.Tensor
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
 
         :raises NotImplementedError: Child class must implement this method
 
         :return: Computation performed by the models
-        :rtype: tuple of torch.Tensor and dictionary
+        :rtype: tuple of torch.Tensor and dict
         """
         raise NotImplementedError("The computation performed by the models (.compute()) is not implemented")
 
     def act(self,
             inputs: Mapping[str, Union[torch.Tensor, Any]],
             role: str = "") -> Tuple[torch.Tensor, Union[torch.Tensor, None], Mapping[str, Union[torch.Tensor, Any]]]:
         """Act according to the specified behavior (to be implemented by the inheriting classes)
@@ -406,15 +406,15 @@
         :type role: str, optional
 
         :raises NotImplementedError: Child class must implement this method
 
         :return: Model output. The first component is the action to be taken by the agent.
                  The second component is the log of the probability density function for stochastic models
                  or None for deterministic models. The third component is a dictionary containing extra output values
-        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dictionary
+        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dict
         """
         logger.warning("Make sure to place Mixins before Model during model definition")
         raise NotImplementedError("The action to be taken by the agent (.act()) is not implemented")
 
     def set_mode(self, mode: str) -> None:
         """Set the model mode (training or evaluation)
 
@@ -598,20 +598,20 @@
                     state_dict = {}
             else:
                 raise ValueError("Cannot identify file type")
 
         # show state_dict
         if verbose:
             logger.info("Models")
-            logger.info("  |-- current: {} items".format(len(self.state_dict().keys())))
+            logger.info(f"  |-- current: {len(self.state_dict().keys())} items")
             for name, tensor in self.state_dict().items():
-                logger.info("  |    |-- {} : {}".format(name, list(tensor.shape)))
-            logger.info("  |-- source: {} items".format(len(state_dict.keys())))
+                logger.info(f"  |    |-- {name} : {list(tensor.shape)}")
+            logger.info(f"  |-- source: {len(state_dict.keys())} items")
             for name, tensor in state_dict.items():
-                logger.info("  |    |-- {} : {}".format(name, list(tensor.shape)))
+                logger.info(f"  |    |-- {name} : {list(tensor.shape)}")
             logger.info("Migration")
 
         # migrate the state_dict to current model
         new_state_dict = collections.OrderedDict()
         match_counter = collections.defaultdict(list)
         used_counter = collections.defaultdict(list)
         for name, tensor in self.state_dict().items():
@@ -619,53 +619,53 @@
                 # mapped names
                 if name_map.get(name, "") == external_name:
                     if tensor.shape == external_tensor.shape:
                         new_state_dict[name] = external_tensor
                         match_counter[name].append(external_name)
                         used_counter[external_name].append(name)
                         if verbose:
-                            logger.info("  |-- map:  {} <- {}".format(name, external_name))
+                            logger.info(f"  |-- map:  {name} <- {external_name}")
                         break
                     else:
-                        logger.warning("Shape mismatch for {} <- {} : {} != {}".format(name, external_name, tensor.shape, external_tensor.shape))
+                        logger.warning(f"Shape mismatch for {name} <- {external_name} : {tensor.shape} != {external_tensor.shape}")
                 # auto-mapped names
                 if auto_mapping and name not in name_map:
                     if tensor.shape == external_tensor.shape:
                         if name.endswith(".weight"):
                             if external_name.endswith(".weight"):
                                 new_state_dict[name] = external_tensor
                                 match_counter[name].append(external_name)
                                 used_counter[external_name].append(name)
                                 if verbose:
-                                    logger.info("  |-- auto: {} <- {}".format(name, external_name))
+                                    logger.info(f"  |-- auto: {name} <- {external_name}")
                         elif name.endswith(".bias"):
                             if external_name.endswith(".bias"):
                                 new_state_dict[name] = external_tensor
                                 match_counter[name].append(external_name)
                                 used_counter[external_name].append(name)
                                 if verbose:
-                                    logger.info("  |-- auto: {} <- {}".format(name, external_name))
+                                    logger.info(f"  |-- auto: {name} <- {external_name}")
                         else:
                             if not external_name.endswith(".weight") and not external_name.endswith(".bias"):
                                 new_state_dict[name] = external_tensor
                                 match_counter[name].append(external_name)
                                 used_counter[external_name].append(name)
                                 if verbose:
-                                    logger.info("  |-- auto: {} <- {}".format(name, external_name))
+                                    logger.info(f"  |-- auto: {name} <- {external_name}")
 
         # show ambiguous matches
         status = True
         for name, tensor in self.state_dict().items():
             if len(match_counter.get(name, [])) > 1:
                 logger.warning("Ambiguous match for {} <- [{}]".format(name, ", ".join(match_counter.get(name, []))))
                 status = False
         # show missing matches
         for name, tensor in self.state_dict().items():
             if not match_counter.get(name, []):
-                logger.warning("Missing match for {}".format(name))
+                logger.warning(f"Missing match for {name}")
                 status = False
         # show multiple uses
         for name, tensor in state_dict.items():
             if len(used_counter.get(name, [])) > 1:
                 logger.warning("Multiple use of {} -> [{}]".format(name, ", ".join(used_counter.get(name, []))))
                 status = False
```

### Comparing `skrl-0.9.1/skrl/models/torch/categorical.py` & `skrl-1.0.0rc1/skrl/models/torch/categorical.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Mapping, Tuple, Any
+from typing import Any, Mapping, Tuple, Union
 
 import torch
 from torch.distributions import Categorical
 
 
 class CategoricalMixin:
     def __init__(self, unnormalized_log_prob: bool = True, role: str = "") -> None:
@@ -73,15 +73,15 @@
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
 
         :return: Model output. The first component is the action to be taken by the agent.
                  The second component is the log of the probability density function.
                  The third component is a dictionary containing the network output ``"net_output"``
                  and extra output values
-        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dictionary
+        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dict
 
         Example::
 
             >>> # given a batch of sample states with shape (4096, 4)
             >>> actions, log_prob, outputs = model.act({"states": states})
             >>> print(actions.shape, log_prob.shape, outputs["net_output"].shape)
             torch.Size([4096, 1]) torch.Size([4096, 1]) torch.Size([4096, 2])
@@ -99,14 +99,33 @@
         # actions and log of the probability density function
         actions = self._c_distribution[role].sample()
         log_prob = self._c_distribution[role].log_prob(inputs.get("taken_actions", actions).view(-1))
 
         outputs["net_output"] = net_output
         return actions.unsqueeze(-1), log_prob.unsqueeze(-1), outputs
 
+    def get_entropy(self, role: str = "") -> torch.Tensor:
+        """Compute and return the entropy of the model
+
+        :return: Entropy of the model
+        :rtype: torch.Tensor
+        :param role: Role play by the model (default: ``""``)
+        :type role: str, optional
+
+        Example::
+
+            >>> entropy = model.get_entropy()
+            >>> print(entropy.shape)
+            torch.Size([4096, 1])
+        """
+        distribution = self._c_distribution[role] if role in self._c_distribution else self._c_distribution[""]
+        if distribution is None:
+            return torch.tensor(0.0, device=self.device)
+        return distribution.entropy().to(self.device)
+
     def distribution(self, role: str = "") -> torch.distributions.Categorical:
         """Get the current distribution of the model
 
         :return: Distribution of the model
         :rtype: torch.distributions.Categorical
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
```

### Comparing `skrl-0.9.1/skrl/models/torch/deterministic.py` & `skrl-1.0.0rc1/skrl/models/torch/deterministic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Mapping, Tuple, Any
+from typing import Any, Mapping, Tuple, Union
 
 import gym
 import gymnasium
 
 import torch
 
 
@@ -74,15 +74,15 @@
                        - ``"taken_actions"``: actions taken by the policy for the given states
         :type inputs: dict where the values are typically torch.Tensor
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
 
         :return: Model output. The first component is the action to be taken by the agent.
                  The second component is ``None``. The third component is a dictionary containing extra output values
-        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dictionary
+        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dict
 
         Example::
 
             >>> # given a batch of sample states with shape (4096, 60)
             >>> actions, _, outputs = model.act({"states": states})
             >>> print(actions.shape, outputs)
             torch.Size([4096, 1]) {}
```

### Comparing `skrl-0.9.1/skrl/models/torch/gaussian.py` & `skrl-1.0.0rc1/skrl/models/torch/gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Mapping, Tuple, Any
+from typing import Any, Mapping, Tuple, Union
 
 import gym
 import gymnasium
 
 import torch
 from torch.distributions import Normal
 
@@ -124,15 +124,15 @@
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
 
         :return: Model output. The first component is the action to be taken by the agent.
                  The second component is the log of the probability density function.
                  The third component is a dictionary containing the mean actions ``"mean_actions"``
                  and extra output values
-        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dictionary
+        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dict
 
         Example::
 
             >>> # given a batch of sample states with shape (4096, 60)
             >>> actions, log_prob, outputs = model.act({"states": states})
             >>> print(actions.shape, log_prob.shape, outputs["mean_actions"].shape)
             torch.Size([4096, 8]) torch.Size([4096, 1]) torch.Size([4096, 8])
```

### Comparing `skrl-0.9.1/skrl/models/torch/multivariate_gaussian.py` & `skrl-1.0.0rc1/skrl/models/torch/multivariate_gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Mapping, Tuple, Any
+from typing import Any, Mapping, Tuple, Union
 
 import gym
 import gymnasium
 
 import torch
 from torch.distributions import MultivariateNormal
 
@@ -110,15 +110,15 @@
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
 
         :return: Model output. The first component is the action to be taken by the agent.
                  The second component is the log of the probability density function.
                  The third component is a dictionary containing the mean actions ``"mean_actions"``
                  and extra output values
-        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dictionary
+        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dict
 
         Example::
 
             >>> # given a batch of sample states with shape (4096, 60)
             >>> actions, log_prob, outputs = model.act({"states": states})
             >>> print(actions.shape, log_prob.shape, outputs["mean_actions"].shape)
             torch.Size([4096, 8]) torch.Size([4096, 1]) torch.Size([4096, 8])
```

### Comparing `skrl-0.9.1/skrl/models/torch/tabular.py` & `skrl-1.0.0rc1/skrl/models/torch/tabular.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, Mapping, Sequence, Tuple, Any
+from typing import Any, Mapping, Optional, Sequence, Tuple, Union
 
 import torch
 
 from skrl.models.torch import Model
 
 
 class TabularMixin:
@@ -46,15 +46,15 @@
 
     def __repr__(self) -> str:
         """String representation of an object as torch.nn.Module
         """
         lines = []
         for name in self._get_tensor_names():
             tensor = getattr(self, name)
-            lines.append("({}): {}(shape={})".format(name, tensor.__class__.__name__, list(tensor.shape)))
+            lines.append(f"({name}): {tensor.__class__.__name__}(shape={list(tensor.shape)})")
 
         main_str = self.__class__.__name__ + '('
         if lines:
             main_str += "\n  {}\n".format("\n  ".join(lines))
         main_str += ')'
         return main_str
 
@@ -81,15 +81,15 @@
                        - ``"taken_actions"``: actions taken by the policy for the given states
         :type inputs: dict where the values are typically torch.Tensor
         :param role: Role play by the model (default: ``""``)
         :type role: str, optional
 
         :return: Model output. The first component is the action to be taken by the agent.
                  The second component is ``None``. The third component is a dictionary containing extra output values
-        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dictionary
+        :rtype: tuple of torch.Tensor, torch.Tensor or None, and dict
 
         Example::
 
             >>> # given a batch of sample states with shape (1, 100)
             >>> actions, _, outputs = model.act({"states": states})
             >>> print(actions[0], outputs)
             tensor([[3]], device='cuda:0') {}
@@ -151,18 +151,17 @@
         for name, tensor in state_dict.items():
             if hasattr(self, name) and isinstance(getattr(self, name), torch.Tensor):
                 _tensor = getattr(self, name)
                 if isinstance(_tensor, torch.Tensor):
                     if _tensor.shape == tensor.shape and _tensor.dtype == tensor.dtype:
                         setattr(self, name, tensor)
                     else:
-                        raise ValueError("Tensor shape ({} vs {}) or dtype ({} vs {}) mismatch"\
-                            .format(_tensor.shape, tensor.shape, _tensor.dtype, tensor.dtype))
+                        raise ValueError(f"Tensor shape ({_tensor.shape} vs {tensor.shape}) or dtype ({_tensor.dtype} vs {tensor.dtype}) mismatch")
             else:
-                raise ValueError("{} is not a tensor of {}".format(name, self.__class__.__name__))
+                raise ValueError(f"{name} is not a tensor of {self.__class__.__name__}")
 
     def save(self, path: str, state_dict: Optional[dict] = None) -> None:
         """Save the model to the specified path
 
         :param path: Path to save the model to
         :type path: str
         :param state_dict: State dictionary to save (default: ``None``).
@@ -201,11 +200,10 @@
         for name, tensor in tensors.items():
             if hasattr(self, name) and isinstance(getattr(self, name), torch.Tensor):
                 _tensor = getattr(self, name)
                 if isinstance(_tensor, torch.Tensor):
                     if _tensor.shape == tensor.shape and _tensor.dtype == tensor.dtype:
                         setattr(self, name, tensor)
                     else:
-                        raise ValueError("Tensor shape ({} vs {}) or dtype ({} vs {}) mismatch"\
-                            .format(_tensor.shape, tensor.shape, _tensor.dtype, tensor.dtype))
+                        raise ValueError(f"Tensor shape ({_tensor.shape} vs {tensor.shape}) or dtype ({_tensor.dtype} vs {tensor.dtype}) mismatch")
             else:
-                raise ValueError("{} is not a tensor of {}".format(name, self.__class__.__name__))
+                raise ValueError(f"{name} is not a tensor of {self.__class__.__name__}")
```

### Comparing `skrl-0.9.1/skrl/resources/noises/torch/base.py` & `skrl-1.0.0rc1/skrl/resources/noises/torch/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-from typing import Optional, Union, Tuple
+from typing import Optional, Tuple, Union
 
 import torch
 
 
 class Noise():
     def __init__(self, device: Optional[Union[str, torch.device]] = None) -> None:
         """Base class representing a noise
 
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
 
         Custom noises should override the ``sample`` method::
 
             import torch
             from skrl.resources.noises.torch import Noise
 
             class CustomNoise(Noise):
                 def __init__(self, device=None):
                     super().__init__(device)
 
                 def sample(self, size):
                     return torch.rand(size, device=self.device)
         """
-        self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu") if device is None else torch.device(device)
+        if device is None:
+            self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        else:
+            self.device = torch.device(device)
 
     def sample_like(self, tensor: torch.Tensor) -> torch.Tensor:
         """Sample a noise with the same size (shape) as the input tensor
 
-        This method will call the sampling method as follows ``.sample(tensor.size())``
+        This method will call the sampling method as follows ``.sample(tensor.shape)``
 
         :param tensor: Input tensor used to determine output tensor size (shape)
         :type tensor: torch.Tensor
 
         :return: Sampled noise
         :rtype: torch.Tensor
 
@@ -40,21 +43,21 @@
 
             >>> x = torch.rand(3, 2, device="cuda:0")
             >>> noise.sample_like(x)
             tensor([[-0.0423, -0.1325],
                     [-0.0639, -0.0957],
                     [-0.1367,  0.1031]], device='cuda:0')
         """
-        return self.sample(tensor.size())
+        return self.sample(tensor.shape)
 
     def sample(self, size: Union[Tuple[int], torch.Size]) -> torch.Tensor:
         """Noise sampling method to be implemented by the inheriting classes
 
         :param size: Shape of the sampled tensor
-        :type size: tuple or list of integers, or torch.Size
+        :type size: tuple or list of int, or torch.Size
 
         :raises NotImplementedError: The method is not implemented by the inheriting classes
 
         :return: Sampled noise
         :rtype: torch.Tensor
         """
         raise NotImplementedError("The sampling method (.sample()) is not implemented")
```

### Comparing `skrl-0.9.1/skrl/resources/noises/torch/gaussian.py` & `skrl-1.0.0rc1/skrl/resources/noises/torch/gaussian.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, Tuple
+from typing import Optional, Tuple, Union
 
 import torch
 from torch.distributions import Normal
 
 from skrl.resources.noises.torch import Noise
 
 
@@ -10,16 +10,16 @@
     def __init__(self, mean: float, std: float, device: Optional[Union[str, torch.device]] = None) -> None:
         """Class representing a Gaussian noise
 
         :param mean: Mean of the normal distribution
         :type mean: float
         :param std: Standard deviation of the normal distribution
         :type std: float
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
 
         Example::
 
             >>> noise = GaussianNoise(mean=0, std=1)
         """
         super().__init__(device)
@@ -27,15 +27,15 @@
         self.distribution = Normal(loc=torch.tensor(mean, device=self.device, dtype=torch.float32),
                                    scale=torch.tensor(std, device=self.device, dtype=torch.float32))
 
     def sample(self, size: Union[Tuple[int], torch.Size]) -> torch.Tensor:
         """Sample a Gaussian noise
 
         :param size: Shape of the sampled tensor
-        :type size: tuple or list of integers, or torch.Size
+        :type size: tuple or list of int, or torch.Size
 
         :return: Sampled noise
         :rtype: torch.Tensor
 
         Example::
 
             >>> noise.sample((3, 2))
```

### Comparing `skrl-0.9.1/skrl/resources/noises/torch/ornstein_uhlenbeck.py` & `skrl-1.0.0rc1/skrl/resources/noises/torch/ornstein_uhlenbeck.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, Tuple
+from typing import Optional, Tuple, Union
 
 import torch
 from torch.distributions import Normal
 
 from skrl.resources.noises.torch import Noise
 
 
@@ -22,17 +22,17 @@
         :type sigma: float
         :param base_scale: Factor to apply to returned noise
         :type base_scale: float
         :param mean: Mean of the normal distribution (default: ``0.0``)
         :type mean: float, optional
         :param std: Standard deviation of the normal distribution (default: ``1.0``)
         :type std: float, optional
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
-        :type device: str or torch.device, optional
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
+        :type device: str or jax.Device, optional
 
         Example::
 
             >>> noise = OrnsteinUhlenbeckNoise(theta=0.1, sigma=0.2, base_scale=0.5)
         """
         super().__init__(device)
 
@@ -44,15 +44,15 @@
         self.distribution = Normal(loc=torch.tensor(mean, device=self.device, dtype=torch.float32),
                                    scale=torch.tensor(std, device=self.device, dtype=torch.float32))
 
     def sample(self, size: Union[Tuple[int], torch.Size]) -> torch.Tensor:
         """Sample an Ornstein-Uhlenbeck noise
 
         :param size: Shape of the sampled tensor
-        :type size: tuple or list of integers, or torch.Size
+        :type size: tuple or list of int, or torch.Size
 
         :return: Sampled noise
         :rtype: torch.Tensor
 
         Example::
 
             >>> noise.sample((3, 2))
@@ -62,12 +62,12 @@
 
             >>> x = torch.rand(3, 2, device="cuda:0")
             >>> noise.sample(x.shape)
             tensor([[-0.0540,  0.0461],
                     [ 0.1117, -0.1157],
                     [-0.0074,  0.0420]], device='cuda:0')
         """
-        if isinstance(self.state, torch.Tensor) and self.state.size() != torch.Size(size):
+        if hasattr(self.state, "shape") and self.state.shape != torch.Size(size):
             self.state = 0
         self.state += -self.state * self.theta + self.sigma * self.distribution.sample(size)
 
         return self.base_scale * self.state
```

### Comparing `skrl-0.9.1/skrl/resources/preprocessors/torch/running_standard_scaler.py` & `skrl-1.0.0rc1/skrl/resources/preprocessors/torch/running_standard_scaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Optional, Union, Tuple
+from typing import Optional, Tuple, Union
 
 import gym
 import gymnasium
-import numpy as np
 
+import numpy as np
 import torch
 import torch.nn as nn
 
 
 class RunningStandardScaler(nn.Module):
     def __init__(self,
                  size: Union[int, Tuple[int], gym.Space, gymnasium.Space],
@@ -30,29 +30,32 @@
 
         :param size: Size of the input space
         :type size: int, tuple or list of integers, gym.Space, or gymnasium.Space
         :param epsilon: Small number to avoid division by zero (default: ``1e-8``)
         :type epsilon: float
         :param clip_threshold: Threshold to clip the data (default: ``5.0``)
         :type clip_threshold: float
-        :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                       If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+        :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                       If None, the device will be either ``"cuda"`` if available or ``"cpu"``
         :type device: str or torch.device, optional
         """
         super().__init__()
 
         self.epsilon = epsilon
         self.clip_threshold = clip_threshold
-        self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu") if device is None else torch.device(device)
+        if device is None:
+            self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        else:
+            self.device = torch.device(device)
 
         size = self._get_space_size(size)
 
-        self.register_buffer("running_mean", torch.zeros(size, dtype = torch.float64, device=self.device))
-        self.register_buffer("running_variance", torch.ones(size, dtype = torch.float64, device=self.device))
-        self.register_buffer("current_count", torch.ones((), dtype = torch.float64, device=self.device))
+        self.register_buffer("running_mean", torch.zeros(size, dtype=torch.float64, device=self.device))
+        self.register_buffer("running_variance", torch.ones(size, dtype=torch.float64, device=self.device))
+        self.register_buffer("current_count", torch.ones((), dtype=torch.float64, device=self.device))
 
     def _get_space_size(self, space: Union[int, Tuple[int], gym.Space, gymnasium.Space]) -> int:
         """Get the size (number of elements) of a space
 
         :param space: Space or shape from which to obtain the number of elements
         :type space: int, tuple or list of integers, gym.Space, or gymnasium.Space
 
@@ -75,15 +78,15 @@
         elif issubclass(type(space), gymnasium.Space):
             if issubclass(type(space), gymnasium.spaces.Discrete):
                 return 1
             elif issubclass(type(space), gymnasium.spaces.Box):
                 return np.prod(space.shape)
             elif issubclass(type(space), gymnasium.spaces.Dict):
                 return sum([self._get_space_size(space.spaces[key]) for key in space.spaces])
-        raise ValueError("Space type {} not supported".format(type(space)))
+        raise ValueError(f"Space type {type(space)} not supported")
 
     def _parallel_variance(self, input_mean: torch.Tensor, input_var: torch.Tensor, input_count: int) -> None:
         """Update internal variables using the parallel algorithm for computing variance
 
         https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Parallel_algorithm
 
         :param input_mean: Mean of the input data
@@ -108,31 +111,38 @@
 
         :param x: Input tensor
         :type x: torch.Tensor
         :param train: Whether to train the standardizer (default: ``False``)
         :type train: bool, optional
         :param inverse: Whether to inverse the standardizer to scale back the data (default: ``False``)
         :type inverse: bool, optional
+
+        :return: Standardized tensor
+        :rtype: torch.Tensor
         """
         if train:
             if x.dim() == 3:
-                self._parallel_variance(torch.mean(x, dim=(0,1)), torch.var(x, dim=(0,1)), x.shape[0] * x.shape[1])
+                self._parallel_variance(torch.mean(x, dim=(0, 1)), torch.var(x, dim=(0, 1)), x.shape[0] * x.shape[1])
             else:
                 self._parallel_variance(torch.mean(x, dim=0), torch.var(x, dim=0), x.shape[0])
 
         # scale back the data to the original representation
         if inverse:
             return torch.sqrt(self.running_variance.float()) \
                 * torch.clamp(x, min=-self.clip_threshold, max=self.clip_threshold) + self.running_mean.float()
         # standardization by centering and scaling
-        else:
-            return torch.clamp((x - self.running_mean.float()) / (torch.sqrt(self.running_variance.float()) + self.epsilon),
-                                min=-self.clip_threshold, max=self.clip_threshold)
-
-    def forward(self, x: torch.Tensor, train: bool = False, inverse: bool = False, no_grad: bool = True) -> torch.Tensor:
+        return torch.clamp((x - self.running_mean.float()) / (torch.sqrt(self.running_variance.float()) + self.epsilon),
+                           min=-self.clip_threshold,
+                           max=self.clip_threshold)
+
+    def forward(self,
+                x: torch.Tensor,
+                train: bool = False,
+                inverse: bool = False,
+                no_grad: bool = True) -> torch.Tensor:
         """Forward pass of the standardizer
 
         Example::
 
             >>> x = torch.rand(3, 2, device="cuda:0")
             >>> running_standard_scaler(x)
             tensor([[0.6933, 0.1905],
@@ -153,13 +163,15 @@
         :type x: torch.Tensor
         :param train: Whether to train the standardizer (default: ``False``)
         :type train: bool, optional
         :param inverse: Whether to inverse the standardizer to scale back the data (default: ``False``)
         :type inverse: bool, optional
         :param no_grad: Whether to disable the gradient computation (default: ``True``)
         :type no_grad: bool, optional
+
+        :return: Standardized tensor
+        :rtype: torch.Tensor
         """
         if no_grad:
             with torch.no_grad():
                 return self._compute(x, train, inverse)
-        else:
-            return self._compute(x, train, inverse)
+        return self._compute(x, train, inverse)
```

### Comparing `skrl-0.9.1/skrl/resources/schedulers/torch/kl_adaptive.py` & `skrl-1.0.0rc1/skrl/resources/schedulers/torch/kl_adaptive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Union, Optional
+from typing import Optional, Union
 
 import torch
 from torch.optim.lr_scheduler import _LRScheduler
 
 
-class KLAdaptiveRL(_LRScheduler):
+class KLAdaptiveLR(_LRScheduler):
     def __init__(self,
                  optimizer: torch.optim.Optimizer,
                  kl_threshold: float = 0.008,
                  min_lr: float = 1e-6,
                  max_lr: float = 1e-2,
                  kl_factor: float = 2,
                  lr_factor: float = 1.5,
@@ -23,18 +23,17 @@
         .. note::
 
             This scheduler is only available for PPO at the moment.
             Applying it to other agents will not change the learning rate
 
         Example::
 
-            >>> scheduler = KLAdaptiveRL(optimizer, kl_threshold=0.01)
+            >>> scheduler = KLAdaptiveLR(optimizer, kl_threshold=0.01)
             >>> for epoch in range(100):
-            >>>     train(...)
-            >>>     validate(...)
+            >>>     # ...
             >>>     kl_divergence = ...
             >>>     scheduler.step(kl_divergence)
 
         :param optimizer: Wrapped optimizer
         :type optimizer: torch.optim.Optimizer
         :param kl_threshold: Threshold for KL divergence (default: ``0.008``)
         :type kl_threshold: float, optional
@@ -71,22 +70,22 @@
             >>> kl
             tensor([0.0332, 0.0500, 0.0383,  ..., 0.0076, 0.0240, 0.0164])
             >>> scheduler.step(kl.mean())
 
             >>> kl = 0.0046
             >>> scheduler.step(kl)
 
-        :param kl: KL divergence (default: None)
+        :param kl: KL divergence (default: ``None``)
                    If None, no adjustment is made.
                    If tensor, the number of elements must be 1
-        :type kl: torch.Tensor, float, None, optional
-        :param epoch: Epoch (default: None)
+        :type kl: torch.Tensor, float or None, optional
+        :param epoch: Epoch (default: ``None``)
         :type epoch: int, optional
         """
         if kl is not None:
             for group in self.optimizer.param_groups:
-                if kl >  self.kl_threshold * self._kl_factor:
+                if kl > self.kl_threshold * self._kl_factor:
                     group['lr'] = max(group['lr'] / self._lr_factor, self.min_lr)
                 elif kl < self.kl_threshold / self._kl_factor:
                     group['lr'] = min(group['lr'] * self._lr_factor, self.max_lr)
 
             self._last_lr = [group['lr'] for group in self.optimizer.param_groups]
```

### Comparing `skrl-0.9.1/skrl/trainers/torch/base.py` & `skrl-1.0.0rc1/skrl/trainers/jax/manual.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,246 +1,251 @@
-from typing import Union, List, Optional
+from typing import List, Optional, Union
 
+import contextlib
+import copy
 import tqdm
 
-import torch
+import jax.numpy as jnp
 
-from skrl.envs.torch import Wrapper
-from skrl.agents.torch import Agent
+from skrl.agents.jax import Agent
+from skrl.envs.jax import Wrapper
+from skrl.trainers.jax import Trainer
 
 
-def generate_equally_spaced_scopes(num_envs: int, num_agents: int) -> List[int]:
-    """Generate a list of equally spaced scopes for the agents
+MANUAL_TRAINER_DEFAULT_CONFIG = {
+    "timesteps": 100000,            # number of timesteps to train for
+    "headless": False,              # whether to use headless mode (no rendering)
+    "disable_progressbar": False,   # whether to disable the progressbar. If None, disable on non-TTY
+    "close_environment_at_exit": True,   # whether to close the environment on normal program termination
+}
 
-    :param num_envs: Number of environments
-    :type num_envs: int
-    :param num_agents: Number of agents
-    :type num_agents: int
 
-    :raises ValueError: If the number of agents is greater than the number of environments
-
-    :return: List of equally spaced scopes
-    :rtype: List[int]
-    """
-    scopes = [int(num_envs / num_agents)] * num_agents
-    if sum(scopes):
-        scopes[-1] += num_envs - sum(scopes)
-    else:
-        raise ValueError("The number of agents ({}) is greater than the number of environments ({})" \
-            .format(num_agents, num_envs))
-    return scopes
-
-
-class Trainer:
+class ManualTrainer(Trainer):
     def __init__(self,
                  env: Wrapper,
                  agents: Union[Agent, List[Agent]],
                  agents_scope: Optional[List[int]] = None,
                  cfg: Optional[dict] = None) -> None:
-        """Base class for trainers
+        """Manual trainer
+
+        Train agents by manually controlling the training/evaluation loop
 
         :param env: Environment to train on
-        :type env: skrl.env.torch.Wrapper
+        :type env: skrl.env.jax.Wrapper
         :param agents: Agents to train
         :type agents: Union[Agent, List[Agent]]
-        :param agents_scope: Number of environments for each agent to train on (default: [])
-        :type agents_scope: tuple or list of integers
-        :param cfg: Configuration dictionary (default: {})
+        :param agents_scope: Number of environments for each agent to train on (default: ``None``)
+        :type agents_scope: tuple or list of int, optional
+        :param cfg: Configuration dictionary (default: ``None``).
+                    See MANUAL_TRAINER_DEFAULT_CONFIG for default values
         :type cfg: dict, optional
         """
-        self.cfg = cfg if cfg is not None else {}
-        self.env = env
-        self.agents = agents
-        self.agents_scope = agents_scope if agents_scope is not None else []
-
-        # get configuration
-        self.timesteps = self.cfg.get("timesteps", 0)
-        self.headless = self.cfg.get("headless", False)
-        self.disable_progressbar = self.cfg.get("disable_progressbar", False)
-
-        self.initial_timestep = 0
-
-        # setup agents
-        self.num_agents = 0
-        self._setup_agents()
-
-    def __str__(self) -> str:
-        """Generate a string representation of the trainer
-
-        :return: Representation of the trainer as string
-        :rtype: str
-        """
-        string = "Trainer: {}".format(repr(self))
-        string += "\n  |-- Number of parallelizable environments: {}".format(self.env.num_envs)
-        string += "\n  |-- Number of agents: {}".format(self.num_agents)
-        string += "\n  |-- Agents and scopes:"
-        if self.num_agents > 1:
-            for agent, scope in zip(self.agents, self.agents_scope):
-                string += "\n  |     |-- agent: {}".format(type(agent))
-                string += "\n  |     |     |-- scope: {} environments ({}:{})".format(scope[1] - scope[0], scope[0], scope[1])
+        _cfg = copy.deepcopy(MANUAL_TRAINER_DEFAULT_CONFIG)
+        _cfg.update(cfg if cfg is not None else {})
+        agents_scope = agents_scope if agents_scope is not None else []
+        super().__init__(env=env, agents=agents, agents_scope=agents_scope, cfg=_cfg)
+
+        # init agents
+        if self.num_simultaneous_agents > 1:
+            for agent in self.agents:
+                agent.init(trainer_cfg=self.cfg)
         else:
-            string += "\n  |     |-- agent: {}".format(type(self.agents))
-            string += "\n  |     |     |-- scope: {} environment(s)".format(self.env.num_envs)
-        return string
+            self.agents.init(trainer_cfg=self.cfg)
 
-    def _setup_agents(self) -> None:
-        """Setup agents for training
+        self._timestep = 0
+        self._progress = None
 
-        :raises ValueError: Invalid setup
-        """
-        # validate agents and their scopes
-        if type(self.agents) in [tuple, list]:
-            # single agent
-            if len(self.agents) == 1:
-                self.num_agents = 1
-                self.agents = self.agents[0]
-                self.agents_scope = [1]
-            # parallel agents
-            elif len(self.agents) > 1:
-                self.num_agents = len(self.agents)
-                # check scopes
-                if not len(self.agents_scope):
-                    print("[WARNING] The agents' scopes are empty, they will be generated as equal as possible")
-                    self.agents_scope = [int(self.env.num_envs / len(self.agents))] * len(self.agents)
-                    if sum(self.agents_scope):
-                        self.agents_scope[-1] += self.env.num_envs - sum(self.agents_scope)
-                    else:
-                        raise ValueError("The number of agents ({}) is greater than the number of parallelizable environments ({})" \
-                            .format(len(self.agents), self.env.num_envs))
-                elif len(self.agents_scope) != len(self.agents):
-                    raise ValueError("The number of agents ({}) doesn't match the number of scopes ({})" \
-                        .format(len(self.agents), len(self.agents_scope)))
-                elif sum(self.agents_scope) != self.env.num_envs:
-                    raise ValueError("The scopes ({}) don't cover the number of parallelizable environments ({})" \
-                        .format(sum(self.agents_scope), self.env.num_envs))
-                # generate agents' scopes
-                index = 0
-                for i in range(len(self.agents_scope)):
-                    index += self.agents_scope[i]
-                    self.agents_scope[i] = (index - self.agents_scope[i], index)
-            else:
-                raise ValueError("A list of agents is expected")
-        else:
-            self.num_agents = 1
+        self.states = None
 
-    def train(self) -> None:
-        """Train the agents
+    def train(self, timestep: Optional[int] = None, timesteps: Optional[int] = None) -> None:
+        """Execute a training iteration
 
-        :raises NotImplementedError: Not implemented
-        """
-        raise NotImplementedError
+        This method executes the following steps once:
 
-    def eval(self) -> None:
-        """Evaluate the agents
-
-        :raises NotImplementedError: Not implemented
-        """
-        raise NotImplementedError
-
-    def single_agent_train(self) -> None:
-        """Train a single agent
-
-        This method executes the following steps in loop:
-
-        - Pre-interaction
-        - Compute actions
+        - Pre-interaction (sequentially if num_simultaneous_agents > 1)
+        - Compute actions (sequentially if num_simultaneous_agents > 1)
         - Interact with the environments
         - Render scene
-        - Record transitions
-        - Post-interaction
+        - Record transitions (sequentially if num_simultaneous_agents > 1)
+        - Post-interaction (sequentially if num_simultaneous_agents > 1)
         - Reset environments
-        """
-        assert self.num_agents == 1, "This method is only valid for a single agent"
 
-        # reset env
-        states, infos = self.env.reset()
+        :param timestep: Current timestep (default: ``None``).
+                         If None, the current timestep will be carried by an internal variable
+        :type timestep: int, optional
+        :param timesteps: Total number of timesteps (default: ``None``).
+                          If None, the total number of timesteps is obtained from the trainer's config
+        :type timesteps: int, optional
+        """
+        if timestep is None:
+            self._timestep += 1
+            timestep = self._timestep
+        timesteps = self.timesteps if timesteps is None else timesteps
+
+        if self._progress is None:
+            self._progress = tqdm.tqdm(total=timesteps, disable=self.disable_progressbar)
+        self._progress.update(n=1)
+
+        # set running mode
+        if self.num_simultaneous_agents > 1:
+            for agent in self.agents:
+                agent.set_running_mode("train")
+        else:
+            self.agents.set_running_mode("train")
 
-        for timestep in tqdm.tqdm(range(self.initial_timestep, self.timesteps), disable=self.disable_progressbar):
+        # reset env
+        if self.states is None:
+            self.states, infos = self.env.reset()
 
+        if self.num_simultaneous_agents == 1:
             # pre-interaction
-            self.agents.pre_interaction(timestep=timestep, timesteps=self.timesteps)
+            self.agents.pre_interaction(timestep=timestep, timesteps=timesteps)
 
             # compute actions
-            with torch.no_grad():
-                actions = self.agents.act(states, timestep=timestep, timesteps=self.timesteps)[0]
+            with contextlib.nullcontext():
+                actions = self.agents.act(self.states, timestep=timestep, timesteps=timesteps)[0]
 
-            # step the environments
-            next_states, rewards, terminated, truncated, infos = self.env.step(actions)
+        else:
+            # pre-interaction
+            for agent in self.agents:
+                agent.pre_interaction(timestep=timestep, timesteps=timesteps)
 
-            # render scene
-            if not self.headless:
-                self.env.render()
+            # compute actions
+            with contextlib.nullcontext():
+                actions = jnp.vstack([agent.act(self.states[scope[0]:scope[1]], timestep=timestep, timesteps=timesteps)[0] \
+                                      for agent, scope in zip(self.agents, self.agents_scope)])
+
+        # step the environments
+        next_states, rewards, terminated, truncated, infos = self.env.step(actions)
+
+        # render scene
+        if not self.headless:
+            self.env.render()
 
+        if self.num_simultaneous_agents == 1:
             # record the environments' transitions
-            with torch.no_grad():
-                self.agents.record_transition(states=states,
+            with contextlib.nullcontext():
+                self.agents.record_transition(states=self.states,
                                               actions=actions,
                                               rewards=rewards,
                                               next_states=next_states,
                                               terminated=terminated,
                                               truncated=truncated,
                                               infos=infos,
                                               timestep=timestep,
-                                              timesteps=self.timesteps)
+                                              timesteps=timesteps)
 
             # post-interaction
-            self.agents.post_interaction(timestep=timestep, timesteps=self.timesteps)
+            self.agents.post_interaction(timestep=timestep, timesteps=timesteps)
 
-            # reset environments
-            with torch.no_grad():
-                if terminated.any() or truncated.any():
-                    states, infos = self.env.reset()
-                else:
-                    states.copy_(next_states)
+        else:
+            # record the environments' transitions
+            with contextlib.nullcontext():
+                for agent, scope in zip(self.agents, self.agents_scope):
+                    agent.record_transition(states=self.states[scope[0]:scope[1]],
+                                            actions=actions[scope[0]:scope[1]],
+                                            rewards=rewards[scope[0]:scope[1]],
+                                            next_states=next_states[scope[0]:scope[1]],
+                                            terminated=terminated[scope[0]:scope[1]],
+                                            truncated=truncated[scope[0]:scope[1]],
+                                            infos=infos,
+                                            timestep=timestep,
+                                            timesteps=timesteps)
 
-        # close the environment
-        self.env.close()
+            # post-interaction
+            for agent in self.agents:
+                agent.post_interaction(timestep=timestep, timesteps=timesteps)
 
-    def single_agent_eval(self) -> None:
+        # reset environments
+        with contextlib.nullcontext():
+            if terminated.any() or truncated.any():
+                self.states, infos = self.env.reset()
+            else:
+                self.states = next_states
+
+    def eval(self, timestep: Optional[int] = None, timesteps: Optional[int] = None) -> None:
         """Evaluate the agents sequentially
 
         This method executes the following steps in loop:
 
-        - Compute actions (sequentially)
+        - Compute actions (sequentially if num_simultaneous_agents > 1)
         - Interact with the environments
         - Render scene
         - Reset environments
-        """
-        assert self.num_agents == 1, "This method is only valid for a single agent"
 
-        # reset env
-        states, infos = self.env.reset()
-
-        for timestep in tqdm.tqdm(range(self.initial_timestep, self.timesteps), disable=self.disable_progressbar):
+        :param timestep: Current timestep (default: ``None``).
+                         If None, the current timestep will be carried by an internal variable
+        :type timestep: int, optional
+        :param timesteps: Total number of timesteps (default: ``None``).
+                          If None, the total number of timesteps is obtained from the trainer's config
+        :type timesteps: int, optional
+        """
+        if timestep is None:
+            self._timestep += 1
+            timestep = self._timestep
+        timesteps = self.timesteps if timesteps is None else timesteps
+
+        if self._progress is None:
+            self._progress = tqdm.tqdm(total=timesteps, disable=self.disable_progressbar)
+        self._progress.update(n=1)
+
+        # set running mode
+        if self.num_simultaneous_agents > 1:
+            for agent in self.agents:
+                agent.set_running_mode("eval")
+        else:
+            self.agents.set_running_mode("eval")
 
-            # compute actions
-            with torch.no_grad():
-                actions = self.agents.act(states, timestep=timestep, timesteps=self.timesteps)[0]
+        # reset env
+        if self.states is None:
+            self.states, infos = self.env.reset()
 
-            # step the environments
-            next_states, rewards, terminated, truncated, infos = self.env.step(actions)
+        with contextlib.nullcontext():
+            if self.num_simultaneous_agents == 1:
+                # compute actions
+                actions = self.agents.act(self.states, timestep=timestep, timesteps=timesteps)[0]
 
-            # render scene
-            if not self.headless:
-                self.env.render()
+            else:
+                # compute actions
+                actions = jnp.vstack([agent.act(self.states[scope[0]:scope[1]], timestep=timestep, timesteps=timesteps)[0] \
+                                      for agent, scope in zip(self.agents, self.agents_scope)])
+
+        # step the environments
+        next_states, rewards, terminated, truncated, infos = self.env.step(actions)
+
+        # render scene
+        if not self.headless:
+            self.env.render()
 
-            with torch.no_grad():
+        with contextlib.nullcontext():
+            if self.num_simultaneous_agents == 1:
                 # write data to TensorBoard
-                self.agents.record_transition(states=states,
+                self.agents.record_transition(states=self.states,
                                               actions=actions,
                                               rewards=rewards,
                                               next_states=next_states,
                                               terminated=terminated,
                                               truncated=truncated,
                                               infos=infos,
                                               timestep=timestep,
-                                              timesteps=self.timesteps)
-                super(type(self.agents), self.agents).post_interaction(timestep=timestep, timesteps=self.timesteps)
+                                              timesteps=timesteps)
+                super(type(self.agents), self.agents).post_interaction(timestep=timestep, timesteps=timesteps)
 
-                # reset environments
-                if terminated.any() or truncated.any():
-                    states, infos = self.env.reset()
-                else:
-                    states.copy_(next_states)
+            else:
+                # write data to TensorBoard
+                for agent, scope in zip(self.agents, self.agents_scope):
+                    agent.record_transition(states=self.states[scope[0]:scope[1]],
+                                            actions=actions[scope[0]:scope[1]],
+                                            rewards=rewards[scope[0]:scope[1]],
+                                            next_states=next_states[scope[0]:scope[1]],
+                                            terminated=terminated[scope[0]:scope[1]],
+                                            truncated=truncated[scope[0]:scope[1]],
+                                            infos=infos,
+                                            timestep=timestep,
+                                            timesteps=timesteps)
+                    super(type(agent), agent).post_interaction(timestep=timestep, timesteps=timesteps)
 
-        # close the environment
-        self.env.close()
+            # reset environments
+            if terminated.any() or truncated.any():
+                self.states, infos = self.env.reset()
+            else:
+                self.states = next_states
```

### Comparing `skrl-0.9.1/skrl/trainers/torch/manual.py` & `skrl-1.0.0rc1/skrl/trainers/torch/manual.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Union, List, Optional
+from typing import List, Optional, Union
 
 import copy
 import tqdm
 
 import torch
 
-from skrl.envs.torch import Wrapper
 from skrl.agents.torch import Agent
-
+from skrl.envs.torch import Wrapper
 from skrl.trainers.torch import Trainer
 
 
 MANUAL_TRAINER_DEFAULT_CONFIG = {
     "timesteps": 100000,            # number of timesteps to train for
     "headless": False,              # whether to use headless mode (no rendering)
     "disable_progressbar": False,   # whether to disable the progressbar. If None, disable on non-TTY
+    "close_environment_at_exit": True,   # whether to close the environment on normal program termination
 }
 
 
 class ManualTrainer(Trainer):
     def __init__(self,
                  env: Wrapper,
                  agents: Union[Agent, List[Agent]],
@@ -28,27 +28,27 @@
 
         Train agents by manually controlling the training/evaluation loop
 
         :param env: Environment to train on
         :type env: skrl.env.torch.Wrapper
         :param agents: Agents to train
         :type agents: Union[Agent, List[Agent]]
-        :param agents_scope: Number of environments for each agent to train on (default: [])
-        :type agents_scope: tuple or list of integers
-        :param cfg: Configuration dictionary (default: {}).
+        :param agents_scope: Number of environments for each agent to train on (default: ``None``)
+        :type agents_scope: tuple or list of int, optional
+        :param cfg: Configuration dictionary (default: ``None``).
                     See MANUAL_TRAINER_DEFAULT_CONFIG for default values
         :type cfg: dict, optional
         """
         _cfg = copy.deepcopy(MANUAL_TRAINER_DEFAULT_CONFIG)
         _cfg.update(cfg if cfg is not None else {})
         agents_scope = agents_scope if agents_scope is not None else []
         super().__init__(env=env, agents=agents, agents_scope=agents_scope, cfg=_cfg)
 
         # init agents
-        if self.num_agents > 1:
+        if self.num_simultaneous_agents > 1:
             for agent in self.agents:
                 agent.init(trainer_cfg=self.cfg)
         else:
             self.agents.init(trainer_cfg=self.cfg)
 
         self._timestep = 0
         self._progress = None
@@ -56,50 +56,50 @@
         self.states = None
 
     def train(self, timestep: Optional[int] = None, timesteps: Optional[int] = None) -> None:
         """Execute a training iteration
 
         This method executes the following steps once:
 
-        - Pre-interaction (sequentially if num_agents > 1)
-        - Compute actions (sequentially if num_agents > 1)
+        - Pre-interaction (sequentially if num_simultaneous_agents > 1)
+        - Compute actions (sequentially if num_simultaneous_agents > 1)
         - Interact with the environments
         - Render scene
-        - Record transitions (sequentially if num_agents > 1)
-        - Post-interaction (sequentially if num_agents > 1)
+        - Record transitions (sequentially if num_simultaneous_agents > 1)
+        - Post-interaction (sequentially if num_simultaneous_agents > 1)
         - Reset environments
 
-        :param timestep: Current timestep
-        :type timestep: int, optional (default: None).
-                        If None, the current timestep will be carried by an internal variable
-        :param timesteps: Total number of timesteps (default: None).
+        :param timestep: Current timestep (default: ``None``).
+                         If None, the current timestep will be carried by an internal variable
+        :type timestep: int, optional
+        :param timesteps: Total number of timesteps (default: ``None``).
                           If None, the total number of timesteps is obtained from the trainer's config
         :type timesteps: int, optional
         """
         if timestep is None:
             self._timestep += 1
             timestep = self._timestep
         timesteps = self.timesteps if timesteps is None else timesteps
 
         if self._progress is None:
             self._progress = tqdm.tqdm(total=timesteps, disable=self.disable_progressbar)
         self._progress.update(n=1)
 
         # set running mode
-        if self.num_agents > 1:
+        if self.num_simultaneous_agents > 1:
             for agent in self.agents:
                 agent.set_running_mode("train")
         else:
             self.agents.set_running_mode("train")
 
         # reset env
         if self.states is None:
             self.states, infos = self.env.reset()
 
-        if self.num_agents == 1:
+        if self.num_simultaneous_agents == 1:
             # pre-interaction
             self.agents.pre_interaction(timestep=timestep, timesteps=timesteps)
 
             # compute actions
             with torch.no_grad():
                 actions = self.agents.act(self.states, timestep=timestep, timesteps=timesteps)[0]
 
@@ -109,22 +109,23 @@
                 agent.pre_interaction(timestep=timestep, timesteps=timesteps)
 
             # compute actions
             with torch.no_grad():
                 actions = torch.vstack([agent.act(self.states[scope[0]:scope[1]], timestep=timestep, timesteps=timesteps)[0] \
                                         for agent, scope in zip(self.agents, self.agents_scope)])
 
-        # step the environments
-        next_states, rewards, terminated, truncated, infos = self.env.step(actions)
+        with torch.no_grad():
+            # step the environments
+            next_states, rewards, terminated, truncated, infos = self.env.step(actions)
 
-        # render scene
-        if not self.headless:
-            self.env.render()
+            # render scene
+            if not self.headless:
+                self.env.render()
 
-        if self.num_agents == 1:
+        if self.num_simultaneous_agents == 1:
             # record the environments' transitions
             with torch.no_grad():
                 self.agents.record_transition(states=self.states,
                                               actions=actions,
                                               rewards=rewards,
                                               next_states=next_states,
                                               terminated=terminated,
@@ -155,73 +156,71 @@
                 agent.post_interaction(timestep=timestep, timesteps=timesteps)
 
         # reset environments
         with torch.no_grad():
             if terminated.any() or truncated.any():
                 self.states, infos = self.env.reset()
             else:
-                self.states.copy_(next_states)
-
+                self.states = next_states
 
     def eval(self, timestep: Optional[int] = None, timesteps: Optional[int] = None) -> None:
         """Evaluate the agents sequentially
 
         This method executes the following steps in loop:
 
-        - Compute actions (sequentially if num_agents > 1)
+        - Compute actions (sequentially if num_simultaneous_agents > 1)
         - Interact with the environments
         - Render scene
         - Reset environments
 
-        :param timestep: Current timestep
-        :type timestep: int, optional (default: None).
-                        If None, the current timestep will be carried by an internal variable
-        :param timesteps: Total number of timesteps (default: None).
+        :param timestep: Current timestep (default: ``None``).
+                         If None, the current timestep will be carried by an internal variable
+        :type timestep: int, optional
+        :param timesteps: Total number of timesteps (default: ``None``).
                           If None, the total number of timesteps is obtained from the trainer's config
         :type timesteps: int, optional
         """
         if timestep is None:
             self._timestep += 1
             timestep = self._timestep
         timesteps = self.timesteps if timesteps is None else timesteps
 
         if self._progress is None:
             self._progress = tqdm.tqdm(total=timesteps, disable=self.disable_progressbar)
         self._progress.update(n=1)
 
         # set running mode
-        if self.num_agents > 1:
+        if self.num_simultaneous_agents > 1:
             for agent in self.agents:
                 agent.set_running_mode("eval")
         else:
             self.agents.set_running_mode("eval")
 
         # reset env
         if self.states is None:
             self.states, infos = self.env.reset()
 
         with torch.no_grad():
-            if self.num_agents == 1:
+            if self.num_simultaneous_agents == 1:
                 # compute actions
                 actions = self.agents.act(self.states, timestep=timestep, timesteps=timesteps)[0]
 
             else:
                 # compute actions
                 actions = torch.vstack([agent.act(self.states[scope[0]:scope[1]], timestep=timestep, timesteps=timesteps)[0] \
                                         for agent, scope in zip(self.agents, self.agents_scope)])
 
-        # step the environments
-        next_states, rewards, terminated, truncated, infos = self.env.step(actions)
+            # step the environments
+            next_states, rewards, terminated, truncated, infos = self.env.step(actions)
 
-        # render scene
-        if not self.headless:
-            self.env.render()
+            # render scene
+            if not self.headless:
+                self.env.render()
 
-        with torch.no_grad():
-            if self.num_agents == 1:
+            if self.num_simultaneous_agents == 1:
                 # write data to TensorBoard
                 self.agents.record_transition(states=self.states,
                                               actions=actions,
                                               rewards=rewards,
                                               next_states=next_states,
                                               terminated=terminated,
                                               truncated=truncated,
@@ -244,8 +243,8 @@
                                             timesteps=timesteps)
                     super(type(agent), agent).post_interaction(timestep=timestep, timesteps=timesteps)
 
             # reset environments
             if terminated.any() or truncated.any():
                 self.states, infos = self.env.reset()
             else:
-                self.states.copy_(next_states)
+                self.states = next_states
```

### Comparing `skrl-0.9.1/skrl/trainers/torch/parallel.py` & `skrl-1.0.0rc1/skrl/trainers/torch/parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Union, List, Optional
+from typing import List, Optional, Union
 
 import copy
 import tqdm
 
 import torch
 import torch.multiprocessing as mp
 
-from skrl.envs.torch import Wrapper
 from skrl.agents.torch import Agent
-
+from skrl.envs.torch import Wrapper
 from skrl.trainers.torch import Trainer
 
 
 PARALLEL_TRAINER_DEFAULT_CONFIG = {
     "timesteps": 100000,            # number of timesteps to train for
     "headless": False,              # whether to use headless mode (no rendering)
     "disable_progressbar": False,   # whether to disable the progressbar. If None, disable on non-TTY
+    "close_environment_at_exit": True,   # whether to close the environment on normal program termination
 }
 
 
 def fn_processor(process_index, *args):
-    print("[INFO] Processor {}: started".format(process_index))
+    print(f"[INFO] Processor {process_index}: started")
 
     pipe = args[0][process_index]
     queue = args[1][process_index]
     barrier = args[2]
     scope = args[3][process_index]
     trainer_cfg = args[4]
 
@@ -43,15 +43,15 @@
         if task == 'terminate':
             break
 
         # initialize agent
         elif task == 'init':
             agent = queue.get()
             agent.init(trainer_cfg=trainer_cfg)
-            print("[INFO] Processor {}: init agent {} with scope {}".format(process_index, type(agent).__name__, scope))
+            print(f"[INFO] Processor {process_index}: init agent {type(agent).__name__} with scope {scope}")
             barrier.wait()
 
         # execute agent's pre-interaction step
         elif task == "pre_interaction":
             agent.pre_interaction(timestep=msg['timestep'], timesteps=msg['timesteps'])
             barrier.wait()
 
@@ -110,17 +110,17 @@
 
         Train agents in parallel using multiple processes
 
         :param env: Environment to train on
         :type env: skrl.env.torch.Wrapper
         :param agents: Agents to train
         :type agents: Union[Agent, List[Agent]]
-        :param agents_scope: Number of environments for each agent to train on (default: [])
-        :type agents_scope: tuple or list of integers
-        :param cfg: Configuration dictionary (default: {}).
+        :param agents_scope: Number of environments for each agent to train on (default: ``None``)
+        :type agents_scope: tuple or list of int, optional
+        :param cfg: Configuration dictionary (default: ``None``).
                     See PARALLEL_TRAINER_DEFAULT_CONFIG for default values
         :type cfg: dict, optional
         """
         _cfg = copy.deepcopy(PARALLEL_TRAINER_DEFAULT_CONFIG)
         _cfg.update(cfg if cfg is not None else {})
         agents_scope = agents_scope if agents_scope is not None else []
         super().__init__(env=env, agents=agents, agents_scope=agents_scope, cfg=_cfg)
@@ -137,34 +137,39 @@
         - Interact with the environments
         - Render scene
         - Record transitions (in parallel)
         - Post-interaction (in parallel)
         - Reset environments
         """
         # set running mode
-        if self.num_agents > 1:
+        if self.num_simultaneous_agents > 1:
             for agent in self.agents:
                 agent.set_running_mode("train")
         else:
             self.agents.set_running_mode("train")
 
-        # single agent
-        if self.num_agents == 1:
+        # non-simultaneous agents
+        if self.num_simultaneous_agents == 1:
             self.agents.init(trainer_cfg=self.cfg)
-            self.single_agent_train()
+            # single-agent
+            if self.env.num_agents == 1:
+                self.single_agent_train()
+            # multi-agent
+            else:
+                self.multi_agent_train()
             return
 
         # initialize multiprocessing variables
         queues = []
         producer_pipes = []
         consumer_pipes = []
-        barrier = mp.Barrier(self.num_agents + 1)
+        barrier = mp.Barrier(self.num_simultaneous_agents + 1)
         processes = []
 
-        for i in range(self.num_agents):
+        for i in range(self.num_simultaneous_agents):
             pipe_read, pipe_write = mp.Pipe(duplex=False)
             producer_pipes.append(pipe_write)
             consumer_pipes.append(pipe_read)
             queues.append(mp.Queue())
 
         # move tensors to shared memory
         for agent in self.agents:
@@ -173,15 +178,15 @@
             for model in agent.models.values():
                 try:
                     model.share_memory()
                 except RuntimeError:
                     pass
 
         # spawn and wait for all processes to start
-        for i in range(self.num_agents):
+        for i in range(self.num_simultaneous_agents):
             process = mp.Process(target=fn_processor,
                                  args=(i, consumer_pipes, queues, barrier, self.agents_scope, self.cfg),
                                  daemon=True)
             processes.append(process)
             process.start()
         barrier.wait()
 
@@ -208,23 +213,22 @@
                 for pipe, queue in zip(producer_pipes, queues):
                     pipe.send({"task": "act", "timestep": timestep, "timesteps": self.timesteps})
                     queue.put(states)
 
                 barrier.wait()
                 actions = torch.vstack([queue.get() for queue in queues])
 
-            # step the environments
-            next_states, rewards, terminated, truncated, infos = self.env.step(actions)
+                # step the environments
+                next_states, rewards, terminated, truncated, infos = self.env.step(actions)
 
-            # render scene
-            if not self.headless:
-                self.env.render()
+                # render scene
+                if not self.headless:
+                    self.env.render()
 
-            # record the environments' transitions
-            with torch.no_grad():
+                # record the environments' transitions
                 if not rewards.is_cuda:
                     rewards.share_memory_()
                 if not next_states.is_cuda:
                     next_states.share_memory_()
                 if not terminated.is_cuda:
                     terminated.share_memory_()
                 if not truncated.is_cuda:
@@ -257,48 +261,50 @@
         for pipe in producer_pipes:
             pipe.send({"task": "terminate"})
 
         # join processes
         for process in processes:
             process.join()
 
-        # close the environment
-        self.env.close()
-
     def eval(self) -> None:
         """Evaluate the agents sequentially
 
         This method executes the following steps in loop:
 
         - Compute actions (in parallel)
         - Interact with the environments
         - Render scene
         - Reset environments
         """
         # set running mode
-        if self.num_agents > 1:
+        if self.num_simultaneous_agents > 1:
             for agent in self.agents:
                 agent.set_running_mode("eval")
         else:
             self.agents.set_running_mode("eval")
 
-        # single agent
-        if self.num_agents == 1:
+        # non-simultaneous agents
+        if self.num_simultaneous_agents == 1:
             self.agents.init(trainer_cfg=self.cfg)
-            self.single_agent_eval()
+            # single-agent
+            if self.env.num_agents == 1:
+                self.single_agent_eval()
+            # multi-agent
+            else:
+                self.multi_agent_eval()
             return
 
         # initialize multiprocessing variables
         queues = []
         producer_pipes = []
         consumer_pipes = []
-        barrier = mp.Barrier(self.num_agents + 1)
+        barrier = mp.Barrier(self.num_simultaneous_agents + 1)
         processes = []
 
-        for i in range(self.num_agents):
+        for i in range(self.num_simultaneous_agents):
             pipe_read, pipe_write = mp.Pipe(duplex=False)
             producer_pipes.append(pipe_write)
             consumer_pipes.append(pipe_read)
             queues.append(mp.Queue())
 
         # move tensors to shared memory
         for agent in self.agents:
@@ -308,15 +314,15 @@
                 if model is not None:
                     try:
                         model.share_memory()
                     except RuntimeError:
                         pass
 
         # spawn and wait for all processes to start
-        for i in range(self.num_agents):
+        for i in range(self.num_simultaneous_agents):
             process = mp.Process(target=fn_processor,
                                  args=(i, consumer_pipes, queues, barrier, self.agents_scope, self.cfg),
                                  daemon=True)
             processes.append(process)
             process.start()
         barrier.wait()
 
@@ -338,22 +344,21 @@
                 for pipe, queue in zip(producer_pipes, queues):
                     pipe.send({"task": "act", "timestep": timestep, "timesteps": self.timesteps})
                     queue.put(states)
 
                 barrier.wait()
                 actions = torch.vstack([queue.get() for queue in queues])
 
-            # step the environments
-            next_states, rewards, terminated, truncated, infos = self.env.step(actions)
+                # step the environments
+                next_states, rewards, terminated, truncated, infos = self.env.step(actions)
 
-            # render scene
-            if not self.headless:
-                self.env.render()
+                # render scene
+                if not self.headless:
+                    self.env.render()
 
-            with torch.no_grad():
                 # write data to TensorBoard
                 if not rewards.is_cuda:
                     rewards.share_memory_()
                 if not next_states.is_cuda:
                     next_states.share_memory_()
                 if not terminated.is_cuda:
                     terminated.share_memory_()
@@ -382,10 +387,7 @@
         # terminate processes
         for pipe in producer_pipes:
             pipe.send({"task": "terminate"})
 
         # join processes
         for process in processes:
             process.join()
-
-        # close the environment
-        self.env.close()
```

### Comparing `skrl-0.9.1/skrl/trainers/torch/sequential.py` & `skrl-1.0.0rc1/skrl/trainers/jax/sequential.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-from typing import Union, List, Optional
+from typing import List, Optional, Union
 
+import contextlib
 import copy
 import tqdm
 
-import torch
+import jax.numpy as jnp
 
-from skrl.envs.torch import Wrapper
-from skrl.agents.torch import Agent
-
-from skrl.trainers.torch import Trainer
+from skrl.agents.jax import Agent
+from skrl.envs.jax import Wrapper
+from skrl.trainers.jax import Trainer
 
 
 SEQUENTIAL_TRAINER_DEFAULT_CONFIG = {
     "timesteps": 100000,            # number of timesteps to train for
     "headless": False,              # whether to use headless mode (no rendering)
     "disable_progressbar": False,   # whether to disable the progressbar. If None, disable on non-TTY
+    "close_environment_at_exit": True,   # whether to close the environment on normal program termination
 }
 
 
 class SequentialTrainer(Trainer):
     def __init__(self,
                  env: Wrapper,
                  agents: Union[Agent, List[Agent]],
                  agents_scope: Optional[List[int]] = None,
                  cfg: Optional[dict] = None) -> None:
         """Sequential trainer
 
         Train agents sequentially (i.e., one after the other in each interaction with the environment)
 
         :param env: Environment to train on
-        :type env: skrl.env.torch.Wrapper
+        :type env: skrl.env.jax.Wrapper
         :param agents: Agents to train
         :type agents: Union[Agent, List[Agent]]
-        :param agents_scope: Number of environments for each agent to train on (default: [])
-        :type agents_scope: tuple or list of integers
-        :param cfg: Configuration dictionary (default: {}).
+        :param agents_scope: Number of environments for each agent to train on (default: ``None``)
+        :type agents_scope: tuple or list of int, optional
+        :param cfg: Configuration dictionary (default: ``None``).
                     See SEQUENTIAL_TRAINER_DEFAULT_CONFIG for default values
         :type cfg: dict, optional
         """
         _cfg = copy.deepcopy(SEQUENTIAL_TRAINER_DEFAULT_CONFIG)
         _cfg.update(cfg if cfg is not None else {})
         agents_scope = agents_scope if agents_scope is not None else []
         super().__init__(env=env, agents=agents, agents_scope=agents_scope, cfg=_cfg)
 
         # init agents
-        if self.num_agents > 1:
+        if self.num_simultaneous_agents > 1:
             for agent in self.agents:
                 agent.init(trainer_cfg=self.cfg)
         else:
             self.agents.init(trainer_cfg=self.cfg)
 
     def train(self) -> None:
         """Train the agents sequentially
@@ -60,48 +61,53 @@
         - Interact with the environments
         - Render scene
         - Record transitions (sequentially)
         - Post-interaction (sequentially)
         - Reset environments
         """
         # set running mode
-        if self.num_agents > 1:
+        if self.num_simultaneous_agents > 1:
             for agent in self.agents:
                 agent.set_running_mode("train")
         else:
             self.agents.set_running_mode("train")
 
-        # single agent
-        if self.num_agents == 1:
-            self.single_agent_train()
+        # non-simultaneous agents
+        if self.num_simultaneous_agents == 1:
+            # single-agent
+            if self.env.num_agents == 1:
+                self.single_agent_train()
+            # multi-agent
+            else:
+                self.multi_agent_train()
             return
 
         # reset env
         states, infos = self.env.reset()
 
         for timestep in tqdm.tqdm(range(self.initial_timestep, self.timesteps), disable=self.disable_progressbar):
 
             # pre-interaction
             for agent in self.agents:
                 agent.pre_interaction(timestep=timestep, timesteps=self.timesteps)
 
             # compute actions
-            with torch.no_grad():
-                actions = torch.vstack([agent.act(states[scope[0]:scope[1]], timestep=timestep, timesteps=self.timesteps)[0] \
-                                        for agent, scope in zip(self.agents, self.agents_scope)])
+            with contextlib.nullcontext():
+                actions = jnp.vstack([agent.act(states[scope[0]:scope[1]], timestep=timestep, timesteps=self.timesteps)[0] \
+                                      for agent, scope in zip(self.agents, self.agents_scope)])
 
             # step the environments
             next_states, rewards, terminated, truncated, infos = self.env.step(actions)
 
             # render scene
             if not self.headless:
                 self.env.render()
 
             # record the environments' transitions
-            with torch.no_grad():
+            with contextlib.nullcontext():
                 for agent, scope in zip(self.agents, self.agents_scope):
                     agent.record_transition(states=states[scope[0]:scope[1]],
                                             actions=actions[scope[0]:scope[1]],
                                             rewards=rewards[scope[0]:scope[1]],
                                             next_states=next_states[scope[0]:scope[1]],
                                             terminated=terminated[scope[0]:scope[1]],
                                             truncated=truncated[scope[0]:scope[1]],
@@ -110,63 +116,65 @@
                                             timesteps=self.timesteps)
 
             # post-interaction
             for agent in self.agents:
                 agent.post_interaction(timestep=timestep, timesteps=self.timesteps)
 
             # reset environments
-            with torch.no_grad():
+            with contextlib.nullcontext():
                 if terminated.any() or truncated.any():
                     states, infos = self.env.reset()
                 else:
-                    states.copy_(next_states)
-
-        # close the environment
-        self.env.close()
+                    states = next_states
 
     def eval(self) -> None:
         """Evaluate the agents sequentially
 
         This method executes the following steps in loop:
 
         - Compute actions (sequentially)
         - Interact with the environments
         - Render scene
         - Reset environments
         """
         # set running mode
-        if self.num_agents > 1:
+        if self.num_simultaneous_agents > 1:
             for agent in self.agents:
                 agent.set_running_mode("eval")
         else:
             self.agents.set_running_mode("eval")
 
-        # single agent
-        if self.num_agents == 1:
-            self.single_agent_eval()
+        # non-simultaneous agents
+        if self.num_simultaneous_agents == 1:
+            # single-agent
+            if self.env.num_agents == 1:
+                self.single_agent_eval()
+            # multi-agent
+            else:
+                self.multi_agent_eval()
             return
 
         # reset env
         states, infos = self.env.reset()
 
         for timestep in tqdm.tqdm(range(self.initial_timestep, self.timesteps), disable=self.disable_progressbar):
 
             # compute actions
-            with torch.no_grad():
-                actions = torch.vstack([agent.act(states[scope[0]:scope[1]], timestep=timestep, timesteps=self.timesteps)[0] \
-                                        for agent, scope in zip(self.agents, self.agents_scope)])
+            with contextlib.nullcontext():
+                actions = jnp.vstack([agent.act(states[scope[0]:scope[1]], timestep=timestep, timesteps=self.timesteps)[0] \
+                                      for agent, scope in zip(self.agents, self.agents_scope)])
 
             # step the environments
             next_states, rewards, terminated, truncated, infos = self.env.step(actions)
 
             # render scene
             if not self.headless:
                 self.env.render()
 
-            with torch.no_grad():
+            with contextlib.nullcontext():
                 # write data to TensorBoard
                 for agent, scope in zip(self.agents, self.agents_scope):
                     agent.record_transition(states=states[scope[0]:scope[1]],
                                             actions=actions[scope[0]:scope[1]],
                                             rewards=rewards[scope[0]:scope[1]],
                                             next_states=next_states[scope[0]:scope[1]],
                                             terminated=terminated[scope[0]:scope[1]],
@@ -176,11 +184,8 @@
                                             timesteps=self.timesteps)
                     super(type(agent), agent).post_interaction(timestep=timestep, timesteps=self.timesteps)
 
                 # reset environments
                 if terminated.any() or truncated.any():
                     states, infos = self.env.reset()
                 else:
-                    states.copy_(next_states)
-
-        # close the environment
-        self.env.close()
+                    states = next_states
```

### Comparing `skrl-0.9.1/skrl/utils/__init__.py` & `skrl-1.0.0rc1/skrl/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from typing import Optional
 
 import os
+import random
 import sys
 import time
-import torch
-import random
+
 import numpy as np
 
-from skrl import logger
+from skrl import config, logger
 
 
 def set_seed(seed: Optional[int] = None, deterministic: bool = False) -> int:
     """
     Set the seed for the random number generators
 
     Due to NumPy's legacy seeding constraint the seed must be between 0 and 2**32 - 1.
     Otherwise a NumPy exception (``ValueError: Seed must be between 0 and 2**32 - 1``) will be raised
 
     Modified packages:
 
     - random
     - numpy
-    - torch
+    - torch (if available)
+    - jax (skrl's PRNG key: ``config.jax.key``)
 
     Example::
 
         # fixed seed
         >>> from skrl.utils import set_seed
         >>> set_seed(42)
         [skrl:INFO] Seed: 42
@@ -35,51 +36,65 @@
         >>> from skrl.utils import set_seed
         >>> set_seed()
         [skrl:INFO] Seed: 1776118066
         1776118066
 
         # enable deterministic. The following environment variables should be established:
         # - CUDA 10.1: CUDA_LAUNCH_BLOCKING=1
-        # - CUDA 10.2 or later: CUBLAS_WORKSPACE_CONFIG=:16:8 or CUBLAS_WORKSPACE_CONFIG=:4096:2
+        # - CUDA 10.2 or later: CUBLAS_WORKSPACE_CONFIG=:16:8 or CUBLAS_WORKSPACE_CONFIG=:4096:8
         >>> from skrl.utils import set_seed
         >>> set_seed(42, deterministic=True)
         [skrl:INFO] Seed: 42
         [skrl:WARNING] PyTorch/cuDNN deterministic algorithms are enabled. This may affect performance
         42
 
     :param seed: The seed to set. Is None, a random seed will be generated (default: ``None``)
     :type seed: int, optional
     :param deterministic: Whether PyTorch is configured to use deterministic algorithms (default: ``False``).
                           The following environment variables should be established for CUDA 10.1 (``CUDA_LAUNCH_BLOCKING=1``)
-                          and for CUDA 10.2 or later (``CUBLAS_WORKSPACE_CONFIG=:16:8`` or ``CUBLAS_WORKSPACE_CONFIG=:4096:2``).
+                          and for CUDA 10.2 or later (``CUBLAS_WORKSPACE_CONFIG=:16:8`` or ``CUBLAS_WORKSPACE_CONFIG=:4096:8``).
                           See PyTorch `Reproducibility <https://pytorch.org/docs/stable/notes/randomness.html>`_ for details
     :type deterministic: bool, optional
 
     :return: Seed
     :rtype: int
     """
     # generate a random seed
     if seed is None:
         try:
             seed = int.from_bytes(os.urandom(4), byteorder=sys.byteorder)
         except NotImplementedError:
             seed = int(time.time() * 1000)
         seed %= 2 ** 31  # NumPy's legacy seeding seed must be between 0 and 2**32 - 1
 
+    seed = int(seed)
+    logger.info(f"Seed: {seed}")
+
+    # numpy
     random.seed(seed)
     np.random.seed(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed(seed)
-    torch.cuda.manual_seed_all(seed)
-
-    logger.info("Seed: {}".format(seed))
-
-    if deterministic:
-        torch.backends.cudnn.benchmark = False
-        torch.backends.cudnn.deterministic = True
 
-        # On CUDA 10.1, set environment variable CUDA_LAUNCH_BLOCKING=1
-        # On CUDA 10.2 or later, set environment variable CUBLAS_WORKSPACE_CONFIG=:16:8 or CUBLAS_WORKSPACE_CONFIG=:4096:2
+    # torch
+    try:
+        import torch
+
+        torch.manual_seed(seed)
+        torch.cuda.manual_seed(seed)
+        torch.cuda.manual_seed_all(seed)
+
+        if deterministic:
+            torch.backends.cudnn.benchmark = False
+            torch.backends.cudnn.deterministic = True
+
+            # On CUDA 10.1, set environment variable CUDA_LAUNCH_BLOCKING=1
+            # On CUDA 10.2 or later, set environment variable CUBLAS_WORKSPACE_CONFIG=:16:8 or CUBLAS_WORKSPACE_CONFIG=:4096:8
+
+            logger.warning("PyTorch/cuDNN deterministic algorithms are enabled. This may affect performance")
+    except ImportError:
+        pass
+    except Exception as e:
+        logger.warning(f"PyTorch seeding error: {e}")
 
-        logger.warning("PyTorch/cuDNN deterministic algorithms are enabled. This may affect performance")
+    # jax
+    config.jax.key = seed
 
     return seed
```

### Comparing `skrl-0.9.1/skrl/utils/control.py` & `skrl-1.0.0rc1/skrl/utils/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import isaacgym.torch_utils as torch_utils
+
 import torch
 
 
 def ik(jacobian_end_effector,
        current_position, current_orientation,
        goal_position, goal_orientation,
        damping_factor=0.05):
```

### Comparing `skrl-0.9.1/skrl/utils/huggingface.py` & `skrl-1.0.0rc1/skrl/utils/huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from skrl import logger, __version__
+from skrl import __version__, logger
 
 
 def download_model_from_huggingface(repo_id: str, filename: str = "agent.pt") -> str:
     """Download a model from Hugging Face Hub
 
     :param repo_id: Hugging Face user or organization name and a repo name separated by a ``/``
     :type repo_id: str
@@ -23,14 +23,15 @@
         '/home/user/.cache/huggingface/hub/models--skrl--OmniIsaacGymEnvs-Cartpole-PPO/snapshots/892e629903de6bf3ef102ae760406a5dd0f6f873/agent.pt'
 
         # download model (e.g. "policy.pth") from another user/organization (e.g. "org/ddpg-Pendulum-v1")
         >>> from skrl.utils.huggingface import download_model_from_huggingface
         >>> download_model_from_huggingface("org/ddpg-Pendulum-v1", "policy.pth")
         '/home/user/.cache/huggingface/hub/models--org--ddpg-Pendulum-v1/snapshots/b44ee96f93ff2e296156b002a2ca4646e197ba32/policy.pth'
     """
+    logger.info(f"Downloading model from Hugging Face Hub: {repo_id}/{filename}")
     try:
         import huggingface_hub
     except ImportError:
         logger.error("Hugging Face Hub package is not installed. Use 'pip install huggingface-hub' to install it")
         huggingface_hub = None
 
     if huggingface_hub is None:
```

### Comparing `skrl-0.9.1/skrl/utils/isaacgym_utils.py` & `skrl-1.0.0rc1/skrl/utils/isaacgym_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import List, Optional
 
-import math
 import logging
+import math
 import threading
+
 import numpy as np
+import torch
+
+
 try:
     import flask
 except ImportError:
     flask = None
 
 try:
     import imageio
@@ -16,16 +20,14 @@
     from isaacgym import gymapi
 except ImportError:
     imageio = None
     isaacgym = None
     torch_utils = None
     gymapi = None
 
-import torch
-
 
 class WebViewer:
     def __init__(self, host: str = "127.0.0.1", port: int = 5000) -> None:
         """
         Web viewer for Isaac Gym
 
         :param host: Host address (default: "127.0.0.1")
@@ -51,15 +53,15 @@
         self._event_load = threading.Event()
         self._event_stream = threading.Event()
 
         # start server
         self._thread = threading.Thread(target=lambda: \
             self._app.run(host=host, port=port, debug=False, use_reloader=False), daemon=True)
         self._thread.start()
-        print("\nStarting web viewer on http://{}:{}/\n".format(host, port))
+        print(f"\nStarting web viewer on http://{host}:{port}/\n")
 
     def _route_index(self) -> 'flask.Response':
         """Render the web page
 
         :return: Flask response
         :rtype: flask.Response
         """
@@ -424,36 +426,35 @@
     else:
         return transpose @ torch.inverse(jacobian_end_effector @ transpose + lmbda) @ error
 
 def print_arguments(args):
     print("")
     print("Arguments")
     for a in args.__dict__:
-        print("  |-- {}: {}".format(a, args.__getattribute__(a)))
+        print(f"  |-- {a}: {args.__getattribute__(a)}")
 
 def print_asset_options(asset_options: 'isaacgym.gymapi.AssetOptions', asset_name: str = ""):
     attrs = ["angular_damping", "armature", "collapse_fixed_joints", "convex_decomposition_from_submeshes",
              "default_dof_drive_mode", "density", "disable_gravity", "fix_base_link", "flip_visual_attachments",
              "linear_damping", "max_angular_velocity", "max_linear_velocity", "mesh_normal_mode", "min_particle_mass",
              "override_com", "override_inertia", "replace_cylinder_with_capsule", "tendon_limit_stiffness", "thickness",
              "use_mesh_materials", "use_physx_armature", "vhacd_enabled"]  # vhacd_params
-    print("\nAsset options{}".format(" ({})".format(asset_name) if asset_name else ""))
+    print("\nAsset options{}".format(f" ({asset_name})" if asset_name else ""))
     for attr in attrs:
         print("  |-- {}: {}".format(attr, getattr(asset_options, attr) if hasattr(asset_options, attr) else "--"))
         # vhacd attributes
         if attr == "vhacd_enabled" and hasattr(asset_options, attr) and getattr(asset_options, attr):
             vhacd_attrs = ["alpha", "beta", "concavity", "convex_hull_approximation", "convex_hull_downsampling",
                            "max_convex_hulls", "max_num_vertices_per_ch", "min_volume_per_ch", "mode", "ocl_acceleration",
                            "pca", "plane_downsampling", "project_hull_vertices", "resolution"]
             print("  |-- vhacd_params:")
             for vhacd_attr in vhacd_attrs:
                 print("  |   |-- {}: {}".format(vhacd_attr, getattr(asset_options.vhacd_params, vhacd_attr) \
                     if hasattr(asset_options.vhacd_params, vhacd_attr) else "--"))
 
-
 def print_sim_components(gym, sim):
     print("")
     print("Sim components")
     print("  |--  env count:", gym.get_env_count(sim))
     print("  |--  actor count:", gym.get_sim_actor_count(sim))
     print("  |--  rigid body count:", gym.get_sim_rigid_body_count(sim))
     print("  |--  joint count:", gym.get_sim_joint_count(sim))
@@ -500,11 +501,11 @@
 def print_links_and_dofs(gym, asset):
     link_dict = gym.get_asset_rigid_body_dict(asset)
     dof_dict = gym.get_asset_dof_dict(asset)
 
     print("")
     print("Links")
     for k in link_dict:
-        print("  |-- {}: {}".format(k, link_dict[k]))
+        print(f"  |-- {k}: {link_dict[k]}")
     print("DOFs")
     for k in dof_dict:
-        print("  |-- {}: {}".format(k, dof_dict[k]))
+        print(f"  |-- {k}: {dof_dict[k]}")
```

### Comparing `skrl-0.9.1/skrl/utils/model_instantiators.py` & `skrl-1.0.0rc1/skrl/utils/model_instantiators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import Union, Tuple, Optional
+from typing import Any, Mapping, Optional, Sequence, Tuple, Union
 
+from enum import Enum
 import gym
 import gymnasium
-from enum import Enum
 
 import torch
 import torch.nn as nn
 
-from skrl.models.torch import Model
-from skrl.models.torch import GaussianMixin
-from skrl.models.torch import CategoricalMixin
-from skrl.models.torch import DeterministicMixin
-from skrl.models.torch import MultivariateGaussianMixin
+from skrl.models.torch import Model  # noqa
+from skrl.models.torch import CategoricalMixin, DeterministicMixin, GaussianMixin, MultivariateGaussianMixin  # noqa
+
 
 __all__ = ["categorical_model", "deterministic_model", "gaussian_model", "multivariate_gaussian_model", "Shape"]
 
 
 class Shape(Enum):
     """
     Enum to select the shape of the model's inputs and outputs
@@ -38,23 +36,26 @@
     - "selu"
     - "sigmoid"
     - "softmax"
     - "softplus"
     - "softsign"
     - "tanh"
 
-    :param activation: activation function name
+    :param activation: activation function name.
+                       If activation is an empty string, a placeholder will be returned (``torch.nn.Identity()``)
     :type activation: str
 
     :raises: ValueError if activation is not a valid activation function
 
     :return: activation function
     :rtype: nn.Module
     """
-    if activation == "relu":
+    if not activation:
+        return torch.nn.Identity()
+    elif activation == "relu":
         return torch.nn.ReLU()
     elif activation == "tanh":
         return torch.nn.Tanh()
     elif activation == "sigmoid":
         return torch.nn.Sigmoid()
     elif activation == "leaky_relu":
         return torch.nn.LeakyReLU()
@@ -65,15 +66,15 @@
     elif activation == "softsign":
         return torch.nn.Softsign()
     elif activation == "selu":
         return torch.nn.SELU()
     elif activation == "softmax":
         return torch.nn.Softmax()
     else:
-        raise ValueError("Unknown activation function: {}".format(activation))
+        raise ValueError(f"Unknown activation function: {activation}")
 
 def _get_num_units_by_shape(model: Model, shape: Shape) -> int:
     """Get the number of units in a layer by shape
 
     :param model: Model to get the number of units for
     :type model: Model
     :param shape: Shape of the layer
@@ -82,15 +83,18 @@
     :return: Number of units in the layer
     :rtype: int
     """
     num_units = {Shape.ONE: 1,
                  Shape.STATES: model.num_observations,
                  Shape.ACTIONS: model.num_actions,
                  Shape.STATES_ACTIONS: model.num_observations + model.num_actions}
-    return num_units[shape]
+    try:
+        return num_units[shape]
+    except:
+        return shape
 
 def _generate_sequential(model: Model,
                          input_shape: Shape = Shape.STATES,
                          hiddens: list = [256, 256],
                          hidden_activation: list = ["relu", "relu"],
                          output_shape: Shape = Shape.ACTIONS,
                          output_activation: Union[str, None] = "tanh",
@@ -148,16 +152,16 @@
 
     :param observation_space: Observation/state space or shape (default: None).
                               If it is not None, the num_observations property will contain the size of that space
     :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
     :param action_space: Action space or shape (default: None).
                          If it is not None, the num_actions property will contain the size of that space
     :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-    :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                   If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+    :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                   If None, the device will be either ``"cuda"`` if available or ``"cpu"``
     :type device: str or torch.device, optional
     :param clip_actions: Flag to indicate whether the actions should be clipped (default: False)
     :type clip_actions: bool, optional
     :param clip_log_std: Flag to indicate whether the log standard deviations should be clipped (default: True)
     :type clip_log_std: bool, optional
     :param min_log_std: Minimum value of the log standard deviation (default: -20)
     :type min_log_std: float, optional
@@ -241,16 +245,16 @@
 
     :param observation_space: Observation/state space or shape (default: None).
                               If it is not None, the num_observations property will contain the size of that space
     :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
     :param action_space: Action space or shape (default: None).
                          If it is not None, the num_actions property will contain the size of that space
     :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-    :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                   If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+    :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                   If None, the device will be either ``"cuda"`` if available or ``"cpu"``
     :type device: str or torch.device, optional
     :param clip_actions: Flag to indicate whether the actions should be clipped (default: False)
     :type clip_actions: bool, optional
     :param clip_log_std: Flag to indicate whether the log standard deviations should be clipped (default: True)
     :type clip_log_std: bool, optional
     :param min_log_std: Minimum value of the log standard deviation (default: -20)
     :type min_log_std: float, optional
@@ -329,18 +333,18 @@
                         output_scale: float = 1.0) -> Model:
     """Instantiate a deterministic model
 
     :param observation_space: Observation/state space or shape (default: None).
                               If it is not None, the num_observations property will contain the size of that space
     :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
     :param action_space: Action space or shape (default: None).
-                            If it is not None, the num_actions property will contain the size of that space
+                         If it is not None, the num_actions property will contain the size of that space
     :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-    :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                   If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+    :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                   If None, the device will be either ``"cuda"`` if available or ``"cpu"``
     :type device: str or torch.device, optional
     :param clip_actions: Flag to indicate whether the actions should be clipped to the action space (default: False)
     :type clip_actions: bool, optional
     :param input_shape: Shape of the input (default: Shape.STATES)
     :type input_shape: Shape, optional
     :param hiddens: Number of hidden units in each hidden layer
     :type hiddens: int or list of ints
@@ -407,18 +411,18 @@
                       output_activation: Optional[str] = None) -> Model:
     """Instantiate a categorical model
 
     :param observation_space: Observation/state space or shape (default: None).
                               If it is not None, the num_observations property will contain the size of that space
     :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
     :param action_space: Action space or shape (default: None).
-                            If it is not None, the num_actions property will contain the size of that space
+                         If it is not None, the num_actions property will contain the size of that space
     :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
-    :param device: Device on which a torch tensor is or will be allocated (default: ``None``).
-                   If None, the device will be either ``"cuda:0"`` if available or ``"cpu"``
+    :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                   If None, the device will be either ``"cuda"`` if available or ``"cpu"``
     :type device: str or torch.device, optional
     :param unnormalized_log_prob: Flag to indicate how to be interpreted the model's output (default: True).
                                   If True, the model's output is interpreted as unnormalized log probabilities
                                   (it can be any real number), otherwise as normalized probabilities
                                   (the output must be non-negative, finite and have a non-zero sum)
     :type unnormalized_log_prob: bool, optional
     :param input_shape: Shape of the input (default: Shape.STATES)
@@ -466,7 +470,99 @@
                 "output_activation": output_activation}
 
     return CategoricalModel(observation_space=observation_space,
                             action_space=action_space,
                             device=device,
                             unnormalized_log_prob=unnormalized_log_prob,
                             metadata=metadata)
+
+def shared_model(observation_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
+                 action_space: Optional[Union[int, Tuple[int], gym.Space, gymnasium.Space]] = None,
+                 device: Optional[Union[str, torch.device]] = None,
+                 structure: str = "",
+                 roles: Sequence[str] = [],
+                 parameters: Sequence[Mapping[str, Any]] = []) -> Model:
+    """Instantiate a shared model
+
+    :param observation_space: Observation/state space or shape (default: None).
+                              If it is not None, the num_observations property will contain the size of that space
+    :type observation_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
+    :param action_space: Action space or shape (default: None).
+                         If it is not None, the num_actions property will contain the size of that space
+    :type action_space: int, tuple or list of integers, gym.Space, gymnasium.Space or None, optional
+    :param device: Device on which a tensor/array is or will be allocated (default: ``None``).
+                   If None, the device will be either ``"cuda"`` if available or ``"cpu"``
+    :type device: str or torch.device, optional
+    :param structure: Shared model structure (default: ``""``).
+                      Note: this parameter is ignored for the moment
+    :type structure: str, optional
+    :param roles: Organized list of model roles (default: ``[]``)
+    :type roles: sequence of strings, optional
+    :param parameters: Organized list of model instantiator parameters (default: ``[]``)
+    :type parameters: sequence of dict, optional
+
+    :return: Shared model instance
+    :rtype: Model
+    """
+    class GaussianDeterministicModel(GaussianMixin, DeterministicMixin, Model):
+        def __init__(self, observation_space, action_space, device, roles, metadata):
+            Model.__init__(self, observation_space, action_space, device)
+            GaussianMixin.__init__(self,
+                                   clip_actions=metadata[0]["clip_actions"],
+                                   clip_log_std=metadata[0]["clip_log_std"],
+                                   min_log_std=metadata[0]["min_log_std"],
+                                   max_log_std=metadata[0]["max_log_std"],
+                                   role=roles[0])
+            DeterministicMixin.__init__(self, clip_actions=metadata[1]["clip_actions"], role=roles[1])
+
+            self._roles = roles
+            self.instantiator_input_type = metadata[0]["input_shape"].value
+            self.instantiator_output_scales = [m["output_scale"] for m in metadata]
+
+            # shared layers/network
+            self.net = _generate_sequential(model=self,
+                                            input_shape=metadata[0]["input_shape"],
+                                            hiddens=metadata[0]["hiddens"][:-1],
+                                            hidden_activation=metadata[0]["hidden_activation"][:-1],
+                                            output_shape=metadata[0]["hiddens"][-1],
+                                            output_activation=metadata[0]["hidden_activation"][-1])
+
+            # separated layers ("policy")
+            mean_layers = [nn.Linear(metadata[0]["hiddens"][-1], _get_num_units_by_shape(self, metadata[0]["output_shape"]))]
+            if metadata[0]["output_activation"] is not None:
+                mean_layers.append(_get_activation_function(metadata[0]["output_activation"]))
+            self.mean_net = nn.Sequential(*mean_layers)
+
+            self.log_std_parameter = nn.Parameter(torch.zeros(_get_num_units_by_shape(self, metadata[0]["output_shape"])))
+
+            # separated layer ("value")
+            value_layers = [nn.Linear(metadata[1]["hiddens"][-1], _get_num_units_by_shape(self, metadata[1]["output_shape"]))]
+            if metadata[1]["output_activation"] is not None:
+                value_layers.append(_get_activation_function(metadata[1]["output_activation"]))
+            self.value_net = nn.Sequential(*value_layers)
+
+        def act(self, inputs, role):
+            if role == self._roles[0]:
+                return GaussianMixin.act(self, inputs, role)
+            elif role == self._roles[1]:
+                return DeterministicMixin.act(self, inputs, role)
+
+        def compute(self, inputs, role):
+            if self.instantiator_input_type == 0:
+                output = self.net(inputs["states"])
+            elif self.instantiator_input_type == -1:
+                output = self.net(inputs["taken_actions"])
+            elif self.instantiator_input_type == -2:
+                output = self.net(torch.cat((inputs["states"], inputs["taken_actions"]), dim=1))
+
+            if role == self._roles[0]:
+                return self.instantiator_output_scales[0] * self.mean_net(output), self.log_std_parameter, {}
+            elif role == self._roles[1]:
+                return self.instantiator_output_scales[1] * self.value_net(output), {}
+
+    # TODO: define the model using the specified structure
+
+    return GaussianDeterministicModel(observation_space=observation_space,
+                                        action_space=action_space,
+                                        device=device,
+                                        roles=roles,
+                                        metadata=parameters)
```

### Comparing `skrl-0.9.1/skrl/utils/omniverse_isaacgym_utils.py` & `skrl-1.0.0rc1/skrl/utils/omniverse_isaacgym_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from typing import Optional, Union
+from typing import Mapping, Optional
+
+import queue
 
-import torch
 import numpy as np
+import torch
+
+from skrl import logger
 
 
 def _np_quat_mul(a, b):
     assert a.shape == b.shape
     shape = a.shape
     a = a.reshape(-1, 4)
     b = b.reshape(-1, 4)
@@ -55,78 +59,131 @@
     return torch.cat((a[:, :1], -a[:, 1:]), dim=-1).view(shape)
 
 def ik(jacobian_end_effector: torch.Tensor,
        current_position: torch.Tensor,
        current_orientation: torch.Tensor,
        goal_position: torch.Tensor,
        goal_orientation: Optional[torch.Tensor] = None,
-       damping_factor: float = 0.05,
-       squeeze_output: bool = True) -> torch.Tensor:
-    """Inverse kinematics using damped least squares method
+       method: str = "damped least-squares",
+       method_cfg: Mapping[str, float] = {"scale": 1, "damping": 0.05, "min_singular_value": 1e-5},
+       squeeze_output: bool = True,) -> torch.Tensor:
+    """Differential inverse kinematics
 
     :param jacobian_end_effector: End effector's jacobian
     :type jacobian_end_effector: torch.Tensor
     :param current_position: End effector's current position
     :type current_position: torch.Tensor
     :param current_orientation: End effector's current orientation
     :type current_orientation: torch.Tensor
     :param goal_position: End effector's goal position
     :type goal_position: torch.Tensor
-    :param goal_orientation: End effector's goal orientation (default: ``None``)
+    :param goal_orientation: End effector's goal orientation (default: ``None``).
+                             If not provided, the current orientation will be used instead.
     :type goal_orientation: torch.Tensor, optional
-    :param damping_factor: Damping factor (default: ``0.05``)
-    :type damping_factor: float, optional
+    :param method: Differential inverse kinematics formulation (default: ``"damped least-squares"``).
+                   The supported methods are described in the following table:
+
+                   +----------------------------------+----------------------------------+
+                   |IK Method                         |Method tag                        |
+                   +==================================+==================================+
+                   |Damped least-squares              |``"damped least-squares"``        |
+                   +----------------------------------+----------------------------------+
+                   |Tanspose                          |``"transpose"``                   |
+                   +----------------------------------+----------------------------------+
+                   |Pseduoinverse                     |``"pseudoinverse"``               |
+                   +----------------------------------+----------------------------------+
+                   |Singular-vale decomposition (SVD) |``"singular-vale decomposition"`` |
+                   +----------------------------------+----------------------------------+
+    :type method: str, optional
+    :param method_cfg: Method configurations (default: ``{"scale": 1, "damping": 0.05, "min_singular_value": 1e-5}``)
+    :type method_cfg: dict, optional
     :param squeeze_output: Squeeze output (default: ``True``)
     :type squeeze_output: bool, optional
 
     :return: Change in joint angles
     :rtype: torch.Tensor
     """
     if goal_orientation is None:
         goal_orientation = current_orientation
 
     # torch
     if isinstance(jacobian_end_effector, torch.Tensor):
         # compute error
-
         q = _torch_quat_mul(goal_orientation, _torch_quat_conjugate(current_orientation))
         error = torch.cat([goal_position - current_position,  # position error
                            q[:, 1:] * torch.sign(q[:, 0]).unsqueeze(-1)],  # orientation error
                           dim=-1).unsqueeze(-1)
 
-        # solve damped least squares (dO = J.T * V)
-        transpose = torch.transpose(jacobian_end_effector, 1, 2)
-        lmbda = torch.eye(6, device=jacobian_end_effector.device) * (damping_factor ** 2)
-        if squeeze_output:
-            return (transpose @ torch.inverse(jacobian_end_effector @ transpose + lmbda) @ error).squeeze(dim=2)
+        scale = method_cfg.get("scale", 1.0)
+
+        # adaptive Singular Value Decomposition (SVD)
+        if method == "singular-vale decomposition":
+            min_singular_value = method_cfg.get("min_singular_value", 1e-5)
+            U, S, Vh = torch.linalg.svd(jacobian_end_effector)  # U: 6xd, S: dxd, V: d x num_dof
+            inv_s = torch.where(S > min_singular_value, 1.0 / S, torch.zeros_like(S))
+            pseudoinverse = torch.transpose(Vh, 1, 2)[:, :, :6] @ torch.diag_embed(inv_s) @ torch.transpose(U, 1, 2)
+            if squeeze_output:
+                return (scale * pseudoinverse @ error).squeeze(dim=2)
+            else:
+                return scale * pseudoinverse @ error
+        # jacobian pseudoinverse
+        elif method == "pseudoinverse":
+            pseudoinverse = torch.linalg.pinv(jacobian_end_effector)
+            if squeeze_output:
+                return (scale * pseudoinverse @ error).squeeze(dim=2)
+            else:
+                return scale * pseudoinverse @ error
+        # jacobian transpose
+        elif method == "transpose":
+            transpose = torch.transpose(jacobian_end_effector, 1, 2)
+            if squeeze_output:
+                return (scale * transpose @ error).squeeze(dim=2)
+            else:
+                return scale * transpose @ error
+        # damped least-squares
+        elif method == "damped least-squares":
+            damping = method_cfg.get("damping", 0.05)
+            transpose = torch.transpose(jacobian_end_effector, 1, 2)
+            lmbda = torch.eye(jacobian_end_effector.shape[1], device=jacobian_end_effector.device) * (damping ** 2)
+            if squeeze_output:
+                return (scale * transpose @ torch.inverse(jacobian_end_effector @ transpose + lmbda) @ error).squeeze(dim=2)
+            else:
+                return scale * transpose @ torch.inverse(jacobian_end_effector @ transpose + lmbda) @ error
         else:
-            return transpose @ torch.inverse(jacobian_end_effector @ transpose + lmbda) @ error
+            raise ValueError("Invalid IK method")
 
     # numpy
     # TODO: test and fix this
     else:
         # compute error
         q = _np_quat_mul(goal_orientation, _np_quat_conjugate(current_orientation))
         error = np.concatenate([goal_position - current_position,  # position error
                                 q[:, 0:3] * np.sign(q[:, 3])])  # orientation error
 
         # solve damped least squares (dO = J.T * V)
         transpose = np.transpose(jacobian_end_effector, 1, 2)
-        lmbda = np.eye(6) * (damping_factor ** 2)
+        lmbda = np.eye(6) * (method_cfg.get("damping", 0.05) ** 2)
         if squeeze_output:
             return (transpose @ np.linalg.inv(jacobian_end_effector @ transpose + lmbda) @ error)
         else:
             return transpose @ np.linalg.inv(jacobian_end_effector @ transpose + lmbda) @ error
 
-def get_env_instance(headless: bool = True, multi_threaded: bool = False) -> "omni.isaac.gym.vec_env.VecEnvBase":
+def get_env_instance(headless: bool = True,
+                     enable_livestream: bool = False,
+                     enable_viewport: bool = False,
+                     multi_threaded: bool = False) -> "omni.isaac.gym.vec_env.VecEnvBase":
     """
     Instantiate a VecEnvBase-based object compatible with OmniIsaacGymEnvs
 
     :param headless: Disable UI when running (default: ``True``)
     :type headless: bool, optional
+    :param enable_livestream: Whether to enable live streaming (default: ``False``)
+    :type enable_livestream: bool, optional
+    :param enable_viewport: Whether to enable viewport (default: ``False``)
+    :type enable_viewport: bool, optional
     :param multi_threaded: Whether to return a multi-threaded environment instance (default: ``False``)
     :type multi_threaded: bool, optional
 
     :return: Environment instance
     :rtype: omni.isaac.gym.vec_env.VecEnvBase
 
     Example::
@@ -138,15 +195,17 @@
         env = get_env_instance(headless=True)
 
         # parse sim configuration
         from omniisaacgymenvs.utils.config_utils.sim_config import SimConfig
         sim_config = SimConfig({"test": False,
                                 "device_id": 0,
                                 "headless": True,
+                                "multi_gpu": False,
                                 "sim_device": "gpu",
+                                "enable_livestream": False,
                                 "task": {"name": "CustomTask",
                                          "physics_engine": "physx",
                                          "env": {"numEnvs": 512,
                                                  "envSpacing": 1.5,
                                                  "enableDebugVis": False,
                                                  "clipObservations": 1000.0,
                                                  "clipActions": 1.0,
@@ -189,15 +248,15 @@
         from custom_task import CustomTask
         task = CustomTask(name="CustomTask", sim_config=sim_config, env=env)
         env.set_task(task=task, sim_params=sim_config.get_physics_params(), backend="torch", init_sim=True)
 
         # wrap the environment
         env = wrap_env(env, "omniverse-isaacgym")
     """
-    from omni.isaac.gym.vec_env import VecEnvBase, VecEnvMT, TaskStopException
+    from omni.isaac.gym.vec_env import TaskStopException, VecEnvBase, VecEnvMT
     from omni.isaac.gym.vec_env.vec_env_mt import TrainerMT
 
     class _OmniIsaacGymVecEnv(VecEnvBase):
         def step(self, actions):
             actions = torch.clamp(actions, -self._task.clip_actions, self._task.clip_actions).to(self._task.device).clone()
             self._task.pre_physics_step(actions)
 
@@ -219,16 +278,16 @@
         def run(self):
             pass
 
         def stop(self):
             pass
 
     class _OmniIsaacGymVecEnvMT(VecEnvMT):
-        def __init__(self, headless):
-            super().__init__(headless)
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
 
             self.action_queue = queue.Queue(1)
             self.data_queue = queue.Queue(1)
 
         def run(self, trainer=None):
             super().run(_OmniIsaacGymTrainerMT() if trainer is None else trainer)
 
@@ -256,10 +315,18 @@
 
         def close(self):
             # end stop signal to main thread
             self.send_actions(None)
             self.stop = True
 
     if multi_threaded:
-        return _OmniIsaacGymVecEnvMT(headless=headless)
+        try:
+            return _OmniIsaacGymVecEnvMT(headless=headless, enable_livestream=enable_livestream, enable_viewport=enable_viewport)
+        except TypeError:
+            logger.warning("Using an older version of Isaac Sim (2022.2.0 or earlier)")
+            return _OmniIsaacGymVecEnvMT(headless=headless)  # Isaac Sim 2022.2.0 and earlier
     else:
-        return _OmniIsaacGymVecEnv(headless=headless)
+        try:
+            return _OmniIsaacGymVecEnv(headless=headless, enable_livestream=enable_livestream, enable_viewport=enable_viewport)
+        except TypeError:
+            logger.warning("Using an older version of Isaac Sim (2022.2.0 or earlier)")
+            return _OmniIsaacGymVecEnv(headless=headless)  # Isaac Sim 2022.2.0 and earlier
```

### Comparing `skrl-0.9.1/skrl/utils/postprocessing.py` & `skrl-1.0.0rc1/skrl/utils/postprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Union, Tuple, List
+from typing import List, Tuple, Union
 
-import os
+import collections
 import csv
 import glob
-import numpy as np
+import os
 
+import numpy as np
 import torch
-import collections
 
 
 class MemoryFileIterator():
     def __init__(self, pathname: str) -> None:
         """Python iterator for loading data from exported memories
 
         The iterator will load the next memory file in the list of path names.
@@ -54,15 +54,15 @@
         if self.file_paths[self.n].endswith(".pt"):
             return self._format_torch()
         elif self.file_paths[self.n].endswith(".npz"):
             return self._format_numpy()
         elif self.file_paths[self.n].endswith(".csv"):
             return self._format_csv()
         else:
-            raise ValueError("Unsupported format: {}. Available formats: pt, csv, npz".format(format))
+            raise ValueError(f"Unsupported format for {self.file_paths[self.n]}. Available formats: .pt, .csv, .npz")
 
     def _format_numpy(self) -> Tuple[str, dict]:
         """Load numpy array from file
 
         :return: Tuple of file name and data
         :rtype: tuple
         """
```

### Comparing `skrl-0.9.1/skrl.egg-info/PKG-INFO` & `skrl-1.0.0rc1/skrl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 Metadata-Version: 2.1
 Name: skrl
-Version: 0.9.1
-Summary: Modular and flexible library for Reinforcement Learning
-Home-page: https://github.com/Toni-SM/skrl
+Version: 1.0.0rc1
+Summary: Modular and flexible library for reinforcement learning on PyTorch and JAX
 Author: Toni-SM
-License: MIT
+Maintainer: Toni-SM
+License: MIT License
+Project-URL: Homepage, https://github.com/Toni-SM/skrl
 Project-URL: Documentation, https://skrl.readthedocs.io
-Project-URL: Repository, https://github.com/Toni-SM/skrl
-Project-URL: Bug Tracker, https://github.com/Toni-SM/skrl/issues
 Project-URL: Discussions, https://github.com/Toni-SM/skrl/discussions
-Keywords: reinforcement,machine,learning,rl
+Project-URL: Bug Reports, https://github.com/Toni-SM/skrl/issues
+Project-URL: Say Thanks!, https://github.com/Toni-SM
+Project-URL: Source, https://github.com/Toni-SM/skrl
+Keywords: reinforcement-learning,machine-learning,reinforcement,machine,learning,rl
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6.*
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: torch
+Provides-Extra: jax
+Provides-Extra: all
 License-File: LICENSE
 
 [![pypi](https://img.shields.io/pypi/v/skrl)](https://pypi.org/project/skrl)
-[<img src="https://img.shields.io/badge/%F0%9F%A4%97%20Models-Huggingface-F8D521">](https://huggingface.co/skrl)
+[<img src="https://img.shields.io/badge/%F0%9F%A4%97%20models-hugging%20face-F8D521">](https://huggingface.co/skrl)
 ![discussions](https://img.shields.io/github/discussions/Toni-SM/skrl)
 <br>
 [![license](https://img.shields.io/github/license/Toni-SM/skrl)](https://github.com/Toni-SM/skrl)
 <span>&nbsp;&nbsp;&nbsp;&nbsp;</span>
 [![docs](https://readthedocs.org/projects/skrl/badge/?version=latest)](https://skrl.readthedocs.io/en/latest/?badge=latest)
 [![pytest](https://github.com/Toni-SM/skrl/actions/workflows/python-test.yml/badge.svg)](https://github.com/Toni-SM/skrl/actions/workflows/python-test.yml)
 [![pre-commit](https://github.com/Toni-SM/skrl/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/Toni-SM/skrl/actions/workflows/pre-commit.yml)
 
 <br>
 <p align="center">
-  <img width="300rem" src="https://raw.githubusercontent.com/Toni-SM/skrl/main/docs/source/_static/data/skrl-up-transparent.png">
+  <img width="300rem" src="https://raw.githubusercontent.com/Toni-SM/skrl/main/docs/source/_static/data/logo-light-mode.png">
 </p>
 <h2 align="center" style="border-bottom: 0 !important;">SKRL - Reinforcement Learning library</h2>
 <br>
 
-**skrl** is an open-source modular library for Reinforcement Learning written in Python (using [PyTorch](https://pytorch.org/)) and designed with a focus on readability, simplicity, and transparency of algorithm implementation. In addition to supporting the OpenAI [Gym](https://www.gymlibrary.dev) / Farama [Gymnasium](https://gymnasium.farama.org) and [DeepMind](https://github.com/deepmind/dm_env) environment interfaces, it allows loading and configuring [NVIDIA Isaac Gym](https://developer.nvidia.com/isaac-gym/) and [NVIDIA Omniverse Isaac Gym](https://docs.omniverse.nvidia.com/app_isaacsim/app_isaacsim/tutorial_gym_isaac_gym.html) environments, enabling agents' simultaneous training by scopes (subsets of environments among all available environments), which may or may not share resources, in the same run
+**skrl** is an open-source modular library for Reinforcement Learning written in Python (on top of [PyTorch](https://pytorch.org/) and [JAX](https://jax.readthedocs.io) and designed with a focus on modularity, readability, simplicity, and transparency of algorithm implementation. In addition to supporting the OpenAI [Gym](https://www.gymlibrary.dev) / Farama [Gymnasium](https://gymnasium.farama.org) and [DeepMind](https://github.com/deepmind/dm_env) and other environment interfaces, it allows loading and configuring [NVIDIA Isaac Gym](https://developer.nvidia.com/isaac-gym/), [NVIDIA Isaac Orbit](https://isaac-orbit.github.io/orbit/index.html) and [NVIDIA Omniverse Isaac Gym](https://docs.omniverse.nvidia.com/app_isaacsim/app_isaacsim/tutorial_gym_isaac_gym.html) environments, enabling agents' simultaneous training by scopes (subsets of environments among all available environments), which may or may not share resources, in the same run.
 
 <br>
 
 ### Please, visit the documentation for usage details and examples
 
 https://skrl.readthedocs.io/en/latest/
```

