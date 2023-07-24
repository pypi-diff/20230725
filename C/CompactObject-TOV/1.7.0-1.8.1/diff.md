# Comparing `tmp/CompactObject_TOV-1.7.0.tar.gz` & `tmp/CompactObject_TOV-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CompactObject_TOV-1.7.0.tar", last modified: Mon Jul 24 20:27:57 2023, max compression
+gzip compressed data, was "CompactObject_TOV-1.8.1.tar", last modified: Mon Jul 24 22:52:30 2023, max compression
```

## Comparing `CompactObject_TOV-1.7.0.tar` & `CompactObject_TOV-1.8.1.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 20:27:57.555179 CompactObject_TOV-1.7.0/
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 20:27:57.516040 CompactObject_TOV-1.7.0/CompactObject_TOV.egg-info/
--rw-r--r--   0 a9         (501) staff       (20)      164 2023-07-24 20:27:57.000000 CompactObject_TOV-1.7.0/CompactObject_TOV.egg-info/PKG-INFO
--rw-r--r--   0 a9         (501) staff       (20)      345 2023-07-24 20:27:57.000000 CompactObject_TOV-1.7.0/CompactObject_TOV.egg-info/SOURCES.txt
--rw-r--r--   0 a9         (501) staff       (20)        1 2023-07-24 20:27:57.000000 CompactObject_TOV-1.7.0/CompactObject_TOV.egg-info/dependency_links.txt
--rw-r--r--   0 a9         (501) staff       (20)       42 2023-07-24 20:27:57.000000 CompactObject_TOV-1.7.0/CompactObject_TOV.egg-info/top_level.txt
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 20:27:57.520034 CompactObject_TOV-1.7.0/EOSgenerators/
--rw-r--r--   0 a9         (501) staff       (20)       21 2023-07-24 20:25:57.000000 CompactObject_TOV-1.7.0/EOSgenerators/__init__.py
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 20:27:57.531850 CompactObject_TOV-1.7.0/InferenceWorkflow/
--rw-r--r--   0 a9         (501) staff       (20)       22 2023-07-24 20:18:17.000000 CompactObject_TOV-1.7.0/InferenceWorkflow/__init__.py
--rw-r--r--   0 a9         (501) staff       (20)       21 2023-07-24 20:25:51.000000 CompactObject_TOV-1.7.0/InferenceWorkflow/__int__.py
--rw-r--r--   0 a9         (501) staff       (20)     1099 2023-07-16 23:02:27.000000 CompactObject_TOV-1.7.0/LICENSE
--rw-r--r--   0 a9         (501) staff       (20)      164 2023-07-24 20:27:57.554772 CompactObject_TOV-1.7.0/PKG-INFO
--rw-r--r--   0 a9         (501) staff       (20)     5021 2023-07-18 22:23:01.000000 CompactObject_TOV-1.7.0/README.md
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 20:27:57.553078 CompactObject_TOV-1.7.0/TOVsolver/
--rw-r--r--   0 a9         (501) staff       (20)       25 2023-07-24 20:25:44.000000 CompactObject_TOV-1.7.0/TOVsolver/__init__.py
--rw-r--r--   0 a9         (501) staff       (20)      158 2023-07-17 19:25:29.000000 CompactObject_TOV-1.7.0/TOVsolver/constant.py
--rw-r--r--   0 a9         (501) staff       (20)     1772 2023-07-16 23:02:27.000000 CompactObject_TOV-1.7.0/TOVsolver/tests_script.py
--rw-r--r--   0 a9         (501) staff       (20)       38 2023-07-24 20:27:57.563432 CompactObject_TOV-1.7.0/setup.cfg
--rw-r--r--   0 a9         (501) staff       (20)      136 2023-07-24 20:26:03.000000 CompactObject_TOV-1.7.0/setup.py
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.923030 CompactObject_TOV-1.8.1/
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.856800 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/
+-rw-r--r--   0 a9         (501) staff       (20)      164 2023-07-24 22:52:30.000000 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/PKG-INFO
+-rw-r--r--   0 a9         (501) staff       (20)      587 2023-07-24 22:52:30.000000 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/SOURCES.txt
+-rw-r--r--   0 a9         (501) staff       (20)        1 2023-07-24 22:52:30.000000 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/dependency_links.txt
+-rw-r--r--   0 a9         (501) staff       (20)       42 2023-07-24 22:52:30.000000 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/top_level.txt
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.858800 CompactObject_TOV-1.8.1/EOSgenerators/
+-rw-r--r--   0 a9         (501) staff       (20)     9223 2023-07-18 21:03:49.000000 CompactObject_TOV-1.8.1/EOSgenerators/RMF_EOS.py
+-rw-r--r--   0 a9         (501) staff       (20)       21 2023-07-24 22:46:50.000000 CompactObject_TOV-1.8.1/EOSgenerators/__init__.py
+-rw-r--r--   0 a9         (501) staff       (20)     1112 2023-07-18 21:08:17.000000 CompactObject_TOV-1.8.1/EOSgenerators/crust_EOS.py
+-rw-r--r--   0 a9         (501) staff       (20)     9814 2023-07-18 22:03:03.000000 CompactObject_TOV-1.8.1/EOSgenerators/fastRMF_EoS.py
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.869106 CompactObject_TOV-1.8.1/InferenceWorkflow/
+-rw-r--r--   0 a9         (501) staff       (20)     3480 2023-07-24 22:49:11.000000 CompactObject_TOV-1.8.1/InferenceWorkflow/BayesianSampler.py
+-rw-r--r--   0 a9         (501) staff       (20)    11009 2023-07-19 16:32:07.000000 CompactObject_TOV-1.8.1/InferenceWorkflow/Likelihood.py
+-rw-r--r--   0 a9         (501) staff       (20)       21 2023-07-24 22:49:13.000000 CompactObject_TOV-1.8.1/InferenceWorkflow/__int__.py
+-rw-r--r--   0 a9         (501) staff       (20)     1141 2023-07-18 21:25:02.000000 CompactObject_TOV-1.8.1/InferenceWorkflow/prior.py
+-rw-r--r--   0 a9         (501) staff       (20)     1099 2023-07-16 23:02:27.000000 CompactObject_TOV-1.8.1/LICENSE
+-rw-r--r--   0 a9         (501) staff       (20)      164 2023-07-24 22:52:30.919409 CompactObject_TOV-1.8.1/PKG-INFO
+-rw-r--r--   0 a9         (501) staff       (20)     5021 2023-07-18 22:23:01.000000 CompactObject_TOV-1.8.1/README.md
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.911679 CompactObject_TOV-1.8.1/TOVsolver/
+-rw-r--r--   0 a9         (501) staff       (20)     2620 2023-07-16 23:02:27.000000 CompactObject_TOV-1.8.1/TOVsolver/EoS_import.py
+-rw-r--r--   0 a9         (501) staff       (20)       25 2023-07-24 22:46:38.000000 CompactObject_TOV-1.8.1/TOVsolver/__init__.py
+-rw-r--r--   0 a9         (501) staff       (20)      158 2023-07-17 19:25:29.000000 CompactObject_TOV-1.8.1/TOVsolver/constant.py
+-rw-r--r--   0 a9         (501) staff       (20)     8666 2023-07-18 18:57:17.000000 CompactObject_TOV-1.8.1/TOVsolver/main.py
+-rw-r--r--   0 a9         (501) staff       (20)     8979 2023-07-18 19:01:46.000000 CompactObject_TOV-1.8.1/TOVsolver/solver_code.py
+-rw-r--r--   0 a9         (501) staff       (20)      785 2023-07-16 23:02:27.000000 CompactObject_TOV-1.8.1/TOVsolver/speed_of_sound.py
+-rw-r--r--   0 a9         (501) staff       (20)     1772 2023-07-16 23:02:27.000000 CompactObject_TOV-1.8.1/TOVsolver/tests_script.py
+-rw-r--r--   0 a9         (501) staff       (20)       38 2023-07-24 22:52:30.923774 CompactObject_TOV-1.8.1/setup.cfg
+-rw-r--r--   0 a9         (501) staff       (20)      170 2023-07-24 22:52:22.000000 CompactObject_TOV-1.8.1/setup.py
```

### Comparing `CompactObject_TOV-1.7.0/LICENSE` & `CompactObject_TOV-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.7.0/README.md` & `CompactObject_TOV-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.7.0/TOVsolver/tests_script.py` & `CompactObject_TOV-1.8.1/TOVsolver/tests_script.py`

 * *Files identical despite different names*

