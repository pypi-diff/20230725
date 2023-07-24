# Comparing `tmp/genomap-1.3.4.tar.gz` & `tmp/genomap-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.3.4.tar", last modified: Mon Jul 24 20:37:36 2023, max compression
+gzip compressed data, was "genomap-1.3.5.tar", last modified: Mon Jul 24 22:19:48 2023, max compression
```

## Comparing `genomap-1.3.4.tar` & `genomap-1.3.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.674315 genomap-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 20:33:40.000000 genomap-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 20:33:40.000000 genomap-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-24 20:37:36.674315 genomap-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-07-24 20:33:40.000000 genomap-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.658315 genomap-1.3.4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 20:33:40.000000 genomap-1.3.4/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.658315 genomap-1.3.4/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/genoAnnotate/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoAnnotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoAnnotate/genoAnnotate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoNet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNet/genoNet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoNetus/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNetus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoNetus/genoNetus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.666315 genomap-1.3.4/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.670315 genomap-1.3.4/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.670315 genomap-1.3.4/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.670315 genomap-1.3.4/genomap/genotype/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/genotype/genotype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.674315 genomap-1.3.4/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 20:33:40.000000 genomap-1.3.4/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:37:36.662315 genomap-1.3.4/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 20:37:36.000000 genomap-1.3.4/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 20:33:40.000000 genomap-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:37:36.674315 genomap-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 20:33:40.000000 genomap-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.134258 genomap-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-24 22:15:00.000000 genomap-1.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 22:15:00.000000 genomap-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-07-24 22:19:48.134258 genomap-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-24 22:15:00.000000 genomap-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.098257 genomap-1.3.5/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 22:15:00.000000 genomap-1.3.5/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.098257 genomap-1.3.5/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.102257 genomap-1.3.5/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.110257 genomap-1.3.5/genomap/genoAnnotate/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoAnnotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoAnnotate/genoAnnotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.110257 genomap-1.3.5/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.110257 genomap-1.3.5/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.110257 genomap-1.3.5/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.114257 genomap-1.3.5/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.114257 genomap-1.3.5/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.114257 genomap-1.3.5/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.114257 genomap-1.3.5/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.118257 genomap-1.3.5/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.118257 genomap-1.3.5/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.118257 genomap-1.3.5/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.118257 genomap-1.3.5/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.122257 genomap-1.3.5/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.122257 genomap-1.3.5/genomap/genotype/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/genotype/genotype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.130257 genomap-1.3.5/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 22:15:00.000000 genomap-1.3.5/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:48.102257 genomap-1.3.5/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-07-24 22:19:47.000000 genomap-1.3.5/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 22:19:48.000000 genomap-1.3.5/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:19:47.000000 genomap-1.3.5/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 22:19:47.000000 genomap-1.3.5/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 22:19:47.000000 genomap-1.3.5/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 22:15:00.000000 genomap-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 22:19:48.134258 genomap-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 22:15:00.000000 genomap-1.3.5/setup.py
```

### Comparing `genomap-1.3.4/LICENSE.txt` & `genomap-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/PKG-INFO` & `genomap-1.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.4
+Version: 1.3.5
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, gene signature extraction, multi-omics data integration, and trajectory analysis 
+# Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, automatic cell annotation, gene signature extraction, multi-omics data integration, and trajectory analysis 
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## How to use genomap
 
 The easiest way to start with genomap is to install it from pypi using 
 
@@ -207,53 +207,53 @@
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
 # returns 2D visualization, cluster labels, and intgerated data
 resVis,cli,int_data=gp.genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-
+# Plot colored with cell class labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 
+# Plot colored with batch labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
-```
 
-```python
 # Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
 
 # returns 2D embedding, cluster labels, and intgerated data
 resTraj,cli,int_data=gp.genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-
+# Plot colored with cell class labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 
+# Plot colored with batch labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
@@ -269,19 +269,17 @@
 
 # Input: adata: annData containing the raw gene counts
 # tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
  
 adataP=gp.genoAnnotate(adata,species="human", tissue_type="Immune system")
 cell_annotations=adataP.obs['cell_type'].values # numpy array containing the
 # cell annotations
-
 # Compute t-SNE
 sc.tl.tsne(adataP)
 # Create a t-SNE plot colored by cell type labels
-cell_annotations=adataP.obs['cell_type']
 sc.pl.tsne(adataP, color='cell_type')
 ```
 
 ### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
```

### Comparing `genomap-1.3.4/README.md` & `genomap-1.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, gene signature extraction, multi-omics data integration, and trajectory analysis 
+# Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, automatic cell annotation, gene signature extraction, multi-omics data integration, and trajectory analysis 
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## How to use genomap
 
 The easiest way to start with genomap is to install it from pypi using 
 
@@ -194,53 +194,53 @@
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
 # returns 2D visualization, cluster labels, and intgerated data
 resVis,cli,int_data=gp.genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-
+# Plot colored with cell class labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 
+# Plot colored with batch labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
-```
 
-```python
 # Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
 
 # returns 2D embedding, cluster labels, and intgerated data
 resTraj,cli,int_data=gp.genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-
+# Plot colored with cell class labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 
+# Plot colored with batch labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
@@ -256,19 +256,17 @@
 
 # Input: adata: annData containing the raw gene counts
 # tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
  
 adataP=gp.genoAnnotate(adata,species="human", tissue_type="Immune system")
 cell_annotations=adataP.obs['cell_type'].values # numpy array containing the
 # cell annotations
-
 # Compute t-SNE
 sc.tl.tsne(adataP)
 # Create a t-SNE plot colored by cell type labels
-cell_annotations=adataP.obs['cell_type']
 sc.pl.tsne(adataP, color='cell_type')
 ```
 
 ### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
```

### Comparing `genomap-1.3.4/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.3.5/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoAnnotate/genoAnnotate.py` & `genomap-1.3.5/genomap/genoAnnotate/genoAnnotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sun Jul 23 15:18:43 2023
 
 @author: Md Tauhidul Islam
 # This code is inspired by scType (https://github.com/IanevskiAleksandr/sc-type)
-# We are in the process of using image matching techique for further enhancement
+# We are in the process of using image matching technique for further enhancement
 # of the cell annotation
 """
 
 
 from genomap.genotype import *
 import scanpy as sc
```

### Comparing `genomap-1.3.4/genomap/genoClassification/genoClassification.py` & `genomap-1.3.5/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoDR/genoDimReduction.py` & `genomap-1.3.5/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoMOI/genoMOI.py` & `genomap-1.3.5/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoNet/genoNet.py` & `genomap-1.3.5/genomap/genoNet/genoNet.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.3.5/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoNetus/genoNetus.py` & `genomap-1.3.5/genomap/genoNetus/genoNetus.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoRegression/genoRegression.py` & `genomap-1.3.5/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoSig/genoSig.py` & `genomap-1.3.5/genomap/genoSig/genoSig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoTraj/genoTraj.py` & `genomap-1.3.5/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genoVis/genoVis.py` & `genomap-1.3.5/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genomap.py` & `genomap-1.3.5/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genomapOPT/genomapOPT.py` & `genomap-1.3.5/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genomapT/genomapT.py` & `genomap-1.3.5/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/genotype/genotype.py` & `genomap-1.3.5/genomap/genotype/genotype.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/ConvDEC.py` & `genomap-1.3.5/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/ConvIDEC.py` & `genomap-1.3.5/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/FcDEC.py` & `genomap-1.3.5/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/FcIDEC.py` & `genomap-1.3.5/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/class_discriminative_opt.py` & `genomap-1.3.5/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/gTraj_utils.py` & `genomap-1.3.5/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/group_centroid_opt.py` & `genomap-1.3.5/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/metrics.py` & `genomap-1.3.5/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/util_Sig.py` & `genomap-1.3.5/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap/utils/utils_MOI.py` & `genomap-1.3.5/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/genomap.egg-info/PKG-INFO` & `genomap-1.3.5/genomap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.3.4
+Version: 1.3.5
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, gene signature extraction, multi-omics data integration, and trajectory analysis 
+# Genomap creates images from gene expression data and offers high-performance dimensionality reduction and visualization, data clustering, classification and regression, automatic cell annotation, gene signature extraction, multi-omics data integration, and trajectory analysis 
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## How to use genomap
 
 The easiest way to start with genomap is to install it from pypi using 
 
@@ -207,53 +207,53 @@
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genomap-based multi omic integration and visualize the integrated data with local structure for cluster analysis
 # returns 2D visualization, cluster labels, and intgerated data
 resVis,cli,int_data=gp.genoMOIvis(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-
+# Plot colored with cell class labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=y,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 
+# Plot colored with batch labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resVis[:, 0], resVis[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
-```
 
-```python
 # Apply genomap-based multi omic integration and visualize the integrated data with global structure for trajectory analysis
 
 # returns 2D embedding, cluster labels, and intgerated data
 resTraj,cli,int_data=gp.genoMOItraj(data, data2, data3, data4, data5, colNum=12, rowNum=12, n_dim=32, epoch=10, prealign_method='scanorama')
 
-
+# Plot colored with cell class labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=y,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 
+# Plot colored with batch labels
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
-h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
+h1=plt.scatter(resTraj[:, 0], resTraj[:, 1], c=ybatch,cmap='jet', marker='o', s=18)      
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
@@ -269,19 +269,17 @@
 
 # Input: adata: annData containing the raw gene counts
 # tissue type: e.g. Immune system,Pancreas,Liver,Eye,Kidney,Brain,Lung,Adrenal,Heart,Intestine,Muscle,Placenta,Spleen,Stomach,Thymus 
  
 adataP=gp.genoAnnotate(adata,species="human", tissue_type="Immune system")
 cell_annotations=adataP.obs['cell_type'].values # numpy array containing the
 # cell annotations
-
 # Compute t-SNE
 sc.tl.tsne(adataP)
 # Create a t-SNE plot colored by cell type labels
-cell_annotations=adataP.obs['cell_type']
 sc.pl.tsne(adataP, color='cell_type')
 ```
 
 ### Example 7 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
```

### Comparing `genomap-1.3.4/genomap.egg-info/SOURCES.txt` & `genomap-1.3.5/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.3.4/setup.py` & `genomap-1.3.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.3.4",
+    version="1.3.5",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

