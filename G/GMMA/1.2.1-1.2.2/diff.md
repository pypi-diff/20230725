# Comparing `tmp/GMMA-1.2.1.tar.gz` & `tmp/GMMA-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GMMA-1.2.1.tar", last modified: Tue Jul 11 00:18:14 2023, max compression
+gzip compressed data, was "GMMA-1.2.2.tar", last modified: Tue Jul 25 18:43:31 2023, max compression
```

## Comparing `GMMA-1.2.1.tar` & `GMMA-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:18:14.759226 GMMA-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:18:14.755226 GMMA-1.2.1/GMMA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 00:18:14.000000 GMMA-1.2.1/GMMA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 00:18:04.000000 GMMA-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 00:18:14.759226 GMMA-1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:18:14.759226 GMMA-1.2.1/gamma/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    37223 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/_bayesian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    33646 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/_gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/seismic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-11 00:18:04.000000 GMMA-1.2.1/gamma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 00:18:14.759226 GMMA-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-11 00:18:04.000000 GMMA-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:18:14.759226 GMMA-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-11 00:18:05.000000 GMMA-1.2.1/tests/test_seismoc_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:43:31.124877 GMMA-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:43:31.124877 GMMA-1.2.2/GMMA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-25 18:43:31.000000 GMMA-1.2.2/GMMA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 18:43:31.000000 GMMA-1.2.2/GMMA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:43:31.000000 GMMA-1.2.2/GMMA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 18:43:31.000000 GMMA-1.2.2/GMMA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 18:43:31.000000 GMMA-1.2.2/GMMA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 18:43:21.000000 GMMA-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-25 18:43:31.124877 GMMA-1.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:43:31.124877 GMMA-1.2.2/gamma/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-25 18:43:21.000000 GMMA-1.2.2/gamma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-07-25 18:43:21.000000 GMMA-1.2.2/gamma/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37223 2023-07-25 18:43:21.000000 GMMA-1.2.2/gamma/_bayesian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33646 2023-07-25 18:43:21.000000 GMMA-1.2.2/gamma/_gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-25 18:43:21.000000 GMMA-1.2.2/gamma/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-07-25 18:43:21.000000 GMMA-1.2.2/gamma/seismic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-07-25 18:43:21.000000 GMMA-1.2.2/gamma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:43:31.124877 GMMA-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-25 18:43:21.000000 GMMA-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:43:31.124877 GMMA-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-25 18:43:21.000000 GMMA-1.2.2/tests/test_seismoc_ops.py
```

### Comparing `GMMA-1.2.1/LICENSE` & `GMMA-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.1/gamma/_base.py` & `GMMA-1.2.2/gamma/_base.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.1/gamma/_bayesian_mixture.py` & `GMMA-1.2.2/gamma/_bayesian_mixture.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.1/gamma/_gaussian_mixture.py` & `GMMA-1.2.2/gamma/_gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.1/gamma/app.py` & `GMMA-1.2.2/gamma/app.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.1/gamma/seismic_ops.py` & `GMMA-1.2.2/gamma/seismic_ops.py`

 * *Files identical despite different names*

### Comparing `GMMA-1.2.1/gamma/utils.py` & `GMMA-1.2.2/gamma/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,34 @@
 from collections import Counter
 from datetime import datetime
 import platform
 
 import numpy as np
 import pandas as pd
 from sklearn.cluster import DBSCAN
+from scipy.sparse.csgraph import minimum_spanning_tree
 
 from ._bayesian_mixture import BayesianGaussianMixture
 from ._gaussian_mixture import GaussianMixture
 from .seismic_ops import calc_amp, calc_time, initialize_eikonal
 
 to_seconds = lambda t: t.timestamp(tz="UTC")
 from_seconds = lambda t: pd.Timestamp.utcfromtimestamp(t).strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3]
 # to_seconds = lambda t: datetime.strptime(t, "%Y-%m-%dT%H:%M:%S.%f").timestamp()
 # from_seconds = lambda t: [datetime.utcfromtimestamp(x).strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] for x in t]
 
 
+def estimate_station_spacing(stations):
+    X = stations[["x(km)", "y(km)", "z(km)"]].values
+    D = np.sqrt(((X[:, np.newaxis, :] -  X[np.newaxis, :, :])**2).sum(axis=-1))
+    Tcsr = minimum_spanning_tree(D).toarray()
+    spacing = Tcsr[Tcsr > 0].mean() 
+    return spacing
+
+
 def convert_picks_csv(picks, stations, config):
     # t = picks["timestamp"].apply(lambda x: x.timestamp()).to_numpy()
     if type(picks["timestamp"].iloc[0]) is str:
         picks.loc[:, "timestamp"] = picks["timestamp"].apply(lambda x: datetime.fromisoformat(x))
     t = (
         picks["timestamp"]
         .apply(lambda x: x.tz_convert("UTC").timestamp() if x.tzinfo is not None else x.tz_localize("UTC").timestamp())
```

### Comparing `GMMA-1.2.1/tests/test_seismoc_ops.py` & `GMMA-1.2.2/tests/test_seismoc_ops.py`

 * *Files identical despite different names*

