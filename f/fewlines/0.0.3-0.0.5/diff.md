# Comparing `tmp/fewlines-0.0.3.tar.gz` & `tmp/fewlines-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fewlines-0.0.3.tar", last modified: Thu Jun 29 15:41:44 2023, max compression
+gzip compressed data, was "fewlines-0.0.5.tar", last modified: Tue Jul 25 01:28:54 2023, max compression
```

## Comparing `fewlines-0.0.3.tar` & `fewlines-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:41:44.529752 fewlines-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 15:41:32.000000 fewlines-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 15:41:44.529752 fewlines-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-29 15:41:32.000000 fewlines-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:41:44.529752 fewlines-0.0.3/fewlines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:41:32.000000 fewlines-0.0.3/fewlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-29 15:41:32.000000 fewlines-0.0.3/fewlines/horizon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:41:44.529752 fewlines-0.0.3/fewlines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 15:41:44.000000 fewlines-0.0.3/fewlines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 15:41:44.000000 fewlines-0.0.3/fewlines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:41:44.000000 fewlines-0.0.3/fewlines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 15:41:44.000000 fewlines-0.0.3/fewlines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:41:44.529752 fewlines-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-29 15:41:32.000000 fewlines-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:28:54.048626 fewlines-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-25 01:28:42.000000 fewlines-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 01:28:54.048626 fewlines-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-25 01:28:42.000000 fewlines-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:28:54.044626 fewlines-0.0.5/fewlines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:28:42.000000 fewlines-0.0.5/fewlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-25 01:28:42.000000 fewlines-0.0.5/fewlines/horizon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:28:54.044626 fewlines-0.0.5/fewlines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 01:28:54.000000 fewlines-0.0.5/fewlines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 01:28:54.000000 fewlines-0.0.5/fewlines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:28:54.000000 fewlines-0.0.5/fewlines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 01:28:54.000000 fewlines-0.0.5/fewlines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:28:54.048626 fewlines-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-25 01:28:42.000000 fewlines-0.0.5/setup.py
```

### Comparing `fewlines-0.0.3/LICENSE` & `fewlines-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fewlines-0.0.3/README.md` & `fewlines-0.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,44 @@
 
 Whether we like it or not, we debug things by putting print statements around.
 
 `fewlines` is a supplement for this, allowing to plot charts which only take few lines in a terminal output, but can be a very useful piece of information.
 
 Example use-case could be plotting distribution of weights, gradients and activations for layers in NN.
 
-TODO: insert screenshots here.
+![self-attention weights](static/fewlines_self_attention.png)
 
 While created originally to plot distributions of weights/gradients it can be also used to visualize time series and
 is not restricted to ML use cases, obviously. Can be used to show latency distribution, for example.
 
 Installation:
 ```
 pip install fewlines
 ```
 
-TODO: Examples here
+## Usage examples
 
-## TODO
+Minimal example:
+```
+from fewlines.horizon import horizon_line
+print(horizon_line([i for i in range(100)]))
+```
+
+![minimal](static/fewlines_minimal.png)
+
+Print distribution with default formatting:
+```
+from fewlines.horizon import print_histogram
+import numpy as np
+print_histogram(np.random.normal(size=10000))
+```
+
+![histogram](static/fewlines_hist.png)
 
+
+## TODO
+* more examples, including Colab
+* move torch-specific printing to separate module
 * unit tests
-* examples
 * scatter-like chart
-* negative values support
+* negative values support
+* shared y scale
```

