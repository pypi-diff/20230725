# Comparing `tmp/jsrl-0.0.2.tar.gz` & `tmp/jsrl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsrl-0.0.2.tar", last modified: Tue Jul 25 17:50:59 2023, max compression
+gzip compressed data, was "jsrl-0.0.3.tar", last modified: Tue Jul 25 18:12:03 2023, max compression
```

## Comparing `jsrl-0.0.2.tar` & `jsrl-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:50:59.191223 jsrl-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 17:50:44.000000 jsrl-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-25 17:50:59.191223 jsrl-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 17:50:44.000000 jsrl-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-25 17:50:44.000000 jsrl-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:50:59.191223 jsrl-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:50:59.187223 jsrl-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:50:59.187223 jsrl-0.0.2/src/jsrl/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 17:50:44.000000 jsrl-0.0.2/src/jsrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-25 17:50:44.000000 jsrl-0.0.2/src/jsrl/jsrl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:50:59.191223 jsrl-0.0.2/src/jsrl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:12:03.208760 jsrl-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 18:11:47.000000 jsrl-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-25 18:12:03.208760 jsrl-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-25 18:11:47.000000 jsrl-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-25 18:11:47.000000 jsrl-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:12:03.208760 jsrl-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:12:03.204759 jsrl-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:12:03.204759 jsrl-0.0.3/src/jsrl/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 18:11:47.000000 jsrl-0.0.3/src/jsrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-25 18:11:47.000000 jsrl-0.0.3/src/jsrl/jsrl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:12:03.204759 jsrl-0.0.3/src/jsrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-25 18:12:03.000000 jsrl-0.0.3/src/jsrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-25 18:12:03.000000 jsrl-0.0.3/src/jsrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:12:03.000000 jsrl-0.0.3/src/jsrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 18:12:03.000000 jsrl-0.0.3/src/jsrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 18:12:03.000000 jsrl-0.0.3/src/jsrl.egg-info/top_level.txt
```

### Comparing `jsrl-0.0.2/LICENSE` & `jsrl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsrl-0.0.2/PKG-INFO` & `jsrl-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: jsrl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementation of Jump-Start Reinforcement Learning with Stable Baselines3.
 Author-email: Steven Tang <stang5@ualberta.ca>
 Project-URL: Homepage, https://github.com/steventango/jumpstart-rl
 Project-URL: Bug Tracker, https://github.com/steventango/jumpstart-rl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Jump-start Reinforcement Learning
 
-Implementation of [Jump-Start Reinforcement Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3).
+Implementation of [Jump-Start Reinforcement
+Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable
+Baselines3](https://github.com/DLR-RM/stable-baselines3).
 
 ## Installation
 
 ```bash
 pip install jsrl
 ```
 
 ## Usage
 
-See `examples/train_jsrl.py` for an example of how to train TD3 + JSRL on the `PointMaze-v3` environment.
+See `examples/train_jsrl_curriculum.py` or ``examples/train_jsrl_random.py`` for
+examples on how to train TD3 + JSRL on the `PointMaze-v3` environment.
 
 ## References
 
 ```bibtex
 @inproceedings{jsrl2022arxiv,
     title={Jump-Start Reinforcement Learning},
     author={Ikechukwu Uchendu, Ted Xiao, Yao Lu, Banghua Zhu, Mengyuan Yan, Joséphine Simon, Matthew Bennice, Chuyuan Fu, Cong Ma, Jiantao Jiao, Sergey Levine, and Karol Hausman},
```

### Comparing `jsrl-0.0.2/README.md` & `jsrl-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Jump-start Reinforcement Learning
 
-Implementation of [Jump-Start Reinforcement Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3).
+Implementation of [Jump-Start Reinforcement
+Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable
+Baselines3](https://github.com/DLR-RM/stable-baselines3).
 
 ## Installation
 
 ```bash
 pip install jsrl
 ```
 
 ## Usage
 
-See `examples/train_jsrl.py` for an example of how to train TD3 + JSRL on the `PointMaze-v3` environment.
+See `examples/train_jsrl_curriculum.py` or ``examples/train_jsrl_random.py`` for
+examples on how to train TD3 + JSRL on the `PointMaze-v3` environment.
 
 ## References
 
 ```bibtex
 @inproceedings{jsrl2022arxiv,
     title={Jump-Start Reinforcement Learning},
     author={Ikechukwu Uchendu, Ted Xiao, Yao Lu, Banghua Zhu, Mengyuan Yan, Joséphine Simon, Matthew Bennice, Chuyuan Fu, Cong Ma, Jiantao Jiao, Sergey Levine, and Karol Hausman},
```

### Comparing `jsrl-0.0.2/pyproject.toml` & `jsrl-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsrl"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Steven Tang", email="stang5@ualberta.ca" },
 ]
 description = "Implementation of Jump-Start Reinforcement Learning with Stable Baselines3."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jsrl-0.0.2/src/jsrl/jsrl.py` & `jsrl-0.0.3/src/jsrl/jsrl.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,23 @@
         self.logger = logger
         self.best_moving_mean_reward = -np.inf
         self.tolerated_moving_mean_reward = -np.inf
         self.mean_rewards = np.full(policy.window_size, -np.inf, dtype=np.float32)
 
     def _on_step(self) -> bool:
         self.policy.jsrl_evaluation = False
+        self.logger.record("jsrl/horizon", self.policy.horizon)
+
+        if self.policy.strategy == "random":
+            return True
+
         self.mean_rewards = np.roll(self.mean_rewards, 1)
         self.mean_rewards[0] = self.parent.last_mean_reward
         moving_mean_reward = np.mean(self.mean_rewards)
 
-        self.logger.record("jsrl/horizon", self.policy.horizon)
         self.logger.record("jsrl/moving_mean_reward", moving_mean_reward)
         self.logger.record("jsrl/best_moving_mean_reward", self.best_moving_mean_reward)
         self.logger.record("jsrl/tolerated_moving_mean_reward", self.tolerated_moving_mean_reward)
         self.logger.dump(self.num_timesteps)
 
         if self.mean_rewards[-1] == -np.inf or self.policy.horizon <= 0:
             return True
@@ -89,21 +93,26 @@
             eval_freq: int = 1000,
             n_eval_episodes: int = 20,
             **kwargs,
         ) -> None:
             super().__init__(*args, **kwargs)
             self.guide_policy = guide_policy
             self.tolerance = tolerance
+            assert strategy in ["curriculum", "random"], f"strategy: '{strategy}' must be 'curriculum' or 'random'"
             self.strategy = strategy
             self.horizon_step = 0
             self.max_horizon = max_horizon
             self.horizons = horizons
+            assert window_size > 0, f"window_size: {window_size} must be greater than 0"
             self.window_size = window_size
             self.eval_freq = eval_freq
-            self.n_eval_episodes = n_eval_episodes
+            if self.strategy == "curriculum":
+                self.n_eval_episodes = n_eval_episodes
+            else:
+                self.n_eval_episodes = 0
             self.jsrl_evaluation = False
 
         @property
         def horizon(self):
             return self.horizons[self.horizon_step]
 
         def predict(
@@ -178,17 +187,15 @@
             """
             Update the horizon based on the current strategy.
             """
             if self.strategy == "curriculum":
                 self.horizon_step += 1
                 self.horizon_step = min(self.horizon_step, len(self.horizons) - 1)
             elif self.strategy == "random":
-                self.horizon_step = np.random.choice(self.max_horizon)
-            else:
-                raise ValueError(f"Unknown strategy: {self.strategy}")
+                self.horizons = [np.random.choice(self.max_horizon)]
 
     return JSRLPolicy
 
 
 def get_jsrl_algorithm(Algorithm: BaseAlgorithm):
     class JSRLAlgorithm(Algorithm):
         def __init__(self, policy, *args, **kwargs):
@@ -252,10 +259,12 @@
             :return: the model's action and the next hidden state
                 (used in recurrent policies)
             """
             action, state = self.policy.predict(observation, self._timesteps, state, episode_start, deterministic)
 
             self._timesteps += 1
             self._timesteps[self.env.buf_dones] = 0
+            if self.policy.strategy == "random" and self.env.buf_dones.any():
+                self.policy.update_horizon()
             return action, state
 
     return JSRLAlgorithm
```

### Comparing `jsrl-0.0.2/src/jsrl.egg-info/PKG-INFO` & `jsrl-0.0.3/src/jsrl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: jsrl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementation of Jump-Start Reinforcement Learning with Stable Baselines3.
 Author-email: Steven Tang <stang5@ualberta.ca>
 Project-URL: Homepage, https://github.com/steventango/jumpstart-rl
 Project-URL: Bug Tracker, https://github.com/steventango/jumpstart-rl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Jump-start Reinforcement Learning
 
-Implementation of [Jump-Start Reinforcement Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3).
+Implementation of [Jump-Start Reinforcement
+Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable
+Baselines3](https://github.com/DLR-RM/stable-baselines3).
 
 ## Installation
 
 ```bash
 pip install jsrl
 ```
 
 ## Usage
 
-See `examples/train_jsrl.py` for an example of how to train TD3 + JSRL on the `PointMaze-v3` environment.
+See `examples/train_jsrl_curriculum.py` or ``examples/train_jsrl_random.py`` for
+examples on how to train TD3 + JSRL on the `PointMaze-v3` environment.
 
 ## References
 
 ```bibtex
 @inproceedings{jsrl2022arxiv,
     title={Jump-Start Reinforcement Learning},
     author={Ikechukwu Uchendu, Ted Xiao, Yao Lu, Banghua Zhu, Mengyuan Yan, Joséphine Simon, Matthew Bennice, Chuyuan Fu, Cong Ma, Jiantao Jiao, Sergey Levine, and Karol Hausman},
```

