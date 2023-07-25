# Comparing `tmp/QCpython-1.0.3.tar.gz` & `tmp/qcpython-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QCpython-1.0.3.tar", last modified: Sun Apr 30 21:25:58 2023, max compression
+gzip compressed data, was "qcpython-1.1.0.tar", last modified: Tue Jul 25 03:25:22 2023, max compression
```

## Comparing `QCpython-1.0.3.tar` & `qcpython-1.1.0.tar`

### file list

```diff
@@ -1,98 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.726928 QCpython-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-30 21:25:46.000000 QCpython-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    33292 2023-04-30 21:25:58.726928 QCpython-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.710928 QCpython-1.0.3/QCpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/CircuitDrawing/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/CircuitDrawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/CircuitDrawing/circuitdrawing.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/CircuitDrawing/gateformatting.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/CircuitDrawing/quantumgatedraw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/Core/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/Core/qmace/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/qmace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/qmace/qmace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/qmace/quantumcircuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    41098 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/quantumcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/Core/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/phaseangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Core/tools/probabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/QuantumGate/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/QuantumGate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/QuantumGate/multiqubit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/QuantumGate/singlequbit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.714928 QCpython-1.0.3/QCpy/Visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/blochsphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/qsphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/statevector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.718928 QCpython-1.0.3/QCpy/Visualizer/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/Visualizer/tools/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-30 21:25:46.000000 QCpython-1.0.3/QCpy/qubit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.718928 QCpython-1.0.3/QCpython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33292 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 21:25:58.000000 QCpython-1.0.3/QCpython.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32500 2023-04-30 21:25:46.000000 QCpython-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-30 21:25:58.726928 QCpython-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-30 21:25:46.000000 QCpython-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.718928 QCpython-1.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.722928 QCpython-1.0.3/test/quantumcircuit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_03.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_04.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_05.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_06.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_08.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_09.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_11.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_12.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_14.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_15.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_19.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumcircuit/test_qc_20.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.726928 QCpython-1.0.3/test/quantumgate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_01.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_02.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_03.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_04.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_05.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_06.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_07.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_08.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_09.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_10.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_11.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_12.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_13.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_14.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_15.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_16.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_17.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_18.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_19.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_20.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_21.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_22.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/quantumgate/test_qg_23.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:58.726928 QCpython-1.0.3/test/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:25:46.000000 QCpython-1.0.3/test/visualizer/__init__.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.452844 qcpython-1.1.0/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1064 2023-02-24 06:22:36.000000 qcpython-1.1.0/LICENSE.txt
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)    34723 2023-07-25 03:25:22.452844 qcpython-1.1.0/PKG-INFO
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)    33871 2023-07-25 03:24:44.000000 qcpython-1.1.0/README.md
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/qcpy/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      147 2023-07-25 02:54:56.000000 qcpython-1.1.0/qcpy/__init__.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/qcpy/circuitdrawing/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      157 2023-02-26 06:10:12.000000 qcpython-1.1.0/qcpy/circuitdrawing/__init__.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1447 2023-02-26 06:10:12.000000 qcpython-1.1.0/qcpy/circuitdrawing/circuitdrawing.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      626 2023-07-23 04:40:02.000000 qcpython-1.1.0/qcpy/circuitdrawing/gateformatting.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      473 2023-02-26 06:10:12.000000 qcpython-1.1.0/qcpy/circuitdrawing/quantumgatedraw.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/qcpy/core/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)       63 2023-07-25 02:56:30.000000 qcpython-1.1.0/qcpy/core/__init__.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)    37902 2023-07-25 02:29:44.000000 qcpython-1.1.0/qcpy/core/quantumcircuit.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/qcpy/core/tools/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      102 2023-03-06 04:04:18.000000 qcpython-1.1.0/qcpy/core/tools/__init__.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1959 2023-03-06 04:04:18.000000 qcpython-1.1.0/qcpy/core/tools/amplitude.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      878 2023-03-06 04:04:18.000000 qcpython-1.1.0/qcpy/core/tools/measure.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1474 2023-07-23 06:46:59.000000 qcpython-1.1.0/qcpy/core/tools/phaseangle.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1665 2023-03-06 04:04:18.000000 qcpython-1.1.0/qcpy/core/tools/probabilities.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/qcpy/quantumgate/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      135 2023-02-26 06:10:12.000000 qcpython-1.1.0/qcpy/quantumgate/__init__.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     6637 2023-07-23 19:10:32.000000 qcpython-1.1.0/qcpy/quantumgate/multiqubit.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     8006 2023-07-23 04:38:22.000000 qcpython-1.1.0/qcpy/quantumgate/singlequbit.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1245 2023-07-23 07:06:52.000000 qcpython-1.1.0/qcpy/qubit.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/qcpy/visualizer/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      507 2023-07-23 06:55:41.000000 qcpython-1.1.0/qcpy/visualizer/__init__.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     3543 2023-07-23 07:08:05.000000 qcpython-1.1.0/qcpy/visualizer/bloch.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     2519 2023-07-23 07:08:05.000000 qcpython-1.1.0/qcpy/visualizer/probability.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     9803 2023-07-23 19:55:02.000000 qcpython-1.1.0/qcpy/visualizer/qsphere.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     3840 2023-07-23 07:08:05.000000 qcpython-1.1.0/qcpy/visualizer/statevector.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/qcpy/visualizer/tools/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)        0 2023-02-24 06:22:36.000000 qcpython-1.1.0/qcpy/visualizer/tools/__init__.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      951 2023-07-23 06:49:41.000000 qcpython-1.1.0/qcpy/visualizer/tools/graph.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1694 2023-07-23 06:49:28.000000 qcpython-1.1.0/qcpy/visualizer/tools/sphere.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/qcpython.egg-info/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)    34723 2023-07-25 03:25:22.000000 qcpython-1.1.0/qcpython.egg-info/PKG-INFO
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     2404 2023-07-25 03:25:22.000000 qcpython-1.1.0/qcpython.egg-info/SOURCES.txt
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)        1 2023-07-25 03:25:22.000000 qcpython-1.1.0/qcpython.egg-info/dependency_links.txt
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)       51 2023-07-25 03:25:22.000000 qcpython-1.1.0/qcpython.egg-info/requires.txt
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)       10 2023-07-25 03:25:22.000000 qcpython-1.1.0/qcpython.egg-info/top_level.txt
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      837 2023-07-25 03:25:22.452844 qcpython-1.1.0/setup.cfg
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1179 2023-07-25 03:25:02.000000 qcpython-1.1.0/setup.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/test/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)        0 2023-02-24 06:22:36.000000 qcpython-1.1.0/test/__init__.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.442844 qcpython-1.1.0/test/quantumcircuit/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)        0 2023-02-24 06:22:36.000000 qcpython-1.1.0/test/quantumcircuit/__init__.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      900 2023-07-24 20:38:41.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_01.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1089 2023-07-24 20:39:26.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_02.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1243 2023-07-24 20:39:43.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_03.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      876 2023-07-24 20:39:50.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_04.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      880 2023-07-24 20:39:56.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_05.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      924 2023-07-24 20:40:03.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_06.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      956 2023-07-24 20:42:07.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_07.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1268 2023-07-24 20:40:18.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_08.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1280 2023-07-24 20:40:24.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_09.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1209 2023-07-24 20:40:36.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_10.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1276 2023-07-24 20:40:43.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_11.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      897 2023-07-24 20:40:49.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_12.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      943 2023-07-24 20:40:55.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_13.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1256 2023-07-24 20:41:02.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_14.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1259 2023-07-24 20:41:09.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_15.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1454 2023-07-24 20:41:12.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_16.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1110 2023-07-24 20:41:18.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_17.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)     1124 2023-07-24 20:41:24.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_18.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      979 2023-07-24 20:41:36.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_19.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      987 2023-07-24 20:41:46.000000 qcpython-1.1.0/test/quantumcircuit/test_qc_20.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.452844 qcpython-1.1.0/test/quantumgate/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)        0 2023-02-24 06:22:36.000000 qcpython-1.1.0/test/quantumgate/__init__.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      243 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_01.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      237 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_02.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      237 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_03.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      238 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_04.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      263 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_05.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      681 2023-07-23 19:12:19.000000 qcpython-1.1.0/test/quantumgate/test_qg_06.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      355 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_07.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      804 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_08.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      256 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_09.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      222 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_10.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      228 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_11.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      244 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_12.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      250 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_13.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      283 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_14.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      311 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_15.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      298 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_16.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      226 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_17.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      232 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_18.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      529 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_19.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      772 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_20.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      776 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_21.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      371 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_22.py
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)      350 2023-07-23 04:40:02.000000 qcpython-1.1.0/test/quantumgate/test_qg_23.py
+drwxr-xr-x   0 bfreeze   (1000) bfreeze   (1000)        0 2023-07-25 03:25:22.452844 qcpython-1.1.0/test/visualizer/
+-rw-r--r--   0 bfreeze   (1000) bfreeze   (1000)        0 2023-02-24 06:22:36.000000 qcpython-1.1.0/test/visualizer/__init__.py
```

### Comparing `QCpython-1.0.3/LICENSE.txt` & `qcpython-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QCpython-1.0.3/PKG-INFO` & `qcpython-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,746 +1,900 @@
 Metadata-Version: 2.1
-Name: QCpython
-Version: 1.0.3
-Summary: QCpy is a comprehensive and user-friendly library for quantum computing, providing a wide range of functionality for quantum algorithms and quantum circuits. It is built on using open-source libraries NumPy and Matplotlib; compatible with Python 3.
+Name: qcpython
+Version: 1.1.0
+Summary: QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing.
 Home-page: https://github.com/QCpython/QCpy
 Author: Brennan Freeze, Paris Osuch, Aundre Barras, Soren Richenberg, Suzanne Rivoire
 Author-email: freezebrennan@gmail.com, osuch@sonoma.edu, barras@sonoma.edu, richenbe@sonoma.edu, rivoire@sonoma.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # README.md
 
 # QCpy - A Quantum Computing Library for Python
 
-QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing (QC).
+QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing.
 
 You can download the package using pip:
 
 ```txt
-pip install QCpython
+pip install qcpython
 ```
-
-## Recommended Resources on Quantum Computing:
-
-- [Microsoft’s Linear Algebra for Quantum Computing](https://learn.microsoft.com/en-us/azure/quantum/overview-algebra-for-quantum-computing)
-- [IBM’s Quantum Computing: a field guide](https://quantum-computing.ibm.com/composer/docs/iqx/guide/)
-- [Wikipedia: Quantum Computing](https://en.wikipedia.org/wiki/Quantum_computing)
-
 ---
 
-# Qubits
+# Qubit
 
-> ## *class* QCpy.`Qubit`(*initial_state=’z’*)
+> ## qcpy.`qubit`(*initial_state=’z’*)
 
 *Object representation of a qubit.*
 
 ### Parameters:
 
-`initial_state (chr)` - Character input for starting direction in the *x*, *y*, or *z* axis.
+`initial_state (chr)` default: `z` - Character input for starting direction in the *x*, *y*, or *z* axis.
 
 ### Attributes:
 
-`state (numpy.ndarray)` -  current state of qubit in matrix representation.
+`None`
+
+### Example:
+
+```python
+from qcpy import qubit
 
+qx = qubit(initial_state = 'x')
+qy = qubit(initial_state = 'y')
+qz = qubit(initial_state = 'z')
+print("qx:\n", qx)
+print("qy:\n", qy)
+print("qz:\n", qz)
+
+
+# qx:
+#  [[0.70710677+0.j]
+#  [0.70710677+0.j]]
+# qy:
+#  [[0.70710677+0.j]
+#  [0.+0.70710677j]]
+# qz:
+#  [[1.+0.j]
+#  [0.+0.j]]
+```
 ---
 
 # Quantum Gates
 
-> ## *class* QC.QuantumGate.`Identity`()
+> ## quantumgate.`identity`()
 
 *Gate that does not modify the quantum state.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Identity gate.
-
 ```python
-Identity.matrix = [1+0j, 0+0j], 
-	          [0+0j, 1+0j]
+identity=[1+0j, 0+0j], 
+         [0+0j, 1+0j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`PauliX`()
+```python
+from qcpy import identity 
+
+print(identity())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j]]
+```
+> ## quantumgate.`paulix`()
 
 *Quantum equivalent of the NOT gate in classical computing with respect to the standard basis |0>, |1>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-X gate.
-
 ```python
-PauliX.matrix = [0+0j, 1+0j], 
-	        [1+0j, 0+0j]
+PauliX = [0+0j, 1+0j], 
+	 [1+0j, 0+0j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`PauliY`()
+```python
+from qcpy import paulix
+
+print(paulix())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j]]
+```
+> ## quantumgate.`pauliy`()
 
 *Rotation around y-axis of the bloch sphere by π radiains, mapping |0> to i|1> and |1> to -i|0>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-Y gate.
-
 ```python
-PauliY.matrix = [0+0j, 0-1j],
-                [0+1j, 0+0j]
+PauliY = [0+0j, 0-1j],
+         [0+1j, 0+0j]
 ```
+### Example:
+
+```python
+from qcpy import pauliy
+
+print(pauliy())
 
-> ## *class* QC.QuantumGate.`PauliZ`()
+# [[0+0j, 0-1j]
+#  [0+1j, 0+0j]]
+```
+> ## quantumgate.`pauliz`()
 
 *Rotation around z-axis of the bloch sphere by π radiains, mapping |1> to -|1>; known as the phase-flip.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-Z gate.
-
 ```python
-PauliZ.matrix = [1+0j, 0+0j], 
-                [0+0j, -1+0j]
+PauliZ = [1+0j, 0+0j], 
+         [0+0j, -1+0j]
 ```
+### Example:
+
+```python
+from qcpy import pauliz
 
-> ## *class* QC.QuantumGate.`Hadamard`()
+print(pauliz())
+
+# [[1+0j, 0+0j], 
+#  [0+0j, -1+0j]]
+```
+> ## quantumgate.`hadamard`()
 
 *Maps the basis states |0> to |+> and |1> to |->, creating a superposition state if given a computation basis state.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Hadamard gate.
-
 ```python
-Hadamard.matrix = ([1,  1] 
-                   [1, -1]) * (1/sqrt(2))
+Hadamard = [1,  1] 
+           [1, -1] * (1/sqrt(2))
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`CNot`(*inverse=False*)
+```python
+from qcpy import hadamard
 
-*Controlled gate acts on two or more qubits, performing the NOT operation of the target qubit only if the control qubits are |1>, can act as a quantum regiester and is used to entangle and disentangle Bell states.*
+print(hadamard())
 
-### Parameters:
+# [[ 0.70710677+0.j  0.70710677+0.j]
+#  [ 0.70710677+0.j -0.70710677+0.j]]
+```
+> ## quantumgate.`cnot`(*little_endian=False*)
 
-`inverse (bool)` - if the gate is an inverse, with the target being above the control.
+*Controlled gate acts on two or more qubits, performing the NOT operation of the target qubit only if the control qubits are |1>, can act as a quantum regiester and is used to entangle and disentangle Bell states.*
 
-### Attributes:
+### Parameters:
 
-`matrix (np.ndarray)` - matrix representation of CNOT gate.
+`little_endian (bool)` - if the gate is an inverse, with the target being above the control.
 
 ```python
 # regular
-CNot.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j]
-# inverse
-CNot.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j] 
+CNot = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j]
+# little_endian = True
+CNot = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j] 
 ```
+### Example:
+
+```python
+from qcpy import cnot
+
+print(cnot())
+
+# [[1.+0.j 0.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 0.+0.j 0.+0.j 1.+0.j]
+#  [0.+0.j 0.+0.j 1.+0.j 0.+0.j]]
 
-> ## *class* QC.QuantumGate.`Swap`()
+# [[1.+0.j 0.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 0.+0.j 0.+0.j 1.+0.j]
+#  [0.+0.j 0.+0.j 1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j 0.+0.j 0.+0.j]]
+```
+> ## quantumgate.`swap`()
 
 *Swaps two qubits, with respect to the basis |00>, |01>, |10>, and |11>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of SWAP gate.
-
 ```python
-Swap.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j]
+Swap = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j]
 ```
+### Example:
+
+```python
+from qcpy import swap
 
-> ## *class* QC.QuantumGate.`Toffoli`()
+print(swap())
+
+# [1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j]
+```
+> ## quantumgate.`toffoli`()
 
 *Universal reversible logic gate, known as the “controlled-controlled-NOT” gate; if the two control bits are set to 1, it will invert the target.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Toffoli gate.
-
 ```python
-Toffoli.matrix = [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+Toffoli = [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
 ```
+### Example:
+
+```python
+from qcpy import toffoli
 
-> ## *class* QC.QuantumGate.`Phase`(*theta=numpy.pi/2*)
+print(toffoli())
+
+# [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+```
+> ## quantumgate.`phase`(*theta=numpy.pi/2*)
 
 *Applies a rotation of theta around the z-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around z-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Phase gate.
-
 ```python
-Phase.matrix = [1+0j, 0+0j],
-	       [0+0j, numpy.exp(0+1j * theta)]
+Phase = [1+0j, 0+0j],
+	[0+0j, numpy.exp(0+1j * theta)]
 ```
+### Example:
+
+```python
+from qcpy import phase
 
-> ## *class* QC.QuantumGate.`S`()
+print(phase())
+
+# [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+```
+> ## quantumgate.`s`()
 
 *Equivalent to a pi/2 rotation around the z-axis.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of S gate.
-
 ```python
 S.matrix = [1+0j, 0+0j],
            [0+0j, 0+1j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Sdg`()
+```python
+from qcpy import s
+
+print(s())
+
+# [1+0j, 0+0j],
+# [0+0j, 0+1j]
+```
+> ## quantumgate.`sdg`()
 
 *Inverse of S gate; a -pi/2 rotation around the z-axis.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an inverse S gate.
-
 ```python
 Sdg.matrix = [1+0j, 0+0j],
              [0+0j, 0-1j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`T`()
+```python
+from qcpy import sdg
+
+print(sdg())
+
+# [1+0j, 0+0j],
+# [0+0j, 0-1j]
+```
+> ## quantumgate.`t`()
 
 *Square of S gate; where T = S^2.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a T gate.
-
 ```python
 T.matrix = [1+0j, 0+0j],
            [0+0j, numpy.exp((0+1j * numpy.pi) / 4)]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Tdg`()
+```python
+from qcpy import t
+
+print(t())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 0.70710677+0.70710677j]]
+```
+> ## quantumgate.`tdg`()
 
 *Inverse of T gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a inverse of T gate.
-
 ```python
-Tdg.matrix = [1+0j, 0+0j],
-             [0+0j, numpy.exp((0-1j * numpy.pi) / 4)]
+Tdg = [1+0j, 0+0j],
+      [0+0j, numpy.exp((0-1j * numpy.pi) / 4)]
 ```
+### Example:
+
+```python
+from qcpy import tdg
 
-> ## *class* QC.QuantumGate.`Rz`(*theta=numpy.pi/2*)
+print(tdg())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 0.70710677-0.70710677j]]
+```
+> ## quantumgate.`rz`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the z-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around z-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rz gate.
-
 ```python
-Rz.matrix = [numpy.exp((0-1j * (theta / 2))), 0+0j],
-            [0+0j, numpy.exp(0+1j * (theta / 2))]
+Rz = [numpy.exp((0-1j * (theta / 2))), 0+0j],
+     [0+0j, numpy.exp(0+1j * (theta / 2))]
 ```
 
-> ## *class* QC.QuantumGate.`Rx`(*theta=numpy.pi/2*)
+> ## quantumgate.`rx`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the x-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around x-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rx gate.
-
 ```python
-Rx.matrix = [numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2)],
-            [0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2)]
+Rx = [numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2)],
+     [0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2)]
 ```
+### Example:
+
+```python
+from qcpy import rx
 
-> ## *class* QC.QuantumGate.`Ry`(*theta=numpy.pi/2*)
+print(rx())
+
+# [[0.70710677+0.j 0.-0.70710677j]
+#  [0.-0.70710677j 0.70710677+0.j]]
+```
+> ## quantumgate.`ry`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the y-axis.*
 
 ### Parameters:
 
 `theta (float)`default: `numpy.pi/2` -  angle of rotation around y-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Ry gate.
-
 ```python
-Ry.matrix = [numpy.cos(theta / 2), -1 * numpy.sin(theta / 2)],
-            [numpy.sin(theta / 2), numpy.cos(theta / 2)]
+Ry = [numpy.cos(theta / 2), -1 * numpy.sin(theta / 2)],
+     [numpy.sin(theta / 2), numpy.cos(theta / 2)]
 ```
+### Example:
+
+```python
+from qcpy import ry
 
-> ## *class* QC.QuantumGate.`Sx`()
+print(ry())
+
+# [[ 0.70710677+0.j -0.70710677+0.j]
+#  [ 0.70710677+0.j  0.70710677+0.j]]
+```
+> ## quantumgate.`sx`()
 
 *Rotation around the x-axis by 90 degrees in the counter-clockwise direction. Also known as the “square-root X gate” due to the fact that applying the SX gate twice results in an X gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Sx gate.
-
 ```python
-Sx.matrix = [1+1j, 1-1j], 
-            [1-1j, 1+1j]]) * (1 / 2)
+Sx = [1+1j, 1-1j], 
+     [1-1j, 1+1j] * (1 / 2)
 ```
+### Example:
+
+```python
+from qcpy import sx
 
-> ## *class* QC.QuantumGate.`Sxdg`()
+print(sx())
+
+# [[0.5+0.5j 0.5-0.5j]
+#  [0.5-0.5j 0.5+0.5j]]
+```
+> ## quantumgate.`sxdg`()
 
 *Inverse of the Sx gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an inverse Sx gate.
-
 ```python
-Sxdg.matrix = [1-1j, 1+1j], 
-              [1+1j, 1-1j]]) * (1 / 2)
+Sxdg = [1-1j, 1+1j], 
+       [1+1j, 1-1j] * (1 / 2)
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`U`(*theta=numpy.pi/2, phi=numpy.pi/2, lmbda=numpy.pi/2*)
+```python
+from qcpy import sxdg
+
+print(sxdg())
+
+# [[0.5-0.5j 0.5+0.5j]
+#  [0.5+0.5j 0.5-0.5j]]
+```
+> ## quantumgate.`u`(*theta=numpy.pi/2, phi=numpy.pi/2, lmbda=numpy.pi/2*)
 
 *Rotation of qubit with respect to theta, phi, and lambda, in Euler angles.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around Euler angle theta.
 
 `phi (float)` default: `numpy.pi/2` -  angle of rotation around Euler angle phi.
 
 `lmbda (float)` default: `numpy.pi/2` -  angle of rotation around Eulear angle lambda.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a U gate.
-
 ```python
 U.matrix = [numpy.cos(theta / 2), -1 * numpy.exp(0+1j * lmbda) * numpy.sin(theta / 2)], 
            [numpy.exp(0+1j * phi) * numpy.sin(theta / 2), numpy.exp(0+1j * (lmbda + phi)) * numpy.cos(theta / 2)]]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Rxx`(*theta=numpy.pi/2*)
+```python
+from qcpy import u
+
+print(u())
+
+# [[0.7071+0.j -0.-0.7071j]
+#  [0.+0.7071j -0.7071+0.j]]
+```
+> ## quantumgate.`rxx`(*theta=numpy.pi/2*)
 
 *Rotation about XX, maximally entangling at theta = pi/2.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around XX.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rxx gate.
-
 ```python
 Rxx.matrix = [numpy.cos(theta / 2), 0+0j, 0+0j, 0-1j * numpy.sin(theta / 2)],
              [0+0j, numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2), 0+0j],
              [0+0j, 0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2), 0+0j],
              [0-1j * numpy.sin(theta / 2), 0+0j, 0+0j, numpy.cos(theta / 2)]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Rzz`(*theta=numpy.pi/2*)
+```python
+from qcpy import rxx
+
+print(rxx())
+
+# [[0.70710677+0.j 0+0.j 0+0.j 0-0.70710677j]
+#  [0+0.j 0.70710677+0.j 0-0.70710677j 0+0.j]
+#  [0+0.j 0-0.70710677j 0.70710677+0.j 0+0.j]
+#  [0-0.70710677j 0+0.j 0.+0.j 0.70710677+0.j]]
+```
+> ## quantumgate.`rzz`(*theta=numpy.pi/2*)
 
 *Rotation about ZZ, maximally entangling at theta = pi/2.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around ZZ.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rzz gate.
-
 ```python
 Rzz.matrix = [numpy.exp(0-1j * (theta / 2)), 0+0j, 0+0j, 0+0j],
              [0+0j, numpy.exp(0+1j * (theta / 2)), 0+0j, 0+0j],
              [0+0j, 0+0j, numpy.exp(0+1j * (theta / 2)), 0+0j],
              [0+0j, 0+0j, 0+0j, numpy.exp(0-1j * (theta / 2))]
 ```
+### Example:
+
+```python
+from qcpy import rzz
 
-> ## *class* QC.QuantumGate.`Cr`(*theta=numpy.pi/2*)
+print(rzz())
+
+# [[0.70710677-0.70710677j 0+0.j 0+0.jn 0+0.j]
+#  [0+0.j 0.70710677+0.70710677j 0+0.j 0+0.j]
+#  [0+0.j 0+0.j 0.70710677+0.70710677j 0+0.j]
+#  [0+0.j 0+0.j 0+0.j 0.70710677-0.70710677j]]
+```
+> ## quantumgate.`cr`(*theta=numpy.pi/2*)
 
 *Controlled phase shift rotation in theta radians; generalization of Cz gate.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation in theta radians.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Cr gate.
-
 ```python
-Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-            [0+0j, 1+0j, 0+0j, 0+0j],
-            [0+0j, 0+0j, 1+0j, 0+0j],
-            [0+0j, 0+0j, 0+0j, numpy.exp(theta * 0+1j)]
+Cr = [1+0j, 0+0j, 0+0j, 0+0j],
+     [0+0j, 1+0j, 0+0j, 0+0j],
+     [0+0j, 0+0j, 1+0j, 0+0j],
+     [0+0j, 0+0j, 0+0j, exp(theta * 0+1j)]
 ```
+### Example:
+
+```python
+from qcpy import cr
 
-> ## *class* QC.QuantumGate.`Cz`(*theta=numpy.pi/2*)
+print(cr())
+
+# [[1+0.j 0+0.j 0+0.j 0+0.j]
+#  [0+0.j 1+0.j 0+0.j 0+0.j]
+#  [0+0.j 0+0.j 1+0.j 0+0.j]
+#  [0+0.j 0+0.j 0+0.j 0.5403023+0.84147096j]]
+```
+> ## quantumgate.`cz`(*theta=numpy.pi/2*)
 
 *Controlled phase shift rotation in theta radians.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation in theta radians.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Cz gate.
+```python
+Cz = [1+0j, 0+0j, 0+0j, 0+0j],
+     [0+0j, 1+0j, 0+0j, 0+0j],
+     [0+0j, 0+0j, 1+0j, 0+0j],
+     [0+0j, 0+0j, 0+0j, -1+0j]
+```
+### Example:
 
 ```python
-Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-            [0+0j, 1+0j, 0+0j, 0+0j],
-            [0+0j, 0+0j, 1+0j, 0+0j],
-            [0+0j, 0+0j, 0+0j, -1+0j]
+from qcpy import cz
+
+print(cz())
+
+# [[ 1.+0.j  0.+0.j  0.+0.j  0.+0.j]
+#  [ 0.+0.j  1.+0.j  0.+0.j  0.+0.j]
+#  [ 0.+0.j  0.+0.j  1.+0.j  0.+0.j]
+#  [ 0.+0.j  0.+0.j  0.+0.j -1.+0.j]]
 ```
 ---
 # Quantum Circuit
-> ## *class* QCpy.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
+> ## *class* qcpy.`quantumcircuit`(*qubits: int*, *little_endian: bool=False*, *prep: char='z'*)
 
 *Quantum circuit that represents the state of a quantum system and performs operations on select qubits.*
 
 ### Parameters:
 
 `qubits (int)` - number of qubits in the circuit.
 
 `little_endian (bool)` default: `False` - order of qubits and tensor products.
 
 `prep (char)` options: [`z`, `y`, `x`] - initial direction of the qubits' phase angle.
 
 ### Attributes:
 
-`None`
-
-> ## QuantumCircuit.`circuit`()
-
-*Dictionary representation of the circuit*
-
-### Parameters:
-
-`None`
-
-### Returns:
-
-`circuit (dict[int, list[str]])` - key: qubit; value: name of gate.
-
-### Example:
-
-```python
-from QCpy import QuantumCircuit
-
-qc = QuantumCircuit(2)
-
-qc.hadamard(0)
-qc.cnot(0, 1)
-qc.hadamard(0)
-
-print(qc.circuit())
+`state (numpy.ndarray)` -  current state of quantum circuit in matrix representation.
 
-# {0: ['hadamard', 'cnot_control', 'hadamard'], 
-#  1: ['cnot_target']}
-```
 
-> ## QuantumCircuit.`amplitude`(*round=3*)
+> ## quantumcircuit.`amplitude`(*round: int=3*)
 
 *Returns vector of all possible amplitudes for the quantum circuit*
 
 ### Parameters:
 
 `round (int)` - rounding the amplitude to the nearest `round`
 
 ### Returns:
 
 `amplitude (numpy.ndarray[float16])` - amplitude of the quantum circuit.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
-qc.hadamard(0)
+qc.h(0)
 
 print(qc.amplitude())
 
 # [[0.5]
 # [0.5]
 # [0.5]
 # [0.5]]
 ```
 
-> ## QuantumCircuit.`phaseAngle`(*round=2*, *radian=True*)
+> ## quantumcircuit.`phaseangle`(*round: int=2*, *radian: bool=True*)
 
 *Calculates possible phase angles for the quantum circuit*
 
 ### Parameters:
 
-`round (int)` - rounding the amplitude to the nearest `round`
+`round (int)` - round phase angle for readability.
 
 `radian (bool)` - whether or not the values are in radians or degrees.
 
 ### Returns:
 
 `phase_angle (numpy.ndarray)` - array of qubit's phase angle.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.phaseAngle())
+print(qc.phaseangle())
 
 # [[0.        ]
 # [0.         ]
 # [0.         ]
 # [3.14159265]]
 ```
 
-> ## QuantumCircuit.`state`(*round=3*)
+> ## quantumcircuit.`state`
 
 *Returns state of the quantum circuit.*
 
 ### Parameters:
 
-`round (int)` - rounding the state to the nearest `round`
+`None`
 
 ### Returns:
 
-`_state (numpy.ndarray)` - array of quantum circuit's state.
+`state (numpy.ndarray)` - array of quantum circuit's state.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`circuitQueue()`
+> ## quantumcircuit.`flatten(round: int=3)`
+
+*Returns state of the quantum circuit in a 1D array.*
+
+### Parameters:
+
+`round (int)` - round state for readability.
+
+### Returns:
+
+`state (numpy.ndarray)` - array of quantum circuit's state.
+
+### Example:
+
+```python
+from qcpy import quantumcircuit
+
+qc = quantumcircuit(2)
+
+qc.h(0)
+qc.cnot(0, 1)
+
+print(qc.flatten())
+
+# [0.707+0.j 0.   +0.j 0.   +0.j 0.707+0.j]
+```
+
+> ## quantumcircuit.`circuitqueue()`
 
 *Returns queue of gates on quantum circuit.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 `queue (list)` - list of gates queued on quantum circuit.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
 qc = QuantumCircuit(4)
 
 qc.x(0)
 qc.x(1)
 qc.x(2)
 qc.rc3x(0, 1, 2, 3)
 
-print(qc.circuitQueue())
+print(qc.circuitqueue())
 
 # [('X', 0), ('X', 1), ('X', 2), ('U', 3), ('U', 3), ('cnot', 2, # 3), ('U', 3), ('U', 3), ('swap', 2, 3), ('swap', 1, 2), 
 # ('swap', 1, 2), ('swap', 2, 3), ('cnot', 0, 3), ('U', 3),
 # ('swap', 2, 3), ('swap', 2, 3), ('cnot', 1, 3), ('U', 3), 
 # ('swap', 2, 3), ('swap', 1, 2), ('swap', 1, 2), ('swap', 2, 
 # 3), ('cnot', 0, 3), ('U', 3), ('swap', 2, 3), ('swap', 2, 3),
 #  ('cnot', 1, 3), ('U', 3), ('U', 3), ('U', 3), ('cnot', 2, 3),
 #  ('U', 3), ('U', 3), ('rc3x', 0, 1, 2, 3)]
 ```
 
-> ## QuantumCircuit.`probabilities`(*round=3*)
+> ## quantumcircuit.`probabilities`(*show_percent: bool=False*, *show_bit=-1*, *round: int=3*)
 
 *Returns probabilitiy of the qubits within the quantum circuit.*
 
 ### Parameters:
 
-`round (int)` - rounding the probabilities to the nearest `round`
+`show_percent (bool)` - convert probability to be shown in percentage.
+
+`show_bit (int or str)` - get the probability of a single bit with a given string of binary or a integer.
+
+`round (int)` - rounding the probabilities to the nearest `round`.
 
 ### Returns:
 
 `prob_matrix (numpy.ndarray)` - array of quantum circuit's probabilities.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cnot(0, 1)
 
 print(qc.probabilities())
 
 # [0.5 0.  0.  0.5]
 ```
 
-> ## QuantumCircuit.`measure`()
+> ## quantumcircuit.`measure`()
 
 *Collapses the state based on the quantum circuit's probabilities.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 
 `final_state (numpy.ndarray)` - array of quantum circuit's measurement.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
 
 print(qc.measure())
 
-# ~Results may vary~
 # 00
 ```
 
-> ## QuantumCircuit.`reverse`()
+> ## quantumcircuit.`reverse`()
 
 *Reverses the quantum circuit's values.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.state())
+print(qc.state)
 
 qc.reverse()
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
  
 # [[0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
-> ## QuantumCircuit.`toffoli`(*control_1*, *control_2*, *target*)
+> ## quantumcircuit.`toffoli`(*control_1: int*, *control_2: int*, *target: int*)
 
 *A 3-qubit quantum gate that takes in two control qubits and one target qubit.*
 
 ### Parameters:
 
 `control_1 (int)` - first control qubit.
 
@@ -751,37 +905,37 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
 qc.toffoli(0,1,2)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j]
 # [0. +0.j]
 # [0.5+0.j]
 # [0. +0.j]
 # [0.5+0.j]
 # [0. +0.j]
 # [0. +0.j]
 # [0.5+0.j]]
 ```
 
-> ## QuantumCircuit.`rccx`(*control_1*, *control_2*, *target*)
+> ## quantumcircuit.`rccx`(*control_1*, *control_2*, *target*)
 
 *A 3-qubit quantum gate that takes in two control qubits and one target qubit.*
 
 ### Parameters:
 
 `control_1 (int)` - first control qubit.
 
@@ -792,68 +946,68 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(3)
+from qcpy import quantumcircuit
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
 qc.rccx(0,1,2)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.5-0.j ]
 # [ 0. +0.j ]
 # [ 0.5-0.j ]
 # [ 0. +0.j ]
 # [ 0.5-0.j ]
 # [ 0. +0.j ]
 # [-0. +0.j ]
 # [ 0. +0.5j]]
 ```
 
-> ## QuantumCircuit.`rc3x`(*a*, *b*, *c*, *d*)
+> ## quantumcircuit.`rc3x`(*qubit_1: int*, *qubit_2: int*, *qubit_3: int*, *qubit_4: int*)
 
 *A 4-qubit quantum gate that takes in 4 unique qubits.*
 
 ### Parameters:
 
-`a (int)` - first input qubit.
+`qubit_1 (int)` - first input qubit.
 
-`b (int)` - second input qubit.
+`qubit_2 (int)` - second input qubit.
 
-`c (int)` - third input qubit.
+`qubit_3 (int)` - third input qubit.
 
-`d (int)` - fourth input qubit.
+`qubit_4 (int)` - fourth input qubit.
 
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(4)
+from qcpy import quantumcircuit
+qc = quantumcircuit(4)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
-qc.hadamard(2)
+qc.h(2)
 
-qc.rc3x(0,1,2)
+qc.rc3x(0,1,2,3)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
@@ -864,15 +1018,15 @@
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.   +0.354j]
 # [-0.   +0.j   ]
 # [ 0.   -0.j   ]
 # [-0.354+0.j   ]]
 ```
-> ## QuantumCircuit.`cnot`(*control*, *target*)
+> ## quantumcircuit.`cnot`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -881,30 +1035,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cnot(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`cr`(*control*, *target*)
+> ## quantumcircuit.`cr`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -913,31 +1067,31 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cr(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
 
-> ## QuantumCircuit.`cz`(*control*, *target*)
+> ## quantumcircuit.`cz`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -946,30 +1100,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cz(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`swap`(*qubit_1*, *qubit_2*)
+> ## quantumcircuit.`swap`(*qubit_1: int*, *qubit_2: int*)
 
 *A 2-qubit quantum gate that takes in 2 qubits to swap there properties.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit to swap.
 
@@ -978,30 +1132,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.swap(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`rxx`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rxx`(*qubit_1: int*, *qubit_2: int*, *theta: float=numpy.pi/2*)
 
 *A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit input.
 
@@ -1011,30 +1165,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rxx(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j ]
 # [0. -0.5j]
 # [0.5+0.j ]
 # [0. -0.5j]]
 ```
 
-> ## QuantumCircuit.`rzz`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rzz`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
 
 *A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit input.
 
@@ -1045,211 +1199,209 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rxx(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j ]
 # [0. -0.5j]
 # [0.5+0.j ]
 # [0. -0.5j]]
 ```
 
-> ## QuantumCircuit.`customControlPhase`(*control*, *target*, *custom_matrix*)
+> ## quantumcircuit.`customcontrolled`(*control: int*, *target: int*, *custom_matrix: np.array*)
 
 *Used to insert single qubit based quantum gates to have a control qubit apart of it and committing to the quantum state.*
 
 ### Parameters:
 
 `control (int)` - control qubit for given matrix.
 
 `target (int)` - target qubit for given matrix.
 
-`custom_matrix (np.array)` -  matrix to be applied to the quantum circuit.
+`custom_matrix (np.array)` - (2,2) matrix to be applied to the quantum circuit.
 
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-
-from QCpy.QuantumGate import PauliX
+from qcpy import quantumcircuit, paulix
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.customControlPhase(0,1, PauliX().matrix)
+qc.customcontrolled(0,1, paulix())
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`identity`(*qubit*)
+> ## quantumcircuit.`i`(*qubit: int*)
 
 *Used to confirm value that a qubit is representing and does nothing to manipulate the value of such qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the identity gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.identity(0)
+qc.i(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[1.+0.j]
 # [0.+0.j]
 # [0.+0.j]
 # [0.+0.j]]
 ```
 
-> ## QuantumCircuit.`x`(*qubit*)
+> ## quantumcircuit.`x`(*qubit: int*)
 
 *Used to invert the value of what a qubit is representing.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-X gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.x(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [1.+0.j]
 # [0.+0.j]]
 ```
 
 
-> ## QuantumCircuit.`hadmard`(*qubit*)
+> ## quantumcircuit.`hadmard`(*qubit: int*)
 
 *Used to put a given qubit into superposition.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Hadamard gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`y`(*qubit*)
+> ## quantumcircuit.`y`(*qubit: int*)
 
 *Changes the state of a qubit by pi around the y-axis of a Bloch Sphere.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Y gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.y(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [0.+1.j]
 # [0.+0.j]]
 ```
 
 
-> ## QuantumCircuit.`z`(*qubit*)
+> ## quantumcircuit.`z`(*qubit: int*)
 
 *Changes the state of a qubit by pi around the z-axis of a Bloch Sphere.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Z gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.z(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.707+0.j]
 # [ 0.   +0.j]
 # [-0.707+0.j]
 # [ 0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`phase`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`phase`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *Commits to a rotation around the z-axis based off of the inputted theta value.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Phase gate be applied to the quantum wire.
 
@@ -1257,151 +1409,151 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.phase(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   +0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`s`(*qubit*)
+> ## quantumcircuit.`s`(*qubit: int*)
 
 *Is a Phase gate where the inputted theta value is given as a constant of theta = pi / 2.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Z gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.s(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   +0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`sdg`(*qubit*)
+> ## quantumcircuit.`sdg`(*qubit: int*)
 
 *Is a Phase gate and inverse of the S gate where the inputted theta value is given as a constant of theta = -pi / 2.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Sdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.sdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   -0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`t`(*qubit*)
+> ## quantumcircuit.`t`(*qubit: int*)
 
 *T gate is a special use case gate that in implemented from the P Gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the T gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.t(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j ]
 # [0.   +0.j ]
 # [0.5  +0.5j]
 # [0.   +0.j ]]
 ```
 
-> ## QuantumCircuit.`tdg`(*qubit*)
+> ## quantumcircuit.`tdg`(*qubit: int*)
 
 *Tdg gate is a special use case gate that in implemented from the P Gate and is the inverse of the T gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Tdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.tdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j ]
 # [0.   +0.j ]
 # [0.5  -0.5j]
 # [0.   +0.j ]]
 ```
 
-> ## QuantumCircuit.`rz`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rz`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RZ gate commits a rotation around the z-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Rz gate be applied to the quantum wire.
 
@@ -1409,31 +1561,31 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rz(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`ry`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`ry`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RY gate commits a rotation around the y-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Ry gate be applied to the quantum wire.
 
@@ -1441,29 +1593,29 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.ry(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`rx`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rx`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RX gate commits a rotation around the x-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Ry gate be applied to the quantum wire.
 
@@ -1471,85 +1623,85 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumCircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.rx(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   -0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`sx`(*qubit*)
+> ## quantumcircuit.`sx`(*qubit: int*)
 
 *SX gate is the square root of the Inverse gate (X, PauliX Gate).*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Sx gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.sx(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.5j]
 # [0. +0.j ]
 # [0.5-0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`sxdg`(*qubit*)
+> ## quantumcircuit.`sxdg`(*qubit: int*)
 
 *SXDG gate is the negative square root of the Inverse gate (X, PauliX Gate) and inverse of the SX gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the SXdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.sxdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`u`(*qubit*, *theta=numpy.pi/2*, *phi=numpy.pi/2*, *lmbda=numpy.pi/2*)
+> ## quantumcircuit.`u`(*qubit: int*, *theta: float=numpy.pi/2*, *phi: float=numpy.pi/2*, *lmbda: float=numpy.pi/2*)
 
 *U gate is given three inputs (theta, phi, and lambda) that allow the inputs to manipulate the base matrix to allow for the position of the enacted qubit around the bloch sphere representation.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the U gate be applied to the quantum wire.
 
@@ -1561,29 +1713,29 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.u(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`custom`(*qubit*, *custom_matrix*)
+> ## quantumcircuit.`custom`(*qubit: int*, *custom_matrix: np.array*)
 
 *Will take in a custom single qubit quantum gate and implement it on a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the U gate be applied to the quantum wire.
 
@@ -1591,47 +1743,45 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-
-from QCpy.QuantumGate import PauliX
+from qcpy import quantumcircuit, paulix
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.custom(0, PauliX().matrix)
+qc.custom(0, paulix())
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [1.+0.j]
 # [0.+0.j]]
 ```
 
 # Visualizer
 
 *A collection of classes to visualize the quantum circuit*
 
-> ## *class* QCpy.Visualizer.QSphere(*circuit*)
+> ## *class* qcpy.qsphere(*circuit*)
 
 *Visualizes the quantum circuit as a q-sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## QSphere.`makeSphere`(*path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## qsphere.`make`(*path: str="qsphere.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a Q-Sphere that plots a global visualization of the quantum states in a 3D global view*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1644,40 +1794,39 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, qsphere
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-sphere_ex = QSphere(qc)
-sphere_ex.makeSphere(save=False, show=True)
+sphere_ex = qsphere(qc)
+sphere_ex.make(save=False, show=True)
 ```
 
-> ## *class* QC.Visualizer.BlochSphere(*circuit*)
+> ## *class* qcpy.bloch(*circuit*)
 
 *Visualizes the quantum state of a single qubit as a sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## BlochSphere.`makeSphere`(*show_bit=0*, *path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## blochsphere.`make`(*show_bit: int=0*, *path: str="qsphere.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a Bloch Sphere that plots the quantum state of a single qubit in a 3D global view*
 
 ### Parameters:
 
 `show_bit (int)` - the qubit on the circuit to be visualized, initialized as the 0th bit
 
@@ -1692,40 +1841,39 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, bloch
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-sphere_ex = BlochSphere(qc)
-sphere_ex.makeSphere(show_bit=1, save=False, show=True)
+sphere_ex = bloch(qc)
+sphere_ex.make(show_bit=1, save=False, show=True)
 ```
 
-> ## *class* QCpy.Visualizer.StateVector(*circuit*)
+> ## *class* qcpy.statevector(*circuit*)
 
 *Visualizes the quantum circuit's quantum amplitutes using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## StateVector.`makeGraph`(*path="statevector.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## statevector.`make`(*path: str="statevector.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a graph that plots all the amplitudes of the qubits being measured*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1738,40 +1886,38 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, statevector
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-stateVector_ex = StateVector(qc)
-stateVector_ex.makeGraph(save=False, show=True)
+statevector(qc).make(save=False, show=True)
 ```
 
-> ## *class* QCpy.Visualizer.Probabilities(*circuit*)
+> ## *class* qcpy.probability(*circuit*)
 
 *Visualizes the quantum circuit's qubits probability of being measured using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## Probabilities.`makeGraph`(*path="probabilities.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## probability.`make`(*path: str="probability.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a graph that plots all the probabilities of the qubits being measured*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1784,19 +1930,17 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, probability
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-probabilities_ex = Probabilities(qc)
-probabilities_ex.makeGraph(save=False, show=True)
+probability(qc).make(save=False, show=True)
 ```
```

### Comparing `QCpython-1.0.3/QCpy/CircuitDrawing/circuitdrawing.py` & `qcpython-1.1.0/qcpy/circuitdrawing/circuitdrawing.py`

 * *Files identical despite different names*

### Comparing `QCpython-1.0.3/QCpy/CircuitDrawing/gateformatting.py` & `qcpython-1.1.0/qcpy/circuitdrawing/gateformatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..QuantumGate import *
+from ..quantumgate import *
 import sys
 
 class GateFormatting:
     def __init__(self):
         self.single_gates = []
         self.multi_gates = []
         current_module = sys.modules[__name__]
```

### Comparing `QCpython-1.0.3/QCpy/Core/quantumcircuit.py` & `qcpython-1.1.0/qcpy/core/quantumcircuit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-QuantumCircuit.py
+quantumcircuit.py
 """
-from ..qubit import Qubit
-from ..QuantumGate import *
-from .tools import amplitude, phaseAngle, probabilities, measure
+from ..qubit import qubit
+from ..quantumgate import *
+from .tools import amplitude, phaseangle, probabilities, measure
 import numpy as np
 
 """
 Purpose:
     To apply various quantum gates to a quantum wire given any amount of qubits. With this, to then return the state at any given moment
     alongside calculations to be examined upon.
 Methods:
@@ -88,78 +88,84 @@
     custom:
         Will take in a custom single qubit quantum gate and implement it on a qubit.
 --------
 
 """
 
 
-class QuantumCircuit:
+class quantumcircuit:
     def __init__(
             self,
             qubits: int,
             little_endian: bool = False,
             prep: chr = 'z'):
         """
-        Constructor that initilizes the quantum state in a vector given the number of qubits, endian positioning, and prepping of the qubits.
+        Constructor that initilizes the quantum state in a vector given the 
+        number of qubits, endian positioning, and prepping of the qubits.
         Args:
             qubits:
                 The number of qubits that will be within the circuit.
             little_endian:
-                a boolean variable to determine the placement of values, as well as determining the inverse of tensor product.
+                a boolean variable to determine the placement of values, as 
+                well as determining the inverse of tensor product.
             prep:
 
         ------
         Variables:
             _little_endian :
                 the number of qubits on the circuit
             _circuit_size :
                 all the states of the qubits on the circuit
             _probabilities :
                 an array of all the probabilities of the qubits being measured
             _percents :
-                the array of probabilities turned into an array of values adding to 100
+                the array of probabilities turned into an array of values adding
+                to 100
             _state :
                 the state values for the qubit being taken into consideration
         """
         if (qubits < 1):
             exit(
-                f"Error: QuantumCircuit().__init__ -- Quantum Circuit size must be 1 or more qubits. Current number of qubits is: {qubits}")
+                f"Error: QuantumCircuit().__init__ -- Quantum Circuit size must \
+                be 1 or more qubits. Current number of qubits is: {qubits}")
         # Determines if tensor calculation of __operator_matrix__ will be
         # reversed or not.
         self._little_endian = little_endian
         # Gets the number of qubits in play to store for later use.
         self._circuit_size = qubits
         # Makes tensored vector state of all qubits, and stores it within
         # _state to get a vector of [[1], [0], [0],....2^n].
-        self._state = Qubit(prep).state
+        
         # represent the circuit in dict
         self._circuit = []
+        self.state = qubit(prep)
         # increases the current vector size on the number of qubits - 1.
         for _ in range(qubits - 1):
             # _state is converted into the new lengthed vector based on the
             # kronocker product on the prepped qubit state.
-            self._state = np.kron(self._state, Qubit(prep).state)
+            self.state = np.kron(self.state, qubit(prep))
 
     def __operator_matrix__(
             self,
             gate_matrix: np.array,
             qubit: int,
             double: bool = False):
         """
-        Return a matrix from the tensor product calculation algorithm from any inplaced quantum gate.
+        Return a matrix from the tensor product calculation algorithm from any 
+        inplaced quantum gate.
         Params:
             gate_matrix: np.array
             qubit: integer
             double: boolean
         Returns:
             operator_matrix (numpy array):
                 Matrix after final calculation from the tensor product algorithm.
         """
         # Identity matrix is called.
-        i_matrix = Identity().matrix
+        i_matrix = identity()
         # gate queue for the computation
         gate_queue = [i_matrix for _ in range(self._circuit_size)]
         # replaces the placement of the identity gate at the qubit index with
         # the gate to get a correct calculation of final product
         gate_queue[qubit] = gate_matrix
         # if double is true, then CNOT, toffli, or any gate more than one qubit
         # is being asked to be implemented.
@@ -179,78 +185,69 @@
 
     def __controlled_phase_handler__(
             self,
             matrix_to_calculate: np.array,
             control_qubit: int,
             target_qubit: int):
         """
-        Calls a control_qubit and target_qubit represented as integers and will then correctly create a system of mathematic implementations of
-        any given controlled quantum gate.
+        Calls a control_qubit and target_qubit represented as integers and will 
+        then correctly create a system of mathematic implementations of any 
+        given controlled quantum gate.
         Params:
             matrix_to_calculate: np.array
             control_qubit: integer
             target_qubit: integer
         Returns:
             None.
         """
-        # inverse bool variable to determine if controlled gate representation
-        # needs to invert for confirming logic structuring.
+
         inverse = False
-        # checking to see if target_qubit is less than control_qubit indices:
+
         if (target_qubit < control_qubit):
             inverse = True
-        # create temp target_qubit variable
+
         temp_target_qubit = target_qubit
-        # call from QuantumGate and stores Hadamard gate into variable.
-        hadamard = Hadamard().matrix
-        # If target_qubit and control_qubit qubits are next to each other, then no further
-        # logic needs to be done and calls base system.
+
         if (abs(target_qubit - control_qubit) == 1):
-            # calls from called bool variable to see if the base CNOT matrix
-            # needs to be inverted to confirm correct logic structuring.
+
             if inverse:
-                # This is implemented due to other controlled gates not needing
-                # this implementation.
-                self._state = np.dot(
+
+                self.state = np.dot(
                     self.__operator_matrix__(
-                        hadamard, temp_target_qubit), self._state)
-                self._state = np.dot(
+                        hadamard(), temp_target_qubit), self.state)
+                
+                self.state = np.dot(
                     self.__operator_matrix__(
-                        hadamard, temp_target_qubit + 1), self._state)
-                # Call to _state to commit a dot product on the state to
-                # include the given gate of the method.
-                self._state = np.dot(
+                        hadamard(), temp_target_qubit + 1), self.state)
+
+                self.state = np.dot(
                     self.__operator_matrix__(
                         matrix_to_calculate,
                         temp_target_qubit,
                         double=True),
-                    self._state)
-                # This is implemented due to other controlled gates not needing
-                # this implementation.
+                    self.state)
 
-                self._state = np.dot(
+
+                self.state = np.dot(
                     self.__operator_matrix__(
-                        hadamard, temp_target_qubit), self._state)
-                self._state = np.dot(
+                        hadamard(), temp_target_qubit), self.state)
+                self.state = np.dot(
                     self.__operator_matrix__(
-                        hadamard, temp_target_qubit + 1), self._state)
-                # used for inversing all other gates that the target_qubit is less
-                # than the control_qubit to make it inversed in logic.
+                        hadamard(), temp_target_qubit + 1), self.state)
+
             else:
-                # if not inverse, what the controlled gate is will be enacted
-                # on the _state using dot product system.
-                self._state = np.dot(
+
+                self.state = np.dot(
                     self.__operator_matrix__(
                         matrix_to_calculate,
                         control_qubit,
                         double=True),
-                    self._state)
+                    self.state)
             return
-        # while the difference between the temp target_qubit and control_qubit is not -1 or
-        # 1.
+        
         while (abs(temp_target_qubit - control_qubit) != 1):
             # calls from called bool variable to see if the base CNOT matrix
             # needs to be inverted to confirm correct logic structuring.
             if inverse:
                 # This is implemented due to other controlled gates not needing
                 # this implementation.
                 self.swap(temp_target_qubit, temp_target_qubit + 1)
@@ -262,52 +259,52 @@
                 # update temp target_qubit position.
                 temp_target_qubit -= 1
         # calls from called bool variable to see if the base CNOT matrix needs
         # to be inverted to confirm correct logic structuring.
         if inverse:
             # will create inversed controlled_phase of what is inputted through here, determined if the inversed variable is marked true.
             # call hadamard gates on control_qubit and target_qubit variables.
-            self._state = np.dot(
+            self.state = np.dot(
                 self.__operator_matrix__(
-                    hadamard, temp_target_qubit), self._state)
-            self._state = np.dot(
+                    hadamard(), temp_target_qubit), self.state)
+            self.state = np.dot(
                 self.__operator_matrix__(
-                    hadamard,
+                    hadamard(),
                     temp_target_qubit + 1),
-                self._state)
+                self.state)
             # Call to _state to commit a dot product on the state to include
             # the given gate of the method.
-            self._state = np.dot(
+            self.state = np.dot(
                 self.__operator_matrix__(
                     matrix_to_calculate,
                     temp_target_qubit,
                     double=True),
-                self._state)
+                self.state)
             # This is implemented due to other controlled gates not needing
             # this implementation.
-            self._state = np.dot(
+            self.state = np.dot(
                 self.__operator_matrix__(
-                    hadamard, temp_target_qubit),
-                self._state)
-            self._state = np.dot(
+                    hadamard(), temp_target_qubit),
+                self.state)
+            self.state = np.dot(
                 self.__operator_matrix__(
-                    hadamard,
+                    hadamard(),
                     temp_target_qubit + 1),
-                self._state)
+                self.state)
             # used for inversing all other gates that the target_qubit is less than
             # the control_qubit to make it inversed in logic.
         else:
             # if not inverse, what the controlled gate is will be enacted on
             # the _state using dot product system.
-            self._state = np.dot(
+            self.state = np.dot(
                 self.__operator_matrix__(
                     matrix_to_calculate,
                     control_qubit,
                     double=True),
-                self._state)
+                self.state)
 
         # while the temp target_qubit does not equal the original target_qubit
         while (temp_target_qubit != target_qubit):
             if inverse:
                 # swap the temp target_qubit with the position closer to original
                 # target_qubit
                 self.swap(temp_target_qubit - 1, temp_target_qubit)
@@ -339,84 +336,84 @@
             show_bit: string or int
             round: int
             radian: bool
         Returns:
             np.around(statevector) (numpy array):
                 Matrix after final calculation from the sqrt(x^2 + y^2) algorithm for finding the amplitude.
         """
-        return amplitude(self._state, self._circuit_size, show_bit, round, radian)
+        return amplitude(self.state, self._circuit_size, show_bit, round, radian)
 
-    def phaseAngle(self, show_bit = -1, round: int = 3, radian: bool = True):
+    def phaseangle(self, show_bit = -1, round: int = 3, radian: bool = True):
         """
         Calculates an array of possible phase angles based off the state. Converts each value using np.angle() function then degree to radian.
         Params:
             show_bit: string or int
             round: int
             radian: bool
         Returns:
             np.around(phaseAngles) (numpy array):
                 Matrix after final calculation from the phase angle algorithm.
         """
-        return phaseAngle(self._state, self._circuit_size, show_bit, round, radian)
-
-    def state(self, round: int = 3):
-        """
-        Return a numpy array of the current quantum circuit.
-        Params:
-            round: int
-        Returns:
-            np.around(self._state) (numpy array):
-                vector of the given state rounded based off of the parameter
-        """
-        if (round < 0):
-            exit(
-                f"Error: QuantumCircuit().state -- round placement must be a value greater than 0.")
-        return np.around(self._state, decimals=round)
+        return phaseangle(self.state, self._circuit_size, show_bit, round, radian)
     
-    def circuitQueue(self):
+    def circuitqueue(self):
         return self._circuit
     
-    def circuitSize(self):
+    def circuitsize(self):
         return self._circuit_size
 
     def probabilities(self, show_percent: bool = False, show_bit: int = -1, round: int = 3):
         """
         Return a matrix with all the probabilities for each state
         Params:
             show_percent: bool
             show_bit: string or int
             round: int
         Returns:
             prob_matrix (numpy array):
                 matrix with all the weighted probabilities of being measured
         """
-        return probabilities(self._state, self._circuit_size, show_percent, show_bit, round)
+        return probabilities(self.state, self._circuit_size, show_percent, show_bit, round)
 
     def measure(self):
         """
         Collapes the quantum circuit into classical bits
         Params:
             None
         Returns:
             final_state (str):
                 the winning state displayed in classical bits notation
         """
         # randomly selects the measured state using self.probabilities()
-        return measure(self._state, self._circuit_size, self.probabilities())
+        return measure(self.state, self._circuit_size, self.probabilities())
 
     def reverse(self):
         """
         Reverses the quantum state.
         Params:
             None.
         Returns:
             None.
         """
         # reverses the entire state, useful for quantum algorithms.
-        self._state = self._state[::-1]
+        self.state = self.state[::-1]
+
+    def flatten(self, round: int = 3):
+        """
+        Return a numpy array of the current quantum circuit.
+        Params:
+            round: int
+        Returns:
+            np.around(self._state) (numpy array):
+                vector of the given state rounded based off of the parameter
+        """
+        if (round < 0):
+            exit(
+                f"Error: QuantumCircuit().state -- round placement must be a value greater than 0.")
+        return np.around(self.state, decimals=round).flatten()
     """
     Multiple qubit quantum gates
     """
 
     def toffoli(self, control_1: int, control_2: int, target_qubit: int):
         """
         A 3-qubit quantum gate that takes in two control_qubit qubits and one target_qubit qubit.
@@ -429,19 +426,19 @@
         """
         # If circuit is less than 3, means Toffoli gate cannot be allowed.
         if (self._circuit_size < 3):
             exit(
                 f"Error: QuantumCircuit().toffoli -- Quantum Circuit size must be 3 or more qubits. Current number of qubits is: {self._circuit_size}")
         # Calls of gates here represent the Toffoli matrix using other quantum
         # gates.
-        self.customControlPhase(control_2, target_qubit, Sx().matrix)
+        self.customcontrolled(control_2, target_qubit, sx())
         self.cnot(control_1, control_2)
-        self.customControlPhase(control_2, target_qubit, Sxdg().matrix)
+        self.customcontrolled(control_2, target_qubit, sxdg())
         self.cnot(control_1, control_2)
-        self.customControlPhase(control_1, target_qubit, Sx().matrix)
+        self.customcontrolled(control_1, target_qubit, sx())
         # append gate to self._circuit
         self._circuit.append(('toffoli', control_1, control_2, target_qubit))
 
     def rccx(self, control_1: int, control_2: int, target_qubit: int):
         """
         A 3-qubit quantum gate that takes in two control_qubit qubits and one target_qubit qubit.
         Params:
@@ -465,15 +462,15 @@
         self.u(target_qubit, 0, 0, np.pi / 4)
         self.cnot(control_2, target_qubit)
         self.u(target_qubit, 0, 0, (-1 * np.pi) / 4)
         self.u(target_qubit, np.pi / 2, 0, np.pi)
         # append gate to self._circuit
         self._circuit.append(('rccx', control_1, control_2, target_qubit))
 
-    def rc3x(self, a: int, b: int, c: int, d: int):
+    def rc3x(self, qubit_1: int, qubit_2: int, qubit_3: int, qubit_4: int):
         """
         A 4-qubit quantum gate that is a simplified Toffoli gate and can be used in placed where the Toffoli gate is uncomputed again.
         Params:
             a: int
             b: int
             c: int
             d: int
@@ -482,34 +479,34 @@
         """
         # If circuit is less than 4, means RC3X gate cannot be allowed.
         if (self._circuit_size < 4):
             exit(
                 f"Error: QuantumCircuit().rc3x -- Quantum Circuit size must be 4 or more qubits. Current number of qubits is: {self._circuit_size}")
         # Calls of gates here represent the RC3X matrix using other quantum
         # gates.
-        self.u(d, np.pi / 2, 0, np.pi)
-        self.u(d, 0, 0, np.pi / 4)
-        self.cnot(c, d)
-        self.u(d, 0, 0, (-1 * np.pi) / 4)
-        self.u(d, np.pi / 2, 0, np.pi)
-        self.cnot(a, d)
-        self.u(d, 0, 0, np.pi / 4)
-        self.cnot(b, d)
-        self.u(d, 0, 0, (-1 * np.pi / 4))
-        self.cnot(a, d)
-        self.u(d, 0, 0, np.pi / 4)
-        self.cnot(b, d)
-        self.u(d, 0, 0, (-1 * np.pi) / 4)
-        self.u(d, np.pi / 2, 0, np.pi)
-        self.u(d, 0, 0, np.pi / 4)
-        self.cnot(c, d)
-        self.u(d, 0, 0, (-1 * np.pi / 4))
-        self.u(d, np.pi / 2, 0, np.pi)
+        self.u(qubit_4, np.pi / 2, 0, np.pi)
+        self.u(qubit_4, 0, 0, np.pi / 4)
+        self.cnot(qubit_3, qubit_4)
+        self.u(qubit_4, 0, 0, (-1 * np.pi) / 4)
+        self.u(qubit_4, np.pi / 2, 0, np.pi)
+        self.cnot(qubit_1, qubit_4)
+        self.u(qubit_4, 0, 0, np.pi / 4)
+        self.cnot(qubit_2, qubit_4)
+        self.u(qubit_4, 0, 0, (-1 * np.pi / 4))
+        self.cnot(qubit_1, qubit_4)
+        self.u(qubit_4, 0, 0, np.pi / 4)
+        self.cnot(qubit_2, qubit_4)
+        self.u(qubit_4, 0, 0, (-1 * np.pi) / 4)
+        self.u(qubit_4, np.pi / 2, 0, np.pi)
+        self.u(qubit_4, 0, 0, np.pi / 4)
+        self.cnot(qubit_3, qubit_4)
+        self.u(qubit_4, 0, 0, (-1 * np.pi / 4))
+        self.u(qubit_4, np.pi / 2, 0, np.pi)
         # append gate to self._circuit
-        self._circuit.append(('rc3x', a, b, c, d))
+        self._circuit.append(('rc3x', qubit_1, qubit_2, qubit_3, qubit_4))
 
     def cnot(self, control_qubit: int, target_qubit: int):
         """
         A 2-qubit quantum gate that takes in control_qubit and target_qubit qubits, and will entangle the qubits if the control_qubit qubit is greater than 0.
         Params:
             control_qubit: int
             target_qubit: int
@@ -519,17 +516,17 @@
         # If circuit is less than 2, means CNOT gate cannot be allowed.
         if (self._circuit_size < 2):
             exit(
                 f"Error: QuantumCircuit().cnot -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
         # Determines if the little endian or big endian CNOT gate needs to be
         # established for calculations.
         if self._little_endian:
-            cnot_matrix = CNot().matrix
+            cnot_matrix = cnot(little_endian=True)
         else:
-            cnot_matrix = CNot(inverse=True).matrix
+            cnot_matrix = cnot()
         # Sends to __controlled_phase_handler alongside a boolean confirming
         # the gate is indeed a CNOT gate
         self.__controlled_phase_handler__(
             cnot_matrix, control_qubit, target_qubit)
         # append gate to self._circuit
         self._circuit.append(('cnot', control_qubit, target_qubit))
 
@@ -543,17 +540,15 @@
             None.
         """
         # If circuit is less than 2, means CR gate cannot be allowed.
         if (self._circuit_size < 2):
             exit(
                 f"Error: QuantumCircuit().cr -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
         self.__controlled_phase_handler__(
-            Cr().matrix, control_qubit, target_qubit)
-        # append gate to self._circuit
-        self._circuit.append(('cr', control_qubit, target_qubit))
+            cr(), control_qubit, target_qubit)
 
     def cz(self, control_qubit: int, target_qubit: int):
         """
         A 2-qubit quantum gate that takes in control_qubit and target_qubit qubits to perform calculations upon the state.
         Params:
             control_qubit: int
             target_qubit: int
@@ -561,17 +556,15 @@
             None.
         """
         # If circuit is less than 2, means CZ gate cannot be allowed.
         if (self._circuit_size < 2):
             exit(
                 f"Error: QuantumCircuit().cz -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
         self.__controlled_phase_handler__(
-            Cz().matrix, control_qubit, target_qubit)
-        # append gate to self._circuit
-        self._circuit.append(('cz', control_qubit, target_qubit))
+            cz(), control_qubit, target_qubit)
 
     def swap(self, qubit_1: int, qubit_2: int):
         """
         A 2-qubit quantum gate that takes in two qubits to swap the qubits values they represent.
         Params:
             qubit_1: int
             qubit_2: int
@@ -579,37 +572,37 @@
             None.
         """
         # If circuit is less than 2, means SWAP gate cannot be allowed.
         if (self._circuit_size < 2):
             exit(
                 f"Error: QuantumCircuit().swap -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
         # get the swap matrix
-        swap_matrix = Swap().matrix
+        swap_matrix = swap()
         # determines if the two values at play are at distance greater than
         # one, if so it will call in private method for larger matrix
         # operations.
         if (qubit_1 - qubit_2 != 1 and qubit_1 - qubit_2 != -1):
             self.__controlled_phase_handler__(swap_matrix, qubit_1, qubit_2)
         # if qubit_2 is above qubit_1 on the quantum wire, then it will use
         # qubit_2 as the call to __operator_matrix__.
         elif (qubit_1 > qubit_2):
-            self._state = np.dot(
+            self.state = np.dot(
                 self.__operator_matrix__(
                     swap_matrix,
                     qubit_2,
                     double=True),
-                self._state)
+                self.state)
         # simply commits a normal SWAP quantum gate functionality.
         else:
-            self._state = np.dot(
+            self.state = np.dot(
                 self.__operator_matrix__(
                     swap_matrix,
                     qubit_1,
                     double=True),
-                self._state)
+                self.state)
         # append gate to self._circuit
         self._circuit.append(('swap', qubit_1, qubit_2))
 
     def rxx(self, qubit_1: int, qubit_2: int, theta: float = np.pi / 2):
         """
         A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.
         Params:
@@ -619,15 +612,15 @@
         Returns:
             None.
         """
         # If circuit is less than 2, means RXX gate cannot be allowed.
         if (self._circuit_size < 2):
             exit(
                 f"Error: QuantumCircuit().rxx -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
-        rxx_matrix = Rxx(theta).matrix
+        rxx_matrix = rxx(theta)
         self.__controlled_phase_handler__(rxx_matrix, qubit_1, qubit_2)
         # append gate to self._circuit
         self._circuit.append(('rxx', qubit_1, qubit_2))
 
     def rzz(self, qubit_1: int, qubit_2: int, theta: float = np.pi / 2):
         """
         A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.
@@ -640,23 +633,21 @@
         """
         # If circuit is less than 2, means RZZ gate cannot be allowed.
         if (self._circuit_size < 2):
             exit(
                 f"Error: QuantumCircuit().rzz -- Quantum Circuit size must be 2 or more qubits. Current number of qubits is: {self._circuit_size}")
         if (qubit_2 < qubit_1):
             qubit_2, qubit_1 = qubit_1, qubit_2
-        rzz_matrix = Rzz(theta).matrix
+        rzz_matrix = rzz(theta)
         # determines if the two values at play are at distance greater than
         # one, if so it will call in private method for larger matrix
         # operations.
         self.__controlled_phase_handler__(rzz_matrix, qubit_1, qubit_2)
-        # append gate to self._circuit
-        self._circuit.append(('rzz', qubit_1, qubit_2))
 
-    def customControlPhase(
+    def customcontrolled(
             self,
             control_qubit: int,
             target_qubit: int,
             custom_matrix: np.array):
         """
         Used to insert single qubit based quantum gates to have a control_qubit qubit apart of it and committing to the quantum state.
         Params:
@@ -693,288 +684,258 @@
             controlled_custom_matrix, control_qubit, target_qubit)
         self._circuit.append(('C', control_qubit, target_qubit))
 
     """
     Single Qubit Gates
     """
 
-    def identity(self, qubit: int):
+    def i(self, qubit: int):
         """
         Used to confirm value that a qubit is representing and does nothing to manipulate the value of such qubit.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().identity -- Must select a qubit to enact on quantum gate.")
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Identity().matrix,
+                identity(),
                 qubit),
-            self._state)
-        # append gate to self._circuit
-        self._circuit.append((Identity().symbol, qubit))
+            self.state)
 
     def x(self, qubit: int):
         """
         Used to invert the value of what a qubit is representing.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().x -- Must select a qubit to enact on quantum gate.")
         # get the not matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                PauliX().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((PauliX().symbol, qubit))
+                paulix(), qubit), self.state)
 
-    def hadamard(self, qubit: int):
+    def h(self, qubit: int):
         """
         Used to put a given qubit into superposition.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().hadamard -- Must select a qubit to enact on quantum gate.")
         # get the hadamard matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Hadamard().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Hadamard().symbol, qubit))
+                hadamard(), qubit), self.state)
 
     def y(self, qubit: int):
         """
         Changes the state of a qubit by pi around the y-axis of a Bloch Sphere.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().y -- Must select a qubit to enact on quantum gate.")
         # get the Y matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                PauliY().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append(PauliY().symbol)
+                pauliy(), qubit), self.state)
 
     def z(self, qubit: int):
         """
         Changes the state of a qubit by pi around the z-axis of a Bloch Sphere.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().z -- Must select a qubit to enact on quantum gate.")
         # get the Z matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                PauliZ().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((PauliZ().symbol, qubit))
+                pauliz(), qubit), self.state)
 
     def phase(self, qubit: int, theta: float = np.pi / 2):
         """
         Commits to a rotation around the z-axis based off of the inputted theta value.
         Params:
             qubit: int
             theta: float
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().phase -- Must select a qubit to enact on quantum gate.")
         # get the Phase matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Phase(theta).matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Phase(theta).symbol, qubit))
+                phase(theta), qubit), self.state)
 
     def s(self, qubit: int):
         """
         Is a Phase gate where the inputted theta value is given as a constant of theta = pi / 2.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().s -- Must select a qubit to enact on quantum gate.")
         # get the Phase matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                S().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((S().symbol, qubit))
+                s(), qubit), self.state)
 
     def sdg(self, qubit: int):
         """
         Is a Phase gate and inverse of the S gate where the inputted theta value is given as a constant of theta = -pi / 2.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().sdg -- Must select a qubit to enact on quantum gate.")
         # get the Sdg matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Sdg().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Sdg().symbol, qubit))
+                sdg(), qubit), self.state)
 
     def t(self, qubit: int):
         """
         T gate is a special use case gate that in implemented from the P Gate.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().t -- Must select a qubit to enact on quantum gate.")
         # get the T matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                T().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((T().symbol, qubit))
+                t(), qubit), self.state)
 
     def tdg(self, qubit: int):
         """
         TDG gate is a special use case gate that in implemented from the P Gate and is the inverse of the T gate.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().tdg -- Must select a qubit to enact on quantum gate.")
         # get the Tdg matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Tdg().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Tdg().symbol, qubit))
+                tdg(), qubit), self.state)
 
     def rz(self, qubit: int, theta: float = np.pi / 2):
         """
         RZ gate commits a rotation around the z-axis for a qubit.
         Params:
             qubit: int
             theta: float
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().rz -- Must select a qubit to enact on quantum gate.")
         # get the Rz matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Rz(theta).matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Rz(theta).matrix, qubit))
+                rz(theta), qubit), self.state)
 
     def ry(self, qubit: int, theta: float = np.pi / 2):
         """
         RY gate commits a rotation around the y-axis for a qubit.
         Params:
             qubit: int
             theta: float
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().ry -- Must select a qubit to enact on quantum gate.")
         # get the Ry matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Ry(theta).matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Ry().symbol, qubit))
+                ry(theta), qubit), self.state)
 
     def rx(self, qubit: int, theta: float = np.pi / 2):
         """
         RX gate commits a rotation around the x-axis for a qubit.
         Params:
             qubit: int
             theta: float
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().rx -- Must select a qubit to enact on quantum gate.")
         # get the Rx matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Rx(theta).matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Rx(theta).matrix, qubit))
+                rx(theta), qubit), self.state)
 
     def sx(self, qubit: int):
         """
         SX gate is the square root of the Inverse gate (X, PauliX Gate).
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().sx -- Must select a qubit to enact on quantum gate.")
         # get the Sx matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Sx().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Sx().symbol, qubit))
+                sx(), qubit), self.state)
 
     def sxdg(self, qubit: int):
         """
         SXDG gate is the negative square root of the Inverse gate (X, PauliX Gate) and inverse of the SX gate.
         Params:
             qubit: int
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().sxdg -- Must select a qubit to enact on quantum gate.")
         # get the Sxdg matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                Sxdg().matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((Sxdg().symbol, qubit))
+                sxdg(), qubit), self.state)
 
     def u(
         self,
         qubit: int,
         theta: float = np.pi / 2,
         phi: float = np.pi / 2,
             lmbda: float = np.pi / 2):
@@ -989,32 +950,29 @@
         Returns:
             None.
         """
         if qubit is None:
             exit(
                 f"Error: QuantumCircuit().u -- Must select a qubit to enact on quantum gate.")
         # get the U matrix
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
-                U(theta, phi, lmbda).matrix, qubit), self._state)
-        # append gate to self._circuit
-        self._circuit.append((U().symbol, qubit))
+                u(theta, phi, lmbda), qubit), self.state)
 
     def custom(self, qubit: int, custom_matrix: np.array):
         """
         Will take in a custom single qubit quantum gate and implement it on a qubit.
         Params:
             qubit: int
             custom_matrix: np.array
         Returns:
             None.
         """
         # if gate is not a single qubit, will exit.
         if (custom_matrix.shape != (2, 2)):
             exit(f"Error: QuantumCircuit().insertGate -- can only include a single qubit based quantum gate (2,2) matrix for state manipulation.")
         # calls gate and will operate on state as per usual
-        self._state = np.dot(
+        self.state = np.dot(
             self.__operator_matrix__(
                 custom_matrix,
                 qubit),
-            self._state)
-        self._circuit.append(('C', qubit))
+            self.state)
```

### Comparing `QCpython-1.0.3/QCpy/Core/tools/amplitude.py` & `qcpython-1.1.0/qcpy/core/tools/amplitude.py`

 * *Files identical despite different names*

### Comparing `QCpython-1.0.3/QCpy/Core/tools/measure.py` & `qcpython-1.1.0/qcpy/core/tools/measure.py`

 * *Files identical despite different names*

### Comparing `QCpython-1.0.3/QCpy/Core/tools/phaseangle.py` & `qcpython-1.1.0/qcpy/core/tools/phaseangle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from numpy import mod, pi, around, angle
 
-def phaseAngle(state, circuit_size, show_bit = -1, round: int = 3, radian: bool = True):
+def phaseangle(state, circuit_size, show_bit = -1, round: int = 3, radian: bool = True):
     """
     Calculates an array of possible phase angles based off the state. Converts each value using np.angle() function then degree to radian.
     Params:
         round: int
         radian: bool
     Returns:
         np.around(phaseAngles) (numpy array):
```

### Comparing `QCpython-1.0.3/QCpy/Core/tools/probabilities.py` & `qcpython-1.1.0/qcpy/core/tools/probabilities.py`

 * *Files identical despite different names*

### Comparing `QCpython-1.0.3/QCpy/Visualizer/blochsphere.py` & `qcpython-1.1.0/qcpy/visualizer/bloch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-from ..Core import QuantumCircuit
+from ..core import quantumcircuit
 import matplotlib.pyplot as plt
-from .tools.sphere import Sphere
+from .tools.sphere import sphere
 
 
-class BlochSphere:
+class bloch:
     """
     Visualizes the quantum state of a single qubit as a sphere
 
     Methods
     --------
     makeSphere():
         returns a Bloch Sphere that plots the quantum state of a single qubit in a
@@ -33,15 +33,15 @@
             exit(
                 f"Error: BlochSphere() --",
                 f"BlochSphere only calculates 1 qubit circuits."
             )
         self._amplitutes = circuit.amplitude().flatten()
         self._phase_angles = circuit.phaseAngle().flatten()
 
-    def makeSphere(
+    def make(
             self,
             path: str = "BlochSphere.png",
             show_bit: int = 0,
             save: bool = False,
             show: bool = True,
             darkmode: bool = True):
         """
@@ -60,15 +60,15 @@
             _background = '#2e3037'
         else:
             _text = 'black'
             _accent = 'black'
             _background = 'white'
 
         # creates a sphere
-        ax = Sphere(_background)
+        ax = sphere(_background)
         # x-axis arrow
         ax.quiver(1, 0, 0, .75, 0, 0, color="lightgray")
         ax.text(2, 0, 0, "+x", color="gray")
         # y-axis arrow
         ax.quiver(0, 1, 0, 0, .75, 0, color="lightgray")
         ax.text(0, 2, 0, "+y", color="gray")
         # +z and |0> arrow
```

### Comparing `QCpython-1.0.3/QCpy/Visualizer/probabilities.py` & `qcpython-1.1.0/qcpy/visualizer/probability.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-from ..Core import QuantumCircuit
+from ..core import quantumcircuit
 import matplotlib.pyplot as plt
-from .tools.graph import Graph
+from .tools.graph import graph
 
 
-class Probabilities:
+class probability:
     """
     Visualizes the quantum circuit's qubits probability of being measured using a bar graph
 
     Methods
     --------
     makeGraph(path: str, show: bool) :
         returns a graph that plots all the probabilities of the qubits being measured
@@ -31,15 +31,15 @@
         self._num_qubits = circuit.circuitSize()
         self._state_list = [
             format(i, 'b').zfill(self._num_qubits)
             for i in range(2**self._num_qubits)
         ]
         self._percents = [i * 100 for i in circuit.probabilities()]
 
-    def makeGraph(
+    def make(
             self,
             path: str = "probabilities.png",
             save: bool = False,
             show: bool = True,
             darkmode: bool = True):
         """
             Creates a graph of the circuit's probabilties
@@ -59,15 +59,15 @@
             _accent = 'black'
             _background = 'white'
 
         # clears any previous plots
         plt.clf()
         plt.close()
         # sets up bar graph
-        ax = Graph(_text, _background, self._num_qubits)
+        ax = graph(_text, _background, self._num_qubits)
         # sets x and y labels and title
         ax.bar(self._state_list, self._percents, color='#39c0ba')
         plt.xlabel('Computational basis states', color=_accent)
         plt.ylabel('Probability (%)', labelpad=5, color=_accent)
         plt.title('Probabilities', pad=10, color=_accent)
         plt.tight_layout()
```

### Comparing `QCpython-1.0.3/QCpy/Visualizer/qsphere.py` & `qcpython-1.1.0/qcpy/visualizer/qsphere.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import numpy as np
-from ..Core import QuantumCircuit
 import matplotlib.pyplot as plt
-from .tools.sphere import Sphere
-# ScalerMappable is needed for creating the color bar on the State Vector visualization
-# that shows what each qubit's phase angle is
 from matplotlib.cm import ScalarMappable
-# deque is needed for the function that gets the qubit states in order of which the appear
-# on a QSphere
 from collections import deque
+from .tools.sphere import sphere
+from ..core.tools import amplitude, phaseangle, probabilities
 
-
-class QSphere:
+class qsphere:
     """
     Visualizes the quantum circuit as a q-sphere
 
     Methods
     --------
-    makeSphere() :
-        returns a Q-Sphere that plots a global visualization of the quantum states
-        in a 3D global view
+    make() :
+        returns a Q-Sphere that plots a global visualization of the quantum 
+        states in a 3D global view
     """
 
     def __init__(self, circuit=None):
         """
         Args:
             circuit:
                 the quantum circuit
@@ -31,64 +26,72 @@
             _num_qubits :
                 the number of qubits on the circuit
             _state_list :
                 all the states of the qubits on the circuit
             _probabilities :
                 an array of all the probabilities of the qubits being measured
             _percents :
-                the array of probabilities turned into an array of values adding to 100
+                the array of probabilities turned into an array of values adding 
+                to 100
             _amplitudes :
                 an array of the amplitude for every state
             _phase_angles :
                 an array of the phase angle for every state
             _prob_dict :
                 a dictionary of the probabilities mapped to the state list
             _phase_dict :
                 a dictionary of the phase angles mapped to the state list
             _lat_vals :
-                a list of lists of the qubit states in order as the appear upon the latitudes of a QSphere
+                a list of lists of the qubit states in order as the appear upon 
+                the latitudes of a QSphere
         """
         self._num_qubits = int(np.log2(len(circuit.probabilities())))
         self._state_list = [
             format(i, 'b').zfill(self._num_qubits)
             for i in range(2**self._num_qubits)
         ]
         self._probabilities = circuit.probabilities()
         self._percents = [i * 100 for i in self._probabilities]
         self._amplitutes = circuit.amplitude().flatten()
-        self._phase_angles = circuit.phaseAngle().flatten()
+        self._phase_angles = circuit.phaseangle().flatten()
         self._prob_dict = {
             self._state_list[i]: self._probabilities[i]
             for i in range(len(self._state_list))
         }
         self._phase_dict = {
             self._state_list[i]: self._phase_angles[i]
             for i in range(len(self._state_list))
         }
         self._lat_vals = self.__latitude_finder__()
 
     def __hamming_distance__(self, l1: str, l2: str):
         """
-        Determines if the count of the number of 1 values match up between two strings.
+        Determines if the count of the number of 1 values match up between
+            two strings.
 
         Args:
             l1: string
             l2: string
         Returns:
-            Boolean representation if the count of ones in l1 and l2 are equal to each other.
+            Boolean representation if the count of ones in l1 and l2 are equal 
+            to each other.
         """
         return l1.count("1") == l2.count("1")
 
     def __latitude_finder__(self):
         """
-        Creates a 2D array of placed values on each latitude ring, alongside the amount of rotations around the specific lognitude that need to shifted for proper placement.
+        Creates a 2D array of placed values on each latitude ring, alongside the 
+        amount of rotations around the specific lognitude that need to shifted 
+        for proper placement.
         Args:
             None
         Returns:
-            2D array of needed values and an abstract view of the rotation around each longitude placement, given the length of each row within the 2D array.
+            2D array of needed values and an abstract view of the rotation 
+            around each longitude placement, given the length of each row within 
+            the 2D array.
         """
         # Main holder of values of latitude placement values
         latitude_values = [[]]
         # will create a 2d array of empty arrays based on the number of qubits
         # - 1, for the starting empty array.
         for _ in range(self._num_qubits - 1):
             latitude_values.append([])
@@ -161,15 +164,15 @@
                 y1 = 1 * np.sin(phi[i]) * np.sin(theta[i][j])
                 z1 = 1 * np.cos(phi[i])
                 x, y, z = [0, x1], [0, y1], [0, z1]
                 coords.append([x, y, z])
 
         return coords
 
-    def makeSphere(
+    def make(
             self,
             path: str = "qsphere.png",
             save: bool = False,
             show: bool = True,
             darkmode: bool = True):
         """
             Creates a sphere that visualizes the qubits phase angles if their probability of being measured is greater than 0
@@ -184,15 +187,15 @@
             _text = 'white'
             _accent = '#39c0ba'
             _background = '#2e3037'
         else:
             _text = 'black'
             _accent = 'black'
             _background = 'white'
-        ax = Sphere(_background)
+        ax = sphere(_background)
         # coords will be in the order of states from the __latitude_finder__ function
         # and not in order of self._state_list, we can use our dict to look up each states
         # probability in any order now b/c we do not want to plot a qubit if it
         # has a probability of 0
         coords = self.__getCoords__()
         # turns self._lat_vals into a single list instead of a list of lists
         ham_states = [item for sublist in self._lat_vals for item in sublist]
```

### Comparing `QCpython-1.0.3/QCpy/Visualizer/statevector.py` & `qcpython-1.1.0/qcpy/visualizer/statevector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
-from ..Core import QuantumCircuit
+from ..core import quantumcircuit
 import matplotlib.pyplot as plt
 # ScalerMappable is needed for creating the color bar on the State Vector
 # visualization
 from matplotlib.cm import ScalarMappable
 from matplotlib.colors import rgb2hex
-from .tools.graph import Graph
+from .tools.graph import graph
 
 
-class StateVector:
+class statevector:
     """
     Visualizes the quantum circuit's quantum amplitutes using a bar graph
 
     Methods
     --------
     makeGraph() :
         returns a graph that plots all the amplitudes of the qubits being measured
@@ -44,15 +44,15 @@
             for i in range(2**self._num_qubits)
         ]
         self._probabilities = circuit.probabilities()
         self._percents = [i * 100 for i in circuit.probabilities()]
         self._amplitutes = circuit.amplitude().flatten()
         self._phase_angles = circuit.phaseAngle().flatten()
 
-    def makeGraph(
+    def make(
             self,
             path: str = "statevector.png",
             save: bool = True,
             show: bool = False,
             darkmode: bool = True):
         """
             Creates a graph of the circuit's amplitudes and phase angles
@@ -69,15 +69,15 @@
             _background = '#2e3037'
         else:
             _text = 'black'
             _accent = 'black'
             _background = 'white'
 
         # clears any previous plots
-        ax = Graph(_text, _background, self._num_qubits)
+        ax = graph(_text, _background, self._num_qubits)
 
         ax.set_ylim(0, np.amax(self._amplitutes))
         colors = plt.get_cmap('hsv')  # color map
         # need phase angle values to be normalized from 0 to 2pi
         norm = plt.Normalize(0, np.pi * 2)
         # array of hexvals corresponding to qubit's phase angles
         hex_arr = [rgb2hex(i) for i in colors(norm(self._phase_angles))]
```

### Comparing `QCpython-1.0.3/QCpy/Visualizer/tools/graph.py` & `qcpython-1.1.0/qcpy/visualizer/tools/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 # ScalerMappable is needed for creating the color bar on the State Vector
 # visualization
 
 
-def Graph(_text, _background, num_qubits):
+def graph(_text, _background, num_qubits):
     plt.clf()
     plt.close()
     # sets up bar graph and colors that map to a qubits phase angle
     fig, ax = plt.subplots(figsize=(num_qubits + 3, num_qubits + 3))
     # sets up tick labels
     plt.setp(ax.get_xticklabels(), rotation=75, ha='right', color=_text)
     plt.setp(ax.get_yticklabels(), color=_text)
```

### Comparing `QCpython-1.0.3/QCpy/Visualizer/tools/sphere.py` & `qcpython-1.1.0/qcpy/visualizer/tools/sphere.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import matplotlib.pyplot as plt
 # ScalerMappable is needed for creating the color bar on the State Vector visualization
 # that shows what each qubit's phase angle is
 from matplotlib.cm import ScalarMappable
 import numpy as np
 
 
-def Sphere(_background):
+def sphere(_background):
     # creates a sphere
     plt.clf()
     plt.close()
     plt.clf()
     plt.close()
     fig = plt.figure()
     ax = fig.add_subplot(111, projection="3d")
```

### Comparing `QCpython-1.0.3/QCpython.egg-info/PKG-INFO` & `qcpython-1.1.0/qcpython.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,746 +1,900 @@
 Metadata-Version: 2.1
-Name: QCpython
-Version: 1.0.3
-Summary: QCpy is a comprehensive and user-friendly library for quantum computing, providing a wide range of functionality for quantum algorithms and quantum circuits. It is built on using open-source libraries NumPy and Matplotlib; compatible with Python 3.
+Name: qcpython
+Version: 1.1.0
+Summary: QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing.
 Home-page: https://github.com/QCpython/QCpy
 Author: Brennan Freeze, Paris Osuch, Aundre Barras, Soren Richenberg, Suzanne Rivoire
 Author-email: freezebrennan@gmail.com, osuch@sonoma.edu, barras@sonoma.edu, richenbe@sonoma.edu, rivoire@sonoma.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # README.md
 
 # QCpy - A Quantum Computing Library for Python
 
-QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing (QC).
+QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing.
 
 You can download the package using pip:
 
 ```txt
-pip install QCpython
+pip install qcpython
 ```
-
-## Recommended Resources on Quantum Computing:
-
-- [Microsoft’s Linear Algebra for Quantum Computing](https://learn.microsoft.com/en-us/azure/quantum/overview-algebra-for-quantum-computing)
-- [IBM’s Quantum Computing: a field guide](https://quantum-computing.ibm.com/composer/docs/iqx/guide/)
-- [Wikipedia: Quantum Computing](https://en.wikipedia.org/wiki/Quantum_computing)
-
 ---
 
-# Qubits
+# Qubit
 
-> ## *class* QCpy.`Qubit`(*initial_state=’z’*)
+> ## qcpy.`qubit`(*initial_state=’z’*)
 
 *Object representation of a qubit.*
 
 ### Parameters:
 
-`initial_state (chr)` - Character input for starting direction in the *x*, *y*, or *z* axis.
+`initial_state (chr)` default: `z` - Character input for starting direction in the *x*, *y*, or *z* axis.
 
 ### Attributes:
 
-`state (numpy.ndarray)` -  current state of qubit in matrix representation.
+`None`
+
+### Example:
+
+```python
+from qcpy import qubit
 
+qx = qubit(initial_state = 'x')
+qy = qubit(initial_state = 'y')
+qz = qubit(initial_state = 'z')
+print("qx:\n", qx)
+print("qy:\n", qy)
+print("qz:\n", qz)
+
+
+# qx:
+#  [[0.70710677+0.j]
+#  [0.70710677+0.j]]
+# qy:
+#  [[0.70710677+0.j]
+#  [0.+0.70710677j]]
+# qz:
+#  [[1.+0.j]
+#  [0.+0.j]]
+```
 ---
 
 # Quantum Gates
 
-> ## *class* QC.QuantumGate.`Identity`()
+> ## quantumgate.`identity`()
 
 *Gate that does not modify the quantum state.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Identity gate.
-
 ```python
-Identity.matrix = [1+0j, 0+0j], 
-	          [0+0j, 1+0j]
+identity=[1+0j, 0+0j], 
+         [0+0j, 1+0j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`PauliX`()
+```python
+from qcpy import identity 
+
+print(identity())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j]]
+```
+> ## quantumgate.`paulix`()
 
 *Quantum equivalent of the NOT gate in classical computing with respect to the standard basis |0>, |1>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-X gate.
-
 ```python
-PauliX.matrix = [0+0j, 1+0j], 
-	        [1+0j, 0+0j]
+PauliX = [0+0j, 1+0j], 
+	 [1+0j, 0+0j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`PauliY`()
+```python
+from qcpy import paulix
+
+print(paulix())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j]]
+```
+> ## quantumgate.`pauliy`()
 
 *Rotation around y-axis of the bloch sphere by π radiains, mapping |0> to i|1> and |1> to -i|0>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-Y gate.
-
 ```python
-PauliY.matrix = [0+0j, 0-1j],
-                [0+1j, 0+0j]
+PauliY = [0+0j, 0-1j],
+         [0+1j, 0+0j]
 ```
+### Example:
+
+```python
+from qcpy import pauliy
+
+print(pauliy())
 
-> ## *class* QC.QuantumGate.`PauliZ`()
+# [[0+0j, 0-1j]
+#  [0+1j, 0+0j]]
+```
+> ## quantumgate.`pauliz`()
 
 *Rotation around z-axis of the bloch sphere by π radiains, mapping |1> to -|1>; known as the phase-flip.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-Z gate.
-
 ```python
-PauliZ.matrix = [1+0j, 0+0j], 
-                [0+0j, -1+0j]
+PauliZ = [1+0j, 0+0j], 
+         [0+0j, -1+0j]
 ```
+### Example:
+
+```python
+from qcpy import pauliz
 
-> ## *class* QC.QuantumGate.`Hadamard`()
+print(pauliz())
+
+# [[1+0j, 0+0j], 
+#  [0+0j, -1+0j]]
+```
+> ## quantumgate.`hadamard`()
 
 *Maps the basis states |0> to |+> and |1> to |->, creating a superposition state if given a computation basis state.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Hadamard gate.
-
 ```python
-Hadamard.matrix = ([1,  1] 
-                   [1, -1]) * (1/sqrt(2))
+Hadamard = [1,  1] 
+           [1, -1] * (1/sqrt(2))
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`CNot`(*inverse=False*)
+```python
+from qcpy import hadamard
 
-*Controlled gate acts on two or more qubits, performing the NOT operation of the target qubit only if the control qubits are |1>, can act as a quantum regiester and is used to entangle and disentangle Bell states.*
+print(hadamard())
 
-### Parameters:
+# [[ 0.70710677+0.j  0.70710677+0.j]
+#  [ 0.70710677+0.j -0.70710677+0.j]]
+```
+> ## quantumgate.`cnot`(*little_endian=False*)
 
-`inverse (bool)` - if the gate is an inverse, with the target being above the control.
+*Controlled gate acts on two or more qubits, performing the NOT operation of the target qubit only if the control qubits are |1>, can act as a quantum regiester and is used to entangle and disentangle Bell states.*
 
-### Attributes:
+### Parameters:
 
-`matrix (np.ndarray)` - matrix representation of CNOT gate.
+`little_endian (bool)` - if the gate is an inverse, with the target being above the control.
 
 ```python
 # regular
-CNot.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j]
-# inverse
-CNot.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j] 
+CNot = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j]
+# little_endian = True
+CNot = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j] 
 ```
+### Example:
+
+```python
+from qcpy import cnot
+
+print(cnot())
+
+# [[1.+0.j 0.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 0.+0.j 0.+0.j 1.+0.j]
+#  [0.+0.j 0.+0.j 1.+0.j 0.+0.j]]
 
-> ## *class* QC.QuantumGate.`Swap`()
+# [[1.+0.j 0.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 0.+0.j 0.+0.j 1.+0.j]
+#  [0.+0.j 0.+0.j 1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j 0.+0.j 0.+0.j]]
+```
+> ## quantumgate.`swap`()
 
 *Swaps two qubits, with respect to the basis |00>, |01>, |10>, and |11>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of SWAP gate.
-
 ```python
-Swap.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j]
+Swap = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j]
 ```
+### Example:
+
+```python
+from qcpy import swap
 
-> ## *class* QC.QuantumGate.`Toffoli`()
+print(swap())
+
+# [1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j]
+```
+> ## quantumgate.`toffoli`()
 
 *Universal reversible logic gate, known as the “controlled-controlled-NOT” gate; if the two control bits are set to 1, it will invert the target.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Toffoli gate.
-
 ```python
-Toffoli.matrix = [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+Toffoli = [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
 ```
+### Example:
+
+```python
+from qcpy import toffoli
 
-> ## *class* QC.QuantumGate.`Phase`(*theta=numpy.pi/2*)
+print(toffoli())
+
+# [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+```
+> ## quantumgate.`phase`(*theta=numpy.pi/2*)
 
 *Applies a rotation of theta around the z-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around z-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Phase gate.
-
 ```python
-Phase.matrix = [1+0j, 0+0j],
-	       [0+0j, numpy.exp(0+1j * theta)]
+Phase = [1+0j, 0+0j],
+	[0+0j, numpy.exp(0+1j * theta)]
 ```
+### Example:
+
+```python
+from qcpy import phase
 
-> ## *class* QC.QuantumGate.`S`()
+print(phase())
+
+# [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+```
+> ## quantumgate.`s`()
 
 *Equivalent to a pi/2 rotation around the z-axis.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of S gate.
-
 ```python
 S.matrix = [1+0j, 0+0j],
            [0+0j, 0+1j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Sdg`()
+```python
+from qcpy import s
+
+print(s())
+
+# [1+0j, 0+0j],
+# [0+0j, 0+1j]
+```
+> ## quantumgate.`sdg`()
 
 *Inverse of S gate; a -pi/2 rotation around the z-axis.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an inverse S gate.
-
 ```python
 Sdg.matrix = [1+0j, 0+0j],
              [0+0j, 0-1j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`T`()
+```python
+from qcpy import sdg
+
+print(sdg())
+
+# [1+0j, 0+0j],
+# [0+0j, 0-1j]
+```
+> ## quantumgate.`t`()
 
 *Square of S gate; where T = S^2.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a T gate.
-
 ```python
 T.matrix = [1+0j, 0+0j],
            [0+0j, numpy.exp((0+1j * numpy.pi) / 4)]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Tdg`()
+```python
+from qcpy import t
+
+print(t())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 0.70710677+0.70710677j]]
+```
+> ## quantumgate.`tdg`()
 
 *Inverse of T gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a inverse of T gate.
-
 ```python
-Tdg.matrix = [1+0j, 0+0j],
-             [0+0j, numpy.exp((0-1j * numpy.pi) / 4)]
+Tdg = [1+0j, 0+0j],
+      [0+0j, numpy.exp((0-1j * numpy.pi) / 4)]
 ```
+### Example:
+
+```python
+from qcpy import tdg
 
-> ## *class* QC.QuantumGate.`Rz`(*theta=numpy.pi/2*)
+print(tdg())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 0.70710677-0.70710677j]]
+```
+> ## quantumgate.`rz`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the z-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around z-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rz gate.
-
 ```python
-Rz.matrix = [numpy.exp((0-1j * (theta / 2))), 0+0j],
-            [0+0j, numpy.exp(0+1j * (theta / 2))]
+Rz = [numpy.exp((0-1j * (theta / 2))), 0+0j],
+     [0+0j, numpy.exp(0+1j * (theta / 2))]
 ```
 
-> ## *class* QC.QuantumGate.`Rx`(*theta=numpy.pi/2*)
+> ## quantumgate.`rx`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the x-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around x-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rx gate.
-
 ```python
-Rx.matrix = [numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2)],
-            [0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2)]
+Rx = [numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2)],
+     [0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2)]
 ```
+### Example:
+
+```python
+from qcpy import rx
 
-> ## *class* QC.QuantumGate.`Ry`(*theta=numpy.pi/2*)
+print(rx())
+
+# [[0.70710677+0.j 0.-0.70710677j]
+#  [0.-0.70710677j 0.70710677+0.j]]
+```
+> ## quantumgate.`ry`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the y-axis.*
 
 ### Parameters:
 
 `theta (float)`default: `numpy.pi/2` -  angle of rotation around y-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Ry gate.
-
 ```python
-Ry.matrix = [numpy.cos(theta / 2), -1 * numpy.sin(theta / 2)],
-            [numpy.sin(theta / 2), numpy.cos(theta / 2)]
+Ry = [numpy.cos(theta / 2), -1 * numpy.sin(theta / 2)],
+     [numpy.sin(theta / 2), numpy.cos(theta / 2)]
 ```
+### Example:
+
+```python
+from qcpy import ry
 
-> ## *class* QC.QuantumGate.`Sx`()
+print(ry())
+
+# [[ 0.70710677+0.j -0.70710677+0.j]
+#  [ 0.70710677+0.j  0.70710677+0.j]]
+```
+> ## quantumgate.`sx`()
 
 *Rotation around the x-axis by 90 degrees in the counter-clockwise direction. Also known as the “square-root X gate” due to the fact that applying the SX gate twice results in an X gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Sx gate.
-
 ```python
-Sx.matrix = [1+1j, 1-1j], 
-            [1-1j, 1+1j]]) * (1 / 2)
+Sx = [1+1j, 1-1j], 
+     [1-1j, 1+1j] * (1 / 2)
 ```
+### Example:
+
+```python
+from qcpy import sx
 
-> ## *class* QC.QuantumGate.`Sxdg`()
+print(sx())
+
+# [[0.5+0.5j 0.5-0.5j]
+#  [0.5-0.5j 0.5+0.5j]]
+```
+> ## quantumgate.`sxdg`()
 
 *Inverse of the Sx gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an inverse Sx gate.
-
 ```python
-Sxdg.matrix = [1-1j, 1+1j], 
-              [1+1j, 1-1j]]) * (1 / 2)
+Sxdg = [1-1j, 1+1j], 
+       [1+1j, 1-1j] * (1 / 2)
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`U`(*theta=numpy.pi/2, phi=numpy.pi/2, lmbda=numpy.pi/2*)
+```python
+from qcpy import sxdg
+
+print(sxdg())
+
+# [[0.5-0.5j 0.5+0.5j]
+#  [0.5+0.5j 0.5-0.5j]]
+```
+> ## quantumgate.`u`(*theta=numpy.pi/2, phi=numpy.pi/2, lmbda=numpy.pi/2*)
 
 *Rotation of qubit with respect to theta, phi, and lambda, in Euler angles.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around Euler angle theta.
 
 `phi (float)` default: `numpy.pi/2` -  angle of rotation around Euler angle phi.
 
 `lmbda (float)` default: `numpy.pi/2` -  angle of rotation around Eulear angle lambda.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a U gate.
-
 ```python
 U.matrix = [numpy.cos(theta / 2), -1 * numpy.exp(0+1j * lmbda) * numpy.sin(theta / 2)], 
            [numpy.exp(0+1j * phi) * numpy.sin(theta / 2), numpy.exp(0+1j * (lmbda + phi)) * numpy.cos(theta / 2)]]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Rxx`(*theta=numpy.pi/2*)
+```python
+from qcpy import u
+
+print(u())
+
+# [[0.7071+0.j -0.-0.7071j]
+#  [0.+0.7071j -0.7071+0.j]]
+```
+> ## quantumgate.`rxx`(*theta=numpy.pi/2*)
 
 *Rotation about XX, maximally entangling at theta = pi/2.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around XX.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rxx gate.
-
 ```python
 Rxx.matrix = [numpy.cos(theta / 2), 0+0j, 0+0j, 0-1j * numpy.sin(theta / 2)],
              [0+0j, numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2), 0+0j],
              [0+0j, 0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2), 0+0j],
              [0-1j * numpy.sin(theta / 2), 0+0j, 0+0j, numpy.cos(theta / 2)]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Rzz`(*theta=numpy.pi/2*)
+```python
+from qcpy import rxx
+
+print(rxx())
+
+# [[0.70710677+0.j 0+0.j 0+0.j 0-0.70710677j]
+#  [0+0.j 0.70710677+0.j 0-0.70710677j 0+0.j]
+#  [0+0.j 0-0.70710677j 0.70710677+0.j 0+0.j]
+#  [0-0.70710677j 0+0.j 0.+0.j 0.70710677+0.j]]
+```
+> ## quantumgate.`rzz`(*theta=numpy.pi/2*)
 
 *Rotation about ZZ, maximally entangling at theta = pi/2.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around ZZ.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rzz gate.
-
 ```python
 Rzz.matrix = [numpy.exp(0-1j * (theta / 2)), 0+0j, 0+0j, 0+0j],
              [0+0j, numpy.exp(0+1j * (theta / 2)), 0+0j, 0+0j],
              [0+0j, 0+0j, numpy.exp(0+1j * (theta / 2)), 0+0j],
              [0+0j, 0+0j, 0+0j, numpy.exp(0-1j * (theta / 2))]
 ```
+### Example:
+
+```python
+from qcpy import rzz
 
-> ## *class* QC.QuantumGate.`Cr`(*theta=numpy.pi/2*)
+print(rzz())
+
+# [[0.70710677-0.70710677j 0+0.j 0+0.jn 0+0.j]
+#  [0+0.j 0.70710677+0.70710677j 0+0.j 0+0.j]
+#  [0+0.j 0+0.j 0.70710677+0.70710677j 0+0.j]
+#  [0+0.j 0+0.j 0+0.j 0.70710677-0.70710677j]]
+```
+> ## quantumgate.`cr`(*theta=numpy.pi/2*)
 
 *Controlled phase shift rotation in theta radians; generalization of Cz gate.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation in theta radians.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Cr gate.
-
 ```python
-Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-            [0+0j, 1+0j, 0+0j, 0+0j],
-            [0+0j, 0+0j, 1+0j, 0+0j],
-            [0+0j, 0+0j, 0+0j, numpy.exp(theta * 0+1j)]
+Cr = [1+0j, 0+0j, 0+0j, 0+0j],
+     [0+0j, 1+0j, 0+0j, 0+0j],
+     [0+0j, 0+0j, 1+0j, 0+0j],
+     [0+0j, 0+0j, 0+0j, exp(theta * 0+1j)]
 ```
+### Example:
+
+```python
+from qcpy import cr
 
-> ## *class* QC.QuantumGate.`Cz`(*theta=numpy.pi/2*)
+print(cr())
+
+# [[1+0.j 0+0.j 0+0.j 0+0.j]
+#  [0+0.j 1+0.j 0+0.j 0+0.j]
+#  [0+0.j 0+0.j 1+0.j 0+0.j]
+#  [0+0.j 0+0.j 0+0.j 0.5403023+0.84147096j]]
+```
+> ## quantumgate.`cz`(*theta=numpy.pi/2*)
 
 *Controlled phase shift rotation in theta radians.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation in theta radians.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Cz gate.
+```python
+Cz = [1+0j, 0+0j, 0+0j, 0+0j],
+     [0+0j, 1+0j, 0+0j, 0+0j],
+     [0+0j, 0+0j, 1+0j, 0+0j],
+     [0+0j, 0+0j, 0+0j, -1+0j]
+```
+### Example:
 
 ```python
-Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-            [0+0j, 1+0j, 0+0j, 0+0j],
-            [0+0j, 0+0j, 1+0j, 0+0j],
-            [0+0j, 0+0j, 0+0j, -1+0j]
+from qcpy import cz
+
+print(cz())
+
+# [[ 1.+0.j  0.+0.j  0.+0.j  0.+0.j]
+#  [ 0.+0.j  1.+0.j  0.+0.j  0.+0.j]
+#  [ 0.+0.j  0.+0.j  1.+0.j  0.+0.j]
+#  [ 0.+0.j  0.+0.j  0.+0.j -1.+0.j]]
 ```
 ---
 # Quantum Circuit
-> ## *class* QCpy.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
+> ## *class* qcpy.`quantumcircuit`(*qubits: int*, *little_endian: bool=False*, *prep: char='z'*)
 
 *Quantum circuit that represents the state of a quantum system and performs operations on select qubits.*
 
 ### Parameters:
 
 `qubits (int)` - number of qubits in the circuit.
 
 `little_endian (bool)` default: `False` - order of qubits and tensor products.
 
 `prep (char)` options: [`z`, `y`, `x`] - initial direction of the qubits' phase angle.
 
 ### Attributes:
 
-`None`
-
-> ## QuantumCircuit.`circuit`()
-
-*Dictionary representation of the circuit*
-
-### Parameters:
-
-`None`
-
-### Returns:
-
-`circuit (dict[int, list[str]])` - key: qubit; value: name of gate.
-
-### Example:
-
-```python
-from QCpy import QuantumCircuit
-
-qc = QuantumCircuit(2)
-
-qc.hadamard(0)
-qc.cnot(0, 1)
-qc.hadamard(0)
-
-print(qc.circuit())
+`state (numpy.ndarray)` -  current state of quantum circuit in matrix representation.
 
-# {0: ['hadamard', 'cnot_control', 'hadamard'], 
-#  1: ['cnot_target']}
-```
 
-> ## QuantumCircuit.`amplitude`(*round=3*)
+> ## quantumcircuit.`amplitude`(*round: int=3*)
 
 *Returns vector of all possible amplitudes for the quantum circuit*
 
 ### Parameters:
 
 `round (int)` - rounding the amplitude to the nearest `round`
 
 ### Returns:
 
 `amplitude (numpy.ndarray[float16])` - amplitude of the quantum circuit.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
-qc.hadamard(0)
+qc.h(0)
 
 print(qc.amplitude())
 
 # [[0.5]
 # [0.5]
 # [0.5]
 # [0.5]]
 ```
 
-> ## QuantumCircuit.`phaseAngle`(*round=2*, *radian=True*)
+> ## quantumcircuit.`phaseangle`(*round: int=2*, *radian: bool=True*)
 
 *Calculates possible phase angles for the quantum circuit*
 
 ### Parameters:
 
-`round (int)` - rounding the amplitude to the nearest `round`
+`round (int)` - round phase angle for readability.
 
 `radian (bool)` - whether or not the values are in radians or degrees.
 
 ### Returns:
 
 `phase_angle (numpy.ndarray)` - array of qubit's phase angle.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.phaseAngle())
+print(qc.phaseangle())
 
 # [[0.        ]
 # [0.         ]
 # [0.         ]
 # [3.14159265]]
 ```
 
-> ## QuantumCircuit.`state`(*round=3*)
+> ## quantumcircuit.`state`
 
 *Returns state of the quantum circuit.*
 
 ### Parameters:
 
-`round (int)` - rounding the state to the nearest `round`
+`None`
 
 ### Returns:
 
-`_state (numpy.ndarray)` - array of quantum circuit's state.
+`state (numpy.ndarray)` - array of quantum circuit's state.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`circuitQueue()`
+> ## quantumcircuit.`flatten(round: int=3)`
+
+*Returns state of the quantum circuit in a 1D array.*
+
+### Parameters:
+
+`round (int)` - round state for readability.
+
+### Returns:
+
+`state (numpy.ndarray)` - array of quantum circuit's state.
+
+### Example:
+
+```python
+from qcpy import quantumcircuit
+
+qc = quantumcircuit(2)
+
+qc.h(0)
+qc.cnot(0, 1)
+
+print(qc.flatten())
+
+# [0.707+0.j 0.   +0.j 0.   +0.j 0.707+0.j]
+```
+
+> ## quantumcircuit.`circuitqueue()`
 
 *Returns queue of gates on quantum circuit.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 `queue (list)` - list of gates queued on quantum circuit.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
 qc = QuantumCircuit(4)
 
 qc.x(0)
 qc.x(1)
 qc.x(2)
 qc.rc3x(0, 1, 2, 3)
 
-print(qc.circuitQueue())
+print(qc.circuitqueue())
 
 # [('X', 0), ('X', 1), ('X', 2), ('U', 3), ('U', 3), ('cnot', 2, # 3), ('U', 3), ('U', 3), ('swap', 2, 3), ('swap', 1, 2), 
 # ('swap', 1, 2), ('swap', 2, 3), ('cnot', 0, 3), ('U', 3),
 # ('swap', 2, 3), ('swap', 2, 3), ('cnot', 1, 3), ('U', 3), 
 # ('swap', 2, 3), ('swap', 1, 2), ('swap', 1, 2), ('swap', 2, 
 # 3), ('cnot', 0, 3), ('U', 3), ('swap', 2, 3), ('swap', 2, 3),
 #  ('cnot', 1, 3), ('U', 3), ('U', 3), ('U', 3), ('cnot', 2, 3),
 #  ('U', 3), ('U', 3), ('rc3x', 0, 1, 2, 3)]
 ```
 
-> ## QuantumCircuit.`probabilities`(*round=3*)
+> ## quantumcircuit.`probabilities`(*show_percent: bool=False*, *show_bit=-1*, *round: int=3*)
 
 *Returns probabilitiy of the qubits within the quantum circuit.*
 
 ### Parameters:
 
-`round (int)` - rounding the probabilities to the nearest `round`
+`show_percent (bool)` - convert probability to be shown in percentage.
+
+`show_bit (int or str)` - get the probability of a single bit with a given string of binary or a integer.
+
+`round (int)` - rounding the probabilities to the nearest `round`.
 
 ### Returns:
 
 `prob_matrix (numpy.ndarray)` - array of quantum circuit's probabilities.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cnot(0, 1)
 
 print(qc.probabilities())
 
 # [0.5 0.  0.  0.5]
 ```
 
-> ## QuantumCircuit.`measure`()
+> ## quantumcircuit.`measure`()
 
 *Collapses the state based on the quantum circuit's probabilities.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 
 `final_state (numpy.ndarray)` - array of quantum circuit's measurement.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
 
 print(qc.measure())
 
-# ~Results may vary~
 # 00
 ```
 
-> ## QuantumCircuit.`reverse`()
+> ## quantumcircuit.`reverse`()
 
 *Reverses the quantum circuit's values.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.state())
+print(qc.state)
 
 qc.reverse()
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
  
 # [[0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
-> ## QuantumCircuit.`toffoli`(*control_1*, *control_2*, *target*)
+> ## quantumcircuit.`toffoli`(*control_1: int*, *control_2: int*, *target: int*)
 
 *A 3-qubit quantum gate that takes in two control qubits and one target qubit.*
 
 ### Parameters:
 
 `control_1 (int)` - first control qubit.
 
@@ -751,37 +905,37 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
 qc.toffoli(0,1,2)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j]
 # [0. +0.j]
 # [0.5+0.j]
 # [0. +0.j]
 # [0.5+0.j]
 # [0. +0.j]
 # [0. +0.j]
 # [0.5+0.j]]
 ```
 
-> ## QuantumCircuit.`rccx`(*control_1*, *control_2*, *target*)
+> ## quantumcircuit.`rccx`(*control_1*, *control_2*, *target*)
 
 *A 3-qubit quantum gate that takes in two control qubits and one target qubit.*
 
 ### Parameters:
 
 `control_1 (int)` - first control qubit.
 
@@ -792,68 +946,68 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(3)
+from qcpy import quantumcircuit
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
 qc.rccx(0,1,2)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.5-0.j ]
 # [ 0. +0.j ]
 # [ 0.5-0.j ]
 # [ 0. +0.j ]
 # [ 0.5-0.j ]
 # [ 0. +0.j ]
 # [-0. +0.j ]
 # [ 0. +0.5j]]
 ```
 
-> ## QuantumCircuit.`rc3x`(*a*, *b*, *c*, *d*)
+> ## quantumcircuit.`rc3x`(*qubit_1: int*, *qubit_2: int*, *qubit_3: int*, *qubit_4: int*)
 
 *A 4-qubit quantum gate that takes in 4 unique qubits.*
 
 ### Parameters:
 
-`a (int)` - first input qubit.
+`qubit_1 (int)` - first input qubit.
 
-`b (int)` - second input qubit.
+`qubit_2 (int)` - second input qubit.
 
-`c (int)` - third input qubit.
+`qubit_3 (int)` - third input qubit.
 
-`d (int)` - fourth input qubit.
+`qubit_4 (int)` - fourth input qubit.
 
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(4)
+from qcpy import quantumcircuit
+qc = quantumcircuit(4)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
-qc.hadamard(2)
+qc.h(2)
 
-qc.rc3x(0,1,2)
+qc.rc3x(0,1,2,3)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
@@ -864,15 +1018,15 @@
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.   +0.354j]
 # [-0.   +0.j   ]
 # [ 0.   -0.j   ]
 # [-0.354+0.j   ]]
 ```
-> ## QuantumCircuit.`cnot`(*control*, *target*)
+> ## quantumcircuit.`cnot`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -881,30 +1035,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cnot(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`cr`(*control*, *target*)
+> ## quantumcircuit.`cr`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -913,31 +1067,31 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cr(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
 
-> ## QuantumCircuit.`cz`(*control*, *target*)
+> ## quantumcircuit.`cz`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -946,30 +1100,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cz(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`swap`(*qubit_1*, *qubit_2*)
+> ## quantumcircuit.`swap`(*qubit_1: int*, *qubit_2: int*)
 
 *A 2-qubit quantum gate that takes in 2 qubits to swap there properties.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit to swap.
 
@@ -978,30 +1132,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.swap(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`rxx`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rxx`(*qubit_1: int*, *qubit_2: int*, *theta: float=numpy.pi/2*)
 
 *A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit input.
 
@@ -1011,30 +1165,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rxx(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j ]
 # [0. -0.5j]
 # [0.5+0.j ]
 # [0. -0.5j]]
 ```
 
-> ## QuantumCircuit.`rzz`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rzz`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
 
 *A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit input.
 
@@ -1045,211 +1199,209 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rxx(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j ]
 # [0. -0.5j]
 # [0.5+0.j ]
 # [0. -0.5j]]
 ```
 
-> ## QuantumCircuit.`customControlPhase`(*control*, *target*, *custom_matrix*)
+> ## quantumcircuit.`customcontrolled`(*control: int*, *target: int*, *custom_matrix: np.array*)
 
 *Used to insert single qubit based quantum gates to have a control qubit apart of it and committing to the quantum state.*
 
 ### Parameters:
 
 `control (int)` - control qubit for given matrix.
 
 `target (int)` - target qubit for given matrix.
 
-`custom_matrix (np.array)` -  matrix to be applied to the quantum circuit.
+`custom_matrix (np.array)` - (2,2) matrix to be applied to the quantum circuit.
 
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-
-from QCpy.QuantumGate import PauliX
+from qcpy import quantumcircuit, paulix
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.customControlPhase(0,1, PauliX().matrix)
+qc.customcontrolled(0,1, paulix())
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`identity`(*qubit*)
+> ## quantumcircuit.`i`(*qubit: int*)
 
 *Used to confirm value that a qubit is representing and does nothing to manipulate the value of such qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the identity gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.identity(0)
+qc.i(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[1.+0.j]
 # [0.+0.j]
 # [0.+0.j]
 # [0.+0.j]]
 ```
 
-> ## QuantumCircuit.`x`(*qubit*)
+> ## quantumcircuit.`x`(*qubit: int*)
 
 *Used to invert the value of what a qubit is representing.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-X gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.x(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [1.+0.j]
 # [0.+0.j]]
 ```
 
 
-> ## QuantumCircuit.`hadmard`(*qubit*)
+> ## quantumcircuit.`hadmard`(*qubit: int*)
 
 *Used to put a given qubit into superposition.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Hadamard gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`y`(*qubit*)
+> ## quantumcircuit.`y`(*qubit: int*)
 
 *Changes the state of a qubit by pi around the y-axis of a Bloch Sphere.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Y gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.y(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [0.+1.j]
 # [0.+0.j]]
 ```
 
 
-> ## QuantumCircuit.`z`(*qubit*)
+> ## quantumcircuit.`z`(*qubit: int*)
 
 *Changes the state of a qubit by pi around the z-axis of a Bloch Sphere.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Z gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.z(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.707+0.j]
 # [ 0.   +0.j]
 # [-0.707+0.j]
 # [ 0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`phase`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`phase`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *Commits to a rotation around the z-axis based off of the inputted theta value.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Phase gate be applied to the quantum wire.
 
@@ -1257,151 +1409,151 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.phase(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   +0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`s`(*qubit*)
+> ## quantumcircuit.`s`(*qubit: int*)
 
 *Is a Phase gate where the inputted theta value is given as a constant of theta = pi / 2.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Z gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.s(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   +0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`sdg`(*qubit*)
+> ## quantumcircuit.`sdg`(*qubit: int*)
 
 *Is a Phase gate and inverse of the S gate where the inputted theta value is given as a constant of theta = -pi / 2.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Sdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.sdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   -0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`t`(*qubit*)
+> ## quantumcircuit.`t`(*qubit: int*)
 
 *T gate is a special use case gate that in implemented from the P Gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the T gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.t(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j ]
 # [0.   +0.j ]
 # [0.5  +0.5j]
 # [0.   +0.j ]]
 ```
 
-> ## QuantumCircuit.`tdg`(*qubit*)
+> ## quantumcircuit.`tdg`(*qubit: int*)
 
 *Tdg gate is a special use case gate that in implemented from the P Gate and is the inverse of the T gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Tdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.tdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j ]
 # [0.   +0.j ]
 # [0.5  -0.5j]
 # [0.   +0.j ]]
 ```
 
-> ## QuantumCircuit.`rz`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rz`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RZ gate commits a rotation around the z-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Rz gate be applied to the quantum wire.
 
@@ -1409,31 +1561,31 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rz(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`ry`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`ry`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RY gate commits a rotation around the y-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Ry gate be applied to the quantum wire.
 
@@ -1441,29 +1593,29 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.ry(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`rx`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rx`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RX gate commits a rotation around the x-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Ry gate be applied to the quantum wire.
 
@@ -1471,85 +1623,85 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumCircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.rx(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   -0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`sx`(*qubit*)
+> ## quantumcircuit.`sx`(*qubit: int*)
 
 *SX gate is the square root of the Inverse gate (X, PauliX Gate).*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Sx gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.sx(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.5j]
 # [0. +0.j ]
 # [0.5-0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`sxdg`(*qubit*)
+> ## quantumcircuit.`sxdg`(*qubit: int*)
 
 *SXDG gate is the negative square root of the Inverse gate (X, PauliX Gate) and inverse of the SX gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the SXdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.sxdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`u`(*qubit*, *theta=numpy.pi/2*, *phi=numpy.pi/2*, *lmbda=numpy.pi/2*)
+> ## quantumcircuit.`u`(*qubit: int*, *theta: float=numpy.pi/2*, *phi: float=numpy.pi/2*, *lmbda: float=numpy.pi/2*)
 
 *U gate is given three inputs (theta, phi, and lambda) that allow the inputs to manipulate the base matrix to allow for the position of the enacted qubit around the bloch sphere representation.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the U gate be applied to the quantum wire.
 
@@ -1561,29 +1713,29 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.u(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`custom`(*qubit*, *custom_matrix*)
+> ## quantumcircuit.`custom`(*qubit: int*, *custom_matrix: np.array*)
 
 *Will take in a custom single qubit quantum gate and implement it on a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the U gate be applied to the quantum wire.
 
@@ -1591,47 +1743,45 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-
-from QCpy.QuantumGate import PauliX
+from qcpy import quantumcircuit, paulix
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.custom(0, PauliX().matrix)
+qc.custom(0, paulix())
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [1.+0.j]
 # [0.+0.j]]
 ```
 
 # Visualizer
 
 *A collection of classes to visualize the quantum circuit*
 
-> ## *class* QCpy.Visualizer.QSphere(*circuit*)
+> ## *class* qcpy.qsphere(*circuit*)
 
 *Visualizes the quantum circuit as a q-sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## QSphere.`makeSphere`(*path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## qsphere.`make`(*path: str="qsphere.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a Q-Sphere that plots a global visualization of the quantum states in a 3D global view*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1644,40 +1794,39 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, qsphere
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-sphere_ex = QSphere(qc)
-sphere_ex.makeSphere(save=False, show=True)
+sphere_ex = qsphere(qc)
+sphere_ex.make(save=False, show=True)
 ```
 
-> ## *class* QC.Visualizer.BlochSphere(*circuit*)
+> ## *class* qcpy.bloch(*circuit*)
 
 *Visualizes the quantum state of a single qubit as a sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## BlochSphere.`makeSphere`(*show_bit=0*, *path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## blochsphere.`make`(*show_bit: int=0*, *path: str="qsphere.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a Bloch Sphere that plots the quantum state of a single qubit in a 3D global view*
 
 ### Parameters:
 
 `show_bit (int)` - the qubit on the circuit to be visualized, initialized as the 0th bit
 
@@ -1692,40 +1841,39 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, bloch
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-sphere_ex = BlochSphere(qc)
-sphere_ex.makeSphere(show_bit=1, save=False, show=True)
+sphere_ex = bloch(qc)
+sphere_ex.make(show_bit=1, save=False, show=True)
 ```
 
-> ## *class* QCpy.Visualizer.StateVector(*circuit*)
+> ## *class* qcpy.statevector(*circuit*)
 
 *Visualizes the quantum circuit's quantum amplitutes using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## StateVector.`makeGraph`(*path="statevector.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## statevector.`make`(*path: str="statevector.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a graph that plots all the amplitudes of the qubits being measured*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1738,40 +1886,38 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, statevector
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-stateVector_ex = StateVector(qc)
-stateVector_ex.makeGraph(save=False, show=True)
+statevector(qc).make(save=False, show=True)
 ```
 
-> ## *class* QCpy.Visualizer.Probabilities(*circuit*)
+> ## *class* qcpy.probability(*circuit*)
 
 *Visualizes the quantum circuit's qubits probability of being measured using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## Probabilities.`makeGraph`(*path="probabilities.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## probability.`make`(*path: str="probability.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a graph that plots all the probabilities of the qubits being measured*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1784,19 +1930,17 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, probability
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-probabilities_ex = Probabilities(qc)
-probabilities_ex.makeGraph(save=False, show=True)
+probability(qc).make(save=False, show=True)
 ```
```

### Comparing `QCpython-1.0.3/README.md` & `qcpython-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,732 +1,886 @@
 # README.md
 
 # QCpy - A Quantum Computing Library for Python
 
-QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing (QC).
+QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing.
 
 You can download the package using pip:
 
 ```txt
-pip install QCpython
+pip install qcpython
 ```
-
-## Recommended Resources on Quantum Computing:
-
-- [Microsoft’s Linear Algebra for Quantum Computing](https://learn.microsoft.com/en-us/azure/quantum/overview-algebra-for-quantum-computing)
-- [IBM’s Quantum Computing: a field guide](https://quantum-computing.ibm.com/composer/docs/iqx/guide/)
-- [Wikipedia: Quantum Computing](https://en.wikipedia.org/wiki/Quantum_computing)
-
 ---
 
-# Qubits
+# Qubit
 
-> ## *class* QCpy.`Qubit`(*initial_state=’z’*)
+> ## qcpy.`qubit`(*initial_state=’z’*)
 
 *Object representation of a qubit.*
 
 ### Parameters:
 
-`initial_state (chr)` - Character input for starting direction in the *x*, *y*, or *z* axis.
+`initial_state (chr)` default: `z` - Character input for starting direction in the *x*, *y*, or *z* axis.
 
 ### Attributes:
 
-`state (numpy.ndarray)` -  current state of qubit in matrix representation.
+`None`
+
+### Example:
+
+```python
+from qcpy import qubit
 
+qx = qubit(initial_state = 'x')
+qy = qubit(initial_state = 'y')
+qz = qubit(initial_state = 'z')
+print("qx:\n", qx)
+print("qy:\n", qy)
+print("qz:\n", qz)
+
+
+# qx:
+#  [[0.70710677+0.j]
+#  [0.70710677+0.j]]
+# qy:
+#  [[0.70710677+0.j]
+#  [0.+0.70710677j]]
+# qz:
+#  [[1.+0.j]
+#  [0.+0.j]]
+```
 ---
 
 # Quantum Gates
 
-> ## *class* QC.QuantumGate.`Identity`()
+> ## quantumgate.`identity`()
 
 *Gate that does not modify the quantum state.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Identity gate.
-
 ```python
-Identity.matrix = [1+0j, 0+0j], 
-	          [0+0j, 1+0j]
+identity=[1+0j, 0+0j], 
+         [0+0j, 1+0j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`PauliX`()
+```python
+from qcpy import identity 
+
+print(identity())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j]]
+```
+> ## quantumgate.`paulix`()
 
 *Quantum equivalent of the NOT gate in classical computing with respect to the standard basis |0>, |1>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-X gate.
-
 ```python
-PauliX.matrix = [0+0j, 1+0j], 
-	        [1+0j, 0+0j]
+PauliX = [0+0j, 1+0j], 
+	 [1+0j, 0+0j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`PauliY`()
+```python
+from qcpy import paulix
+
+print(paulix())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j]]
+```
+> ## quantumgate.`pauliy`()
 
 *Rotation around y-axis of the bloch sphere by π radiains, mapping |0> to i|1> and |1> to -i|0>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-Y gate.
-
 ```python
-PauliY.matrix = [0+0j, 0-1j],
-                [0+1j, 0+0j]
+PauliY = [0+0j, 0-1j],
+         [0+1j, 0+0j]
 ```
+### Example:
+
+```python
+from qcpy import pauliy
+
+print(pauliy())
 
-> ## *class* QC.QuantumGate.`PauliZ`()
+# [[0+0j, 0-1j]
+#  [0+1j, 0+0j]]
+```
+> ## quantumgate.`pauliz`()
 
 *Rotation around z-axis of the bloch sphere by π radiains, mapping |1> to -|1>; known as the phase-flip.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Pauli-Z gate.
-
 ```python
-PauliZ.matrix = [1+0j, 0+0j], 
-                [0+0j, -1+0j]
+PauliZ = [1+0j, 0+0j], 
+         [0+0j, -1+0j]
 ```
+### Example:
+
+```python
+from qcpy import pauliz
 
-> ## *class* QC.QuantumGate.`Hadamard`()
+print(pauliz())
+
+# [[1+0j, 0+0j], 
+#  [0+0j, -1+0j]]
+```
+> ## quantumgate.`hadamard`()
 
 *Maps the basis states |0> to |+> and |1> to |->, creating a superposition state if given a computation basis state.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Hadamard gate.
-
 ```python
-Hadamard.matrix = ([1,  1] 
-                   [1, -1]) * (1/sqrt(2))
+Hadamard = [1,  1] 
+           [1, -1] * (1/sqrt(2))
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`CNot`(*inverse=False*)
+```python
+from qcpy import hadamard
 
-*Controlled gate acts on two or more qubits, performing the NOT operation of the target qubit only if the control qubits are |1>, can act as a quantum regiester and is used to entangle and disentangle Bell states.*
+print(hadamard())
 
-### Parameters:
+# [[ 0.70710677+0.j  0.70710677+0.j]
+#  [ 0.70710677+0.j -0.70710677+0.j]]
+```
+> ## quantumgate.`cnot`(*little_endian=False*)
 
-`inverse (bool)` - if the gate is an inverse, with the target being above the control.
+*Controlled gate acts on two or more qubits, performing the NOT operation of the target qubit only if the control qubits are |1>, can act as a quantum regiester and is used to entangle and disentangle Bell states.*
 
-### Attributes:
+### Parameters:
 
-`matrix (np.ndarray)` - matrix representation of CNOT gate.
+`little_endian (bool)` - if the gate is an inverse, with the target being above the control.
 
 ```python
 # regular
-CNot.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j]
-# inverse
-CNot.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j] 
+CNot = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j]
+# little_endian = True
+CNot = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j] 
 ```
+### Example:
+
+```python
+from qcpy import cnot
+
+print(cnot())
+
+# [[1.+0.j 0.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 0.+0.j 0.+0.j 1.+0.j]
+#  [0.+0.j 0.+0.j 1.+0.j 0.+0.j]]
 
-> ## *class* QC.QuantumGate.`Swap`()
+# [[1.+0.j 0.+0.j 0.+0.j 0.+0.j]
+#  [0.+0.j 0.+0.j 0.+0.j 1.+0.j]
+#  [0.+0.j 0.+0.j 1.+0.j 0.+0.j]
+#  [0.+0.j 1.+0.j 0.+0.j 0.+0.j]]
+```
+> ## quantumgate.`swap`()
 
 *Swaps two qubits, with respect to the basis |00>, |01>, |10>, and |11>.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of SWAP gate.
-
 ```python
-Swap.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 1+0j, 0+0j],
-              [0+0j, 1+0j, 0+0j, 0+0j],
-              [0+0j, 0+0j, 0+0j, 1+0j]
+Swap = [1+0j, 0+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 1+0j, 0+0j],
+       [0+0j, 1+0j, 0+0j, 0+0j],
+       [0+0j, 0+0j, 0+0j, 1+0j]
 ```
+### Example:
+
+```python
+from qcpy import swap
 
-> ## *class* QC.QuantumGate.`Toffoli`()
+print(swap())
+
+# [1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j]
+```
+> ## quantumgate.`toffoli`()
 
 *Universal reversible logic gate, known as the “controlled-controlled-NOT” gate; if the two control bits are set to 1, it will invert the target.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Toffoli gate.
-
 ```python
-Toffoli.matrix = [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
-                 [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+Toffoli = [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+          [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
 ```
+### Example:
+
+```python
+from qcpy import toffoli
 
-> ## *class* QC.QuantumGate.`Phase`(*theta=numpy.pi/2*)
+print(toffoli())
+
+# [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+```
+> ## quantumgate.`phase`(*theta=numpy.pi/2*)
 
 *Applies a rotation of theta around the z-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around z-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of Phase gate.
-
 ```python
-Phase.matrix = [1+0j, 0+0j],
-	       [0+0j, numpy.exp(0+1j * theta)]
+Phase = [1+0j, 0+0j],
+	[0+0j, numpy.exp(0+1j * theta)]
 ```
+### Example:
+
+```python
+from qcpy import phase
 
-> ## *class* QC.QuantumGate.`S`()
+print(phase())
+
+# [1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j, 0+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j],
+# [0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 0+0j, 1+0j, 0+0j]
+```
+> ## quantumgate.`s`()
 
 *Equivalent to a pi/2 rotation around the z-axis.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of S gate.
-
 ```python
 S.matrix = [1+0j, 0+0j],
            [0+0j, 0+1j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Sdg`()
+```python
+from qcpy import s
+
+print(s())
+
+# [1+0j, 0+0j],
+# [0+0j, 0+1j]
+```
+> ## quantumgate.`sdg`()
 
 *Inverse of S gate; a -pi/2 rotation around the z-axis.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an inverse S gate.
-
 ```python
 Sdg.matrix = [1+0j, 0+0j],
              [0+0j, 0-1j]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`T`()
+```python
+from qcpy import sdg
+
+print(sdg())
+
+# [1+0j, 0+0j],
+# [0+0j, 0-1j]
+```
+> ## quantumgate.`t`()
 
 *Square of S gate; where T = S^2.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a T gate.
-
 ```python
 T.matrix = [1+0j, 0+0j],
            [0+0j, numpy.exp((0+1j * numpy.pi) / 4)]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Tdg`()
+```python
+from qcpy import t
+
+print(t())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 0.70710677+0.70710677j]]
+```
+> ## quantumgate.`tdg`()
 
 *Inverse of T gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a inverse of T gate.
-
 ```python
-Tdg.matrix = [1+0j, 0+0j],
-             [0+0j, numpy.exp((0-1j * numpy.pi) / 4)]
+Tdg = [1+0j, 0+0j],
+      [0+0j, numpy.exp((0-1j * numpy.pi) / 4)]
 ```
+### Example:
+
+```python
+from qcpy import tdg
 
-> ## *class* QC.QuantumGate.`Rz`(*theta=numpy.pi/2*)
+print(tdg())
+
+# [[1.+0.j 0.+0.j]
+#  [0.+0.j 0.70710677-0.70710677j]]
+```
+> ## quantumgate.`rz`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the z-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around z-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rz gate.
-
 ```python
-Rz.matrix = [numpy.exp((0-1j * (theta / 2))), 0+0j],
-            [0+0j, numpy.exp(0+1j * (theta / 2))]
+Rz = [numpy.exp((0-1j * (theta / 2))), 0+0j],
+     [0+0j, numpy.exp(0+1j * (theta / 2))]
 ```
 
-> ## *class* QC.QuantumGate.`Rx`(*theta=numpy.pi/2*)
+> ## quantumgate.`rx`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the x-axis.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around x-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rx gate.
-
 ```python
-Rx.matrix = [numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2)],
-            [0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2)]
+Rx = [numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2)],
+     [0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2)]
 ```
+### Example:
+
+```python
+from qcpy import rx
 
-> ## *class* QC.QuantumGate.`Ry`(*theta=numpy.pi/2*)
+print(rx())
+
+# [[0.70710677+0.j 0.-0.70710677j]
+#  [0.-0.70710677j 0.70710677+0.j]]
+```
+> ## quantumgate.`ry`(*theta=numpy.pi/2*)
 
 *Rotation of qubit around the y-axis.*
 
 ### Parameters:
 
 `theta (float)`default: `numpy.pi/2` -  angle of rotation around y-axis.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Ry gate.
-
 ```python
-Ry.matrix = [numpy.cos(theta / 2), -1 * numpy.sin(theta / 2)],
-            [numpy.sin(theta / 2), numpy.cos(theta / 2)]
+Ry = [numpy.cos(theta / 2), -1 * numpy.sin(theta / 2)],
+     [numpy.sin(theta / 2), numpy.cos(theta / 2)]
 ```
+### Example:
+
+```python
+from qcpy import ry
 
-> ## *class* QC.QuantumGate.`Sx`()
+print(ry())
+
+# [[ 0.70710677+0.j -0.70710677+0.j]
+#  [ 0.70710677+0.j  0.70710677+0.j]]
+```
+> ## quantumgate.`sx`()
 
 *Rotation around the x-axis by 90 degrees in the counter-clockwise direction. Also known as the “square-root X gate” due to the fact that applying the SX gate twice results in an X gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Sx gate.
-
 ```python
-Sx.matrix = [1+1j, 1-1j], 
-            [1-1j, 1+1j]]) * (1 / 2)
+Sx = [1+1j, 1-1j], 
+     [1-1j, 1+1j] * (1 / 2)
 ```
+### Example:
+
+```python
+from qcpy import sx
 
-> ## *class* QC.QuantumGate.`Sxdg`()
+print(sx())
+
+# [[0.5+0.5j 0.5-0.5j]
+#  [0.5-0.5j 0.5+0.5j]]
+```
+> ## quantumgate.`sxdg`()
 
 *Inverse of the Sx gate.*
 
 ### Parameters:
 
 `None`
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an inverse Sx gate.
-
 ```python
-Sxdg.matrix = [1-1j, 1+1j], 
-              [1+1j, 1-1j]]) * (1 / 2)
+Sxdg = [1-1j, 1+1j], 
+       [1+1j, 1-1j] * (1 / 2)
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`U`(*theta=numpy.pi/2, phi=numpy.pi/2, lmbda=numpy.pi/2*)
+```python
+from qcpy import sxdg
+
+print(sxdg())
+
+# [[0.5-0.5j 0.5+0.5j]
+#  [0.5+0.5j 0.5-0.5j]]
+```
+> ## quantumgate.`u`(*theta=numpy.pi/2, phi=numpy.pi/2, lmbda=numpy.pi/2*)
 
 *Rotation of qubit with respect to theta, phi, and lambda, in Euler angles.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around Euler angle theta.
 
 `phi (float)` default: `numpy.pi/2` -  angle of rotation around Euler angle phi.
 
 `lmbda (float)` default: `numpy.pi/2` -  angle of rotation around Eulear angle lambda.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of a U gate.
-
 ```python
 U.matrix = [numpy.cos(theta / 2), -1 * numpy.exp(0+1j * lmbda) * numpy.sin(theta / 2)], 
            [numpy.exp(0+1j * phi) * numpy.sin(theta / 2), numpy.exp(0+1j * (lmbda + phi)) * numpy.cos(theta / 2)]]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Rxx`(*theta=numpy.pi/2*)
+```python
+from qcpy import u
+
+print(u())
+
+# [[0.7071+0.j -0.-0.7071j]
+#  [0.+0.7071j -0.7071+0.j]]
+```
+> ## quantumgate.`rxx`(*theta=numpy.pi/2*)
 
 *Rotation about XX, maximally entangling at theta = pi/2.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around XX.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rxx gate.
-
 ```python
 Rxx.matrix = [numpy.cos(theta / 2), 0+0j, 0+0j, 0-1j * numpy.sin(theta / 2)],
              [0+0j, numpy.cos(theta / 2), 0-1j * numpy.sin(theta / 2), 0+0j],
              [0+0j, 0-1j * numpy.sin(theta / 2), numpy.cos(theta / 2), 0+0j],
              [0-1j * numpy.sin(theta / 2), 0+0j, 0+0j, numpy.cos(theta / 2)]
 ```
+### Example:
 
-> ## *class* QC.QuantumGate.`Rzz`(*theta=numpy.pi/2*)
+```python
+from qcpy import rxx
+
+print(rxx())
+
+# [[0.70710677+0.j 0+0.j 0+0.j 0-0.70710677j]
+#  [0+0.j 0.70710677+0.j 0-0.70710677j 0+0.j]
+#  [0+0.j 0-0.70710677j 0.70710677+0.j 0+0.j]
+#  [0-0.70710677j 0+0.j 0.+0.j 0.70710677+0.j]]
+```
+> ## quantumgate.`rzz`(*theta=numpy.pi/2*)
 
 *Rotation about ZZ, maximally entangling at theta = pi/2.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation around ZZ.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Rzz gate.
-
 ```python
 Rzz.matrix = [numpy.exp(0-1j * (theta / 2)), 0+0j, 0+0j, 0+0j],
              [0+0j, numpy.exp(0+1j * (theta / 2)), 0+0j, 0+0j],
              [0+0j, 0+0j, numpy.exp(0+1j * (theta / 2)), 0+0j],
              [0+0j, 0+0j, 0+0j, numpy.exp(0-1j * (theta / 2))]
 ```
+### Example:
+
+```python
+from qcpy import rzz
 
-> ## *class* QC.QuantumGate.`Cr`(*theta=numpy.pi/2*)
+print(rzz())
+
+# [[0.70710677-0.70710677j 0+0.j 0+0.jn 0+0.j]
+#  [0+0.j 0.70710677+0.70710677j 0+0.j 0+0.j]
+#  [0+0.j 0+0.j 0.70710677+0.70710677j 0+0.j]
+#  [0+0.j 0+0.j 0+0.j 0.70710677-0.70710677j]]
+```
+> ## quantumgate.`cr`(*theta=numpy.pi/2*)
 
 *Controlled phase shift rotation in theta radians; generalization of Cz gate.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation in theta radians.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Cr gate.
-
 ```python
-Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-            [0+0j, 1+0j, 0+0j, 0+0j],
-            [0+0j, 0+0j, 1+0j, 0+0j],
-            [0+0j, 0+0j, 0+0j, numpy.exp(theta * 0+1j)]
+Cr = [1+0j, 0+0j, 0+0j, 0+0j],
+     [0+0j, 1+0j, 0+0j, 0+0j],
+     [0+0j, 0+0j, 1+0j, 0+0j],
+     [0+0j, 0+0j, 0+0j, exp(theta * 0+1j)]
 ```
+### Example:
+
+```python
+from qcpy import cr
 
-> ## *class* QC.QuantumGate.`Cz`(*theta=numpy.pi/2*)
+print(cr())
+
+# [[1+0.j 0+0.j 0+0.j 0+0.j]
+#  [0+0.j 1+0.j 0+0.j 0+0.j]
+#  [0+0.j 0+0.j 1+0.j 0+0.j]
+#  [0+0.j 0+0.j 0+0.j 0.5403023+0.84147096j]]
+```
+> ## quantumgate.`cz`(*theta=numpy.pi/2*)
 
 *Controlled phase shift rotation in theta radians.*
 
 ### Parameters:
 
 `theta (float)` default: `numpy.pi/2` -  angle of rotation in theta radians.
 
-### Attributes:
-
-`matrix (np.ndarray)` - matrix representation of an Cz gate.
+```python
+Cz = [1+0j, 0+0j, 0+0j, 0+0j],
+     [0+0j, 1+0j, 0+0j, 0+0j],
+     [0+0j, 0+0j, 1+0j, 0+0j],
+     [0+0j, 0+0j, 0+0j, -1+0j]
+```
+### Example:
 
 ```python
-Cz.matrix = [1+0j, 0+0j, 0+0j, 0+0j],
-            [0+0j, 1+0j, 0+0j, 0+0j],
-            [0+0j, 0+0j, 1+0j, 0+0j],
-            [0+0j, 0+0j, 0+0j, -1+0j]
+from qcpy import cz
+
+print(cz())
+
+# [[ 1.+0.j  0.+0.j  0.+0.j  0.+0.j]
+#  [ 0.+0.j  1.+0.j  0.+0.j  0.+0.j]
+#  [ 0.+0.j  0.+0.j  1.+0.j  0.+0.j]
+#  [ 0.+0.j  0.+0.j  0.+0.j -1.+0.j]]
 ```
 ---
 # Quantum Circuit
-> ## *class* QCpy.`QuantumCircuit`(*qubits*, *little_endian=False*, *prep='z'*)
+> ## *class* qcpy.`quantumcircuit`(*qubits: int*, *little_endian: bool=False*, *prep: char='z'*)
 
 *Quantum circuit that represents the state of a quantum system and performs operations on select qubits.*
 
 ### Parameters:
 
 `qubits (int)` - number of qubits in the circuit.
 
 `little_endian (bool)` default: `False` - order of qubits and tensor products.
 
 `prep (char)` options: [`z`, `y`, `x`] - initial direction of the qubits' phase angle.
 
 ### Attributes:
 
-`None`
-
-> ## QuantumCircuit.`circuit`()
+`state (numpy.ndarray)` -  current state of quantum circuit in matrix representation.
 
-*Dictionary representation of the circuit*
 
-### Parameters:
-
-`None`
-
-### Returns:
-
-`circuit (dict[int, list[str]])` - key: qubit; value: name of gate.
-
-### Example:
-
-```python
-from QCpy import QuantumCircuit
-
-qc = QuantumCircuit(2)
-
-qc.hadamard(0)
-qc.cnot(0, 1)
-qc.hadamard(0)
-
-print(qc.circuit())
-
-# {0: ['hadamard', 'cnot_control', 'hadamard'], 
-#  1: ['cnot_target']}
-```
-
-> ## QuantumCircuit.`amplitude`(*round=3*)
+> ## quantumcircuit.`amplitude`(*round: int=3*)
 
 *Returns vector of all possible amplitudes for the quantum circuit*
 
 ### Parameters:
 
 `round (int)` - rounding the amplitude to the nearest `round`
 
 ### Returns:
 
 `amplitude (numpy.ndarray[float16])` - amplitude of the quantum circuit.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
-qc.hadamard(0)
+qc.h(0)
 
 print(qc.amplitude())
 
 # [[0.5]
 # [0.5]
 # [0.5]
 # [0.5]]
 ```
 
-> ## QuantumCircuit.`phaseAngle`(*round=2*, *radian=True*)
+> ## quantumcircuit.`phaseangle`(*round: int=2*, *radian: bool=True*)
 
 *Calculates possible phase angles for the quantum circuit*
 
 ### Parameters:
 
-`round (int)` - rounding the amplitude to the nearest `round`
+`round (int)` - round phase angle for readability.
 
 `radian (bool)` - whether or not the values are in radians or degrees.
 
 ### Returns:
 
 `phase_angle (numpy.ndarray)` - array of qubit's phase angle.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.phaseAngle())
+print(qc.phaseangle())
 
 # [[0.        ]
 # [0.         ]
 # [0.         ]
 # [3.14159265]]
 ```
 
-> ## QuantumCircuit.`state`(*round=3*)
+> ## quantumcircuit.`state`
 
 *Returns state of the quantum circuit.*
 
 ### Parameters:
 
-`round (int)` - rounding the state to the nearest `round`
+`None`
 
 ### Returns:
 
-`_state (numpy.ndarray)` - array of quantum circuit's state.
+`state (numpy.ndarray)` - array of quantum circuit's state.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`circuitQueue()`
+> ## quantumcircuit.`flatten(round: int=3)`
+
+*Returns state of the quantum circuit in a 1D array.*
+
+### Parameters:
+
+`round (int)` - round state for readability.
+
+### Returns:
+
+`state (numpy.ndarray)` - array of quantum circuit's state.
+
+### Example:
+
+```python
+from qcpy import quantumcircuit
+
+qc = quantumcircuit(2)
+
+qc.h(0)
+qc.cnot(0, 1)
+
+print(qc.flatten())
+
+# [0.707+0.j 0.   +0.j 0.   +0.j 0.707+0.j]
+```
+
+> ## quantumcircuit.`circuitqueue()`
 
 *Returns queue of gates on quantum circuit.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 `queue (list)` - list of gates queued on quantum circuit.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
 qc = QuantumCircuit(4)
 
 qc.x(0)
 qc.x(1)
 qc.x(2)
 qc.rc3x(0, 1, 2, 3)
 
-print(qc.circuitQueue())
+print(qc.circuitqueue())
 
 # [('X', 0), ('X', 1), ('X', 2), ('U', 3), ('U', 3), ('cnot', 2, # 3), ('U', 3), ('U', 3), ('swap', 2, 3), ('swap', 1, 2), 
 # ('swap', 1, 2), ('swap', 2, 3), ('cnot', 0, 3), ('U', 3),
 # ('swap', 2, 3), ('swap', 2, 3), ('cnot', 1, 3), ('U', 3), 
 # ('swap', 2, 3), ('swap', 1, 2), ('swap', 1, 2), ('swap', 2, 
 # 3), ('cnot', 0, 3), ('U', 3), ('swap', 2, 3), ('swap', 2, 3),
 #  ('cnot', 1, 3), ('U', 3), ('U', 3), ('U', 3), ('cnot', 2, 3),
 #  ('U', 3), ('U', 3), ('rc3x', 0, 1, 2, 3)]
 ```
 
-> ## QuantumCircuit.`probabilities`(*round=3*)
+> ## quantumcircuit.`probabilities`(*show_percent: bool=False*, *show_bit=-1*, *round: int=3*)
 
 *Returns probabilitiy of the qubits within the quantum circuit.*
 
 ### Parameters:
 
-`round (int)` - rounding the probabilities to the nearest `round`
+`show_percent (bool)` - convert probability to be shown in percentage.
+
+`show_bit (int or str)` - get the probability of a single bit with a given string of binary or a integer.
+
+`round (int)` - rounding the probabilities to the nearest `round`.
 
 ### Returns:
 
 `prob_matrix (numpy.ndarray)` - array of quantum circuit's probabilities.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cnot(0, 1)
 
 print(qc.probabilities())
 
 # [0.5 0.  0.  0.5]
 ```
 
-> ## QuantumCircuit.`measure`()
+> ## quantumcircuit.`measure`()
 
 *Collapses the state based on the quantum circuit's probabilities.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 
 `final_state (numpy.ndarray)` - array of quantum circuit's measurement.
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 qc.cnot(0, 1)
 
 print(qc.measure())
 
-# ~Results may vary~
 # 00
 ```
 
-> ## QuantumCircuit.`reverse`()
+> ## quantumcircuit.`reverse`()
 
 *Reverses the quantum circuit's values.*
 
 ### Parameters:
 
 `None`
 
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.state())
+print(qc.state)
 
 qc.reverse()
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
  
 # [[0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
-> ## QuantumCircuit.`toffoli`(*control_1*, *control_2*, *target*)
+> ## quantumcircuit.`toffoli`(*control_1: int*, *control_2: int*, *target: int*)
 
 *A 3-qubit quantum gate that takes in two control qubits and one target qubit.*
 
 ### Parameters:
 
 `control_1 (int)` - first control qubit.
 
@@ -737,37 +891,37 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
 qc.toffoli(0,1,2)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j]
 # [0. +0.j]
 # [0.5+0.j]
 # [0. +0.j]
 # [0.5+0.j]
 # [0. +0.j]
 # [0. +0.j]
 # [0.5+0.j]]
 ```
 
-> ## QuantumCircuit.`rccx`(*control_1*, *control_2*, *target*)
+> ## quantumcircuit.`rccx`(*control_1*, *control_2*, *target*)
 
 *A 3-qubit quantum gate that takes in two control qubits and one target qubit.*
 
 ### Parameters:
 
 `control_1 (int)` - first control qubit.
 
@@ -778,68 +932,68 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(3)
+from qcpy import quantumcircuit
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
 qc.rccx(0,1,2)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.5-0.j ]
 # [ 0. +0.j ]
 # [ 0.5-0.j ]
 # [ 0. +0.j ]
 # [ 0.5-0.j ]
 # [ 0. +0.j ]
 # [-0. +0.j ]
 # [ 0. +0.5j]]
 ```
 
-> ## QuantumCircuit.`rc3x`(*a*, *b*, *c*, *d*)
+> ## quantumcircuit.`rc3x`(*qubit_1: int*, *qubit_2: int*, *qubit_3: int*, *qubit_4: int*)
 
 *A 4-qubit quantum gate that takes in 4 unique qubits.*
 
 ### Parameters:
 
-`a (int)` - first input qubit.
+`qubit_1 (int)` - first input qubit.
 
-`b (int)` - second input qubit.
+`qubit_2 (int)` - second input qubit.
 
-`c (int)` - third input qubit.
+`qubit_3 (int)` - third input qubit.
 
-`d (int)` - fourth input qubit.
+`qubit_4 (int)` - fourth input qubit.
 
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(4)
+from qcpy import quantumcircuit
+qc = quantumcircuit(4)
 
-qc.hadamard(0)
+qc.h(0)
 
-qc.hadamard(1)
+qc.h(1)
 
-qc.hadamard(2)
+qc.h(2)
 
-qc.rc3x(0,1,2)
+qc.rc3x(0,1,2,3)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
@@ -850,15 +1004,15 @@
 # [ 0.354-0.j   ]
 # [ 0.   +0.j   ]
 # [ 0.   +0.354j]
 # [-0.   +0.j   ]
 # [ 0.   -0.j   ]
 # [-0.354+0.j   ]]
 ```
-> ## QuantumCircuit.`cnot`(*control*, *target*)
+> ## quantumcircuit.`cnot`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -867,30 +1021,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cnot(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`cr`(*control*, *target*)
+> ## quantumcircuit.`cr`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -899,31 +1053,31 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cr(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
 
-> ## QuantumCircuit.`cz`(*control*, *target*)
+> ## quantumcircuit.`cz`(*control: int*, *target: int*)
 
 *A 2-qubit quantum gate that takes in a control qubit and one target qubit.*
 
 ### Parameters:
 
 `control (int)` - control qubit.
 
@@ -932,30 +1086,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.cz(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`swap`(*qubit_1*, *qubit_2*)
+> ## quantumcircuit.`swap`(*qubit_1: int*, *qubit_2: int*)
 
 *A 2-qubit quantum gate that takes in 2 qubits to swap there properties.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit to swap.
 
@@ -964,30 +1118,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.swap(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`rxx`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rxx`(*qubit_1: int*, *qubit_2: int*, *theta: float=numpy.pi/2*)
 
 *A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit input.
 
@@ -997,30 +1151,30 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rxx(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j ]
 # [0. -0.5j]
 # [0.5+0.j ]
 # [0. -0.5j]]
 ```
 
-> ## QuantumCircuit.`rzz`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rzz`(*qubit_1*, *qubit_2*, *theta=numpy.pi/2*)
 
 *A 2-qubit quantum gate that takes in two qubits and a representation of theta to initialize in the quantum state.*
 
 ### Parameters:
 
 `qubit_1 (int)` - first qubit input.
 
@@ -1031,211 +1185,209 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-qc = QuantumCircuit(2)
+from qcpy import quantumcircuit
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rxx(0,1)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.j ]
 # [0. -0.5j]
 # [0.5+0.j ]
 # [0. -0.5j]]
 ```
 
-> ## QuantumCircuit.`customControlPhase`(*control*, *target*, *custom_matrix*)
+> ## quantumcircuit.`customcontrolled`(*control: int*, *target: int*, *custom_matrix: np.array*)
 
 *Used to insert single qubit based quantum gates to have a control qubit apart of it and committing to the quantum state.*
 
 ### Parameters:
 
 `control (int)` - control qubit for given matrix.
 
 `target (int)` - target qubit for given matrix.
 
-`custom_matrix (np.array)` -  matrix to be applied to the quantum circuit.
+`custom_matrix (np.array)` - (2,2) matrix to be applied to the quantum circuit.
 
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit, paulix
 
-from QCpy.QuantumGate import PauliX
+qc = quantumcircuit(2)
 
-qc = QuantumCircuit(2)
+qc.h(0)
 
-qc.hadamard(0)
+qc.customcontrolled(0,1, paulix())
 
-qc.customControlPhase(0,1, PauliX().matrix)
-
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.   +0.j]
 # [0.707+0.j]]
 ```
 
-> ## QuantumCircuit.`identity`(*qubit*)
+> ## quantumcircuit.`i`(*qubit: int*)
 
 *Used to confirm value that a qubit is representing and does nothing to manipulate the value of such qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the identity gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.identity(0)
+qc.i(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[1.+0.j]
 # [0.+0.j]
 # [0.+0.j]
 # [0.+0.j]]
 ```
 
-> ## QuantumCircuit.`x`(*qubit*)
+> ## quantumcircuit.`x`(*qubit: int*)
 
 *Used to invert the value of what a qubit is representing.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-X gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.x(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [1.+0.j]
 # [0.+0.j]]
 ```
 
 
-> ## QuantumCircuit.`hadmard`(*qubit*)
+> ## quantumcircuit.`hadmard`(*qubit: int*)
 
 *Used to put a given qubit into superposition.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Hadamard gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`y`(*qubit*)
+> ## quantumcircuit.`y`(*qubit: int*)
 
 *Changes the state of a qubit by pi around the y-axis of a Bloch Sphere.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Y gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.y(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [0.+1.j]
 # [0.+0.j]]
 ```
 
 
-> ## QuantumCircuit.`z`(*qubit*)
+> ## quantumcircuit.`z`(*qubit: int*)
 
 *Changes the state of a qubit by pi around the z-axis of a Bloch Sphere.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Z gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.z(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[ 0.707+0.j]
 # [ 0.   +0.j]
 # [-0.707+0.j]
 # [ 0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`phase`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`phase`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *Commits to a rotation around the z-axis based off of the inputted theta value.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Phase gate be applied to the quantum wire.
 
@@ -1243,151 +1395,151 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.phase(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   +0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`s`(*qubit*)
+> ## quantumcircuit.`s`(*qubit: int*)
 
 *Is a Phase gate where the inputted theta value is given as a constant of theta = pi / 2.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Pauli-Z gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.s(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   +0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`sdg`(*qubit*)
+> ## quantumcircuit.`sdg`(*qubit: int*)
 
 *Is a Phase gate and inverse of the S gate where the inputted theta value is given as a constant of theta = -pi / 2.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Sdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.sdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   -0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`t`(*qubit*)
+> ## quantumcircuit.`t`(*qubit: int*)
 
 *T gate is a special use case gate that in implemented from the P Gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the T gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.t(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j ]
 # [0.   +0.j ]
 # [0.5  +0.5j]
 # [0.   +0.j ]]
 ```
 
-> ## QuantumCircuit.`tdg`(*qubit*)
+> ## quantumcircuit.`tdg`(*qubit: int*)
 
 *Tdg gate is a special use case gate that in implemented from the P Gate and is the inverse of the T gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Tdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.tdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j ]
 # [0.   +0.j ]
 # [0.5  -0.5j]
 # [0.   +0.j ]]
 ```
 
-> ## QuantumCircuit.`rz`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rz`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RZ gate commits a rotation around the z-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Rz gate be applied to the quantum wire.
 
@@ -1395,31 +1547,31 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.hadamard(0)
+qc.h(0)
 
 qc.rz(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`ry`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`ry`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RY gate commits a rotation around the y-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Ry gate be applied to the quantum wire.
 
@@ -1427,29 +1579,29 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.ry(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j]
 # [0.   +0.j]
 # [0.707+0.j]
 # [0.   +0.j]]
 ```
 
-> ## QuantumCircuit.`rx`(*qubit*, *theta=numpy.pi/2*)
+> ## quantumcircuit.`rx`(*qubit: int*, *theta: float=numpy.pi/2*)
 
 *RX gate commits a rotation around the x-axis for a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Ry gate be applied to the quantum wire.
 
@@ -1457,85 +1609,85 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumCircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.rx(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.707+0.j   ]
 # [0.   +0.j   ]
 # [0.   -0.707j]
 # [0.   +0.j   ]]
 ```
 
-> ## QuantumCircuit.`sx`(*qubit*)
+> ## quantumcircuit.`sx`(*qubit: int*)
 
 *SX gate is the square root of the Inverse gate (X, PauliX Gate).*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the Sx gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.sx(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5+0.5j]
 # [0. +0.j ]
 # [0.5-0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`sxdg`(*qubit*)
+> ## quantumcircuit.`sxdg`(*qubit: int*)
 
 *SXDG gate is the negative square root of the Inverse gate (X, PauliX Gate) and inverse of the SX gate.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the SXdg gate be applied to the quantum wire.
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.sxdg(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`u`(*qubit*, *theta=numpy.pi/2*, *phi=numpy.pi/2*, *lmbda=numpy.pi/2*)
+> ## quantumcircuit.`u`(*qubit: int*, *theta: float=numpy.pi/2*, *phi: float=numpy.pi/2*, *lmbda: float=numpy.pi/2*)
 
 *U gate is given three inputs (theta, phi, and lambda) that allow the inputs to manipulate the base matrix to allow for the position of the enacted qubit around the bloch sphere representation.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the U gate be applied to the quantum wire.
 
@@ -1547,29 +1699,29 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
 qc.u(0)
 
-print(qc.state())
+print(qc.state)
 
 # [[0.5-0.5j]
 # [0. +0.j ]
 # [0.5+0.5j]
 # [0. +0.j ]]
 ```
 
-> ## QuantumCircuit.`custom`(*qubit*, *custom_matrix*)
+> ## quantumcircuit.`custom`(*qubit: int*, *custom_matrix: np.array*)
 
 *Will take in a custom single qubit quantum gate and implement it on a qubit.*
 
 ### Parameters:
 
 `qubit (int)` - the qubit to have the U gate be applied to the quantum wire.
 
@@ -1577,47 +1729,45 @@
 
 ### Returns:
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-
-from QCpy.QuantumGate import PauliX
+from qcpy import quantumcircuit, paulix
 
-qc = QuantumCircuit(2)
+qc = quantumcircuit(2)
 
-qc.custom(0, PauliX().matrix)
+qc.custom(0, paulix())
 
-print(qc.state())
+print(qc.state)
 
 # [[0.+0.j]
 # [0.+0.j]
 # [1.+0.j]
 # [0.+0.j]]
 ```
 
 # Visualizer
 
 *A collection of classes to visualize the quantum circuit*
 
-> ## *class* QCpy.Visualizer.QSphere(*circuit*)
+> ## *class* qcpy.qsphere(*circuit*)
 
 *Visualizes the quantum circuit as a q-sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## QSphere.`makeSphere`(*path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## qsphere.`make`(*path: str="qsphere.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a Q-Sphere that plots a global visualization of the quantum states in a 3D global view*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1630,40 +1780,39 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, qsphere
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-sphere_ex = QSphere(qc)
-sphere_ex.makeSphere(save=False, show=True)
+sphere_ex = qsphere(qc)
+sphere_ex.make(save=False, show=True)
 ```
 
-> ## *class* QC.Visualizer.BlochSphere(*circuit*)
+> ## *class* qcpy.bloch(*circuit*)
 
 *Visualizes the quantum state of a single qubit as a sphere*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## BlochSphere.`makeSphere`(*show_bit=0*, *path="qsphere.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## blochsphere.`make`(*show_bit: int=0*, *path: str="qsphere.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a Bloch Sphere that plots the quantum state of a single qubit in a 3D global view*
 
 ### Parameters:
 
 `show_bit (int)` - the qubit on the circuit to be visualized, initialized as the 0th bit
 
@@ -1678,40 +1827,39 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, bloch
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-sphere_ex = BlochSphere(qc)
-sphere_ex.makeSphere(show_bit=1, save=False, show=True)
+sphere_ex = bloch(qc)
+sphere_ex.make(show_bit=1, save=False, show=True)
 ```
 
-> ## *class* QCpy.Visualizer.StateVector(*circuit*)
+> ## *class* qcpy.statevector(*circuit*)
 
 *Visualizes the quantum circuit's quantum amplitutes using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## StateVector.`makeGraph`(*path="statevector.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## statevector.`make`(*path: str="statevector.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a graph that plots all the amplitudes of the qubits being measured*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1724,40 +1872,38 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, statevector
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-stateVector_ex = StateVector(qc)
-stateVector_ex.makeGraph(save=False, show=True)
+statevector(qc).make(save=False, show=True)
 ```
 
-> ## *class* QCpy.Visualizer.Probabilities(*circuit*)
+> ## *class* qcpy.probability(*circuit*)
 
 *Visualizes the quantum circuit's qubits probability of being measured using a bar graph*
 
 ### Parameters:
 
 `circuit` - the quantum circuit
 
 ### Attributes:
 
 `None`
 
-> ## Probabilities.`makeGraph`(*path="probabilities.png"*, *save=True*, *show=True*, *darkmode=True*)
+> ## probability.`make`(*path: str="probability.png"*, *save: bool=True*, *show: bool=True*, *darkmode: bool=True*)
 
 *Returns a graph that plots all the probabilities of the qubits being measured*
 
 ### Parameters:
 
 `path (str)` - name of the image to be saved
 
@@ -1770,19 +1916,17 @@
 ### Returns:
 
 `None`
 
 ### Example:
 
 ```python
-from QCpy import QuantumCircuit
-from QCpy.Visualizer import *
+from qcpy import quantumcircuit, probability
 
-qc = QuantumCircuit(3)
+qc = quantumcircuit(3)
 
-qc.hadamard(0)
-qc.hadamard(1)
-qc.hadamard(2)
+qc.h(0)
+qc.h(1)
+qc.h(2)
 
-probabilities_ex = Probabilities(qc)
-probabilities_ex.makeGraph(save=False, show=True)
-```
+probability(qc).make(save=False, show=True)
+```
```

### Comparing `QCpython-1.0.3/setup.py` & `qcpython-1.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="QCpython",
-    version="1.0.3",
+    name="qcpython",
+    version="1.1.0",
     author='Brennan Freeze, Paris Osuch, Aundre Barras, Soren Richenberg, Suzanne Rivoire',
     author_email='freezebrennan@gmail.com, osuch@sonoma.edu, barras@sonoma.edu, richenbe@sonoma.edu, rivoire@sonoma.edu',
-    description="QCpy is a comprehensive and user-friendly library for quantum computing, providing a wide range of functionality for quantum algorithms and quantum circuits. It is built on using open-source libraries NumPy and Matplotlib; compatible with Python 3.",
+    description="QCpy is an open source python library and collaborative project for flexible simulations and visualizations of quantum circuits. Designed by college students with students in mind, this library contains a powerful set of tools to teach computer scientists about the emerging discipline of quantum computing.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/QCpython/QCpy",
     packages=setuptools.find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
     install_requires=[
-        "numpy>=1.22.0",
-        "matplotlib>=3.5.1",
-        "six>=1.16.0",
-        "pyparsing>=3.0.4",
-        "pytest>=6.2.4"
+        "matplotlib==3.7.2",
+        "numpy==1.25.1",
+        "setuptools==65.5.0",
     ],
 )
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_01.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_01.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    return qc.state()
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    return qc.flatten()
 
 
 def test_01a():
     assert (
-        inc(1) == np.array([1 + 0j, 0 + 0j], 'F').reshape(2, 1)
+        inc(1) == np.array([1 + 0j, 0 + 0j], 'F')
     ).all(), "test_01a Failed on QuantumCircuit"
 
 
 def test_01b():
     assert (
-        inc(2) == np.array([1 + 0j, 0 + 0j, 0 + 0j, 0 + 0j], 'F').reshape(4, 1)
+        inc(2) == np.array([1 + 0j, 0 + 0j, 0 + 0j, 0 + 0j], 'F')
     ).all(), "test_01b Failed on QuantumCircuit"
 
 
 def test_01c():
     assert (
         inc(3) == np.array([
             1 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ]).reshape(8, 1)
+        ])
     ).all(), "test_01c Failed on QuantumCircuit"
 
 
 def test_01d():
     assert (
         inc(4) == np.array([
             1 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_01d Failed on QuantumCircuit"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_02.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_02.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
     for i in range(x):
-        qc.hadamard(i)
-    return qc.state()
+        qc.h(i)
+    return qc.flatten()
 
 
 def test_02a():
     assert (
-        inc(1) == np.array([0.707 + 0j, 0.707 + 0j], 'F').reshape(2, 1)
+        inc(1) == np.array([0.707 + 0j, 0.707 + 0j], 'F')
     ).all(), "test_02a Failed on hadamard"
 
 
 def test_02b():
     assert (
         inc(2) == np.array([
             0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0.5 + 0j
-        ], 'F').reshape(4, 1)
+        ], 'F')
     ).all(), "test_02b Failed on hadamard"
 
 
 def test_02c():
     assert (
         inc(3) == np.array([
             0.354 + 0j, 0.354 + 0j, 0.354 + 0j, 0.354 + 0j,
             0.354 + 0j, 0.354 + 0j, 0.354 + 0j, 0.354 + 0j
-        ], 'F').reshape(8, 1)
+        ], 'F')
     ).all(), "test_02c Failed on hadamard"
 
 
 def test_02d():
     assert (
         inc(4) == np.array([
             0.25 + 0j, 0.25 + 0j, 0.25 + 0j, 0.25 + 0j,
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_03.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_03.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
     for i in range(x):
-        qc.hadamard(i)
+        qc.h(i)
     for i in range(x):
         qc.t(i)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_03a():
     assert (
-        inc(1) == np.array([0.707 + 0j, 0.5 + 0.5j], 'F').reshape(2, 1)
+        inc(1) == np.array([0.707 + 0j, 0.5 + 0.5j], 'F')
     ).all(), \
         "test_03a Failed on hadamard and t"
 
 
 def test_03b():
     assert (
         inc(2) == np.array([
             0.5 + 0j, 0.354 + 0.354j, 0.354 + 0.354j, 0 + 0.5j
-        ], 'F').reshape(4, 1)
+        ], 'F')
     ).all(), \
         "test_03b Failed on hadamard and t"
 
 
 def test_03c():
     assert (
         inc(3) == np.array([
             0.354 + 0j, 0.25 + 0.25j, 0.25 + 0.25j, 0 + 0.354j,
             0.25 + 0.25j, 0 + 0.354j, 0 + 0.354j, -0.25 + 0.25j
-        ], 'F').reshape(8, 1)
+        ], 'F')
     ).all(), \
         "test_03c Failed on hadamard and t"
 
 
 def test_03d():
     assert (
         inc(4) == np.array([
             0.25 + 0j, 0.177 + 0.177j, 0.177 + 0.177j, 0 + 0.25j,
             0.177 + 0.177j, 0 + 0.25j, 0 + 0.25j, -0.177 + 0.177j,
             0.177 + 0.177j, 0 + 0.25j, 0 + 0.25j, -0.177 + 0.177j,
             0 + 0.25j, -0.177 + 0.177j, -0.177 + 0.177j, -0.25 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), \
         "test_03d Failed on hadamard and t"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_04.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_20.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-from QCpy import QuantumCircuit
-import numpy as np
-
-
-def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
-    qc.cnot(0, x - 1)
-    return qc.state()
-
-
-def test_04a():
-    assert (
-        inc(2) == np.array([
-            0.707 + 0j, 0 + 0j, 0 + 0j, 0.707 + 0j
-        ], 'F').reshape(4, 1)
-    ).all(), "test_04a Failed on hadamard and cnot"
-
-
-def test_04b():
-    assert (
-        inc(3) == np.array([
-            0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0.707 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(8, 1)
-    ).all(), "test_04b Failed on hadamard and cnot"
-
-
-def test_04c():
-    assert (
-        inc(4) == np.array([
-            0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
-    ).all(), "test_04c Failed on hadamard and cnot"
+from qcpy import quantumcircuit
+import numpy as np
+
+
+def inc(x):
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(x - 1)
+    qc.rzz(x - 1, 0)
+    qc.h(x - 1)
+    return qc.flatten()
+
+
+def test_20a():
+    assert (
+        inc(2) == np.array([
+            0.707 + 0j, 0 + 0j, 0 - 0.707j, 0 + 0j
+        ], 'F')
+    ).all(), "test_20a Failed on hadamard -> rzz -> hadamard"
+
+
+def test_20b():
+    assert (
+        inc(3) == np.array([
+            0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 - 0.707j, 0 + 0j, 0 + 0j, 0 + 0j
+        ], 'F')
+    ).all(), "test_20b Failed on hadamard -> rzz -> hadamard"
+
+
+def test_20c():
+    assert (
+        inc(4) == np.array([
+            0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 - 0.707j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
+        ], 'F')
+    ).all(), "test_20c Failed on hadamard -> rzz -> hadamard"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_05.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_05.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(x - 1)
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(x - 1)
     qc.cnot(x - 1, 0)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_05a():
     assert (
         inc(2) == np.array([
             0.707 + 0j, 0 + 0j, 0 + 0j, 0.707 + 0j
-        ], 'F').reshape(4, 1)
+        ], 'F')
     ).all(), "test_05a Failed on hadamard and cnot"
 
 
 def test_05b():
     assert (
         inc(3) == np.array([
             0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0.707 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(8, 1)
+        ], 'F')
     ).all(), "test_05b Failed on hadamard and cnot"
 
 
 def test_05c():
     assert (
         inc(4) == np.array([
             0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_05c Failed on hadamard and cnot"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_06.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_07.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
-    qc.cnot(0, x - 1)
-    qc.hadamard(0)
-    return qc.state()
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(x - 1)
+    qc.cnot(x - 1, 0)
+    qc.h(x - 1)
+    return qc.flatten()
 
 
-def test_06a():
+def test_07a():
     assert (
         inc(2) == np.array([
             0.5 + 0j, 0.5 + 0j, 0.5 + 0j, -0.5 + 0j
-        ], 'F').reshape(4, 1)
-    ).all(), "test_06a Failed on hadamard -> cnot -> hadamard"
+        ], 'F')
+    ).all(), "test_07a Failed on hadamard -> cnot -> hadamard"
 
 
-def test_06b():
+def test_07b():
     assert (
         inc(3) == np.array([
             0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
             0.5 + 0j, -0.5 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(8, 1)
-    ).all(), "test_06b Failed on hadamard -> cnot -> hadamard"
+        ], 'F')
+    ).all(), "test_07b Failed on hadamard -> cnot -> hadamard"
 
 
-def test_06c():
+def test_07c():
     assert (
         inc(4) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, -0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
-    ).all(), "test_06c Failed on hadamard -> cnot -> hadamard"
+            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, -0.5 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
+        ], 'F')
+    ).all(), "test_07c Failed on hadamard -> cnot -> hadamard"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_07.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_14.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,45 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(x - 1)
-    qc.cnot(x - 1, 0)
-    qc.hadamard(x - 1)
-    return qc.state()
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(0)
+    qc.h(1)
+    qc.rccx(0, 1, x - 1)
+    return qc.flatten()
 
 
-def test_07a():
+def test_11a():
     assert (
-        inc(2) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0.5 + 0j, -0.5 + 0j
-        ], 'F').reshape(4, 1)
-    ).all(), "test_07a Failed on hadamard -> cnot -> hadamard"
+        inc(3) == np.array([
+            0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0.5j
+        ], 'F')
+    ).all(), "test_11a Failed on hadamard -> hadamard -> rccx"
 
 
-def test_07b():
+def test_11b():
     assert (
-        inc(3) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, -0.5 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(8, 1)
-    ).all(), "test_07b Failed on hadamard -> cnot -> hadamard"
+        inc(4) == np.array([
+            0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0.5j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
+        ], 'F')
+    ).all(), "test_11b Failed on hadamard -> hadamard -> rccx"
 
 
-def test_07c():
+def test_11c():
     assert (
-        inc(4) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
+        inc(5) == np.array([
+            0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0.5j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, -0.5 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
-    ).all(), "test_07c Failed on hadamard -> cnot -> hadamard"
+        ], 'F')
+    ).all(), "test_11c Failed on hadamard -> hadamard -> rccx"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_08.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_08.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
-    qc.hadamard(1)
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(0)
+    qc.h(1)
     qc.toffoli(0, 1, x - 1)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_08a():
     assert (
         inc(3) == np.array([
             0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0.5 + 0j
-        ], 'F').reshape(8, 1)
+        ], 'F')
     ).all(), "test_08a Failed on hadamard -> hadamard -> toffoli"
 
 
 def test_08b():
     assert (
         inc(4) == np.array([
             0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0.5 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_08b Failed on hadamard -> hadamard -> toffoli"
 
 
 def test_08c():
     assert (
         inc(5) == np.array([
             0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0.5 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(32, 1)
+        ], 'F')
     ).all(), "test_08c Failed on hadamard -> hadamard -> toffoli"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_09.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_11.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(x - 1)
-    qc.hadamard(x - 2)
-    qc.toffoli(x - 1, x - 2, 0)
-    return qc.state()
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(x - 1)
+    qc.h(0)
+    qc.toffoli(x - 1, 0, x - 2)
+    return qc.flatten()
 
 
-def test_09a():
+def test_11a():
     assert (
         inc(3) == np.array([
-            0.5 + 0j, 0 + 0j, 0.5 + 0j, 0 + 0j,
+            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
             0.5 + 0j, 0 + 0j, 0 + 0j, 0.5 + 0j
-        ], 'F').reshape(8, 1)
-    ).all(), "test_09a Failed on hadamard -> hadamard -> toffoli"
+        ], 'F')
+    ).all(), "test_11a Failed on hadamard -> hadamard -> toffoli"
 
 
-def test_09b():
+def test_11b():
     assert (
         inc(4) == np.array([
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
-    ).all(), "test_09b Failed on hadamard -> hadamard -> toffoli"
+        ], 'F')
+    ).all(), "test_11b Failed on hadamard -> hadamard -> toffoli"
 
 
-def test_09c():
+def test_11c():
     assert (
         inc(5) == np.array([
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(32, 1)
-    ).all(), "test_09c Failed on hadamard -> hadamard -> toffoli"
+        ], 'F')
+    ).all(), "test_11c Failed on hadamard -> hadamard -> toffoli"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_10.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_10.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
     for i in range(x):
-        qc.hadamard(i)
+        qc.h(i)
     for i in range(x):
         qc.tdg(i)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_10a():
     assert (
-        inc(1) == np.array([0.707 + 0j, 0.5 - 0.5j], 'F').reshape(2, 1)
+        inc(1) == np.array([0.707 + 0j, 0.5 - 0.5j], 'F')
     ).all(), "test_10a Failed on hadamard -> tdg"
 
 
 def test_10b():
     assert (
         inc(2) == np.array([
             0.5 + 0j, 0.354 - 0.354j, 0.354 - 0.354j, 0 - 0.5j
-        ], 'F').reshape(4, 1)
+        ], 'F')
     ).all(), "test_10b Failed on hadamard -> tdg"
 
 
 def test_10c():
     assert (
         inc(3) == np.array([
             0.354 + 0j, 0.25 - 0.25j, 0.25 - 0.25j, 0 - 0.354j,
             0.25 - 0.25j, 0 - 0.354j, 0 - 0.354j, -0.25 - 0.25j
-        ], 'F').reshape(8, 1)
+        ], 'F')
     ).all(), "test_10c Failed on hadamard -> tdg"
 
 
 def test_10d():
     assert (
         inc(4) == np.array([
             0.25 + 0j, 0.177 - 0.177j, 0.177 - 0.177j, 0 - 0.25j,
             0.177 - 0.177j, 0 - 0.25j, 0 - 0.25j, -0.177 - 0.177j,
             0.177 - 0.177j, 0 - 0.25j, 0 - 0.25j, -0.177 - 0.177j,
             0 - 0.25j, -0.177 - 0.177j, -0.177 - 0.177j, -0.25 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_10d Failed on hadamard -> tdg"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_11.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_09.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(x - 1)
-    qc.hadamard(0)
-    qc.toffoli(x - 1, 0, x - 2)
-    return qc.state()
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(x - 1)
+    qc.h(x - 2)
+    qc.toffoli(x - 1, x - 2, 0)
+    return qc.flatten()
 
 
-def test_11a():
+def test_09a():
     assert (
         inc(3) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0.5 + 0j, 0 + 0j,
             0.5 + 0j, 0 + 0j, 0 + 0j, 0.5 + 0j
-        ], 'F').reshape(8, 1)
-    ).all(), "test_11a Failed on hadamard -> hadamard -> toffoli"
+        ], 'F')
+    ).all(), "test_09a Failed on hadamard -> hadamard -> toffoli"
 
 
-def test_11b():
+def test_09b():
     assert (
         inc(4) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
-    ).all(), "test_11b Failed on hadamard -> hadamard -> toffoli"
+        ], 'F')
+    ).all(), "test_09b Failed on hadamard -> hadamard -> toffoli"
 
 
-def test_11c():
+def test_09c():
     assert (
         inc(5) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(32, 1)
-    ).all(), "test_11c Failed on hadamard -> hadamard -> toffoli"
+        ], 'F')
+    ).all(), "test_09c Failed on hadamard -> hadamard -> toffoli"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_12.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_12.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(0)
     qc.swap(0, x - 1)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_12a():
     assert (
         inc(2) == np.array([
             0.707 + 0j, 0 + 0j, 0.707 + 0j, 0 + 0j
-        ], 'F').reshape(4, 1)
+        ], 'F')
     ).all(), "test_12a Failed on hadamard -> swap"
 
 
 def test_12b():
     assert (
         inc(3) == np.array([
             0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(8, 1)
+        ], 'F')
     ).all(), "test_12b Failed on hadamard -> swap"
 
 
 def test_12c():
     assert (
         inc(4) == np.array([
             0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.707 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_12c Failed on hadamard -> swap"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_13.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_13.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(0)
     qc.swap(0, x - 1)
     qc.swap(x - 1, 0)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_13a():
     assert (
         inc(2) == np.array([
             0.707 + 0j, 0.707 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(4, 1)
+        ], 'F')
     ).all(), "test_13a Failed on hadamard -> swap -> swap"
 
 
 def test_13b():
     assert (
         inc(3) == np.array([
             0.707 + 0j, 0.707 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(8, 1)
+        ], 'F')
     ).all(), "test_13b Failed on hadamard -> swap -> swap"
 
 
 def test_13c():
     assert (
         inc(4) == np.array([
             0.707 + 0j, 0.707 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_13c Failed on hadamard -> swap -> swap"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_14.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_15.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
-    qc.hadamard(1)
-    qc.rccx(0, 1, x - 1)
-    return qc.state()
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(x - 2)
+    qc.h(x - 1)
+    qc.rccx(x - 1, x - 2, 0)
+    return qc.flatten()
 
 
-def test_11a():
+def test_15a():
     assert (
         inc(3) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0.5j
-        ], 'F').reshape(8, 1)
-    ).all(), "test_11a Failed on hadamard -> hadamard -> rccx"
+            0.5 + 0j, 0 + 0j, 0.5 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0.5j
+        ], 'F')
+    ).all(), "test_15a Failed hadamard -> hadamard -> rccx"
 
 
-def test_11b():
+def test_15b():
     assert (
         inc(4) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0.5j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
-    ).all(), "test_11b Failed on hadamard -> hadamard -> rccx"
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0.5j, 0 + 0j, 0 + 0j
+        ], 'F')
+    ).all(), "test_15b Failed hadamard -> hadamard -> rccx"
 
 
-def test_11c():
+def test_15c():
     assert (
         inc(5) == np.array([
-            0.5 + 0j, 0.5 + 0j, 0.5 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0.5j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0 + 0j, 0 + 0.5j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(32, 1)
-    ).all(), "test_11c Failed on hadamard -> hadamard -> rccx"
+        ], 'F')
+    ).all(), "test_15c Failed hadamard -> hadamard -> rccx"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_15.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_06.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,36 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(x - 2)
-    qc.hadamard(x - 1)
-    qc.rccx(x - 1, x - 2, 0)
-    return qc.state()
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(0)
+    qc.cnot(0, x - 1)
+    qc.h(0)
+    return qc.flatten()
 
 
-def test_15a():
+def test_06a():
     assert (
-        inc(3) == np.array([
-            0.5 + 0j, 0 + 0j, 0.5 + 0j, 0 + 0j,
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0.5j
-        ], 'F').reshape(8, 1)
-    ).all(), "test_15a Failed hadamard -> hadamard -> rccx"
+        inc(2) == np.array([
+            0.5 + 0j, 0.5 + 0j, 0.5 + 0j, -0.5 + 0j
+        ], 'F')
+    ).all(), "test_06a Failed on hadamard -> cnot -> hadamard"
 
 
-def test_15b():
+def test_06b():
     assert (
-        inc(4) == np.array([
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0.5j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
-    ).all(), "test_15b Failed hadamard -> hadamard -> rccx"
+        inc(3) == np.array([
+            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, -0.5 + 0j, 0 + 0j, 0 + 0j
+        ], 'F')
+    ).all(), "test_06b Failed on hadamard -> cnot -> hadamard"
 
 
-def test_15c():
+def test_06c():
     assert (
-        inc(5) == np.array([
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0.5j, 0 + 0j, 0 + 0j,
-            0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(32, 1)
-    ).all(), "test_15c Failed hadamard -> hadamard -> rccx"
+        inc(4) == np.array([
+            0.5 + 0j, 0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
+            0.5 + 0j, -0.5 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
+        ], 'F')
+    ).all(), "test_06c Failed on hadamard -> cnot -> hadamard"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_16.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_16.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
-    qc.hadamard(1)
-    qc.hadamard(2)
-    qc.hadamard(3)
-    qc.hadamard(4)
-    qc.hadamard(5)
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(0)
+    qc.h(1)
+    qc.h(2)
+    qc.h(3)
+    qc.h(4)
+    qc.h(5)
     qc.rxx(0, 1)
     qc.rxx(2, 3)
     qc.rxx(4, 5)
     qc.rx(5)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_16a():
     assert (
         inc(6) == np.array([
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j,
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j,
@@ -32,9 +32,9 @@
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j,
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j,
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j,
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j,
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j,
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j,
             -0.125 + 0j, -0.125 + 0j, -0.125 + 0j, -0.125 + 0j
-        ], 'F').reshape(64, 1)
+        ], 'F')
     ).all(), "test_16a Failed on hadamard (x6) -> rxx (x3) -> rx"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_17.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_17.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
-    qc.hadamard(1)
-    qc.hadamard(2)
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(0)
+    qc.h(1)
+    qc.h(2)
     qc.rc3x(0, 1, 2, x - 1)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_17a():
     assert (
         inc(4) == np.array([
             0.354 + 0j, 0.354 + 0j, 0.354 + 0j, 0 + 0.354j,
             0.354 + 0j, 0.354 + 0j, 0.354 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, -0.354 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_17a Failed on hadamard (x3) -> rc3x"
 
 
 def test_17b():
     assert (
         inc(5) == np.array([
             0.354 + 0j, 0.354 + 0j, 0.354 + 0j, 0 + 0.354j,
             0.354 + 0j, 0.354 + 0j, 0.354 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, -0.354 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(32, 1)
+        ], 'F')
     ).all(), "test_17b Failed on hadamard (x3) -> rc3x"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_18.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_18.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(x - 1)
-    qc.hadamard(x - 2)
-    qc.hadamard(x - 3)
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(x - 1)
+    qc.h(x - 2)
+    qc.h(x - 3)
     qc.rc3x(x - 1, x - 2, x - 3, 0)
-    return qc.state()
+    return qc.flatten()
 
 
 def test_18a():
     assert (
         inc(4) == np.array([
             0.354 + 0j, 0 + 0j, 0.354 + 0j, 0 + 0j,
             0.354 + 0j, 0 + 0j, 0.354 + 0j, 0 + 0j,
             0.354 + 0j, 0 + 0j, 0.354 + 0j, 0 + 0j,
             0 + 0.354j, 0 + 0j, 0 + 0j, -0.354 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_18a Failed hadamard (x3) -> rc3x"
 
 
 def test_18b():
     assert (
         inc(5) == np.array([
             0.354 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.354 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.354 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.354 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.354 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0.354 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0.354j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, -0.354 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(32, 1)
+        ], 'F')
     ).all(), "test_18b Failed hadamard (x3) -> rc3x"
```

### Comparing `QCpython-1.0.3/test/quantumcircuit/test_qc_19.py` & `qcpython-1.1.0/test/quantumcircuit/test_qc_19.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from QCpy import QuantumCircuit
+from qcpy import quantumcircuit
 import numpy as np
 
 
 def inc(x):
-    qc = QuantumCircuit(qubits=x, little_endian=True, prep='z')
-    qc.hadamard(0)
+    qc = quantumcircuit(qubits=x, little_endian=True, prep='z')
+    qc.h(0)
     qc.rzz(0, x - 1)
-    qc.hadamard(0)
-    return qc.state()
+    qc.h(0)
+    return qc.flatten()
 
 
 def test_19a():
     assert (
         inc(2) == np.array([
             0.707 + 0j, 0 - 0.707j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(4, 1)
+        ], 'F')
     ).all(), "test_19a Failed on hadamard -> rzz -> hadamard"
 
 
 def test_19b():
     assert (
         inc(3) == np.array([
             0.707 + 0j, 0 - 0.707j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(8, 1)
+        ], 'F')
     ).all(), "test_19b Failed on hadamard -> rzz -> hadamard"
 
 
 def test_19c():
     assert (
         inc(4) == np.array([
             0.707 + 0j, 0 - 0.707j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j,
             0 + 0j, 0 + 0j, 0 + 0j, 0 + 0j
-        ], 'F').reshape(16, 1)
+        ], 'F')
     ).all(), "test_19c Failed on hadamard -> rzz -> hadamard"
```

### Comparing `QCpython-1.0.3/test/quantumgate/test_qg_06.py` & `qcpython-1.1.0/test/quantumgate/test_qg_06.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from QCpy.QuantumGate import CNot
+from qcpy.quantumgate import cnot
 import numpy as np
 
 
 def test_qg_06a():
     assert (
-        CNot(inverse=False).matrix == np.array([
+        cnot() == np.array([
             [1 + 0j, 0 + 0j, 0 + 0j, 0 + 0j],
+            [0 + 0j, 1 + 0j, 0 + 0j, 0 + 0j],
             [0 + 0j, 0 + 0j, 0 + 0j, 1 + 0j],
-            [0 + 0j, 0 + 0j, 1 + 0j, 0 + 0j],
-            [0 + 0j, 1 + 0j, 0 + 0j, 0 + 0j]
+            [0 + 0j, 0 + 0j, 1 + 0j, 0 + 0j]
         ], 'F')
-    ).all(), 'test_qg_06a Failed on CNot'
-
+    ).all(), 'test_qg_06b Failed on CNot'
 
 def test_qg_06b():
     assert (
-        CNot(inverse=True).matrix == np.array([
+        cnot(little_endian=True) == np.array([
             [1 + 0j, 0 + 0j, 0 + 0j, 0 + 0j],
-            [0 + 0j, 1 + 0j, 0 + 0j, 0 + 0j],
             [0 + 0j, 0 + 0j, 0 + 0j, 1 + 0j],
-            [0 + 0j, 0 + 0j, 1 + 0j, 0 + 0j]
+            [0 + 0j, 0 + 0j, 1 + 0j, 0 + 0j],
+            [0 + 0j, 1 + 0j, 0 + 0j, 0 + 0j]
         ], 'F')
-    ).all(), 'test_qg_06b Failed on CNot'
+    ).all(), 'test_qg_06a Failed on CNot'
+
+
+
```

### Comparing `QCpython-1.0.3/test/quantumgate/test_qg_19.py` & `qcpython-1.1.0/test/quantumgate/test_qg_19.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from QCpy.QuantumGate import U
+from qcpy.quantumgate import u
 import numpy as np
 
 
 def test_qg_19():
     assert (
-        U().matrix == np.array([
+        u() == np.array([
             [
                 np.cos((np.pi / 2) / 2),
                 -1 * np.exp(0 + 1j * (np.pi / 2)) * np.sin((np.pi / 2) / 2)
             ],
             [
                 np.exp(0 + 1j * (np.pi / 2))
                 * np.sin((np.pi / 2) / 2),
```

### Comparing `QCpython-1.0.3/test/quantumgate/test_qg_21.py` & `qcpython-1.1.0/test/quantumgate/test_qg_21.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from QCpy.QuantumGate import Rzz
+from qcpy.quantumgate import rzz
 import numpy as np
 
 
 def test_qg_21():
     assert (
-        Rzz().matrix == np.array([
+        rzz() == np.array([
             [
                 np.exp(0 - 1j * ((np.pi / 2) / 2)),
                 0 + 0j,
                 0 + 0j,
                 0 + 0j
             ],
             [
```

