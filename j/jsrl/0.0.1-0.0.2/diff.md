# Comparing `tmp/jsrl-0.0.1.tar.gz` & `tmp/jsrl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsrl-0.0.1.tar", last modified: Thu Jul 20 15:43:33 2023, max compression
+gzip compressed data, was "jsrl-0.0.2.tar", last modified: Tue Jul 25 17:50:59 2023, max compression
```

## Comparing `jsrl-0.0.1.tar` & `jsrl-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-07-20 15:43:33.176636 jsrl-0.0.1/
--rw-rw-r--   0 steven    (1000) steven    (1000)     1068 2023-07-12 20:19:00.000000 jsrl-0.0.1/LICENSE
--rw-rw-r--   0 steven    (1000) steven    (1000)     1939 2023-07-20 15:43:33.176636 jsrl-0.0.1/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)     1383 2023-07-20 15:31:17.000000 jsrl-0.0.1/README.md
--rw-rw-r--   0 steven    (1000) steven    (1000)      630 2023-07-20 15:42:47.000000 jsrl-0.0.1/pyproject.toml
--rw-rw-r--   0 steven    (1000) steven    (1000)       38 2023-07-20 15:43:33.176636 jsrl-0.0.1/setup.cfg
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-07-20 15:43:33.175636 jsrl-0.0.1/src/
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-07-20 15:43:33.175636 jsrl-0.0.1/src/jsrl/
--rw-rw-r--   0 steven    (1000) steven    (1000)        0 2023-07-20 15:39:10.000000 jsrl-0.0.1/src/jsrl/__init__.py
--rw-rw-r--   0 steven    (1000) steven    (1000)     9108 2023-07-20 15:26:11.000000 jsrl-0.0.1/src/jsrl/jsrl.py
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-07-20 15:43:33.175636 jsrl-0.0.1/src/jsrl.egg-info/
--rw-rw-r--   0 steven    (1000) steven    (1000)     1939 2023-07-20 15:43:33.000000 jsrl-0.0.1/src/jsrl.egg-info/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)      198 2023-07-20 15:43:33.000000 jsrl-0.0.1/src/jsrl.egg-info/SOURCES.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        1 2023-07-20 15:43:33.000000 jsrl-0.0.1/src/jsrl.egg-info/dependency_links.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        5 2023-07-20 15:43:33.000000 jsrl-0.0.1/src/jsrl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:50:59.191223 jsrl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 17:50:44.000000 jsrl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-25 17:50:59.191223 jsrl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 17:50:44.000000 jsrl-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-25 17:50:44.000000 jsrl-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:50:59.191223 jsrl-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:50:59.187223 jsrl-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:50:59.187223 jsrl-0.0.2/src/jsrl/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 17:50:44.000000 jsrl-0.0.2/src/jsrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-25 17:50:44.000000 jsrl-0.0.2/src/jsrl/jsrl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:50:59.191223 jsrl-0.0.2/src/jsrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 17:50:59.000000 jsrl-0.0.2/src/jsrl.egg-info/top_level.txt
```

### Comparing `jsrl-0.0.1/LICENSE` & `jsrl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsrl-0.0.1/PKG-INFO` & `jsrl-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: jsrl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implementation of Jump-Start Reinforcement Learning with Stable Baselines3.
 Author-email: Steven Tang <stang5@ualberta.ca>
 Project-URL: Homepage, https://github.com/steventango/jumpstart-rl
 Project-URL: Bug Tracker, https://github.com/steventango/jumpstart-rl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # Jump-start Reinforcement Learning
 
 Implementation of [Jump-Start Reinforcement Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3).
 
+## Installation
+
+```bash
+pip install jsrl
+```
+
 ## Usage
 
-See `examples/train_jsrl.py` for an example of how to train SAC + JSRL on the `PointMaze-v3` environment.
+See `examples/train_jsrl.py` for an example of how to train TD3 + JSRL on the `PointMaze-v3` environment.
 
 ## References
 
 ```bibtex
 @inproceedings{jsrl2022arxiv,
     title={Jump-Start Reinforcement Learning},
     author={Ikechukwu Uchendu, Ted Xiao, Yao Lu, Banghua Zhu, Mengyuan Yan, Joséphine Simon, Matthew Bennice, Chuyuan Fu, Cong Ma, Jiantao Jiao, Sergey Levine, and Karol Hausman},
```

### Comparing `jsrl-0.0.1/README.md` & `jsrl-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Jump-start Reinforcement Learning
 
 Implementation of [Jump-Start Reinforcement Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3).
 
+## Installation
+
+```bash
+pip install jsrl
+```
+
 ## Usage
 
-See `examples/train_jsrl.py` for an example of how to train SAC + JSRL on the `PointMaze-v3` environment.
+See `examples/train_jsrl.py` for an example of how to train TD3 + JSRL on the `PointMaze-v3` environment.
 
 ## References
 
 ```bibtex
 @inproceedings{jsrl2022arxiv,
     title={Jump-Start Reinforcement Learning},
     author={Ikechukwu Uchendu, Ted Xiao, Yao Lu, Banghua Zhu, Mengyuan Yan, Joséphine Simon, Matthew Bennice, Chuyuan Fu, Cong Ma, Jiantao Jiao, Sergey Levine, and Karol Hausman},
```

### Comparing `jsrl-0.0.1/pyproject.toml` & `jsrl-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsrl"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Steven Tang", email="stang5@ualberta.ca" },
 ]
 description = "Implementation of Jump-Start Reinforcement Learning with Stable Baselines3."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "stable-baselines3[extra]>=2.0.0"
+]
+
+[project.optional-dependencies]
+test = [
+    "gymnasium-robotics>=1.2.2"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/steventango/jumpstart-rl"
 "Bug Tracker" = "https://github.com/steventango/jumpstart-rl/issues"
```

### Comparing `jsrl-0.0.1/src/jsrl.egg-info/PKG-INFO` & `jsrl-0.0.2/src/jsrl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: jsrl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implementation of Jump-Start Reinforcement Learning with Stable Baselines3.
 Author-email: Steven Tang <stang5@ualberta.ca>
 Project-URL: Homepage, https://github.com/steventango/jumpstart-rl
 Project-URL: Bug Tracker, https://github.com/steventango/jumpstart-rl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # Jump-start Reinforcement Learning
 
 Implementation of [Jump-Start Reinforcement Learning](https://arxiv.org/abs/2204.02372) (JSRL) with [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3).
 
+## Installation
+
+```bash
+pip install jsrl
+```
+
 ## Usage
 
-See `examples/train_jsrl.py` for an example of how to train SAC + JSRL on the `PointMaze-v3` environment.
+See `examples/train_jsrl.py` for an example of how to train TD3 + JSRL on the `PointMaze-v3` environment.
 
 ## References
 
 ```bibtex
 @inproceedings{jsrl2022arxiv,
     title={Jump-Start Reinforcement Learning},
     author={Ikechukwu Uchendu, Ted Xiao, Yao Lu, Banghua Zhu, Mengyuan Yan, Joséphine Simon, Matthew Bennice, Chuyuan Fu, Cong Ma, Jiantao Jiao, Sergey Levine, and Karol Hausman},
```

