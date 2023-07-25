# Comparing `tmp/protes-0.3.2.tar.gz` & `tmp/protes-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protes-0.3.2.tar", last modified: Tue Jun 13 07:29:16 2023, max compression
+gzip compressed data, was "protes-0.3.3.tar", last modified: Tue Jul 25 14:48:31 2023, max compression
```

## Comparing `protes-0.3.2.tar` & `protes-0.3.3.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.512707 protes-0.3.2/
--rw-r--r--   0 andrei     (501) staff       (20)       88 2023-05-11 08:52:02.000000 protes-0.3.2/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     8287 2023-06-13 07:29:16.511937 protes-0.3.2/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     7049 2023-06-13 07:20:22.000000 protes-0.3.2/README.md
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.475800 protes-0.3.2/calc/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-06-06 07:29:34.000000 protes-0.3.2/calc/.DS_Store
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.476890 protes-0.3.2/calc/__pycache__/
--rw-r--r--   0 andrei     (501) staff       (20)     1941 2023-05-17 14:35:24.000000 protes-0.3.2/calc/__pycache__/constr.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)    23864 2023-05-17 14:35:24.000000 protes-0.3.2/calc/__pycache__/construct_TT.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     7201 2023-05-17 19:07:28.000000 protes-0.3.2/calc/calc.py
--rw-r--r--   0 andrei     (501) staff       (20)     1716 2023-05-18 13:39:57.000000 protes-0.3.2/calc/calc_one.py
--rw-r--r--   0 andrei     (501) staff       (20)     1429 2023-05-16 21:18:20.000000 protes-0.3.2/calc/constr.py
--rw-r--r--   0 andrei     (501) staff       (20)    25285 2023-05-15 20:02:07.000000 protes-0.3.2/calc/construct_TT.py
--rw-r--r--   0 andrei     (501) staff       (20)   212397 2023-05-17 19:07:32.000000 protes-0.3.2/calc/deps.png
--rw-r--r--   0 andrei     (501) staff       (20)    23388 2023-06-13 07:28:05.000000 protes-0.3.2/calc/log.txt
--rw-r--r--   0 andrei     (501) staff       (20)     6927 2023-05-18 17:49:24.000000 protes-0.3.2/calc/log_one.txt
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.482651 protes-0.3.2/calc/opti/
--rw-r--r--   0 andrei     (501) staff       (20)      295 2023-05-14 21:16:31.000000 protes-0.3.2/calc/opti/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.488639 protes-0.3.2/calc/opti/__pycache__/
--rw-r--r--   0 andrei     (501) staff       (20)      527 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     3929 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)      999 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_nb.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_opo.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1378 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1039 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1476 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_protes.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)      997 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_pso.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:25.000000 protes-0.3.2/calc/opti/__pycache__/opti_spsa.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1478 2023-05-17 14:35:25.000000 protes-0.3.2/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     3667 2023-05-15 17:29:36.000000 protes-0.3.2/calc/opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      452 2023-05-14 21:10:44.000000 protes-0.3.2/calc/opti/opti_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      453 2023-05-14 21:10:36.000000 protes-0.3.2/calc/opti/opti_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)      763 2023-05-16 22:11:55.000000 protes-0.3.2/calc/opti/opti_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)      464 2023-05-14 21:10:27.000000 protes-0.3.2/calc/opti/opti_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)      923 2023-05-17 14:32:54.000000 protes-0.3.2/calc/opti/opti_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)      446 2023-05-14 21:10:16.000000 protes-0.3.2/calc/opti/opti_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)      449 2023-05-14 21:09:27.000000 protes-0.3.2/calc/opti/opti_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1042 2023-05-16 22:11:42.000000 protes-0.3.2/calc/opti/opti_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)    42609 2023-06-13 07:28:09.000000 protes-0.3.2/calc/res.pickle
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.499536 protes-0.3.2/demo/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:44.000000 protes-0.3.2/demo/.DS_Store
--rw-r--r--   0 andrei     (501) staff       (20)   342526 2023-05-18 12:20:34.000000 protes-0.3.2/demo/check_ackley.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)   536657 2023-05-18 11:46:30.000000 protes-0.3.2/demo/check_knapsack.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     2206 2023-05-18 13:10:28.000000 protes-0.3.2/demo/demo_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     2591 2023-05-18 13:15:03.000000 protes-0.3.2/demo/demo_qubo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.505361 protes-0.3.2/demo/figures/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:49.000000 protes-0.3.2/demo/figures/.DS_Store
--rw-r--r--   0 andrei     (501) staff       (20)   137856 2023-05-18 12:01:07.000000 protes-0.3.2/demo/figures/check_ackley.png
--rw-r--r--   0 andrei     (501) staff       (20)    99993 2023-05-18 12:20:12.000000 protes-0.3.2/demo/figures/check_ackley_ext.png
--rw-r--r--   0 andrei     (501) staff       (20)   202943 2023-05-17 15:13:23.000000 protes-0.3.2/demo/figures/check_knapsack.png
--rw-r--r--   0 andrei     (501) staff       (20)   180807 2023-05-18 11:44:44.000000 protes-0.3.2/demo/figures/check_knapsack_ext.png
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.508723 protes-0.3.2/protes/
--rw-r--r--   0 andrei     (501) staff       (20)      127 2023-06-13 07:28:41.000000 protes-0.3.2/protes/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4670 2023-05-18 16:29:00.000000 protes-0.3.2/protes/animation.py
--rw-r--r--   0 andrei     (501) staff       (20)     5895 2023-05-18 13:02:30.000000 protes-0.3.2/protes/protes.py
--rw-r--r--   0 andrei     (501) staff       (20)     5369 2023-05-18 13:02:40.000000 protes-0.3.2/protes/protes_general.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.511223 protes-0.3.2/protes.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     8287 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1445 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       98 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)        7 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/top_level.txt
--rw-r--r--   0 andrei     (501) staff       (20)       38 2023-06-13 07:29:16.512827 protes-0.3.2/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2467 2023-05-19 10:43:02.000000 protes-0.3.2/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.910621 protes-0.3.3/
+-rw-r--r--   0 andrei     (501) staff       (20)      118 2023-07-25 11:52:11.000000 protes-0.3.3/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     9793 2023-07-25 14:48:31.909955 protes-0.3.3/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     8555 2023-07-25 14:48:12.000000 protes-0.3.3/README.md
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.879732 protes-0.3.3/calc/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-07-14 14:53:51.000000 protes-0.3.3/calc/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)     7201 2023-05-17 19:07:28.000000 protes-0.3.3/calc/calc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1716 2023-07-25 13:56:59.000000 protes-0.3.3/calc/calc_one.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1429 2023-05-16 21:18:20.000000 protes-0.3.3/calc/constr.py
+-rw-r--r--   0 andrei     (501) staff       (20)    25285 2023-05-15 20:02:07.000000 protes-0.3.3/calc/construct_TT.py
+-rw-r--r--   0 andrei     (501) staff       (20)   212397 2023-05-17 19:07:32.000000 protes-0.3.3/calc/deps.png
+-rw-r--r--   0 andrei     (501) staff       (20)    23388 2023-06-13 07:47:54.000000 protes-0.3.3/calc/log.txt
+-rw-r--r--   0 andrei     (501) staff       (20)     6927 2023-07-25 13:56:59.000000 protes-0.3.3/calc/log_one.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.886166 protes-0.3.3/calc/opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      295 2023-05-14 21:16:31.000000 protes-0.3.3/calc/opti/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.891141 protes-0.3.3/calc/opti/__pycache__/
+-rw-r--r--   0 andrei     (501) staff       (20)      527 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     3929 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)      999 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_nb.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_opo.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1378 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1039 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1476 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_protes.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)      997 2023-05-17 14:35:24.000000 protes-0.3.3/calc/opti/__pycache__/opti_pso.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:25.000000 protes-0.3.3/calc/opti/__pycache__/opti_spsa.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1478 2023-05-17 14:35:25.000000 protes-0.3.3/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     3667 2023-05-15 17:29:36.000000 protes-0.3.3/calc/opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      452 2023-05-14 21:10:44.000000 protes-0.3.3/calc/opti/opti_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      453 2023-05-14 21:10:36.000000 protes-0.3.3/calc/opti/opti_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      763 2023-05-16 22:11:55.000000 protes-0.3.3/calc/opti/opti_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)      464 2023-05-14 21:10:27.000000 protes-0.3.3/calc/opti/opti_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)      923 2023-05-17 14:32:54.000000 protes-0.3.3/calc/opti/opti_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)      446 2023-05-14 21:10:16.000000 protes-0.3.3/calc/opti/opti_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)      449 2023-05-14 21:09:27.000000 protes-0.3.3/calc/opti/opti_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1042 2023-05-16 22:11:42.000000 protes-0.3.3/calc/opti/opti_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)    42609 2023-06-13 07:47:54.000000 protes-0.3.3/calc/res.pickle
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.898066 protes-0.3.3/demo/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:44.000000 protes-0.3.3/demo/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)   342526 2023-05-18 12:20:34.000000 protes-0.3.3/demo/check_ackley.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)   536657 2023-05-18 11:46:30.000000 protes-0.3.3/demo/check_knapsack.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     2512 2023-07-25 14:47:04.000000 protes-0.3.3/demo/demo_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2738 2023-07-25 14:47:29.000000 protes-0.3.3/demo/demo_qubo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.903964 protes-0.3.3/demo/figures/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:49.000000 protes-0.3.3/demo/figures/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)   137856 2023-05-18 12:01:07.000000 protes-0.3.3/demo/figures/check_ackley.png
+-rw-r--r--   0 andrei     (501) staff       (20)    99993 2023-05-18 12:20:12.000000 protes-0.3.3/demo/figures/check_ackley_ext.png
+-rw-r--r--   0 andrei     (501) staff       (20)   202943 2023-05-17 15:13:23.000000 protes-0.3.3/demo/figures/check_knapsack.png
+-rw-r--r--   0 andrei     (501) staff       (20)   180807 2023-05-18 11:44:44.000000 protes-0.3.3/demo/figures/check_knapsack_ext.png
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.907246 protes-0.3.3/protes/
+-rw-r--r--   0 andrei     (501) staff       (20)      127 2023-07-25 14:48:06.000000 protes-0.3.3/protes/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4670 2023-05-18 16:29:00.000000 protes-0.3.3/protes/animation.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5962 2023-07-25 14:29:04.000000 protes-0.3.3/protes/protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5450 2023-07-25 14:29:03.000000 protes-0.3.3/protes/protes_general.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 14:48:31.909246 protes-0.3.3/protes.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     9793 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1400 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      189 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        7 2023-07-25 14:48:31.000000 protes-0.3.3/protes.egg-info/top_level.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      243 2023-07-25 13:10:12.000000 protes-0.3.3/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      118 2023-05-15 20:03:14.000000 protes-0.3.3/requirements_calc.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       38 2023-07-25 14:48:31.910780 protes-0.3.3/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2467 2023-05-19 10:43:02.000000 protes-0.3.3/setup.py
```

### Comparing `protes-0.3.2/PKG-INFO` & `protes-0.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protes
-Version: 0.3.2
+Version: 0.3.3
 Summary: Method PROTES (PRobability Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
 Home-page: https://github.com/anabatsh/PROTES
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/anabatsh/PROTES
 Keywords: Derivative-free optimization multidimensional optimization low-rank representation tensor train format
 Classifier: Development Status :: 4 - Beta
@@ -28,83 +28,88 @@
 ## Description
 
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-To use this package, please install manually first the [python](https://www.python.org) programming language of the version >= 3.8, then, the package can be installed via pip: `pip install protes`.
+> Current version "0.3.3".
 
-> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product. To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
+To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip: `pip install protes`.
 
-To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt`.
+> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.4+), [scipy](https://github.com/scipy/scipy) (1.9+) and [seaborn](https://seaborn.pydata.org/) (0.12.2+) will be automatically installed during the installation of the main software product (see `requirements.txt` for more details). To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
+
+To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt` (please, note that the versions specified in this file are only suitable for `python 3.8`).
 
 
 ## Usage
 
-Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary array element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
+Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary tensor element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
 
 ```python
 import jax.numpy as jnp
 from protes import protes
 f_batch = lambda I: jnp.sum(I, axis=1)
 i_opt, y_opt = protes(f=f_batch, d=10, n=5, m=5.E+3, log=True)
 ```
 
-The function `f_batch` takes a set of multi-indices `I` (jax array having a size `samples x d`; it can be easily converted to a numpy array if needed) and returns a list or numpy array of the corresponding array values; `m` is is the computational budget (the allowed number of requested array elements). Returned values `i_opt` (jax array) and `y_opt` (float) are the found multi-index and the value in this multi-index for the approximate optimum, respectively.
+The function `f_batch` takes a set of multi-indices `I` (`jax` array having a size `samples x d`) and returns a list (or `jax` array or `numpy` array) of the corresponding tensor values; `m` is is the computational budget (the allowed number of requested tensor elements). Returned values `i_opt` (`jax` array) and `y_opt` (float) are the found multi-index and the value in this multi-index for the approximate optimum (minimum, since the flag `is_max` is not set) of the target tensor, respectively.
+
+> The input `I` it can be easily converted to a `numpy` array if needed (i.e.m `import numpy as np; I = np.array(I)`), so you you can use the ordinary `numpy` inside the taget function and do not use the `jax` at all.
 
-Note that the code runs orders of magnitude faster if the array's mode size (`n`) is constant, as shown in the example above. If you need to optimize an array with discriminating mode sizes, then you should use the slow `protes_general` method (i.e., `from protes import protes_general`). In this case, instead of two parameters `d` and `n`, one parameter `n` should be passed, which is a list of the length `d` corresponding to the mode sizes in each dimension.
+> Note that the code runs orders of magnitude faster if the tensor's mode size (`n`) is the same for all modes, as shown in the example above. If you need to optimize a tensor with discriminating mode sizes, then you should use the slow `protes_general` function (i.e., `from protes import protes_general`). In this case, instead of two parameters `d` and `n`, one parameter `n` should be passed, which is a list of the length `d` corresponding to the mode sizes in each dimension (all other parameters for the function `protes_general` are the same as for the function `protes`, which are detailed in the next section).
 
 Please, see also:
 
-- The `demo` folder contains several examples of using the PROTES method for real tasks (a simple demo can be run in the console with a command `python demo/demo_func.py` and `python demo/demo_qubo.py`).
+- The `demo` folder contains several examples of using the `PROTES` method for real tasks (a simple demo can be run in the console with a command `python demo/demo_func.py` and `python demo/demo_qubo.py`).
 
-- The `calc` folder contains test runs of the PROTES method for various model problems (20 benchmarks) and compare it with other optimization methods (7 baselines). Additional dependencies from the `requirements_calc.txt` file should be installed to run the related script `calc/calc.py`.
+- The `calc` folder contains test runs of the `PROTES` method for various model problems (20 benchmarks) and its comparison with other optimization methods (7 baselines). Additional dependencies from the `requirements_calc.txt` file should be installed to run the related script `calc/calc.py` and `calc/calc_one.py`.
 
 - The `animation` folder contains a script `animate.py` for building an animation of the 2D optimization process.
 
 
 ## Parameters of the `protes` function
 
 **Mandatory arguments**:
 
-- `f` (function) - the target function `f(I)`, where input `I` is a 2D array of the shape `[samples, d]` (`d` is a number of dimensions of the function's input and `samples` is a batch size of requested multi-indices). The function should return 1D list or numpy array or jax array of the length equals to `samples` (the values of the target function for all provided multi-indices).
-- `d` (int) - number of array dimensions.
-- `n` (int) - mode size for each array's dimension.
-- `m` (int) - the number of allowed requests to the objective function.
+- `f` (function) - the target function `f(I)`, where input `I` is a 2D jax array of the shape `[samples, d]` (`d` is a number of dimensions of the function's input and `samples` is a batch size of requested multi-indices). The function should return 1D list or jax array or numpy array of the length equals to `samples` (the values of the target function for all provided multi-indices, i.e., the the values of the optimized tensor).
+- `d` (int) - number of tensor dimensions.
+- `n` (int) - mode size for each tensor's dimension.
 
 **Optional arguments**:
 
+- `m` (int) - the number of allowed requests to the objective function (the default value is `None`). If this parameter is not set, then the optimization process will continue until the objective function returns `None` instead of a list of values.
 - `k` (int) - the batch size for optimization (the default value is `100`).
 - `k_top` (int) - number of selected candidates in the batch (it should be `< k`; the default value is `10`).
 - `k_gd` (int) - number of gradient lifting iterations for each batch (the default value is `1`).
 - `lr` (float): learning rate for gradient lifting iterations (the default value is `5.E-2`).
 - `r` (int): TT-rank of the constructed probability TT-tensor (the default value is `5`).
 - `seed` (int): parameter for jax random generator (the default value is `0`).
 - `is_max` (bool): if flag is set, then maximization rather than minimization will be performed.
 - `log` (bool): if flag is set, then the information about the progress of the algorithm will be printed after each improvement of the optimization result and at the end of the algorithm's work.
 - `log_ind` (bool): if flag is set and `log` is True, then the current optimal multi-index will be printed every step.
 - `info` (dict): optional dictionary, which will be filled with reference information about the process of the algorithm operation.
-- `P` (list): optional initial probability tensor in the TT-format. If this parameter is not set, then a random initial TT-tensor will be generated. Note that this tensor will be changed inplace.
+- `P` (list): optional initial probability tensor in the TT-format (represented as a list of jax arrays, where all non-edge TT-cores are merged into one array; see the function `_generate_initial` in `protes.py` for details). If this parameter is not set, then a random initial TT-tensor will be generated. Note that this tensor will be changed inplace.
 
 
 ## Notes
 
-- You can use the outer cache for the values requested by the optimizer (that is, for each requested batch, check if any of the multi-indices have already been calculated), this can in some cases reduce the number of requests to the objective function.
+- You can use the outer cache for the values requested by the optimizer (that is, for each requested batch, check if any of the multi-indices have already been calculated), this can in some cases reduce the number of requests to the objective function. In this case, it is convenient not to set limits on the number of requests (parameter `m`), but instead, when the budget is exhausted (including the cache), return the `None` value from the target function (`f`), in which case the optimization algorithm will be automatically terminated.
 
 - For a number of tasks, performance can be improved by switching to increased precision in the representation of numbers in `jax`; for this, at the beginning of the script, you should specify the code:
     ```python
-    from jax.config import config
-    config.update('jax_enable_x64', True)
+    import jax
+    jax.config.update('jax_enable_x64', True)
     ```
 
-- If there is a GPU, the jax optimizer code will be automatically executed on it, however, the current version of the code works better on the CPU. To use CPU, you should specify the following code at the beginning of the executable script:
+- If there is a GPU, the `jax` optimizer code will be automatically executed on it, however, the current version of the code works better on the CPU (also, we did not conduct thorough testing of the current version of the code on the GPU). To use CPU on a device with available GPU, you should specify the following code at the beginning of the executable script:
     ```python
-    import os
-    os.environ['JAX_PLATFORM_NAME'] = 'cpu'
+    import jax
+    jax.config.update('jax_platform_name', 'cpu')
+    jax.default_device(jax.devices('cpu')[0]);
     ```
 
 
 ## Authors
 
 - [Anastasia Batsheva](https://github.com/anabatsh)
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
@@ -116,15 +121,15 @@
 
 If you find our approach and/or code useful in your research, please consider citing:
 
 ```bibtex
 @article{batsheva2023protes,
     author    = {Batsheva, Anastasia and Chertkov, Andrei and Ryzhakov, Gleb and Oseledets, Ivan},
     year      = {2023},
-    title     = {PROTES: Probabilistic Optimization with Tensor Sampling},
+    title     = {{PROTES}: {P}robabilistic optimization with tensor sampling},
     journal   = {arXiv preprint arXiv:2301.12162},
     url       = {https://arxiv.org/pdf/2301.12162.pdf}
 }
 ```
 
 > ✭ 🚂 The stars that you give to **PROTES**, motivate us to develop faster and add new interesting features to the code 😃
```

### Comparing `protes-0.3.2/README.md` & `protes-0.3.3/protes.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,115 @@
+Metadata-Version: 2.1
+Name: protes
+Version: 0.3.3
+Summary: Method PROTES (PRobability Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
+Home-page: https://github.com/anabatsh/PROTES
+Author: Andrei Chertkov
+Author-email: andre.chertkov@gmail.com
+Project-URL: Source, https://github.com/anabatsh/PROTES
+Keywords: Derivative-free optimization multidimensional optimization low-rank representation tensor train format
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # PROTES
 
 
 ## Description
 
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-To use this package, please install manually first the [python](https://www.python.org) programming language of the version >= 3.8, then, the package can be installed via pip: `pip install protes`.
+> Current version "0.3.3".
+
+To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip: `pip install protes`.
 
-> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product. To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
+> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.4+), [scipy](https://github.com/scipy/scipy) (1.9+) and [seaborn](https://seaborn.pydata.org/) (0.12.2+) will be automatically installed during the installation of the main software product (see `requirements.txt` for more details). To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
 
-To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt`.
+To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt` (please, note that the versions specified in this file are only suitable for `python 3.8`).
 
 
 ## Usage
 
-Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary array element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
+Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary tensor element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
 
 ```python
 import jax.numpy as jnp
 from protes import protes
 f_batch = lambda I: jnp.sum(I, axis=1)
 i_opt, y_opt = protes(f=f_batch, d=10, n=5, m=5.E+3, log=True)
 ```
 
-The function `f_batch` takes a set of multi-indices `I` (jax array having a size `samples x d`; it can be easily converted to a numpy array if needed) and returns a list or numpy array of the corresponding array values; `m` is is the computational budget (the allowed number of requested array elements). Returned values `i_opt` (jax array) and `y_opt` (float) are the found multi-index and the value in this multi-index for the approximate optimum, respectively.
+The function `f_batch` takes a set of multi-indices `I` (`jax` array having a size `samples x d`) and returns a list (or `jax` array or `numpy` array) of the corresponding tensor values; `m` is is the computational budget (the allowed number of requested tensor elements). Returned values `i_opt` (`jax` array) and `y_opt` (float) are the found multi-index and the value in this multi-index for the approximate optimum (minimum, since the flag `is_max` is not set) of the target tensor, respectively.
+
+> The input `I` it can be easily converted to a `numpy` array if needed (i.e.m `import numpy as np; I = np.array(I)`), so you you can use the ordinary `numpy` inside the taget function and do not use the `jax` at all.
 
-Note that the code runs orders of magnitude faster if the array's mode size (`n`) is constant, as shown in the example above. If you need to optimize an array with discriminating mode sizes, then you should use the slow `protes_general` method (i.e., `from protes import protes_general`). In this case, instead of two parameters `d` and `n`, one parameter `n` should be passed, which is a list of the length `d` corresponding to the mode sizes in each dimension.
+> Note that the code runs orders of magnitude faster if the tensor's mode size (`n`) is the same for all modes, as shown in the example above. If you need to optimize a tensor with discriminating mode sizes, then you should use the slow `protes_general` function (i.e., `from protes import protes_general`). In this case, instead of two parameters `d` and `n`, one parameter `n` should be passed, which is a list of the length `d` corresponding to the mode sizes in each dimension (all other parameters for the function `protes_general` are the same as for the function `protes`, which are detailed in the next section).
 
 Please, see also:
 
-- The `demo` folder contains several examples of using the PROTES method for real tasks (a simple demo can be run in the console with a command `python demo/demo_func.py` and `python demo/demo_qubo.py`).
+- The `demo` folder contains several examples of using the `PROTES` method for real tasks (a simple demo can be run in the console with a command `python demo/demo_func.py` and `python demo/demo_qubo.py`).
 
-- The `calc` folder contains test runs of the PROTES method for various model problems (20 benchmarks) and compare it with other optimization methods (7 baselines). Additional dependencies from the `requirements_calc.txt` file should be installed to run the related script `calc/calc.py`.
+- The `calc` folder contains test runs of the `PROTES` method for various model problems (20 benchmarks) and its comparison with other optimization methods (7 baselines). Additional dependencies from the `requirements_calc.txt` file should be installed to run the related script `calc/calc.py` and `calc/calc_one.py`.
 
 - The `animation` folder contains a script `animate.py` for building an animation of the 2D optimization process.
 
 
 ## Parameters of the `protes` function
 
 **Mandatory arguments**:
 
-- `f` (function) - the target function `f(I)`, where input `I` is a 2D array of the shape `[samples, d]` (`d` is a number of dimensions of the function's input and `samples` is a batch size of requested multi-indices). The function should return 1D list or numpy array or jax array of the length equals to `samples` (the values of the target function for all provided multi-indices).
-- `d` (int) - number of array dimensions.
-- `n` (int) - mode size for each array's dimension.
-- `m` (int) - the number of allowed requests to the objective function.
+- `f` (function) - the target function `f(I)`, where input `I` is a 2D jax array of the shape `[samples, d]` (`d` is a number of dimensions of the function's input and `samples` is a batch size of requested multi-indices). The function should return 1D list or jax array or numpy array of the length equals to `samples` (the values of the target function for all provided multi-indices, i.e., the the values of the optimized tensor).
+- `d` (int) - number of tensor dimensions.
+- `n` (int) - mode size for each tensor's dimension.
 
 **Optional arguments**:
 
+- `m` (int) - the number of allowed requests to the objective function (the default value is `None`). If this parameter is not set, then the optimization process will continue until the objective function returns `None` instead of a list of values.
 - `k` (int) - the batch size for optimization (the default value is `100`).
 - `k_top` (int) - number of selected candidates in the batch (it should be `< k`; the default value is `10`).
 - `k_gd` (int) - number of gradient lifting iterations for each batch (the default value is `1`).
 - `lr` (float): learning rate for gradient lifting iterations (the default value is `5.E-2`).
 - `r` (int): TT-rank of the constructed probability TT-tensor (the default value is `5`).
 - `seed` (int): parameter for jax random generator (the default value is `0`).
 - `is_max` (bool): if flag is set, then maximization rather than minimization will be performed.
 - `log` (bool): if flag is set, then the information about the progress of the algorithm will be printed after each improvement of the optimization result and at the end of the algorithm's work.
 - `log_ind` (bool): if flag is set and `log` is True, then the current optimal multi-index will be printed every step.
 - `info` (dict): optional dictionary, which will be filled with reference information about the process of the algorithm operation.
-- `P` (list): optional initial probability tensor in the TT-format. If this parameter is not set, then a random initial TT-tensor will be generated. Note that this tensor will be changed inplace.
+- `P` (list): optional initial probability tensor in the TT-format (represented as a list of jax arrays, where all non-edge TT-cores are merged into one array; see the function `_generate_initial` in `protes.py` for details). If this parameter is not set, then a random initial TT-tensor will be generated. Note that this tensor will be changed inplace.
 
 
 ## Notes
 
-- You can use the outer cache for the values requested by the optimizer (that is, for each requested batch, check if any of the multi-indices have already been calculated), this can in some cases reduce the number of requests to the objective function.
+- You can use the outer cache for the values requested by the optimizer (that is, for each requested batch, check if any of the multi-indices have already been calculated), this can in some cases reduce the number of requests to the objective function. In this case, it is convenient not to set limits on the number of requests (parameter `m`), but instead, when the budget is exhausted (including the cache), return the `None` value from the target function (`f`), in which case the optimization algorithm will be automatically terminated.
 
 - For a number of tasks, performance can be improved by switching to increased precision in the representation of numbers in `jax`; for this, at the beginning of the script, you should specify the code:
     ```python
-    from jax.config import config
-    config.update('jax_enable_x64', True)
+    import jax
+    jax.config.update('jax_enable_x64', True)
     ```
 
-- If there is a GPU, the jax optimizer code will be automatically executed on it, however, the current version of the code works better on the CPU. To use CPU, you should specify the following code at the beginning of the executable script:
+- If there is a GPU, the `jax` optimizer code will be automatically executed on it, however, the current version of the code works better on the CPU (also, we did not conduct thorough testing of the current version of the code on the GPU). To use CPU on a device with available GPU, you should specify the following code at the beginning of the executable script:
     ```python
-    import os
-    os.environ['JAX_PLATFORM_NAME'] = 'cpu'
+    import jax
+    jax.config.update('jax_platform_name', 'cpu')
+    jax.default_device(jax.devices('cpu')[0]);
     ```
 
 
 ## Authors
 
 - [Anastasia Batsheva](https://github.com/anabatsh)
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
@@ -92,15 +121,15 @@
 
 If you find our approach and/or code useful in your research, please consider citing:
 
 ```bibtex
 @article{batsheva2023protes,
     author    = {Batsheva, Anastasia and Chertkov, Andrei and Ryzhakov, Gleb and Oseledets, Ivan},
     year      = {2023},
-    title     = {PROTES: Probabilistic Optimization with Tensor Sampling},
+    title     = {{PROTES}: {P}robabilistic optimization with tensor sampling},
     journal   = {arXiv preprint arXiv:2301.12162},
     url       = {https://arxiv.org/pdf/2301.12162.pdf}
 }
 ```
 
 > ✭ 🚂 The stars that you give to **PROTES**, motivate us to develop faster and add new interesting features to the code 😃
```

### Comparing `protes-0.3.2/calc/.DS_Store` & `protes-0.3.3/calc/.DS_Store`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0087 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
-00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
-00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
+00000050: 0000 0001 0000 1000 6c67 3153 636f 6d70  ........lg1Scomp
+00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000080: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00000090: 006f 0070 0074 0069 6c67 3153 636f 6d70  .o.p.t.ilg1Scomp
+000000a0: 0000 0000 0000 5901 0000 0004 006f 0070  ......Y......o.p
+000000b0: 0074 0069 6d6f 4444 626c 6f62 0000 0008  .t.imoDDblob....
+000000c0: e8f4 5cd6 8e0a c541 0000 0004 006f 0070  ..\....A.....o.p
+000000d0: 0074 0069 6d6f 6444 626c 6f62 0000 0008  .t.imodDblob....
+000000e0: e8f4 5cd6 8e0a c541 0000 0004 006f 0070  ..\....A.....o.p
+000000f0: 0074 0069 7068 3153 636f 6d70 0000 0000  .t.iph1Scomp....
+00000100: 0001 4000 0000 0000 0000 0000 0000 0000  ..@.............
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,34 +26,34 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
-00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000230: 0000 0000 64cd 0000 000b 005f 005f 0070  ....d......_._.p
-00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000250: 6d6f 4444 626c 6f62 0000 0008 218e 33d6  moDDblob....!.3.
-00000260: 8e0a c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
-00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000280: 6444 626c 6f62 0000 0008 218e 33d6 8e0a  dDblob....!.3...
-00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000002b0: 636f 6d70 0000 0000 0000 7000 0000 0004  comp......p.....
-000002c0: 006f 0070 0074 0069 6c67 3153 636f 6d70  .o.p.t.ilg1Scomp
-000002d0: 0000 0000 0000 5901 0000 0004 006f 0070  ......Y......o.p
-000002e0: 0074 0069 6d6f 4444 626c 6f62 0000 0008  .t.imoDDblob....
-000002f0: e8f4 5cd6 8e0a c541 0000 0004 006f 0070  ..\....A.....o.p
-00000300: 0074 0069 6d6f 6444 626c 6f62 0000 0008  .t.imodDblob....
-00000310: e8f4 5cd6 8e0a c541 0000 0004 006f 0070  ..\....A.....o.p
-00000320: 0074 0069 7068 3153 636f 6d70 0000 0000  .t.iph1Scomp....
-00000330: 0001 4000 0000 0000 0000 0000 0000 0000  ..@.............
+00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0087 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001440: 0000 0000 0100 0001 0000 0000 0100 0002  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `protes-0.3.2/calc/calc.py` & `protes-0.3.3/calc/calc.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/calc_one.py` & `protes-0.3.3/calc/calc_one.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/constr.py` & `protes-0.3.3/calc/constr.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/construct_TT.py` & `protes-0.3.3/calc/construct_TT.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/deps.png` & `protes-0.3.3/calc/deps.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/log.txt` & `protes-0.3.3/calc/log.txt`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/log_one.txt` & `protes-0.3.3/calc/log_one.txt`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/__init__.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti_nb.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti_nb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti_opo.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti_opo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti_protes.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti_protes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti_pso.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti_pso.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti_spsa.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti_spsa.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc` & `protes-0.3.3/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/opti.py` & `protes-0.3.3/calc/opti/opti.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/opti_optimatt.py` & `protes-0.3.3/calc/opti/opti_optimatt.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/opti_protes.py` & `protes-0.3.3/calc/opti/opti_protes.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/opti/opti_ttopt.py` & `protes-0.3.3/calc/opti/opti_ttopt.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/calc/res.pickle` & `protes-0.3.3/calc/res.pickle`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/demo/.DS_Store` & `protes-0.3.3/demo/.DS_Store`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/demo/check_ackley.ipynb` & `protes-0.3.3/demo/check_ackley.ipynb`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/demo/check_knapsack.ipynb` & `protes-0.3.3/demo/check_knapsack.ipynb`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/demo/demo_func.py` & `protes-0.3.3/demo/demo_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+import jax
+jax.config.update('jax_enable_x64', True)
+jax.config.update('jax_platform_name', 'cpu')
+jax.default_device(jax.devices('cpu')[0])
+
+
 import jax.numpy as jnp
 from time import perf_counter as tpc
 
 
 from protes import protes
 
 
@@ -38,33 +44,36 @@
     We will find the minimum of an implicitly given "d"-dimensional array
     having "n" elements in each dimension. The array is obtained from the
     discretization of an analytic function.
 
     The result in console should looks like this (note that the exact minimum
     of this function is y = 0 and it is reached at the origin of coordinates):
 
-    protes > m 1.0e+02 | t 3.190e+00 | y  2.0214e+01
-    protes > m 2.0e+02 | t 3.203e+00 | y  1.8211e+01
-    protes > m 5.0e+02 | t 3.216e+00 | y  1.8174e+01
-    protes > m 6.0e+02 | t 3.220e+00 | y  1.7491e+01
-    protes > m 7.0e+02 | t 3.224e+00 | y  1.7078e+01
-    protes > m 8.0e+02 | t 3.228e+00 | y  1.6180e+01
-    protes > m 1.1e+03 | t 3.238e+00 | y  1.4116e+01
-    protes > m 1.4e+03 | t 3.250e+00 | y  8.4726e+00
-    protes > m 2.7e+03 | t 3.293e+00 | y  0.0000e+00
-    protes > m 1.0e+04 | t 3.534e+00 | y  0.0000e+00 <<< DONE
+    protes > m 1.0e+02 | t 3.298e+00 | y  2.0224e+01
+    protes > m 2.0e+02 | t 3.311e+00 | y  1.8719e+01
+    protes > m 3.0e+02 | t 3.315e+00 | y  1.8706e+01
+    protes > m 5.0e+02 | t 3.323e+00 | y  1.7536e+01
+    protes > m 6.0e+02 | t 3.327e+00 | y  1.6648e+01
+    protes > m 8.0e+02 | t 3.334e+00 | y  1.6180e+01
+    protes > m 1.3e+03 | t 3.351e+00 | y  1.5263e+01
+    protes > m 1.4e+03 | t 3.355e+00 | y  1.4116e+01
+    protes > m 1.9e+03 | t 3.372e+00 | y  1.3057e+01
+    protes > m 2.1e+03 | t 3.379e+00 | y  1.3057e+01
+    protes > m 2.5e+03 | t 3.392e+00 | y  8.4726e+00
+    protes > m 4.1e+03 | t 3.446e+00 | y  0.0000e+00
+    protes > m 1.0e+04 | t 3.647e+00 | y  0.0000e+00 <<< DONE
 
-    RESULT | y opt =  0.0000e+00 | time =     3.5459
+    RESULT | y opt =  0.0000e+00 | time =     3.6594
 
     """
     d = 7                # Dimension
     n = 11               # Mode size
     m = int(1.E+4)       # Number of requests to the objective function
     f = func_build(d, n) # Target function, which defines the array elements
 
     t = tpc()
     i_opt, y_opt = protes(f, d, n, m, log=True)
-    print(f'\nRESULT | y opt = {y_opt:-11.4e} | time = {tpc()-t:-10.4f}')
+    print(f'\nRESULT | y opt = {y_opt:-11.4e} | time = {tpc()-t:-10.4f}\n\n')
 
 
 if __name__ == '__main__':
     demo()
```

### Comparing `protes-0.3.2/demo/demo_qubo.py` & `protes-0.3.3/demo/demo_qubo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+import jax
+jax.config.update('jax_enable_x64', True)
+jax.config.update('jax_platform_name', 'cpu')
+jax.default_device(jax.devices('cpu')[0])
+
+
 import numpy as np
 from time import perf_counter as tpc
 
 
 from protes import protes
 
 
@@ -41,35 +47,35 @@
     C = 1000. It is from work (Dong et al., 2021) (problem k3; d = 50), where
     anglemodulated bat algorithm (AMBA) was proposed for high-dimensional
     binary optimization problems with engineering application to antenna
     topology optimization. Note that ths problem has known exact solution -3103.
 
     The result in console should looks like this:
 
-    protes > m 1.0e+02 | t 3.021e+00 | y -2.7560e+03
-    protes > m 3.0e+02 | t 3.051e+00 | y -2.8150e+03
-    protes > m 4.0e+02 | t 3.061e+00 | y -2.8350e+03
-    protes > m 8.0e+02 | t 3.099e+00 | y -2.8700e+03
-    protes > m 1.0e+03 | t 3.116e+00 | y -2.8850e+03
-    protes > m 1.1e+03 | t 3.124e+00 | y -2.9070e+03
-    protes > m 1.3e+03 | t 3.139e+00 | y -2.9350e+03
-    protes > m 1.4e+03 | t 3.147e+00 | y -2.9690e+03
-    protes > m 1.7e+03 | t 3.171e+00 | y -2.9990e+03
-    protes > m 2.0e+03 | t 3.194e+00 | y -3.0030e+03
-    protes > m 2.2e+03 | t 3.210e+00 | y -3.0700e+03
-    protes > m 6.9e+03 | t 3.574e+00 | y -3.0720e+03
-    protes > m 8.5e+03 | t 3.701e+00 | y -3.0750e+03
-    protes > m 1.0e+04 | t 3.816e+00 | y -3.0750e+03 <<< DONE
+    protes > m 1.0e+02 | t 3.447e+00 | y -2.7530e+03
+    protes > m 2.0e+02 | t 3.464e+00 | y -2.7650e+03
+    protes > m 7.0e+02 | t 3.498e+00 | y -2.7680e+03
+    protes > m 9.0e+02 | t 3.510e+00 | y -2.7760e+03
+    protes > m 1.0e+03 | t 3.515e+00 | y -2.8630e+03
+    protes > m 1.3e+03 | t 3.533e+00 | y -2.8730e+03
+    protes > m 1.4e+03 | t 3.539e+00 | y -2.9310e+03
+    protes > m 1.6e+03 | t 3.551e+00 | y -2.9390e+03
+    protes > m 1.8e+03 | t 3.563e+00 | y -2.9510e+03
+    protes > m 1.9e+03 | t 3.568e+00 | y -2.9990e+03
+    protes > m 2.5e+03 | t 3.604e+00 | y -3.0020e+03
+    protes > m 2.9e+03 | t 3.627e+00 | y -3.0250e+03
+    protes > m 3.0e+03 | t 3.633e+00 | y -3.0790e+03
+    protes > m 1.0e+04 | t 4.029e+00 | y -3.0790e+03 <<< DONE
 
-    RESULT | y opt = -3.0750e+03 | time =     3.8277
+    RESULT | y opt = -3.0790e+03 | time =     4.0412
 
     """
     d, n, f = func_build() # Target function, and array shape
     m = int(1.E+4)         # Number of requests to the objective function
 
     t = tpc()
     i_opt, y_opt = protes(f, d, n, m, log=True)
-    print(f'\nRESULT | y opt = {y_opt:-11.4e} | time = {tpc()-t:-10.4f}')
+    print(f'\nRESULT | y opt = {y_opt:-11.4e} | time = {tpc()-t:-10.4f}\n\n')
 
 
 if __name__ == '__main__':
     demo()
```

### Comparing `protes-0.3.2/demo/figures/.DS_Store` & `protes-0.3.3/demo/figures/.DS_Store`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/demo/figures/check_ackley.png` & `protes-0.3.3/demo/figures/check_ackley.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/demo/figures/check_ackley_ext.png` & `protes-0.3.3/demo/figures/check_ackley_ext.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/demo/figures/check_knapsack.png` & `protes-0.3.3/demo/figures/check_knapsack.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/demo/figures/check_knapsack_ext.png` & `protes-0.3.3/demo/figures/check_knapsack_ext.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/protes/animation.py` & `protes-0.3.3/protes/animation.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.2/protes/protes.py` & `protes-0.3.3/protes/protes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import jax
 import jax.numpy as jnp
 import optax
 from time import perf_counter as tpc
 
 
-def protes(f, d, n, m, k=100, k_top=10, k_gd=1, lr=5.E-2, r=5, seed=0,
+def protes(f, d, n, m=None, k=100, k_top=10, k_gd=1, lr=5.E-2, r=5, seed=0,
            is_max=False, log=False, log_ind=False, info={}, P=None,
            with_info_i_opt_list=False, with_info_full=False):
     time = tpc()
     info.update({'d': d, 'n': n, 'm_max': m, 'm': 0, 'k': k, 'k_top': k_top,
         'k_gd': k_gd, 'lr': lr, 'r': r, 'seed': seed, 'is_max': is_max,
         'is_rand': P is None, 't': 0, 'i_opt': None, 'y_opt': None,
         'm_opt_list': [], 'i_opt_list': [], 'y_opt_list': []})
@@ -50,33 +50,35 @@
     while True:
         Pl, Pm, Pr = P
         Zm = interface_matrices(Pm, Pr)
         rng, key = jax.random.split(rng)
         I = sample(Pl, Pm, Pr, Zm, jax.random.split(key, k))
 
         y = f(I)
+        if y is None:
+            break
+
         y = jnp.array(y)
         info['m'] += y.shape[0]
 
         is_new = _check(P, I, y, info, with_info_i_opt_list, with_info_full)
 
-        if info['m'] >= m:
-            info['t'] = tpc() - time
+        if info['m_max'] and info['m'] >= info['m_max']:
             break
 
         ind = jnp.argsort(y, kind='stable')
         ind = (ind[::-1] if is_max else ind)[:k_top]
 
         for _ in range(k_gd):
             state, P = optimize(state, P, I[ind, :])
 
         info['t'] = tpc() - time
-
         _log(info, log, log_ind, is_new)
 
+    info['t'] = tpc() - time
     _log(info, log, log_ind, is_new, is_end=True)
 
     return info['i_opt'], info['y_opt']
 
 
 def _check(P, I, y, info, with_info_i_opt_list, with_info_full):
     """Check the current batch of function values and save the improvement."""
```

### Comparing `protes-0.3.2/protes/protes_general.py` & `protes-0.3.3/protes/protes_general.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import jax
 import jax.numpy as jnp
 import optax
 from time import perf_counter as tpc
 
 
-def protes_general(f, n, m, k=100, k_top=10, k_gd=1, lr=5.E-2, r=5, seed=0,
+def protes_general(f, n, m=None, k=100, k_top=10, k_gd=1, lr=5.E-2, r=5, seed=0,
                    is_max=False, log=False, log_ind=False, info={}, P=None,
                    with_info_i_opt_list=False, with_info_full=False):
     time = tpc()
     info.update({'n': n, 'm_max': m, 'm': 0, 'k': k, 'k_top': k_top,
         'k_gd': k_gd, 'lr': lr, 'r': r, 'seed': seed, 'is_max': is_max,
         'is_rand': P is None, 't': 0, 'i_opt': None, 'y_opt': None,
         'm_opt_list': [], 'i_opt_list': [], 'y_opt_list': []})
@@ -26,15 +26,16 @@
     state = optim.init(P)
 
     sample = jax.jit(jax.vmap(_sample, (None, 0)))
     likelihood = jax.jit(jax.vmap(_likelihood, (None, 0)))
 
     @jax.jit
     def loss(P_cur, I_cur):
-        return jnp.mean(-likelihood(P_cur, I_cur))
+        l = likelihood(P_cur, I_cur)
+        return jnp.mean(-l)
 
     loss_grad = jax.grad(loss)
 
     @jax.jit
     def optimize(state, P_cur, I_cur):
         grads = loss_grad(P_cur, I_cur)
         updates, state = optim.update(grads, state)
@@ -42,33 +43,35 @@
         return state, P_cur
 
     while True:
         rng, key = jax.random.split(rng)
         I = sample(P, jax.random.split(key, k))
 
         y = f(I)
+        if y is None:
+            break
+
         y = jnp.array(y)
         info['m'] += y.shape[0]
 
         is_new = _check(P, I, y, info, with_info_i_opt_list, with_info_full)
 
-        if info['m'] >= m:
-            info['t'] = tpc() - time
+        if info['m_max'] and info['m'] >= info['m_max']:
             break
 
         ind = jnp.argsort(y, kind='stable')
         ind = (ind[::-1] if is_max else ind)[:k_top]
 
         for _ in range(k_gd):
             state, P = optimize(state, P, I[ind, :])
 
         info['t'] = tpc() - time
-
         _log(info, log, log_ind, is_new)
 
+    info['t'] = tpc() - time
     _log(info, log, log_ind, is_new, is_end=True)
 
     return info['i_opt'], info['y_opt']
 
 
 def _check(P, I, y, info, with_info_i_opt_list, with_info_full):
     """Check the current batch of function values and save the improvement."""
```

### Comparing `protes-0.3.2/protes.egg-info/PKG-INFO` & `protes-0.3.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,110 +1,91 @@
-Metadata-Version: 2.1
-Name: protes
-Version: 0.3.2
-Summary: Method PROTES (PRobability Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
-Home-page: https://github.com/anabatsh/PROTES
-Author: Andrei Chertkov
-Author-email: andre.chertkov@gmail.com
-Project-URL: Source, https://github.com/anabatsh/PROTES
-Keywords: Derivative-free optimization multidimensional optimization low-rank representation tensor train format
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # PROTES
 
 
 ## Description
 
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-To use this package, please install manually first the [python](https://www.python.org) programming language of the version >= 3.8, then, the package can be installed via pip: `pip install protes`.
+> Current version "0.3.3".
+
+To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip: `pip install protes`.
 
-> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product. To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
+> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.4+), [scipy](https://github.com/scipy/scipy) (1.9+) and [seaborn](https://seaborn.pydata.org/) (0.12.2+) will be automatically installed during the installation of the main software product (see `requirements.txt` for more details). To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
 
-To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt`.
+To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt` (please, note that the versions specified in this file are only suitable for `python 3.8`).
 
 
 ## Usage
 
-Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary array element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
+Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary tensor element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
 
 ```python
 import jax.numpy as jnp
 from protes import protes
 f_batch = lambda I: jnp.sum(I, axis=1)
 i_opt, y_opt = protes(f=f_batch, d=10, n=5, m=5.E+3, log=True)
 ```
 
-The function `f_batch` takes a set of multi-indices `I` (jax array having a size `samples x d`; it can be easily converted to a numpy array if needed) and returns a list or numpy array of the corresponding array values; `m` is is the computational budget (the allowed number of requested array elements). Returned values `i_opt` (jax array) and `y_opt` (float) are the found multi-index and the value in this multi-index for the approximate optimum, respectively.
+The function `f_batch` takes a set of multi-indices `I` (`jax` array having a size `samples x d`) and returns a list (or `jax` array or `numpy` array) of the corresponding tensor values; `m` is is the computational budget (the allowed number of requested tensor elements). Returned values `i_opt` (`jax` array) and `y_opt` (float) are the found multi-index and the value in this multi-index for the approximate optimum (minimum, since the flag `is_max` is not set) of the target tensor, respectively.
+
+> The input `I` it can be easily converted to a `numpy` array if needed (i.e.m `import numpy as np; I = np.array(I)`), so you you can use the ordinary `numpy` inside the taget function and do not use the `jax` at all.
 
-Note that the code runs orders of magnitude faster if the array's mode size (`n`) is constant, as shown in the example above. If you need to optimize an array with discriminating mode sizes, then you should use the slow `protes_general` method (i.e., `from protes import protes_general`). In this case, instead of two parameters `d` and `n`, one parameter `n` should be passed, which is a list of the length `d` corresponding to the mode sizes in each dimension.
+> Note that the code runs orders of magnitude faster if the tensor's mode size (`n`) is the same for all modes, as shown in the example above. If you need to optimize a tensor with discriminating mode sizes, then you should use the slow `protes_general` function (i.e., `from protes import protes_general`). In this case, instead of two parameters `d` and `n`, one parameter `n` should be passed, which is a list of the length `d` corresponding to the mode sizes in each dimension (all other parameters for the function `protes_general` are the same as for the function `protes`, which are detailed in the next section).
 
 Please, see also:
 
-- The `demo` folder contains several examples of using the PROTES method for real tasks (a simple demo can be run in the console with a command `python demo/demo_func.py` and `python demo/demo_qubo.py`).
+- The `demo` folder contains several examples of using the `PROTES` method for real tasks (a simple demo can be run in the console with a command `python demo/demo_func.py` and `python demo/demo_qubo.py`).
 
-- The `calc` folder contains test runs of the PROTES method for various model problems (20 benchmarks) and compare it with other optimization methods (7 baselines). Additional dependencies from the `requirements_calc.txt` file should be installed to run the related script `calc/calc.py`.
+- The `calc` folder contains test runs of the `PROTES` method for various model problems (20 benchmarks) and its comparison with other optimization methods (7 baselines). Additional dependencies from the `requirements_calc.txt` file should be installed to run the related script `calc/calc.py` and `calc/calc_one.py`.
 
 - The `animation` folder contains a script `animate.py` for building an animation of the 2D optimization process.
 
 
 ## Parameters of the `protes` function
 
 **Mandatory arguments**:
 
-- `f` (function) - the target function `f(I)`, where input `I` is a 2D array of the shape `[samples, d]` (`d` is a number of dimensions of the function's input and `samples` is a batch size of requested multi-indices). The function should return 1D list or numpy array or jax array of the length equals to `samples` (the values of the target function for all provided multi-indices).
-- `d` (int) - number of array dimensions.
-- `n` (int) - mode size for each array's dimension.
-- `m` (int) - the number of allowed requests to the objective function.
+- `f` (function) - the target function `f(I)`, where input `I` is a 2D jax array of the shape `[samples, d]` (`d` is a number of dimensions of the function's input and `samples` is a batch size of requested multi-indices). The function should return 1D list or jax array or numpy array of the length equals to `samples` (the values of the target function for all provided multi-indices, i.e., the the values of the optimized tensor).
+- `d` (int) - number of tensor dimensions.
+- `n` (int) - mode size for each tensor's dimension.
 
 **Optional arguments**:
 
+- `m` (int) - the number of allowed requests to the objective function (the default value is `None`). If this parameter is not set, then the optimization process will continue until the objective function returns `None` instead of a list of values.
 - `k` (int) - the batch size for optimization (the default value is `100`).
 - `k_top` (int) - number of selected candidates in the batch (it should be `< k`; the default value is `10`).
 - `k_gd` (int) - number of gradient lifting iterations for each batch (the default value is `1`).
 - `lr` (float): learning rate for gradient lifting iterations (the default value is `5.E-2`).
 - `r` (int): TT-rank of the constructed probability TT-tensor (the default value is `5`).
 - `seed` (int): parameter for jax random generator (the default value is `0`).
 - `is_max` (bool): if flag is set, then maximization rather than minimization will be performed.
 - `log` (bool): if flag is set, then the information about the progress of the algorithm will be printed after each improvement of the optimization result and at the end of the algorithm's work.
 - `log_ind` (bool): if flag is set and `log` is True, then the current optimal multi-index will be printed every step.
 - `info` (dict): optional dictionary, which will be filled with reference information about the process of the algorithm operation.
-- `P` (list): optional initial probability tensor in the TT-format. If this parameter is not set, then a random initial TT-tensor will be generated. Note that this tensor will be changed inplace.
+- `P` (list): optional initial probability tensor in the TT-format (represented as a list of jax arrays, where all non-edge TT-cores are merged into one array; see the function `_generate_initial` in `protes.py` for details). If this parameter is not set, then a random initial TT-tensor will be generated. Note that this tensor will be changed inplace.
 
 
 ## Notes
 
-- You can use the outer cache for the values requested by the optimizer (that is, for each requested batch, check if any of the multi-indices have already been calculated), this can in some cases reduce the number of requests to the objective function.
+- You can use the outer cache for the values requested by the optimizer (that is, for each requested batch, check if any of the multi-indices have already been calculated), this can in some cases reduce the number of requests to the objective function. In this case, it is convenient not to set limits on the number of requests (parameter `m`), but instead, when the budget is exhausted (including the cache), return the `None` value from the target function (`f`), in which case the optimization algorithm will be automatically terminated.
 
 - For a number of tasks, performance can be improved by switching to increased precision in the representation of numbers in `jax`; for this, at the beginning of the script, you should specify the code:
     ```python
-    from jax.config import config
-    config.update('jax_enable_x64', True)
+    import jax
+    jax.config.update('jax_enable_x64', True)
     ```
 
-- If there is a GPU, the jax optimizer code will be automatically executed on it, however, the current version of the code works better on the CPU. To use CPU, you should specify the following code at the beginning of the executable script:
+- If there is a GPU, the `jax` optimizer code will be automatically executed on it, however, the current version of the code works better on the CPU (also, we did not conduct thorough testing of the current version of the code on the GPU). To use CPU on a device with available GPU, you should specify the following code at the beginning of the executable script:
     ```python
-    import os
-    os.environ['JAX_PLATFORM_NAME'] = 'cpu'
+    import jax
+    jax.config.update('jax_platform_name', 'cpu')
+    jax.default_device(jax.devices('cpu')[0]);
     ```
 
 
 ## Authors
 
 - [Anastasia Batsheva](https://github.com/anabatsh)
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
@@ -116,15 +97,15 @@
 
 If you find our approach and/or code useful in your research, please consider citing:
 
 ```bibtex
 @article{batsheva2023protes,
     author    = {Batsheva, Anastasia and Chertkov, Andrei and Ryzhakov, Gleb and Oseledets, Ivan},
     year      = {2023},
-    title     = {PROTES: Probabilistic Optimization with Tensor Sampling},
+    title     = {{PROTES}: {P}robabilistic optimization with tensor sampling},
     journal   = {arXiv preprint arXiv:2301.12162},
     url       = {https://arxiv.org/pdf/2301.12162.pdf}
 }
 ```
 
 > ✭ 🚂 The stars that you give to **PROTES**, motivate us to develop faster and add new interesting features to the code 😃
```

### Comparing `protes-0.3.2/protes.egg-info/SOURCES.txt` & `protes-0.3.3/protes.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 MANIFEST.in
 README.md
+requirements.txt
+requirements_calc.txt
 setup.py
 calc/.DS_Store
 calc/calc.py
 calc/calc_one.py
 calc/constr.py
 calc/construct_TT.py
 calc/deps.png
 calc/log.txt
 calc/log_one.txt
 calc/res.pickle
-calc/__pycache__/constr.cpython-38.pyc
-calc/__pycache__/construct_TT.cpython-38.pyc
 calc/opti/__init__.py
 calc/opti/opti.py
 calc/opti/opti_nb.py
 calc/opti/opti_opo.py
 calc/opti/opti_optimatt.py
 calc/opti/opti_portfolio.py
 calc/opti/opti_protes.py
```

### Comparing `protes-0.3.2/setup.py` & `protes-0.3.3/setup.py`

 * *Files identical despite different names*

