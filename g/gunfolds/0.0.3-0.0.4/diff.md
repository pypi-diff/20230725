# Comparing `tmp/gunfolds-0.0.3.tar.gz` & `tmp/gunfolds-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunfolds-0.0.3.tar", last modified: Thu Jul 20 02:56:44 2023, max compression
+gzip compressed data, was "gunfolds-0.0.4.tar", last modified: Tue Jul 25 04:47:07 2023, max compression
```

## Comparing `gunfolds-0.0.3.tar` & `gunfolds-0.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.200742 gunfolds-0.0.3/
--rw-r--r--   0 gm         (501) staff       (20)    35121 2023-07-20 02:54:22.000000 gunfolds-0.0.3/LICENSE
--rw-r--r--   0 gm         (501) staff       (20)       50 2023-07-20 02:54:22.000000 gunfolds-0.0.3/MANIFEST.in
--rw-r--r--   0 gm         (501) staff       (20)     2020 2023-07-20 02:56:44.200547 gunfolds-0.0.3/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)     1734 2023-07-20 02:54:22.000000 gunfolds-0.0.3/README.md
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.178973 gunfolds-0.0.3/gunfolds/
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)    23311 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/conversions.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.192572 gunfolds-0.0.3/gunfolds/data/
--rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/data/allloops.zkl
--rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/data/circular_p.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3987 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/data/colors.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3691 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/data/testgraphs.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.194501 gunfolds-0.0.3/gunfolds/estimation/
--rw-r--r--   0 gm         (501) staff       (20)        0 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/estimation/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)     2676 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/estimation/grangercausality.py
--rw-r--r--   0 gm         (501) staff       (20)    25419 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/estimation/linear_model.py
--rw-r--r--   0 gm         (501) staff       (20)     5904 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/estimation/pc.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.194960 gunfolds-0.0.3/gunfolds/figures/
--rw-r--r--   0 gm         (501) staff       (20)     2976 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/figures/shipfig.tex
--rw-r--r--   0 gm         (501) staff       (20)     1412 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/figures/shippage.sty
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.196354 gunfolds-0.0.3/gunfolds/solvers/
--rw-r--r--   0 gm         (501) staff       (20)        0 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/solvers/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)     4156 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/solvers/clingo_msl.py
--rw-r--r--   0 gm         (501) staff       (20)    15841 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/solvers/clingo_rasl.py
--rw-r--r--   0 gm         (501) staff       (20)    43259 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/solvers/traversal.py
--rw-r--r--   0 gm         (501) staff       (20)    18670 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/solvers/unknownrate.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.198939 gunfolds-0.0.3/gunfolds/utils/
--rw-r--r--   0 gm         (501) staff       (20)      816 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)    15415 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/bfutils.py
--rw-r--r--   0 gm         (501) staff       (20)     1130 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/calc_procs.py
--rw-r--r--   0 gm         (501) staff       (20)     3188 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/clingo.py
--rw-r--r--   0 gm         (501) staff       (20)     3684 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/comparison.py
--rw-r--r--   0 gm         (501) staff       (20)     4344 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/ecj.py
--rw-r--r--   0 gm         (501) staff       (20)    31572 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/graphkit.py
--rw-r--r--   0 gm         (501) staff       (20)     2332 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/myTimeout.py
--rw-r--r--   0 gm         (501) staff       (20)     3368 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/neighborhoods.py
--rw-r--r--   0 gm         (501) staff       (20)      864 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/simpleloops.py
--rw-r--r--   0 gm         (501) staff       (20)     1235 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/utils/zickle.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.199584 gunfolds-0.0.3/gunfolds/viz/
--rw-r--r--   0 gm         (501) staff       (20)        0 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/viz/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)    20874 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/viz/dbn2latex.py
--rw-r--r--   0 gm         (501) staff       (20)    10784 2023-07-20 02:54:22.000000 gunfolds-0.0.3/gunfolds/viz/gtool.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.180367 gunfolds-0.0.3/gunfolds.egg-info/
--rw-r--r--   0 gm         (501) staff       (20)     2020 2023-07-20 02:56:44.000000 gunfolds-0.0.3/gunfolds.egg-info/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)     1135 2023-07-20 02:56:44.000000 gunfolds-0.0.3/gunfolds.egg-info/SOURCES.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-07-20 02:56:44.000000 gunfolds-0.0.3/gunfolds.egg-info/dependency_links.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-07-20 02:56:44.000000 gunfolds-0.0.3/gunfolds.egg-info/not-zip-safe
--rw-r--r--   0 gm         (501) staff       (20)       95 2023-07-20 02:56:44.000000 gunfolds-0.0.3/gunfolds.egg-info/requires.txt
--rw-r--r--   0 gm         (501) staff       (20)       15 2023-07-20 02:56:44.000000 gunfolds-0.0.3/gunfolds.egg-info/top_level.txt
--rw-r--r--   0 gm         (501) staff       (20)       38 2023-07-20 02:56:44.200810 gunfolds-0.0.3/setup.cfg
--rw-r--r--   0 gm         (501) staff       (20)     1223 2023-07-20 02:54:22.000000 gunfolds-0.0.3/setup.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-20 02:56:44.199976 gunfolds-0.0.3/tests/
--rw-r--r--   0 gm         (501) staff       (20)        0 2023-07-20 02:54:22.000000 gunfolds-0.0.3/tests/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)    20222 2023-07-20 02:54:22.000000 gunfolds-0.0.3/tests/tests.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.301102 gunfolds-0.0.4/
+-rw-r--r--   0 gm         (501) staff       (20)    35121 2023-07-25 04:46:09.000000 gunfolds-0.0.4/LICENSE
+-rw-r--r--   0 gm         (501) staff       (20)       50 2023-07-25 04:46:09.000000 gunfolds-0.0.4/MANIFEST.in
+-rw-r--r--   0 gm         (501) staff       (20)     2020 2023-07-25 04:47:07.300903 gunfolds-0.0.4/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)     1734 2023-07-25 04:46:09.000000 gunfolds-0.0.4/README.md
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.265356 gunfolds-0.0.4/gunfolds/
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    23425 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/conversions.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.292970 gunfolds-0.0.4/gunfolds/data/
+-rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/data/allloops.zkl
+-rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/data/circular_p.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3987 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/data/colors.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3691 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/data/testgraphs.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.294702 gunfolds-0.0.4/gunfolds/estimation/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/estimation/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)     2676 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/estimation/grangercausality.py
+-rw-r--r--   0 gm         (501) staff       (20)    25419 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/estimation/linear_model.py
+-rw-r--r--   0 gm         (501) staff       (20)     5904 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/estimation/pc.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.295128 gunfolds-0.0.4/gunfolds/figures/
+-rw-r--r--   0 gm         (501) staff       (20)     2976 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/figures/shipfig.tex
+-rw-r--r--   0 gm         (501) staff       (20)     1412 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/figures/shippage.sty
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.296499 gunfolds-0.0.4/gunfolds/solvers/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/solvers/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)     4156 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/solvers/clingo_msl.py
+-rw-r--r--   0 gm         (501) staff       (20)    16216 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/solvers/clingo_rasl.py
+-rw-r--r--   0 gm         (501) staff       (20)    43259 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/solvers/traversal.py
+-rw-r--r--   0 gm         (501) staff       (20)    18670 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/solvers/unknownrate.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.299389 gunfolds-0.0.4/gunfolds/utils/
+-rw-r--r--   0 gm         (501) staff       (20)      816 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    15415 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/bfutils.py
+-rw-r--r--   0 gm         (501) staff       (20)     1130 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/calc_procs.py
+-rw-r--r--   0 gm         (501) staff       (20)     3188 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/clingo.py
+-rw-r--r--   0 gm         (501) staff       (20)     3684 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/comparison.py
+-rw-r--r--   0 gm         (501) staff       (20)     4344 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/ecj.py
+-rw-r--r--   0 gm         (501) staff       (20)    31572 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/graphkit.py
+-rw-r--r--   0 gm         (501) staff       (20)     2332 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/myTimeout.py
+-rw-r--r--   0 gm         (501) staff       (20)     3368 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/neighborhoods.py
+-rw-r--r--   0 gm         (501) staff       (20)      864 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/simpleloops.py
+-rw-r--r--   0 gm         (501) staff       (20)     1235 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/utils/zickle.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.300016 gunfolds-0.0.4/gunfolds/viz/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/viz/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    20874 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/viz/dbn2latex.py
+-rw-r--r--   0 gm         (501) staff       (20)    10784 2023-07-25 04:46:09.000000 gunfolds-0.0.4/gunfolds/viz/gtool.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.266525 gunfolds-0.0.4/gunfolds.egg-info/
+-rw-r--r--   0 gm         (501) staff       (20)     2020 2023-07-25 04:47:07.000000 gunfolds-0.0.4/gunfolds.egg-info/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)     1135 2023-07-25 04:47:07.000000 gunfolds-0.0.4/gunfolds.egg-info/SOURCES.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-07-25 04:47:07.000000 gunfolds-0.0.4/gunfolds.egg-info/dependency_links.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-07-25 04:47:07.000000 gunfolds-0.0.4/gunfolds.egg-info/not-zip-safe
+-rw-r--r--   0 gm         (501) staff       (20)       95 2023-07-25 04:47:07.000000 gunfolds-0.0.4/gunfolds.egg-info/requires.txt
+-rw-r--r--   0 gm         (501) staff       (20)       15 2023-07-25 04:47:07.000000 gunfolds-0.0.4/gunfolds.egg-info/top_level.txt
+-rw-r--r--   0 gm         (501) staff       (20)       38 2023-07-25 04:47:07.301164 gunfolds-0.0.4/setup.cfg
+-rw-r--r--   0 gm         (501) staff       (20)     1223 2023-07-25 04:46:09.000000 gunfolds-0.0.4/setup.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-07-25 04:47:07.300377 gunfolds-0.0.4/tests/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-07-25 04:46:09.000000 gunfolds-0.0.4/tests/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    20222 2023-07-25 04:46:09.000000 gunfolds-0.0.4/tests/tests.py
```

### Comparing `gunfolds-0.0.3/LICENSE` & `gunfolds-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/PKG-INFO` & `gunfolds-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.0.3/README.md` & `gunfolds-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/conversions.py` & `gunfolds-0.0.4/gunfolds/conversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,18 +497,22 @@
     :type bidirected: string
     
     :returns: ``clingo`` predicate
     :rtype: string  
     """
     s = ''
     n = len(g)
+
     if directed_weights_matrix is None:
-        directed_weights_matrix = np.ones((n, n)).astype('int')
+        directed_weights_matrix = np.ones((n, n))
+    directed_weights_matrix = directed_weights_matrix.astype('int')
+
     if bidirected_weights_matrix is None:
-        bidirected_weights_matrix = np.ones((n, n)).astype('int')
+        bidirected_weights_matrix = np.ones((n, n))
+    bidirected_weights_matrix = bidirected_weights_matrix.astype('int')
 
     assert directed_weights_matrix.shape[0] == n
     assert directed_weights_matrix.shape[1] == n
     assert bidirected_weights_matrix.shape[0] == n
     assert bidirected_weights_matrix.shape[1] == n
 
     for v in range(1, n+1):
```

### Comparing `gunfolds-0.0.3/gunfolds/data/allloops.zkl` & `gunfolds-0.0.4/gunfolds/data/allloops.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/data/circular_p.zkl` & `gunfolds-0.0.4/gunfolds/data/circular_p.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/data/colors.zkl` & `gunfolds-0.0.4/gunfolds/data/colors.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/data/testgraphs.py` & `gunfolds-0.0.4/gunfolds/data/testgraphs.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/estimation/grangercausality.py` & `gunfolds-0.0.4/gunfolds/estimation/grangercausality.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/estimation/linear_model.py` & `gunfolds-0.0.4/gunfolds/estimation/linear_model.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/estimation/pc.py` & `gunfolds-0.0.4/gunfolds/estimation/pc.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/figures/shipfig.tex` & `gunfolds-0.0.4/gunfolds/figures/shipfig.tex`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/figures/shippage.sty` & `gunfolds-0.0.4/gunfolds/figures/shippage.sty`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/solvers/clingo_msl.py` & `gunfolds-0.0.4/gunfolds/solvers/clingo_msl.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/solvers/clingo_rasl.py` & `gunfolds-0.0.4/gunfolds/solvers/clingo_rasl.py`

 * *Files 6% similar despite different names*

```diff
@@ -229,16 +229,20 @@
     :type bdm: list of numpy arrays
 
     :returns: ``clingo`` predicates as a string
     :rtype: string
     """
     if dm is None:
         dm = [None]*len(g_list)
+    else:
+        dm = [nd.astype('int') for nd in dm]
     if bdm is None:
         bdm = [None]*len(g_list)
+    else:
+        bdm = [nd.astype('int') for nd in bdm]
     s = ''
     for count, (g, D, B) in enumerate(zip(g_list, dm, bdm)):
         if weighted:
             s += numbered_g2wclingo(g, count+1, directed_weights_matrix=D, bidirected_weights_matrix=B) + ' '
         else:
             s += numbered_g2clingo(g, count+1) + ' '
     return s
@@ -261,15 +265,15 @@
     :type weighted: boolean
 
     :param scc: whether to assume that each SCC in the input graph is
         either a singleton or have ``gcd=1``.  If `True` a much more
         efficient algorithm is employed.
     :type scc: (GUESS)boolean
 
-    :param scc_members: a list of dictionaries for nodes in each SCC
+    :param scc_members: a list of sets for nodes in each SCC
     :type scc_members: list
 
     :param dm: a list of n-by-n 2-d square matrix of the weights for
         directed edges of each input n-node graph
     :type dm: list of numpy arrays
 
     :param bdm: a list of *symmetric* n-by-n 2-d square matrix of the
@@ -279,14 +283,19 @@
     :param edge_weights: a tuple of 2 values, the first is importance of matching
         directed weights when solving optimization problem and the second is for bidirected.
     :type edge_weights: tuple with 2 elements
 
     :returns: clingo code as a string
     :rtype: string
     """
+    if dm is not None:
+        dm = [nd.astype('int') for nd in dm]
+    if bdm is not None:
+        bdm = [nd.astype('int') for nd in bdm]
+
     assert len({len(g) for g in g_list}) == 1, "Input graphs have variable number of nodes!"
 
     if not max_urate:
         max_urate = 1+3*len(g_list[0])
     n = len(g_list)
     command = clingo_preamble(g_list[0])
     if scc:
@@ -331,15 +340,15 @@
     :type weighted: boolean
 
     :param scc: whether to assume that each SCC in the input graph is
         either a singleton or have ``gcd=1``.  If ``True`` a much more
         efficient algorithm is employed.
     :type scc: boolean
 
-    :param scc_members: a list of dictionaries for nodes in each SCC
+    :param scc_members: a list of sets for nodes in each SCC
     :type scc_members: list
 
     :param dm: a list of n-by-n 2-d square matrix of the weights for
         directed edges of each input n-node graph
     :type dm: list of numpy arrays
 
     :param bdm: a list of *symmetric* n-by-n 2-d square matrix of the
@@ -352,14 +361,18 @@
     :param edge_weights: a tuple of 2 values, the first is importance
         of matching directed weights when solving optimization problem and the second is for bidirected.
     :type edge_weights: tuple with 2 elements
 
     :returns: results of parsed equivalent class
     :rtype: dictionary
     """
+    if dm is not None:
+        dm = [nd.astype('int') for nd in dm]
+    if bdm is not None:
+        bdm = [nd.astype('int') for nd in bdm]
     if not isinstance(glist, list):
         glist = [glist]
     return clingo(drasl_command(glist, max_urate=urate, weighted=weighted,
                                 scc=scc, scc_members=scc_members, dm=dm, bdm=bdm, edge_weights=edge_weights),
                   capsize=capsize, convert=drasl_jclingo2g,
                   timeout=timeout, exact=not weighted, pnum=pnum)
```

### Comparing `gunfolds-0.0.3/gunfolds/solvers/traversal.py` & `gunfolds-0.0.4/gunfolds/solvers/traversal.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/solvers/unknownrate.py` & `gunfolds-0.0.4/gunfolds/solvers/unknownrate.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/__init__.py` & `gunfolds-0.0.4/gunfolds/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/bfutils.py` & `gunfolds-0.0.4/gunfolds/utils/bfutils.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/calc_procs.py` & `gunfolds-0.0.4/gunfolds/utils/calc_procs.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/clingo.py` & `gunfolds-0.0.4/gunfolds/utils/clingo.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/comparison.py` & `gunfolds-0.0.4/gunfolds/utils/comparison.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/ecj.py` & `gunfolds-0.0.4/gunfolds/utils/ecj.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/graphkit.py` & `gunfolds-0.0.4/gunfolds/utils/graphkit.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/myTimeout.py` & `gunfolds-0.0.4/gunfolds/utils/myTimeout.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/neighborhoods.py` & `gunfolds-0.0.4/gunfolds/utils/neighborhoods.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/simpleloops.py` & `gunfolds-0.0.4/gunfolds/utils/simpleloops.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/utils/zickle.py` & `gunfolds-0.0.4/gunfolds/utils/zickle.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/viz/dbn2latex.py` & `gunfolds-0.0.4/gunfolds/viz/dbn2latex.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds/viz/gtool.py` & `gunfolds-0.0.4/gunfolds/viz/gtool.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/gunfolds.egg-info/PKG-INFO` & `gunfolds-0.0.4/gunfolds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.0.3/gunfolds.egg-info/SOURCES.txt` & `gunfolds-0.0.4/gunfolds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/setup.py` & `gunfolds-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.0.3/tests/tests.py` & `gunfolds-0.0.4/tests/tests.py`

 * *Files identical despite different names*

